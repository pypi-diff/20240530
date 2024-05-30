# Comparing `tmp/tuneapi-0.4.1.tar.gz` & `tmp/tuneapi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.4.1.tar", max compression
+gzip compressed data, was "tuneapi-0.4.2.tar", max compression
```

## Comparing `tuneapi-0.4.1.tar` & `tuneapi-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.4.1/LICENSE
--rw-r--r--   0        0        0      184 2024-05-13 05:27:01.434096 tuneapi-0.4.1/README.md
--rw-r--r--   0        0        0      769 2024-05-23 17:10:07.027196 tuneapi-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       78 2024-05-23 17:10:01.975687 tuneapi-0.4.1/tuneapi/__init__.py
--rw-r--r--   0        0        0      351 2024-05-21 04:32:29.030680 tuneapi-0.4.1/tuneapi/__main__.py
--rw-r--r--   0        0        0     6012 2024-05-21 06:57:23.060317 tuneapi-0.4.1/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     8597 2024-05-23 09:49:53.188434 tuneapi-0.4.1/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     8131 2024-05-23 12:07:04.181995 tuneapi-0.4.1/tuneapi/apis/model_gemini.py
--rw-r--r--   0        0        0     5897 2024-05-23 09:48:23.978502 tuneapi-0.4.1/tuneapi/apis/model_groq.py
--rw-r--r--   0        0        0     6065 2024-05-23 09:48:52.204641 tuneapi-0.4.1/tuneapi/apis/model_mistral.py
--rw-r--r--   0        0        0     7729 2024-05-23 09:49:19.313038 tuneapi-0.4.1/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     6278 2024-05-23 09:49:47.799288 tuneapi-0.4.1/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0     3714 2024-05-21 06:57:20.143110 tuneapi-0.4.1/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      220 2024-05-23 09:12:22.307150 tuneapi-0.4.1/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    17546 2024-05-23 12:37:01.286725 tuneapi-0.4.1/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1247 2024-05-21 04:49:29.146672 tuneapi-0.4.1/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0     9846 2024-05-21 05:00:43.950665 tuneapi-0.4.1/tuneapi/utils/code.py
--rw-r--r--   0        0        0      345 2024-05-12 08:34:03.731467 tuneapi-0.4.1/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2987 2024-05-12 08:34:17.889266 tuneapi-0.4.1/tuneapi/utils/fs.py
--rw-r--r--   0        0        0     1024 2024-05-13 05:28:35.812363 tuneapi-0.4.1/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33527 2024-05-12 08:34:20.152416 tuneapi-0.4.1/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3778 2024-05-12 08:34:28.068601 tuneapi-0.4.1/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2131 2024-05-12 08:34:30.772098 tuneapi-0.4.1/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4883 2024-05-12 08:34:35.753162 tuneapi-0.4.1/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0     1220 2024-05-12 08:34:38.734730 tuneapi-0.4.1/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2496 2024-05-12 08:34:41.922150 tuneapi-0.4.1/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5838 2024-05-12 08:34:44.657582 tuneapi-0.4.1/tuneapi/utils/subway.py
--rw-r--r--   0        0        0     1430 2024-05-13 05:28:59.510065 tuneapi-0.4.1/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 tuneapi-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.4.2/LICENSE
+-rw-r--r--   0        0        0      184 2024-05-13 05:27:01.434096 tuneapi-0.4.2/README.md
+-rw-r--r--   0        0        0      769 2024-05-30 07:26:47.495509 tuneapi-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-05-30 07:26:44.643294 tuneapi-0.4.2/tuneapi/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-21 04:32:29.030680 tuneapi-0.4.2/tuneapi/__main__.py
+-rw-r--r--   0        0        0     6012 2024-05-21 06:57:23.060317 tuneapi-0.4.2/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     8597 2024-05-23 09:49:53.188434 tuneapi-0.4.2/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8131 2024-05-23 12:07:04.181995 tuneapi-0.4.2/tuneapi/apis/model_gemini.py
+-rw-r--r--   0        0        0     5897 2024-05-30 06:57:07.159092 tuneapi-0.4.2/tuneapi/apis/model_groq.py
+-rw-r--r--   0        0        0     6065 2024-05-30 06:57:07.179854 tuneapi-0.4.2/tuneapi/apis/model_mistral.py
+-rw-r--r--   0        0        0     7729 2024-05-30 07:03:30.383634 tuneapi-0.4.2/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     6479 2024-05-30 07:12:25.274042 tuneapi-0.4.2/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0     5393 2024-05-24 03:47:21.853954 tuneapi-0.4.2/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      220 2024-05-23 09:12:22.307150 tuneapi-0.4.2/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    18250 2024-05-30 07:03:24.320899 tuneapi-0.4.2/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1247 2024-05-21 04:49:29.146672 tuneapi-0.4.2/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0     9846 2024-05-21 05:00:43.950665 tuneapi-0.4.2/tuneapi/utils/code.py
+-rw-r--r--   0        0        0      345 2024-05-12 08:34:03.731467 tuneapi-0.4.2/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2987 2024-05-12 08:34:17.889266 tuneapi-0.4.2/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0     1024 2024-05-13 05:28:35.812363 tuneapi-0.4.2/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33527 2024-05-12 08:34:20.152416 tuneapi-0.4.2/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3778 2024-05-12 08:34:28.068601 tuneapi-0.4.2/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2131 2024-05-12 08:34:30.772098 tuneapi-0.4.2/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4883 2024-05-12 08:34:35.753162 tuneapi-0.4.2/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0     1220 2024-05-12 08:34:38.734730 tuneapi-0.4.2/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2496 2024-05-12 08:34:41.922150 tuneapi-0.4.2/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5838 2024-05-12 08:34:44.657582 tuneapi-0.4.2/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0     1430 2024-05-13 05:28:59.510065 tuneapi-0.4.2/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 tuneapi-0.4.2/PKG-INFO
```

### Comparing `tuneapi-0.4.1/LICENSE` & `tuneapi-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/pyproject.toml` & `tuneapi-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.4.1"
+version = "0.4.2"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.4.1/tuneapi/apis/__init__.py` & `tuneapi-0.4.2/tuneapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/apis/model_anthropic.py` & `tuneapi-0.4.2/tuneapi/apis/model_anthropic.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/apis/model_gemini.py` & `tuneapi-0.4.2/tuneapi/apis/model_gemini.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/apis/model_groq.py` & `tuneapi-0.4.2/tuneapi/apis/model_groq.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                         "role": "tool",
                         "tool_call_id": prev_tool_id,
                         "content": tu.to_json(_m, tight=True),
                     }
                 )
                 prev_tool_id = tu.get_random_string(5)  # reset tool id
             else:
-                raise Exception(f"Invalid message type: {m.role}")
+                raise Exception(f"Invalid message role: {m.role}")
 
         headers = {
             "Authorization": "Bearer " + token,
             "Content-Type": "application/json",
         }
         return headers, final_messages
```

### Comparing `tuneapi-0.4.1/tuneapi/apis/model_mistral.py` & `tuneapi-0.4.2/tuneapi/apis/model_mistral.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                         "role": "tool",
                         "tool_call_id": prev_tool_id,
                         "content": tu.to_json(_m, tight=True),
                     }
                 )
                 prev_tool_id = tu.get_random_string(5)  # reset tool id
             else:
-                raise Exception(f"Invalid message type: {m.role}")
+                raise Exception(f"Invalid message role: {m.role}")
 
         headers = {
             "Authorization": "Bearer " + token,
             "Content-Type": "application/json",
         }
         return headers, final_messages
```

### Comparing `tuneapi-0.4.1/tuneapi/apis/model_openai.py` & `tuneapi-0.4.2/tuneapi/apis/model_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                         "role": "tool",
                         "tool_call_id": prev_tool_id,
                         "content": tu.to_json(_m, tight=True),
                     }
                 )
                 prev_tool_id = tu.get_random_string(5)  # reset tool id
             else:
-                raise Exception(f"Invalid message type: {m.role}")
+                raise Exception(f"Invalid message role: {m.role}")
 
         headers = self._process_header(token)
         return headers, final_messages
 
     def _process_header(self, token: Optional[str] = None):
         return {
             "Authorization": "Bearer " + (token or self.openai_api_token),
```

### Comparing `tuneapi-0.4.1/tuneapi/apis/model_tune.py` & `tuneapi-0.4.2/tuneapi/apis/model_tune.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                         "role": "tool",
                         "tool_call_id": prev_tool_id,
                         "content": tu.to_json(_m, tight=True),
                     }
                 )
                 prev_tool_id = tu.get_random_string(5)  # reset tool id
             else:
-                raise Exception(f"Invalid message type: {m.role}")
+                raise Exception(f"Invalid message role: {m.role}")
 
         headers = {
             "Authorization": token,
             "Content-Type": "application/json",
         }
         if self.tune_org_id:
             headers["X-Org-Id"] = self.tune_org_id
@@ -127,19 +127,24 @@
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
         timeout=(5, 60),
         raw: bool = False,
         debug: bool = False,
     ):
+        model = model or self.tune_model_id
+        if not model:
+            raise Exception(
+                "Tune Model ID not found. Please set TUNEAPI_MODEL environment variable or pass through function"
+            )
         headers, messages = self._process_input(chats, token)
         data = {
             "temperature": temperature,
             "messages": messages,
-            "model": model or self.tune_model_id,
+            "model": model,
             "stream": True,
             "max_tokens": max_tokens,
         }
         if isinstance(chats, tt.Thread):
             data["tools"] = [
                 {"type": "function", "function": x.to_dict()} for x in chats.tools
             ]
```

### Comparing `tuneapi-0.4.1/tuneapi/types/chats.py` & `tuneapi-0.4.2/tuneapi/types/chats.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import json
 import random
 from functools import partial
 from collections.abc import Iterable
 from typing import Dict, List, Any, Tuple, Optional, Generator, Union
 
+import tuneapi.utils as tu
 from tuneapi.utils import to_json, get_random_string, logger, from_json
 
 
 class Tool:
 
     class Prop:
         def __init__(
@@ -104,23 +105,29 @@
         "function_call": FUNCTION_CALL,
         "function-call": FUNCTION_CALL,
         "function_resp": FUNCTION_RESP,
         "function-resp": FUNCTION_RESP,
     }
 
     # start initialization here
-    def __init__(self, value: str | float | List[Dict[str, Any]], role: str, **kwargs):
+    def __init__(
+        self,
+        value: str | float | List[Dict[str, Any]],
+        role: str,
+        id: str = None,
+        **kwargs,
+    ):
         if role not in self.KNOWN_ROLES:
             raise ValueError(f"Unknown role: {role}. Update dictionary `KNOWN_ROLES`")
         if value is None:
             raise ValueError("value cannot be None")
 
-        self.role = role
+        self.role = self.KNOWN_ROLES[role]
         self.value = value
-        self._unq_value = get_random_string(6)
+        self.id = id or tu.get_snowflake()
         self.metadata = kwargs
 
     def __str__(self) -> str:
         try:
             idx = max(os.get_terminal_size().columns - len(self.role) - 40, 10)
         except OSError:
             idx = 50
@@ -144,20 +151,22 @@
         self,
         format: Optional[str] = None,
         meta: bool = False,
     ):  #  ft: bool = False
         """
         if format == `ft` then export to following format: `{"from": "system/human/gpt", "value": "..."}`
         elif format == `api` then `{"role": "system/user/assistant", "content": [{"type": "text", "text": {"value": "..."}]}`
+        elif format == `full` then `{"id": 1234421123, "role": "system/user/assistant", "content": [{"type": "text", "text": {"value": "..."}]}`
         else export to following format: `{"role": "system/user/assistant", "content": "..."}`
         """
         role = self.role
 
         ft = format == "ft"
-        api = format == "api"
+        api = format in ["api", "full"]
+        full = format == "full"
 
         if not ft:
             if self.role == self.HUMAN:
                 role = "user"
             elif self.role == self.GPT:
                 role = "assistant"
 
@@ -173,14 +182,17 @@
             chat_message["content"] = [{"type": "text", "text": {"value": self.value}}]
         else:
             chat_message["content"] = self.value
 
         if meta:
             chat_message["metadata"] = self.metadata
 
+        if full:
+            chat_message["id"] = self.id
+
         return chat_message
 
     @classmethod
     def from_dict(cls, data):
         return cls(
             value=data.get("value") or data.get("content"),
             role=data.get("from") or data.get("role"),
@@ -315,14 +327,27 @@
     def add(self, message: Message):
         self.chats.append(message)
 
     def append(self, message: Message):
         self.chats.append(message)
 
 
+class ThreadTree:
+    """This is the tree representation of a thread, where each leaf is a Message object."""
+
+    def __init__(
+        self,
+        message: Message,
+        parent_message: Message,
+    ):
+        self.children = []
+        self.parent_id = parent_message.id or tu.get_snowflake()
+        self.id = message.id or tu.get_snowflake()
+
+
 # these are the classes that we use for tune datasets from r-stack
 
 
 class ThreadsList(list):
     """This class implements some basic container methods for a list of Chat objects"""
 
     def __init__(self):
```

### Comparing `tuneapi-0.4.1/tuneapi/utils/__init__.py` & `tuneapi-0.4.2/tuneapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/code.py` & `tuneapi-0.4.2/tuneapi/utils/code.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/fs.py` & `tuneapi-0.4.2/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/logger.py` & `tuneapi-0.4.2/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/mime.py` & `tuneapi-0.4.2/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/misc.py` & `tuneapi-0.4.2/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/networking.py` & `tuneapi-0.4.2/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/parallel.py` & `tuneapi-0.4.2/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/randomness.py` & `tuneapi-0.4.2/tuneapi/utils/randomness.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/serdeser.py` & `tuneapi-0.4.2/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/subway.py` & `tuneapi-0.4.2/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/tuneapi/utils/terminal.py` & `tuneapi-0.4.2/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.1/PKG-INFO` & `tuneapi-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: MIT
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

