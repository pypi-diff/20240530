# Comparing `tmp/uugai_python_color_prediction-1.0.0.tar.gz` & `tmp/uugai_python_color_prediction-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uugai_python_color_prediction-1.0.0.tar", last modified: Thu May 30 10:26:18 2024, max compression
+gzip compressed data, was "uugai_python_color_prediction-1.1.0.tar", last modified: Thu May 30 10:42:38 2024, max compression
```

## Comparing `uugai_python_color_prediction-1.0.0.tar` & `uugai_python_color_prediction-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:26:18.488339 uugai_python_color_prediction-1.0.0/
--rw-r--r--   0 glenn      (502) staff       (20)     4014 2024-05-30 10:26:18.488005 uugai_python_color_prediction-1.0.0/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)     3717 2024-05-30 09:44:37.000000 uugai_python_color_prediction-1.0.0/README.md
--rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-30 10:26:18.488431 uugai_python_color_prediction-1.0.0/setup.cfg
--rw-r--r--   0 glenn      (502) staff       (20)      497 2024-05-30 09:42:53.000000 uugai_python_color_prediction-1.0.0/setup.py
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:26:18.484989 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction/
--rw-r--r--   0 glenn      (502) staff       (20)        0 2024-05-30 09:40:23.000000 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction/__init__.py
--rw-r--r--   0 glenn      (502) staff       (20)     9273 2024-05-30 08:51:51.000000 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:26:18.487621 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction.egg-info/
--rw-r--r--   0 glenn      (502) staff       (20)     4014 2024-05-30 10:26:18.000000 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction.egg-info/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)      388 2024-05-30 10:26:18.000000 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction.egg-info/SOURCES.txt
--rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-30 10:26:18.000000 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction.egg-info/dependency_links.txt
--rw-r--r--   0 glenn      (502) staff       (20)      314 2024-05-30 10:26:18.000000 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction.egg-info/requires.txt
--rw-r--r--   0 glenn      (502) staff       (20)       30 2024-05-30 10:26:18.000000 uugai_python_color_prediction-1.0.0/uugai_python_color_prediction.egg-info/top_level.txt
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:42:38.694785 uugai_python_color_prediction-1.1.0/
+-rw-r--r--   0 glenn      (502) staff       (20)     4014 2024-05-30 10:42:38.694517 uugai_python_color_prediction-1.1.0/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)     3717 2024-05-30 09:44:37.000000 uugai_python_color_prediction-1.1.0/README.md
+-rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-30 10:42:38.694888 uugai_python_color_prediction-1.1.0/setup.cfg
+-rw-r--r--   0 glenn      (502) staff       (20)      497 2024-05-30 10:41:38.000000 uugai_python_color_prediction-1.1.0/setup.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:42:38.692375 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/
+-rw-r--r--   0 glenn      (502) staff       (20)        0 2024-05-30 09:40:23.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/__init__.py
+-rw-r--r--   0 glenn      (502) staff       (20)     9273 2024-05-30 08:51:51.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-30 10:42:38.694125 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/
+-rw-r--r--   0 glenn      (502) staff       (20)     4014 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)      388 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/SOURCES.txt
+-rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/dependency_links.txt
+-rw-r--r--   0 glenn      (502) staff       (20)      314 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/requires.txt
+-rw-r--r--   0 glenn      (502) staff       (20)       30 2024-05-30 10:42:38.000000 uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/top_level.txt
```

### Comparing `uugai_python_color_prediction-1.0.0/PKG-INFO` & `uugai_python_color_prediction-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uugai_python_color_prediction
-Version: 1.0.0
+Version: 1.1.0
 Summary: Color prediction Python library used to find the main colors in an image.
 Home-page: UNKNOWN
 Author: uug.ai
 Author-email: support@uug.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `uugai_python_color_prediction-1.0.0/README.md` & `uugai_python_color_prediction-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `uugai_python_color_prediction-1.0.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py` & `uugai_python_color_prediction-1.1.0/uugai_python_color_prediction/uug_ai_python_color_prediction.py`

 * *Files identical despite different names*

### Comparing `uugai_python_color_prediction-1.0.0/uugai_python_color_prediction.egg-info/PKG-INFO` & `uugai_python_color_prediction-1.1.0/uugai_python_color_prediction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uugai-python-color-prediction
-Version: 1.0.0
+Version: 1.1.0
 Summary: Color prediction Python library used to find the main colors in an image.
 Home-page: UNKNOWN
 Author: uug.ai
 Author-email: support@uug.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

