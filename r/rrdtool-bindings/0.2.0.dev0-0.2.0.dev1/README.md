# Comparing `tmp/rrdtool_bindings-0.2.0.dev0.tar.gz` & `tmp/rrdtool_bindings-0.2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrdtool_bindings-0.2.0.dev0.tar", last modified: Thu May 30 20:12:23 2024, max compression
+gzip compressed data, was "rrdtool_bindings-0.2.0.dev1.tar", last modified: Thu May 30 20:47:03 2024, max compression
```

## Comparing `rrdtool_bindings-0.2.0.dev0.tar` & `rrdtool_bindings-0.2.0.dev1.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:12:23.721266 rrdtool_bindings-0.2.0.dev0/
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     2621 2024-05-30 20:12:23.721266 rrdtool_bindings-0.2.0.dev0/PKG-INFO
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     1706 2024-05-30 20:07:47.000000 rrdtool_bindings-0.2.0.dev0/README.md
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     1789 2024-05-30 20:10:21.000000 rrdtool_bindings-0.2.0.dev0/pyproject.toml
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)       38 2024-05-30 20:12:23.721266 rrdtool_bindings-0.2.0.dev0/setup.cfg
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      465 2024-05-30 07:29:16.000000 rrdtool_bindings-0.2.0.dev0/setup.py
-drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:12:23.720266 rrdtool_bindings-0.2.0.dev0/src/
-drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:12:23.721266 rrdtool_bindings-0.2.0.dev0/src/rrdtool_bindings.egg-info/
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     2621 2024-05-30 20:12:23.000000 rrdtool_bindings-0.2.0.dev0/src/rrdtool_bindings.egg-info/PKG-INFO
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      252 2024-05-30 20:12:23.000000 rrdtool_bindings-0.2.0.dev0/src/rrdtool_bindings.egg-info/SOURCES.txt
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)        1 2024-05-30 20:12:23.000000 rrdtool_bindings-0.2.0.dev0/src/rrdtool_bindings.egg-info/dependency_links.txt
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)        8 2024-05-30 20:12:23.000000 rrdtool_bindings-0.2.0.dev0/src/rrdtool_bindings.egg-info/top_level.txt
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)    43262 2024-05-26 05:35:57.000000 rrdtool_bindings-0.2.0.dev0/src/rrdtoolmodule.c
-drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:12:23.721266 rrdtool_bindings-0.2.0.dev0/tests/
--rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     2737 2024-05-30 07:27:48.000000 rrdtool_bindings-0.2.0.dev0/tests/test_bindings.py
+drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:47:03.088302 rrdtool_bindings-0.2.0.dev1/
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      424 2024-05-30 19:42:31.000000 rrdtool_bindings-0.2.0.dev1/.editorconfig
+drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:47:03.086303 rrdtool_bindings-0.2.0.dev1/.github/
+drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:47:03.087303 rrdtool_bindings-0.2.0.dev1/.github/workflows/
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      895 2024-05-30 07:29:16.000000 rrdtool_bindings-0.2.0.dev1/.github/workflows/ci.yml
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     3104 2024-05-26 04:44:38.000000 rrdtool_bindings-0.2.0.dev1/.gitignore
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      735 2024-05-30 07:29:16.000000 rrdtool_bindings-0.2.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     2621 2024-05-30 20:47:03.088302 rrdtool_bindings-0.2.0.dev1/PKG-INFO
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     1706 2024-05-30 20:07:47.000000 rrdtool_bindings-0.2.0.dev1/README.md
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      383 2024-05-30 19:43:59.000000 rrdtool_bindings-0.2.0.dev1/justfile
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)    15883 2024-05-30 07:29:16.000000 rrdtool_bindings-0.2.0.dev1/pdm.lock
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     1859 2024-05-30 20:40:56.000000 rrdtool_bindings-0.2.0.dev1/pyproject.toml
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      416 2024-05-30 19:54:13.000000 rrdtool_bindings-0.2.0.dev1/requirements.txt
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)       38 2024-05-30 20:47:03.088302 rrdtool_bindings-0.2.0.dev1/setup.cfg
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      473 2024-05-30 20:31:04.000000 rrdtool_bindings-0.2.0.dev1/setup.py
+drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:47:03.086303 rrdtool_bindings-0.2.0.dev1/src/
+drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:47:03.087303 rrdtool_bindings-0.2.0.dev1/src/rrdtool/
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)    43262 2024-05-30 20:23:05.000000 rrdtool_bindings-0.2.0.dev1/src/rrdtool/rrdtoolmodule.c
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     1044 2024-05-30 20:23:05.000000 rrdtool_bindings-0.2.0.dev1/src/rrdtool/rrdtoolmodule.h
+drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:47:03.088302 rrdtool_bindings-0.2.0.dev1/src/rrdtool_bindings.egg-info/
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     2621 2024-05-30 20:47:03.000000 rrdtool_bindings-0.2.0.dev1/src/rrdtool_bindings.egg-info/PKG-INFO
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)      415 2024-05-30 20:47:03.000000 rrdtool_bindings-0.2.0.dev1/src/rrdtool_bindings.egg-info/SOURCES.txt
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)        1 2024-05-30 20:47:03.000000 rrdtool_bindings-0.2.0.dev1/src/rrdtool_bindings.egg-info/dependency_links.txt
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)        8 2024-05-30 20:47:03.000000 rrdtool_bindings-0.2.0.dev1/src/rrdtool_bindings.egg-info/top_level.txt
+drwxr-xr-x   0 smsearcy  (1000) smsearcy  (1000)        0 2024-05-30 20:47:03.088302 rrdtool_bindings-0.2.0.dev1/tests/
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)       13 2024-05-29 19:40:46.000000 rrdtool_bindings-0.2.0.dev1/tests/__init__.py
+-rw-r--r--   0 smsearcy  (1000) smsearcy  (1000)     2737 2024-05-30 07:27:48.000000 rrdtool_bindings-0.2.0.dev1/tests/test_bindings.py
```

### Comparing `rrdtool_bindings-0.2.0.dev0/PKG-INFO` & `rrdtool_bindings-0.2.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrdtool-bindings
-Version: 0.2.0.dev0
+Version: 0.2.0.dev1
 Summary: Modern Python packaging for RRDtool C bindings.
 Author: Christian Kroeger, Hye-Shik Chang
 Maintainer: Scott Searcy
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/smsearcy/rrdtool-python-bindings
 Project-URL: Source, https://github.com/smsearcy/rrdtool-python-bindings
 Keywords: rrdtool
```

### Comparing `rrdtool_bindings-0.2.0.dev0/README.md` & `rrdtool_bindings-0.2.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `rrdtool_bindings-0.2.0.dev0/pyproject.toml` & `rrdtool_bindings-0.2.0.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["setuptools>=61", "wheel"]
+requires = ["setuptools>=64", "setuptools_scm>=8", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rrdtool-bindings"
 description = "Modern Python packaging for RRDtool C bindings."
-version = "0.2.0.dev0"
+version = "0.2.0.dev1"
 
 authors = [
   {name = "Christian Kroeger"},
   {name = "Hye-Shik Chang"},
 ]
 maintainers = [
   {name = "Scott Searcy"},
@@ -31,14 +31,17 @@
 license = {text = "GPL-2.0-or-later"}
 keywords = ["rrdtool"]
 
 [project.urls]
 Homepage = "https://github.com/smsearcy/rrdtool-python-bindings"
 Source = "https://github.com/smsearcy/rrdtool-python-bindings"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 testing = [
   "pytest>=8.2.1",
 ]
```

### Comparing `rrdtool_bindings-0.2.0.dev0/src/rrdtool_bindings.egg-info/PKG-INFO` & `rrdtool_bindings-0.2.0.dev1/src/rrdtool_bindings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrdtool-bindings
-Version: 0.2.0.dev0
+Version: 0.2.0.dev1
 Summary: Modern Python packaging for RRDtool C bindings.
 Author: Christian Kroeger, Hye-Shik Chang
 Maintainer: Scott Searcy
 License: GPL-2.0-or-later
 Project-URL: Homepage, https://github.com/smsearcy/rrdtool-python-bindings
 Project-URL: Source, https://github.com/smsearcy/rrdtool-python-bindings
 Keywords: rrdtool
```

### Comparing `rrdtool_bindings-0.2.0.dev0/src/rrdtoolmodule.c` & `rrdtool_bindings-0.2.0.dev1/src/rrdtool/rrdtoolmodule.c`

 * *Files identical despite different names*

### Comparing `rrdtool_bindings-0.2.0.dev0/tests/test_bindings.py` & `rrdtool_bindings-0.2.0.dev1/tests/test_bindings.py`

 * *Files identical despite different names*

