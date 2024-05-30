# Comparing `tmp/ywp-0.9.0.tar.gz` & `tmp/ywp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-0.9.0.tar", last modified: Thu May 30 14:53:11 2024, max compression
+gzip compressed data, was "ywp-0.9.1.tar", last modified: Thu May 30 16:30:22 2024, max compression
```

## Comparing `ywp-0.9.0.tar` & `ywp-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:53:11.601215 ywp-0.9.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     2562 2024-05-30 14:53:11.597217 ywp-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2043 2024-05-30 14:51:10.000000 ywp-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 14:53:11.568233 ywp-0.9.0/YWP/
--rw-rw-rw-   0        0        0      178 2024-05-30 14:23:35.000000 ywp-0.9.0/YWP/AIMP_Run.py
--rw-rw-rw-   0        0        0      824 2024-05-30 14:50:57.000000 ywp-0.9.0/YWP/__init__.py
--rw-rw-rw-   0        0        0      289 2024-05-30 14:31:02.000000 ywp-0.9.0/YWP/add_task.py
--rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.9.0/YWP/create_file.py
--rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.9.0/YWP/delete_all_files.py
--rw-rw-rw-   0        0        0      274 2024-05-30 14:41:36.000000 ywp-0.9.0/YWP/delete_all_tasks.py
--rw-rw-rw-   0        0        0      369 2024-05-30 14:50:42.000000 ywp-0.9.0/YWP/delete_task.py
--rw-rw-rw-   0        0        0      396 2024-05-30 14:42:06.000000 ywp-0.9.0/YWP/edit_mark_done.py
--rw-rw-rw-   0        0        0      287 2024-05-30 14:42:28.000000 ywp-0.9.0/YWP/edit_task.py
--rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-0.9.0/YWP/hibernate.py
--rw-rw-rw-   0        0        0      237 2024-05-30 14:41:21.000000 ywp-0.9.0/YWP/load_tasks.py
--rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-0.9.0/YWP/log_off.py
--rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.9.0/YWP/open_file.py
--rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.9.0/YWP/open_website.py
--rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-0.9.0/YWP/play_audio.py
--rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-0.9.0/YWP/play_audio_online.py
--rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.9.0/YWP/play_sound.py
--rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.9.0/YWP/record_audio.py
--rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-0.9.0/YWP/restart.py
--rw-rw-rw-   0        0        0      338 2024-05-30 14:27:53.000000 ywp-0.9.0/YWP/settings.py
--rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.9.0/YWP/shutdown.py
--rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.9.0/YWP/stop_recording.py
--rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-0.9.0/YWP/text_to_speech.py
--rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-0.9.0/YWP/token_information.py
--rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.9.0/YWP/transcribe_audio.py
--rw-rw-rw-   0        0        0     6797 2024-05-30 14:51:49.000000 ywp-0.9.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:53:11.590221 ywp-0.9.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     2562 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      652 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 14:53:09.000000 ywp-0.9.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 14:53:11.601215 ywp-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1566 2024-05-30 14:52:16.000000 ywp-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:22.042774 ywp-0.9.1/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     2562 2024-05-30 16:30:22.040777 ywp-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2043 2024-05-30 14:51:10.000000 ywp-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:22.022785 ywp-0.9.1/YWP/
+-rw-rw-rw-   0        0        0      818 2024-05-30 16:06:43.000000 ywp-0.9.1/YWP/__init__.py
+-rw-rw-rw-   0        0        0      289 2024-05-30 14:31:02.000000 ywp-0.9.1/YWP/add_task.py
+-rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-0.9.1/YWP/create_file.py
+-rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-0.9.1/YWP/delete_all_files.py
+-rw-rw-rw-   0        0        0      274 2024-05-30 14:41:36.000000 ywp-0.9.1/YWP/delete_all_tasks.py
+-rw-rw-rw-   0        0        0      369 2024-05-30 14:50:42.000000 ywp-0.9.1/YWP/delete_task.py
+-rw-rw-rw-   0        0        0      391 2024-05-30 16:06:34.000000 ywp-0.9.1/YWP/edit_mark_done.py
+-rw-rw-rw-   0        0        0      286 2024-05-30 16:06:01.000000 ywp-0.9.1/YWP/edit_task.py
+-rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-0.9.1/YWP/hibernate.py
+-rw-rw-rw-   0        0        0      237 2024-05-30 14:41:21.000000 ywp-0.9.1/YWP/load_tasks.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-0.9.1/YWP/log_off.py
+-rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-0.9.1/YWP/open_file.py
+-rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-0.9.1/YWP/open_website.py
+-rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-0.9.1/YWP/play_audio.py
+-rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-0.9.1/YWP/play_audio_online.py
+-rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-0.9.1/YWP/play_sound.py
+-rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-0.9.1/YWP/record_audio.py
+-rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-0.9.1/YWP/restart.py
+-rw-rw-rw-   0        0        0      338 2024-05-30 14:27:53.000000 ywp-0.9.1/YWP/settings.py
+-rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-0.9.1/YWP/shutdown.py
+-rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-0.9.1/YWP/stop_recording.py
+-rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-0.9.1/YWP/text_to_speech.py
+-rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-0.9.1/YWP/token_information.py
+-rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-0.9.1/YWP/transcribe_audio.py
+-rw-rw-rw-   0        0        0     6797 2024-05-30 14:51:49.000000 ywp-0.9.1/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:30:22.038775 ywp-0.9.1/YWP.egg-info/
+-rw-rw-rw-   0        0        0     2562 2024-05-30 16:30:21.000000 ywp-0.9.1/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-05-30 16:30:21.000000 ywp-0.9.1/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:30:21.000000 ywp-0.9.1/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 16:30:21.000000 ywp-0.9.1/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 16:30:21.000000 ywp-0.9.1/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 16:30:22.043775 ywp-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2024-05-30 16:30:04.000000 ywp-0.9.1/setup.py
```

### Comparing `ywp-0.9.0/PKG-INFO` & `ywp-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.9.0
+Version: 0.9.1
 Summary: A big Package has a lot of things
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ywp-0.9.0/README.md` & `ywp-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ywp-0.9.0/YWP/__init__.py` & `ywp-0.9.1/YWP/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 from .log_off import log_off
 from .hibernate import hibernate
 from .play_audio_online import play_audio_online
 from .token_information import token_information
 from .load_tasks import load_tasks
 from .delete_all_tasks import delete_all_tasks
 from .add_task import add_task
-from .edit_mark_done import edit_mark_done_task
-from .edit_task import edit_tasks
+from .edit_mark_done import task_mark_done
+from .edit_task import edit_task
 from .delete_task import delete_task
```

### Comparing `ywp-0.9.0/YWP/create_file.py` & `ywp-0.9.1/YWP/create_file.py`

 * *Files identical despite different names*

### Comparing `ywp-0.9.0/YWP/delete_all_files.py` & `ywp-0.9.1/YWP/delete_all_files.py`

 * *Files identical despite different names*

### Comparing `ywp-0.9.0/YWP/record_audio.py` & `ywp-0.9.1/YWP/record_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.9.0/YWP/token_information.py` & `ywp-0.9.1/YWP/token_information.py`

 * *Files identical despite different names*

### Comparing `ywp-0.9.0/YWP/transcribe_audio.py` & `ywp-0.9.1/YWP/transcribe_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-0.9.0/YWP/ywp.py` & `ywp-0.9.1/YWP/ywp.py`

 * *Files identical despite different names*

### Comparing `ywp-0.9.0/YWP.egg-info/PKG-INFO` & `ywp-0.9.1/YWP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 0.9.0
+Version: 0.9.1
 Summary: A big Package has a lot of things
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ywp-0.9.0/YWP.egg-info/SOURCES.txt` & `ywp-0.9.1/YWP.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 setup.py
-YWP/AIMP_Run.py
 YWP/__init__.py
 YWP/add_task.py
 YWP/create_file.py
 YWP/delete_all_files.py
 YWP/delete_all_tasks.py
 YWP/delete_task.py
 YWP/edit_mark_done.py
```

### Comparing `ywp-0.9.0/setup.py` & `ywp-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #         os.system(f'curl -o aimp.exe {url}')  # Use appropriate command for downloading
 
 #         # Continue with the regular installation process
 #         super().run()
 
 setup(
     name="YWP",
-    version="0.9.0",
+    version="0.9.1",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

