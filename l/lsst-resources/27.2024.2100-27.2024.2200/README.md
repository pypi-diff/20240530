# Comparing `tmp/lsst_resources-27.2024.2100.tar.gz` & `tmp/lsst_resources-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_resources-27.2024.2100.tar", last modified: Thu May 23 10:09:47 2024, max compression
+gzip compressed data, was "lsst_resources-27.2024.2200.tar", last modified: Thu May 30 09:57:28 2024, max compression
```

## Comparing `lsst_resources-27.2024.2100.tar` & `lsst_resources-27.2024.2200.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.459575 lsst_resources-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-23 10:09:47.459575 lsst_resources-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.447575 lsst_resources-27.2024.2100/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.447575 lsst_resources-27.2024.2100/doc/lsst.resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/doc/lsst.resources/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/doc/lsst.resources/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/doc/lsst.resources/internal-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.447575 lsst_resources-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.447575 lsst_resources-27.2024.2100/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.451575 lsst_resources-27.2024.2100/python/lsst/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.455575 lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)    58003 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/_resourcePath.py
--rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70133 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/packageresource.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/schemeless.py
--rw-r--r--   0 runner    (1001) docker     (127)    36780 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/python/lsst/resources/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:09:47.000000 lsst_resources-27.2024.2100/python/lsst/resources/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.455575 lsst_resources-27.2024.2100/python/lsst_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-23 10:09:47.000000 lsst_resources-27.2024.2100/python/lsst_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 10:09:47.000000 lsst_resources-27.2024.2100/python/lsst_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:09:47.000000 lsst_resources-27.2024.2100/python/lsst_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-23 10:09:47.000000 lsst_resources-27.2024.2100/python/lsst_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:09:47.000000 lsst_resources-27.2024.2100/python/lsst_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:09:47.000000 lsst_resources-27.2024.2100/python/lsst_resources.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 10:09:47.459575 lsst_resources-27.2024.2100/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:47.455575 lsst_resources-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_gs.py
--rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_s3utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-23 10:09:40.000000 lsst_resources-27.2024.2100/tests/test_schemeless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.599482 lsst_resources-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-30 09:57:28.599482 lsst_resources-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.587482 lsst_resources-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.591482 lsst_resources-27.2024.2200/doc/lsst.resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/doc/lsst.resources/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/doc/lsst.resources/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/doc/lsst.resources/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.591482 lsst_resources-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.591482 lsst_resources-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.595482 lsst_resources-27.2024.2200/python/lsst/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.595482 lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_baseResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_fileResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_httpResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58003 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/_resourcePath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21878 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70133 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/packageresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21730 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/schemeless.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37990 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/python/lsst/resources/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:57:28.000000 lsst_resources-27.2024.2200/python/lsst/resources/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.599482 lsst_resources-27.2024.2200/python/lsst_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-30 09:57:28.000000 lsst_resources-27.2024.2200/python/lsst_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-30 09:57:28.000000 lsst_resources-27.2024.2200/python/lsst_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:57:28.000000 lsst_resources-27.2024.2200/python/lsst_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-30 09:57:28.000000 lsst_resources-27.2024.2200/python/lsst_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:57:28.000000 lsst_resources-27.2024.2200/python/lsst_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:57:28.000000 lsst_resources-27.2024.2200/python/lsst_resources.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 09:57:28.599482 lsst_resources-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:57:28.599482 lsst_resources-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_gs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-30 09:57:21.000000 lsst_resources-27.2024.2200/tests/test_schemeless.py
```

### Comparing `lsst_resources-27.2024.2100/LICENSE` & `lsst_resources-27.2024.2200/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/PKG-INFO` & `lsst_resources-27.2024.2200/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_resources-27.2024.2100/README.md` & `lsst_resources-27.2024.2200/README.md`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/doc/lsst.resources/CHANGES.rst` & `lsst_resources-27.2024.2200/doc/lsst.resources/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/doc/lsst.resources/index.rst` & `lsst_resources-27.2024.2200/doc/lsst.resources/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/pyproject.toml` & `lsst_resources-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/__init__.py` & `lsst_resources-27.2024.2200/python/lsst/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_baseResourceHandle.py` & `lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_baseResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_fileResourceHandle.py` & `lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_fileResourceHandle.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_httpResourceHandle.py` & `lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_httpResourceHandle.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from collections.abc import Callable, Iterable
 from logging import Logger
 from typing import AnyStr, NamedTuple
 
 import requests
 from lsst.utils.timer import time_this
 
+from .._resourcePath import ResourcePath
 from ._baseResourceHandle import BaseResourceHandle, CloseStatus
 
 
 class HttpReadResourceHandle(BaseResourceHandle[bytes]):
     """HTTP-based specialization of `.BaseResourceHandle`.
 
     Parameters
@@ -71,14 +72,15 @@
         self._timeout = timeout
 
         self._completeBuffer: io.BytesIO | None = None
 
         self._closed = CloseStatus.OPEN
         self._current_position = 0
         self._eof = False
+        self._total_size = -1  # Unknown
 
     def close(self) -> None:
         self._closed = CloseStatus.CLOSED
         self._completeBuffer = None
         self._eof = True
 
     @property
@@ -102,20 +104,27 @@
 
     def readline(self, size: int = -1) -> bytes:
         raise io.UnsupportedOperation("HttpReadResourceHandles Do not support line by line reading")
 
     def readlines(self, size: int = -1) -> Iterable[bytes]:
         raise io.UnsupportedOperation("HttpReadResourceHandles Do not support line by line reading")
 
+    def _size(self) -> int:
+        if self._total_size == -1:
+            self._total_size = ResourcePath(self._url).size()
+        return self._total_size
+
     def seek(self, offset: int, whence: int = io.SEEK_SET) -> int:
         self._eof = False
         if whence == io.SEEK_CUR and (self._current_position + offset) >= 0:
             self._current_position += offset
         elif whence == io.SEEK_SET and offset >= 0:
             self._current_position = offset
+        elif whence == io.SEEK_END:
+            self._current_position = self._size() + offset
         else:
             raise io.UnsupportedOperation("Seek value is incorrect, or whence mode is unsupported")
 
         # handle if the complete file has be read already
         if self._completeBuffer is not None:
             self._completeBuffer.seek(self._current_position, whence)
         return self._current_position
@@ -186,39 +195,33 @@
             return b""
 
         if (code := resp.status_code) not in (requests.codes.ok, requests.codes.partial):
             raise FileNotFoundError(
                 f"Unable to read resource {self._url}, or bytes are out of range; status code: {code}"
             )
 
-        len_content = len(resp.content)
-
-        # verify this is not actually the whole file and the server did not lie
-        # about supporting ranges
-        if len_content > size or code != requests.codes.partial:
-            self._completeBuffer = io.BytesIO()
-            self._completeBuffer.write(resp.content)
-            self._completeBuffer.seek(0)
-            return self.read(size=size)
-
         # The response header should tell us the total number of bytes
         # in the file and also the current position we have got to in the
         # server.
         if "Content-Range" in resp.headers:
             content_range = parse_content_range_header(resp.headers["Content-Range"])
+            if content_range.total is not None:
+                # Store in case we need this later.
+                self._total_size = content_range.total
             if (
                 content_range.total is not None
                 and content_range.range_end is not None
                 and content_range.range_end >= content_range.total - 1
             ):
                 self._eof = True
 
         # Try to guess that we overran the end. This will not help if we
         # read exactly the number of bytes to get us to the end and so we
         # will need to do one more read and get a 416.
+        len_content = len(resp.content)
         if len_content < size:
             self._eof = True
 
         self._current_position += len_content
         return resp.content
```

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py` & `lsst_resources-27.2024.2200/python/lsst/resources/_resourceHandles/_s3ResourceHandle.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from logging import Logger
 from typing import TYPE_CHECKING
 
 from botocore.exceptions import ClientError
 from lsst.utils.introspection import find_outside_stacklevel
 from lsst.utils.timer import time_this
 
+from .._resourcePath import ResourcePath
 from ..s3utils import all_retryable_errors, backoff, max_retry_time
 from ._baseResourceHandle import BaseResourceHandle, CloseStatus
 
 if TYPE_CHECKING:
     import boto3
 
 
@@ -42,14 +43,16 @@
     client : `boto3.client`
         An existing boto3 client that will be used for interacting with the
         remote s3 server.
     bucket : `str`
         The name of the s3 bucket of this resource.
     key : `str`
         The identifier of the resource within the specified bucket.
+    uri : `ResourcePath`
+        The `ResourcePath` object corresponding to this handle.
     newline : `str`
         When doing multiline operations, break the stream on given character.
         Defaults to newline.
 
     Notes
     -----
     It is only possible to incrementally flush this object if each chunk that
@@ -70,28 +73,37 @@
 
     S3 handles only support operations in binary mode. To get other modes of
     reading and writing, wrap this handle inside an `io.TextIOWrapper` context
     manager. An example of this can be found in `S3ResourcePath`.
     """
 
     def __init__(
-        self, mode: str, log: Logger, client: boto3.client, bucket: str, key: str, newline: bytes = b"\n"
+        self,
+        mode: str,
+        log: Logger,
+        client: boto3.client,
+        bucket: str,
+        key: str,
+        uri: ResourcePath,
+        newline: bytes = b"\n",
     ):
         super().__init__(mode, log, newline=newline)
         self._client = client
         self._bucket = bucket
         self._key = key
         self._buffer = BytesIO()
         self._position = 0
         self._writable = False
         self._last_flush_position: int | None = None
         self._warned = False
         self._readable = bool({"r", "+"} & set(self._mode))
         self._max_size: int | None = None
         self._recursing = False
+        self._uri = uri
+        self._total_size = -1  # Unknown size.
         if {"w", "a", "x", "+"} & set(self._mode):
             self._writable = True
             self._multiPartUpload = client.create_multipart_upload(Bucket=bucket, Key=key)
             self._partNo = 1
             self._parts: list[Mapping] = []
             # Below is a workaround for append mode. It basically must read in
             # everything that exists in the file so that it is in the buffer to
@@ -206,14 +218,20 @@
         self._last_flush_position = self._buffer.tell() + (self._last_flush_position or 0)
         self._buffer = BytesIO()
 
     @property
     def isatty(self) -> bool:
         return False
 
+    def _size(self) -> int:
+        # To allow SEEK_END to work.
+        if self._total_size == -1:
+            self._total_size = self._uri.size()
+        return self._total_size
+
     def readable(self) -> bool:
         return self._readable
 
     def readline(self, size: int = -1) -> bytes:
         raise OSError("S3 Does not support line by line reads")
 
     def readlines(self, hint: int = -1) -> Iterable[bytes]:
@@ -235,16 +253,15 @@
             self._position = self._buffer.tell()
         else:
             if whence == SEEK_SET:
                 self._position = offset
             elif whence == SEEK_CUR:
                 self._position += offset
             elif whence == SEEK_END:
-                offset = abs(offset)
-                self._position -= offset
+                self._position = self._size() + offset
         return self._position
 
     def seekable(self) -> bool:
         return True
 
     def truncate(self, size: int | None = None) -> int:
         if self.writable():
```

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/_resourcePath.py` & `lsst_resources-27.2024.2200/python/lsst/resources/_resourcePath.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/file.py` & `lsst_resources-27.2024.2200/python/lsst/resources/file.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/gs.py` & `lsst_resources-27.2024.2200/python/lsst/resources/gs.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/http.py` & `lsst_resources-27.2024.2200/python/lsst/resources/http.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/location.py` & `lsst_resources-27.2024.2200/python/lsst/resources/location.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/mem.py` & `lsst_resources-27.2024.2200/python/lsst/resources/mem.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/packageresource.py` & `lsst_resources-27.2024.2200/python/lsst/resources/packageresource.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/s3.py` & `lsst_resources-27.2024.2200/python/lsst/resources/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,15 +540,17 @@
     @contextlib.contextmanager
     def _openImpl(
         self,
         mode: str = "r",
         *,
         encoding: str | None = None,
     ) -> Iterator[ResourceHandleProtocol]:
-        with S3ResourceHandle(mode, log, self.client, self._bucket, self.relativeToPathRoot) as handle:
+        with S3ResourceHandle(
+            mode, log, self.client, self._bucket, self.relativeToPathRoot, uri=self
+        ) as handle:
             if "b" in mode:
                 yield handle
             else:
                 if encoding is None:
                     encoding = sys.getdefaultencoding()
                 # cast because the protocol is compatible, but does not have
                 # BytesIO in the inheritance tree
```

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/s3utils.py` & `lsst_resources-27.2024.2200/python/lsst/resources/s3utils.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/schemeless.py` & `lsst_resources-27.2024.2200/python/lsst/resources/schemeless.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/tests.py` & `lsst_resources-27.2024.2200/python/lsst/resources/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,37 @@
             test_case.assertEqual(read_buffer.read(), double_content)
         # Final mode to check is w+, which does read/write but truncates first.
         with uri.open("w+" + mode_suffix, **kwargs) as rw_buffer:
             test_case.assertEqual(rw_buffer.read(), empty_content_by_mode_suffix[mode_suffix])
             rw_buffer.write(content)
             rw_buffer.seek(0)
             test_case.assertEqual(rw_buffer.read(), content)
+        # Check that two seeks with reads to end return correctly.
+        # Seek is only reliable with "b" mode.
+        if mode_suffix == "b":
+            with uri.open("r" + mode_suffix, **kwargs) as read_buffer:
+                size = len(content)
+                seek1 = 2 * size // 3
+                read_buffer.seek(seek1)
+                content1 = read_buffer.read()
+                test_case.assertEqual(len(content1), size - seek1)
+                # Seek earlier and then read to end.
+                seek2 = size // 2
+                read_buffer.seek(seek2)
+                content2 = read_buffer.read()
+                test_case.assertEqual(len(content2), size - seek2)
+            # Check that we can seek from end and read and seek and read.
+            # Negative seek only works in binary mode.
+            with uri.open("rb", **kwargs) as read_buffer:
+                read_buffer.seek(-5, 2)  # Relative to end
+                content_read = read_buffer.read()
+                test_case.assertEqual(len(content_read), 5)
+                read_buffer.seek(-10, 2)  # Relative to end
+                content_read = read_buffer.read()
+                test_case.assertEqual(len(content_read), 10)
         with uri.open("r" + mode_suffix, **kwargs) as read_buffer:
             test_case.assertEqual(read_buffer.read(), content)
         # Remove file to make room for the next loop of tests with this URI.
         uri.remove()
 
 
 if TYPE_CHECKING:
```

### Comparing `lsst_resources-27.2024.2100/python/lsst/resources/utils.py` & `lsst_resources-27.2024.2200/python/lsst/resources/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/python/lsst_resources.egg-info/PKG-INFO` & `lsst_resources-27.2024.2200/python/lsst_resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-resources
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: An abstraction layer for reading and writing from URI file resources.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/resources
 Keywords: lsst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_resources-27.2024.2100/python/lsst_resources.egg-info/SOURCES.txt` & `lsst_resources-27.2024.2200/python/lsst_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_file.py` & `lsst_resources-27.2024.2200/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_gs.py` & `lsst_resources-27.2024.2200/tests/test_gs.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_http.py` & `lsst_resources-27.2024.2200/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_location.py` & `lsst_resources-27.2024.2200/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_mem.py` & `lsst_resources-27.2024.2200/tests/test_mem.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_resource.py` & `lsst_resources-27.2024.2200/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_s3.py` & `lsst_resources-27.2024.2200/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_s3utils.py` & `lsst_resources-27.2024.2200/tests/test_s3utils.py`

 * *Files identical despite different names*

### Comparing `lsst_resources-27.2024.2100/tests/test_schemeless.py` & `lsst_resources-27.2024.2200/tests/test_schemeless.py`

 * *Files identical despite different names*

