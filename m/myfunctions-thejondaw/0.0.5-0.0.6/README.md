# Comparing `tmp/myfunctions_thejondaw-0.0.5.tar.gz` & `tmp/myfunctions_thejondaw-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/thejondaw/python-class/evolve_cyber/class_05/dist/tmpe3soabl5/myfunctions_thejondaw-0.0.5.tar", last modified: Thu May 30 01:21:16 2024, max compression
+gzip compressed data, was "/mnt/thejondaw/python-class/evolve_cyber/class_05/dist/tmp7z9duysh/myfunctions_thejondaw-0.0.6.tar", last modified: Thu May 30 01:24:53 2024, max compression
```

## Comparing `myfunctions_thejondaw-0.0.5.tar` & `myfunctions_thejondaw-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/
--rwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)      627 2024-05-30 01:21:06.000000 myfunctions_thejondaw-0.0.5/setup.py
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw.egg-info/
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       22 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw.egg-info/top_level.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      262 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw.egg-info/SOURCES.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        1 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw.egg-info/dependency_links.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw.egg-info/PKG-INFO
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw/
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      106 2024-05-30 00:54:35.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw/math.py
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:42.000000 myfunctions_thejondaw-0.0.5/myfunctions_thejondaw/__init__.py
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       49 2024-05-30 01:20:30.000000 myfunctions_thejondaw-0.0.5/README.md
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/PKG-INFO
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       38 2024-05-30 01:21:16.000000 myfunctions_thejondaw-0.0.5/setup.cfg
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:24:53.000000 myfunctions_thejondaw-0.0.6/
+-rwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)      627 2024-05-30 01:24:40.000000 myfunctions_thejondaw-0.0.6/setup.py
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:24:53.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw.egg-info/
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       22 2024-05-30 01:24:52.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw.egg-info/top_level.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      262 2024-05-30 01:24:52.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        1 2024-05-30 01:24:52.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:24:52.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw.egg-info/PKG-INFO
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:24:52.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw/
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      241 2024-05-30 01:24:32.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw/math.py
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:42.000000 myfunctions_thejondaw-0.0.6/myfunctions_thejondaw/__init__.py
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       49 2024-05-30 01:20:30.000000 myfunctions_thejondaw-0.0.6/README.md
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:24:53.000000 myfunctions_thejondaw-0.0.6/PKG-INFO
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       38 2024-05-30 01:24:53.000000 myfunctions_thejondaw-0.0.6/setup.cfg
```

### Comparing `myfunctions_thejondaw-0.0.5/setup.py` & `myfunctions_thejondaw-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_thejondaw',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/thejondaw',
     license='MIT',
     author='Jon Daw',
     author_email='mrjondaw@gmail.com',
     description='A description of your package',
```

