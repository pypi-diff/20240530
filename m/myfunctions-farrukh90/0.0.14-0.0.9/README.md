# Comparing `tmp/myfunctions_farrukh90-0.0.14.tar.gz` & `tmp/myfunctions_farrukh90-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class5/dist/tmpu5ft0oau/myfunctions_farrukh90-0.0.14.tar", last modified: Thu May 30 01:32:40 2024, max compression
+gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class5/dist/tmpcbl0psmv/myfunctions_farrukh90-0.0.9.tar", last modified: Thu May 30 00:59:41 2024, max compression
```

## Comparing `myfunctions_farrukh90-0.0.14.tar` & `myfunctions_farrukh90-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      648 2024-05-30 01:32:31.000000 myfunctions_farrukh90-0.0.14/setup.py
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90.egg-info/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       22 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90.egg-info/top_level.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      306 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90.egg-info/SOURCES.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        3 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90.egg-info/requires.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90.egg-info/dependency_links.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     2852 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90.egg-info/PKG-INFO
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      438 2024-05-30 01:30:49.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90/math.py
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 00:48:36.000000 myfunctions_farrukh90-0.0.14/myfunctions_farrukh90/__init__.py
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     2400 2024-05-30 01:18:29.000000 myfunctions_farrukh90-0.0.14/README.md
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     2852 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-30 01:32:40.000000 myfunctions_farrukh90-0.0.14/setup.cfg
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      643 2024-05-30 00:59:30.000000 myfunctions_farrukh90-0.0.9/setup.py
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90.egg-info/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       22 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90.egg-info/top_level.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      262 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90.egg-info/SOURCES.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90.egg-info/dependency_links.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      458 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90.egg-info/PKG-INFO
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      107 2024-05-30 00:54:47.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90/math.py
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 00:48:36.000000 myfunctions_farrukh90-0.0.9/myfunctions_farrukh90/__init__.py
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 00:48:16.000000 myfunctions_farrukh90-0.0.9/README.md
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      458 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/PKG-INFO
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-30 00:59:41.000000 myfunctions_farrukh90-0.0.9/setup.cfg
```

### Comparing `myfunctions_farrukh90-0.0.14/setup.py` & `myfunctions_farrukh90-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_farrukh90',
-    version='0.0.14',
+    version='0.0.9',
     packages=find_packages(),
-    install_requires=["os"],
+    install_requires=[],
     url='https://github.com/farrukh90/',
     license='MIT',
     author='Farrukh Sadykov',
     author_email='farrukhsadykov@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

