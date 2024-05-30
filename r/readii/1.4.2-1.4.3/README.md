# Comparing `tmp/readii-1.4.2.tar.gz` & `tmp/readii-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readii-1.4.2.tar", max compression
+gzip compressed data, was "readii-1.4.3.tar", max compression
```

## Comparing `readii-1.4.2.tar` & `readii-1.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1069 2024-05-30 19:20:36.230259 readii-1.4.2/LICENSE
--rw-r--r--   0        0        0     2096 2024-05-30 19:20:36.230259 readii-1.4.2/README.md
--rw-r--r--   0        0        0     1450 2024-05-30 19:21:02.678097 readii-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      100 2024-05-30 19:20:36.230259 readii-1.4.2/src/readii/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 19:20:36.230259 readii-1.4.2/src/readii/data/__init__.py
--rw-r--r--   0        0        0      299 2024-05-30 19:20:36.230259 readii-1.4.2/src/readii/data/default_pyradiomics.yaml
--rw-r--r--   0        0        0    15195 2024-05-30 19:20:36.234259 readii-1.4.2/src/readii/feature_extraction.py
--rw-r--r--   0        0        0    12227 2024-05-30 19:20:36.234259 readii-1.4.2/src/readii/image_processing.py
--rw-r--r--   0        0        0     4192 2024-05-30 19:20:36.234259 readii-1.4.2/src/readii/loaders.py
--rw-r--r--   0        0        0     5959 2024-05-30 19:20:36.234259 readii-1.4.2/src/readii/metadata.py
--rw-r--r--   0        0        0    24474 2024-05-30 19:20:36.234259 readii-1.4.2/src/readii/negative_controls.py
--rw-r--r--   0        0        0     6365 2024-05-30 19:20:36.234259 readii-1.4.2/src/readii/pipeline.py
--rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 readii-1.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2024-05-30 20:10:56.539481 readii-1.4.3/LICENSE
+-rw-r--r--   0        0        0     2096 2024-05-30 20:10:56.539481 readii-1.4.3/README.md
+-rw-r--r--   0        0        0     1450 2024-05-30 20:11:18.791683 readii-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/data/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/data/default_pyradiomics.yaml
+-rw-r--r--   0        0        0    15195 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/feature_extraction.py
+-rw-r--r--   0        0        0    12227 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/image_processing.py
+-rw-r--r--   0        0        0     4192 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/loaders.py
+-rw-r--r--   0        0        0     5959 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/metadata.py
+-rw-r--r--   0        0        0    24474 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/negative_controls.py
+-rw-r--r--   0        0        0     6365 2024-05-30 20:10:56.543481 readii-1.4.3/src/readii/pipeline.py
+-rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 readii-1.4.3/PKG-INFO
```

### Comparing `readii-1.4.2/LICENSE` & `readii-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/README.md` & `readii-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/pyproject.toml` & `readii-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readii"
-version = "1.4.2"
+version = "1.4.3"
 description = "A package to extract radiomic features!"
 authors = ["Katy Scott"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
```

### Comparing `readii-1.4.2/src/readii/feature_extraction.py` & `readii-1.4.3/src/readii/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/src/readii/image_processing.py` & `readii-1.4.3/src/readii/image_processing.py`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/src/readii/loaders.py` & `readii-1.4.3/src/readii/loaders.py`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/src/readii/metadata.py` & `readii-1.4.3/src/readii/metadata.py`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/src/readii/negative_controls.py` & `readii-1.4.3/src/readii/negative_controls.py`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/src/readii/pipeline.py` & `readii-1.4.3/src/readii/pipeline.py`

 * *Files identical despite different names*

### Comparing `readii-1.4.2/PKG-INFO` & `readii-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readii
-Version: 1.4.2
+Version: 1.4.3
 Summary: A package to extract radiomic features!
 License: MIT
 Author: Katy Scott
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

