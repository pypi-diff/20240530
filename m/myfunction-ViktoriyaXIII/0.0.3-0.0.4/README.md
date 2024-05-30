# Comparing `tmp/myfunction_ViktoriyaXIII-0.0.3.tar.gz` & `tmp/myfunction_ViktoriyaXIII-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/ViktoriyaXIII/Python/evolve_cyber/class5/dist/tmpwze9l3v8/myfunction_ViktoriyaXIII-0.0.3.tar", last modified: Thu May 30 01:20:15 2024, max compression
+gzip compressed data, was "/mnt/ViktoriyaXIII/Python/evolve_cyber/class5/dist/tmpijub5869/myfunction_ViktoriyaXIII-0.0.4.tar", last modified: Thu May 30 01:25:03 2024, max compression
```

## Comparing `myfunction_ViktoriyaXIII-0.0.3.tar` & `myfunction_ViktoriyaXIII-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII/
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      180 2024-05-30 01:13:10.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII/math.py
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 00:48:58.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII/__init__.py
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      645 2024-05-30 01:19:46.000000 myfunction_ViktoriyaXIII-0.0.3/setup.py
-drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       25 2024-05-30 01:20:14.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/top_level.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      280 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/SOURCES.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        1 2024-05-30 01:20:14.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/dependency_links.txt
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:20:14.000000 myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/PKG-INFO
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     1797 2024-05-30 01:18:49.000000 myfunction_ViktoriyaXIII-0.0.3/README.md
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/PKG-INFO
--rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       38 2024-05-30 01:20:15.000000 myfunction_ViktoriyaXIII-0.0.3/setup.cfg
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII/
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      340 2024-05-30 01:24:40.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII/math.py
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 00:48:58.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII/__init__.py
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      645 2024-05-30 01:24:52.000000 myfunction_ViktoriyaXIII-0.0.4/setup.py
+drwxrwxr-x   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        0 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII.egg-info/
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       25 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII.egg-info/top_level.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)      280 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII.egg-info/SOURCES.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)        1 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII.egg-info/dependency_links.txt
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII.egg-info/PKG-INFO
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     1797 2024-05-30 01:18:49.000000 myfunction_ViktoriyaXIII-0.0.4/README.md
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)     2251 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/PKG-INFO
+-rw-rw-r--   0 ViktoriyaXIII  (1676) ViktoriyaXIII  (1677)       38 2024-05-30 01:25:03.000000 myfunction_ViktoriyaXIII-0.0.4/setup.cfg
```

### Comparing `myfunction_ViktoriyaXIII-0.0.3/setup.py` & `myfunction_ViktoriyaXIII-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunction_ViktoriyaXIII',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/ViktoriyaXIII',
     license='MIT',
     author='Viktoriia',
     author_email='viktoriya.bielova@gmail.com',
     description='A description of your package',
```

### Comparing `myfunction_ViktoriyaXIII-0.0.3/myfunction_ViktoriyaXIII.egg-info/PKG-INFO` & `myfunction_ViktoriyaXIII-0.0.4/myfunction_ViktoriyaXIII.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunction-ViktoriyaXIII
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/ViktoriyaXIII
 Author: Viktoriia
 Author-email: viktoriya.bielova@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunction_ViktoriyaXIII-0.0.3/README.md` & `myfunction_ViktoriyaXIII-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfunction_ViktoriyaXIII-0.0.3/PKG-INFO` & `myfunction_ViktoriyaXIII-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunction_ViktoriyaXIII
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/ViktoriyaXIII
 Author: Viktoriia
 Author-email: viktoriya.bielova@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

