# Comparing `tmp/databricks_genai-1.0.2.tar.gz` & `tmp/databricks_genai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_genai-1.0.2.tar", last modified: Tue May 14 23:39:04 2024, max compression
+gzip compressed data, was "databricks_genai-1.0.3.tar", last modified: Tue May 28 22:44:45 2024, max compression
```

## Comparing `databricks_genai-1.0.2.tar` & `databricks_genai-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.227518 databricks_genai-1.0.2/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1757 2024-05-14 23:39:04.227205 databricks_genai-1.0.2/PKG-INFO
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      274 2024-03-05 23:56:49.000000 databricks_genai-1.0.2/README.md
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.215484 databricks_genai-1.0.2/databricks/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      350 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/__init__.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.216243 databricks_genai-1.0.2/databricks/model_training/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      185 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/__init__.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.217481 databricks_genai-1.0.2/databricks/model_training/api/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     3170 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/config.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.218198 databricks_genai-1.0.2/databricks/model_training/api/engine/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      355 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/engine/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)    32800 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/engine/engine.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     6573 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/exceptions.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.221410 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      334 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     2639 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/cancel.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     8601 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/create.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     3611 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/delete.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1049 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/get.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     3328 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/get_events.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     4748 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/foundation_model/list.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)    17961 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/api/utils.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.223135 databricks_genai-1.0.2/databricks/model_training/types/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      131 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/types/__init__.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5516 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/types/common.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     5255 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/types/run_status.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     6109 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/types/train_config.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)    12102 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/databricks/model_training/types/training_run.py
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)       47 2024-05-14 23:36:37.000000 databricks_genai-1.0.2/databricks/model_training/version.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.223710 databricks_genai-1.0.2/databricks_genai/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      162 2024-05-14 23:36:18.000000 databricks_genai-1.0.2/databricks_genai/__init__.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.226073 databricks_genai-1.0.2/databricks_genai.egg-info/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1757 2024-05-14 23:39:04.000000 databricks_genai-1.0.2/databricks_genai.egg-info/PKG-INFO
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1270 2024-05-14 23:39:04.000000 databricks_genai-1.0.2/databricks_genai.egg-info/SOURCES.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)        1 2024-05-14 23:39:04.000000 databricks_genai-1.0.2/databricks_genai.egg-info/dependency_links.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      465 2024-05-14 23:39:04.000000 databricks_genai-1.0.2/databricks_genai.egg-info/requires.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)       28 2024-05-14 23:39:04.000000 databricks_genai-1.0.2/databricks_genai.egg-info/top_level.txt
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)    31118 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/pyproject.toml
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)       38 2024-05-14 23:39:04.227613 databricks_genai-1.0.2/setup.cfg
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)     1778 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/setup.py
-drwxr-xr-x   0 nicholas.garcia   (502) staff       (20)        0 2024-05-14 23:39:04.225480 databricks_genai-1.0.2/tests/
--rw-r--r--   0 nicholas.garcia   (502) staff       (20)      358 2024-05-14 23:32:27.000000 databricks_genai-1.0.2/tests/test_package.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.341648 databricks_genai-1.0.3/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     1757 2024-05-28 22:44:45.341185 databricks_genai-1.0.3/PKG-INFO
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      274 2024-02-22 00:58:56.000000 databricks_genai-1.0.3/README.md
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.329343 databricks_genai-1.0.3/databricks/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      350 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/__init__.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.330045 databricks_genai-1.0.3/databricks/model_training/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      185 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/__init__.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.331689 databricks_genai-1.0.3/databricks/model_training/api/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/__init__.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     3170 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/config.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.332405 databricks_genai-1.0.3/databricks/model_training/api/engine/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      355 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/engine/__init__.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)    32800 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/engine/engine.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     6573 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/exceptions.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.335047 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      334 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/__init__.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     2639 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/cancel.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     8601 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/create.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     3611 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/delete.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     1049 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/get.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     3328 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/get_events.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     5001 2024-05-28 22:39:16.000000 databricks_genai-1.0.3/databricks/model_training/api/foundation_model/list.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)    18744 2024-05-28 22:39:16.000000 databricks_genai-1.0.3/databricks/model_training/api/utils.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.336846 databricks_genai-1.0.3/databricks/model_training/types/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      131 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/types/__init__.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     5516 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/types/common.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     5255 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/types/run_status.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     6109 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/types/train_config.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)    12102 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks/model_training/types/training_run.py
+-rw-r--r--   0 jane.zhang   (502) staff       (20)       47 2024-05-28 22:39:27.000000 databricks_genai-1.0.3/databricks/model_training/version.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.337287 databricks_genai-1.0.3/databricks_genai/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      162 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/databricks_genai/__init__.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.339925 databricks_genai-1.0.3/databricks_genai.egg-info/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     1757 2024-05-28 22:44:45.000000 databricks_genai-1.0.3/databricks_genai.egg-info/PKG-INFO
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     1270 2024-05-28 22:44:45.000000 databricks_genai-1.0.3/databricks_genai.egg-info/SOURCES.txt
+-rw-r--r--   0 jane.zhang   (502) staff       (20)        1 2024-05-28 22:44:45.000000 databricks_genai-1.0.3/databricks_genai.egg-info/dependency_links.txt
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      465 2024-05-28 22:44:45.000000 databricks_genai-1.0.3/databricks_genai.egg-info/requires.txt
+-rw-r--r--   0 jane.zhang   (502) staff       (20)       28 2024-05-28 22:44:45.000000 databricks_genai-1.0.3/databricks_genai.egg-info/top_level.txt
+-rw-r--r--   0 jane.zhang   (502) staff       (20)    31118 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/pyproject.toml
+-rw-r--r--   0 jane.zhang   (502) staff       (20)       38 2024-05-28 22:44:45.341807 databricks_genai-1.0.3/setup.cfg
+-rw-r--r--   0 jane.zhang   (502) staff       (20)     1778 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/setup.py
+drwxr-xr-x   0 jane.zhang   (502) staff       (20)        0 2024-05-28 22:44:45.339218 databricks_genai-1.0.3/tests/
+-rw-r--r--   0 jane.zhang   (502) staff       (20)      358 2024-05-28 22:35:27.000000 databricks_genai-1.0.3/tests/test_package.py
```

### Comparing `databricks_genai-1.0.2/PKG-INFO` & `databricks_genai-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +28,15 @@
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
 Provides-Extra: notebook
 Requires-Dist: ipywidgets<9,>=8; extra == "notebook"
 Provides-Extra: all
-Requires-Dist: ipywidgets<9,>=8; extra == "all"
-Requires-Dist: pyright==1.1.256; extra == "all"
-Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: yapf>=0.40.0; extra == "all"
-Requires-Dist: packaging<23,>=21; extra == "all"
 Requires-Dist: pylint>=3.0.0; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: packaging<23,>=21; extra == "all"
+Requires-Dist: isort>=5.9.3; extra == "all"
 Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: pyright==1.1.256; extra == "all"
+Requires-Dist: ipywidgets<9,>=8; extra == "all"
+Requires-Dist: yapf>=0.40.0; extra == "all"
```

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/config.py` & `databricks_genai-1.0.3/databricks/model_training/api/config.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/engine/engine.py` & `databricks_genai-1.0.3/databricks/model_training/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/exceptions.py` & `databricks_genai-1.0.3/databricks/model_training/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/foundation_model/cancel.py` & `databricks_genai-1.0.3/databricks/model_training/api/foundation_model/cancel.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/foundation_model/create.py` & `databricks_genai-1.0.3/databricks/model_training/api/foundation_model/create.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/foundation_model/delete.py` & `databricks_genai-1.0.3/databricks/model_training/api/foundation_model/delete.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/foundation_model/get.py` & `databricks_genai-1.0.3/databricks/model_training/api/foundation_model/get.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/foundation_model/get_events.py` & `databricks_genai-1.0.3/databricks/model_training/api/foundation_model/get_events.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/foundation_model/list.py` & `databricks_genai-1.0.3/databricks/model_training/api/foundation_model/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import datetime
 from typing import List, Optional, Union
 
 from mcli.config import MCLIConfig
 
 from databricks.model_training.api.config import configure_request
 from databricks.model_training.api.engine import get_return_response, run_paginated_mapi_request
+from databricks.model_training.api.utils import parse_datetime
 from databricks.model_training.types import TrainingRun
 from databricks.model_training.types.common import ObjectList
 from databricks.model_training.types.run_status import RunStatus
 
 DEFAULT_LIMIT = 100
 
 QUERY_FUNCTION = 'getFinetunesPaginated'
@@ -110,17 +111,19 @@
     if training_runs:
         filters['name'] = {'in': [r.name if isinstance(r, TrainingRun) else r for r in training_runs]}
     if statuses:
         filters['status'] = {'in': [s.value if isinstance(s, RunStatus) else s for s in statuses]}
     if before or after:
         date_filters = {}
         if before:
-            date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
+            date_filters['lt'] = before.astimezone().isoformat() if isinstance(before,
+                                                                               datetime) else parse_datetime(before)
         if after:
-            date_filters['gte'] = after.astimezone().isoformat() if isinstance(after, datetime) else after
+            date_filters['gte'] = after.astimezone().isoformat() if isinstance(after,
+                                                                               datetime) else parse_datetime(after)
         filters['createdAt'] = date_filters
 
     variables = {
         VARIABLE_DATA_NAME: {
             'filters': filters,
             'includeDeleted': False,
             'limit': limit,
```

### Comparing `databricks_genai-1.0.2/databricks/model_training/api/utils.py` & `databricks_genai-1.0.3/databricks/model_training/api/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utils for model training API"""
 import json
 import os
 import re
 import uuid
+from datetime import datetime
 from typing import Any, List, Optional
 
 from databricks.sdk import WorkspaceClient
 from databricks.sdk import errors as dbx_errors
 from databricks.sdk.service.compute import ClusterDetails
 from datasets import get_dataset_split_names
 from mlflow import MlflowClient
@@ -346,7 +347,31 @@
             validate_uc_path(data_path, task_type)
         elif '/' in data_path:  # assume HF dataset TODO state this assumption in docs
             validate_hf_dataset(data_path)
         else:
             # if we have delta table input, we must also ensure the cluster input is valid
             validate_delta_table(data_path, data_path_type)
             validate_data_prep(data_prep_cluster)
+
+
+def parse_datetime(value: str) -> str:
+    """Parse a datetime string into an ISO format datetime string.
+
+    value:
+        value: Datetime string
+
+    Returns:
+        String of datetime in ISO format
+
+    Raises:
+        ValidationError: If arg is not a valid datetime format"""
+    for fmt in [
+            '%Y-%m-%d', '%m-%d-%Y', '%H:%M:%S.%f', '%H:%M:%S', '%Y-%m-%d %H:%M:%S.%f', '%m-%d-%Y %H:%M:%S.%f',
+            '%Y-%m-%d %H:%M:%S', '%m-%d-%Y %H:%M:%S'
+    ]:
+        try:
+            return datetime.strptime(value, fmt).astimezone().isoformat()
+        except ValueError:
+            pass
+
+    raise ValidationError(
+        'Invalid datetime format passed. Examples: \'2023-01-13\', \'01-12-2023, 5:32:23.34\', \'2023-12-30 05:34:23\'')
```

### Comparing `databricks_genai-1.0.2/databricks/model_training/types/common.py` & `databricks_genai-1.0.3/databricks/model_training/types/common.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/types/run_status.py` & `databricks_genai-1.0.3/databricks/model_training/types/run_status.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/types/train_config.py` & `databricks_genai-1.0.3/databricks/model_training/types/train_config.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks/model_training/types/training_run.py` & `databricks_genai-1.0.3/databricks/model_training/types/training_run.py`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/databricks_genai.egg-info/PKG-INFO` & `databricks_genai-1.0.3/databricks_genai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-genai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interact with the Databricks Generative AI APIs in python
 Home-page: https://docs.mosaicml.com/projects/mcli/en/latest/finetuning/finetuning.html
 Author: Databricks
 Author-email: genai-eng-team@databricks.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,15 +28,15 @@
 Requires-Dist: pylint>=3.0.0; extra == "dev"
 Requires-Dist: pyright==1.1.256; extra == "dev"
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: yapf>=0.40.0; extra == "dev"
 Provides-Extra: notebook
 Requires-Dist: ipywidgets<9,>=8; extra == "notebook"
 Provides-Extra: all
-Requires-Dist: ipywidgets<9,>=8; extra == "all"
-Requires-Dist: pyright==1.1.256; extra == "all"
-Requires-Dist: isort>=5.9.3; extra == "all"
-Requires-Dist: yapf>=0.40.0; extra == "all"
-Requires-Dist: packaging<23,>=21; extra == "all"
 Requires-Dist: pylint>=3.0.0; extra == "all"
-Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: packaging<23,>=21; extra == "all"
+Requires-Dist: isort>=5.9.3; extra == "all"
 Requires-Dist: pytest>=7.4.0; extra == "all"
+Requires-Dist: pre-commit>=2.17.0; extra == "all"
+Requires-Dist: pyright==1.1.256; extra == "all"
+Requires-Dist: ipywidgets<9,>=8; extra == "all"
+Requires-Dist: yapf>=0.40.0; extra == "all"
```

### Comparing `databricks_genai-1.0.2/databricks_genai.egg-info/SOURCES.txt` & `databricks_genai-1.0.3/databricks_genai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/pyproject.toml` & `databricks_genai-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_genai-1.0.2/setup.py` & `databricks_genai-1.0.3/setup.py`

 * *Files identical despite different names*

