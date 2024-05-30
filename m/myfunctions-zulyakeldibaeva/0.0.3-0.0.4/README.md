# Comparing `tmp/myfunctions_zulyakeldibaeva-0.0.3.tar.gz` & `tmp/myfunctions_zulyakeldibaeva-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/zulyakeldibaeva/python-class/evolvecyber/class5/dist/tmpm2omrwaa/myfunctions_zulyakeldibaeva-0.0.3.tar", last modified: Thu May 30 01:20:29 2024, max compression
+gzip compressed data, was "/mnt/zulyakeldibaeva/python-class/evolvecyber/class5/dist/tmpf4qd1su_/myfunctions_zulyakeldibaeva-0.0.4.tar", last modified: Thu May 30 01:28:28 2024, max compression
```

## Comparing `myfunctions_zulyakeldibaeva-0.0.3.tar` & `myfunctions_zulyakeldibaeva-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      659 2024-05-30 01:20:18.000000 myfunctions_zulyakeldibaeva-0.0.3/setup.py
-drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       28 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/top_level.txt
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      298 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/SOURCES.txt
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        1 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/dependency_links.txt
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2863 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/PKG-INFO
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2395 2024-05-30 01:19:31.000000 myfunctions_zulyakeldibaeva-0.0.3/README.md
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2863 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/PKG-INFO
-drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva/
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      174 2024-05-30 01:15:19.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva/math.py
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 00:49:22.000000 myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva/__init__.py
--rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       38 2024-05-30 01:20:29.000000 myfunctions_zulyakeldibaeva-0.0.3/setup.cfg
+drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:28:28.000000 myfunctions_zulyakeldibaeva-0.0.4/
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      659 2024-05-30 01:28:11.000000 myfunctions_zulyakeldibaeva-0.0.4/setup.py
+drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:28:28.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva.egg-info/
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       28 2024-05-30 01:28:27.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva.egg-info/top_level.txt
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      298 2024-05-30 01:28:27.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva.egg-info/SOURCES.txt
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        1 2024-05-30 01:28:27.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva.egg-info/dependency_links.txt
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2863 2024-05-30 01:28:27.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva.egg-info/PKG-INFO
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2395 2024-05-30 01:19:31.000000 myfunctions_zulyakeldibaeva-0.0.4/README.md
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)     2863 2024-05-30 01:28:28.000000 myfunctions_zulyakeldibaeva-0.0.4/PKG-INFO
+drwxrwxr-x   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 01:28:27.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva/
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)      331 2024-05-30 01:26:48.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva/math.py
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)        0 2024-05-30 00:49:22.000000 myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva/__init__.py
+-rw-rw-r--   0 zulyakeldibaeva  (1643) zulyakeldibaeva  (1644)       38 2024-05-30 01:28:28.000000 myfunctions_zulyakeldibaeva-0.0.4/setup.cfg
```

### Comparing `myfunctions_zulyakeldibaeva-0.0.3/setup.py` & `myfunctions_zulyakeldibaeva-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_zulyakeldibaeva',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/zulyakeldibaeva',
     license='MIT',
     author='Zulfiia Keldibaeva',
     author_email='zulfiiakeldibaeva@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_zulyakeldibaeva-0.0.3/myfunctions_zulyakeldibaeva.egg-info/PKG-INFO` & `myfunctions_zulyakeldibaeva-0.0.4/myfunctions_zulyakeldibaeva.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-zulyakeldibaeva
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/zulyakeldibaeva
 Author: Zulfiia Keldibaeva
 Author-email: zulfiiakeldibaeva@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_zulyakeldibaeva-0.0.3/README.md` & `myfunctions_zulyakeldibaeva-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_zulyakeldibaeva-0.0.3/PKG-INFO` & `myfunctions_zulyakeldibaeva-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_zulyakeldibaeva
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/zulyakeldibaeva
 Author: Zulfiia Keldibaeva
 Author-email: zulfiiakeldibaeva@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

