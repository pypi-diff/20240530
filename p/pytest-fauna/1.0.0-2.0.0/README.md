# Comparing `tmp/pytest_fauna-1.0.0.tar.gz` & `tmp/pytest_fauna-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_fauna-1.0.0.tar", max compression
+gzip compressed data, was "pytest_fauna-2.0.0.tar", max compression
```

## Comparing `pytest_fauna-1.0.0.tar` & `pytest_fauna-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-04-22 02:37:05.474776 pytest_fauna-1.0.0/LICENSE
--rw-r--r--   0        0        0     1099 2024-04-22 02:37:05.474776 pytest_fauna-1.0.0/README.md
--rw-r--r--   0        0        0     1089 2024-04-22 02:38:01.798389 pytest_fauna-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 02:37:05.498776 pytest_fauna-1.0.0/pytest_fauna/__init__.py
--rw-r--r--   0        0        0     5613 2024-04-22 02:37:05.475776 pytest_fauna-1.0.0/pytest_fauna/plugin.py
--rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 pytest_fauna-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-30 04:06:35.916338 pytest_fauna-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1099 2024-05-30 04:06:35.916338 pytest_fauna-2.0.0/README.md
+-rw-r--r--   0        0        0     1089 2024-05-30 04:07:36.285625 pytest_fauna-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 04:06:35.945338 pytest_fauna-2.0.0/pytest_fauna/__init__.py
+-rw-r--r--   0        0        0     5613 2024-05-30 04:06:35.917338 pytest_fauna-2.0.0/pytest_fauna/plugin.py
+-rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 pytest_fauna-2.0.0/PKG-INFO
```

### Comparing `pytest_fauna-1.0.0/LICENSE` & `pytest_fauna-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_fauna-1.0.0/README.md` & `pytest_fauna-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_fauna-1.0.0/pyproject.toml` & `pytest_fauna-2.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "pytest-fauna"
-version = "1.0.0"
+version = "2.0.0"
 description = "A collection of helpful test fixtures for Fauna DB."
 authors = ["Ryan Causey <ryan.causey@munipal.io>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/munipal-oss/pytest-fauna"
 homepage = "https://gitlab.com/munipal-oss/pytest-fauna"
 classifiers = [
     "Framework :: Pytest"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fauna = "^1.0.0"
+fauna = "^2.0.0"
 python-decouple = "^3.8"
 pytest-aws-fixtures = {version = "^1.2.0", optional = true}
-fluctuate = {version = "^2.0.0", optional = true}
+fluctuate = {version = "^3.0.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 prospector = "^1.7.7"
-black = "^23.0.0"
+black = "^24.0.0"
 isort = "^5.10.1"
 pre-commit = "^3.0.0"
 
 [tool.poetry.extras]
 aws = ["pytest-aws-fixtures"]
 fluctuate = ["fluctuate"]
```

### Comparing `pytest_fauna-1.0.0/pytest_fauna/plugin.py` & `pytest_fauna-2.0.0/pytest_fauna/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_fauna-1.0.0/PKG-INFO` & `pytest_fauna-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-fauna
-Version: 1.0.0
+Version: 2.0.0
 Summary: A collection of helpful test fixtures for Fauna DB.
 Home-page: https://gitlab.com/munipal-oss/pytest-fauna
 License: MIT
 Author: Ryan Causey
 Author-email: ryan.causey@munipal.io
 Requires-Python: >=3.10,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aws
 Provides-Extra: fluctuate
-Requires-Dist: fauna (>=1.0.0,<2.0.0)
-Requires-Dist: fluctuate (>=2.0.0,<3.0.0) ; extra == "fluctuate"
+Requires-Dist: fauna (>=2.0.0,<3.0.0)
+Requires-Dist: fluctuate (>=3.0.0,<4.0.0) ; extra == "fluctuate"
 Requires-Dist: pytest-aws-fixtures (>=1.2.0,<2.0.0) ; extra == "aws"
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Project-URL: Repository, https://gitlab.com/munipal-oss/pytest-fauna
 Description-Content-Type: text/markdown
 
 # pytest-fauna
```

