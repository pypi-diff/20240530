# Comparing `tmp/ywp-1.1.0.tar.gz` & `tmp/ywp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ywp-1.1.0.tar", last modified: Thu May 30 17:15:08 2024, max compression
+gzip compressed data, was "ywp-1.2.0.tar", last modified: Thu May 30 17:20:32 2024, max compression
```

## Comparing `ywp-1.1.0.tar` & `ywp-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 17:15:08.075540 ywp-1.1.0/
--rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2555 2024-05-30 17:15:08.072547 ywp-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2024-05-30 16:54:16.000000 ywp-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 17:15:08.053556 ywp-1.1.0/YWP/
--rw-rw-rw-   0        0        0      944 2024-05-30 17:05:01.000000 ywp-1.1.0/YWP/__init__.py
--rw-rw-rw-   0        0        0      484 2024-05-30 17:11:29.000000 ywp-1.1.0/YWP/add_task.py
--rw-rw-rw-   0        0        0      203 2024-05-30 17:12:49.000000 ywp-1.1.0/YWP/all_tasks.py
--rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-1.1.0/YWP/create_file.py
--rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-1.1.0/YWP/delete_all_files.py
--rw-rw-rw-   0        0        0      405 2024-05-30 17:11:17.000000 ywp-1.1.0/YWP/delete_all_tasks.py
--rw-rw-rw-   0        0        0      572 2024-05-30 17:12:14.000000 ywp-1.1.0/YWP/delete_task.py
--rw-rw-rw-   0        0        0      602 2024-05-30 17:11:46.000000 ywp-1.1.0/YWP/edit_mark_done.py
--rw-rw-rw-   0        0        0      489 2024-05-30 17:12:02.000000 ywp-1.1.0/YWP/edit_task.py
--rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-1.1.0/YWP/hibernate.py
--rw-rw-rw-   0        0        0      368 2024-05-30 17:11:05.000000 ywp-1.1.0/YWP/load_tasks.py
--rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-1.1.0/YWP/log_off.py
--rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-1.1.0/YWP/open_file.py
--rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-1.1.0/YWP/open_website.py
--rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-1.1.0/YWP/play_audio.py
--rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-1.1.0/YWP/play_audio_online.py
--rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-1.1.0/YWP/play_sound.py
--rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-1.1.0/YWP/record_audio.py
--rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-1.1.0/YWP/restart.py
--rw-rw-rw-   0        0        0      782 2024-05-30 17:13:23.000000 ywp-1.1.0/YWP/settings.py
--rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-1.1.0/YWP/shutdown.py
--rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-1.1.0/YWP/stop_recording.py
--rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-1.1.0/YWP/text_to_speech.py
--rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-1.1.0/YWP/token_information.py
--rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-1.1.0/YWP/transcribe_audio.py
--rw-rw-rw-   0        0        0     7239 2024-05-30 17:13:13.000000 ywp-1.1.0/YWP/ywp.py
-drwxrwxrwx   0        0        0        0 2024-05-30 17:15:08.070543 ywp-1.1.0/YWP.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-30 17:15:07.000000 ywp-1.1.0/YWP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 17:15:08.075540 ywp-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1566 2024-05-30 17:00:05.000000 ywp-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:20:32.806758 ywp-1.2.0/
+-rw-rw-rw-   0        0        0        0 2024-05-30 05:46:39.000000 ywp-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2694 2024-05-30 17:20:32.804755 ywp-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2175 2024-05-30 17:19:55.000000 ywp-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 17:20:32.786767 ywp-1.2.0/YWP/
+-rw-rw-rw-   0        0        0      976 2024-05-30 17:18:56.000000 ywp-1.2.0/YWP/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-05-30 17:11:29.000000 ywp-1.2.0/YWP/add_task.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 17:12:49.000000 ywp-1.2.0/YWP/all_tasks.py
+-rw-rw-rw-   0        0        0      656 2024-05-30 07:08:24.000000 ywp-1.2.0/YWP/create_file.py
+-rw-rw-rw-   0        0        0      526 2024-05-30 07:07:57.000000 ywp-1.2.0/YWP/delete_all_files.py
+-rw-rw-rw-   0        0        0      405 2024-05-30 17:11:17.000000 ywp-1.2.0/YWP/delete_all_tasks.py
+-rw-rw-rw-   0        0        0      572 2024-05-30 17:12:14.000000 ywp-1.2.0/YWP/delete_task.py
+-rw-rw-rw-   0        0        0      602 2024-05-30 17:11:46.000000 ywp-1.2.0/YWP/edit_mark_done.py
+-rw-rw-rw-   0        0        0      489 2024-05-30 17:12:02.000000 ywp-1.2.0/YWP/edit_task.py
+-rw-rw-rw-   0        0        0      205 2024-05-30 08:31:40.000000 ywp-1.2.0/YWP/hibernate.py
+-rw-rw-rw-   0        0        0      368 2024-05-30 17:11:05.000000 ywp-1.2.0/YWP/load_tasks.py
+-rw-rw-rw-   0        0        0      203 2024-05-30 08:31:36.000000 ywp-1.2.0/YWP/log_off.py
+-rw-rw-rw-   0        0        0      337 2024-05-30 07:09:22.000000 ywp-1.2.0/YWP/open_file.py
+-rw-rw-rw-   0        0        0      217 2024-05-30 07:08:55.000000 ywp-1.2.0/YWP/open_website.py
+-rw-rw-rw-   0        0        0      313 2024-05-30 09:15:16.000000 ywp-1.2.0/YWP/play_audio.py
+-rw-rw-rw-   0        0        0      226 2024-05-30 09:15:30.000000 ywp-1.2.0/YWP/play_audio_online.py
+-rw-rw-rw-   0        0        0      250 2024-05-30 07:12:31.000000 ywp-1.2.0/YWP/play_sound.py
+-rw-rw-rw-   0        0        0      579 2024-05-30 07:10:44.000000 ywp-1.2.0/YWP/record_audio.py
+-rw-rw-rw-   0        0        0      208 2024-05-30 08:31:31.000000 ywp-1.2.0/YWP/restart.py
+-rw-rw-rw-   0        0        0      782 2024-05-30 17:13:23.000000 ywp-1.2.0/YWP/settings.py
+-rw-rw-rw-   0        0        0      382 2024-05-30 07:10:03.000000 ywp-1.2.0/YWP/shutdown.py
+-rw-rw-rw-   0        0        0      132 2024-05-30 07:07:17.000000 ywp-1.2.0/YWP/stop_recording.py
+-rw-rw-rw-   0        0        0      166 2024-05-30 09:09:19.000000 ywp-1.2.0/YWP/text_to_speech.py
+-rw-rw-rw-   0        0        0      556 2024-05-30 09:06:12.000000 ywp-1.2.0/YWP/token_information.py
+-rw-rw-rw-   0        0        0      524 2024-05-30 07:11:19.000000 ywp-1.2.0/YWP/transcribe_audio.py
+-rw-rw-rw-   0        0        0     7239 2024-05-30 17:13:13.000000 ywp-1.2.0/YWP/ywp.py
+drwxrwxrwx   0        0        0        0 2024-05-30 17:20:32.801761 ywp-1.2.0/YWP.egg-info/
+-rw-rw-rw-   0        0        0     2694 2024-05-30 17:20:32.000000 ywp-1.2.0/YWP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-30 17:20:32.000000 ywp-1.2.0/YWP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 17:20:32.000000 ywp-1.2.0/YWP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-30 17:20:32.000000 ywp-1.2.0/YWP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-30 17:20:32.000000 ywp-1.2.0/YWP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 17:20:32.807757 ywp-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1566 2024-05-30 17:20:08.000000 ywp-1.2.0/setup.py
```

### Comparing `ywp-1.1.0/PKG-INFO` & `ywp-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 1.1.0
+Version: 1.2.0
 Summary: A big Package has a lot of things
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -60,14 +60,19 @@
 from YWP import edit_mark_done_task(task_name, new_mark="yes") :
     new_mark values:
         yes
         no
 from YWP import edit_tasks(task_name, new_task_dis)
 from YWP import load_tasks()
 from YWP import delete_task(task_name)
+from YWP import tasks()
+from YWP import marks()
+from YWP import tasks_file()
+from YWP import marks_file()
+from YWP import all_tasks()
 ```
 
 ### LICENSE
 
 MIT License
 ```
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ywp-1.1.0/README.md` & `ywp-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 from YWP import edit_mark_done_task(task_name, new_mark="yes") :
     new_mark values:
         yes
         no
 from YWP import edit_tasks(task_name, new_task_dis)
 from YWP import load_tasks()
 from YWP import delete_task(task_name)
+from YWP import tasks()
+from YWP import marks()
+from YWP import tasks_file()
+from YWP import marks_file()
+from YWP import all_tasks()
 ```
 
 ### LICENSE
 
 MIT License
 ```
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ywp-1.1.0/YWP/__init__.py` & `ywp-1.2.0/YWP/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 from .edit_mark_done import task_mark_done
 from .edit_task import edit_task
 from .delete_task import delete_task
 from .settings import tasks
 from .settings import marks
 from .settings import tasks_file
 from .settings import marks_file
+from .all_tasks import all_tasks
```

### Comparing `ywp-1.1.0/YWP/create_file.py` & `ywp-1.2.0/YWP/create_file.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/delete_all_files.py` & `ywp-1.2.0/YWP/delete_all_files.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/delete_task.py` & `ywp-1.2.0/YWP/delete_task.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/edit_mark_done.py` & `ywp-1.2.0/YWP/edit_mark_done.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/record_audio.py` & `ywp-1.2.0/YWP/record_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/settings.py` & `ywp-1.2.0/YWP/settings.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/token_information.py` & `ywp-1.2.0/YWP/token_information.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/transcribe_audio.py` & `ywp-1.2.0/YWP/transcribe_audio.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP/ywp.py` & `ywp-1.2.0/YWP/ywp.py`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/YWP.egg-info/PKG-INFO` & `ywp-1.2.0/YWP.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YWP
-Version: 1.1.0
+Version: 1.2.0
 Summary: A big Package has a lot of things
 Author: Your Wanted Products
 Author-email: pbstzidr@ywp.freewebhostmost.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -60,14 +60,19 @@
 from YWP import edit_mark_done_task(task_name, new_mark="yes") :
     new_mark values:
         yes
         no
 from YWP import edit_tasks(task_name, new_task_dis)
 from YWP import load_tasks()
 from YWP import delete_task(task_name)
+from YWP import tasks()
+from YWP import marks()
+from YWP import tasks_file()
+from YWP import marks_file()
+from YWP import all_tasks()
 ```
 
 ### LICENSE
 
 MIT License
 ```
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ywp-1.1.0/YWP.egg-info/SOURCES.txt` & `ywp-1.2.0/YWP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ywp-1.1.0/setup.py` & `ywp-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #         os.system(f'curl -o aimp.exe {url}')  # Use appropriate command for downloading
 
 #         # Continue with the regular installation process
 #         super().run()
 
 setup(
     name="YWP",
-    version="1.1.0",
+    version="1.2.0",
     packages=find_packages(),
     install_requires=[
         "SpeechRecognition",
         "gtts",
         "pygame",
         "sounddevice",
         "pyaudio"
```

