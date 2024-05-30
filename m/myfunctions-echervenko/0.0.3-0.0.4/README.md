# Comparing `tmp/myfunctions_echervenko-0.0.3.tar.gz` & `tmp/myfunctions_echervenko-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/echervenko/python-class/evolvecyber/Class5/dist/tmp9t2w_127/myfunctions_echervenko-0.0.3.tar", last modified: Thu May 30 01:19:09 2024, max compression
+gzip compressed data, was "/mnt/echervenko/python-class/evolvecyber/Class5/dist/tmpj6b1oyjs/myfunctions_echervenko-0.0.4.tar", last modified: Thu May 30 01:31:44 2024, max compression
```

## Comparing `myfunctions_echervenko-0.0.3.tar` & `myfunctions_echervenko-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko/
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      170 2024-05-30 01:12:35.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko/math.py
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:50.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko/__init__.py
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      643 2024-05-30 01:18:42.000000 myfunctions_echervenko-0.0.3/setup.py
-drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko.egg-info/
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       23 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko.egg-info/top_level.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      268 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko.egg-info/SOURCES.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        1 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko.egg-info/dependency_links.txt
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/myfunctions_echervenko.egg-info/PKG-INFO
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2395 2024-05-30 01:18:36.000000 myfunctions_echervenko-0.0.3/README.md
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/PKG-INFO
--rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       38 2024-05-30 01:19:09.000000 myfunctions_echervenko-0.0.3/setup.cfg
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko/
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      363 2024-05-30 01:30:57.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko/math.py
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 00:48:50.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko/__init__.py
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      643 2024-05-30 01:27:13.000000 myfunctions_echervenko-0.0.4/setup.py
+drwxrwxr-x   0 echervenko  (1636) echervenko  (1637)        0 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       23 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/top_level.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)      268 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/SOURCES.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)        1 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/dependency_links.txt
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/PKG-INFO
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2395 2024-05-30 01:18:36.000000 myfunctions_echervenko-0.0.4/README.md
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)     2847 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/PKG-INFO
+-rw-rw-r--   0 echervenko  (1636) echervenko  (1637)       38 2024-05-30 01:31:44.000000 myfunctions_echervenko-0.0.4/setup.cfg
```

### Comparing `myfunctions_echervenko-0.0.3/setup.py` & `myfunctions_echervenko-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_echervenko',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/echervenko',
     license='MIT',
     author='Elena Chervenko',
     author_email='chervenkoelena@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_echervenko-0.0.3/myfunctions_echervenko.egg-info/PKG-INFO` & `myfunctions_echervenko-0.0.4/myfunctions_echervenko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-echervenko
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/echervenko
 Author: Elena Chervenko
 Author-email: chervenkoelena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_echervenko-0.0.3/README.md` & `myfunctions_echervenko-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_echervenko-0.0.3/PKG-INFO` & `myfunctions_echervenko-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_echervenko
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/echervenko
 Author: Elena Chervenko
 Author-email: chervenkoelena@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

