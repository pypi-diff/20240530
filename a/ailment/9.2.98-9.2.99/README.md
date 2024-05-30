# Comparing `tmp/ailment-9.2.98.tar.gz` & `tmp/ailment-9.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailment-9.2.98.tar", last modified: Tue Apr  9 17:02:18 2024, max compression
+gzip compressed data, was "ailment-9.2.99.tar", last modified: Tue Apr 16 17:02:14 2024, max compression
```

## Comparing `ailment-9.2.98.tar` & `ailment-9.2.99.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:18.960615 ailment-9.2.98/
--rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-09 17:01:32.000000 ailment-9.2.98/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-04-09 17:02:18.960615 ailment-9.2.98/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-09 17:01:32.000000 ailment-9.2.98/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:18.956615 ailment-9.2.98/ailment/
--rw-r--r--   0 vsts      (1001) docker     (127)     2014 2024-04-09 17:01:43.000000 ailment-9.2.98/ailment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2260 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/block.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19143 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/block_walker.py
--rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/converter_common.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23721 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/converter_pcode.py
--rw-r--r--   0 vsts      (1001) docker     (127)    26673 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/converter_vex.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36737 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/expression.py
--rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20109 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/statement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1538 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/tagged_object.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-04-09 17:01:32.000000 ailment-9.2.98/ailment/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:18.960615 ailment-9.2.98/ailment.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-04-09 17:02:18.000000 ailment-9.2.98/ailment.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-09 17:02:18.000000 ailment-9.2.98/ailment.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-09 17:02:18.000000 ailment-9.2.98/ailment.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-09 17:02:18.000000 ailment-9.2.98/ailment.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-09 17:02:18.000000 ailment-9.2.98/ailment.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-09 17:01:43.000000 ailment-9.2.98/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-04-09 17:02:18.960615 ailment-9.2.98/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-09 17:02:18.960615 ailment-9.2.98/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-04-09 17:01:32.000000 ailment-9.2.98/tests/test_irsb.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:14.685614 ailment-9.2.99/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1327 2024-04-16 17:01:29.000000 ailment-9.2.99/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-04-16 17:02:14.685614 ailment-9.2.99/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-16 17:01:29.000000 ailment-9.2.99/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:14.681614 ailment-9.2.99/ailment/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2014 2024-04-16 17:01:35.000000 ailment-9.2.99/ailment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2260 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/block.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19143 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/block_walker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/converter_common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23721 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/converter_pcode.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    26673 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/converter_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36737 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/expression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      704 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20109 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/statement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1538 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/tagged_object.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-04-16 17:01:29.000000 ailment-9.2.99/ailment/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:14.681614 ailment-9.2.99/ailment.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1584 2024-04-16 17:02:14.000000 ailment-9.2.99/ailment.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      460 2024-04-16 17:02:14.000000 ailment-9.2.99/ailment.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-16 17:02:14.000000 ailment-9.2.99/ailment.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-16 17:02:14.000000 ailment-9.2.99/ailment.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        8 2024-04-16 17:02:14.000000 ailment-9.2.99/ailment.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      277 2024-04-16 17:01:35.000000 ailment-9.2.99/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      820 2024-04-16 17:02:14.685614 ailment-9.2.99/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 17:02:14.681614 ailment-9.2.99/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1479 2024-04-16 17:01:29.000000 ailment-9.2.99/tests/test_irsb.py
```

### Comparing `ailment-9.2.98/LICENSE` & `ailment-9.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/PKG-INFO` & `ailment-9.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailment
-Version: 9.2.98
+Version: 9.2.99
 Summary: The angr intermediate language.
 Home-page: https://github.com/angr/ailment
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ailment-9.2.98/README.md` & `ailment-9.2.99/README.md`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/__init__.py` & `ailment-9.2.99/ailment/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "9.2.98"
+__version__ = "9.2.99"
 
 import logging
 from typing import Set
 
 from .block import Block
 from . import statement as Stmt
 from . import expression as Expr
```

### Comparing `ailment-9.2.98/ailment/block.py` & `ailment-9.2.99/ailment/block.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/block_walker.py` & `ailment-9.2.99/ailment/block_walker.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/converter_pcode.py` & `ailment-9.2.99/ailment/converter_pcode.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/converter_vex.py` & `ailment-9.2.99/ailment/converter_vex.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/expression.py` & `ailment-9.2.99/ailment/expression.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/manager.py` & `ailment-9.2.99/ailment/manager.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/statement.py` & `ailment-9.2.99/ailment/statement.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/tagged_object.py` & `ailment-9.2.99/ailment/tagged_object.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment/utils.py` & `ailment-9.2.99/ailment/utils.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/ailment.egg-info/PKG-INFO` & `ailment-9.2.99/ailment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailment
-Version: 9.2.98
+Version: 9.2.99
 Summary: The angr intermediate language.
 Home-page: https://github.com/angr/ailment
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ailment-9.2.98/setup.cfg` & `ailment-9.2.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `ailment-9.2.98/tests/test_irsb.py` & `ailment-9.2.99/tests/test_irsb.py`

 * *Files identical despite different names*

