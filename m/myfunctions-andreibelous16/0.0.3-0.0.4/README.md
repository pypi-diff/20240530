# Comparing `tmp/myfunctions_andreibelous16-0.0.3.tar.gz` & `tmp/myfunctions_andreibelous16-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Andreibelous16/python_class/evolvecyber/class5/dist/tmp7cy6d1h9/myfunctions_andreibelous16-0.0.3.tar", last modified: Thu May 30 01:19:18 2024, max compression
+gzip compressed data, was "/mnt/Andreibelous16/python_class/evolvecyber/class5/dist/tmpjwilwdo8/myfunctions_andreibelous16-0.0.4.tar", last modified: Thu May 30 01:32:35 2024, max compression
```

## Comparing `myfunctions_andreibelous16-0.0.3.tar` & `myfunctions_andreibelous16-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      649 2024-05-30 01:18:51.000000 myfunctions_andreibelous16-0.0.3/setup.py
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       27 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/top_level.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      292 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/SOURCES.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        1 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/dependency_links.txt
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2852 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/PKG-INFO
-drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16/
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      175 2024-05-30 01:12:57.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16/math.py
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:50.000000 myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16/__init__.py
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2394 2024-05-30 01:18:43.000000 myfunctions_andreibelous16-0.0.3/README.md
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2852 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/PKG-INFO
--rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       38 2024-05-30 01:19:18.000000 myfunctions_andreibelous16-0.0.3/setup.cfg
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      649 2024-05-30 01:32:24.000000 myfunctions_andreibelous16-0.0.4/setup.py
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16.egg-info/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       27 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16.egg-info/top_level.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      292 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16.egg-info/SOURCES.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        1 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16.egg-info/dependency_links.txt
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2852 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16.egg-info/PKG-INFO
+drwxrwxr-x   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16/
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)      450 2024-05-30 01:31:39.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16/math.py
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)        0 2024-05-30 00:48:50.000000 myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16/__init__.py
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2394 2024-05-30 01:18:43.000000 myfunctions_andreibelous16-0.0.4/README.md
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)     2852 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/PKG-INFO
+-rw-rw-r--   0 Andreibelous16  (1709) Andreibelous16  (1710)       38 2024-05-30 01:32:35.000000 myfunctions_andreibelous16-0.0.4/setup.cfg
```

### Comparing `myfunctions_andreibelous16-0.0.3/setup.py` & `myfunctions_andreibelous16-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_andreibelous16',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/Andreibelous16',
     license='MIT',
     author='Andrei Belous',
     author_email='andrewbelousit@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_andreibelous16-0.0.3/myfunctions_andreibelous16.egg-info/PKG-INFO` & `myfunctions_andreibelous16-0.0.4/myfunctions_andreibelous16.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-andreibelous16
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/Andreibelous16
 Author: Andrei Belous
 Author-email: andrewbelousit@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_andreibelous16-0.0.3/README.md` & `myfunctions_andreibelous16-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_andreibelous16-0.0.3/PKG-INFO` & `myfunctions_andreibelous16-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_andreibelous16
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/Andreibelous16
 Author: Andrei Belous
 Author-email: andrewbelousit@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

