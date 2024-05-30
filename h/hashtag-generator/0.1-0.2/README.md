# Comparing `tmp/hashtag_generator-0.1.tar.gz` & `tmp/hashtag_generator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashtag_generator-0.1.tar", last modified: Thu May 30 19:14:41 2024, max compression
+gzip compressed data, was "hashtag_generator-0.2.tar", last modified: Thu May 30 19:56:02 2024, max compression
```

## Comparing `hashtag_generator-0.1.tar` & `hashtag_generator-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 19:14:41.232665 hashtag_generator-0.1/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_generator-0.1/LICENSE
--rw-r--r--   0 aditya.patange   (502) staff       (20)      621 2024-05-30 19:14:41.232284 hashtag_generator-0.1/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      123 2024-05-30 18:56:08.000000 hashtag_generator-0.1/README.md
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 19:14:41.228586 hashtag_generator-0.1/hashtag-generator/
--rw-r--r--   0 aditya.patange   (502) staff       (20)        0 2024-05-30 19:02:19.000000 hashtag_generator-0.1/hashtag-generator/__init__.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)       35 2024-05-30 19:03:11.000000 hashtag_generator-0.1/hashtag-generator/main.py
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 19:14:41.231836 hashtag_generator-0.1/hashtag_generator.egg-info/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      621 2024-05-30 19:14:41.000000 hashtag_generator-0.1/hashtag_generator.egg-info/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      246 2024-05-30 19:14:41.000000 hashtag_generator-0.1/hashtag_generator.egg-info/SOURCES.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 19:14:41.000000 hashtag_generator-0.1/hashtag_generator.egg-info/dependency_links.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       18 2024-05-30 19:14:41.000000 hashtag_generator-0.1/hashtag_generator.egg-info/top_level.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 19:14:41.232715 hashtag_generator-0.1/setup.cfg
--rw-r--r--   0 aditya.patange   (502) staff       (20)      650 2024-05-30 19:06:18.000000 hashtag_generator-0.1/setup.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 19:56:02.277001 hashtag_generator-0.2/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_generator-0.2/LICENSE
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      621 2024-05-30 19:56:02.276605 hashtag_generator-0.2/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      123 2024-05-30 18:56:08.000000 hashtag_generator-0.2/README.md
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 19:56:02.273923 hashtag_generator-0.2/hashtag-generator/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      125 2024-05-30 19:53:11.000000 hashtag_generator-0.2/hashtag-generator/__init__.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1141 2024-05-30 19:48:16.000000 hashtag_generator-0.2/hashtag-generator/main.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 19:56:02.276138 hashtag_generator-0.2/hashtag_generator.egg-info/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      621 2024-05-30 19:56:02.000000 hashtag_generator-0.2/hashtag_generator.egg-info/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      246 2024-05-30 19:56:02.000000 hashtag_generator-0.2/hashtag_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 19:56:02.000000 hashtag_generator-0.2/hashtag_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       18 2024-05-30 19:56:02.000000 hashtag_generator-0.2/hashtag_generator.egg-info/top_level.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 19:56:02.277056 hashtag_generator-0.2/setup.cfg
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      650 2024-05-30 19:55:57.000000 hashtag_generator-0.2/setup.py
```

### Comparing `hashtag_generator-0.1/LICENSE` & `hashtag_generator-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hashtag_generator-0.1/setup.py` & `hashtag_generator-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hashtag-generator",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     author="Aditya Patange",
     author_email="contact.adityapatange@gmail.com",
     description="An LLM-powered hashtag generator written in Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/AdiPat/hashtag-generator",
```

