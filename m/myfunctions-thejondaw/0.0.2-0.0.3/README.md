# Comparing `tmp/myfunctions_thejondaw-0.0.2.tar.gz` & `tmp/myfunctions_thejondaw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/thejondaw/python-class/evolve_cyber/class_05/dist/tmp5j4o_a00/myfunctions_thejondaw-0.0.2.tar", last modified: Thu May 30 01:13:18 2024, max compression
+gzip compressed data, was "/mnt/thejondaw/python-class/evolve_cyber/class_05/dist/tmp38yhfj3s/myfunctions_thejondaw-0.0.3.tar", last modified: Thu May 30 01:14:37 2024, max compression
```

## Comparing `myfunctions_thejondaw-0.0.2.tar` & `myfunctions_thejondaw-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/
--rwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)      627 2024-05-30 01:13:08.000000 myfunctions_thejondaw-0.0.2/setup.py
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw.egg-info/
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       22 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw.egg-info/top_level.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      262 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw.egg-info/SOURCES.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        1 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw.egg-info/dependency_links.txt
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      443 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw.egg-info/PKG-INFO
-drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw/
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      106 2024-05-30 00:54:35.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw/math.py
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:42.000000 myfunctions_thejondaw-0.0.2/myfunctions_thejondaw/__init__.py
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:22.000000 myfunctions_thejondaw-0.0.2/README.md
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      443 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/PKG-INFO
--rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       38 2024-05-30 01:13:18.000000 myfunctions_thejondaw-0.0.2/setup.cfg
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:14:37.000000 myfunctions_thejondaw-0.0.3/
+-rwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)      627 2024-05-30 01:14:26.000000 myfunctions_thejondaw-0.0.3/setup.py
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:14:37.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw.egg-info/
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       22 2024-05-30 01:14:36.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw.egg-info/top_level.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      262 2024-05-30 01:14:37.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        1 2024-05-30 01:14:36.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      443 2024-05-30 01:14:36.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw.egg-info/PKG-INFO
+drwxrwxr-x   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 01:14:37.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw/
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      106 2024-05-30 00:54:35.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw/math.py
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:42.000000 myfunctions_thejondaw-0.0.3/myfunctions_thejondaw/__init__.py
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)        0 2024-05-30 00:48:22.000000 myfunctions_thejondaw-0.0.3/README.md
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)      443 2024-05-30 01:14:37.000000 myfunctions_thejondaw-0.0.3/PKG-INFO
+-rw-rw-r--   0 thejondaw  (1656) thejondaw  (1657)       38 2024-05-30 01:14:37.000000 myfunctions_thejondaw-0.0.3/setup.cfg
```

### Comparing `myfunctions_thejondaw-0.0.2/setup.py` & `myfunctions_thejondaw-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_thejondaw',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/thejondaw',
     license='MIT',
     author='Jon Daw',
     author_email='mrjondaw@gmail.com',
     description='A description of your package',
```

