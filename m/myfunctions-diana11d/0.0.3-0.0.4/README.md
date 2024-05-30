# Comparing `tmp/myfunctions_diana11d-0.0.3.tar.gz` & `tmp/myfunctions_diana11d-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Diana11d/python-class/evolvecyber/class5/dist/tmpgn_uqmvk/myfunctions_diana11d-0.0.3.tar", last modified: Thu May 30 01:27:30 2024, max compression
+gzip compressed data, was "/mnt/Diana11d/python-class/evolvecyber/class5/dist/tmpnyig9o7u/myfunctions_diana11d-0.0.4.tar", last modified: Thu May 30 01:32:08 2024, max compression
```

## Comparing `myfunctions_diana11d-0.0.3.tar` & `myfunctions_diana11d-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      641 2024-05-30 01:24:47.000000 myfunctions_diana11d-0.0.3/setup.py
-drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d/
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      312 2024-05-30 01:24:31.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d/math.py
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:48:46.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d/__init__.py
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)     2387 2024-05-30 01:18:48.000000 myfunctions_diana11d-0.0.3/README.md
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)     2837 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/PKG-INFO
-drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d.egg-info/
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       21 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d.egg-info/top_level.txt
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      256 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d.egg-info/SOURCES.txt
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        1 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d.egg-info/dependency_links.txt
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)     2837 2024-05-30 01:27:29.000000 myfunctions_diana11d-0.0.3/myfunctions_diana11d.egg-info/PKG-INFO
--rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       38 2024-05-30 01:27:30.000000 myfunctions_diana11d-0.0.3/setup.cfg
+drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      641 2024-05-30 01:31:45.000000 myfunctions_diana11d-0.0.4/setup.py
+drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d/
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      441 2024-05-30 01:30:57.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d/math.py
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 00:48:46.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d/__init__.py
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)     2387 2024-05-30 01:18:48.000000 myfunctions_diana11d-0.0.4/README.md
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)     2837 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/PKG-INFO
+drwxrwxr-x   0 Diana11d  (1693) Diana11d  (1694)        0 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d.egg-info/
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       21 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d.egg-info/top_level.txt
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)      256 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d.egg-info/SOURCES.txt
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)        1 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d.egg-info/dependency_links.txt
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)     2837 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/myfunctions_diana11d.egg-info/PKG-INFO
+-rw-rw-r--   0 Diana11d  (1693) Diana11d  (1694)       38 2024-05-30 01:32:08.000000 myfunctions_diana11d-0.0.4/setup.cfg
```

### Comparing `myfunctions_diana11d-0.0.3/setup.py` & `myfunctions_diana11d-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_diana11d',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/Diana11d',
     license='MIT',
     author='Diana Dauletkerey',
     author_email='ddauletkerey02@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_diana11d-0.0.3/README.md` & `myfunctions_diana11d-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_diana11d-0.0.3/PKG-INFO` & `myfunctions_diana11d-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_diana11d
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/Diana11d
 Author: Diana Dauletkerey
 Author-email: ddauletkerey02@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_diana11d-0.0.3/myfunctions_diana11d.egg-info/PKG-INFO` & `myfunctions_diana11d-0.0.4/myfunctions_diana11d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-diana11d
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/Diana11d
 Author: Diana Dauletkerey
 Author-email: ddauletkerey02@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

