# Comparing `tmp/kebbie-0.3.0.tar.gz` & `tmp/kebbie-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kebbie-0.3.0.tar", last modified: Tue May 28 09:58:28 2024, max compression
+gzip compressed data, was "kebbie-0.3.1.tar", last modified: Thu May 30 10:25:00 2024, max compression
```

## Comparing `kebbie-0.3.0.tar` & `kebbie-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:58:28.863760 kebbie-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 09:58:24.000000 kebbie-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-28 09:58:28.863760 kebbie-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-28 09:58:24.000000 kebbie-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:58:28.863760 kebbie-0.3.0/kebbie/
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/correctors.py
--rw-r--r--   0 runner    (1001) docker     (127)    51089 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/emulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/gesture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/noise_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-28 09:58:24.000000 kebbie-0.3.0/kebbie/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:58:28.863760 kebbie-0.3.0/kebbie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 09:58:28.000000 kebbie-0.3.0/kebbie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-28 09:58:24.000000 kebbie-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:58:28.863760 kebbie-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 09:58:24.000000 kebbie-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:25:00.192767 kebbie-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 10:24:55.000000 kebbie-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-30 10:25:00.192767 kebbie-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-30 10:24:55.000000 kebbie-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:25:00.188767 kebbie-0.3.1/kebbie/
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51089 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/gesture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-30 10:24:55.000000 kebbie-0.3.1/kebbie/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:25:00.192767 kebbie-0.3.1/kebbie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-30 10:25:00.000000 kebbie-0.3.1/kebbie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 10:25:00.000000 kebbie-0.3.1/kebbie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:25:00.000000 kebbie-0.3.1/kebbie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 10:25:00.000000 kebbie-0.3.1/kebbie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-30 10:25:00.000000 kebbie-0.3.1/kebbie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 10:25:00.000000 kebbie-0.3.1/kebbie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-30 10:24:55.000000 kebbie-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:25:00.192767 kebbie-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 10:24:55.000000 kebbie-0.3.1/setup.py
```

### Comparing `kebbie-0.3.0/LICENSE` & `kebbie-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/PKG-INFO` & `kebbie-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kebbie-0.3.0/README.md` & `kebbie-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/__init__.py` & `kebbie-0.3.1/kebbie/__init__.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/cmd.py` & `kebbie-0.3.1/kebbie/cmd.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/correctors.py` & `kebbie-0.3.1/kebbie/correctors.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/emulator.py` & `kebbie-0.3.1/kebbie/emulator.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/gesture.py` & `kebbie-0.3.1/kebbie/gesture.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/layout.py` & `kebbie-0.3.1/kebbie/layout.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/noise_model.py` & `kebbie-0.3.1/kebbie/noise_model.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/oracle.py` & `kebbie-0.3.1/kebbie/oracle.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/scorer.py` & `kebbie-0.3.1/kebbie/scorer.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/tokenizer.py` & `kebbie-0.3.1/kebbie/tokenizer.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie/utils.py` & `kebbie-0.3.1/kebbie/utils.py`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/kebbie.egg-info/PKG-INFO` & `kebbie-0.3.1/kebbie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kebbie
-Version: 0.3.0
+Version: 0.3.1
 Summary: A small framework to test and compare mobile keyboards
 Home-page: https://github.com/FleksySDK/kebbie
 Author: Nicolas REMOND
 Author-email: nicolas.remond@thingthing.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kebbie-0.3.0/kebbie.egg-info/requires.txt` & `kebbie-0.3.1/kebbie.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/pyproject.toml` & `kebbie-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kebbie-0.3.0/setup.py` & `kebbie-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 extras_require["all"] = sum(extras_require.values(), [])
 extras_require["dev"] = (
     extras_require["test"] + extras_require["hook"] + extras_require["lint"] + extras_require["docs"]
 )
 
 setuptools.setup(
     name="kebbie",
-    version="0.3.0",
+    version="0.3.1",
     author="Nicolas REMOND",
     author_email="nicolas.remond@thingthing.co",
     description="A small framework to test and compare mobile keyboards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FleksySDK/kebbie",
     packages=setuptools.find_packages(),
```

