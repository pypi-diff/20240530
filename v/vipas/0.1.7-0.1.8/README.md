# Comparing `tmp/vipas-0.1.7.tar.gz` & `tmp/vipas-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.1.7.tar", last modified: Thu May 30 07:00:51 2024, max compression
+gzip compressed data, was "vipas-0.1.8.tar", last modified: Thu May 30 08:05:44 2024, max compression
```

## Comparing `vipas-0.1.7.tar` & `vipas-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.7/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      381 2024-05-30 07:00:51.151590 vipas-0.1.7/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.7/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.7/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-30 07:00:51.151590 vipas-0.1.7/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1286 2024-05-30 07:00:05.000000 vipas-0.1.7/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.7/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.7/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3270 2024-05-30 06:56:34.000000 vipas-0.1.7/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.7/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2272 2024-05-23 12:40:14.000000 vipas-0.1.7/vipas/error_suggestions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3665 2024-05-30 06:48:54.000000 vipas-0.1.7/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6953 2024-05-30 06:52:00.000000 vipas-0.1.7/vipas/model.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2463 2024-05-22 14:37:58.000000 vipas-0.1.7/vipas/vipas_logger.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 07:00:51.151590 vipas-0.1.7/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      381 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      357 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       71 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-30 07:00:51.000000 vipas-0.1.7/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 08:05:44.149808 vipas-0.1.8/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.8/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      381 2024-05-30 08:05:44.149808 vipas-0.1.8/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.8/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.8/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-30 08:05:44.149808 vipas-0.1.8/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1286 2024-05-30 08:04:53.000000 vipas-0.1.8/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 08:05:44.145808 vipas-0.1.8/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.8/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 08:05:44.145808 vipas-0.1.8/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.8/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3270 2024-05-30 06:56:34.000000 vipas-0.1.8/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.8/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2272 2024-05-23 12:40:14.000000 vipas-0.1.8/vipas/error_suggestions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3665 2024-05-30 06:48:54.000000 vipas-0.1.8/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6969 2024-05-30 07:58:49.000000 vipas-0.1.8/vipas/model.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2463 2024-05-22 14:37:58.000000 vipas-0.1.8/vipas/vipas_logger.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-30 08:05:44.145808 vipas-0.1.8/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      381 2024-05-30 08:05:44.000000 vipas-0.1.8/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      357 2024-05-30 08:05:44.000000 vipas-0.1.8/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-30 08:05:44.000000 vipas-0.1.8/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       71 2024-05-30 08:05:44.000000 vipas-0.1.8/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-30 08:05:44.000000 vipas-0.1.8/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.1.7/LICENSE.md` & `vipas-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/README.md` & `vipas-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/setup.py` & `vipas-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
```

### Comparing `vipas-0.1.7/test/test_model_client.py` & `vipas-0.1.8/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/vipas/__init__.py` & `vipas-0.1.8/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/vipas/_rest.py` & `vipas-0.1.8/vipas/_rest.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/vipas/config.py` & `vipas-0.1.8/vipas/config.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/vipas/error_suggestions.py` & `vipas-0.1.8/vipas/error_suggestions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/vipas/exceptions.py` & `vipas-0.1.8/vipas/exceptions.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.7/vipas/model.py` & `vipas-0.1.8/vipas/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   
   For more information, contact Vipas.AI at legal@vipas.ai
 
 """  # noqa: E501
 import os
 import pybreaker
 import json
+import asyncio
 from typing import Tuple, Optional, List, Dict, Any
 from pydantic import Field, StrictStr
 from typing_extensions import Annotated
 from ratelimit import limits, sleep_and_retry
 
 from vipas.config import Config
 from vipas import _rest
@@ -59,15 +60,15 @@
             self.rate_limit = limits(calls=20, period=60)  # 20 calls per minute
         
         # Apply decorators dynamically
         self.predict = self.breaker(self.predict)
         self.predict = self.rate_limit(self.predict)
         self.predict = sleep_and_retry(self.predict)
 
-    async def predict(
+    def predict(
         self,
         model_id: Annotated[StrictStr, Field(description="Unique identifier for the model from which the prediction is requested")],
         input_data: Annotated[Any, Field(description="Input for the prediction")],
     ) -> dict:
         """
             Get Model Prediction
 
@@ -81,17 +82,17 @@
         self._validate_input_data_size(input_data)
 
         _param = self._predict_serialize(
             model_id=model_id,
             input_data=input_data
         )
 
-        response_data = await self._call_api(
+        response_data = asyncio.run(self._call_api(
             *_param,
-        )
+        ))
 
         return response_data
 
 
     def _predict_serialize(
         self,
         model_id,
```

### Comparing `vipas-0.1.7/vipas/vipas_logger.py` & `vipas-0.1.8/vipas/vipas_logger.py`

 * *Files identical despite different names*

