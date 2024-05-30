# Comparing `tmp/yamx-0.1.7.tar.gz` & `tmp/yamx-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamx-0.1.7.tar", max compression
+gzip compressed data, was "yamx-0.1.8.tar", max compression
```

## Comparing `yamx-0.1.7.tar` & `yamx-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     9893 2023-04-11 11:37:11.485830 yamx-0.1.7/LICENSE
--rw-r--r--   0        0        0     2472 2024-01-31 08:53:43.088610 yamx-0.1.7/README.md
--rw-r--r--   0        0        0     1041 2024-02-13 17:29:57.385226 yamx-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       47 2024-01-13 12:12:01.417687 yamx-0.1.7/yamx/__init__.py
--rw-r--r--   0        0        0     1051 2024-02-13 18:17:21.679300 yamx-0.1.7/yamx/constants.py
--rw-r--r--   0        0        0      398 2024-01-13 12:12:01.418434 yamx-0.1.7/yamx/containers/__init__.py
--rw-r--r--   0        0        0     7102 2024-01-13 12:12:01.419274 yamx-0.1.7/yamx/containers/data.py
--rw-r--r--   0        0        0      131 2024-01-13 12:12:01.419697 yamx-0.1.7/yamx/containers/settings.py
--rw-r--r--   0        0        0     5681 2024-01-31 08:53:43.092127 yamx-0.1.7/yamx/extra.py
--rw-r--r--   0        0        0        0 2024-01-13 12:12:01.419999 yamx-0.1.7/yamx/jinja/__init__.py
--rw-r--r--   0        0        0     4221 2024-01-13 12:12:01.420488 yamx-0.1.7/yamx/jinja/condition.py
--rw-r--r--   0        0        0      169 2024-01-13 12:12:01.420913 yamx-0.1.7/yamx/loader/__init__.py
--rw-r--r--   0        0        0     3725 2024-01-13 12:12:01.421110 yamx-0.1.7/yamx/loader/grouper.py
--rw-r--r--   0        0        0     6253 2024-01-13 12:12:01.421406 yamx-0.1.7/yamx/loader/preprocessor.py
--rw-r--r--   0        0        0      637 2024-01-13 12:12:01.421592 yamx-0.1.7/yamx/loader/utils.py
--rw-r--r--   0        0        0      518 2024-01-13 12:12:01.422107 yamx-0.1.7/yamx/loader/validator.py
--rw-r--r--   0        0        0      244 2024-01-13 12:12:01.422457 yamx-0.1.7/yamx/representer/__init__.py
--rw-r--r--   0        0        0     9448 2024-01-13 12:12:01.422697 yamx-0.1.7/yamx/representer/common.py
--rw-r--r--   0        0        0      611 2024-01-13 12:12:01.422926 yamx-0.1.7/yamx/representer/conditional_map.py
--rw-r--r--   0        0        0      580 2024-01-13 12:12:01.423363 yamx-0.1.7/yamx/representer/conditional_seq.py
--rw-r--r--   0        0        0    18991 2024-02-13 18:17:10.213893 yamx-0.1.7/yamx/representer/rendering.py
--rw-r--r--   0        0        0     5877 2024-02-13 17:29:56.482558 yamx-0.1.7/yamx/yamx.py
--rw-r--r--   0        0        0    13229 1970-01-01 00:00:00.000000 yamx-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     9893 2023-04-11 11:37:11.485830 yamx-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2472 2024-01-31 08:53:43.088610 yamx-0.1.8/README.md
+-rw-r--r--   0        0        0     1041 2024-05-30 14:10:56.256531 yamx-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-01-13 12:12:01.417687 yamx-0.1.8/yamx/__init__.py
+-rw-r--r--   0        0        0     1051 2024-05-30 14:10:56.265956 yamx-0.1.8/yamx/constants.py
+-rw-r--r--   0        0        0      398 2024-01-13 12:12:01.418434 yamx-0.1.8/yamx/containers/__init__.py
+-rw-r--r--   0        0        0     7102 2024-01-13 12:12:01.419274 yamx-0.1.8/yamx/containers/data.py
+-rw-r--r--   0        0        0      131 2024-01-13 12:12:01.419697 yamx-0.1.8/yamx/containers/settings.py
+-rw-r--r--   0        0        0     5659 2024-05-30 14:10:56.274209 yamx-0.1.8/yamx/extra.py
+-rw-r--r--   0        0        0        0 2024-01-13 12:12:01.419999 yamx-0.1.8/yamx/jinja/__init__.py
+-rw-r--r--   0        0        0     4221 2024-01-13 12:12:01.420488 yamx-0.1.8/yamx/jinja/condition.py
+-rw-r--r--   0        0        0      169 2024-01-13 12:12:01.420913 yamx-0.1.8/yamx/loader/__init__.py
+-rw-r--r--   0        0        0     3725 2024-01-13 12:12:01.421110 yamx-0.1.8/yamx/loader/grouper.py
+-rw-r--r--   0        0        0     6253 2024-01-13 12:12:01.421406 yamx-0.1.8/yamx/loader/preprocessor.py
+-rw-r--r--   0        0        0      637 2024-01-13 12:12:01.421592 yamx-0.1.8/yamx/loader/utils.py
+-rw-r--r--   0        0        0      518 2024-01-13 12:12:01.422107 yamx-0.1.8/yamx/loader/validator.py
+-rw-r--r--   0        0        0      244 2024-01-13 12:12:01.422457 yamx-0.1.8/yamx/representer/__init__.py
+-rw-r--r--   0        0        0     9448 2024-01-13 12:12:01.422697 yamx-0.1.8/yamx/representer/common.py
+-rw-r--r--   0        0        0      611 2024-01-13 12:12:01.422926 yamx-0.1.8/yamx/representer/conditional_map.py
+-rw-r--r--   0        0        0      580 2024-01-13 12:12:01.423363 yamx-0.1.8/yamx/representer/conditional_seq.py
+-rw-r--r--   0        0        0    18991 2024-05-30 14:10:56.280543 yamx-0.1.8/yamx/representer/rendering.py
+-rw-r--r--   0        0        0      515 2024-05-30 14:10:56.281760 yamx-0.1.8/yamx/utils.py
+-rw-r--r--   0        0        0     5877 2024-02-13 17:29:56.482558 yamx-0.1.8/yamx/yamx.py
+-rw-r--r--   0        0        0    13280 1970-01-01 00:00:00.000000 yamx-0.1.8/PKG-INFO
```

### Comparing `yamx-0.1.7/LICENSE` & `yamx-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/README.md` & `yamx-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/pyproject.toml` & `yamx-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yamx"
-version = "0.1.7"
+version = "0.1.8"
 description = "YAML parser that supports jinja conditional expressions"
 
 license = "Apache-2.0"
 
 authors = [
     "Eduard Trott <eduard.trott@workday.com>"
 ]
```

### Comparing `yamx-0.1.7/yamx/constants.py` & `yamx-0.1.8/yamx/constants.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/containers/data.py` & `yamx-0.1.8/yamx/containers/data.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/extra.py` & `yamx-0.1.8/yamx/extra.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # not very supported pieces of functionality
 
 from dataclasses import dataclass
-from distutils.util import strtobool
 from typing import Any, Dict, Optional, Set
 
 from jinja2 import nodes
 
 from yamx.containers.data import (
     Condition,
     ConditionalData,
     ConditionalGroup,
     ConditionalMap,
     ConditionalSeq,
 )
 from yamx.loader.utils import get_jinja_env
+from yamx.utils import strtobool
 
 
 @dataclass(frozen=True)
 class ResolvingContext:
     _data: Dict[str, bool]
 
     def __getattr__(self, attr_name):
@@ -71,37 +71,34 @@
     try:
         toggle_names = _extract_toggles_from_if_node(jinja_ast.body[0].test)
     except Exception:
         raise Exception(f"Unsupported toggle condition: {condition.raw_value}")
     return toggle_names
 
 
-def _extract_toggles_from_if_node(if_test_node: nodes.Call) -> Set[str]:
-    """Current implementation supports operators `not` and `and`.
+def _extract_toggles_from_if_node(node: nodes.Call) -> Set[str]:
+    """Current implementation supports operators `not`, `and` and `or`.
     Only following conditions are allowed:
 
     `defines.get("FEATURE_FLAG")`
     `toggles.FEATURE_FLAG`
     `toggles.get("FEATURE_FLAG")`
     `toggles["FEATURE_FLAG"]`
     `config_flags.NAME`
     `config_flags.get("NAME")`
     `config_flags["NAME"]`
     """
-    if isinstance(if_test_node, nodes.And):
-        left_toggles = _extract_toggles_from_if_node(if_test_node.left)
-        right_toggles = _extract_toggles_from_if_node(if_test_node.right)
+    if isinstance(node, nodes.Not):
+        return _extract_toggles_from_if_node(node.node)
+    elif isinstance(node, nodes.And) or isinstance(node, nodes.Or):
+        left_toggles = _extract_toggles_from_if_node(node.left)
+        right_toggles = _extract_toggles_from_if_node(node.right)
         return left_toggles | right_toggles
-    elif isinstance(if_test_node, nodes.Not):
-        node = if_test_node.node
-    else:
-        node = if_test_node
-
     # direct access, e.g. toggles.NAME
-    if isinstance(node, nodes.Getattr):
+    elif isinstance(node, nodes.Getattr):
         name = node.node.name
         value = node.attr
     # getitem access, e.g. toggles[]
     elif isinstance(node, nodes.Getitem):
         name = node.node.name
         value = node.arg.value
     # get access, e.g. toggles.get()
```

### Comparing `yamx-0.1.7/yamx/jinja/condition.py` & `yamx-0.1.8/yamx/jinja/condition.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/loader/grouper.py` & `yamx-0.1.8/yamx/loader/grouper.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/loader/preprocessor.py` & `yamx-0.1.8/yamx/loader/preprocessor.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/loader/utils.py` & `yamx-0.1.8/yamx/loader/utils.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/loader/validator.py` & `yamx-0.1.8/yamx/loader/validator.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/representer/common.py` & `yamx-0.1.8/yamx/representer/common.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/representer/conditional_map.py` & `yamx-0.1.8/yamx/representer/conditional_map.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/representer/conditional_seq.py` & `yamx-0.1.8/yamx/representer/conditional_seq.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/representer/rendering.py` & `yamx-0.1.8/yamx/representer/rendering.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/yamx/yamx.py` & `yamx-0.1.8/yamx/yamx.py`

 * *Files identical despite different names*

### Comparing `yamx-0.1.7/PKG-INFO` & `yamx-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: yamx
-Version: 0.1.7
+Version: 0.1.8
 Summary: YAML parser that supports jinja conditional expressions
 Home-page: https://github.com/maybelinot/yamx
 License: Apache-2.0
 Keywords: yaml,jinja,language
 Author: Eduard Trott
 Author-email: eduard.trott@workday.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: immutables (>=0,<1)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: ruamel.yaml (==0.18.3)
 Requires-Dist: ruamel.yaml.string (==0.1.0)
 Project-URL: Repository, https://github.com/maybelinot/yamx
 Description-Content-Type: text/markdown
```

