# Comparing `tmp/onnxslim-0.1.9.tar.gz` & `tmp/onnxslim-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxslim-0.1.9.tar", last modified: Tue Dec 19 02:44:52 2023, max compression
+gzip compressed data, was "onnxslim-0.1.9.1.tar", last modified: Tue Dec 19 03:15:15 2023, max compression
```

## Comparing `onnxslim-0.1.9.tar` & `onnxslim-0.1.9.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.744208 onnxslim-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-19 02:44:43.000000 onnxslim-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-19 02:44:43.000000 onnxslim-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-19 02:44:52.744208 onnxslim-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-19 02:44:43.000000 onnxslim-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-19 02:44:43.000000 onnxslim-0.1.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.736208 onnxslim-0.1.9/onnxslim/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.740208 onnxslim-0.1.9/onnxslim/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/cli/_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.740208 onnxslim-0.1.9/onnxslim/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25125 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/core/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/core/slim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.740208 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.740208 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/exporters/base_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/exporters/onnx_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.740208 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/importers/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/importers/base_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15011 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/importers/onnx_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.744208 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54050 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10193 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.744208 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.744208 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/util/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/util/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.744208 onnxslim-0.1.9/onnxslim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/utils/font.py
--rw-r--r--   0 runner    (1001) docker     (127)    99128 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/utils/tabulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-12-19 02:44:43.000000 onnxslim-0.1.9/onnxslim/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:44:52.744208 onnxslim-0.1.9/onnxslim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:44:52.000000 onnxslim-0.1.9/onnxslim.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 02:44:52.744208 onnxslim-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-12-19 02:44:43.000000 onnxslim-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.923117 onnxslim-0.1.9.1/onnxslim/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.923117 onnxslim-0.1.9.1/onnxslim/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/cli/_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.923117 onnxslim-0.1.9.1/onnxslim/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25132 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/core/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/core/slim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.923117 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/exporters/base_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/exporters/onnx_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/importers/base_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15011 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/importers/onnx_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54050 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10193 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/util/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/util/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/onnxslim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/utils/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99128 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/utils/tabulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/onnxslim/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/onnxslim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 03:15:15.000000 onnxslim-0.1.9.1/onnxslim.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 03:15:15.927117 onnxslim-0.1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-12-19 03:15:06.000000 onnxslim-0.1.9.1/setup.py
```

### Comparing `onnxslim-0.1.9/LICENSE` & `onnxslim-0.1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/PKG-INFO` & `onnxslim-0.1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxslim
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: OnnxSlim: A Toolkit to Help Optimizer Onnx Model
 Home-page: https://github.com/inisis/OnnxSlim
 Author: inisis
 Author-email: desmond.yao@buaa.edu.cn
 License: MIT
 Project-URL: Bug Tracker, https://github.com/inisis/OnnxSlim/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `onnxslim-0.1.9/README.md` & `onnxslim-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/__init__.py` & `onnxslim-0.1.9.1/onnxslim/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/cli/_main.py` & `onnxslim-0.1.9.1/onnxslim/cli/_main.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/core/optimizer.py` & `onnxslim-0.1.9.1/onnxslim/core/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         DEFAULT_FUSION_PATTERNS[layer_type] = fn
         return fn
 
     return insert
 
 
 def get_fusion_patterns(skip_fusion_patterns: str = None):
-    default_fusion_patterns = DEFAULT_FUSION_PATTERNS
+    default_fusion_patterns = DEFAULT_FUSION_PATTERNS.copy()
     if skip_fusion_patterns:
         for pattern in skip_fusion_patterns:
             default_fusion_patterns.pop(pattern)
 
     return default_fusion_patterns
```

### Comparing `onnxslim-0.1.9/onnxslim/core/slim.py` & `onnxslim-0.1.9.1/onnxslim/core/slim.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/exporters/base_exporter.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/exporters/onnx_exporter.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/exporters/onnx_exporter.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/importers/base_importer.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/importers/base_importer.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/importers/onnx_importer.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/importers/onnx_importer.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/graph.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/graph.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/node.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/node.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/ir/tensor.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/ir/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/logger/logger.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/logger/logger.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/util/exception.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/util/exception.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/onnx_graphsurgeon/util/misc.py` & `onnxslim-0.1.9.1/onnxslim/onnx_graphsurgeon/util/misc.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/utils/tabulate.py` & `onnxslim-0.1.9.1/onnxslim/utils/tabulate.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim/utils/utils.py` & `onnxslim-0.1.9.1/onnxslim/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/onnxslim.egg-info/PKG-INFO` & `onnxslim-0.1.9.1/onnxslim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxslim
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: OnnxSlim: A Toolkit to Help Optimizer Onnx Model
 Home-page: https://github.com/inisis/OnnxSlim
 Author: inisis
 Author-email: desmond.yao@buaa.edu.cn
 License: MIT
 Project-URL: Bug Tracker, https://github.com/inisis/OnnxSlim/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `onnxslim-0.1.9/onnxslim.egg-info/SOURCES.txt` & `onnxslim-0.1.9.1/onnxslim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxslim-0.1.9/setup.py` & `onnxslim-0.1.9.1/setup.py`

 * *Files identical despite different names*

