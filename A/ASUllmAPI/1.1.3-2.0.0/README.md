# Comparing `tmp/asullmapi-1.1.3.tar.gz` & `tmp/asullmapi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asullmapi-1.1.3.tar", last modified: Mon May 13 22:18:20 2024, max compression
+gzip compressed data, was "asullmapi-2.0.0.tar", last modified: Thu May 30 20:58:01 2024, max compression
```

## Comparing `asullmapi-1.1.3.tar` & `asullmapi-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 22:18:20.851169 asullmapi-1.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-13 22:18:20.823839 asullmapi-1.1.3/ASUllmAPI/
--rw-rw-rw-   0        0        0      169 2024-05-08 21:25:24.000000 asullmapi-1.1.3/ASUllmAPI/__init__.py
--rw-rw-rw-   0        0        0     2980 2024-05-09 21:37:02.000000 asullmapi-1.1.3/ASUllmAPI/api.py
--rw-rw-rw-   0        0        0     2006 2024-05-09 21:37:02.000000 asullmapi-1.1.3/ASUllmAPI/model_config.py
--rw-rw-rw-   0        0        0     1705 2024-05-13 19:58:06.000000 asullmapi-1.1.3/ASUllmAPI/multithreading.py
--rw-rw-rw-   0        0        0      666 2024-05-08 21:25:24.000000 asullmapi-1.1.3/ASUllmAPI/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 22:18:20.846069 asullmapi-1.1.3/ASUllmAPI.egg-info/
--rw-rw-rw-   0        0        0     1385 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-13 22:18:20.000000 asullmapi-1.1.3/ASUllmAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1124 2024-04-18 18:53:24.000000 asullmapi-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     1385 2024-05-13 22:18:20.848091 asullmapi-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      671 2024-05-13 22:14:19.000000 asullmapi-1.1.3/README.md
--rw-rw-rw-   0        0        0      724 2024-05-13 22:15:05.000000 asullmapi-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 22:18:20.851666 asullmapi-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 20:58:01.079820 asullmapi-2.0.0/
+drwxrwxrwx   0        0        0        0 2024-05-30 20:58:01.056283 asullmapi-2.0.0/ASUllmAPI/
+-rw-rw-rw-   0        0        0      235 2024-05-22 00:53:41.000000 asullmapi-2.0.0/ASUllmAPI/__init__.py
+-rw-rw-rw-   0        0        0     2387 2024-05-30 18:31:51.000000 asullmapi-2.0.0/ASUllmAPI/api.py
+-rw-rw-rw-   0        0        0     6123 2024-05-30 19:28:29.000000 asullmapi-2.0.0/ASUllmAPI/model_config.py
+-rw-rw-rw-   0        0        0     1779 2024-05-30 18:18:50.000000 asullmapi-2.0.0/ASUllmAPI/multithreading.py
+-rw-rw-rw-   0        0        0      981 2024-05-29 15:38:49.000000 asullmapi-2.0.0/ASUllmAPI/utils.py
+-rw-rw-rw-   0        0        0     4218 2024-05-24 23:12:09.000000 asullmapi-2.0.0/ASUllmAPI/web_socket.py
+drwxrwxrwx   0        0        0        0 2024-05-30 20:58:01.073477 asullmapi-2.0.0/ASUllmAPI.egg-info/
+-rw-rw-rw-   0        0        0     1384 2024-05-30 20:58:01.000000 asullmapi-2.0.0/ASUllmAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-05-30 20:58:01.000000 asullmapi-2.0.0/ASUllmAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 20:58:01.000000 asullmapi-2.0.0/ASUllmAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-30 20:58:01.000000 asullmapi-2.0.0/ASUllmAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 20:58:01.000000 asullmapi-2.0.0/ASUllmAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1124 2024-04-18 18:53:24.000000 asullmapi-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1384 2024-05-30 20:58:01.078042 asullmapi-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-05-13 22:31:06.000000 asullmapi-2.0.0/README.md
+-rw-rw-rw-   0        0        0      724 2024-05-30 20:42:43.000000 asullmapi-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 20:58:01.080845 asullmapi-2.0.0/setup.cfg
```

### Comparing `asullmapi-1.1.3/ASUllmAPI/api.py` & `asullmapi-2.0.0/ASUllmAPI/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 import json
 import requests
 import traceback
 from time import sleep
+
 from .model_config import ModelConfig
 
-__author__ = 'swliu'
+__author__ = ['swliu', 'vshourie']
 
 
 def query_llm(model: ModelConfig, query: str, num_retry: int = 3,
-              success_sleep: float = 0, fail_sleep: float = 1) -> str:
+              success_sleep: float = 0, fail_sleep: float = 1) -> dict:
+    response_dict = {"response": ""}
     for i in range(num_retry):
         try:
-            payload = _compute_payload(model=model, query=query)
-            headers = _compute_headers(model.access_token)
+            payload = model.compute_payload(query=query)
+            headers = model.compute_headers()
             response = requests.post(model.api_url, json=payload, headers=headers)
-            response_text = response.json()['response']
+            response_text = response.json()
+
+            # We parse through relevant keys
+            for key in response_text.keys():
+                response_dict[key] = response_text[key]
 
             if success_sleep > 0:
                 sleep(success_sleep)
-            return response_text
+
         except Exception as e:
             print(traceback.format_exc())
             if fail_sleep > 0:
                 sleep(fail_sleep)
-            continue
-    return ""
+    return response_dict
 
 
-def query_model_info_api(access_token, url, num_retry: int = 3,
-                         success_sleep: float = 1.0, fail_sleep=1.0) -> list:
+def query_model_info_api(model: ModelConfig, num_retry: int = 3,
+                         success_sleep: float = 1.0, fail_sleep: float = 1.0) -> list:
     """
-    :param access_token: API access token.
-    :param url: API endpoint
+    :param model: A ModelConfig configured with the model info endpoint URL AND the access key at a minimum.
     :param num_retry: int
     :param success_sleep: seconds to delay execution when API call successful (float)
     :param fail_sleep: seconds to delay execution when API call unsuccessful (float)
     :return: a list of large language models that are hosted by ASU
     """
     for i in range(num_retry):
         try:
-            headers = _compute_headers(access_token=access_token)
-            response = requests.get(url=url, headers=headers)
+            headers = model.compute_headers()
+            response = requests.get(url=model.api_url, headers=headers)
             models_dict = json.loads(response.content)
             models = models_dict["models"]
             if success_sleep > 0:
                 sleep(success_sleep)
             return models
         except Exception as e:
             print(traceback.format_exc())
@@ -61,34 +65,7 @@
     }
     return mapper
 
 
 def model_list(models: list) -> set:
     models = {model["name"] for model in models}
     return models
-
-
-def _compute_headers(access_token):
-    headers = {
-        "Accept": "application/json",
-        "Authorization": f'Bearer {access_token}'
-    }
-    return headers
-
-
-def _compute_payload(model: ModelConfig, query: str):
-    payload = {"prompt": query}
-
-    if model.name:
-        payload["model_name"] = model.name
-    if model.provider:
-        payload["model_provider"] = model.provider
-    if model.model_params:
-        payload["model_params"] = model.model_params
-    if model.enable_search:
-        payload["enable_search"] = model.enable_search
-    if model.search_params:
-        payload["search_params"] = model.search_params
-    if model.project_id:
-        payload["project_id"] = model.project_id
-
-    return payload
```

### Comparing `asullmapi-1.1.3/ASUllmAPI/multithreading.py` & `asullmapi-2.0.0/ASUllmAPI/multithreading.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .model_config import ModelConfig
 from .utils import time_api
 
 
 @time_api
 def batch_query_llm(model: ModelConfig, queries: Dict[int, str], max_threads: int,
                     num_retry: int = 3, auto_increase_retry: bool = False,
-                    success_sleep: float = 0.0, fail_sleep: float = 1.0) -> Dict[int, str]:
+                    success_sleep: float = 0.0, fail_sleep: float = 1.0) -> Dict[int, dict]:
     with ThreadPoolExecutor(max_workers=max_threads) as executor:
         # Submit tasks to the executor - order of return will be asynchronous.
         # If `auto_increase_retry` enabled, then scaling API backoff is implemented.
         if auto_increase_retry:
             future_to_query = {executor.submit(query_llm, model, question,
                                                qid, success_sleep, fail_sleep): qid
                                for qid, question in queries.items()}
@@ -27,12 +27,13 @@
         # Collect and return results as they complete while maintaining order.
         results = {}
         for future in tqdm(as_completed(future_to_query)):
             qid = future_to_query[future]
             try:
                 result = future.result()
                 results[qid] = result
+                print(f"......Received response for question {qid}...")
             except Exception as exc:
                 print(f"{qid} generated an exception: {exc}")
                 results[qid] = None
 
         return results
```

### Comparing `asullmapi-1.1.3/ASUllmAPI/utils.py` & `asullmapi-2.0.0/ASUllmAPI/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 import time
+import json
+import asyncio
+
+
+def begin_task_execution(async_func):
+    def wrap(*args, **kwargs):
+        return asyncio.run(async_func(*args, **kwargs))
+
+    return wrap
+
+
+def load_json_buffer(string):
+    try:
+        return json.loads(string)
+    except json.JSONDecodeError:
+        return None
 
 
 def time_api(func):
     """
     Decorator to measure the execution time of a function.
     """
```

### Comparing `asullmapi-1.1.3/ASUllmAPI.egg-info/PKG-INFO` & `asullmapi-2.0.0/ASUllmAPI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllmAPI
-Version: 1.1.3
+Version: 2.0.0
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>, Varun Shourie <svarun195@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,8 +26,8 @@
 Note: Depending on your Python distribution, you may need to pip or conda
 install `requests` and `tqdm` if it is not available in your local environment.
 ```markdown
 pip install requests
 pip install tqdm
 ```
 
-See README.md documentation at this [link.](https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/blob/main/base-ASUllm-documentation/README.md).
+See README.md documentation at this [link](https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/blob/main/base-ASUllm-documentation/README.md).
```

### Comparing `asullmapi-1.1.3/LICENSE` & `asullmapi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asullmapi-1.1.3/PKG-INFO` & `asullmapi-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASUllmAPI
-Version: 1.1.3
+Version: 2.0.0
 Summary: A simple python package to facilitate connection to ASU LLM API
 Author-email: Stella Wenxing Liu <stellawenxingliu@gmail.com>, Varun Shourie <svarun195@gmail.com>
 Project-URL: Homepage, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization
 Project-URL: Issues, https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,8 +26,8 @@
 Note: Depending on your Python distribution, you may need to pip or conda
 install `requests` and `tqdm` if it is not available in your local environment.
 ```markdown
 pip install requests
 pip install tqdm
 ```
 
-See README.md documentation at this [link.](https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/blob/main/base-ASUllm-documentation/README.md).
+See README.md documentation at this [link](https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/blob/main/base-ASUllm-documentation/README.md).
```

### Comparing `asullmapi-1.1.3/pyproject.toml` & `asullmapi-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ASUllmAPI"
-version = "1.1.3"
+version = "2.0.0"
 authors = [
     { name="Stella Wenxing Liu", email="stellawenxingliu@gmail.com" },
     { name="Varun Shourie", email="svarun195@gmail.com" }
 ]
 description = "A simple python package to facilitate connection to ASU LLM API"
 readme = "README.md"
 requires-python = ">=3.8"
```

