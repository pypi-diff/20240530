# Comparing `tmp/llm_research-0.1.0.tar.gz` & `tmp/llm_research-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_research-0.1.0.tar", max compression
+gzip compressed data, was "llm_research-0.2.0.tar", max compression
```

## Comparing `llm_research-0.1.0.tar` & `llm_research-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0     1071 2024-01-23 12:56:41.115120 llm_research-0.1.0/LICENSE
--rw-r--r--   0        0        0      104 2024-01-26 15:32:20.933370 llm_research-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-01-23 13:32:10.835245 llm_research-0.1.0/llm_research/__init__.py
--rw-r--r--   0        0        0       70 2024-01-26 00:39:25.780099 llm_research-0.1.0/llm_research/model/__init__.py
--rw-r--r--   0        0        0     6758 2024-01-27 02:19:21.624170 llm_research-0.1.0/llm_research/model/base_model.py
--rw-r--r--   0        0        0     1036 2024-01-26 04:11:06.977838 llm_research-0.1.0/llm_research/model/models.py
--rw-r--r--   0        0        0     4848 2024-01-26 00:58:10.283982 llm_research-0.1.0/llm_research/model/prompt.py
--rw-r--r--   0        0        0     1014 2024-01-26 00:57:41.424533 llm_research-0.1.0/llm_research/model/utils.py
--rw-r--r--   0        0        0        0 2024-01-23 13:32:44.794796 llm_research-0.1.0/llm_research/process/__init__.py
--rw-r--r--   0        0        0       60 2024-01-23 12:47:14.525977 llm_research-0.1.0/llm_research/process/openai_finetune.py
--rw-r--r--   0        0        0      815 2024-01-26 15:14:55.799990 llm_research-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 llm_research-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-23 12:56:41.115120 llm_research-0.2.0/LICENSE
+-rw-r--r--   0        0        0      104 2024-01-26 15:32:20.933370 llm_research-0.2.0/README.md
+-rw-r--r--   0        0        0       82 2024-05-29 18:09:41.957273 llm_research-0.2.0/llm_research/__init__.py
+-rw-r--r--   0        0        0     6797 2024-05-29 17:11:44.563436 llm_research-0.2.0/llm_research/model/base_model.py
+-rw-r--r--   0        0        0     1037 2024-05-30 00:20:35.304327 llm_research-0.2.0/llm_research/model/models.py
+-rw-r--r--   0        0        0     5000 2024-05-29 17:41:54.890597 llm_research-0.2.0/llm_research/model/prompt.py
+-rw-r--r--   0        0        0     1242 2024-05-29 18:08:47.110230 llm_research-0.2.0/llm_research/model/utils.py
+-rw-r--r--   0        0        0     1715 2024-05-30 00:12:31.769711 llm_research-0.2.0/llm_research/utils.py
+-rw-r--r--   0        0        0      815 2024-05-30 02:35:05.527781 llm_research-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 llm_research-0.2.0/PKG-INFO
```

### Comparing `llm_research-0.1.0/LICENSE` & `llm_research-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_research-0.1.0/llm_research/model/base_model.py` & `llm_research-0.2.0/llm_research/model/base_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     RunnableSequence,
     RunnableSerializable
 )
 from langchain.globals import set_verbose
 from langchain.memory.buffer import ConversationBufferMemory
 import numpy as np
 import orjson
-import openai
 from operator import itemgetter
 from pathlib import Path
 import sys
 from shutil import rmtree
 from tqdm import trange
 import time
 from typing import Tuple, List, Dict, Optional
@@ -39,15 +38,15 @@
 
         log_dir = Path(f'log/{self.experiment_name}')
         log_dir.mkdir(parents=True, exist_ok=True)
         self.log_file_path = log_dir / f'{self.run_name}.log'
         logger.remove()
         logger.add(self.log_file_path, level = "INFO")
 
-        llm_response_dir = Path(f'data/model_results/{self.experiment_name}')
+        llm_response_dir = Path(f'data/request_results/{self.experiment_name}')
         llm_response_dir.mkdir(parents=True, exist_ok=True)
         self.llm_response_file_path = llm_response_dir / f'{self.run_name}.jsonl'
 
 
     @staticmethod
     def __add_memory(chain: RunnableSequence):
         memory = ConversationBufferMemory(return_messages=True)
@@ -66,15 +65,15 @@
                         ):
         retry = True
         while retry:
             try:
                 res = chain.invoke({'instructions': instructions})
 
                 bad = False
-                for key in self.prompt.response_keys:
+                for key in self.prompt.response_variables:
                     if res.get(key) is None:
                         bad = True
                         break
                 if not bad:
                     retry = False
                 else:
                     logger.info(f"formatting error(KeyError) for {i+1} th sample, re-generate")
@@ -115,35 +114,35 @@
 
     @property
     def __run_id(self):
         run_info = mlflow.search_runs(self.__experiment_id, filter_string=f"run_name='{self.run_name}'")
         return run_info['run_id'].values[0]
 
 
-    def __hook_process(self, query_file_path: str) -> Tuple[int, int, List]:
-        data = read_jsonl(query_file_path)
+    def __hook_process(self, request_file_path: str) -> Tuple[int, int, List]:
+        data = read_jsonl(request_file_path)
 
         if not self.llm_response_file_path.exists():
             _i = 0
-            n_query = len(data)
+            n_request = len(data)
         else:
             _i = len(read_jsonl(self.llm_response_file_path))
             if _i == len(data):
                 rmtree(f'mlruns/{self.__experiment_id}/{self.__run_id}')
                 self.log_file_path.unlink(missing_ok=True)
                 self.llm_response_file_path.unlink(missing_ok=True)
 
                 _i = 0
-                n_query = len(data)
+                n_request = len(data)
             else:
-                n_query = len(data) - _i
-                logger.info(f"restart the process form the {_i+1}th query")
+                n_request = len(data) - _i
+                logger.info(f"restart the process form the {_i+1}th request")
 
         mlflow.start_run(experiment_id=self.__experiment_id, run_name=self.run_name)
-        return _i, n_query, data
+        return _i, n_request, data
 
 
     def mlflow_logging(self, data: List[Dict]):
         mlflow.log_artifact(self.prompt.system_prompt_path)
         mlflow.log_artifact(self.prompt.human_prompt_path)
 
         res = read_jsonl(self.llm_response_file_path)
@@ -153,45 +152,45 @@
             +
             np.array([list(i.values()) for i in res]).transpose().tolist()
         )
         table_dict = {
             key: value
             for key, value in zip(keys, values)
         }
-        mlflow.log_table(table_dict, "query_response.json")
+        mlflow.log_table(table_dict, "request_response.json")
 
 
     def request_batch(self,
                       prompt: Prompt,
-                      query_file_path: str,
+                      request_file_path: str,
                       fewshot_examples_path: Optional[str] = None,
                       sleep: int = 3,
                      ) -> None:
         self.prompt = prompt
-        _i, n_query, data = self.__hook_process(query_file_path)
-        query_list = [i.get(prompt.query_key) for i in data]
+        _i, n_request, data = self.__hook_process(request_file_path)
+        request_list = [i.get(prompt.request_variable) for i in data]
 
         if fewshot_examples_path is not None:
             message_prompt = prompt.few_shot(fewshot_examples_path)
             mlflow.log_artifact(fewshot_examples_path)
         else:
             message_prompt = prompt.zero_shot()
 
-        logger.info('start the query process')
+        logger.info('start the request process')
         with self.llm_response_file_path.open('ab') as f:
-            for i in trange(n_query, position=0, leave=True):
+            for i in trange(n_request, position=0, leave=True):
                 chain = (
-                     message_prompt.partial(**{prompt.query_key: query_list[_i+i]})
+                     message_prompt.partial(**{prompt.request_variable: request_list[_i+i]})
                     | self.llm
                     | prompt.parser
                 )
                 res = self.request_instance("", chain, _i+i)
                 f.write(orjson.dumps(res , option=orjson.OPT_APPEND_NEWLINE))
                 time.sleep(sleep)
 
-        logger.info('finish the query process')
+        logger.info('finish the request process')
         self.mlflow_logging(data)
 
 
     @staticmethod
     def end_request():
         mlflow.end_run()
```

### Comparing `llm_research-0.1.0/llm_research/model/models.py` & `llm_research-0.2.0/llm_research/model/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             model = model,
             temperature = temperature,
             timeout = timeout,
             verbose = verbose
         )
 
 
+
 class VertexAILLM(BaseModel):
     def __init__(self,
                  *,
                  model: str = "gemini-pro",
                  verbose = False
                  ):
         super().__init__(verbose)
```

### Comparing `llm_research-0.1.0/llm_research/model/prompt.py` & `llm_research-0.2.0/llm_research/model/prompt.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,61 +17,70 @@
 class Prompt:
     def __init__(self,
                  pydantic_object: ModelMetaclass,
                  system_prompt_path: str,
                  human_prompt_path:str ,
                  **system_message_input_variables
                 ):
-        self.response_keys = list(pydantic_object.__fields__.keys())
+        self.response_variables = list(pydantic_object.__fields__.keys())
         self.parser = JsonOutputParser(pydantic_object=pydantic_object)
         self.output_instructions = self.parser.get_format_instructions()
 
         self.system_prompt_path = system_prompt_path
         self.system_prompt_template = load_prompt(system_prompt_path).template
-        self.system_message = system_message_input_variables
+        self.system_message_input_variables = system_message_input_variables
 
         self.human_prompt_path = human_prompt_path
         human_prompt = load_prompt(human_prompt_path)
         self.human_prompt_template = human_prompt.template
 
-        query_variables = human_prompt.input_variables
-        if not 'instructions' in query_variables:
+        request_variables = human_prompt.input_variables
+        if not 'instructions' in request_variables:
             logger.debug('"instuctions" is not the input variable of human prompt')
             sys.exit()
-        elif not 'output_instructions' in query_variables:
+        elif not 'output_instructions' in request_variables:
             logger.debug('"output_instructions" is not the input variable of human prompt')
             sys.exit()
         else:
-            query_variables.remove('instructions')
-            query_variables.remove('output_instructions')
-            self.query_key = query_variables[0]
+            request_variables.remove('instructions')
+            request_variables.remove('output_instructions')
+            self.request_variable = request_variables[0]
+
+
+    @property
+    def system_message(self):
+        return (
+            self
+            .system_prompt_template
+            .format(**self.system_message_input_variables)
+        )
 
 
     def zero_shot(self) -> ChatPromptTemplate:
         return (
             ChatPromptTemplate
             .from_messages([
                 ("system", self.system_prompt_template),
                 MessagesPlaceholder(variable_name = "history"),
                 ("human", self.human_prompt_template)
             ])
             .partial(
-                **self.system_message,
+                **self.system_message_input_variables,
                 output_instructions = self.output_instructions,
             )
         )
 
 
     def __create_fewshot_prompt(self,
-                                query_examples: List[str],
+                                request_examples: List[str],
                                 response_examples: List[str],
                                ) -> ChatPromptTemplate:
         few_shot_example = [
             {
-                self.query_key: query_examples[i],
+                self.request_variable: request_examples[i],
                 "response": response_examples[i],
                 "instructions": "",
                 "output_instructions": "",
             }
             for i in range(len(response_examples))
         ]
 
@@ -89,48 +98,45 @@
             .from_messages([
                 ("system", self.system_prompt_template),
                 few_shot_prompt,
                 MessagesPlaceholder(variable_name = "history"),
                 ("human", self.human_prompt_template),
             ])
             .partial(
-                **self.system_message,
+                **self.system_message_input_variables,
                 output_instructions = self.output_instructions
             )
         )
 
 
     def few_shot(self, fewshot_examples_path: str) -> ChatPromptTemplate:
         """Create fewshot prompt.
         Args:
             `fewshot_examples_path`: It must be json lines file. 
 
-            `query_key`: Each json instance must contains this key and for all
-                the other keys are the keys of json format of LLM response.
-
         Example:
             .. code-block:: python
 
                 fewshot_examples = [
-                    {"query": "", "label": "", "reason": ""},
-                    {"query": "", "label": "", "reason": ""},
+                    {"request_varialbe": "", "label": "", "reason": ""},
+                    {"request_variable": "", "label": "", "reason": ""},
                 ]
                 with Path('fewshot_examples.jsonl').open('w') as f:
                     for i in fewshot_examples:
                         f.write(orjson.dumps(i, option=orjson.OPT_APPEND_NEWLINE))
 
                 Prompt.few_shot('fewshot_examples.jsonl')
         """
         fewshot_examples = read_jsonl(fewshot_examples_path)
-        query_examples = []
+        request_examples = []
         response_examples = []
 
         for item in fewshot_examples:
-            query_examples.append(item[self.query_key])
+            request_examples.append(item[self.request_variable])
             response_examples.append(
                 orjson.dumps(
-                    {k: item[k] for k in self.response_keys}
+                    {k: item[k] for k in self.response_variables}
                 )
                 .decode()
             )
 
-        return self.__create_fewshot_prompt(query_examples, response_examples)
+        return self.__create_fewshot_prompt(request_examples, response_examples)
```

### Comparing `llm_research-0.1.0/llm_research/model/utils.py` & `llm_research-0.2.0/llm_research/model/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dotenv import load_dotenv
 import orjson
 from os import getenv
 from pathlib import Path
 from typing import Dict, List
 
 
+
 def env_setup(tag: str = "OPENAI", env_file: str = '.env') -> None:
     load_dotenv(env_file)
     match tag:
         case "GOOGLE":
             key_name = 'GOOGLE_APPLICATION_CREDENTIALS'
         case _:
             key_name = 'OPENAI_API_KEY'
@@ -23,20 +24,28 @@
             with file.open("a") as f:
                 f.write(f"{key_name}={key}\n")
         else:
             with file.open("w") as f:
                 f.write(f"{key_name}={key}\n")
 
 
-def read_jsonl(
-    path: str | Path,
-    n: int = -1,
-    return_str: bool = False
-) -> List[Dict] | List[str]:
-    return (
-        [orjson.loads(i) for i in Path(path).read_text().split("\n")[:n]]
-        if not return_str
-        else
-        [i for i in Path(path).read_text().split("\n")[:n]]
-    )
+def read_jsonl(path: str | Path,
+               n: int = -1,
+               return_str: bool = False) -> List[Dict] | List[str]:
+
+    res = Path(path).read_text().split('\n')
+    if n == len(res):
+        n = -1
+
+    if not return_str and n == -1 and res[-1] != '':
+        return [orjson.loads(i) for i in res]
+    if return_str and n == -1 and res[-1] != '':
+        return res
+    else:
+         return (
+            [orjson.loads(i) for i in res[:n]]
+            if not return_str
+            else
+            res[:n]
+        )
```

### Comparing `llm_research-0.1.0/pyproject.toml` & `llm_research-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-research"
-version = "0.1.0"
+version = "0.2.0"
 description = "A minimum Python package built on top of the LangChain framework to interact with LLM."
 authors = ["githubjacky"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "llm_research"}]
```

### Comparing `llm_research-0.1.0/PKG-INFO` & `llm_research-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-research
-Version: 0.1.0
+Version: 0.2.0
 Summary: A minimum Python package built on top of the LangChain framework to interact with LLM.
 License: MIT
 Author: githubjacky
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

