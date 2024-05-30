# Comparing `tmp/catask-3.0.1.tar.gz` & `tmp/catask-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catask-3.0.1.tar", last modified: Wed May 29 20:07:18 2024, max compression
+gzip compressed data, was "catask-3.0.2.tar", last modified: Thu May 30 20:39:32 2024, max compression
```

## Comparing `catask-3.0.1.tar` & `catask-3.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-29 20:07:18.958070 catask-3.0.1/
--rw-r--r--   0 artems     (502) staff       (20)     1070 2024-05-26 17:11:48.000000 catask-3.0.1/LICENSE
--rw-r--r--   0 artems     (502) staff       (20)     5663 2024-05-29 20:07:18.957729 catask-3.0.1/PKG-INFO
--rw-r--r--   0 artems     (502) staff       (20)     4818 2024-05-29 18:58:33.000000 catask-3.0.1/README.md
-drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-29 20:07:18.954748 catask-3.0.1/cata/
--rw-r--r--   0 artems     (502) staff       (20)    46341 2024-05-29 19:00:26.000000 catask-3.0.1/cata/__main__.py
--rw-r--r--   0 artems     (502) staff       (20)     2542 2024-05-26 17:23:49.000000 catask-3.0.1/cata/calendars.py
--rw-r--r--   0 artems     (502) staff       (20)     4245 2024-05-26 20:29:50.000000 catask-3.0.1/cata/colors.py
--rw-r--r--   0 artems     (502) staff       (20)    20459 2024-05-29 08:09:42.000000 catask-3.0.1/cata/configuration.py
--rw-r--r--   0 artems     (502) staff       (20)    28854 2024-05-29 08:07:59.000000 catask-3.0.1/cata/controls.py
--rw-r--r--   0 artems     (502) staff       (20)    14423 2024-05-26 20:29:50.000000 catask-3.0.1/cata/data.py
--rw-r--r--   0 artems     (502) staff       (20)     4025 2024-05-26 17:08:38.000000 catask-3.0.1/cata/dialogues.py
--rw-r--r--   0 artems     (502) staff       (20)     1467 2024-05-26 17:21:30.000000 catask-3.0.1/cata/errors.py
--rw-r--r--   0 artems     (502) staff       (20)     1479 2024-05-29 08:10:22.000000 catask-3.0.1/cata/importers.py
--rw-r--r--   0 artems     (502) staff       (20)    18062 2024-05-26 17:08:39.000000 catask-3.0.1/cata/loaders.py
--rw-r--r--   0 artems     (502) staff       (20)     2639 2024-05-26 17:23:23.000000 catask-3.0.1/cata/savers.py
--rw-r--r--   0 artems     (502) staff       (20)     5879 2024-05-26 17:08:39.000000 catask-3.0.1/cata/screen.py
-drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-29 20:07:18.955472 catask-3.0.1/cata/translations/
--rw-r--r--   0 artems     (502) staff       (20)     4250 2024-05-29 07:58:23.000000 catask-3.0.1/cata/translations/en.py
--rw-r--r--   0 artems     (502) staff       (20)     6969 2024-05-29 08:07:29.000000 catask-3.0.1/cata/translations/ru.py
--rw-r--r--   0 artems     (502) staff       (20)      986 2024-05-26 17:21:30.000000 catask-3.0.1/cata/weather.py
--rw-r--r--   0 artems     (502) staff       (20)      858 2024-05-26 17:18:03.000000 catask-3.0.1/cata.gz
-drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-29 20:07:18.957128 catask-3.0.1/catask.egg-info/
--rw-r--r--   0 artems     (502) staff       (20)     5663 2024-05-29 20:07:18.000000 catask-3.0.1/catask.egg-info/PKG-INFO
--rw-r--r--   0 artems     (502) staff       (20)      494 2024-05-29 20:07:18.000000 catask-3.0.1/catask.egg-info/SOURCES.txt
--rw-r--r--   0 artems     (502) staff       (20)        1 2024-05-29 20:07:18.000000 catask-3.0.1/catask.egg-info/dependency_links.txt
--rw-r--r--   0 artems     (502) staff       (20)       43 2024-05-29 20:07:18.000000 catask-3.0.1/catask.egg-info/entry_points.txt
--rw-r--r--   0 artems     (502) staff       (20)       35 2024-05-29 20:07:18.000000 catask-3.0.1/catask.egg-info/requires.txt
--rw-r--r--   0 artems     (502) staff       (20)        5 2024-05-29 20:07:18.000000 catask-3.0.1/catask.egg-info/top_level.txt
--rw-r--r--   0 artems     (502) staff       (20)       91 2024-05-26 17:08:02.000000 catask-3.0.1/pyproject.toml
--rw-r--r--   0 artems     (502) staff       (20)       38 2024-05-29 20:07:18.958303 catask-3.0.1/setup.cfg
--rw-r--r--   0 artems     (502) staff       (20)     1448 2024-05-29 20:07:11.000000 catask-3.0.1/setup.py
+drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-30 20:39:32.842321 catask-3.0.2/
+-rw-r--r--   0 artems     (502) staff       (20)     1070 2024-05-26 17:11:48.000000 catask-3.0.2/LICENSE
+-rw-r--r--   0 artems     (502) staff       (20)     5671 2024-05-30 20:39:32.842007 catask-3.0.2/PKG-INFO
+-rw-r--r--   0 artems     (502) staff       (20)     4826 2024-05-29 20:10:02.000000 catask-3.0.2/README.md
+drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-30 20:39:32.840242 catask-3.0.2/cata/
+-rw-r--r--   0 artems     (502) staff       (20)    46341 2024-05-30 20:39:05.000000 catask-3.0.2/cata/__main__.py
+-rw-r--r--   0 artems     (502) staff       (20)     2542 2024-05-26 17:23:49.000000 catask-3.0.2/cata/calendars.py
+-rw-r--r--   0 artems     (502) staff       (20)     4245 2024-05-26 20:29:50.000000 catask-3.0.2/cata/colors.py
+-rw-r--r--   0 artems     (502) staff       (20)    20459 2024-05-30 20:38:59.000000 catask-3.0.2/cata/configuration.py
+-rw-r--r--   0 artems     (502) staff       (20)    28854 2024-05-29 08:07:59.000000 catask-3.0.2/cata/controls.py
+-rw-r--r--   0 artems     (502) staff       (20)    14423 2024-05-26 20:29:50.000000 catask-3.0.2/cata/data.py
+-rw-r--r--   0 artems     (502) staff       (20)     4025 2024-05-26 17:08:38.000000 catask-3.0.2/cata/dialogues.py
+-rw-r--r--   0 artems     (502) staff       (20)     1467 2024-05-26 17:21:30.000000 catask-3.0.2/cata/errors.py
+-rw-r--r--   0 artems     (502) staff       (20)     1479 2024-05-29 08:10:22.000000 catask-3.0.2/cata/importers.py
+-rw-r--r--   0 artems     (502) staff       (20)    18178 2024-05-30 20:26:36.000000 catask-3.0.2/cata/loaders.py
+-rw-r--r--   0 artems     (502) staff       (20)     2639 2024-05-26 17:23:23.000000 catask-3.0.2/cata/savers.py
+-rw-r--r--   0 artems     (502) staff       (20)     5879 2024-05-26 17:08:39.000000 catask-3.0.2/cata/screen.py
+drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-30 20:39:32.840794 catask-3.0.2/cata/translations/
+-rw-r--r--   0 artems     (502) staff       (20)     4250 2024-05-29 07:58:23.000000 catask-3.0.2/cata/translations/en.py
+-rw-r--r--   0 artems     (502) staff       (20)     6969 2024-05-29 08:07:29.000000 catask-3.0.2/cata/translations/ru.py
+-rw-r--r--   0 artems     (502) staff       (20)      986 2024-05-26 17:21:30.000000 catask-3.0.2/cata/weather.py
+-rw-r--r--   0 artems     (502) staff       (20)      858 2024-05-26 17:18:03.000000 catask-3.0.2/cata.gz
+drwxr-xr-x   0 artems     (502) staff       (20)        0 2024-05-30 20:39:32.841752 catask-3.0.2/catask.egg-info/
+-rw-r--r--   0 artems     (502) staff       (20)     5671 2024-05-30 20:39:32.000000 catask-3.0.2/catask.egg-info/PKG-INFO
+-rw-r--r--   0 artems     (502) staff       (20)      494 2024-05-30 20:39:32.000000 catask-3.0.2/catask.egg-info/SOURCES.txt
+-rw-r--r--   0 artems     (502) staff       (20)        1 2024-05-30 20:39:32.000000 catask-3.0.2/catask.egg-info/dependency_links.txt
+-rw-r--r--   0 artems     (502) staff       (20)       43 2024-05-30 20:39:32.000000 catask-3.0.2/catask.egg-info/entry_points.txt
+-rw-r--r--   0 artems     (502) staff       (20)       35 2024-05-30 20:39:32.000000 catask-3.0.2/catask.egg-info/requires.txt
+-rw-r--r--   0 artems     (502) staff       (20)        5 2024-05-30 20:39:32.000000 catask-3.0.2/catask.egg-info/top_level.txt
+-rw-r--r--   0 artems     (502) staff       (20)       91 2024-05-26 17:08:02.000000 catask-3.0.2/pyproject.toml
+-rw-r--r--   0 artems     (502) staff       (20)       38 2024-05-30 20:39:32.842361 catask-3.0.2/setup.cfg
+-rw-r--r--   0 artems     (502) staff       (20)     1448 2024-05-29 20:07:11.000000 catask-3.0.2/setup.py
```

### Comparing `catask-3.0.1/LICENSE` & `catask-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/PKG-INFO` & `catask-3.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catask
-Version: 3.0.1
+Version: 3.0.2
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/temiksvyatov/cata
 Author: Artem Svyatov
 Author-email: temiksvyatov@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -45,26 +45,26 @@
 
 ## Установка
 
 ### Linux и Mac OS
 
 Есть несколько способов установки:
 
-`pipx install cata` - актуальная версия с PyPi. Возможно, вам нужно сначала установить `pipx`.
+`pipx install catask` - актуальная версия с PyPi. Возможно, вам нужно сначала установить `pipx`.
 
 ### Windows
 
 1. Установите приложение `Windows Terminal` из магазина приложений
 2. Установите `python 3.x` также из магазина приложений (если вы просто наберете `python` в приложении Windows Terminal, оно предложит вам установить)
-3. Установите программу и библиотеки, набрав в Windows Terminal `pip install windows-curses cata`
-4. Теперь вы можете запустить программу, набрав в Windows Terminal `python -m cata`
+3. Установите программу и библиотеки, набрав в Windows Terminal `pip install windows-curses catask`
+4. Теперь вы можете запустить программу, набрав в Windows Terminal `python -m catask`
 
 ### Обновление до последней версии
 
-`pipx upgrade cata`
+`pipx upgrade catask`
 
 ### Зависимости
 
 - `python` версии 3.7 и выше (обычно уже установлен)
 - библиотеки `holidays`, `jdatetime`, `icalendar` и `taskw` для python (должны быть установлены автоматически вместе с cata).
 - `windows-cata` для Windows
```

### Comparing `catask-3.0.1/README.md` & `catask-3.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 
 ## Установка
 
 ### Linux и Mac OS
 
 Есть несколько способов установки:
 
-`pipx install cata` - актуальная версия с PyPi. Возможно, вам нужно сначала установить `pipx`.
+`pipx install catask` - актуальная версия с PyPi. Возможно, вам нужно сначала установить `pipx`.
 
 ### Windows
 
 1. Установите приложение `Windows Terminal` из магазина приложений
 2. Установите `python 3.x` также из магазина приложений (если вы просто наберете `python` в приложении Windows Terminal, оно предложит вам установить)
-3. Установите программу и библиотеки, набрав в Windows Terminal `pip install windows-curses cata`
-4. Теперь вы можете запустить программу, набрав в Windows Terminal `python -m cata`
+3. Установите программу и библиотеки, набрав в Windows Terminal `pip install windows-curses catask`
+4. Теперь вы можете запустить программу, набрав в Windows Terminal `python -m catask`
 
 ### Обновление до последней версии
 
-`pipx upgrade cata`
+`pipx upgrade catask`
 
 ### Зависимости
 
 - `python` версии 3.7 и выше (обычно уже установлен)
 - библиотеки `holidays`, `jdatetime`, `icalendar` и `taskw` для python (должны быть установлены автоматически вместе с cata).
 - `windows-cata` для Windows
```

### Comparing `catask-3.0.1/cata/__main__.py` & `catask-3.0.2/cata/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # Language:
 if cf.LANG == "ru":
     from cata.translations.ru import *
 else:
     from cata.translations.en import *
 
 
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
 
 def read_items_from_user_arguments(
     screen, user_tasks, user_events, task_saver_csv, event_saver_csv
 ):
     """Read --task and --event flags from user arguments to create new tasks or events"""
     try:
```

### Comparing `catask-3.0.1/cata/calendars.py` & `catask-3.0.2/cata/calendars.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/colors.py` & `catask-3.0.2/cata/colors.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/configuration.py` & `catask-3.0.2/cata/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,13 +496,13 @@
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt == "-d":
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt in ("-h"):
                     self.DEFAULT_VIEW = AppState.HELP
                 elif opt in ("-v"):
                     self.DEFAULT_VIEW = AppState.EXIT
-                    print("Cata - version 3.0.1")
+                    print("Cata - version 3.0.2")
                 elif opt in ("-i"):
                     self.USE_PERSIAN_CALENDAR = True
         except getopt.GetoptError as e_message:
             logging.error("Invalid user arguments. %s", e_message)
             pass
```

### Comparing `catask-3.0.1/cata/controls.py` & `catask-3.0.2/cata/controls.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/data.py` & `catask-3.0.2/cata/data.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/dialogues.py` & `catask-3.0.2/cata/dialogues.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/errors.py` & `catask-3.0.2/cata/errors.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/importers.py` & `catask-3.0.2/cata/importers.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/loaders.py` & `catask-3.0.2/cata/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Module that controls loading data from files and libraries"""
 
 import configparser
 import csv
 import os
 import datetime
+import ssl
 import time
 import icalendar
 import urllib.request
 import io
 import logging
+import certifi
 
 from pathlib import Path
 
 from cata.data import *
 from cata.calendars import convert_to_persian_date, convert_to_gregorian_date
 
 
@@ -295,15 +297,16 @@
             return ""
         with open(path, "r", encoding="utf-8") as file:
             return self.read_lines(file)
 
     def read_url(self, path):
         """Parse an ics URL if it exists and networks works"""
         try:
-            with urllib.request.urlopen(path) as response:
+            context = ssl.create_default_context(cafile=certifi.where())
+            with urllib.request.urlopen(path, context=context) as response:
                 file = io.TextIOWrapper(response, "utf-8")
                 return self.read_lines(file)
         except urllib.error.HTTPError as e_message:
             logging.error(
                 "Failed to load from %s. Probably url is wrong. %s", path, e_message
             )
             return ""
```

### Comparing `catask-3.0.1/cata/savers.py` & `catask-3.0.2/cata/savers.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/screen.py` & `catask-3.0.2/cata/screen.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/translations/en.py` & `catask-3.0.2/cata/translations/en.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/translations/ru.py` & `catask-3.0.2/cata/translations/ru.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata/weather.py` & `catask-3.0.2/cata/weather.py`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/cata.gz` & `catask-3.0.2/cata.gz`

 * *Files identical despite different names*

### Comparing `catask-3.0.1/catask.egg-info/PKG-INFO` & `catask-3.0.2/catask.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catask
-Version: 3.0.1
+Version: 3.0.2
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/temiksvyatov/cata
 Author: Artem Svyatov
 Author-email: temiksvyatov@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -45,26 +45,26 @@
 
 ## Установка
 
 ### Linux и Mac OS
 
 Есть несколько способов установки:
 
-`pipx install cata` - актуальная версия с PyPi. Возможно, вам нужно сначала установить `pipx`.
+`pipx install catask` - актуальная версия с PyPi. Возможно, вам нужно сначала установить `pipx`.
 
 ### Windows
 
 1. Установите приложение `Windows Terminal` из магазина приложений
 2. Установите `python 3.x` также из магазина приложений (если вы просто наберете `python` в приложении Windows Terminal, оно предложит вам установить)
-3. Установите программу и библиотеки, набрав в Windows Terminal `pip install windows-curses cata`
-4. Теперь вы можете запустить программу, набрав в Windows Terminal `python -m cata`
+3. Установите программу и библиотеки, набрав в Windows Terminal `pip install windows-curses catask`
+4. Теперь вы можете запустить программу, набрав в Windows Terminal `python -m catask`
 
 ### Обновление до последней версии
 
-`pipx upgrade cata`
+`pipx upgrade catask`
 
 ### Зависимости
 
 - `python` версии 3.7 и выше (обычно уже установлен)
 - библиотеки `holidays`, `jdatetime`, `icalendar` и `taskw` для python (должны быть установлены автоматически вместе с cata).
 - `windows-cata` для Windows
```

### Comparing `catask-3.0.1/setup.py` & `catask-3.0.2/setup.py`

 * *Files identical despite different names*

