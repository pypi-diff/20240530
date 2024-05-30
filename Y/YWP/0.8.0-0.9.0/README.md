# Comparing `tmp/ywp-0.8.0.tar.gz` & `tmp/ywp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-0.8.0.tar", last modified: Thu May 30 10:28:15 2024, max compression
+gzip compressed data, was "ywp-0.9.0.tar", last modified: Thu May 30 14:53:11 2024, max compression
```

## Comparing `ywp-0.8.0.tar` & `ywp-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 10:28:15.912649 ywp-0.8.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     2231 2024-05-30 10:28:15.910653 ywp-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1712 2024-05-30 09:53:49.000000 ywp-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 10:28:15.883458 ywp-0.8.0/YWP/
--rw-rw-rw-   0        0        0      178 2024-05-30 09:57:41.000000 ywp-0.8.0/YWP/AIMP_Run.py
--rw-rw-rw-   0        0        0      586 2024-05-30 10:28:00.000000 ywp-0.8.0/YWP/__init__.py
--rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.8.0/YWP/create_file.py
--rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.8.0/YWP/delete_all_files.py
--rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-0.8.0/YWP/hibernate.py
--rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-0.8.0/YWP/log_off.py
--rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.8.0/YWP/open_file.py
--rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.8.0/YWP/open_website.py
--rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-0.8.0/YWP/play_audio.py
--rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-0.8.0/YWP/play_audio_online.py
--rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.8.0/YWP/play_sound.py
--rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.8.0/YWP/record_audio.py
--rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-0.8.0/YWP/restart.py
--rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.8.0/YWP/shutdown.py
--rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.8.0/YWP/stop_recording.py
--rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-0.8.0/YWP/text_to_speech.py
--rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-0.8.0/YWP/token_information.py
--rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.8.0/YWP/transcribe_audio.py
--rw-rw-rw-   0        0        0     5102 2024-05-30 09:10:45.000000 ywp-0.8.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 10:28:15.907651 ywp-0.8.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     2231 2024-05-30 10:28:15.000000 ywp-0.8.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-05-30 10:28:15.000000 ywp-0.8.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 10:28:15.000000 ywp-0.8.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 10:28:15.000000 ywp-0.8.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 10:28:15.000000 ywp-0.8.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 10:28:15.912649 ywp-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1562 2024-05-30 10:27:49.000000 ywp-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:53:11.601215 ywp-0.9.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2562 2024-05-30 14:53:11.597217 ywp-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2043 2024-05-30 14:51:10.000000 ywp-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 14:53:11.568233 ywp-0.9.0/YWP/
+-rw-rw-rw-   0        0        0      178 2024-05-30 14:23:35.000000 ywp-0.9.0/YWP/AIMP_Run.py
+-rw-rw-rw-   0        0        0      824 2024-05-30 14:50:57.000000 ywp-0.9.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0      289 2024-05-30 14:31:02.000000 ywp-0.9.0/YWP/add_task.py
+-rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.9.0/YWP/create_file.py
+-rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.9.0/YWP/delete_all_files.py
+-rw-rw-rw-   0        0        0      274 2024-05-30 14:41:36.000000 ywp-0.9.0/YWP/delete_all_tasks.py
+-rw-rw-rw-   0        0        0      369 2024-05-30 14:50:42.000000 ywp-0.9.0/YWP/delete_task.py
+-rw-rw-rw-   0        0        0      396 2024-05-30 14:42:06.000000 ywp-0.9.0/YWP/edit_mark_done.py
+-rw-rw-rw-   0        0        0      287 2024-05-30 14:42:28.000000 ywp-0.9.0/YWP/edit_task.py
+-rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-0.9.0/YWP/hibernate.py
+-rw-rw-rw-   0        0        0      237 2024-05-30 14:41:21.000000 ywp-0.9.0/YWP/load_tasks.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-0.9.0/YWP/log_off.py
+-rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.9.0/YWP/open_file.py
+-rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.9.0/YWP/open_website.py
+-rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-0.9.0/YWP/play_audio.py
+-rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-0.9.0/YWP/play_audio_online.py
+-rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.9.0/YWP/play_sound.py
+-rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.9.0/YWP/record_audio.py
+-rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-0.9.0/YWP/restart.py
+-rw-rw-rw-   0        0        0      338 2024-05-30 14:27:53.000000 ywp-0.9.0/YWP/settings.py
+-rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.9.0/YWP/shutdown.py
+-rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.9.0/YWP/stop_recording.py
+-rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-0.9.0/YWP/text_to_speech.py
+-rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-0.9.0/YWP/token_information.py
+-rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.9.0/YWP/transcribe_audio.py
+-rw-rw-rw-   0        0        0     6797 2024-05-30 14:51:49.000000 ywp-0.9.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:53:11.590221 ywp-0.9.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     2562 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:53:11.601215 ywp-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2024-05-30 14:52:16.000000 ywp-0.9.0/setup.py
```

### Comparing `ywp-0.8.0/YWP/create_file.py` & `ywp-0.9.0/YWP/create_file.py`

 * *Files identical despite different names*

### Comparing `ywp-0.8.0/YWP/delete_all_files.py` & `ywp-0.9.0/YWP/delete_all_files.py`

 * *Files identical despite different names*

### Comparing `ywp-0.8.0/YWP/record_audio.py` & `ywp-0.9.0/YWP/record_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.8.0/YWP/token_information.py` & `ywp-0.9.0/YWP/token_information.py`

 * *Files identical despite different names*

### Comparing `ywp-0.8.0/YWP/transcribe_audio.py` & `ywp-0.9.0/YWP/transcribe_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.8.0/setup.py` & `ywp-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import os
+# import os
 from setuptools import setup, find_packages
-from setuptools.command.install import install as InstallCommand
+# from setuptools.command.install import install as InstallCommand
 
 # class CustomInstallCommand(InstallCommand):
 #     def run(self):
 #         # Download the required file from a URL
 #         url = 'https://example.com/aimp.exe'
 #         os.system(f'curl -o aimp.exe {url}')  # Use appropriate command for downloading
 
 #         # Continue with the regular installation process
 #         super().run()
 
 setup(
     name="YWP",
-    version="0.8.0",
+    version="0.9.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

