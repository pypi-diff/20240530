# Comparing `tmp/ywp-0.5.0.tar.gz` & `tmp/ywp-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-0.5.0.tar", last modified: Thu May 30 09:30:01 2024, max compression
+gzip compressed data, was "ywp-0.6.0.tar", last modified: Thu May 30 09:51:36 2024, max compression
```

## Comparing `ywp-0.5.0.tar` & `ywp-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 09:30:01.706285 ywp-0.5.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     2316 2024-05-30 09:30:01.690295 ywp-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1712 2024-05-30 09:20:31.000000 ywp-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 09:30:01.658312 ywp-0.5.0/YWP/
--rw-rw-rw-   0        0        0      636 2024-05-30 09:07:12.000000 ywp-0.5.0/YWP/__init__.py
--rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.5.0/YWP/create_file.py
--rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.5.0/YWP/delete_all_files.py
--rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-0.5.0/YWP/hibernate.py
--rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-0.5.0/YWP/log_off.py
--rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.5.0/YWP/open_file.py
--rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.5.0/YWP/open_website.py
--rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-0.5.0/YWP/play_audio.py
--rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-0.5.0/YWP/play_audio_online.py
--rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.5.0/YWP/play_sound.py
--rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.5.0/YWP/record_audio.py
--rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-0.5.0/YWP/restart.py
--rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.5.0/YWP/shutdown.py
--rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.5.0/YWP/stop_recording.py
--rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-0.5.0/YWP/text_to_speech.py
--rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-0.5.0/YWP/token_information.py
--rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.5.0/YWP/transcribe_audio.py
--rw-rw-rw-   0        0        0     5102 2024-05-30 09:10:45.000000 ywp-0.5.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 09:30:01.688296 ywp-0.5.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     2316 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-05-30 09:30:01.000000 ywp-0.5.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 09:30:01.706285 ywp-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-05-30 08:41:25.000000 ywp-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:51:36.088524 ywp-0.6.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2310 2024-05-30 09:51:36.086549 ywp-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1706 2024-05-30 09:32:12.000000 ywp-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 09:51:36.048556 ywp-0.6.0/YWP/
+-rw-rw-rw-   0        0        0       99 2024-05-30 09:41:52.000000 ywp-0.6.0/YWP/AIMP_Run.py
+-rw-rw-rw-   0        0        0      668 2024-05-30 09:42:08.000000 ywp-0.6.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.6.0/YWP/create_file.py
+-rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.6.0/YWP/delete_all_files.py
+-rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-0.6.0/YWP/hibernate.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-0.6.0/YWP/log_off.py
+-rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.6.0/YWP/open_file.py
+-rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.6.0/YWP/open_website.py
+-rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-0.6.0/YWP/play_audio.py
+-rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-0.6.0/YWP/play_audio_online.py
+-rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.6.0/YWP/play_sound.py
+-rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.6.0/YWP/record_audio.py
+-rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-0.6.0/YWP/restart.py
+-rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.6.0/YWP/shutdown.py
+-rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.6.0/YWP/stop_recording.py
+-rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-0.6.0/YWP/text_to_speech.py
+-rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-0.6.0/YWP/token_information.py
+-rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.6.0/YWP/transcribe_audio.py
+-rw-rw-rw-   0        0        0     5102 2024-05-30 09:10:45.000000 ywp-0.6.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:51:36.065546 ywp-0.6.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     2310 2024-05-30 09:51:35.000000 ywp-0.6.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-30 09:51:35.000000 ywp-0.6.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:51:35.000000 ywp-0.6.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 09:51:35.000000 ywp-0.6.0/YWP.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 09:51:35.000000 ywp-0.6.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 09:51:35.000000 ywp-0.6.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 09:51:36.089526 ywp-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2024-05-30 09:50:44.000000 ywp-0.6.0/setup.py
```

### Comparing `ywp-0.5.0/PKG-INFO` & `ywp-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.5.0
+Version: 0.6.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,21 +52,20 @@
         1- binance
         2- etherum
         3- geckoterminal
     data required:
         1- binance (token)
         2- etherum (token)
         3- geckoterminal (pool)
+```
 
 ### LICENSE
 
 Choose a license, for YWP, the MIT license:
-```text
 MIT License
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ywp-0.5.0/README.md` & `ywp-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,20 @@
         1- binance
         2- etherum
         3- geckoterminal
     data required:
         1- binance (token)
         2- etherum (token)
         3- geckoterminal (pool)
+```
 
 ### LICENSE
 
 Choose a license, for YWP, the MIT license:
-```text
 MIT License
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ywp-0.5.0/YWP/__init__.py` & `ywp-0.6.0/YWP/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 from .text_to_speech import text_to_speech
 from .play_sound import play_sound
 from .restart import restart
 from .log_off import log_off
 from .hibernate import hibernate
 from .play_audio_online import play_audio_online
 from .token_information import token_information
+from .AIMP_Run import AIMP_Run
```

### Comparing `ywp-0.5.0/YWP/create_file.py` & `ywp-0.6.0/YWP/create_file.py`

 * *Files identical despite different names*

### Comparing `ywp-0.5.0/YWP/delete_all_files.py` & `ywp-0.6.0/YWP/delete_all_files.py`

 * *Files identical despite different names*

### Comparing `ywp-0.5.0/YWP/record_audio.py` & `ywp-0.6.0/YWP/record_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.5.0/YWP/token_information.py` & `ywp-0.6.0/YWP/token_information.py`

 * *Files identical despite different names*

### Comparing `ywp-0.5.0/YWP/transcribe_audio.py` & `ywp-0.6.0/YWP/transcribe_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.5.0/YWP/ywp.py` & `ywp-0.6.0/YWP/ywp.py`

 * *Files identical despite different names*

### Comparing `ywp-0.5.0/YWP.egg-info/PKG-INFO` & `ywp-0.6.0/YWP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.5.0
+Version: 0.6.0
 Summary: A big Package has a lot of things
 Home-page: https://github.com/YourWantedProducts/YWP_Python
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,21 +52,20 @@
         1- binance
         2- etherum
         3- geckoterminal
     data required:
         1- binance (token)
         2- etherum (token)
         3- geckoterminal (pool)
+```
 
 ### LICENSE
 
 Choose a license, for YWP, the MIT license:
-```text
 MIT License
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ywp-0.5.0/setup.py` & `ywp-0.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YWP",
-    version="0.5.0",
+    version="0.6.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
     ],
+    package_data={
+        "": ["aimp.exe"],  # Include aimp.exe at the root level of the package
+    },
+    entry_points={
+        "console_scripts": [
+            "YWP_install_AIMP = YWP:AIMP_Run", 
+        ],
+    },
     author="Your Wanted Products",
     author_email="pbstzidr@ywp.freewebhostmost.com",
     description="A big Package has a lot of things",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/YourWantedProducts/YWP_Python",
     classifiers=[
```

