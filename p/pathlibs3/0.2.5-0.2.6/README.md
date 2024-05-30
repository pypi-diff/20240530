# Comparing `tmp/pathlibs3-0.2.5.tar.gz` & `tmp/pathlibs3-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.5.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.6.tar", max compression
```

## Comparing `pathlibs3-0.2.5.tar` & `pathlibs3-0.2.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.5/pathlibs3/__init__.py
--rw-r--r--   0        0        0     4636 2024-05-16 16:55:44.797522 pathlibs3-0.2.5/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      638 2024-05-16 17:20:49.756077 pathlibs3-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      611 1970-01-01 00:00:00.000000 pathlibs3-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.6/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     4636 2024-05-16 16:55:44.797522 pathlibs3-0.2.6/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      632 2024-05-29 13:06:37.674840 pathlibs3-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pathlibs3-0.2.6/PKG-INFO
```

### Comparing `pathlibs3-0.2.5/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.6/pathlibs3/pathlibs3.py`

 * *Files identical despite different names*

### Comparing `pathlibs3-0.2.5/pyproject.toml` & `pathlibs3-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pathlibs3"
-version = "0.2.5"
+version = "0.2.6"
 description = "S3 navigation using object, inspired by pathlib.Path"
 authors = ["thibault.blanc"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 boto3 = "*"
-urllib3 = "^2.2.1"
-moto = "^4.1.12"
+urllib3 = "*"
+moto = "^4.0.0"
 Sphinx = { version = "4.2.0", optional = true }
 sphinx-rtd-theme = { version = "1.0.0", optional = true }
 sphinxcontrib-napoleon = { version = "0.7", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
```

### Comparing `pathlibs3-0.2.5/PKG-INFO` & `pathlibs3-0.2.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pathlibs3
-Version: 0.2.5
+Version: 0.2.6
 Summary: S3 navigation using object, inspired by pathlib.Path
 Author: thibault.blanc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: Sphinx (==4.2.0) ; extra == "docs"
 Requires-Dist: boto3
-Requires-Dist: moto (>=4.1.12,<5.0.0)
+Requires-Dist: moto (>=4.0.0,<5.0.0)
 Requires-Dist: sphinx-rtd-theme (==1.0.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-napoleon (==0.7) ; extra == "docs"
-Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
+Requires-Dist: urllib3
```

