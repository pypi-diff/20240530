# Comparing `tmp/redbacktechpy-0.5.0.tar.gz` & `tmp/redbacktechpy-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-0.5.0.tar", last modified: Thu May 30 07:45:47 2024, max compression
+gzip compressed data, was "redbacktechpy-0.5.5.tar", last modified: Thu May 30 08:07:06 2024, max compression
```

## Comparing `redbacktechpy-0.5.0.tar` & `redbacktechpy-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.830552 redbacktechpy-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.830552 redbacktechpy-0.5.0/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26024 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:07:06.477346 redbacktechpy-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 08:07:06.477346 redbacktechpy-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:07:06.477346 redbacktechpy-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:07:06.473346 redbacktechpy-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:07:06.477346 redbacktechpy-0.5.5/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26024 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 08:07:01.000000 redbacktechpy-0.5.5/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:07:06.477346 redbacktechpy-0.5.5/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 08:07:06.000000 redbacktechpy-0.5.5/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 08:07:06.000000 redbacktechpy-0.5.5/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:07:06.000000 redbacktechpy-0.5.5/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 08:07:06.000000 redbacktechpy-0.5.5/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 08:07:06.000000 redbacktechpy-0.5.5/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-0.5.0/LICENSE` & `redbacktechpy-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.5.0/PKG-INFO` & `redbacktechpy-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 0.5.0
+Version: 0.5.5
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-0.5.0/pyproject.toml` & `redbacktechpy-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "0.5.0"
+version = "0.5.5"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-0.5.0/src/redbacktechpy/__init__.py` & `redbacktechpy-0.5.5/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.5.0/src/redbacktechpy/constants.py` & `redbacktechpy-0.5.5/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.5.0/src/redbacktechpy/model.py` & `redbacktechpy-0.5.5/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.5.0/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-0.5.5/src/redbacktechpy/redbacktech_client.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.5.0/src/redbacktechpy/str_enum.py` & `redbacktechpy-0.5.5/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.5.0/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-0.5.5/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 0.5.0
+Version: 0.5.5
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

