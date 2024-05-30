# Comparing `tmp/aishalib-0.0.3.tar.gz` & `tmp/aishalib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishalib-0.0.3.tar", last modified: Wed May 29 10:51:48 2024, max compression
+gzip compressed data, was "aishalib-0.0.4.tar", last modified: Thu May 30 11:01:44 2024, max compression
```

## Comparing `aishalib-0.0.3.tar` & `aishalib-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:51:48.905902 aishalib-0.0.3/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.3/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)      597 2024-05-29 10:51:48.901902 aishalib-0.0.3/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-29 10:51:21.000000 aishalib-0.0.3/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-29 10:51:48.905902 aishalib-0.0.3/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:51:48.901902 aishalib-0.0.3/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:51:48.901902 aishalib-0.0.3/src/aishalib/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     3848 2024-05-29 10:48:48.000000 aishalib-0.0.3/src/aishalib/aishalib.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.3/src/aishalib/llmbackend.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-29 10:51:48.901902 aishalib-0.0.3/src/aishalib.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)      597 2024-05-29 10:51:48.000000 aishalib-0.0.3/src/aishalib.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      253 2024-05-29 10:51:48.000000 aishalib-0.0.3/src/aishalib.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-29 10:51:48.000000 aishalib-0.0.3/src/aishalib.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-29 10:51:48.000000 aishalib-0.0.3/src/aishalib.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-29 10:51:48.000000 aishalib-0.0.3/src/aishalib.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.4/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     5892 2024-05-30 11:01:44.056093 aishalib-0.0.4/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     5294 2024-05-30 10:59:59.000000 aishalib-0.0.4/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-30 11:01:36.000000 aishalib-0.0.4/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-30 11:01:44.056093 aishalib-0.0.4/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/src/aishalib/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     3848 2024-05-29 10:48:48.000000 aishalib-0.0.4/src/aishalib/aishalib.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.4/src/aishalib/llmbackend.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/src/aishalib.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     5892 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/top_level.txt
```

### Comparing `aishalib-0.0.3/LICENSE` & `aishalib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.3/pyproject.toml` & `aishalib-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aishalib"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
 description = "AI Smart Human Assistant Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `aishalib-0.0.3/src/aishalib/aishalib.py` & `aishalib-0.0.4/src/aishalib/aishalib.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.3/src/aishalib/llmbackend.py` & `aishalib-0.0.4/src/aishalib/llmbackend.py`

 * *Files identical despite different names*

