# Comparing `tmp/testpythonpackagelibialany-1.0.7.tar.gz` & `tmp/testpythonpackagelibialany-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpythonpackagelibialany-1.0.7.tar", last modified: Thu May 30 14:46:21 2024, max compression
+gzip compressed data, was "testpythonpackagelibialany-1.0.9.tar", last modified: Thu May 30 14:58:38 2024, max compression
```

## Comparing `testpythonpackagelibialany-1.0.7.tar` & `testpythonpackagelibialany-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 aibil     (1000) aibil     (1000)        0 2024-05-30 14:46:21.300541 testpythonpackagelibialany-1.0.7/
--rw-r--r--   0 aibil     (1000) aibil     (1000)     1067 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/LICENSE
--rw-r--r--   0 aibil     (1000) aibil     (1000)        0 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/LICENSE.txt
--rw-r--r--   0 aibil     (1000) aibil     (1000)      668 2024-05-30 14:46:21.300541 testpythonpackagelibialany-1.0.7/PKG-INFO
--rw-r--r--   0 aibil     (1000) aibil     (1000)       40 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/README.md
--rw-r--r--   0 aibil     (1000) aibil     (1000)      317 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/README.rst
--rw-r--r--   0 aibil     (1000) aibil     (1000)       84 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/pyproject.toml
--rw-r--r--   0 aibil     (1000) aibil     (1000)      728 2024-05-30 14:46:21.300541 testpythonpackagelibialany-1.0.7/setup.cfg
--rw-r--r--   0 aibil     (1000) aibil     (1000)       37 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/setup.py
-drwxr-xr-x   0 aibil     (1000) aibil     (1000)        0 2024-05-30 14:46:21.296541 testpythonpackagelibialany-1.0.7/src/
-drwxr-xr-x   0 aibil     (1000) aibil     (1000)        0 2024-05-30 14:46:21.296541 testpythonpackagelibialany-1.0.7/src/divide/
--rw-r--r--   0 aibil     (1000) aibil     (1000)        0 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/src/divide/__init__.py
--rw-r--r--   0 aibil     (1000) aibil     (1000)       42 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/src/divide/divide_by_three.py
-drwxr-xr-x   0 aibil     (1000) aibil     (1000)        0 2024-05-30 14:46:21.296541 testpythonpackagelibialany-1.0.7/src/testpythonpackagelibialany.egg-info/
--rw-r--r--   0 aibil     (1000) aibil     (1000)      668 2024-05-30 14:46:21.000000 testpythonpackagelibialany-1.0.7/src/testpythonpackagelibialany.egg-info/PKG-INFO
--rw-r--r--   0 aibil     (1000) aibil     (1000)      373 2024-05-30 14:46:21.000000 testpythonpackagelibialany-1.0.7/src/testpythonpackagelibialany.egg-info/SOURCES.txt
--rw-r--r--   0 aibil     (1000) aibil     (1000)        1 2024-05-30 14:46:21.000000 testpythonpackagelibialany-1.0.7/src/testpythonpackagelibialany.egg-info/dependency_links.txt
--rw-r--r--   0 aibil     (1000) aibil     (1000)        7 2024-05-30 14:46:21.000000 testpythonpackagelibialany-1.0.7/src/testpythonpackagelibialany.egg-info/top_level.txt
-drwxr-xr-x   0 aibil     (1000) aibil     (1000)        0 2024-05-30 14:46:21.296541 testpythonpackagelibialany-1.0.7/tests/
--rw-r--r--   0 aibil     (1000) aibil     (1000)      207 2024-05-30 13:41:54.000000 testpythonpackagelibialany-1.0.7/tests/test_divide_by_three.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:58:38.022782 testpythonpackagelibialany-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 14:58:38.022782 testpythonpackagelibialany-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-30 14:58:38.026782 testpythonpackagelibialany-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:58:38.022782 testpythonpackagelibialany-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:58:38.022782 testpythonpackagelibialany-1.0.9/src/divide/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/src/divide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/src/divide/divide_by_three.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:58:38.022782 testpythonpackagelibialany-1.0.9/src/testpythonpackagelibialany.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 14:58:38.000000 testpythonpackagelibialany-1.0.9/src/testpythonpackagelibialany.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 14:58:38.000000 testpythonpackagelibialany-1.0.9/src/testpythonpackagelibialany.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:58:38.000000 testpythonpackagelibialany-1.0.9/src/testpythonpackagelibialany.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 14:58:38.000000 testpythonpackagelibialany-1.0.9/src/testpythonpackagelibialany.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:58:38.022782 testpythonpackagelibialany-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 14:58:34.000000 testpythonpackagelibialany-1.0.9/tests/test_divide_by_three.py
```

### Comparing `testpythonpackagelibialany-1.0.7/LICENSE` & `testpythonpackagelibialany-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `testpythonpackagelibialany-1.0.7/PKG-INFO` & `testpythonpackagelibialany-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpythonpackagelibialany
-Version: 1.0.7
+Version: 1.0.9
 Summary: A simple Python package
 Home-page: https://github.com/libialany/testPythonPackage
 Author: elibialany
 Author-email: elibialany@gmail.com
 Project-URL: Bug Tracker, https://github.com/libialany/testPythonPackage/-/issues
 Project-URL: repository, https://github.com/libialany/testPythonPackage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testpythonpackagelibialany-1.0.7/setup.cfg` & `testpythonpackagelibialany-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = testpythonpackagelibialany
-version = 1.0.7
+version = 1.0.9
 author = elibialany
 author_email = elibialany@gmail.com
 description = A simple Python package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/libialany/testPythonPackage
 project_urls =
```

### Comparing `testpythonpackagelibialany-1.0.7/src/testpythonpackagelibialany.egg-info/PKG-INFO` & `testpythonpackagelibialany-1.0.9/src/testpythonpackagelibialany.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpythonpackagelibialany
-Version: 1.0.7
+Version: 1.0.9
 Summary: A simple Python package
 Home-page: https://github.com/libialany/testPythonPackage
 Author: elibialany
 Author-email: elibialany@gmail.com
 Project-URL: Bug Tracker, https://github.com/libialany/testPythonPackage/-/issues
 Project-URL: repository, https://github.com/libialany/testPythonPackage
 Classifier: Programming Language :: Python :: 3
```

