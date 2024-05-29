# Comparing `tmp/baserun-1.0.0b5.tar.gz` & `tmp/baserun-1.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-1.0.0b5.tar", last modified: Wed May 29 19:15:35 2024, max compression
+gzip compressed data, was "baserun-1.0.0b6.tar", last modified: Wed May 29 21:40:05 2024, max compression
```

## Comparing `baserun-1.0.0b5.tar` & `baserun-1.0.0b6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.315815 baserun-1.0.0b5/
--rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b5/LICENSE
--rw-r--r--   0 epeterson   (501) staff       (20)     6559 2024-05-29 19:15:35.315623 baserun-1.0.0b5/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     4905 2024-05-29 18:31:57.000000 baserun-1.0.0b5/README.md
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.286478 baserun-1.0.0b5/baserun/
--rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-29 18:43:55.000000 baserun-1.0.0b5/baserun/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     8668 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/api.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.308880 baserun-1.0.0b5/baserun/integrations/
--rw-r--r--   0 epeterson   (501) staff       (20)      305 2024-05-29 18:45:54.000000 baserun-1.0.0b5/baserun/integrations/integration.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2045 2024-05-29 19:01:42.000000 baserun-1.0.0b5/baserun/integrations/llamaindex.py
--rw-r--r--   0 epeterson   (501) staff       (20)     7049 2024-05-29 18:46:24.000000 baserun-1.0.0b5/baserun/mixins.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.310958 baserun-1.0.0b5/baserun/models/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/models/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/models/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/models/tags.py
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/py.typed
--rw-r--r--   0 epeterson   (501) staff       (20)      481 2024-05-29 19:03:25.000000 baserun-1.0.0b5/baserun/pytest_plugin.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/utils.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.311919 baserun-1.0.0b5/baserun/wrappers/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/wrappers/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    16493 2024-05-29 18:46:48.000000 baserun-1.0.0b5/baserun/wrappers/openai.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.314449 baserun-1.0.0b5/baserun.egg-info/
--rw-r--r--   0 epeterson   (501) staff       (20)     6559 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)      570 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/entry_points.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/requires.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/top_level.txt
--rw-r--r--   0 epeterson   (501) staff       (20)     1091 2024-05-29 19:15:25.000000 baserun-1.0.0b5/pyproject.toml
--rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-29 19:15:35.316764 baserun-1.0.0b5/setup.cfg
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.313201 baserun-1.0.0b5/tests/
--rw-r--r--   0 epeterson   (501) staff       (20)    13539 2024-05-29 18:31:57.000000 baserun-1.0.0b5/tests/testing_functions.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 21:40:05.967913 baserun-1.0.0b6/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b6/LICENSE
+-rw-r--r--   0 epeterson   (501) staff       (20)     6568 2024-05-29 21:40:05.967731 baserun-1.0.0b6/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     4914 2024-05-29 21:35:58.000000 baserun-1.0.0b6/README.md
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 21:40:05.942343 baserun-1.0.0b6/baserun/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-29 18:43:55.000000 baserun-1.0.0b6/baserun/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     8818 2024-05-29 21:39:39.000000 baserun-1.0.0b6/baserun/api.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 21:40:05.963449 baserun-1.0.0b6/baserun/integrations/
+-rw-r--r--   0 epeterson   (501) staff       (20)      305 2024-05-29 19:59:55.000000 baserun-1.0.0b6/baserun/integrations/integration.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2045 2024-05-29 19:59:55.000000 baserun-1.0.0b6/baserun/integrations/llamaindex.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     6943 2024-05-29 19:59:56.000000 baserun-1.0.0b6/baserun/mixins.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 21:40:05.965036 baserun-1.0.0b6/baserun/models/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b6/baserun/models/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-29 18:31:57.000000 baserun-1.0.0b6/baserun/models/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-29 18:31:57.000000 baserun-1.0.0b6/baserun/models/tags.py
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 19:59:55.000000 baserun-1.0.0b6/baserun/py.typed
+-rw-r--r--   0 epeterson   (501) staff       (20)      533 2024-05-29 20:00:24.000000 baserun-1.0.0b6/baserun/pytest_plugin.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-29 18:31:57.000000 baserun-1.0.0b6/baserun/utils.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 21:40:05.965900 baserun-1.0.0b6/baserun/wrappers/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b6/baserun/wrappers/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    17477 2024-05-29 21:33:09.000000 baserun-1.0.0b6/baserun/wrappers/openai.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 21:40:05.967074 baserun-1.0.0b6/baserun.egg-info/
+-rw-r--r--   0 epeterson   (501) staff       (20)     6568 2024-05-29 21:40:05.000000 baserun-1.0.0b6/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)      570 2024-05-29 21:40:05.000000 baserun-1.0.0b6/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-29 21:40:05.000000 baserun-1.0.0b6/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-29 21:40:05.000000 baserun-1.0.0b6/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-29 21:40:05.000000 baserun-1.0.0b6/baserun.egg-info/requires.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-29 21:40:05.000000 baserun-1.0.0b6/baserun.egg-info/top_level.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)     1093 2024-05-29 21:38:17.000000 baserun-1.0.0b6/pyproject.toml
+-rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-29 21:40:05.968522 baserun-1.0.0b6/setup.cfg
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 21:40:05.966432 baserun-1.0.0b6/tests/
+-rw-r--r--   0 epeterson   (501) staff       (20)    13673 2024-05-29 20:29:08.000000 baserun-1.0.0b6/tests/testing_functions.py
```

### Comparing `baserun-1.0.0b5/LICENSE` & `baserun-1.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b5/PKG-INFO` & `baserun-1.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 **[Baserun](https://baserun.ai)** is the testing and observability platform for LLM apps.
 
 # Quick Start
 
 ## 1. Install Baserun
 
 ```bash
-pip install baserun
+pip install baserun==1.0.0b6
 ```
 
 ## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
```

### Comparing `baserun-1.0.0b5/README.md` & `baserun-1.0.0b6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 **[Baserun](https://baserun.ai)** is the testing and observability platform for LLM apps.
 
 # Quick Start
 
 ## 1. Install Baserun
 
 ```bash
-pip install baserun
+pip install baserun==1.0.0b6
 ```
 
 ## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
```

### Comparing `baserun-1.0.0b5/baserun/__init__.py` & `baserun-1.0.0b6/baserun/__init__.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b5/baserun/api.py` & `baserun-1.0.0b6/baserun/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 def count_message_tokens(text: str, encoder="cl100k_base"):
     return len(tiktoken.get_encoding(encoder).encode(text))
 
 
 async def worker(queue: Queue, base_url: str, api_key: str):
     logger.debug(f"Starting worker with base_url: {base_url}")
-    tasks: List[asyncio.Task] = []  # Create tasks locally
     async with httpx.AsyncClient(http2=True) as client:
         while True:
             try:
                 item: Dict = queue.get_nowait()
             except Empty:
                 sleep(1)
                 continue
@@ -76,15 +75,15 @@
     logger.debug(f"Waiting for {len(tasks)} tasks to finish")
     await asyncio.gather(*tasks)
     logger.debug("Exiting worker")
     loop = asyncio.get_running_loop()
     loop.stop()
 
 
-def run_worker(queue, base_url, api_key):
+def run_worker(queue: Queue, base_url: str, api_key: str):
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     loop.create_task(worker(queue, base_url, api_key))
     try:
         loop.run_forever()
     except KeyboardInterrupt:
         pass
@@ -99,14 +98,38 @@
             target=run_worker,
             args=(exporter_queue, base_url, api_key),
         )
         exporter_process.daemon = False
         exporter_process.start()
 
 
+def stop_worker():
+    global exporter_process, exporter_queue, tasks
+
+    # Signal the worker to stop
+    if exporter_queue is not None and not getattr(exporter_queue, "_closed"):
+        exporter_queue.put(None)
+
+    logger.debug("Baserun Exiting")
+
+    if exporter_process is not None and exporter_process.is_alive():
+        loop = asyncio.get_event_loop()
+        if tasks:
+            loop.run_until_complete(asyncio.gather(*tasks))
+
+        # Terminate the process
+        exporter_process.terminate()
+        exporter_process.join()
+
+    # Close and join the queue
+    if exporter_queue is not None and not getattr(exporter_queue, "_closed"):
+        exporter_queue.close()
+        exporter_queue.join_thread()
+
+
 class ApiClient:
     def __init__(
         self,
         client: Union["WrappedOpenAIBaseClient"],
         api_key: Optional[str] = None,
         base_url: Optional[str] = None,
     ):
@@ -117,26 +140,15 @@
 
         start_worker(
             base_url or os.getenv("BASERUN_API_URL") or "https://app.baserun.ai",
             api_key or os.getenv("BASERUN_API_KEY") or "",
         )
 
     def exit_handler(self, *args) -> None:
-        global exporter_process, exporter_queue, tasks  # Add tasks to global variables
-        if exporter_process is not None:
-            # Put None into the queue to signal the worker to stop
-            exporter_queue.put(None)
-            while len(tasks):
-                logger.debug(f"Waiting for {len(tasks)} tasks to finish")
-                sleep(0.25)
-            exporter_process.terminate()
-            exporter_process.join()
-        # Close and join the queue
-        if exporter_queue is not None:
-            exporter_queue.close()
+        stop_worker()
 
     def submit_completion(self, completion: "WrappedChatCompletion"):
         dict_items = completion.model_dump()
         dict_items.pop("client", None)
         start_timestamp = dict_items.pop("start_timestamp", None)
         end_timestamp = dict_items.pop("end_timestamp", None)
         first_token_timestamp = dict_items.pop("first_token_timestamp", None)
```

### Comparing `baserun-1.0.0b5/baserun/integrations/llamaindex.py` & `baserun-1.0.0b6/baserun/integrations/llamaindex.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b5/baserun/mixins.py` & `baserun-1.0.0b6/baserun/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 class CompletionMixin(ABC):
     tags: List[Tag]
     evals: List[CompletionEval]
     completion_id: str
     tool_results: List[Dict[str, Any]]
 
-    # TODO: Should this be an ABC? Or have an ABC somewhere (to define tags, evals, etc without pydantic)
     def annotate(self, key: str, value: str, metadata: Optional[Dict[str, Any]] = None):
         self.tags.append(
             Tag(
                 target_type="completion",
                 target_id=self.completion_id,
                 tag_type="annotation",
                 key=key,
```

### Comparing `baserun-1.0.0b5/baserun/models/evals.py` & `baserun-1.0.0b6/baserun/models/evals.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b5/baserun/models/tags.py` & `baserun-1.0.0b6/baserun/models/tags.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b5/baserun/utils.py` & `baserun-1.0.0b6/baserun/utils.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b5/baserun/wrappers/openai.py` & `baserun-1.0.0b6/baserun/wrappers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from openai import AsyncStream
 from openai import OpenAI as BaseOpenAI
 from openai._streaming import Stream, extract_stream_chunk_type
 from openai._types import ResponseT
 from openai.resources.chat import AsyncChat, AsyncCompletions, Chat, Completions
 from openai.types.chat import ChatCompletion, ChatCompletionChunk, ChatCompletionMessageParam
 from openai.types.chat.chat_completion_chunk import Choice
+from openai.types.completion_usage import CompletionUsage
 from pydantic import BaseModel, ConfigDict, Field
 
 from baserun.api import ApiClient
 from baserun.integrations.integration import Integration
 from baserun.mixins import ClientMixin, CompletionMixin
 from baserun.models.evals import CompletionEval, TraceEval
 from baserun.models.tags import Tag
@@ -26,14 +27,15 @@
 logger = logging.getLogger(__name__)
 
 
 class WrappedChatCompletion(ChatCompletion, CompletionMixin):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     client: "WrappedOpenAIBaseClient"
     name: str
+    error: Optional[str] = None
     trace_id: str
     completion_id: str
     template: Optional[str]
     start_timestamp: datetime
     first_token_timestamp: datetime
     end_timestamp: datetime
     input_messages: List[ChatCompletionMessageParam] = Field(default_factory=list)
@@ -47,14 +49,15 @@
 
 
 class WrappedStreamBase(CompletionMixin, BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     client: "WrappedOpenAIBaseClient"
     id: Optional[str] = None
     name: str
+    error: Optional[str] = None
     trace_id: str
     completion_id: str
     template: Optional[str] = None
     start_timestamp: datetime
     end_timestamp: Optional[datetime] = None
     first_token_timestamp: Optional[datetime] = None
     input_messages: List[ChatCompletionMessageParam] = Field(default_factory=list)
@@ -67,14 +70,15 @@
     captured_choices: List[Choice] = Field(default_factory=list)
 
     def __init__(self, *args, **kwargs):
         CompletionMixin.__init__(self)
         BaseModel.__init__(self, **kwargs)
         # Get rid of special kwargs that we take but OpenAI doesn't
         kwargs.pop("name", None)
+        kwargs.pop("error", None)
         kwargs.pop("completion_id", None)
         kwargs.pop("trace_id", None)
         kwargs.pop("template", None)
         kwargs.pop("config_params", None)
         kwargs.pop("start_timestamp", None)
         kwargs.pop("end_timestamp", None)
         kwargs.pop("first_token_timestamp", None)
@@ -139,24 +143,24 @@
         self,
         *args,
         name: Optional[str] = None,
         variables: Optional[Dict[str, str]] = None,
         template: Optional[str] = None,
         **kwargs,
     ) -> Union[WrappedChatCompletion, WrappedSyncStream]:
-        try:
-            messages: List[ChatCompletionMessageParam] = kwargs.pop("messages", [])
-            if not name:
-                for message in reversed(messages):
-                    if message.get("content") and message.get("role") == "assistant":
-                        name = str(message["content"])[:20]
-                        break
-            if not name:
-                name = "OpenAI Completion"
+        messages: List[ChatCompletionMessageParam] = kwargs.pop("messages", [])
+        if not name:
+            for message in reversed(messages):
+                if message.get("content") and message.get("role") == "assistant":
+                    name = str(message["content"])[:20]
+                    break
+        if not name:
+            name = "OpenAI Completion"
 
+        try:
             start_timestamp = datetime.now(timezone.utc)
             stream_or_completion = super().create(*args, **kwargs, messages=messages)
             first_token_timestamp = datetime.now(timezone.utc)
             wrapped: Union[WrappedChatCompletion, WrappedSyncStream, None] = None
 
             if isinstance(stream_or_completion, ChatCompletion):
                 wrapped = WrappedChatCompletion(
@@ -194,18 +198,38 @@
             if variables:
                 for key, value in variables.items():
                     wrapped.variable(key, value)
             else:
                 wrapped.submit_to_baserun()
 
             return wrapped
-        except Exception as e:
-            # TODO: Probably should assemble a Completion object in an error state and submit that
-            self._client.error = traceback.format_exc()
+        except BaseException as e:
+            self._client.error = "\n".join(traceback.format_exception_only(BaseException, value=e)).strip()
             self._client.submit_to_baserun()
+            completion_id = str(uuid4())
+            wrapped = WrappedChatCompletion(
+                id=f"chatcompl-error-{completion_id}",
+                client=self._client,
+                trace_id=self._client.trace_id,
+                name=name,
+                template=template,
+                start_timestamp=start_timestamp,
+                end_timestamp=datetime.now(),
+                first_token_timestamp=datetime.now(),
+                config_params=kwargs,
+                completion_id=completion_id,
+                input_messages=messages,
+                error=self._client.error,
+                object="chat.completion",
+                choices=[],
+                created=int(datetime.now().timestamp()),
+                usage=CompletionUsage(total_tokens=0, completion_tokens=0, prompt_tokens=0),
+                **kwargs,
+            )
+            wrapped.submit_to_baserun()
             raise e
 
 
 class WrappedAsyncCompletions(AsyncCompletions):
     _client: "WrappedAsyncOpenAIClient"
 
     @copy_type_hints(AsyncCompletions)
```

### Comparing `baserun-1.0.0b5/baserun.egg-info/PKG-INFO` & `baserun-1.0.0b6/baserun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b5
+Version: 1.0.0b6
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 **[Baserun](https://baserun.ai)** is the testing and observability platform for LLM apps.
 
 # Quick Start
 
 ## 1. Install Baserun
 
 ```bash
-pip install baserun
+pip install baserun==1.0.0b6
 ```
 
 ## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
```

### Comparing `baserun-1.0.0b5/baserun.egg-info/SOURCES.txt` & `baserun-1.0.0b6/baserun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b5/pyproject.toml` & `baserun-1.0.0b6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baserun"
-version = "1.0.0b5"
+version = "1.0.0b6"
 description = "tools for testing, debugging, and evaluating llm features."
 readme = "README.md"
 license = { file = "LICENSE" }
-authors = [
-    { name = "Erik Peterson", email = "erik@baserun.ai" }
-]
+authors = [{ name = "Erik Peterson", email = "erik@baserun.ai" }]
 requires-python = ">=3.8, <3.12"
-dependencies = [
-    "httpx[http2]>=0.24.0",
-]
+dependencies = ["httpx[http2]>=0.24.0"]
 
 [project.urls]
 Homepage = "https://baserun.ai"
 Repository = "https://github.com/baserun-ai/baserun-py"
 
 [project.entry-points.pytest11]
 pbaserun = "baserun.pytest_plugin"
 
 [lint]
-extend-select = ["I", "T20"]  # isort, flake8-print
+extend-select = ["I", "T20"] # isort, flake8-print
 target-version = "py38"
 line-length = 120
 extend-exclude = []
 [lint.per-file-ignores]
-"baserun/v1/baserun_pb2.py" = "E501"  # Line too long
-"tests/*" = "T201"  # `print` found
+"baserun/v1/baserun_pb2.py" = "E501" # Line too long
+"tests/*" = "T201"                   # `print` found
 
 [tool.ruff]
 line-length = 120
 
 [tool.black]
 line-length = 120
```

### Comparing `baserun-1.0.0b5/tests/testing_functions.py` & `baserun-1.0.0b6/tests/testing_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import argparse
 import asyncio
 import inspect
 import json
+import logging
 import os
 import sys
 import traceback
 from time import sleep
 
 import openai
 from openai import AsyncOpenAI, NotFoundError, OpenAI
 from openai.types import CreateEmbeddingResponse
 from openai.types.chat.chat_completion_message import FunctionCall
 
-from baserun import init
+from baserun import api, init
 
 
 def openai_chat(prompt="What is the capital of the US?") -> str:
     client = init(OpenAI(), name="openai_chat")
     completion = client.chat.completions.create(
         name="openai_chat completion", model="gpt-4o", messages=[{"role": "user", "content": prompt}]
     )
@@ -202,15 +203,15 @@
         client.chat.completions.create(
             name="openai_chat_error completion",
             model="asdf",
             messages=[{"role": "user", "content": prompt}],
         )
     except NotFoundError as e:
         client.eval("openai_chat_async_streaming.content").includes(e.message, "does not exist")
-        raise e
+        return f"Errored with {e} successfully"
     finally:
         openai.api_type = original_api_type
 
 
 def openai_chat_response_format(prompt="What is the capital of the US?") -> str:
     client = init(OpenAI())
     completion = client.chat.completions.create(
@@ -365,14 +366,16 @@
 
     parser = argparse.ArgumentParser(description="Execute a function with a prompt.")
     parser.add_argument("function_to_call", type=str, help="Name of the function to call")
     parser.add_argument("--prompt", type=str, help="Prompt to pass to the function", default=None)
 
     parsed_args = parser.parse_args()
 
+    logging.basicConfig(level=logging.DEBUG)
+
     # Resolve the string function name to the function object
     function_name = parsed_args.function_to_call
     global_variables = {f: globals().get(f) for f in globals()}
     traced_functions = {n: f for n, f in global_variables.items() if callable(f) and f.__name__ == "wrapper"}
     if function_name == "all":
         for name, func in traced_functions.items():
             print(f"===== Calling function {name} =====\n")
@@ -382,7 +385,10 @@
             except Exception:
                 exc_type, exc_value, exc_traceback = sys.exc_info()
                 traceback.print_exception(exc_type, exc_value, exc_traceback)
     else:
         call_function(traced_functions, function_name, parsed_args)
 
     sleep(4)
+    api.stop_worker()
+
+    sleep(1)
```

