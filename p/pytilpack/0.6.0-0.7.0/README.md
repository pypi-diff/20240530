# Comparing `tmp/pytilpack-0.6.0.tar.gz` & `tmp/pytilpack-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytilpack-0.6.0.tar", max compression
+gzip compressed data, was "pytilpack-0.7.0.tar", max compression
```

## Comparing `pytilpack-0.6.0.tar` & `pytilpack-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2024-05-25 02:38:03.257073 pytilpack-0.6.0/LICENSE
--rw-r--r--   0        0        0     1440 2024-05-25 02:38:03.257073 pytilpack-0.6.0/README.md
--rw-r--r--   0        0        0     2677 2024-05-25 02:38:14.789140 pytilpack-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-25 02:38:03.257073 pytilpack-0.6.0/pytilpack/__init__.py
--rw-r--r--   0        0        0      942 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/csv_.py
--rw-r--r--   0        0        0     5391 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/flask_.py
--rw-r--r--   0        0        0      818 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/flask_login_.py
--rw-r--r--   0        0        0     2377 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/functools_.py
--rw-r--r--   0        0        0     4776 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/openai_.py
--rw-r--r--   0        0        0      566 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/pathlib_.py
--rw-r--r--   0        0        0     1363 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/python_.py
--rw-r--r--   0        0        0     2392 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/sqlalchemy_.py
--rw-r--r--   0        0        0     8055 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/tiktoken_.py
--rw-r--r--   0        0        0      523 2024-05-25 02:38:03.261073 pytilpack-0.6.0/pytilpack/tqdm_.py
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pytilpack-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-30 12:56:23.878782 pytilpack-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1440 2024-05-30 12:56:23.878782 pytilpack-0.7.0/README.md
+-rw-r--r--   0        0        0     2677 2024-05-30 12:56:36.846701 pytilpack-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/csv_.py
+-rw-r--r--   0        0        0     5391 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/flask_.py
+-rw-r--r--   0        0        0      818 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/flask_login_.py
+-rw-r--r--   0        0        0     2377 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/functools_.py
+-rw-r--r--   0        0        0     4776 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/openai_.py
+-rw-r--r--   0        0        0      566 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/pathlib_.py
+-rw-r--r--   0        0        0     1363 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/python_.py
+-rw-r--r--   0        0        0     2392 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/sqlalchemy_.py
+-rw-r--r--   0        0        0     8055 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/tiktoken_.py
+-rw-r--r--   0        0        0     1692 2024-05-30 12:56:23.878782 pytilpack-0.7.0/pytilpack/tqdm_.py
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pytilpack-0.7.0/PKG-INFO
```

### Comparing `pytilpack-0.6.0/LICENSE` & `pytilpack-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/README.md` & `pytilpack-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pyproject.toml` & `pytilpack-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytilpack"
-version = "0.6.0"  # using poetry-dynamic-versioning
+version = "0.7.0"  # using poetry-dynamic-versioning
 description = "Python Utility Pack"
 license = "MIT"
 authors = ["aki. <mark@aur.ll.to>"]
 readme = "README.md"
 homepage = "https://github.com/ak110/pytilpack"
 classifiers = [
     "Environment :: Console",
```

### Comparing `pytilpack-0.6.0/pytilpack/csv_.py` & `pytilpack-0.7.0/pytilpack/csv_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/flask_.py` & `pytilpack-0.7.0/pytilpack/flask_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/flask_login_.py` & `pytilpack-0.7.0/pytilpack/flask_login_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/functools_.py` & `pytilpack-0.7.0/pytilpack/functools_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/openai_.py` & `pytilpack-0.7.0/pytilpack/openai_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/pathlib_.py` & `pytilpack-0.7.0/pytilpack/pathlib_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/python_.py` & `pytilpack-0.7.0/pytilpack/python_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/sqlalchemy_.py` & `pytilpack-0.7.0/pytilpack/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/pytilpack/tiktoken_.py` & `pytilpack-0.7.0/pytilpack/tiktoken_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.6.0/PKG-INFO` & `pytilpack-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytilpack
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python Utility Pack
 Home-page: https://github.com/ak110/pytilpack
 License: MIT
 Author: aki.
 Author-email: mark@aur.ll.to
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
```

