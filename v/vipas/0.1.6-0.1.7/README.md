# Comparing `tmp/vipas-0.1.6.tar.gz` & `tmp/vipas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.1.6.tar", last modified: Thu May 23 12:41:01 2024, max compression
+gzip compressed data, was "vipas-0.1.7.tar", last modified: Thu May 30 07:00:51 2024, max compression
```

## Comparing `vipas-0.1.6.tar` & `vipas-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 12:41:01.663409 vipas-0.1.6/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.6/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-23 12:41:01.663409 vipas-0.1.6/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.6/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.6/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-23 12:41:01.667409 vipas-0.1.6/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-23 12:37:51.000000 vipas-0.1.6/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 12:41:01.663409 vipas-0.1.6/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.6/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 12:41:01.663409 vipas-0.1.6/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.6/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2381 2024-05-23 10:06:07.000000 vipas-0.1.6/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.6/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2272 2024-05-23 12:40:14.000000 vipas-0.1.6/vipas/error_suggestions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4046 2024-05-23 11:16:54.000000 vipas-0.1.6/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6870 2024-05-17 09:04:05.000000 vipas-0.1.6/vipas/model.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2463 2024-05-22 14:37:58.000000 vipas-0.1.6/vipas/vipas_logger.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-23 12:41:01.663409 vipas-0.1.6/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-23 12:41:01.000000 vipas-0.1.6/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      357 2024-05-23 12:41:01.000000 vipas-0.1.6/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-23 12:41:01.000000 vipas-0.1.6/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-23 12:41:01.000000 vipas-0.1.6/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-23 12:41:01.000000 vipas-0.1.6/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.7/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      381 2024-05-30 07:00:51.151590 vipas-0.1.7/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.7/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.7/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-30 07:00:51.151590 vipas-0.1.7/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1286 2024-05-30 07:00:05.000000 vipas-0.1.7/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.7/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.7/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3270 2024-05-30 06:56:34.000000 vipas-0.1.7/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.7/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2272 2024-05-23 12:40:14.000000 vipas-0.1.7/vipas/error_suggestions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3665 2024-05-30 06:48:54.000000 vipas-0.1.7/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6953 2024-05-30 06:52:00.000000 vipas-0.1.7/vipas/model.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2463 2024-05-22 14:37:58.000000 vipas-0.1.7/vipas/vipas_logger.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      381 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      357 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       71 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.1.6/LICENSE.md` & `vipas-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.6/README.md` & `vipas-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.6/setup.py` & `vipas-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
-    "streamlit"
+    "streamlit",
+    "httpx"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Python SDK for Vipas AI Platform",
     author="Vipas Team",
```

### Comparing `vipas-0.1.6/test/test_model_client.py` & `vipas-0.1.7/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.6/vipas/__init__.py` & `vipas-0.1.7/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.6/vipas/config.py` & `vipas-0.1.7/vipas/config.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.6/vipas/error_suggestions.py` & `vipas-0.1.7/vipas/error_suggestions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.6/vipas/exceptions.py` & `vipas-0.1.7/vipas/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,39 +27,33 @@
     """The base exception class for all VipasExceptions"""
 
 class ClientException(VipasException):
 
     def __init__(
         self, 
         status=None, 
-        reason=None, 
         http_resp=None,
         *,
         body: Optional[str] = None,
         data: Optional[Any] = None,
         suggested_actions: Optional[List[str]] = None,
     ) -> None:
         self.status = status
-        self.reason = reason
         self.body = body
         self.data = data
         self.suggested_actions = suggested_actions
-        self.headers = None
 
         if http_resp:
             if self.status is None:
                 self.status = http_resp.status
-            if self.reason is None:
-                self.reason = http_resp.reason
             if self.body is None:
                 try:
                     self.body = http_resp.data.decode('utf-8')
                 except Exception:
                     pass
-            self.headers = http_resp.getheaders()
 
     @classmethod
     def from_response(
         cls, 
         *, 
         http_resp, 
         body: Optional[str],
@@ -69,15 +63,14 @@
 
         # Fetch suggestions from the dictionary
         suggestions = ERROR_SUGGESTIONS.get(http_resp.status_code, {})
         suggested_actions = suggestions.get("suggested_actions")
 
         exception_args = {
             "status": http_resp.status_code,
-            "reason": http_resp.reason,
             "http_resp": http_resp,
             "body": body,
             "data": data,
             "suggested_actions": suggested_actions,
         }
 
         if http_resp.status_code == 400:
@@ -98,26 +91,23 @@
         if 500 <= http_resp.status_code <= 599:
             raise ConnectionException(**exception_args)
 
         raise ClientException(**exception_args)
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = f"({self.status})\nReason: {self.reason}\n"
+        error_message = f"({self.status})\n"
+
+        if self.data or self.body:
+            error_message += f"HTTP response body: {self.data or self.body}\n"
         
         if self.suggested_actions:
             error_message += "Suggested Actions:\n"
             for action in self.suggested_actions:
                 error_message += f"- {action}\n"
-        
-        if self.headers:
-            error_message += f"HTTP response headers: {self.headers}\n"
-
-        if self.data or self.body:
-            error_message += f"HTTP response body: {self.data or self.body}\n"
 
         return error_message
 
 class BadRequestException(ClientException):
     pass
 
 class NotFoundException(ClientException):
```

### Comparing `vipas-0.1.6/vipas/model.py` & `vipas-0.1.7/vipas/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   without the express prior written permission of Vipas.AI.
   
   For more information, contact Vipas.AI at legal@vipas.ai
 
 """  # noqa: E501
 import os
 import pybreaker
+import json
 from typing import Tuple, Optional, List, Dict, Any
 from pydantic import Field, StrictStr
 from typing_extensions import Annotated
 from ratelimit import limits, sleep_and_retry
 
 from vipas.config import Config
 from vipas import _rest
@@ -58,15 +59,15 @@
             self.rate_limit = limits(calls=20, period=60)  # 20 calls per minute
         
         # Apply decorators dynamically
         self.predict = self.breaker(self.predict)
         self.predict = self.rate_limit(self.predict)
         self.predict = sleep_and_retry(self.predict)
 
-    def predict(
+    async def predict(
         self,
         model_id: Annotated[StrictStr, Field(description="Unique identifier for the model from which the prediction is requested")],
         input_data: Annotated[Any, Field(description="Input for the prediction")],
     ) -> dict:
         """
             Get Model Prediction
 
@@ -80,15 +81,15 @@
         self._validate_input_data_size(input_data)
 
         _param = self._predict_serialize(
             model_id=model_id,
             input_data=input_data
         )
 
-        response_data = self._call_api(
+        response_data = await self._call_api(
             *_param,
         )
 
         return response_data
 
 
     def _predict_serialize(
@@ -151,15 +152,15 @@
 
         :param params: Parameters as dict or list of two-tuples
         :return: URL query string (e.g. a=Hello%20World&b=123)
         """
 
         return "&".join(["=".join(map(str, item)) for item in params])
 
-    def _call_api(
+    async def _call_api(
         self,
         method,
         url,
         header_params=None,
         body=None
     ) -> dict:
         """Makes the HTTP request (synchronous)
@@ -169,15 +170,15 @@
             placed in the request header.
         :param body: Request body.
         :return: dict of response data.
         """
 
         try:
             # perform request and return response
-            response_data = self.rest_client.request(
+            response_data = await self.rest_client.request(
                 method, url,
                 headers=header_params,
                 body=body
             )
 
         except ClientException as e:
             raise e
@@ -190,21 +191,24 @@
 
         :param input_data: The data to validate.
         :raises ClientException: If the input_data size is greater than 0.5 MB.
         """
         max_size_mb = 0.5
         max_size_bytes = max_size_mb * 1024 * 1024  # Convert MB to bytes
 
-        # Calculate the size of input_data assuming it's a string or bytes
         if isinstance(input_data, str):
-            input_size = len(input_data.encode('utf-8'))
+            input_size = len(input_data)
         elif isinstance(input_data, bytes):
             input_size = len(input_data)
+        elif isinstance(input_data, (list, dict)):
+            input_size = len(json.dumps(input_data))
         else:
-            raise ClientException(400, "Unsupported data type for input_data.")
+            # Convert other types to string and check their length
+            input_size = len(str(input_data))
+
 
         if input_size > max_size_bytes:
             raise ClientException(400, f"Payload size more than {max_size_mb} MB is not allowed.")
```

### Comparing `vipas-0.1.6/vipas/vipas_logger.py` & `vipas-0.1.7/vipas/vipas_logger.py`

 * *Files identical despite different names*

