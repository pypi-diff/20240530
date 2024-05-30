# Comparing `tmp/rockai_cli_app-0.2.4.tar.gz` & `tmp/rockai_cli_app-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.2.4.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.2.6.tar", max compression
```

## Comparing `rockai_cli_app-0.2.4.tar` & `rockai_cli_app-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      244 2024-05-29 02:21:58.351513 rockai_cli_app-0.2.4/README.md
--rw-r--r--   0        0        0      715 2024-05-30 04:44:30.520167 rockai_cli_app-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     7769 2024-05-30 04:43:44.830882 rockai_cli_app-0.2.4/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0       36 2024-05-16 02:40:27.277757 rockai_cli_app-0.2.4/rockai_cli_app/constant.py
--rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.4/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.4/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    12108 2024-05-11 14:08:05.184260 rockai_cli_app-0.2.4/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     2819 2024-05-06 14:26:16.309849 rockai_cli_app-0.2.4/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      604 2024-05-06 14:26:16.309950 rockai_cli_app-0.2.4/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0     1285 2024-05-06 14:26:16.310077 rockai_cli_app-0.2.4/rockai_cli_app/main.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.4/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.4/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.4/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.4/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.4/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.4/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.4/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.4/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.4/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.4/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.4/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.4/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      393 2024-05-29 03:28:45.579316 rockai_cli_app-0.2.4/rockai_cli_app/test.py
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1181 2024-05-30 08:10:29.119571 rockai_cli_app-0.2.6/README.md
+-rw-r--r--   0        0        0      717 2024-05-30 08:35:13.465910 rockai_cli_app-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     8044 2024-05-30 08:09:03.481852 rockai_cli_app-0.2.6/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0     2346 2024-05-06 14:26:16.309393 rockai_cli_app-0.2.6/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.309507 rockai_cli_app-0.2.6/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    12294 2024-05-30 08:34:54.724275 rockai_cli_app-0.2.6/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     1351 2024-05-30 08:18:34.749394 rockai_cli_app-0.2.6/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      646 2024-05-30 08:22:44.453285 rockai_cli_app-0.2.6/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310199 rockai_cli_app-0.2.6/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 14:26:16.310349 rockai_cli_app-0.2.6/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-05-06 14:26:16.310457 rockai_cli_app-0.2.6/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0     1297 2024-05-30 08:12:33.778287 rockai_cli_app-0.2.6/rockai_cli_app/rock.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310565 rockai_cli_app-0.2.6/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-06 14:26:16.310696 rockai_cli_app-0.2.6/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-05-06 14:26:16.310797 rockai_cli_app-0.2.6/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.310900 rockai_cli_app-0.2.6/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-06 14:26:16.311028 rockai_cli_app-0.2.6/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-05-06 14:26:16.311129 rockai_cli_app-0.2.6/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-05-06 14:26:16.311319 rockai_cli_app-0.2.6/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8718 2024-05-06 14:26:16.311504 rockai_cli_app-0.2.6/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:26:16.311559 rockai_cli_app-0.2.6/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      413 2024-05-30 07:37:18.396062 rockai_cli_app-0.2.6/rockai_cli_app/test.py
+-rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 rockai_cli_app-0.2.6/PKG-INFO
```

### Comparing `rockai_cli_app-0.2.4/pyproject.toml` & `rockai_cli_app-0.2.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.2.4"
-description = "For inference and training"
+version = "0.2.6"
+description = "Python SDK for RockAI.online"
 authors = ["RockAI <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
 rock = "rockai_cli_app.main:app"
```

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/__init__.py` & `rockai_cli_app-0.2.6/rockai_cli_app/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import os
-from typing import Iterator, Dict, Optional, Any, List, AsyncIterator
-import json
+from typing import Iterator, Dict, Optional, Any, List
 import requests
-from sseclient import SSEClient
 import time
 import httpx
 from httpx_sse import connect_sse
 import logging
 import asyncio
-from aiosseclient import aiosseclient
 from aiohttp_sse_client import client as sse_client
 import os
 import aiohttp
 
 logging.basicConfig(level=logging.DEBUG)
 
-
 # client for rock AI
 class Client:
 
-    def __init__(self, api_token=os.environ.get("ROCK_API_TOKEN")):
-        self.api_token = api_token
+    def __init__(self, api_token: str = None):
+        self.api_token = (
+            api_token if api_token is not None else os.environ.get("ROCK_API_TOKEN")
+        )
         # Local testing
         # self.predict_url = "http://localhost:8000/v1/predictions"
         # self.get_url = "http://localhost:8000/v1/predictions/{}"
         # self.cancel_url = "http://localhost:8000/v1/predictions/{}/cancel"
 
         # Production
         self.predict_url = "https://api.rockai.online/v1/predictions"
@@ -70,14 +68,15 @@
                 self.cancel_url.format(id), headers=headers
             ) as response:
                 response.raise_for_status()  # Raise an exception for HTTP errors
                 result = await response.json()
                 logging.info(result)
                 return result
 
+    # Stream output from a model, if model supports streaming like LLama3
     def stream(self, version: str, input: Optional[Dict[str, Any]] = None) -> Iterator:
         url = self.predict_url
 
         payload = {"version": version, "input": input, "stream": True}
 
         headers = {
             "Content-Type": "application/json",
@@ -101,14 +100,15 @@
                 ) as event_source:
                     try:
                         for sse in event_source.iter_sse():
                             yield sse.data
                     except Exception as e:
                         logging.error(str(e))
 
+    # Run a model and return the result from the model
     def run(
         self,
         version: str,
         input: Optional[Dict[str, Any]] = None,
         webhook: Optional[str] = None,
         webhook_events_filter: Optional[List[str]] = None,
     ) -> Any:
@@ -141,14 +141,15 @@
                     or get_result["data"]["status"] == "starting"
                 ):
                     time.sleep(1)
                     continue
                 else:
                     return get_result
 
+    # Stream output from a model, if model supports streaming like LLama3 (async version)
     async def stream_async(self, version: str, input: Optional[Dict[str, Any]] = None):
         url = self.predict_url
 
         payload = {"version": version, "input": input, "stream": True}
 
         headers = {
             "Content-Type": "application/json",
@@ -165,15 +166,15 @@
                     create_result["data"]["urls"]["stream"]
                 ) as event_source:
 
                     async for event in event_source:
                         yield event.data
                         if event.type == "done" and event.message == "done":
                             return
-
+    # Run a model and return the result from the model (Async version)
     async def run_async(
         self,
         version: str,
         input: Optional[Dict[str, Any]] = None,
         webhook: Optional[str] = None,
         webhook_events_filter: Optional[List[str]] = None,
     ):
@@ -204,7 +205,9 @@
                     get_result["data"]["status"] == "processing"
                     or get_result["data"]["status"] == "starting"
                 ):
                     await asyncio.sleep(1)
                     continue
                 else:
                     return get_result
+
+client = Client()
```

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/data_class.py` & `rockai_cli_app-0.2.6/rockai_cli_app/data_class.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.2.6/rockai_cli_app/docker/docker_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import requests
 from pathlib import Path
 import logging
 from rich.progress import Progress, SpinnerColumn, TextColumn
 import subprocess
+import uuid
 
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 logging.getLogger("docker").setLevel(logging.WARNING)
 
 
 def remove_some_libs(file_name,lib_to_be_deleted):
     try:
@@ -84,16 +85,16 @@
     docker_list.append(add_expose(port))
     if config_map['build']['python_requirements']:
         remove_some_libs(config_map['build']['python_requirements'],'tensorflow-metal')
         remove_some_libs(config_map['build']['python_requirements'],'tensorflow-macos')
         docker_list.append(add_run("pip install -r {} {}".format(config_map['build']['python_requirements'],"-i https://mirrors.aliyun.com/pypi/simple/")))
 
     docker_list.append(add_cmd("rock start"))
-    save_docker_file(docker_list)
-    subprocess.run(["docker", "build", "--platform", platform,"-t", tag, "."])
+    docker_file_name = save_docker_file(docker_list)
+    subprocess.run(["docker", "build", "--platform", platform,"-t", tag,"-f {}".format(docker_file_name), "."])
     # subprocess.run(["docker", "run", "--rm", tag])
         
 
 
 def tf_compat_matrix():
     json_data = [{"tf_version": "tensorflow-2.16.1", "python": "3.9-3.12", "cuDNN": "8.9", "CUDA": "12.3"},{"tf_version": "tensorflow-2.15.0", "python": "3.9-3.11", "cuDNN": "8.9", "CUDA": "12.2"}, {"tf_version": "tensorflow-2.14.0", "python": "3.9-3.11", "cuDNN": "8.7", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.13.0", "python": "3.8-3.11", "cuDNN": "8.6", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.12.0", "python": "3.8-3.11", "cuDNN": "8.6", "CUDA": "11.8"}, {"tf_version": "tensorflow-2.11.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.10.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.9.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.8.0", "python": "3.7-3.10", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.7.0", "python": "3.7-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.6.0", "python": "3.6-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.5.0", "python": "3.6-3.9", "cuDNN": "8.1", "CUDA": "11.2"}, {"tf_version": "tensorflow-2.4.0", "python": "3.6-3.8", "cuDNN": "8.0", "CUDA": "11.0"}, {"tf_version": "tensorflow-2.3.0", "python": "3.5-3.8", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.2.0", "python": "3.5-3.8", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.1.0", "python": "2.7,", "cuDNN": "7.6", "CUDA": "10.1"}, {"tf_version": "tensorflow-2.0.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.15.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.14.0", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.13.1", "python": "2.7,", "cuDNN": "7.4", "CUDA": "10.0"}, {"tf_version": "tensorflow_gpu-1.12.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.11.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.10.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.9.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.8.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.7.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.6.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.5.0", "python": "2.7,", "cuDNN": "7", "CUDA": "9"}, {"tf_version": "tensorflow_gpu-1.4.0", "python": "2.7,", "cuDNN": "6", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.3.0", "python": "2.7,", "cuDNN": "6", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.2.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.1.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}, {"tf_version": "tensorflow_gpu-1.0.0", "python": "2.7,", "cuDNN": "5.1", "CUDA": "8"}]
     return json_data
@@ -276,15 +277,17 @@
     return "COPY {} {}\n".format(src, dest)
 
 
 def add_env(env):
     return "ENV {}\n".format(env)
 
 
-def save_docker_file(cmd_list):
+def save_docker_file(cmd_list)->str:
     result = "".join(cmd_list)
     try:
-        with open(Path.cwd() / "Dockerfile", "w") as file:
+        suffix = uuid.uuid4().hex
+        with open(Path.cwd() / "Dockerfile{}".format(suffix), "w") as file:
             file.write(result)
-            print("String successfully written to Dockerfile")
+            print("String successfully written to Dockerfile{}".format(suffix))
+            return "Dockerfile{}".format(suffix)
     except Exception as e:
         print("An error occurred while writing to the file. Error: ", str(e))
```

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.2.6/rockai_cli_app/docker/torch_compat.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'insert': "[(0, OrderedDict([('torch_version', '2.3'), ('python', '>=3.8, <=3.11'), ('CUDA', "*

 * *           "'11.8'), ('cuDNN', '8.7')]))]"}*

```diff
@@ -1,12 +1,18 @@
 [
     {
         "CUDA": "11.8",
         "cuDNN": "8.7",
         "python": ">=3.8, <=3.11",
+        "torch_version": "2.3"
+    },
+    {
+        "CUDA": "11.8",
+        "cuDNN": "8.7",
+        "python": ">=3.8, <=3.11",
         "torch_version": "2.2"
     },
     {
         "CUDA": "11.8",
         "cuDNN": "8.7",
         "python": ">=3.8, <=3.11",
         "torch_version": "2.1"
```

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/main.py` & `rockai_cli_app-0.2.6/rockai_cli_app/rock.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 def callback():
     """
     Callback for the CLI app before any command
     """
     typer.echo("callback excuted")
 
 
-@app.command()
-def login():
-    """
-    Login using auth token
-    """
-    typer.echo("Login to Rock ai")
+# @app.command()
+# def login():
+#     """
+#     Login using auth token
+#     """
+#     typer.echo("Login to Rock ai")
 
 
 @app.command()
 def init():
     file = open('rock.yaml', 'w')
     file.close()
     file = open('predict.py', 'w')
```

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.2.6/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/server/http.py` & `rockai_cli_app-0.2.6/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.2.6/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/server/types.py` & `rockai_cli_app-0.2.6/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.2.4/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.2.6/rockai_cli_app/server/utils.py`

 * *Files identical despite different names*

