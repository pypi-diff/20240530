# Comparing `tmp/athena_python_udf-0.2.0.tar.gz` & `tmp/athena_python_udf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_python_udf-0.2.0.tar", max compression
+gzip compressed data, was "athena_python_udf-0.2.1.tar", max compression
```

## Comparing `athena_python_udf-0.2.0.tar` & `athena_python_udf-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-04-08 11:45:10.895858 athena_python_udf-0.2.0/LICENSE
--rw-r--r--   0        0        0     3578 2024-04-08 11:45:10.895858 athena_python_udf-0.2.0/README.md
--rw-r--r--   0        0        0       71 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/athena_udf/__init__.py
--rw-r--r--   0        0        0     2848 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/athena_udf/base.py
--rw-r--r--   0        0        0     1441 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/athena_udf/utils.py
--rw-r--r--   0        0        0     1366 2024-04-08 11:45:10.899858 athena_python_udf-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4444 1970-01-01 00:00:00.000000 athena_python_udf-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 09:43:37.894785 athena_python_udf-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3601 2024-05-30 09:43:37.894785 athena_python_udf-0.2.1/README.md
+-rw-r--r--   0        0        0       71 2024-05-30 09:43:37.894785 athena_python_udf-0.2.1/athena_udf/__init__.py
+-rw-r--r--   0        0        0     2848 2024-05-30 09:43:37.894785 athena_python_udf-0.2.1/athena_udf/base.py
+-rw-r--r--   0        0        0     1441 2024-05-30 09:43:37.894785 athena_python_udf-0.2.1/athena_udf/utils.py
+-rw-r--r--   0        0        0     1366 2024-05-30 09:43:37.894785 athena_python_udf-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4467 1970-01-01 00:00:00.000000 athena_python_udf-0.2.1/PKG-INFO
```

### Comparing `athena_python_udf-0.2.0/LICENSE` & `athena_python_udf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `athena_python_udf-0.2.0/README.md` & `athena_python_udf-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # athena-python-udf
 
 <!-- markdownlint-disable -->
-[![PyPI](https://img.shields.io/pypi/v/athena-udf.svg)](https://pypi.org/project/athena-udf/)
-[![Changelog](https://img.shields.io/github/v/release/dmarkey/python-athena-udf?include_prereleases&label=changelog)](https://github.com/dmarkey/python-athena-udf/releases)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dmarkey/python-athena-udf/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/athena-python-udf.svg)](https://pypi.org/project/athena-python-udf/)
+[![Changelog](https://img.shields.io/github/v/release/dbt-athena/athena-python-udf?include_prereleases&label=changelog)](https://github.com/dbt-athena/athena-python-udf/releases)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dbt-athena/athena-python-udf/blob/main/LICENSE)
 <!-- markdownlint-restore -->
 
 Athena User Defined Functions(UDFs) in Python made easy!
 
 This library implements the Athena UDF protocol in Python,
 so you don't have to use Java, and you can use any Python library you wish, including numpy/pandas!
```

### Comparing `athena_python_udf-0.2.0/athena_udf/base.py` & `athena_python_udf-0.2.1/athena_udf/base.py`

 * *Files identical despite different names*

### Comparing `athena_python_udf-0.2.0/athena_udf/utils.py` & `athena_python_udf-0.2.1/athena_udf/utils.py`

 * *Files identical despite different names*

### Comparing `athena_python_udf-0.2.0/pyproject.toml` & `athena_python_udf-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "athena-python-udf"
-version = "0.2.0"
+version = "0.2.1"
 description = "Athena User Defined Functions(UDFs) in Python made easy!"
 license = "Apache-2.0"
 authors = ["David Markey <david@dmarkey.com>"]
 maintainers = ["Serhii Dimchenko <svdimchenko@gmail.com>"]
 keywords = ["aws", "athena", "python", "udf", "lambda"]
 readme = "README.md"
 repository = "https://github.com/dbt-athena/athena-python-udf"
```

### Comparing `athena_python_udf-0.2.0/PKG-INFO` & `athena_python_udf-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-python-udf
-Version: 0.2.0
+Version: 0.2.1
 Summary: Athena User Defined Functions(UDFs) in Python made easy!
 Home-page: https://github.com/dbt-athena/athena-python-udf
 License: Apache-2.0
 Keywords: aws,athena,python,udf,lambda
 Author: David Markey
 Author-email: david@dmarkey.com
 Maintainer: Serhii Dimchenko
@@ -19,17 +19,17 @@
 Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Project-URL: Repository, https://github.com/dbt-athena/athena-python-udf
 Description-Content-Type: text/markdown
 
 # athena-python-udf
 
 <!-- markdownlint-disable -->
-[![PyPI](https://img.shields.io/pypi/v/athena-udf.svg)](https://pypi.org/project/athena-udf/)
-[![Changelog](https://img.shields.io/github/v/release/dmarkey/python-athena-udf?include_prereleases&label=changelog)](https://github.com/dmarkey/python-athena-udf/releases)
-[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dmarkey/python-athena-udf/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/athena-python-udf.svg)](https://pypi.org/project/athena-python-udf/)
+[![Changelog](https://img.shields.io/github/v/release/dbt-athena/athena-python-udf?include_prereleases&label=changelog)](https://github.com/dbt-athena/athena-python-udf/releases)
+[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/dbt-athena/athena-python-udf/blob/main/LICENSE)
 <!-- markdownlint-restore -->
 
 Athena User Defined Functions(UDFs) in Python made easy!
 
 This library implements the Athena UDF protocol in Python,
 so you don't have to use Java, and you can use any Python library you wish, including numpy/pandas!
```

