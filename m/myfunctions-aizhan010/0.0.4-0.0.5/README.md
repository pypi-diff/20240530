# Comparing `tmp/myfunctions_aizhan010-0.0.4.tar.gz` & `tmp/myfunctions_aizhan010-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/aizhan010/python/evolvecyber/class5/dist/tmppdsr37ia/myfunctions_aizhan010-0.0.4.tar", last modified: Thu May 30 01:27:22 2024, max compression
+gzip compressed data, was "/mnt/aizhan010/python/evolvecyber/class5/dist/tmppbfte1by/myfunctions_aizhan010-0.0.5.tar", last modified: Thu May 30 01:32:22 2024, max compression
```

## Comparing `myfunctions_aizhan010-0.0.4.tar` & `myfunctions_aizhan010-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      643 2024-05-30 01:25:37.000000 myfunctions_aizhan010-0.0.4/setup.py
-drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/myfunctions_aizhan010.egg-info/
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/myfunctions_aizhan010.egg-info/top_level.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      198 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/myfunctions_aizhan010.egg-info/SOURCES.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/myfunctions_aizhan010.egg-info/dependency_links.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/myfunctions_aizhan010.egg-info/PKG-INFO
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2395 2024-05-30 01:18:35.000000 myfunctions_aizhan010-0.0.4/README.md
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/PKG-INFO
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)       38 2024-05-30 01:27:22.000000 myfunctions_aizhan010-0.0.4/setup.cfg
+drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      643 2024-05-30 01:31:59.000000 myfunctions_aizhan010-0.0.5/setup.py
+drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/myfunctions_aizhan010.egg-info/
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/myfunctions_aizhan010.egg-info/top_level.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      198 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/myfunctions_aizhan010.egg-info/SOURCES.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/myfunctions_aizhan010.egg-info/dependency_links.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/myfunctions_aizhan010.egg-info/PKG-INFO
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2395 2024-05-30 01:18:35.000000 myfunctions_aizhan010-0.0.5/README.md
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/PKG-INFO
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)       38 2024-05-30 01:32:22.000000 myfunctions_aizhan010-0.0.5/setup.cfg
```

### Comparing `myfunctions_aizhan010-0.0.4/setup.py` & `myfunctions_aizhan010-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_aizhan010',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/aizhan010/',
     license='MIT',
     author='Aizhan Maratova',
     author_email='aizhanmaratova6@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_aizhan010-0.0.4/myfunctions_aizhan010.egg-info/PKG-INFO` & `myfunctions_aizhan010-0.0.5/myfunctions_aizhan010.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-aizhan010
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/aizhan010/
 Author: Aizhan Maratova
 Author-email: aizhanmaratova6@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_aizhan010-0.0.4/README.md` & `myfunctions_aizhan010-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_aizhan010-0.0.4/PKG-INFO` & `myfunctions_aizhan010-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_aizhan010
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/aizhan010/
 Author: Aizhan Maratova
 Author-email: aizhanmaratova6@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

