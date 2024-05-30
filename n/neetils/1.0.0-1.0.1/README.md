# Comparing `tmp/neetils-1.0.0.tar.gz` & `tmp/neetils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/neetils-1.0.0.tar", last modified: Thu May 30 08:59:19 2024, max compression
+gzip compressed data, was "neetils-1.0.1.tar", last modified: Thu May 30 09:10:37 2024, max compression
```

## Comparing `neetils-1.0.0.tar` & `neetils-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 nee       (1004) nee       (1004)        0 2024-05-30 08:59:19.000000 neetils-1.0.0/
--rw-r--r--   0 nee       (1004) nee       (1004)      434 2024-05-30 08:59:19.000000 neetils-1.0.0/PKG-INFO
-drwxrwxr-x   0 nee       (1004) nee       (1004)        0 2024-05-30 08:59:19.000000 neetils-1.0.0/neetils/
--rw-r--r--   0 nee       (1004) nee       (1004)       85 2024-05-28 11:55:43.000000 neetils-1.0.0/neetils/__init__.py
--rw-r--r--   0 nee       (1004) nee       (1004)     1151 2024-05-28 11:55:15.000000 neetils-1.0.0/neetils/io.py
-drwxrwxr-x   0 nee       (1004) nee       (1004)        0 2024-05-30 08:59:19.000000 neetils-1.0.0/neetils.egg-info/
--rw-r--r--   0 nee       (1004) nee       (1004)      434 2024-05-30 08:59:19.000000 neetils-1.0.0/neetils.egg-info/PKG-INFO
--rw-r--r--   0 nee       (1004) nee       (1004)      196 2024-05-30 08:59:19.000000 neetils-1.0.0/neetils.egg-info/SOURCES.txt
--rw-r--r--   0 nee       (1004) nee       (1004)        1 2024-05-30 08:59:19.000000 neetils-1.0.0/neetils.egg-info/dependency_links.txt
--rw-r--r--   0 nee       (1004) nee       (1004)       12 2024-05-30 08:59:19.000000 neetils-1.0.0/neetils.egg-info/requires.txt
--rw-r--r--   0 nee       (1004) nee       (1004)        8 2024-05-30 08:59:19.000000 neetils-1.0.0/neetils.egg-info/top_level.txt
--rw-rw-r--   0 nee       (1004) nee       (1004)       38 2024-05-30 08:59:19.000000 neetils-1.0.0/setup.cfg
--rw-r--r--   0 nee       (1004) nee       (1004)      586 2024-04-23 03:29:10.000000 neetils-1.0.0/setup.py
+drwxrwxr-x   0 nee       (1004) nee       (1004)        0 2024-05-30 09:10:37.834844 neetils-1.0.1/
+-rw-r--r--   0 nee       (1004) nee       (1004)      434 2024-05-30 09:10:37.834844 neetils-1.0.1/PKG-INFO
+-rw-r--r--   0 nee       (1004) nee       (1004)      225 2024-04-23 03:29:28.000000 neetils-1.0.1/README.md
+drwxrwxr-x   0 nee       (1004) nee       (1004)        0 2024-05-30 09:10:37.834844 neetils-1.0.1/neetils/
+-rw-r--r--   0 nee       (1004) nee       (1004)       85 2024-05-28 11:55:43.000000 neetils-1.0.1/neetils/__init__.py
+-rw-r--r--   0 nee       (1004) nee       (1004)     1151 2024-05-28 11:55:15.000000 neetils-1.0.1/neetils/io.py
+drwxrwxr-x   0 nee       (1004) nee       (1004)        0 2024-05-30 09:10:37.834844 neetils-1.0.1/neetils.egg-info/
+-rw-r--r--   0 nee       (1004) nee       (1004)      434 2024-05-30 09:10:37.000000 neetils-1.0.1/neetils.egg-info/PKG-INFO
+-rw-r--r--   0 nee       (1004) nee       (1004)      206 2024-05-30 09:10:37.000000 neetils-1.0.1/neetils.egg-info/SOURCES.txt
+-rw-r--r--   0 nee       (1004) nee       (1004)        1 2024-05-30 09:10:37.000000 neetils-1.0.1/neetils.egg-info/dependency_links.txt
+-rw-r--r--   0 nee       (1004) nee       (1004)       12 2024-05-30 09:10:37.000000 neetils-1.0.1/neetils.egg-info/requires.txt
+-rw-r--r--   0 nee       (1004) nee       (1004)        8 2024-05-30 09:10:37.000000 neetils-1.0.1/neetils.egg-info/top_level.txt
+-rw-rw-r--   0 nee       (1004) nee       (1004)       38 2024-05-30 09:10:37.834844 neetils-1.0.1/setup.cfg
+-rw-r--r--   0 nee       (1004) nee       (1004)      660 2024-05-30 09:09:47.000000 neetils-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neetils-1.0.0/neetils/io.py` & `neetils-1.0.1/neetils/io.py`

 * *Files identical despite different names*

### Comparing `neetils-1.0.0/setup.py` & `neetils-1.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 from setuptools import find_packages, setup
 
-with open("readme.md", "r", encoding="utf-8") as f:
+with open(os.path.join(os.path.dirname(__file__), "README.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
 requirements_path = os.path.join(os.path.dirname(__file__), 'requirements.txt')
 setup(name="neetils",
-      version="v1.0.0",
+      version="v1.0.1",
       author="tanknee",
       author_email="nee@tanknee.cn",
       description="A package for tools",
       long_description=long_description,
       long_description_content_type="text/markdown",
-      packages=find_packages(include=["neetils", "neetils.*"]),
+      packages=find_packages(include=["neetils", "neetils.*", "README.md", "requirements.txt"]),
       install_requires=open(requirements_path).readlines())
```

