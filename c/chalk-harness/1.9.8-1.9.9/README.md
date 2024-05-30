# Comparing `tmp/chalk-harness-1.9.8.tar.gz` & `tmp/chalk-harness-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalk-harness-1.9.8.tar", last modified: Wed Oct 25 06:58:42 2023, max compression
+gzip compressed data, was "chalk-harness-1.9.9.tar", last modified: Wed Oct 25 18:00:14 2023, max compression
```

## Comparing `chalk-harness-1.9.8.tar` & `chalk-harness-1.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 06:58:42.581804 chalk-harness-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-25 06:58:42.581804 chalk-harness-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 06:58:42.581804 chalk-harness-1.9.8/chalk_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-25 06:58:42.000000 chalk-harness-1.9.8/chalk_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-10-25 06:58:42.000000 chalk-harness-1.9.8/chalk_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 06:58:42.000000 chalk-harness-1.9.8/chalk_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-25 06:58:42.000000 chalk-harness-1.9.8/chalk_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-25 06:58:42.000000 chalk-harness-1.9.8/chalk_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 06:58:42.581804 chalk-harness-1.9.8/chalkharness/
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/chalkharness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/chalkharness/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 06:58:42.581804 chalk-harness-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 06:58:42.581804 chalk-harness-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/tests/SanityTestCase.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 06:58:27.000000 chalk-harness-1.9.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:00:14.166052 chalk-harness-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-25 18:00:14.166052 chalk-harness-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:00:14.162052 chalk-harness-1.9.9/chalk_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2023-10-25 18:00:14.000000 chalk-harness-1.9.9/chalk_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2023-10-25 18:00:14.000000 chalk-harness-1.9.9/chalk_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 18:00:14.000000 chalk-harness-1.9.9/chalk_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-25 18:00:14.000000 chalk-harness-1.9.9/chalk_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-25 18:00:14.000000 chalk-harness-1.9.9/chalk_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:00:14.162052 chalk-harness-1.9.9/chalkharness/
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/chalkharness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/chalkharness/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 18:00:14.166052 chalk-harness-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 18:00:14.162052 chalk-harness-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/tests/SanityTestCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 17:59:59.000000 chalk-harness-1.9.9/tests/__init__.py
```

### Comparing `chalk-harness-1.9.8/PKG-INFO` & `chalk-harness-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.9.8
+Version: 1.9.9
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.9.8/README.md` & `chalk-harness-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.9.8/chalk_harness.egg-info/PKG-INFO` & `chalk-harness-1.9.9/chalk_harness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalk-harness
-Version: 1.9.8
+Version: 1.9.9
 Summary: Python wrapper for Chalk's CLI
 Home-page: https://chalk.ai
 Author: Chalk AI, Inc.
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
```

### Comparing `chalk-harness-1.9.8/chalkharness/__init__.py` & `chalk-harness-1.9.9/chalkharness/__init__.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.9.8/setup.py` & `chalk-harness-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `chalk-harness-1.9.8/tests/SanityTestCase.py` & `chalk-harness-1.9.9/tests/SanityTestCase.py`

 * *Files identical despite different names*

