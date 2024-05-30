# Comparing `tmp/myfunctions_farrukh90-0.0.11.tar.gz` & `tmp/myfunctions_farrukh90-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class5/dist/tmpzehys57_/myfunctions_farrukh90-0.0.11.tar", last modified: Thu May 30 01:18:51 2024, max compression
+gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class5/dist/tmpcbl0psmv/myfunctions_farrukh90-0.0.9.tar", last modified: Thu May 30 00:59:41 2024, max compression
```

## Comparing `myfunctions_farrukh90-0.0.11.tar` & `myfunctions_farrukh90-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      644 2024-05-30 01:18:34.000000 myfunctions_farrukh90-0.0.11/setup.py
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90.egg-info/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       22 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90.egg-info/top_level.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      262 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90.egg-info/SOURCES.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90.egg-info/dependency_links.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     2852 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90.egg-info/PKG-INFO
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      175 2024-05-30 01:11:59.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90/math.py
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-30 00:48:36.000000 myfunctions_farrukh90-0.0.11/myfunctions_farrukh90/__init__.py
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     2400 2024-05-30 01:18:29.000000 myfunctions_farrukh90-0.0.11/README.md
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     2852 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-30 01:18:51.000000 myfunctions_farrukh90-0.0.11/setup.cfg
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

### Comparing `myfunctions_farrukh90-0.0.11/setup.py` & `myfunctions_farrukh90-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_farrukh90',
-    version='0.0.11',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/farrukh90/',
     license='MIT',
     author='Farrukh Sadykov',
     author_email='farrukhsadykov@gmail.com',
     description='A description of your package',
```

