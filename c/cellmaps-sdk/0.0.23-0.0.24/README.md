# Comparing `tmp/cellmaps_sdk-0.0.23.tar.gz` & `tmp/cellmaps_sdk-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmaps_sdk-0.0.23.tar", last modified: Tue May 28 21:50:31 2024, max compression
+gzip compressed data, was "cellmaps_sdk-0.0.24.tar", last modified: Thu May 30 15:49:10 2024, max compression
```

## Comparing `cellmaps_sdk-0.0.23.tar` & `cellmaps_sdk-0.0.24.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-28 21:50:31.609605 cellmaps_sdk-0.0.23/
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.23/LICENSE.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1689 2024-05-28 21:50:31.609253 cellmaps_sdk-0.0.23/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.23/README.rst
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1635 2024-05-28 21:50:10.000000 cellmaps_sdk-0.0.23/pyproject.toml
--rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-05-28 21:50:31.609661 cellmaps_sdk-0.0.23/setup.cfg
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-28 21:50:31.602047 cellmaps_sdk-0.0.23/src/
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-28 21:50:31.607387 cellmaps_sdk-0.0.23/src/cellmaps_sdk/
--rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/__init__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/__main__.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    36834 2024-05-12 11:33:59.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/_cli_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1765 2024-05-10 14:32:03.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/_config.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     9733 2024-05-09 13:35:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/_raw_data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/_test_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1820 2024-04-24 15:54:59.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    35676 2024-05-28 17:01:10.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/data.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/data_utils.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)    29884 2024-05-28 21:49:59.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/process.py
--rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk/py.typed
-drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-28 21:50:31.608589 cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/
--rw-r--r--   0 colmbrandon   (501) staff       (20)     1689 2024-05-28 21:50:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/PKG-INFO
--rw-r--r--   0 colmbrandon   (501) staff       (20)      595 2024-05-28 21:50:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-05-28 21:50:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-05-28 21:50:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/entry_points.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)      196 2024-05-28 21:50:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/requires.txt
--rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-05-28 21:50:31.000000 cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-30 15:49:10.103458 cellmaps_sdk-0.0.24/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.24/LICENSE.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1743 2024-05-30 15:49:10.103188 cellmaps_sdk-0.0.24/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      192 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.24/README.rst
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1682 2024-05-30 15:48:47.000000 cellmaps_sdk-0.0.24/pyproject.toml
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       38 2024-05-30 15:49:10.103509 cellmaps_sdk-0.0.24/setup.cfg
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-30 15:49:10.098543 cellmaps_sdk-0.0.24/src/
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-30 15:49:10.101191 cellmaps_sdk-0.0.24/src/cellmaps_sdk/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      282 2024-02-06 12:12:31.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/__init__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2871 2024-03-07 12:05:00.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/__main__.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    36834 2024-05-12 11:33:59.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/_cli_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1765 2024-05-10 14:32:03.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/_config.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     9733 2024-05-09 13:35:31.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/_raw_data.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     2657 2024-02-12 17:14:01.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/_test_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1820 2024-04-24 15:54:59.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    35676 2024-05-28 17:01:10.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/data.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     4461 2024-02-23 13:18:34.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/data_utils.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)    29884 2024-05-28 21:49:59.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/process.py
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        0 2024-01-26 12:59:01.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk/py.typed
+drwxr-xr-x   0 colmbrandon   (501) staff       (20)        0 2024-05-30 15:49:10.102542 cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/
+-rw-r--r--   0 colmbrandon   (501) staff       (20)     1743 2024-05-30 15:49:10.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      595 2024-05-30 15:49:10.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)        1 2024-05-30 15:49:10.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       55 2024-05-30 15:49:10.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)      198 2024-05-30 15:49:10.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/requires.txt
+-rw-r--r--   0 colmbrandon   (501) staff       (20)       13 2024-05-30 15:49:10.000000 cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/top_level.txt
```

### Comparing `cellmaps_sdk-0.0.23/PKG-INFO` & `cellmaps_sdk-0.0.24/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.23
+Version: 0.0.24
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
 Keywords: Highly-plexed Tissue Imaging,AI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: jinja2
 Requires-Dist: jinja2-strcase
 Requires-Dist: typing
 Requires-Dist: dataclasses
@@ -36,16 +37,16 @@
 Requires-Dist: pandas
 Requires-Dist: mypy
 Requires-Dist: click
 Provides-Extra: r
 Requires-Dist: rpy2; extra == "r"
 Requires-Dist: types-tzlocal; extra == "r"
 Requires-Dist: mypy; extra == "r"
-Provides-Extra: 3-7
-Requires-Dist: typing-extensions; extra == "3-7"
+Provides-Extra: 3-6-7
+Requires-Dist: typing-extensions; extra == "3-6-7"
 
 ...
 
 Environment Variables;
 _utils = [MINIO_HOST,MINIO_ACCESS_KEY,MINIO_SECRET_KEY]
 data = [REVERSE-PROXY-HOST,REVERSE-PROXY-PORT,MINIO_WORKFLOW_BUCKET]
 process = [JMS_ADDRESS,RABBIT_MQ_HOST]
```

### Comparing `cellmaps_sdk-0.0.23/pyproject.toml` & `cellmaps_sdk-0.0.24/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [project]
 name = "cellmaps-sdk"
 authors = [{name = "Colm Brandon", email = "colm.brandon@ul.ie"}]
-version = "0.0.23"
+version = "0.0.24"
 description = "The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME"
 readme = "README.rst"
 license = {file = "LICENSE.txt"}
 keywords = ["Highly-plexed Tissue Imaging", "AI",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
+    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
-requires-python = ">=3.7" # Can potentially expand on this
+requires-python = ">=3.6" # Can potentially expand on this
 
 # [tool.setuptools]
 # package-data= {'key' : ["*.dat"]}
 
 dependencies = [
     "requests",
     "jinja2",
@@ -43,15 +44,15 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [project.optional-dependencies]
 R = ['rpy2', 'types-tzlocal', 'mypy']
-3_7 = ["typing-extensions"]
+3_6_7 = ["typing-extensions"]
 
 [project.urls]
 Homepage = "http://example.com"
 Documentation = "http://example.com"
 Repository = "http://example.com"
 "Bug Tracker" = "http://example.com"
 Changelog = "http://example.com"
```

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/__main__.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/_cli_utils.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/_cli_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/_config.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/_config.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/_raw_data.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/_raw_data.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/_test_utils.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/_test_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/_utils.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/data.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/data.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/data_utils.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/data_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk/process.py` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk/process.py`

 * *Files identical despite different names*

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/PKG-INFO` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: cellmaps-sdk
-Version: 0.0.23
+Version: 0.0.24
 Summary: The SDK for tool builders who wish to integrate their tool into the CellMaps Analysis Workflow IME
 Author-email: Colm Brandon <colm.brandon@ul.ie>
 Project-URL: Homepage, http://example.com
 Project-URL: Documentation, http://example.com
 Project-URL: Repository, http://example.com
 Project-URL: Bug Tracker, http://example.com
 Project-URL: Changelog, http://example.com
 Keywords: Highly-plexed Tissue Imaging,AI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: jinja2
 Requires-Dist: jinja2-strcase
 Requires-Dist: typing
 Requires-Dist: dataclasses
@@ -36,16 +37,16 @@
 Requires-Dist: pandas
 Requires-Dist: mypy
 Requires-Dist: click
 Provides-Extra: r
 Requires-Dist: rpy2; extra == "r"
 Requires-Dist: types-tzlocal; extra == "r"
 Requires-Dist: mypy; extra == "r"
-Provides-Extra: 3-7
-Requires-Dist: typing-extensions; extra == "3-7"
+Provides-Extra: 3-6-7
+Requires-Dist: typing-extensions; extra == "3-6-7"
 
 ...
 
 Environment Variables;
 _utils = [MINIO_HOST,MINIO_ACCESS_KEY,MINIO_SECRET_KEY]
 data = [REVERSE-PROXY-HOST,REVERSE-PROXY-PORT,MINIO_WORKFLOW_BUCKET]
 process = [JMS_ADDRESS,RABBIT_MQ_HOST]
```

### Comparing `cellmaps_sdk-0.0.23/src/cellmaps_sdk.egg-info/SOURCES.txt` & `cellmaps_sdk-0.0.24/src/cellmaps_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

