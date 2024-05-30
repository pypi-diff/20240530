# Comparing `tmp/myfunctions_thejondaw-0.0.8.tar.gz` & `tmp/myfunctions_thejondaw-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/thejondaw/python-class/evolve_cyber/class_05/dist/tmpuimft0mg/myfunctions_thejondaw-0.0.8.tar", last modified: Thu May 30 01:32:11 2024, max compression
+gzip compressed data, was "/mnt/thejondaw/python-class/evolve_cyber/class_05/dist/tmp26zk8c6e/myfunctions_thejondaw-0.0.9.tar", last modified: Thu May 30 01:32:56 2024, max compression
```

## Comparing `myfunctions_thejondaw-0.0.8.tar` & `myfunctions_thejondaw-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/
--rwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)      627 2024-05-30 01:31:55.000000 myfunctions_thejondaw-0.0.8/setup.py
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw.egg-info/
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       22 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw.egg-info/top_level.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      262 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw.egg-info/SOURCES.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        1 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw.egg-info/dependency_links.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw.egg-info/PKG-INFO
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw/
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      353 2024-05-30 01:30:56.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw/math.py
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:42.000000 myfunctions_thejondaw-0.0.8/myfunctions_thejondaw/__init__.py
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       49 2024-05-30 01:20:30.000000 myfunctions_thejondaw-0.0.8/README.md
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/PKG-INFO
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       38 2024-05-30 01:32:11.000000 myfunctions_thejondaw-0.0.8/setup.cfg
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/
+-rwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)      631 2024-05-30 01:32:43.000000 myfunctions_thejondaw-0.0.9/setup.py
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw.egg-info/
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       22 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw.egg-info/top_level.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      306 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        3 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw.egg-info/requires.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        1 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw.egg-info/PKG-INFO
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw/
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      353 2024-05-30 01:30:56.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw/math.py
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:42.000000 myfunctions_thejondaw-0.0.9/myfunctions_thejondaw/__init__.py
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       49 2024-05-30 01:20:30.000000 myfunctions_thejondaw-0.0.9/README.md
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      485 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/PKG-INFO
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       38 2024-05-30 01:32:56.000000 myfunctions_thejondaw-0.0.9/setup.cfg
```

### Comparing `myfunctions_thejondaw-0.0.8/setup.py` & `myfunctions_thejondaw-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_thejondaw',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=["os"],
     url='https://github.com/thejondaw',
     license='MIT',
     author='Jon Daw',
     author_email='mrjondaw@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

