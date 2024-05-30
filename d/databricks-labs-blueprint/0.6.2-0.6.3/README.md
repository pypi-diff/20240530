# Comparing `tmp/databricks_labs_blueprint-0.6.2.tar.gz` & `tmp/databricks_labs_blueprint-0.6.3.tar.gz`

## Comparing `databricks_labs_blueprint-0.6.2.tar` & `databricks_labs_blueprint-0.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__main__.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/cli.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/commands.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/entrypoint.py
--rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installation.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installer.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/limiter.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/logger.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/parallel.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/py.typed
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/tui.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/upgrades.py
--rw-r--r--   0        0        0    14116 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/wheels.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/LICENSE
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/NOTICE
--rw-r--r--   0        0        0    45992 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/README.md
--rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    46795 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/__main__.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/cli.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/commands.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/entrypoint.py
+-rw-r--r--   0        0        0    42934 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/installation.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/installer.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/limiter.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/logger.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/parallel.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/py.typed
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/tui.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/upgrades.py
+-rw-r--r--   0        0        0    14116 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/wheels.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/LICENSE
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/NOTICE
+-rw-r--r--   0        0        0    45992 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/README.md
+-rw-r--r--   0        0        0    26290 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    46795 2020-02-02 00:00:00.000000 databricks_labs_blueprint-0.6.3/PKG-INFO
```

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/__main__.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/cli.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Baseline CLI for Databricks Labs projects."""
 
 import functools
 import inspect
 import json
 import logging
+import types
 from collections.abc import Callable
 from dataclasses import dataclass
 
 from databricks.sdk import AccountClient, WorkspaceClient
 
 from databricks.labs.blueprint.entrypoint import get_logger, run_main
 from databricks.labs.blueprint.tui import Prompts
@@ -36,15 +37,18 @@
                 return param.name
         return None
 
     def get_argument_type(self, argument_name: str) -> str | None:
         sig = inspect.signature(self.fn)
         if argument_name not in sig.parameters:
             return None
-        return sig.parameters[argument_name].annotation.__name__
+        annotation = sig.parameters[argument_name].annotation
+        if isinstance(annotation, types.UnionType):
+            return str(annotation)
+        return annotation.__name__
 
 
 class App:
     def __init__(self, __file: str):
         self._mapping: dict[str, Command] = {}
         self._logger = get_logger(__file)
         self._product_info = ProductInfo(__file)
```

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/commands.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/commands.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/entrypoint.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/entrypoint.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installation.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/installation.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/installer.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/installer.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/limiter.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/limiter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/logger.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/logger.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/parallel.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/parallel.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/tui.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/tui.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/upgrades.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/upgrades.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/databricks/labs/blueprint/wheels.py` & `databricks_labs_blueprint-0.6.3/databricks/labs/blueprint/wheels.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/.gitignore` & `databricks_labs_blueprint-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/LICENSE` & `databricks_labs_blueprint-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/README.md` & `databricks_labs_blueprint-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/pyproject.toml` & `databricks_labs_blueprint-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_blueprint-0.6.2/PKG-INFO` & `databricks_labs_blueprint-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-blueprint
-Version: 0.6.2
+Version: 0.6.3
 Summary: Common libraries for Databricks Labs
 Project-URL: Issues, https://github.com/databrickslabs/blueprint/issues
 Project-URL: Source, https://github.com/databrickslabs/blueprint
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
 Classifier: Development Status :: 3 - Alpha
```

