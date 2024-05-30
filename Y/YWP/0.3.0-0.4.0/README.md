# Comparing `tmp/ywp-0.3.0.tar.gz` & `tmp/ywp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-0.3.0.tar", last modified: Thu May 30 06:55:26 2024, max compression
+gzip compressed data, was "ywp-0.4.0.tar", last modified: Thu May 30 07:15:30 2024, max compression
```

## Comparing `ywp-0.3.0.tar` & `ywp-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 06:55:26.620079 ywp-0.3.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1658 2024-05-30 06:55:26.618095 ywp-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2024-05-30 06:43:45.000000 ywp-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 06:55:26.601115 ywp-0.3.0/YWP/
--rw-rw-rw-   0        0        0      330 2024-05-30 06:53:11.000000 ywp-0.3.0/YWP/__init__.py
--rw-rw-rw-   0        0        0     4027 2024-05-30 05:32:31.000000 ywp-0.3.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:55:26.615085 ywp-0.3.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     1658 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 06:55:26.000000 ywp-0.3.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 06:55:26.621078 ywp-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-05-30 06:55:18.000000 ywp-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:15:30.370483 ywp-0.4.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1658 2024-05-30 07:15:30.367483 ywp-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2024-05-30 06:43:45.000000 ywp-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 07:15:30.347508 ywp-0.4.0/YWP/
+-rw-rw-rw-   0        0        0      440 2024-05-30 07:13:59.000000 ywp-0.4.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.4.0/YWP/create_file.py
+-rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.4.0/YWP/delete_all_files.py
+-rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.4.0/YWP/open_file.py
+-rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.4.0/YWP/open_website.py
+-rw-rw-rw-   0        0        0      315 2024-05-30 07:06:38.000000 ywp-0.4.0/YWP/play_audio.py
+-rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.4.0/YWP/play_sound.py
+-rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.4.0/YWP/record_audio.py
+-rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.4.0/YWP/shutdown.py
+-rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.4.0/YWP/stop_recording.py
+-rw-rw-rw-   0        0        0      147 2024-05-30 07:11:56.000000 ywp-0.4.0/YWP/text_to_speech.py
+-rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.4.0/YWP/transcribe_audio.py
+-rw-rw-rw-   0        0        0     4027 2024-05-30 07:12:44.000000 ywp-0.4.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:15:30.365487 ywp-0.4.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     1658 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:15:30.371489 ywp-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-05-30 07:05:52.000000 ywp-0.4.0/setup.py
```

### Comparing `ywp-0.3.0/PKG-INFO` & `ywp-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.3.0
+Version: 0.4.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ywp-0.3.0/README.md` & `ywp-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ywp-0.3.0/YWP/ywp.py` & `ywp-0.4.0/YWP/ywp.py`

 * *Files identical despite different names*

### Comparing `ywp-0.3.0/YWP.egg-info/PKG-INFO` & `ywp-0.4.0/YWP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.3.0
+Version: 0.4.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ywp-0.3.0/setup.py` & `ywp-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YWP",
-    version="0.3.0",
+    version="0.4.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

