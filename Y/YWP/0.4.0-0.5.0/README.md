# Comparing `tmp/ywp-0.4.0.tar.gz` & `tmp/ywp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-0.4.0.tar", last modified: Thu May 30 07:15:30 2024, max compression
+gzip compressed data, was "ywp-0.5.0.tar", last modified: Thu May 30 09:30:01 2024, max compression
```

## Comparing `ywp-0.4.0.tar` & `ywp-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:15:30.370483 ywp-0.4.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1658 2024-05-30 07:15:30.367483 ywp-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2024-05-30 06:43:45.000000 ywp-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 07:15:30.347508 ywp-0.4.0/YWP/
--rw-rw-rw-   0        0        0      440 2024-05-30 07:13:59.000000 ywp-0.4.0/YWP/__init__.py
--rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.4.0/YWP/create_file.py
--rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.4.0/YWP/delete_all_files.py
--rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.4.0/YWP/open_file.py
--rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.4.0/YWP/open_website.py
--rw-rw-rw-   0        0        0      315 2024-05-30 07:06:38.000000 ywp-0.4.0/YWP/play_audio.py
--rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.4.0/YWP/play_sound.py
--rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.4.0/YWP/record_audio.py
--rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.4.0/YWP/shutdown.py
--rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.4.0/YWP/stop_recording.py
--rw-rw-rw-   0        0        0      147 2024-05-30 07:11:56.000000 ywp-0.4.0/YWP/text_to_speech.py
--rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.4.0/YWP/transcribe_audio.py
--rw-rw-rw-   0        0        0     4027 2024-05-30 07:12:44.000000 ywp-0.4.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:15:30.365487 ywp-0.4.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     1658 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 07:15:29.000000 ywp-0.4.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 07:15:30.371489 ywp-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      777 2024-05-30 07:05:52.000000 ywp-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:30:01.706285 ywp-0.5.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2316 2024-05-30 09:30:01.690295 ywp-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1712 2024-05-30 09:20:31.000000 ywp-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 09:30:01.658312 ywp-0.5.0/YWP/
+-rw-rw-rw-   0        0        0      636 2024-05-30 09:07:12.000000 ywp-0.5.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.5.0/YWP/create_file.py
+-rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.5.0/YWP/delete_all_files.py
+-rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-0.5.0/YWP/hibernate.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-0.5.0/YWP/log_off.py
+-rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.5.0/YWP/open_file.py
+-rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.5.0/YWP/open_website.py
+-rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-0.5.0/YWP/play_audio.py
+-rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-0.5.0/YWP/play_audio_online.py
+-rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.5.0/YWP/play_sound.py
+-rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.5.0/YWP/record_audio.py
+-rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-0.5.0/YWP/restart.py
+-rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.5.0/YWP/shutdown.py
+-rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.5.0/YWP/stop_recording.py
+-rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-0.5.0/YWP/text_to_speech.py
+-rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-0.5.0/YWP/token_information.py
+-rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.5.0/YWP/transcribe_audio.py
+-rw-rw-rw-   0        0        0     5102 2024-05-30 09:10:45.000000 ywp-0.5.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 09:30:01.688296 ywp-0.5.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     2316 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-05-30 09:30:01.000000 ywp-0.5.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 09:30:00.000000 ywp-0.5.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 09:30:01.706285 ywp-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      777 2024-05-30 08:41:25.000000 ywp-0.5.0/setup.py
```

### Comparing `ywp-0.4.0/PKG-INFO` & `ywp-0.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,54 @@
-Metadata-Version: 2.1
-Name: YWP
-Version: 0.4.0
-Summary: A big Package has a lot of things
-Home-page: https://github.com/YourWantedProducts/YWP_Python
-Author: Your Wanted Products
-Author-email: pbstzidr@ywp.freewebhostmost.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: SpeechRecognition
-Requires-Dist: gtts
-Requires-Dist: pygame
-Requires-Dist: sounddevice
-Requires-Dist: pyaudio
-
 # YWP Package
 
 A big Package has a lot of things From Your Wanted Products (YWP)
 
 ## Installation
 
 You can install this package using pip:
 
 pip install YWP
 
 ## Usage
 
 ```python
-from YWP import play_audio
-from YWP import stop_recording
-from YWP import delete_all_files
-from YWP import create_file
-from YWP import open_file
-from YWP import open_website
-from YWP import shutdown
-from YWP import record_audio
-from YWP import transcribe_audio
-from YWP import text_to_speech
-from YWP import play_sound
-
+from YWP import play_audio(pro_path, mp3_audio_file)
+from YWP import stop_recording()
+from YWP import create_file(name) :
+    name : the name of the file
+    body : show in cmd with input
+from YWP import open_file(filepath)
+from YWP import open_website(url)
+from YWP import shutdown()
+from YWP import record_audio(filename='recorder.wav')
+from YWP import transcribe_audio(filename='recorder.wav')
+from YWP import text_to_speech(text, filename="tts.mp3", language='en')
+from YWP import play_sound(filename='tts.mp3')
+from YWP import restart()
+from YWP import log_off()
+from YWP import hibernate()
+from YWP import play_audio_online(pro_path, mp3_file_link) :
+    pro_path : any program can run online audio like AIMP
+from YWP import token_information(data, type='binance') :
+    Supported Types Now:
+        1- binance
+        2- etherum
+        3- geckoterminal
+    data required:
+        1- binance (token)
+        2- etherum (token)
+        3- geckoterminal (pool)
 
-### `LICENSE`
+### LICENSE
 
 Choose a license, for YWP, the MIT license:
 ```text
 MIT License
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-...
+...
```

### Comparing `ywp-0.4.0/YWP/create_file.py` & `ywp-0.5.0/YWP/create_file.py`

 * *Files identical despite different names*

### Comparing `ywp-0.4.0/YWP/delete_all_files.py` & `ywp-0.5.0/YWP/delete_all_files.py`

 * *Files identical despite different names*

### Comparing `ywp-0.4.0/YWP/record_audio.py` & `ywp-0.5.0/YWP/record_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.4.0/YWP/transcribe_audio.py` & `ywp-0.5.0/YWP/transcribe_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.4.0/YWP/ywp.py` & `ywp-0.5.0/YWP/ywp.py`

 * *Files 19% similar despite different names*

```diff
@@ -122,8 +122,44 @@
 def play_sound(filename="tts.mp3"):
     pygame.mixer.init()
     sound = pygame.mixer.Sound(filename)
     sound.play()
     while pygame.mixer.get_busy():
         pygame.time.Clock().tick(10)
     sound.stop()
-    return "played"
+    return "played"
+
+def restart():
+    system = platform.system()
+    if system == "Windows":
+        os.system("shutdown /r /t 1")
+
+def log_off():
+    system = platform.system()
+    if system == "Windows":
+        os.system("shutdown /l")
+
+def hibernate():
+    system = platform.system()
+    if system == "Windows":
+        os.system("shutdown /h")
+
+def play_audio_online(aimp_path, mp3_file_link):
+        # قم بتشغيل AIMP وتمرير الملف الصوتي إليه
+        subprocess.Popen([aimp_path, mp3_file_link])
+        return "opened"
+
+def token_information(data, type='binance'):
+
+    if type == 'binance':
+        link = "https://bscscan.com/token/" + str(data)
+        open_website(link)
+        return "opened"
+    elif type == 'etherum':
+        link = "https://etherscan.io/token/" + str(data)
+        open_website(link)
+        return "opened"
+    elif type == 'geckoterminal':
+        link = 'https://ywp.freewebhostmost.com/really/token.php?pool=' + str(data)
+        return "opened"
+    else:
+        return "UnSupported type"
```

### Comparing `ywp-0.4.0/setup.py` & `ywp-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="YWP",
-    version="0.4.0",
+    version="0.5.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

