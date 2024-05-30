# Comparing `tmp/ywp-0.1.0.tar.gz` & `tmp/ywp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-0.1.0.tar", last modified: Thu May 30 06:41:33 2024, max compression
+gzip compressed data, was "ywp-0.2.0.tar", last modified: Thu May 30 06:44:20 2024, max compression
```

## Comparing `ywp-0.1.0.tar` & `ywp-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 06:41:33.246008 ywp-0.1.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1656 2024-05-30 06:41:33.224472 ywp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2024-05-30 06:10:53.000000 ywp-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 06:41:33.192173 ywp-0.1.0/YWP/
--rw-rw-rw-   0        0        0       74 2024-05-30 06:09:16.000000 ywp-0.1.0/YWP/__init__.py
--rw-rw-rw-   0        0        0     4027 2024-05-30 05:32:31.000000 ywp-0.1.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 06:41:33.222468 ywp-0.1.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     1656 2024-05-30 06:41:32.000000 ywp-0.1.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-05-30 06:41:32.000000 ywp-0.1.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 06:41:32.000000 ywp-0.1.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 06:41:32.000000 ywp-0.1.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 06:41:32.000000 ywp-0.1.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 06:41:33.246975 ywp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-05-30 06:41:10.000000 ywp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:44:20.751643 ywp-0.2.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1658 2024-05-30 06:44:20.731655 ywp-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2024-05-30 06:43:45.000000 ywp-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 06:44:20.685681 ywp-0.2.0/YWP/
+-rw-rw-rw-   0        0        0       74 2024-05-30 06:09:16.000000 ywp-0.2.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0     4027 2024-05-30 05:32:31.000000 ywp-0.2.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:44:20.718670 ywp-0.2.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     1658 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2024-05-30 06:44:20.000000 ywp-0.2.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 06:44:19.000000 ywp-0.2.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:44:20.752642 ywp-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-05-30 06:44:09.000000 ywp-0.2.0/setup.py
```

### Comparing `ywp-0.1.0/PKG-INFO` & `ywp-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.1.0
+Version: 0.2.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,38 +13,38 @@
 License-File: LICENSE
 Requires-Dist: SpeechRecognition
 Requires-Dist: gtts
 Requires-Dist: pygame
 Requires-Dist: sounddevice
 Requires-Dist: pyaudio
 
-# MyPackage
+# YWP Package
 
 A big Package has a lot of things From Your Wanted Products (YWP)
 
 ## Installation
 
 You can install this package using pip:
 
 pip install YWP
 
 ## Usage
 
 ```python
 from YWP import play_audio
-from ywp import stop_recording
-from ywp import delete_all_files
-from ywp import create_file
-from ywp import open_file
-from ywp import open_website
-from ywp import shutdown
-from ywp import record_audio
-from ywp import transcribe_audio
-from ywp import text_to_speech
-from ywp import play_sound
+from YWP import stop_recording
+from YWP import delete_all_files
+from YWP import create_file
+from YWP import open_file
+from YWP import open_website
+from YWP import shutdown
+from YWP import record_audio
+from YWP import transcribe_audio
+from YWP import text_to_speech
+from YWP import play_sound
 
 
 ### `LICENSE`
 
 Choose a license, for YWP, the MIT license:
 ```text
 MIT License
```

### Comparing `ywp-0.1.0/README.md` & `ywp-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# MyPackage
+# YWP Package
 
 A big Package has a lot of things From Your Wanted Products (YWP)
 
 ## Installation
 
 You can install this package using pip:
 
 pip install YWP
 
 ## Usage
 
 ```python
 from YWP import play_audio
-from ywp import stop_recording
-from ywp import delete_all_files
-from ywp import create_file
-from ywp import open_file
-from ywp import open_website
-from ywp import shutdown
-from ywp import record_audio
-from ywp import transcribe_audio
-from ywp import text_to_speech
-from ywp import play_sound
+from YWP import stop_recording
+from YWP import delete_all_files
+from YWP import create_file
+from YWP import open_file
+from YWP import open_website
+from YWP import shutdown
+from YWP import record_audio
+from YWP import transcribe_audio
+from YWP import text_to_speech
+from YWP import play_sound
 
 
 ### `LICENSE`
 
 Choose a license, for YWP, the MIT license:
 ```text
 MIT License
```

### Comparing `ywp-0.1.0/YWP/ywp.py` & `ywp-0.2.0/YWP/ywp.py`

 * *Files identical despite different names*

### Comparing `ywp-0.1.0/YWP.egg-info/PKG-INFO` & `ywp-0.2.0/YWP.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.1.0
+Version: 0.2.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,38 +13,38 @@
 License-File: LICENSE
 Requires-Dist: SpeechRecognition
 Requires-Dist: gtts
 Requires-Dist: pygame
 Requires-Dist: sounddevice
 Requires-Dist: pyaudio
 
-# MyPackage
+# YWP Package
 
 A big Package has a lot of things From Your Wanted Products (YWP)
 
 ## Installation
 
 You can install this package using pip:
 
 pip install YWP
 
 ## Usage
 
 ```python
 from YWP import play_audio
-from ywp import stop_recording
-from ywp import delete_all_files
-from ywp import create_file
-from ywp import open_file
-from ywp import open_website
-from ywp import shutdown
-from ywp import record_audio
-from ywp import transcribe_audio
-from ywp import text_to_speech
-from ywp import play_sound
+from YWP import stop_recording
+from YWP import delete_all_files
+from YWP import create_file
+from YWP import open_file
+from YWP import open_website
+from YWP import shutdown
+from YWP import record_audio
+from YWP import transcribe_audio
+from YWP import text_to_speech
+from YWP import play_sound
 
 
 ### `LICENSE`
 
 Choose a license, for YWP, the MIT license:
 ```text
 MIT License
```

### Comparing `ywp-0.1.0/setup.py` & `ywp-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YWP",
-    version="0.1.0",
+    version="0.2.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

