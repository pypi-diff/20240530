# Comparing `tmp/dre4my_detection-0.1.1.tar.gz` & `tmp/dre4my_detection-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dre4my_detection-0.1.1.tar", last modified: Wed May 29 21:39:08 2024, max compression
+gzip compressed data, was "dre4my_detection-0.1.2.tar", last modified: Wed May 29 22:00:23 2024, max compression
```

## Comparing `dre4my_detection-0.1.1.tar` & `dre4my_detection-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.936355 dre4my_detection-0.1.1/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      204 2024-05-29 21:31:43.000000 dre4my_detection-0.1.1/MANIFEST.in
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      318 2024-05-29 21:39:08.930117 dre4my_detection-0.1.1/PKG-INFO
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      122 2024-05-29 21:04:21.000000 dre4my_detection-0.1.1/README.md
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.641477 dre4my_detection-0.1.1/anomaly_detection_methods/
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.725926 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/__init__.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)    40863 2024-05-29 17:06:57.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/logistic_regression_model.pkl
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2006 2024-05-29 20:29:31.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/ml_analyzer.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)   185962 2024-05-29 17:06:57.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/tfidf_vectorizer.pkl
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2711 2024-05-29 20:29:33.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/train_model.py
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.792405 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/__init__.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1945 2024-05-24 19:44:07.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      726 2024-05-28 16:14:18.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/signatures.json
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2122 2024-05-24 18:46:44.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/utils.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.1/anomaly_detection_methods/__init__.py
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.842247 dre4my_detection-0.1.1/anomaly_detection_methods/tests/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2146 2024-05-29 20:29:29.000000 dre4my_detection-0.1.1/anomaly_detection_methods/tests/ML_tests.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:46:11.000000 dre4my_detection-0.1.1/anomaly_detection_methods/tests/__init__.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2822 2024-05-28 17:28:59.000000 dre4my_detection-0.1.1/anomaly_detection_methods/tests/signatures_tests.py
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.921589 dre4my_detection-0.1.1/dre4my_detection.egg-info/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      318 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/PKG-INFO
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      863 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/SOURCES.txt
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        1 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/dependency_links.txt
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       26 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/top_level.txt
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       38 2024-05-29 21:39:08.936355 dre4my_detection-0.1.1/setup.cfg
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1842 2024-05-29 21:38:37.000000 dre4my_detection-0.1.1/setup.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 22:00:23.962023 dre4my_detection-0.1.2/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      204 2024-05-29 22:00:03.000000 dre4my_detection-0.1.2/MANIFEST.in
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1633 2024-05-29 22:00:23.956025 dre4my_detection-0.1.2/PKG-INFO
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      122 2024-05-29 21:04:21.000000 dre4my_detection-0.1.2/README.md
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 22:00:23.652657 dre4my_detection-0.1.2/anomaly_detection_methods/
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 22:00:23.743445 dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/__init__.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)    40863 2024-05-29 17:06:57.000000 dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/logistic_regression_model.pkl
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2006 2024-05-29 20:29:31.000000 dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/ml_analyzer.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)   185962 2024-05-29 17:06:57.000000 dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/tfidf_vectorizer.pkl
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2711 2024-05-29 20:29:33.000000 dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/train_model.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 22:00:23.810898 dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/__init__.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1945 2024-05-24 19:44:07.000000 dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      726 2024-05-28 16:14:18.000000 dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/signatures.json
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2122 2024-05-24 18:46:44.000000 dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/utils.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.2/anomaly_detection_methods/__init__.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 22:00:23.862749 dre4my_detection-0.1.2/anomaly_detection_methods/tests/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2146 2024-05-29 20:29:29.000000 dre4my_detection-0.1.2/anomaly_detection_methods/tests/ML_tests.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:46:11.000000 dre4my_detection-0.1.2/anomaly_detection_methods/tests/__init__.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2822 2024-05-28 17:28:59.000000 dre4my_detection-0.1.2/anomaly_detection_methods/tests/signatures_tests.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 22:00:23.948419 dre4my_detection-0.1.2/dre4my_detection.egg-info/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1633 2024-05-29 22:00:22.000000 dre4my_detection-0.1.2/dre4my_detection.egg-info/PKG-INFO
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      902 2024-05-29 22:00:22.000000 dre4my_detection-0.1.2/dre4my_detection.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        1 2024-05-29 22:00:22.000000 dre4my_detection-0.1.2/dre4my_detection.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      702 2024-05-29 22:00:22.000000 dre4my_detection-0.1.2/dre4my_detection.egg-info/requires.txt
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       26 2024-05-29 22:00:22.000000 dre4my_detection-0.1.2/dre4my_detection.egg-info/top_level.txt
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       38 2024-05-29 22:00:23.963022 dre4my_detection-0.1.2/setup.cfg
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2966 2024-05-29 21:59:41.000000 dre4my_detection-0.1.2/setup.py
```

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/logistic_regression_model.pkl` & `dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/logistic_regression_model.pkl`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/ml_analyzer.py` & `dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/ml_analyzer.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/tfidf_vectorizer.pkl` & `dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/tfidf_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/train_model.py` & `dre4my_detection-0.1.2/anomaly_detection_methods/ML_BASED/train_model.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py` & `dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/signatures.json` & `dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/signatures.json`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/utils.py` & `dre4my_detection-0.1.2/anomaly_detection_methods/SIGNATURE_BASED/utils.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/tests/ML_tests.py` & `dre4my_detection-0.1.2/anomaly_detection_methods/tests/ML_tests.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/anomaly_detection_methods/tests/signatures_tests.py` & `dre4my_detection-0.1.2/anomaly_detection_methods/tests/signatures_tests.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.1/dre4my_detection.egg-info/SOURCES.txt` & `dre4my_detection-0.1.2/dre4my_detection.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 anomaly_detection_methods/SIGNATURE_BASED/utils.py
 anomaly_detection_methods/tests/ML_tests.py
 anomaly_detection_methods/tests/__init__.py
 anomaly_detection_methods/tests/signatures_tests.py
 dre4my_detection.egg-info/PKG-INFO
 dre4my_detection.egg-info/SOURCES.txt
 dre4my_detection.egg-info/dependency_links.txt
+dre4my_detection.egg-info/requires.txt
 dre4my_detection.egg-info/top_level.txt
```

