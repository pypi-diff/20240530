# Comparing `tmp/myfunctions_aizhan010-0.0.6.tar.gz` & `tmp/myfunctions_aizhan010-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/aizhan010/python/evolvecyber/class5/dist/tmppnr1i2st/myfunctions_aizhan010-0.0.6.tar", last modified: Thu May 30 01:33:12 2024, max compression
+gzip compressed data, was "/mnt/aizhan010/python/evolvecyber/class5/dist/tmpw0qglurw/myfunctions_aizhan010-0.0.7.tar", last modified: Thu May 30 01:35:51 2024, max compression
```

## Comparing `myfunctions_aizhan010-0.0.6.tar` & `myfunctions_aizhan010-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      647 2024-05-30 01:32:51.000000 myfunctions_aizhan010-0.0.6/setup.py
-drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/myfunctions_aizhan010.egg-info/
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/myfunctions_aizhan010.egg-info/top_level.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      242 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/myfunctions_aizhan010.egg-info/SOURCES.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        3 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/myfunctions_aizhan010.egg-info/requires.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/myfunctions_aizhan010.egg-info/dependency_links.txt
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/myfunctions_aizhan010.egg-info/PKG-INFO
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2395 2024-05-30 01:18:35.000000 myfunctions_aizhan010-0.0.6/README.md
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/PKG-INFO
--rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)       38 2024-05-30 01:33:12.000000 myfunctions_aizhan010-0.0.6/setup.cfg
+drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      645 2024-05-30 01:35:31.000000 myfunctions_aizhan010-0.0.7/setup.py
+drwxrwxr-x   0 aizhan010  (1710) aizhan010  (1711)        0 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/myfunctions_aizhan010.egg-info/
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/myfunctions_aizhan010.egg-info/top_level.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)      198 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/myfunctions_aizhan010.egg-info/SOURCES.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)        1 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/myfunctions_aizhan010.egg-info/dependency_links.txt
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/myfunctions_aizhan010.egg-info/PKG-INFO
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2395 2024-05-30 01:18:35.000000 myfunctions_aizhan010-0.0.7/README.md
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)     2847 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/PKG-INFO
+-rw-rw-r--   0 aizhan010  (1710) aizhan010  (1711)       38 2024-05-30 01:35:51.000000 myfunctions_aizhan010-0.0.7/setup.cfg
```

### Comparing `myfunctions_aizhan010-0.0.6/setup.py` & `myfunctions_aizhan010-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_aizhan010',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
-    install_requires=["os"],
+    install_requires=[""],
     url='https://github.com/aizhan010/',
     license='MIT',
     author='Aizhan Maratova',
     author_email='aizhanmaratova6@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `myfunctions_aizhan010-0.0.6/myfunctions_aizhan010.egg-info/PKG-INFO` & `myfunctions_aizhan010-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: myfunctions-aizhan010
-Version: 0.0.6
+Name: myfunctions_aizhan010
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/aizhan010/
 Author: Aizhan Maratova
 Author-email: aizhanmaratova6@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_aizhan010-0.0.6/README.md` & `myfunctions_aizhan010-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_aizhan010-0.0.6/PKG-INFO` & `myfunctions_aizhan010-0.0.7/myfunctions_aizhan010.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: myfunctions_aizhan010
-Version: 0.0.6
+Name: myfunctions-aizhan010
+Version: 0.0.7
 Summary: A description of your package
 Home-page: https://github.com/aizhan010/
 Author: Aizhan Maratova
 Author-email: aizhanmaratova6@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

