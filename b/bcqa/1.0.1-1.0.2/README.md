# Comparing `tmp/bcqa-1.0.1.tar.gz` & `tmp/bcqa-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcqa-1.0.1.tar", last modified: Thu May 30 18:33:06 2024, max compression
+gzip compressed data, was "bcqa-1.0.2.tar", last modified: Thu May 30 18:38:37 2024, max compression
```

## Comparing `bcqa-1.0.1.tar` & `bcqa-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:33:06.110607 bcqa-1.0.1/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2749 2024-05-30 18:33:06.110607 bcqa-1.0.1/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.0.1/README.md
-drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:33:06.110607 bcqa-1.0.1/bcqa.egg-info/
--rw-r--r--   0 venky    (100600114) venky    (100600114)     2749 2024-05-30 18:33:06.000000 bcqa-1.0.1/bcqa.egg-info/PKG-INFO
--rw-r--r--   0 venky    (100600114) venky    (100600114)      167 2024-05-30 18:33:06.000000 bcqa-1.0.1/bcqa.egg-info/SOURCES.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:33:06.000000 bcqa-1.0.1/bcqa.egg-info/dependency_links.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 18:33:06.000000 bcqa-1.0.1/bcqa.egg-info/requires.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:33:06.000000 bcqa-1.0.1/bcqa.egg-info/top_level.txt
--rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 18:33:06.110607 bcqa-1.0.1/setup.cfg
--rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 18:32:41.000000 bcqa-1.0.1/setup.py
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:38:37.727009 bcqa-1.0.2/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2749 2024-05-30 18:38:37.727009 bcqa-1.0.2/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2001 2024-05-30 16:47:11.000000 bcqa-1.0.2/README.md
+drwxr-xr-x   0 venky    (100600114) venky    (100600114)        0 2024-05-30 18:38:37.727009 bcqa-1.0.2/bcqa.egg-info/
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     2749 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/PKG-INFO
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      167 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/SOURCES.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/dependency_links.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)      194 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/requires.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)        1 2024-05-30 18:38:37.000000 bcqa-1.0.2/bcqa.egg-info/top_level.txt
+-rw-r--r--   0 venky    (100600114) venky    (100600114)       38 2024-05-30 18:38:37.727009 bcqa-1.0.2/setup.cfg
+-rw-r--r--   0 venky    (100600114) venky    (100600114)     1430 2024-05-30 18:38:30.000000 bcqa-1.0.2/setup.py
```

### Comparing `bcqa-1.0.1/PKG-INFO` & `bcqa-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcqa
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Benchmark for Complex Heterogeneous Question answering
 Home-page: https://github.com/VenkteshV/BCQA
 Download-URL: 
 Author: Venktesh V, Deepali Prabhu
 Author-email: venkyviswa12@gmail.com
 License: Apache License 2.0
 Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
```

### Comparing `bcqa-1.0.1/README.md` & `bcqa-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bcqa-1.0.1/bcqa.egg-info/PKG-INFO` & `bcqa-1.0.2/bcqa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcqa
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Benchmark for Complex Heterogeneous Question answering
 Home-page: https://github.com/VenkteshV/BCQA
 Download-URL: 
 Author: Venktesh V, Deepali Prabhu
 Author-email: venkyviswa12@gmail.com
 License: Apache License 2.0
 Keywords: Information Retrieval Transformer Networks BERT PyTorch Complex Question Answering IR NLP deep learning
```

### Comparing `bcqa-1.0.1/setup.py` & `bcqa-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 optional_packages = {
     "tf" : ['tensorflow>=2.2.0', 'tensorflow-text', 'tensorflow-hub']
 }
 
 setup(
     name="bcqa",
-    version="1.0.1",
+    version="1.0.2",
     author="Venktesh V, Deepali Prabhu",
     author_email="venkyviswa12@gmail.com",
     description="A Benchmark for Complex Heterogeneous Question answering",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     url="https://github.com/VenkteshV/BCQA",
```

