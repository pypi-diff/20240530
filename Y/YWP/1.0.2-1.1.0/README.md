# Comparing `tmp/ywp-1.0.2.tar.gz` & `tmp/ywp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-1.0.2.tar", last modified: Thu May 30 16:54:29 2024, max compression
+gzip compressed data, was "ywp-1.1.0.tar", last modified: Thu May 30 17:15:08 2024, max compression
```

## Comparing `ywp-1.0.2.tar` & `ywp-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 16:54:29.928502 ywp-1.0.2/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2555 2024-05-30 16:54:29.926503 ywp-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2024-05-30 16:54:16.000000 ywp-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 16:54:29.906520 ywp-1.0.2/YWP/
--rw-rw-rw-   0        0        0      843 2024-05-30 16:54:22.000000 ywp-1.0.2/YWP/__init__.py
--rw-rw-rw-   0        0        0      289 2024-05-30 14:31:02.000000 ywp-1.0.2/YWP/add_task.py
--rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-1.0.2/YWP/create_file.py
--rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-1.0.2/YWP/delete_all_files.py
--rw-rw-rw-   0        0        0      274 2024-05-30 14:41:36.000000 ywp-1.0.2/YWP/delete_all_tasks.py
--rw-rw-rw-   0        0        0      369 2024-05-30 14:50:42.000000 ywp-1.0.2/YWP/delete_task.py
--rw-rw-rw-   0        0        0      391 2024-05-30 16:06:34.000000 ywp-1.0.2/YWP/edit_mark_done.py
--rw-rw-rw-   0        0        0      286 2024-05-30 16:06:01.000000 ywp-1.0.2/YWP/edit_task.py
--rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-1.0.2/YWP/hibernate.py
--rw-rw-rw-   0        0        0      237 2024-05-30 14:41:21.000000 ywp-1.0.2/YWP/load_tasks.py
--rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-1.0.2/YWP/log_off.py
--rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-1.0.2/YWP/open_file.py
--rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-1.0.2/YWP/open_website.py
--rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-1.0.2/YWP/play_audio.py
--rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-1.0.2/YWP/play_audio_online.py
--rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-1.0.2/YWP/play_sound.py
--rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-1.0.2/YWP/record_audio.py
--rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-1.0.2/YWP/restart.py
--rw-rw-rw-   0        0        0      338 2024-05-30 14:27:53.000000 ywp-1.0.2/YWP/settings.py
--rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-1.0.2/YWP/shutdown.py
--rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-1.0.2/YWP/stop_recording.py
--rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-1.0.2/YWP/text_to_speech.py
--rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-1.0.2/YWP/token_information.py
--rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-1.0.2/YWP/transcribe_audio.py
--rw-rw-rw-   0        0        0     6797 2024-05-30 14:51:49.000000 ywp-1.0.2/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 16:54:29.924503 ywp-1.0.2/YWP.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-30 16:54:29.000000 ywp-1.0.2/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2024-05-30 16:54:29.000000 ywp-1.0.2/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 16:54:29.000000 ywp-1.0.2/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 16:54:29.000000 ywp-1.0.2/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 16:54:29.000000 ywp-1.0.2/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 16:54:29.928502 ywp-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1566 2024-05-30 16:52:13.000000 ywp-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:08.075540 ywp-1.1.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2555 2024-05-30 17:15:08.072547 ywp-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2036 2024-05-30 16:54:16.000000 ywp-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:08.053556 ywp-1.1.0/YWP/
+-rw-rw-rw-   0        0        0      944 2024-05-30 17:05:01.000000 ywp-1.1.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-05-30 17:11:29.000000 ywp-1.1.0/YWP/add_task.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 17:12:49.000000 ywp-1.1.0/YWP/all_tasks.py
+-rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-1.1.0/YWP/create_file.py
+-rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-1.1.0/YWP/delete_all_files.py
+-rw-rw-rw-   0        0        0      405 2024-05-30 17:11:17.000000 ywp-1.1.0/YWP/delete_all_tasks.py
+-rw-rw-rw-   0        0        0      572 2024-05-30 17:12:14.000000 ywp-1.1.0/YWP/delete_task.py
+-rw-rw-rw-   0        0        0      602 2024-05-30 17:11:46.000000 ywp-1.1.0/YWP/edit_mark_done.py
+-rw-rw-rw-   0        0        0      489 2024-05-30 17:12:02.000000 ywp-1.1.0/YWP/edit_task.py
+-rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-1.1.0/YWP/hibernate.py
+-rw-rw-rw-   0        0        0      368 2024-05-30 17:11:05.000000 ywp-1.1.0/YWP/load_tasks.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-1.1.0/YWP/log_off.py
+-rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-1.1.0/YWP/open_file.py
+-rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-1.1.0/YWP/open_website.py
+-rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-1.1.0/YWP/play_audio.py
+-rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-1.1.0/YWP/play_audio_online.py
+-rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-1.1.0/YWP/play_sound.py
+-rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-1.1.0/YWP/record_audio.py
+-rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-1.1.0/YWP/restart.py
+-rw-rw-rw-   0        0        0      782 2024-05-30 17:13:23.000000 ywp-1.1.0/YWP/settings.py
+-rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-1.1.0/YWP/shutdown.py
+-rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-1.1.0/YWP/stop_recording.py
+-rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-1.1.0/YWP/text_to_speech.py
+-rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-1.1.0/YWP/token_information.py
+-rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-1.1.0/YWP/transcribe_audio.py
+-rw-rw-rw-   0        0        0     7239 2024-05-30 17:13:13.000000 ywp-1.1.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:15:08.070543 ywp-1.1.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:15:08.075540 ywp-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2024-05-30 17:00:05.000000 ywp-1.1.0/setup.py
```

### Comparing `ywp-1.0.2/PKG-INFO` & `ywp-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 1.0.2
+Version: 1.1.0
 Summary: A big Package has a lot of things
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ywp-1.0.2/README.md` & `ywp-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ywp-1.0.2/YWP/__init__.py` & `ywp-1.1.0/YWP/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 from .token_information import token_information
 from .load_tasks import load_tasks
 from .delete_all_tasks import delete_all_tasks
 from .add_task import add_task
 from .edit_mark_done import task_mark_done
 from .edit_task import edit_task
 from .delete_task import delete_task
-from .settings import *
+from .settings import tasks
+from .settings import marks
+from .settings import tasks_file
+from .settings import marks_file
```

### Comparing `ywp-1.0.2/YWP/create_file.py` & `ywp-1.1.0/YWP/create_file.py`

 * *Files identical despite different names*

### Comparing `ywp-1.0.2/YWP/delete_all_files.py` & `ywp-1.1.0/YWP/delete_all_files.py`

 * *Files identical despite different names*

### Comparing `ywp-1.0.2/YWP/record_audio.py` & `ywp-1.1.0/YWP/record_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-1.0.2/YWP/token_information.py` & `ywp-1.1.0/YWP/token_information.py`

 * *Files identical despite different names*

### Comparing `ywp-1.0.2/YWP/transcribe_audio.py` & `ywp-1.1.0/YWP/transcribe_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-1.0.2/YWP/ywp.py` & `ywp-1.1.0/YWP/ywp.py`

 * *Files 12% similar despite different names*

```diff
@@ -225,8 +225,30 @@
 
     with open (tasks_file, "w") as file:
         tasks = json.load(file)
     
     with open (marks_file, "w") as file:
         marks = json.load(file)
 
-    return 'loaded'
+    return 'loaded'
+
+def tasks():
+    if os.path.exists(tasks_file):
+        with open(tasks_file, "r") as f:
+            tasks = json.load(f)
+    else:
+        tasks = {}
+    return tasks
+
+def marks():
+    if os.path.exists(marks_file):
+        with open(marks_file, "r") as f:
+            marks = json.load(f)
+    else:
+        marks = {}
+    return marks
+
+def tasks_file():
+    return tasks_file
+
+def marks_file():
+    return marks_file
```

### Comparing `ywp-1.0.2/YWP.egg-info/PKG-INFO` & `ywp-1.1.0/YWP.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 1.0.2
+Version: 1.1.0
 Summary: A big Package has a lot of things
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ywp-1.0.2/YWP.egg-info/SOURCES.txt` & `ywp-1.1.0/YWP.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 YWP/__init__.py
 YWP/add_task.py
+YWP/all_tasks.py
 YWP/create_file.py
 YWP/delete_all_files.py
 YWP/delete_all_tasks.py
 YWP/delete_task.py
 YWP/edit_mark_done.py
 YWP/edit_task.py
 YWP/hibernate.py
```

### Comparing `ywp-1.0.2/setup.py` & `ywp-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #         os.system(f'curl -o aimp.exe {url}')  # Use appropriate command for downloading
 
 #         # Continue with the regular installation process
 #         super().run()
 
 setup(
     name="YWP",
-    version="1.0.2",
+    version="1.1.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

