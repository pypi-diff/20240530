# Comparing `tmp/sentiment_analysis_model-0.0.5.tar.gz` & `tmp/sentiment_analysis_model-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_model-0.0.5.tar", last modified: Thu May 30 09:03:24 2024, max compression
+gzip compressed data, was "sentiment_analysis_model-0.0.6.tar", last modified: Thu May 30 09:13:52 2024, max compression
```

## Comparing `sentiment_analysis_model-0.0.5.tar` & `sentiment_analysis_model-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:24.971016 sentiment_analysis_model-0.0.5/
--rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      241 2024-05-30 09:03:24.970038 sentiment_analysis_model-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.5/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:24.954027 sentiment_analysis_model-0.0.5/sentiment_analysis_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:24.962016 sentiment_analysis_model-0.0.5/sentiment_analysis_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/config/__init__.py
--rw-rw-rw-   0        0        0     1165 2024-05-30 08:47:19.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/config/core.py
--rw-rw-rw-   0        0        0      428 2024-05-30 07:45:43.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/pipeline.py
--rw-rw-rw-   0        0        0      548 2024-05-30 07:45:21.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:24.966012 sentiment_analysis_model-0.0.5/sentiment_analysis_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/processing/__init__.py
--rw-rw-rw-   0        0        0      282 2024-05-30 08:47:16.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/processing/data_manager.py
--rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-30 08:33:20.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/processing/validation.py
--rw-rw-rw-   0        0        0     1692 2024-05-30 07:50:16.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:24.969039 sentiment_analysis_model-0.0.5/sentiment_analysis_model.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-30 09:03:24.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-05-30 09:03:24.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 09:03:24.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-30 09:03:24.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-30 09:03:24.000000 sentiment_analysis_model-0.0.5/sentiment_analysis_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-30 09:03:24.972012 sentiment_analysis_model-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-30 09:00:40.000000 sentiment_analysis_model-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:03:24.968037 sentiment_analysis_model-0.0.5/tests/
--rw-rw-rw-   0        0        0      163 2024-05-30 07:54:26.000000 sentiment_analysis_model-0.0.5/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      255 2024-05-30 07:54:37.000000 sentiment_analysis_model-0.0.5/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:13:52.818706 sentiment_analysis_model-0.0.6/
+-rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      241 2024-05-30 09:13:52.818706 sentiment_analysis_model-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.6/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-30 09:13:52.800709 sentiment_analysis_model-0.0.6/sentiment_analysis_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:13:52.807726 sentiment_analysis_model-0.0.6/sentiment_analysis_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/config/__init__.py
+-rw-rw-rw-   0        0        0     1165 2024-05-30 08:47:19.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/config/core.py
+-rw-rw-rw-   0        0        0      428 2024-05-30 07:45:43.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/pipeline.py
+-rw-rw-rw-   0        0        0      548 2024-05-30 07:45:21.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:13:52.812705 sentiment_analysis_model-0.0.6/sentiment_analysis_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      282 2024-05-30 08:47:16.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-30 08:33:20.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1692 2024-05-30 07:50:16.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:13:52.817704 sentiment_analysis_model-0.0.6/sentiment_analysis_model.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-30 09:13:52.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-05-30 09:13:52.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:13:52.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-30 09:13:52.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 09:13:52.000000 sentiment_analysis_model-0.0.6/sentiment_analysis_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 09:13:52.819737 sentiment_analysis_model-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-30 09:12:43.000000 sentiment_analysis_model-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:13:52.816706 sentiment_analysis_model-0.0.6/tests/
+-rw-rw-rw-   0        0        0      163 2024-05-30 07:54:26.000000 sentiment_analysis_model-0.0.6/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      255 2024-05-30 07:54:37.000000 sentiment_analysis_model-0.0.6/tests/test_processing.py
```

### Comparing `sentiment_analysis_model-0.0.5/sentiment_analysis_model/config/core.py` & `sentiment_analysis_model-0.0.6/sentiment_analysis_model/config/core.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.5/sentiment_analysis_model/predict.py` & `sentiment_analysis_model-0.0.6/sentiment_analysis_model/predict.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.5/sentiment_analysis_model/processing/features.py` & `sentiment_analysis_model-0.0.6/sentiment_analysis_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.5/sentiment_analysis_model/train_pipeline.py` & `sentiment_analysis_model-0.0.6/sentiment_analysis_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.5/sentiment_analysis_model.egg-info/SOURCES.txt` & `sentiment_analysis_model-0.0.6/sentiment_analysis_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

