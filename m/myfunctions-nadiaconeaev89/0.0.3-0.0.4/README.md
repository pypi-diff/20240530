# Comparing `tmp/myfunctions_nadiaconeaev89-0.0.3.tar.gz` & `tmp/myfunctions_nadiaconeaev89-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmplbw7s7e_/myfunctions_nadiaconeaev89-0.0.3.tar", last modified: Thu May 30 01:19:22 2024, max compression
+gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpnjtl9ahe/myfunctions_nadiaconeaev89-0.0.4.tar", last modified: Thu May 30 01:26:39 2024, max compression
```

## Comparing `myfunctions_nadiaconeaev89-0.0.3.tar` & `myfunctions_nadiaconeaev89-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 01:19:03.000000 myfunctions_nadiaconeaev89-0.0.3/setup.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.3/README.md
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      177 2024-05-30 01:13:35.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89/math.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89/__init__.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/PKG-INFO
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/top_level.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:19:22.000000 myfunctions_nadiaconeaev89-0.0.3/setup.cfg
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 01:25:07.000000 myfunctions_nadiaconeaev89-0.0.4/setup.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.4/README.md
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      335 2024-05-30 01:24:52.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89/math.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89/__init__.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/PKG-INFO
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89.egg-info/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89.egg-info/top_level.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:26:39.000000 myfunctions_nadiaconeaev89-0.0.4/setup.cfg
```

### Comparing `myfunctions_nadiaconeaev89-0.0.3/setup.py` & `myfunctions_nadiaconeaev89-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_nadiaconeaev89',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/nadiaconeaev89/',
     license='MIT',
     author='Nadejda Coneaev',
     author_email='nadejda.savin@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_nadiaconeaev89-0.0.3/README.md` & `myfunctions_nadiaconeaev89-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_nadiaconeaev89-0.0.3/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_nadiaconeaev89
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_nadiaconeaev89-0.0.3/myfunctions_nadiaconeaev89.egg-info/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.4/myfunctions_nadiaconeaev89.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-nadiaconeaev89
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

