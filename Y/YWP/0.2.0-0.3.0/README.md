# Comparing `tmp/ywp-0.2.0.tar.gz` & `tmp/ywp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-0.2.0.tar", last modified: Thu May 30 06:44:20 2024, max compression
+gzip compressed data, was "ywp-0.3.0.tar", last modified: Thu May 30 06:55:26 2024, max compression
```

## Comparing `ywp-0.2.0.tar` & `ywp-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 06:44:20.751643 ywp-0.2.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1658 2024-05-30 06:44:20.731655 ywp-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2024-05-30 06:43:45.000000 ywp-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 06:44:20.685681 ywp-0.2.0/YWP/
--rw-rw-rw-   0        0        0       74 2024-05-30 06:09:16.000000 ywp-0.2.0/YWP/__init__.py
--rw-rw-rw-   0        0        0     4027 2024-05-30 05:32:31.000000 ywp-0.2.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:44:20.718670 ywp-0.2.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     1658 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-05-30 06:44:20.000000 ywp-0.2.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 06:44:20.752642 ywp-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-05-30 06:44:09.000000 ywp-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:55:26.620079 ywp-0.3.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1658 2024-05-30 06:55:26.618095 ywp-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2024-05-30 06:43:45.000000 ywp-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:55:26.601115 ywp-0.3.0/YWP/
+-rw-rw-rw-   0        0        0      330 2024-05-30 06:53:11.000000 ywp-0.3.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0     4027 2024-05-30 05:32:31.000000 ywp-0.3.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:55:26.615085 ywp-0.3.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     1658 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:55:26.621078 ywp-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-05-30 06:55:18.000000 ywp-0.3.0/setup.py
```

### Comparing `ywp-0.2.0/PKG-INFO` & `ywp-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.2.0
+Version: 0.3.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ywp-0.2.0/README.md` & `ywp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ywp-0.2.0/YWP/ywp.py` & `ywp-0.3.0/YWP/ywp.py`

 * *Files identical despite different names*

### Comparing `ywp-0.2.0/YWP.egg-info/PKG-INFO` & `ywp-0.3.0/YWP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.2.0
+Version: 0.3.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ywp-0.2.0/setup.py` & `ywp-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YWP",
-    version="0.2.0",
+    version="0.3.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

