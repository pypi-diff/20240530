# Comparing `tmp/myfunction_ViktoriyaXIII-0.0.2.tar.gz` & `tmp/myfunction_ViktoriyaXIII-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/ViktoriyaXIII/Python/evolve_cyber/class5/dist/tmpkjk7o8_c/myfunction_ViktoriyaXIII-0.0.2.tar", last modified: Thu May 30 01:14:22 2024, max compression
+gzip compressed data, was "/mnt/ViktoriyaXIII/Python/evolve_cyber/class5/dist/tmpwze9l3v8/myfunction_ViktoriyaXIII-0.0.3.tar", last modified: Thu May 30 01:20:15 2024, max compression
```

## Comparing `myfunction_ViktoriyaXIII-0.0.2.tar` & `myfunction_ViktoriyaXIII-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII/
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      180 2024-05-30 01:13:10.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII/math.py
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 00:48:58.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII/__init__.py
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      645 2024-05-30 01:13:15.000000 myfunction_ViktoriyaXIII-0.0.2/setup.py
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII.egg-info/
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       25 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII.egg-info/top_level.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      280 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII.egg-info/SOURCES.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        1 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII.egg-info/dependency_links.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      461 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/myfunction_ViktoriyaXIII.egg-info/PKG-INFO
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 00:48:35.000000 myfunction_ViktoriyaXIII-0.0.2/README.md
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      461 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/PKG-INFO
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       38 2024-05-30 01:14:22.000000 myfunction_ViktoriyaXIII-0.0.2/setup.cfg
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII/
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      180 2024-05-30 01:13:10.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII/math.py
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 00:48:58.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII/__init__.py
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      645 2024-05-30 01:19:46.000000 myfunction_ViktoriyaXIII-0.0.3/setup.py
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       25 2024-05-30 01:20:14.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/top_level.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      280 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/SOURCES.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        1 2024-05-30 01:20:14.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/dependency_links.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:20:14.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/PKG-INFO
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     1797 2024-05-30 01:18:49.000000 myfunction_ViktoriyaXIII-0.0.3/README.md
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/PKG-INFO
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       38 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/setup.cfg
```

### Comparing `myfunction_ViktoriyaXIII-0.0.2/setup.py` & `myfunction_ViktoriyaXIII-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunction_ViktoriyaXIII',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/ViktoriyaXIII',
     license='MIT',
     author='Viktoriia',
     author_email='viktoriya.bielova@gmail.com',
     description='A description of your package',
```

