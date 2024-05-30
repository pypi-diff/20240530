# Comparing `tmp/corebridge-0.2.6.tar.gz` & `tmp/corebridge-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.2.6.tar", last modified: Mon May 27 10:15:06 2024, max compression
+gzip compressed data, was "corebridge-0.2.7.tar", last modified: Thu May 30 10:01:43 2024, max compression
```

## Comparing `corebridge-0.2.6.tar` & `corebridge-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-27 10:15:06.835107 corebridge-0.2.6/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.6/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.6/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-27 10:15:06.835107 corebridge-0.2.6/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)     2417 2024-05-27 09:35:23.000000 corebridge-0.2.6/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-27 10:15:06.835107 corebridge-0.2.6/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-27 10:14:49.000000 corebridge-0.2.6/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-27 10:14:49.000000 corebridge-0.2.6/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     4653 2024-05-27 10:14:49.000000 corebridge-0.2.6/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     4377 2024-05-27 10:14:49.000000 corebridge-0.2.6/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-27 10:15:06.835107 corebridge-0.2.6/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-27 10:15:06.000000 corebridge-0.2.6/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-27 10:15:06.000000 corebridge-0.2.6/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-27 10:15:06.000000 corebridge-0.2.6/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-27 10:15:06.000000 corebridge-0.2.6/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.6/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      287 2024-05-27 10:15:06.000000 corebridge-0.2.6/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-27 10:15:06.000000 corebridge-0.2.6/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1208 2024-05-27 10:14:59.000000 corebridge-0.2.6/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-27 10:15:06.835107 corebridge-0.2.6/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.6/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:01:43.245618 corebridge-0.2.7/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.7/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.7/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-30 10:01:43.245618 corebridge-0.2.7/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     2417 2024-05-27 09:35:23.000000 corebridge-0.2.7/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:01:43.245618 corebridge-0.2.7/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     5133 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4377 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:01:43.245618 corebridge-0.2.7/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.7/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      287 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1208 2024-05-30 09:54:45.000000 corebridge-0.2.7/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-30 10:01:43.245618 corebridge-0.2.7/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.7/setup.py
```

### Comparing `corebridge-0.2.6/LICENSE` & `corebridge-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.6/PKG-INFO` & `corebridge-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.6
+Version: 0.2.7
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.6/README.md` & `corebridge-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.6/corebridge/_modidx.py` & `corebridge-0.2.7/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.6/corebridge/aicorebridge.py` & `corebridge-0.2.7/corebridge/aicorebridge.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # %% auto 0
 __all__ = ['syslog', 'AICoreModule']
 
 # %% ../nbs/01_aicorebridge.ipynb 4
 import typing
 import logging
+import traceback
 import inspect
 import datetime
 import json
 import pandas as pd
 import numpy as np
 
 from fastcore.basics import patch_to, patch
@@ -33,21 +34,23 @@
 @patch
 def __init__(self:AICoreModule, 
              processor:typing.Callable, # data processing function
              save_dir:str, # path where the module can keep files 
              assets_dir:str,
              *args, **kwargs):
     
-    self.init_time = datetime.datetime.utcnow()
-    self.save_dir   = save_dir
-    self.assets_dir = assets_dir
+    self.init_time = datetime.datetime.now(datetime.UTC)
     self._init_processor(processor)
 
     self.init_args = args
-    self.init_kwargs = kwargs
+    self.init_kwargs = dict(
+        **kwargs,
+        assets_dir=assets_dir,
+        save_dir=save_dir
+    )
 
 
 
 # %% ../nbs/01_aicorebridge.ipynb 9
 @patch
 def _init_processor(
         self:AICoreModule, 
@@ -58,26 +61,28 @@
     self.processor_signature = inspect.signature(self.processor)
     self.processor_params = dict(self.processor_signature.parameters)
     self.return_param = self.processor_params.pop('return', None)
     self.data_param, *self.call_params = list(self.processor_params.keys())
 
 
 # %% ../nbs/01_aicorebridge.ipynb 10
+# can be overloaded
 @patch
 def call_processor(self:AICoreModule, calldata, **callargs):
     return self.processor(calldata, **callargs)
 
 
-# %% ../nbs/01_aicorebridge.ipynb 11
+# %% ../nbs/01_aicorebridge.ipynb 12
 @patch
 def infer(self:AICoreModule, data:dict, *_, **kwargs):
     try:
 
         msg=[
-            f"{self.processor.__name__}({self.processor_signature})",
+            f"Startup time: {self.init_time.isoformat()}",
+            f"{self.processor.__name__}({self.processor_signature})",             
             f"init_args: {self.init_args}, init_kwargs: {self.init_kwargs}",
         ]
 
         lastSeen = kwargs.pop('lastSeen', False)
         recordformat = kwargs.pop('format', "records").lower()
         reversed = kwargs.pop('reversed', False)
         timezone = kwargs.get('timezone', 'UTC')
@@ -104,37 +109,50 @@
             'data': timeseries_dataframe_to_datadict(
                 result if not lastSeen else result[-1:],
                 recordformat=recordformat,
                 timezone=timezone,
                 reversed=reversed)
         }
     except Exception as err:
+        msg.append(''.join(traceback.format_exception(None, err, err.__traceback__)))
+        syslog.exception(f"Exception {str(err)} in infer()")
         return {
             'msg': f"Unexpected {err=}, {type(err)=}",
             'data': []
         }
 
 
-# %% ../nbs/01_aicorebridge.ipynb 12
+# %% ../nbs/01_aicorebridge.ipynb 14
 @patch
 def get_callargs(self:AICoreModule, **kwargs):
     "Get arguments for the processor call"
 
     # Remove null / None values
     kwargs = {k:v for k,v in kwargs.items() if v is not None}
     
     metadata = kwargs.pop('metadata', {}) # TODO: historic metadata
 
     return {
-        K:self.processor_signature.parameters[K].annotation(kwargs.get(K,metadata.get(K, self.init_kwargs.get(K, self.processor_signature.parameters[K].default))))
+        K:self.processor_signature.parameters[K].annotation(
+            kwargs.get(
+                K,
+                metadata.get(
+                    K, 
+                    self.init_kwargs.get(
+                        K, 
+                        self.processor_signature.parameters[K].default
+                    )
+                )
+            )
+        )
         for K in self.call_params
     }
 
 
-# %% ../nbs/01_aicorebridge.ipynb 13
+# %% ../nbs/01_aicorebridge.ipynb 15
 @patch
 def get_call_data(
         self:AICoreModule, 
         data:dict, 
         recordformat='records', 
         timezone='UTC', 
         reversed=False):
```

### Comparing `corebridge-0.2.6/corebridge/core.py` & `corebridge-0.2.7/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.6/corebridge.egg-info/PKG-INFO` & `corebridge-0.2.7/corebridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.6
+Version: 0.2.7
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.6/settings.ini` & `corebridge-0.2.7/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.2.6
+version = 0.2.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
```

### Comparing `corebridge-0.2.6/setup.py` & `corebridge-0.2.7/setup.py`

 * *Files identical despite different names*

