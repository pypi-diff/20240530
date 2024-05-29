# Comparing `tmp/dre4my_detection-0.1.0.tar.gz` & `tmp/dre4my_detection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dre4my_detection-0.1.0.tar", last modified: Wed May 29 21:01:53 2024, max compression
+gzip compressed data, was "dre4my_detection-0.1.1.tar", last modified: Wed May 29 21:39:08 2024, max compression
```

## Comparing `dre4my_detection-0.1.0.tar` & `dre4my_detection-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:01:53.227915 dre4my_detection-0.1.0/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      154 2024-05-29 21:01:53.221304 dre4my_detection-0.1.0/PKG-INFO
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      141 2024-05-24 15:47:09.000000 dre4my_detection-0.1.0/README.md
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:01:52.981404 dre4my_detection-0.1.0/anomaly_detection_methods/
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:01:53.032615 dre4my_detection-0.1.0/anomaly_detection_methods/ML_BASED/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.0/anomaly_detection_methods/ML_BASED/__init__.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2006 2024-05-29 20:29:31.000000 dre4my_detection-0.1.0/anomaly_detection_methods/ML_BASED/ml_analyzer.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2711 2024-05-29 20:29:33.000000 dre4my_detection-0.1.0/anomaly_detection_methods/ML_BASED/train_model.py
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:01:53.085744 dre4my_detection-0.1.0/anomaly_detection_methods/SIGNATURE_BASED/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.0/anomaly_detection_methods/SIGNATURE_BASED/__init__.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1945 2024-05-24 19:44:07.000000 dre4my_detection-0.1.0/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2122 2024-05-24 18:46:44.000000 dre4my_detection-0.1.0/anomaly_detection_methods/SIGNATURE_BASED/utils.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.0/anomaly_detection_methods/__init__.py
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:01:53.138900 dre4my_detection-0.1.0/anomaly_detection_methods/tests/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2146 2024-05-29 20:29:29.000000 dre4my_detection-0.1.0/anomaly_detection_methods/tests/ML_tests.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:46:11.000000 dre4my_detection-0.1.0/anomaly_detection_methods/tests/__init__.py
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2822 2024-05-28 17:28:59.000000 dre4my_detection-0.1.0/anomaly_detection_methods/tests/signatures_tests.py
-drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:01:53.214279 dre4my_detection-0.1.0/dre4my_detection.egg-info/
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      154 2024-05-29 21:01:51.000000 dre4my_detection-0.1.0/dre4my_detection.egg-info/PKG-INFO
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      672 2024-05-29 21:01:52.000000 dre4my_detection-0.1.0/dre4my_detection.egg-info/SOURCES.txt
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        1 2024-05-29 21:01:51.000000 dre4my_detection-0.1.0/dre4my_detection.egg-info/dependency_links.txt
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       26 2024-05-29 21:01:51.000000 dre4my_detection-0.1.0/dre4my_detection.egg-info/top_level.txt
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       38 2024-05-29 21:01:53.228913 dre4my_detection-0.1.0/setup.cfg
--rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1436 2024-05-29 20:56:22.000000 dre4my_detection-0.1.0/setup.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.936355 dre4my_detection-0.1.1/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      204 2024-05-29 21:31:43.000000 dre4my_detection-0.1.1/MANIFEST.in
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      318 2024-05-29 21:39:08.930117 dre4my_detection-0.1.1/PKG-INFO
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      122 2024-05-29 21:04:21.000000 dre4my_detection-0.1.1/README.md
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.641477 dre4my_detection-0.1.1/anomaly_detection_methods/
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.725926 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/__init__.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)    40863 2024-05-29 17:06:57.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/logistic_regression_model.pkl
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2006 2024-05-29 20:29:31.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/ml_analyzer.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)   185962 2024-05-29 17:06:57.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/tfidf_vectorizer.pkl
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2711 2024-05-29 20:29:33.000000 dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/train_model.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.792405 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/__init__.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1945 2024-05-24 19:44:07.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      726 2024-05-28 16:14:18.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/signatures.json
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2122 2024-05-24 18:46:44.000000 dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/utils.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:42:49.000000 dre4my_detection-0.1.1/anomaly_detection_methods/__init__.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.842247 dre4my_detection-0.1.1/anomaly_detection_methods/tests/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2146 2024-05-29 20:29:29.000000 dre4my_detection-0.1.1/anomaly_detection_methods/tests/ML_tests.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-23 15:46:11.000000 dre4my_detection-0.1.1/anomaly_detection_methods/tests/__init__.py
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     2822 2024-05-28 17:28:59.000000 dre4my_detection-0.1.1/anomaly_detection_methods/tests/signatures_tests.py
+drwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        0 2024-05-29 21:39:08.921589 dre4my_detection-0.1.1/dre4my_detection.egg-info/
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      318 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/PKG-INFO
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)      863 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)        1 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       26 2024-05-29 21:39:07.000000 dre4my_detection-0.1.1/dre4my_detection.egg-info/top_level.txt
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)       38 2024-05-29 21:39:08.936355 dre4my_detection-0.1.1/setup.cfg
+-rwxrwxrwx   0 dreamy    (1000) dreamy    (1000)     1842 2024-05-29 21:38:37.000000 dre4my_detection-0.1.1/setup.py
```

### Comparing `dre4my_detection-0.1.0/anomaly_detection_methods/ML_BASED/ml_analyzer.py` & `dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/ml_analyzer.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.0/anomaly_detection_methods/ML_BASED/train_model.py` & `dre4my_detection-0.1.1/anomaly_detection_methods/ML_BASED/train_model.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.0/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py` & `dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.0/anomaly_detection_methods/SIGNATURE_BASED/utils.py` & `dre4my_detection-0.1.1/anomaly_detection_methods/SIGNATURE_BASED/utils.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.0/anomaly_detection_methods/tests/ML_tests.py` & `dre4my_detection-0.1.1/anomaly_detection_methods/tests/ML_tests.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.0/anomaly_detection_methods/tests/signatures_tests.py` & `dre4my_detection-0.1.1/anomaly_detection_methods/tests/signatures_tests.py`

 * *Files identical despite different names*

### Comparing `dre4my_detection-0.1.0/dre4my_detection.egg-info/SOURCES.txt` & `dre4my_detection-0.1.1/dre4my_detection.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+MANIFEST.in
 README.md
 setup.py
 anomaly_detection_methods/__init__.py
 anomaly_detection_methods/ML_BASED/__init__.py
+anomaly_detection_methods/ML_BASED/logistic_regression_model.pkl
 anomaly_detection_methods/ML_BASED/ml_analyzer.py
+anomaly_detection_methods/ML_BASED/tfidf_vectorizer.pkl
 anomaly_detection_methods/ML_BASED/train_model.py
 anomaly_detection_methods/SIGNATURE_BASED/__init__.py
 anomaly_detection_methods/SIGNATURE_BASED/signature_analyzer.py
+anomaly_detection_methods/SIGNATURE_BASED/signatures.json
 anomaly_detection_methods/SIGNATURE_BASED/utils.py
 anomaly_detection_methods/tests/ML_tests.py
 anomaly_detection_methods/tests/__init__.py
 anomaly_detection_methods/tests/signatures_tests.py
 dre4my_detection.egg-info/PKG-INFO
 dre4my_detection.egg-info/SOURCES.txt
 dre4my_detection.egg-info/dependency_links.txt
```

### Comparing `dre4my_detection-0.1.0/setup.py` & `dre4my_detection-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import find_packages, setup
 
+with open('README.md') as f:
+    long_description = f.read()
+
 setup(
     name='dre4my_detection',
     packages=find_packages(),
-    version='0.1.0',
-    description='''Library for detecting abnormal HTTP-packets using one of the methods:
-    - Signature_Based;
-    - ML_Based.
-    ''',
+    include_package_data=True,
+    package_data={
+        '': ['anomaly_detection_methods/SIGNATURE_BASED/signatures.json', 'anomaly_detection_methods/ML_BASED/logistic_regression_model.pkl', 'anomaly_detection_methods/ML_BASED/tfidf_vectorizer.pkl'],
+        },
+    version='0.1.1',
+    description='Library for detecting abnormal HTTP-packets using one of the methods:\n- Signature_Based;\n- ML_Based.',
     author='Dre4my',
     install_requires=[],
     setup_requires=['certifi==2024.2.2', 'cffi==1.16.0', 'charset-normalizer==3.3.2', 
                     'cryptography==42.0.7', 'docutils==0.21.2', 'idna==3.7', 
                     'importlib_metadata==7.1.0', 'jaraco.classes==3.4.0', 'jaraco.context==5.3.0', 
                     'jaraco.functools==4.0.1', 'jeepney==0.8.0', 'joblib==1.4.2', 
                     'keyring==25.2.1', 'markdown-it-py==3.0.0', 'mdurl==0.1.2', 
@@ -19,8 +23,10 @@
                     'pandas==2.2.2', 'pkginfo==1.10.0', 'pycparser==2.22', 
                     'Pygments==2.18.0', 'python-dateutil==2.9.0.post0', 'pytz==2024.1', 
                     'readme_renderer==43.0', 'requests==2.32.2', 'requests-toolbelt==1.0.0', 
                     'rfc3986==2.0.0', 'rich==13.7.1', 'scikit-learn==1.5.0', 
                     'scipy==1.13.1', 'SecretStorage==3.3.3', 'setuptools==70.0.0', 
                     'six==1.16.0', 'threadpoolctl==3.5.0', 'twine==5.1.0', 
                     'tzdata==2024.1', 'urllib3==2.2.1', 'wheel==0.43.0', 'zipp==3.18.2'],
+    long_description=long_description,
+    long_description_content_type="text/markdown",
 )
```

