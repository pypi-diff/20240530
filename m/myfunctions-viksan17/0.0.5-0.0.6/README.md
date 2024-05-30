# Comparing `tmp/myfunctions_viksan17-0.0.5.tar.gz` & `tmp/myfunctions_viksan17-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/viksan17/python-class/class5/dist/tmpt3cnuwx6/myfunctions_viksan17-0.0.5.tar", last modified: Thu May 30 01:32:16 2024, max compression
+gzip compressed data, was "/mnt/viksan17/python-class/class5/dist/tmp6aen1_9a/myfunctions_viksan17-0.0.6.tar", last modified: Thu May 30 01:33:10 2024, max compression
```

## Comparing `myfunctions_viksan17-0.0.5.tar` & `myfunctions_viksan17-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      636 2024-05-30 01:31:57.000000 myfunctions_viksan17-0.0.5/setup.py
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       21 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/top_level.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      256 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/SOURCES.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        1 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/dependency_links.txt
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/PKG-INFO
-drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17/
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      437 2024-05-30 01:31:33.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17/math.py
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 00:48:44.000000 myfunctions_viksan17-0.0.5/myfunctions_viksan17/__init__.py
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     1798 2024-05-30 01:18:46.000000 myfunctions_viksan17-0.0.5/README.md
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/PKG-INFO
--rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       38 2024-05-30 01:32:16.000000 myfunctions_viksan17-0.0.5/setup.cfg
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      640 2024-05-30 01:32:56.000000 myfunctions_viksan17-0.0.6/setup.py
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17.egg-info/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       21 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17.egg-info/top_level.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      299 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17.egg-info/SOURCES.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        3 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17.egg-info/requires.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        1 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17.egg-info/dependency_links.txt
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17.egg-info/PKG-INFO
+drwxrwxr-x   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17/
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)      437 2024-05-30 01:31:33.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17/math.py
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)        0 2024-05-30 00:48:44.000000 myfunctions_viksan17-0.0.6/myfunctions_viksan17/__init__.py
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     1798 2024-05-30 01:18:46.000000 myfunctions_viksan17-0.0.6/README.md
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)     2243 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/PKG-INFO
+-rw-rw-r--   0 viksan17  (1704) viksan17  (1705)       38 2024-05-30 01:33:10.000000 myfunctions_viksan17-0.0.6/setup.cfg
```

### Comparing `myfunctions_viksan17-0.0.5/setup.py` & `myfunctions_viksan17-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_viksan17',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=["os"],
     url='https://github.com/viksan17/',
     license='MIT',
     author='Victor Sanabria',
     author_email='vicsanab92@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `myfunctions_viksan17-0.0.5/myfunctions_viksan17.egg-info/PKG-INFO` & `myfunctions_viksan17-0.0.6/myfunctions_viksan17.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-viksan17
-Version: 0.0.5
+Version: 0.0.6
 Summary: A description of your package
 Home-page: https://github.com/viksan17/
 Author: Victor Sanabria
 Author-email: vicsanab92@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_viksan17-0.0.5/README.md` & `myfunctions_viksan17-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_viksan17-0.0.5/PKG-INFO` & `myfunctions_viksan17-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_viksan17
-Version: 0.0.5
+Version: 0.0.6
 Summary: A description of your package
 Home-page: https://github.com/viksan17/
 Author: Victor Sanabria
 Author-email: vicsanab92@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

