# Comparing `tmp/ai_helpers_pyspark_utils-0.1.0a1.tar.gz` & `tmp/ai_helpers_pyspark_utils-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_helpers_pyspark_utils-0.1.0a1.tar", max compression
+gzip compressed data, was "ai_helpers_pyspark_utils-0.1.0a2.tar", max compression
```

## Comparing `ai_helpers_pyspark_utils-0.1.0a1.tar` & `ai_helpers_pyspark_utils-0.1.0a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1333 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/README.md
--rw-r--r--   0        0        0     1743 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      447 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/pyspark_utils/__init__.py
--rw-r--r--   0        0        0     3331 2024-05-29 15:03:51.599158 ai_helpers_pyspark_utils-0.1.0a1/pyspark_utils/utils.py
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 ai_helpers_pyspark_utils-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1333 2024-05-30 11:49:30.394311 ai_helpers_pyspark_utils-0.1.0a2/README.md
+-rw-r--r--   0        0        0     2001 2024-05-30 11:49:30.394311 ai_helpers_pyspark_utils-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-30 11:49:30.394311 ai_helpers_pyspark_utils-0.1.0a2/pyspark_utils/__init__.py
+-rw-r--r--   0        0        0     3331 2024-05-30 11:49:30.394311 ai_helpers_pyspark_utils-0.1.0a2/pyspark_utils/utils.py
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 ai_helpers_pyspark_utils-0.1.0a2/PKG-INFO
```

### Comparing `ai_helpers_pyspark_utils-0.1.0a1/README.md` & `ai_helpers_pyspark_utils-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `ai_helpers_pyspark_utils-0.1.0a1/pyproject.toml` & `ai_helpers_pyspark_utils-0.1.0a2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 [tool.poetry]
 name = "ai-helpers-pyspark-utils"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Common pyspark utils"
 authors = ["Corentin Vasseur <vasseur.corentin@gmail.com>"]
 packages = [{ include = "pyspark_utils" }]
 readme = "README.md"
+repository = "https://github.com/ai-helpers/pyspark-utils"
+documentation = "https://ai-helpers.github.io/pyspark-utils/"
+keywords = ["machine-learning", "pyspark", "utils"]
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 pandas = "^2.2.2"
 pyspark = "^3.5.1"
 typing-extensions = "^4.10.0"
```

### Comparing `ai_helpers_pyspark_utils-0.1.0a1/pyspark_utils/utils.py` & `ai_helpers_pyspark_utils-0.1.0a2/pyspark_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pyspark_utils-0.1.0a1/PKG-INFO` & `ai_helpers_pyspark_utils-0.1.0a2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: ai-helpers-pyspark-utils
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Common pyspark utils
+Home-page: https://github.com/ai-helpers/pyspark-utils
+Keywords: machine-learning,pyspark,utils
 Author: Corentin Vasseur
 Author-email: vasseur.corentin@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pyspark (>=3.5.1,<4.0.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
+Project-URL: Documentation, https://ai-helpers.github.io/pyspark-utils/
+Project-URL: Repository, https://github.com/ai-helpers/pyspark-utils
 Description-Content-Type: text/markdown
 
 # AI Helpers - PySpark utils
 
 `pyspark-utils` is a Python module that provides a collection of utilities to simplify and enhance the use of PySpark. These utilities are designed to make working with PySpark more efficient and to reduce boilerplate code.
 
 ## Table of Contents
```

