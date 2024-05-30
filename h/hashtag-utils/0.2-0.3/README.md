# Comparing `tmp/hashtag_utils-0.2.tar.gz` & `tmp/hashtag_utils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashtag_utils-0.2.tar", last modified: Thu May 30 20:35:19 2024, max compression
+gzip compressed data, was "hashtag_utils-0.3.tar", last modified: Thu May 30 20:49:48 2024, max compression
```

## Comparing `hashtag_utils-0.2.tar` & `hashtag_utils-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:35:19.648915 hashtag_utils-0.2/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.2/LICENSE
--rw-r--r--   0 aditya.patange   (502) staff       (20)      599 2024-05-30 20:35:19.648492 hashtag_utils-0.2/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      123 2024-05-30 18:56:08.000000 hashtag_utils-0.2/README.md
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:35:19.645776 hashtag_utils-0.2/hashtag_utils/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      369 2024-05-30 20:06:44.000000 hashtag_utils-0.2/hashtag_utils/__init__.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1142 2024-05-30 20:32:27.000000 hashtag_utils-0.2/hashtag_utils/hashtag_generator.py
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:35:19.647837 hashtag_utils-0.2/hashtag_utils.egg-info/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      599 2024-05-30 20:35:19.000000 hashtag_utils-0.2/hashtag_utils.egg-info/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      235 2024-05-30 20:35:19.000000 hashtag_utils-0.2/hashtag_utils.egg-info/SOURCES.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 20:35:19.000000 hashtag_utils-0.2/hashtag_utils.egg-info/dependency_links.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 20:35:19.000000 hashtag_utils-0.2/hashtag_utils.egg-info/top_level.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 20:35:19.648975 hashtag_utils-0.2/setup.cfg
--rw-r--r--   0 aditya.patange   (502) staff       (20)      628 2024-05-30 20:35:17.000000 hashtag_utils-0.2/setup.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:49:48.084974 hashtag_utils-0.3/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.3/LICENSE
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1482 2024-05-30 20:49:48.084350 hashtag_utils-0.3/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1005 2024-05-30 20:47:35.000000 hashtag_utils-0.3/README.md
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:49:48.080901 hashtag_utils-0.3/hashtag_utils/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      369 2024-05-30 20:06:44.000000 hashtag_utils-0.3/hashtag_utils/__init__.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1142 2024-05-30 20:32:27.000000 hashtag_utils-0.3/hashtag_utils/hashtag_generator.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:49:48.083731 hashtag_utils-0.3/hashtag_utils.egg-info/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1482 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      235 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 20:49:48.000000 hashtag_utils-0.3/hashtag_utils.egg-info/top_level.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 20:49:48.085042 hashtag_utils-0.3/setup.cfg
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      628 2024-05-30 20:49:44.000000 hashtag_utils-0.3/setup.py
```

### Comparing `hashtag_utils-0.2/LICENSE` & `hashtag_utils-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.2/hashtag_utils/hashtag_generator.py` & `hashtag_utils-0.3/hashtag_utils/hashtag_generator.py`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.2/setup.py` & `hashtag_utils-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hashtag_utils",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
     author="Aditya Patange",
     author_email="contact.adityapatange@gmail.com",
     description="Simple LLM-powered hashtag utilities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/AdiPat/hashtag_utils",
```

