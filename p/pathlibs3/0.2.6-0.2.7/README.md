# Comparing `tmp/pathlibs3-0.2.6.tar.gz` & `tmp/pathlibs3-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.6.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.7.tar", max compression
```

## Comparing `pathlibs3-0.2.6.tar` & `pathlibs3-0.2.7.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.6/pathlibs3/__init__.py
--rw-r--r--   0        0        0     4636 2024-05-16 16:55:44.797522 pathlibs3-0.2.6/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      632 2024-05-29 13:06:37.674840 pathlibs3-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 pathlibs3-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1652 2024-05-30 09:52:58.162711 pathlibs3-0.2.7/README.md
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.7/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     4636 2024-05-16 16:55:44.797522 pathlibs3-0.2.7/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      654 2024-05-30 09:53:04.286602 pathlibs3-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 pathlibs3-0.2.7/PKG-INFO
```

### Comparing `pathlibs3-0.2.6/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.7/pathlibs3/pathlibs3.py`

 * *Files identical despite different names*

### Comparing `pathlibs3-0.2.6/pyproject.toml` & `pathlibs3-0.2.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "pathlibs3"
-version = "0.2.6"
+version = "0.2.7"
 description = "S3 navigation using object, inspired by pathlib.Path"
 authors = ["thibault.blanc"]
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 boto3 = "*"
 urllib3 = "*"
-moto = "^4.0.0"
+
 Sphinx = { version = "4.2.0", optional = true }
 sphinx-rtd-theme = { version = "1.0.0", optional = true }
 sphinxcontrib-napoleon = { version = "0.7", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
+moto = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon"]
```

