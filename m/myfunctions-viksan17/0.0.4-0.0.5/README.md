# Comparing `tmp/myfunctions_viksan17-0.0.4.tar.gz` & `tmp/myfunctions_viksan17-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/viksan17/python-class/class5/dist/tmp6lbjmjr9/myfunctions_viksan17-0.0.4.tar", last modified: Thu May 30 01:26:40 2024, max compression
+gzip compressed data, was "/mnt/viksan17/python-class/class5/dist/tmpt3cnuwx6/myfunctions_viksan17-0.0.5.tar", last modified: Thu May 30 01:32:16 2024, max compression
```

## Comparing `myfunctions_viksan17-0.0.4.tar` & `myfunctions_viksan17-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:26:40.000000 myfunctions_viksan17-0.0.4/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      636 2024-05-30 01:24:42.000000 myfunctions_viksan17-0.0.4/setup.py
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:26:40.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17.egg-info/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       21 2024-05-30 01:26:39.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17.egg-info/top_level.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      256 2024-05-30 01:26:39.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17.egg-info/SOURCES.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        1 2024-05-30 01:26:39.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17.egg-info/dependency_links.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:26:39.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17.egg-info/PKG-INFO
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:26:40.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      336 2024-05-30 01:24:31.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17/math.py
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 00:48:44.000000 myfunctions_viksan17-0.0.4/myfunctions_viksan17/__init__.py
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     1798 2024-05-30 01:18:46.000000 myfunctions_viksan17-0.0.4/README.md
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:26:40.000000 myfunctions_viksan17-0.0.4/PKG-INFO
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       38 2024-05-30 01:26:40.000000 myfunctions_viksan17-0.0.4/setup.cfg
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      636 2024-05-30 01:31:57.000000 myfunctions_viksan17-0.0.5/setup.py
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       21 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/top_level.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      256 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/SOURCES.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        1 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/dependency_links.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/PKG-INFO
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      437 2024-05-30 01:31:33.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17/math.py
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 00:48:44.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17/__init__.py
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     1798 2024-05-30 01:18:46.000000 myfunctions_viksan17-0.0.5/README.md
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/PKG-INFO
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       38 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/setup.cfg
```

### Comparing `myfunctions_viksan17-0.0.4/setup.py` & `myfunctions_viksan17-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_viksan17',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/viksan17/',
     license='MIT',
     author='Victor Sanabria',
     author_email='vicsanab92@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_viksan17-0.0.4/myfunctions_viksan17.egg-info/PKG-INFO` & `myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-viksan17
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/viksan17/
 Author: Victor Sanabria
 Author-email: vicsanab92@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_viksan17-0.0.4/README.md` & `myfunctions_viksan17-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_viksan17-0.0.4/PKG-INFO` & `myfunctions_viksan17-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_viksan17
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/viksan17/
 Author: Victor Sanabria
 Author-email: vicsanab92@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

