# Comparing `tmp/sentiment_analysis_model-0.0.2.tar.gz` & `tmp/sentiment_analysis_model-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_model-0.0.2.tar", last modified: Thu May 30 08:04:49 2024, max compression
+gzip compressed data, was "sentiment_analysis_model-0.0.3.tar", last modified: Thu May 30 08:38:07 2024, max compression
```

## Comparing `sentiment_analysis_model-0.0.2.tar` & `sentiment_analysis_model-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.283592 sentiment_analysis_model-0.0.2/
--rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      241 2024-05-30 08:04:49.282561 sentiment_analysis_model-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.2/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.267563 sentiment_analysis_model-0.0.2/sentiment_analysis_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.275561 sentiment_analysis_model-0.0.2/sentiment_analysis_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/config/__init__.py
--rw-rw-rw-   0        0        0      766 2024-05-30 07:39:39.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/config/core.py
--rw-rw-rw-   0        0        0      428 2024-05-30 07:45:43.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/pipeline.py
--rw-rw-rw-   0        0        0      548 2024-05-30 07:45:21.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.278569 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/__init__.py
--rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/validation.py
--rw-rw-rw-   0        0        0     1692 2024-05-30 07:50:16.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.282561 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-30 08:04:49.284562 sentiment_analysis_model-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-30 08:01:47.000000 sentiment_analysis_model-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.280563 sentiment_analysis_model-0.0.2/tests/
--rw-rw-rw-   0        0        0      163 2024-05-30 07:54:26.000000 sentiment_analysis_model-0.0.2/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      255 2024-05-30 07:54:37.000000 sentiment_analysis_model-0.0.2/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:38:07.167889 sentiment_analysis_model-0.0.3/
+-rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      241 2024-05-30 08:38:07.166889 sentiment_analysis_model-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.3/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-30 08:38:07.147889 sentiment_analysis_model-0.0.3/sentiment_analysis_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:38:07.155889 sentiment_analysis_model-0.0.3/sentiment_analysis_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/config/__init__.py
+-rw-rw-rw-   0        0        0     1165 2024-05-30 08:33:25.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/config/core.py
+-rw-rw-rw-   0        0        0      428 2024-05-30 07:45:43.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/pipeline.py
+-rw-rw-rw-   0        0        0      548 2024-05-30 07:45:21.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:38:07.162890 sentiment_analysis_model-0.0.3/sentiment_analysis_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      428 2024-05-30 08:33:18.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-30 08:33:20.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1692 2024-05-30 07:50:16.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:38:07.166889 sentiment_analysis_model-0.0.3/sentiment_analysis_model.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-30 08:38:07.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-05-30 08:38:07.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:38:07.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-30 08:38:07.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 08:38:07.000000 sentiment_analysis_model-0.0.3/sentiment_analysis_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 08:38:07.168889 sentiment_analysis_model-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-30 08:36:40.000000 sentiment_analysis_model-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:38:07.164889 sentiment_analysis_model-0.0.3/tests/
+-rw-rw-rw-   0        0        0      163 2024-05-30 07:54:26.000000 sentiment_analysis_model-0.0.3/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      255 2024-05-30 07:54:37.000000 sentiment_analysis_model-0.0.3/tests/test_processing.py
```

### Comparing `sentiment_analysis_model-0.0.2/sentiment_analysis_model/predict.py` & `sentiment_analysis_model-0.0.3/sentiment_analysis_model/predict.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/features.py` & `sentiment_analysis_model-0.0.3/sentiment_analysis_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.2/sentiment_analysis_model/train_pipeline.py` & `sentiment_analysis_model-0.0.3/sentiment_analysis_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/SOURCES.txt` & `sentiment_analysis_model-0.0.3/sentiment_analysis_model.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 sentiment_analysis_model.egg-info/SOURCES.txt
 sentiment_analysis_model.egg-info/dependency_links.txt
 sentiment_analysis_model.egg-info/requires.txt
 sentiment_analysis_model.egg-info/top_level.txt
 sentiment_analysis_model/config/__init__.py
 sentiment_analysis_model/config/core.py
 sentiment_analysis_model/processing/__init__.py
+sentiment_analysis_model/processing/data_manager.py
 sentiment_analysis_model/processing/features.py
 sentiment_analysis_model/processing/validation.py
 tests/test_pipeline.py
 tests/test_processing.py
```

