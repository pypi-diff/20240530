# Comparing `tmp/extrautilities-1.5.tar.gz` & `tmp/extrautilities-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-1.5.tar", last modified: Thu May 30 09:21:45 2024, max compression
+gzip compressed data, was "extrautilities-1.6.tar", last modified: Thu May 30 09:23:55 2024, max compression
```

## Comparing `extrautilities-1.5.tar` & `extrautilities-1.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 09:21:45.349479 extrautilities-1.5/
-drwxrwxrwx   0        0        0        0 2024-05-30 09:21:45.331555 extrautilities-1.5/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.5/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.5/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-05-29 19:13:25.000000 extrautilities-1.5/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.5/ExtraUtils/callbackVoid.py
--rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.5/ExtraUtils/getFileContent.py
--rw-rw-rw-   0        0        0     3181 2024-05-28 18:10:03.000000 extrautilities-1.5/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.5/ExtraUtils/validate_dict.py
--rw-rw-rw-   0        0        0     3349 2024-05-30 09:21:45.348476 extrautilities-1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 09:21:45.346944 extrautilities-1.5/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     3349 2024-05-30 09:21:45.000000 extrautilities-1.5/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-05-30 09:21:45.000000 extrautilities-1.5/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 09:21:45.000000 extrautilities-1.5/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 09:21:45.000000 extrautilities-1.5/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-30 09:21:45.000000 extrautilities-1.5/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 09:21:45.349479 extrautilities-1.5/setup.cfg
--rw-rw-rw-   0        0        0     1132 2024-05-30 09:20:40.000000 extrautilities-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:23:55.305791 extrautilities-1.6/
+drwxrwxrwx   0        0        0        0 2024-05-30 09:23:55.288247 extrautilities-1.6/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.6/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.6/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0      685 2024-05-30 08:14:34.000000 extrautilities-1.6/ExtraUtils/asyncThreads.py
+-rw-rw-rw-   0        0        0     2909 2024-05-29 19:13:25.000000 extrautilities-1.6/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.6/ExtraUtils/callbackVoid.py
+-rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.6/ExtraUtils/getFileContent.py
+-rw-rw-rw-   0        0        0     3181 2024-05-28 18:10:03.000000 extrautilities-1.6/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     2032 2024-05-25 07:02:09.000000 extrautilities-1.6/ExtraUtils/validate_dict.py
+-rw-rw-rw-   0        0        0     3349 2024-05-30 09:23:55.305285 extrautilities-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 09:23:55.304279 extrautilities-1.6/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3349 2024-05-30 09:23:55.000000 extrautilities-1.6/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-05-30 09:23:55.000000 extrautilities-1.6/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:23:55.000000 extrautilities-1.6/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 09:23:55.000000 extrautilities-1.6/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-30 09:23:55.000000 extrautilities-1.6/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 09:23:55.305791 extrautilities-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2024-05-30 09:23:49.000000 extrautilities-1.6/setup.py
```

### Comparing `extrautilities-1.5/ExtraUtils/RateLimit.py` & `extrautilities-1.6/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.5/ExtraUtils/asyncTokens.py` & `extrautilities-1.6/ExtraUtils/asyncTokens.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.5/ExtraUtils/getFileContent.py` & `extrautilities-1.6/ExtraUtils/getFileContent.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.5/ExtraUtils/timeBasedToken.py` & `extrautilities-1.6/ExtraUtils/timeBasedToken.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.5/ExtraUtils/validate_dict.py` & `extrautilities-1.6/ExtraUtils/validate_dict.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.5/PKG-INFO` & `extrautilities-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.5
+Version: 1.6
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.5/README.md` & `extrautilities-1.6/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-1.5/extrautilities.egg-info/PKG-INFO` & `extrautilities-1.6/extrautilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.5
+Version: 1.6
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
 Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid,validate_dict
 Platform: UNKNOWN
```

### Comparing `extrautilities-1.5/setup.py` & `extrautilities-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='1.5',
+    version='1.6',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
```

