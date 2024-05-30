# Comparing `tmp/crint-0.1.0.tar.gz` & `tmp/crint-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crint-0.1.0.tar", last modified: Sun May 26 15:20:20 2024, max compression
+gzip compressed data, was "crint-0.1.1.tar", last modified: Thu May 30 18:45:48 2024, max compression
```

## Comparing `crint-0.1.0.tar` & `crint-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rajkrishnan   (501) staff       (20)        0 2024-05-26 15:20:20.919247 crint-0.1.0/
--rw-r--r--   0 rajkrishnan   (501) staff       (20)      562 2024-05-26 15:20:20.919036 crint-0.1.0/PKG-INFO
--rw-r--r--   0 rajkrishnan   (501) staff       (20)      138 2024-05-26 15:10:10.000000 crint-0.1.0/README.md
-drwxr-xr-x   0 rajkrishnan   (501) staff       (20)        0 2024-05-26 15:20:20.917843 crint-0.1.0/crint/
--rw-r--r--   0 rajkrishnan   (501) staff       (20)      430 2024-05-26 15:13:12.000000 crint-0.1.0/crint/__init__.py
--rw-r--r--   0 rajkrishnan   (501) staff       (20)      362 2024-05-26 14:44:20.000000 crint-0.1.0/crint/constants.py
-drwxr-xr-x   0 rajkrishnan   (501) staff       (20)        0 2024-05-26 15:20:20.918827 crint-0.1.0/crint.egg-info/
--rw-r--r--   0 rajkrishnan   (501) staff       (20)      562 2024-05-26 15:20:20.000000 crint-0.1.0/crint.egg-info/PKG-INFO
--rw-r--r--   0 rajkrishnan   (501) staff       (20)      171 2024-05-26 15:20:20.000000 crint-0.1.0/crint.egg-info/SOURCES.txt
--rw-r--r--   0 rajkrishnan   (501) staff       (20)        1 2024-05-26 15:20:20.000000 crint-0.1.0/crint.egg-info/dependency_links.txt
--rw-r--r--   0 rajkrishnan   (501) staff       (20)        6 2024-05-26 15:20:20.000000 crint-0.1.0/crint.egg-info/top_level.txt
--rw-r--r--   0 rajkrishnan   (501) staff       (20)       38 2024-05-26 15:20:20.919295 crint-0.1.0/setup.cfg
--rw-r--r--   0 rajkrishnan   (501) staff       (20)      653 2024-05-26 15:11:42.000000 crint-0.1.0/setup.py
+drwxr-xr-x   0 rajkrishnan   (501) staff       (20)        0 2024-05-30 18:45:48.326823 crint-0.1.1/
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)      562 2024-05-30 18:45:48.326645 crint-0.1.1/PKG-INFO
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)      138 2024-05-26 15:10:10.000000 crint-0.1.1/README.md
+drwxr-xr-x   0 rajkrishnan   (501) staff       (20)        0 2024-05-30 18:45:48.325694 crint-0.1.1/crint/
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)      555 2024-05-30 18:36:41.000000 crint-0.1.1/crint/__init__.py
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)      362 2024-05-26 14:44:20.000000 crint-0.1.1/crint/constants.py
+drwxr-xr-x   0 rajkrishnan   (501) staff       (20)        0 2024-05-30 18:45:48.326481 crint-0.1.1/crint.egg-info/
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)      562 2024-05-30 18:45:48.000000 crint-0.1.1/crint.egg-info/PKG-INFO
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)      171 2024-05-30 18:45:48.000000 crint-0.1.1/crint.egg-info/SOURCES.txt
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)        1 2024-05-30 18:45:48.000000 crint-0.1.1/crint.egg-info/dependency_links.txt
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)        6 2024-05-30 18:45:48.000000 crint-0.1.1/crint.egg-info/top_level.txt
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)       38 2024-05-30 18:45:48.326865 crint-0.1.1/setup.cfg
+-rw-r--r--   0 rajkrishnan   (501) staff       (20)      653 2024-05-30 18:43:10.000000 crint-0.1.1/setup.py
```

### Comparing `crint-0.1.0/setup.py` & `crint-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='crint',
-    version='0.1.0',
+    version='0.1.1',
     description='A simple module for colored terminal output',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Raj Krishnan',
     author_email='rajkrishnan.r@outlook.com',
     url='https://github.com/raj-krishnan-r/crint',  # Replace with your GitHub repo URL
     packages=find_packages(),
```

