# Comparing `tmp/fluctuate-2.0.0b3.tar.gz` & `tmp/fluctuate-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluctuate-2.0.0b3.tar", max compression
+gzip compressed data, was "fluctuate-3.0.0.tar", max compression
```

## Comparing `fluctuate-2.0.0b3.tar` & `fluctuate-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-21 22:56:34.665775 fluctuate-2.0.0b3/LICENSE
--rw-r--r--   0        0        0    11094 2023-06-21 22:56:34.665775 fluctuate-2.0.0b3/README.md
--rw-r--r--   0        0        0        0 2023-06-21 22:56:34.689775 fluctuate-2.0.0b3/fluctuate/__init__.py
--rw-r--r--   0        0        0     4404 2023-06-21 22:56:34.665775 fluctuate-2.0.0b3/fluctuate/cli.py
--rw-r--r--   0        0        0    30703 2023-06-21 22:56:34.666775 fluctuate-2.0.0b3/fluctuate/migrations.py
--rw-r--r--   0        0        0     1857 2023-06-21 22:56:34.666775 fluctuate-2.0.0b3/fluctuate/secrets_manager.py
--rw-r--r--   0        0        0     1420 2023-06-21 22:57:12.677679 fluctuate-2.0.0b3/pyproject.toml
--rw-r--r--   0        0        0    12019 1970-01-01 00:00:00.000000 fluctuate-2.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-30 02:22:24.602388 fluctuate-3.0.0/LICENSE
+-rw-r--r--   0        0        0    11094 2024-05-30 02:22:24.603388 fluctuate-3.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 02:22:24.634389 fluctuate-3.0.0/fluctuate/__init__.py
+-rw-r--r--   0        0        0     4404 2024-05-30 02:22:24.603388 fluctuate-3.0.0/fluctuate/cli.py
+-rw-r--r--   0        0        0    30703 2024-05-30 02:22:24.603388 fluctuate-3.0.0/fluctuate/migrations.py
+-rw-r--r--   0        0        0     1857 2024-05-30 02:22:24.603388 fluctuate-3.0.0/fluctuate/secrets_manager.py
+-rw-r--r--   0        0        0     1402 2024-05-30 02:23:29.274994 fluctuate-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12068 1970-01-01 00:00:00.000000 fluctuate-3.0.0/PKG-INFO
```

### Comparing `fluctuate-2.0.0b3/LICENSE` & `fluctuate-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b3/README.md` & `fluctuate-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b3/fluctuate/cli.py` & `fluctuate-3.0.0/fluctuate/cli.py`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b3/fluctuate/migrations.py` & `fluctuate-3.0.0/fluctuate/migrations.py`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b3/fluctuate/secrets_manager.py` & `fluctuate-3.0.0/fluctuate/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `fluctuate-2.0.0b3/pyproject.toml` & `fluctuate-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "fluctuate"
-version = "2.0.0-beta.3"
+version = "3.0.0"
 description = "A simple migration utility for Fauna DB."
 authors = ["Ryan Causey <ryan.causey@munipal.io>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/munipal-oss/fluctuate"
 homepage = "https://gitlab.com/munipal-oss/fluctuate"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
-cloup = "^2.0.0"
+cloup = "^3.0.0"
 faunadb = "^4.3.1"
 boto3 = {extras = ["crt"], version = "^1.26.128", optional = true}
 click-log = "^0.4.0"
-fauna = ">= 0.6.1, < 1.0.0"
+fauna = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 prospector = "^1.7.7"
-black = "^23.0.0"
+black = "^24.0.0"
 isort = "^5.10.1"
 pre-commit = "^3.0.0"
-pytest = "^7.2.0"
+pytest = "^8.0.0"
 python-decouple = "^3.6"
 pytest-xdist = "^3.0.2"
-pytest-cov = "^4.0.0"
-pytest-env = "^0.8.1"
+pytest-cov = "^5.0.0"
+pytest-env = "^1.0.0"
 
 [tool.poetry.extras]
 aws_secrets_manager = ["boto3"]
 
 [tool.poetry.scripts]
 fluctuate = "fluctuate.cli:entrypoint"
```

### Comparing `fluctuate-2.0.0b3/PKG-INFO` & `fluctuate-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: fluctuate
-Version: 2.0.0b3
+Version: 3.0.0
 Summary: A simple migration utility for Fauna DB.
 Home-page: https://gitlab.com/munipal-oss/fluctuate
 License: MIT
 Author: Ryan Causey
 Author-email: ryan.causey@munipal.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aws-secrets-manager
 Requires-Dist: boto3[crt] (>=1.26.128,<2.0.0) ; extra == "aws-secrets-manager"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
-Requires-Dist: cloup (>=2.0.0,<3.0.0)
-Requires-Dist: fauna (>=0.6.1,<1.0.0)
+Requires-Dist: cloup (>=3.0.0,<4.0.0)
+Requires-Dist: fauna (>=2.0.0,<3.0.0)
 Requires-Dist: faunadb (>=4.3.1,<5.0.0)
 Project-URL: Repository, https://gitlab.com/munipal-oss/fluctuate
 Description-Content-Type: text/markdown
 
 # Fluctuate
 
 [![coverage report](https://gitlab.com/munipal-oss/fluctuate/badges/master/coverage.svg)](https://gitlab.com/munipal-oss/fluctuate/-/commits/master)
```

