# Comparing `tmp/bcqa-1.0.2.tar.gz` & `tmp/bcqa-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcqa-1.0.2.tar", last modified: Thu May 30 18:38:37 2024, max compression
+gzip compressed data, was "bcqa-1.0.3.tar", last modified: Thu May 30 18:43:36 2024, max compression
```

## Comparing `bcqa-1.0.2.tar` & `bcqa-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:38:37.727009 bcqa-1.0.2/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2749 2024-05-30 18:38:37.727009 bcqa-1.0.2/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.0.2/README.md
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:38:37.727009 bcqa-1.0.2/bcqa.egg-info/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2749 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)      167 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/SOURCES.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/dependency_links.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/requires.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/top_level.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 18:38:37.727009 bcqa-1.0.2/setup.cfg
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 18:38:30.000000 bcqa-1.0.2/setup.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:43:36.906773 bcqa-1.0.3/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 18:43:36.906773 bcqa-1.0.3/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.0.3/README.md
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:43:36.903440 bcqa-1.0.3/bcqa.egg-info/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     3192 2024-05-30 18:43:36.000000 bcqa-1.0.3/bcqa.egg-info/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      167 2024-05-30 18:43:36.000000 bcqa-1.0.3/bcqa.egg-info/SOURCES.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:43:36.000000 bcqa-1.0.3/bcqa.egg-info/dependency_links.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 18:43:36.000000 bcqa-1.0.3/bcqa.egg-info/requires.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:43:36.000000 bcqa-1.0.3/bcqa.egg-info/top_level.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 18:43:36.906773 bcqa-1.0.3/setup.cfg
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 18:41:18.000000 bcqa-1.0.3/setup.py
```

### Comparing `bcqa-1.0.2/PKG-INFO` & `bcqa-1.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: bcqa
-Version: 1.0.2
-Summary: A Benchmark for Complex Heterogeneous Question answering
-Home-page: https://github.com/VenkteshV/BCQA
-Download-URL: 
-Author: Venktesh V, Deepali Prabhu
-Author-email: venkyviswa12@gmail.com
-License: Apache License 2.0
-Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tf
-
 # BCQA (Benchmarking Complex QA)
 
 BCQA is a benchmark for a wide range of complex Qa tasks. It also aims to provide a easy to use framework for evaluating retrieval and reasoning approaches for answering complex multi-hop questions.
 
 
 # Setup
 1) Clone the repo <br />
```

### Comparing `bcqa-1.0.2/bcqa.egg-info/PKG-INFO` & `bcqa-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 Metadata-Version: 2.1
 Name: bcqa
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Benchmark for Complex Heterogeneous Question answering
 Home-page: https://github.com/VenkteshV/BCQA
 Download-URL: 
 Author: Venktesh V, Deepali Prabhu
 Author-email: venkyviswa12@gmail.com
 License: Apache License 2.0
 Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: sentence-transformers
+Requires-Dist: pytrec_eval
+Requires-Dist: faiss_cpu
+Requires-Dist: elasticsearch==7.9.1
+Requires-Dist: data
+Requires-Dist: toml
+Requires-Dist: zope.interface
+Requires-Dist: transformers==4.30.0
+Requires-Dist: protobuf
+Requires-Dist: openai
+Requires-Dist: pytrec_eval
 Provides-Extra: tf
+Requires-Dist: tensorflow>=2.2.0; extra == "tf"
+Requires-Dist: tensorflow-text; extra == "tf"
+Requires-Dist: tensorflow-hub; extra == "tf"
 
 # BCQA (Benchmarking Complex QA)
 
 BCQA is a benchmark for a wide range of complex Qa tasks. It also aims to provide a easy to use framework for evaluating retrieval and reasoning approaches for answering complex multi-hop questions.
 
 
 # Setup
```

### Comparing `bcqa-1.0.2/setup.py` & `bcqa-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 optional_packages = {
     "tf" : ['tensorflow>=2.2.0', 'tensorflow-text', 'tensorflow-hub']
 }
 
 setup(
     name="bcqa",
-    version="1.0.2",
+    version="1.0.3",
     author="Venktesh V, Deepali Prabhu",
     author_email="venkyviswa12@gmail.com",
     description="A Benchmark for Complex Heterogeneous Question answering",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     url="https://github.com/VenkteshV/BCQA",
```

