# Comparing `tmp/bees-challenge-0.8.0.tar.gz` & `tmp/bees-challenge-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bees-challenge-0.8.0.tar", last modified: Thu May 30 06:17:55 2024, max compression
+gzip compressed data, was "bees-challenge-0.9.0.tar", last modified: Thu May 30 06:22:22 2024, max compression
```

## Comparing `bees-challenge-0.8.0.tar` & `bees-challenge-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:55.763722 bees-challenge-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-30 06:17:55.763722 bees-challenge-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:55.759722 bees-challenge-0.8.0/bees_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-30 06:17:55.000000 bees-challenge-0.8.0/bees_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 06:17:55.000000 bees-challenge-0.8.0/bees_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:17:55.000000 bees-challenge-0.8.0/bees_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 06:17:55.000000 bees-challenge-0.8.0/bees_challenge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:17:55.000000 bees-challenge-0.8.0/bees_challenge.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:55.759722 bees-challenge-0.8.0/fuel_efficency/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 06:17:55.000000 bees-challenge-0.8.0/fuel_efficency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:55.759722 bees-challenge-0.8.0/fuel_efficency/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/algorithms/a_star.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/algorithms/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/algorithms/dijkstra.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/algorithms/path_finding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:55.759722 bees-challenge-0.8.0/fuel_efficency/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/entities/down_hill.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/entities/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/entities/plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/entities/position.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/entities/up_hill.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/fuel_efficency/entities/valley.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:17:55.763722 bees-challenge-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 06:17:55.000000 bees-challenge-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:55.759722 bees-challenge-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/tests/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/tests/test_ci.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-30 06:17:35.000000 bees-challenge-0.8.0/tests/test_entities_raise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:22.706396 bees-challenge-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-30 06:22:22.706396 bees-challenge-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:22.702396 bees-challenge-0.9.0/bees_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-30 06:22:22.000000 bees-challenge-0.9.0/bees_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-30 06:22:22.000000 bees-challenge-0.9.0/bees_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:22:22.000000 bees-challenge-0.9.0/bees_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 06:22:22.000000 bees-challenge-0.9.0/bees_challenge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:22:22.000000 bees-challenge-0.9.0/bees_challenge.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:22.702396 bees-challenge-0.9.0/fuel_efficency/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 06:22:22.000000 bees-challenge-0.9.0/fuel_efficency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:22.702396 bees-challenge-0.9.0/fuel_efficency/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/algorithms/a_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/algorithms/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/algorithms/dijkstra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/algorithms/path_finding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:22.702396 bees-challenge-0.9.0/fuel_efficency/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/entities/down_hill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/entities/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/entities/plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/entities/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/entities/up_hill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/fuel_efficency/entities/valley.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:22:22.706396 bees-challenge-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 06:22:22.000000 bees-challenge-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:22.706396 bees-challenge-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/tests/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/tests/test_ci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-30 06:22:03.000000 bees-challenge-0.9.0/tests/test_entities_raise.py
```

### Comparing `bees-challenge-0.8.0/PKG-INFO` & `bees-challenge-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bees-challenge
-Version: 0.8.0
+Version: 0.9.0
 Summary: challenge submission for the bees ml path challenge
 Home-page: https://github.com/yuiti-ara/yuiti-bees-ml-path-challenge
 Author: yuiti
 Author-email: yuiti.usp@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bees-challenge-0.8.0/README.md` & `bees-challenge-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bees-challenge-0.8.0/bees_challenge.egg-info/PKG-INFO` & `bees-challenge-0.9.0/bees_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bees-challenge
-Version: 0.8.0
+Version: 0.9.0
 Summary: challenge submission for the bees ml path challenge
 Home-page: https://github.com/yuiti-ara/yuiti-bees-ml-path-challenge
 Author: yuiti
 Author-email: yuiti.usp@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `bees-challenge-0.8.0/bees_challenge.egg-info/SOURCES.txt` & `bees-challenge-0.9.0/bees_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bees-challenge-0.8.0/fuel_efficency/algorithms/context.py` & `bees-challenge-0.9.0/fuel_efficency/algorithms/context.py`

 * *Files identical despite different names*

### Comparing `bees-challenge-0.8.0/fuel_efficency/entities/position.py` & `bees-challenge-0.9.0/fuel_efficency/entities/position.py`

 * *Files identical despite different names*

### Comparing `bees-challenge-0.8.0/setup.py` & `bees-challenge-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bees-challenge',
-    version='0.8.0',
+    version='0.9.0',
     author='yuiti',
     author_email='yuiti.usp@gmail.com',
     description='challenge submission for the bees ml path challenge',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yuiti-ara/yuiti-bees-ml-path-challenge',
     packages=find_packages(),
```

### Comparing `bees-challenge-0.8.0/tests/test_algorithms.py` & `bees-challenge-0.9.0/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `bees-challenge-0.8.0/tests/test_entities.py` & `bees-challenge-0.9.0/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `bees-challenge-0.8.0/tests/test_entities_raise.py` & `bees-challenge-0.9.0/tests/test_entities_raise.py`

 * *Files identical despite different names*

