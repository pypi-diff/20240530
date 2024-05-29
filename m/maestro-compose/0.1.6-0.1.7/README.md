# Comparing `tmp/maestro_compose-0.1.6.tar.gz` & `tmp/maestro_compose-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro_compose-0.1.6.tar", max compression
+gzip compressed data, was "maestro_compose-0.1.7.tar", max compression
```

## Comparing `maestro_compose-0.1.6.tar` & `maestro_compose-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4189 2024-05-26 03:15:19.000000 maestro_compose-0.1.6/README.md
--rw-r--r--   0        0        0       57 2024-05-26 03:15:19.000000 maestro_compose-0.1.6/maestro_compose/__init__.py
--rw-r--r--   0        0        0     2285 2024-05-29 23:43:49.957896 maestro_compose-0.1.6/maestro_compose/__main__.py
--rw-r--r--   0        0        0     8373 2024-05-29 23:48:04.155490 maestro_compose-0.1.6/maestro_compose/commands.py
--rw-r--r--   0        0        0     1386 2024-05-29 22:58:43.824067 maestro_compose-0.1.6/maestro_compose/models.py
--rw-r--r--   0        0        0      823 2024-05-29 23:48:43.739429 maestro_compose-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5159 1970-01-01 00:00:00.000000 maestro_compose-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4189 2024-05-26 03:15:19.000000 maestro_compose-0.1.7/README.md
+-rw-r--r--   0        0        0       57 2024-05-26 03:15:19.000000 maestro_compose-0.1.7/maestro_compose/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-29 23:43:49.957896 maestro_compose-0.1.7/maestro_compose/__main__.py
+-rw-r--r--   0        0        0     8373 2024-05-29 23:48:04.155490 maestro_compose-0.1.7/maestro_compose/commands.py
+-rw-r--r--   0        0        0     1386 2024-05-29 23:49:52.873322 maestro_compose-0.1.7/maestro_compose/models.py
+-rw-r--r--   0        0        0      841 2024-05-29 23:55:35.478806 maestro_compose-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 maestro_compose-0.1.7/PKG-INFO
```

### Comparing `maestro_compose-0.1.6/README.md` & `maestro_compose-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.6/maestro_compose/__main__.py` & `maestro_compose-0.1.7/maestro_compose/__main__.py`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.6/maestro_compose/commands.py` & `maestro_compose-0.1.7/maestro_compose/commands.py`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.6/maestro_compose/models.py` & `maestro_compose-0.1.7/maestro_compose/models.py`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.6/pyproject.toml` & `maestro_compose-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "maestro-compose"
-version = "0.1.6"
+version = "0.1.7"
 description = "A simple command line tool for managing Docker Compose stacks using tags and other metadata."
 license = "MIT"
 authors = ["Nick Schenone <nschenone16@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/nschenone/maestro-compose"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 click = "^8.1.7"
 pydantic = "^2.7.1"
 pyyaml = "^6.0.1"
 loguru = "^0.7.2"
 colorama = "^0.4.6"
 tabulate = "^0.9.0"
+pandas = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = ">=3.7.9,<4.0"
 mypy = ">=0.740"
 isort = "^5.12.0"
```

### Comparing `maestro_compose-0.1.6/PKG-INFO` & `maestro_compose-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-compose
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple command line tool for managing Docker Compose stacks using tags and other metadata.
 Home-page: https://github.com/nschenone/maestro-compose
 License: MIT
 Author: Nick Schenone
 Author-email: nschenone16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/nschenone/maestro-compose
 Description-Content-Type: text/markdown
 
 # Maestro
```

