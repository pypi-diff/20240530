# Comparing `tmp/sentiment_analysis_model-0.0.7.tar.gz` & `tmp/sentiment_analysis_model-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_model-0.0.7.tar", last modified: Thu May 30 10:22:52 2024, max compression
+gzip compressed data, was "sentiment_analysis_model-0.0.8.tar", last modified: Thu May 30 10:39:07 2024, max compression
```

## Comparing `sentiment_analysis_model-0.0.7.tar` & `sentiment_analysis_model-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:22:52.398143 sentiment_analysis_model-0.0.7/
--rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      241 2024-05-30 10:22:52.397143 sentiment_analysis_model-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.7/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-30 10:22:52.380143 sentiment_analysis_model-0.0.7/sentiment_analysis_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:22:52.388146 sentiment_analysis_model-0.0.7/sentiment_analysis_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/config/__init__.py
--rw-rw-rw-   0        0        0     1165 2024-05-30 08:47:19.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/config/core.py
--rw-rw-rw-   0        0        0      428 2024-05-30 07:45:43.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/pipeline.py
--rw-rw-rw-   0        0        0      548 2024-05-30 07:45:21.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:22:52.393145 sentiment_analysis_model-0.0.7/sentiment_analysis_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/processing/__init__.py
--rw-rw-rw-   0        0        0      282 2024-05-30 08:47:16.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/processing/data_manager.py
--rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-30 08:33:20.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/processing/validation.py
--rw-rw-rw-   0        0        0     1692 2024-05-30 07:50:16.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:22:52.397143 sentiment_analysis_model-0.0.7/sentiment_analysis_model.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-30 10:22:52.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      777 2024-05-30 10:22:52.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:22:52.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-30 10:22:52.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-30 10:22:52.000000 sentiment_analysis_model-0.0.7/sentiment_analysis_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-30 10:22:52.399143 sentiment_analysis_model-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-30 10:14:55.000000 sentiment_analysis_model-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:22:52.395144 sentiment_analysis_model-0.0.7/tests/
--rw-rw-rw-   0        0        0      163 2024-05-30 07:54:26.000000 sentiment_analysis_model-0.0.7/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      255 2024-05-30 07:54:37.000000 sentiment_analysis_model-0.0.7/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:39:07.938046 sentiment_analysis_model-0.0.8/
+-rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      241 2024-05-30 10:39:07.937044 sentiment_analysis_model-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.8/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-30 10:39:07.921047 sentiment_analysis_model-0.0.8/sentiment_analysis_model/
+-rw-rw-rw-   0        0        0      276 2024-05-30 10:38:37.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:39:07.928068 sentiment_analysis_model-0.0.8/sentiment_analysis_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/config/__init__.py
+-rw-rw-rw-   0        0        0     1165 2024-05-30 08:47:19.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/config/core.py
+-rw-rw-rw-   0        0        0      428 2024-05-30 07:45:43.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/pipeline.py
+-rw-rw-rw-   0        0        0      548 2024-05-30 07:45:21.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:39:07.932071 sentiment_analysis_model-0.0.8/sentiment_analysis_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      282 2024-05-30 08:47:16.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-30 08:33:20.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1692 2024-05-30 07:50:16.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:39:07.937044 sentiment_analysis_model-0.0.8/sentiment_analysis_model.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-30 10:39:07.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      777 2024-05-30 10:39:07.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 10:39:07.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-30 10:39:07.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 10:39:07.000000 sentiment_analysis_model-0.0.8/sentiment_analysis_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 10:39:07.939043 sentiment_analysis_model-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-30 10:32:19.000000 sentiment_analysis_model-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 10:39:07.935043 sentiment_analysis_model-0.0.8/tests/
+-rw-rw-rw-   0        0        0      163 2024-05-30 07:54:26.000000 sentiment_analysis_model-0.0.8/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      255 2024-05-30 07:54:37.000000 sentiment_analysis_model-0.0.8/tests/test_processing.py
```

### Comparing `sentiment_analysis_model-0.0.7/sentiment_analysis_model/config/core.py` & `sentiment_analysis_model-0.0.8/sentiment_analysis_model/config/core.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.7/sentiment_analysis_model/predict.py` & `sentiment_analysis_model-0.0.8/sentiment_analysis_model/predict.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.7/sentiment_analysis_model/processing/features.py` & `sentiment_analysis_model-0.0.8/sentiment_analysis_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.7/sentiment_analysis_model/train_pipeline.py` & `sentiment_analysis_model-0.0.8/sentiment_analysis_model/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.7/sentiment_analysis_model.egg-info/SOURCES.txt` & `sentiment_analysis_model-0.0.8/sentiment_analysis_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

