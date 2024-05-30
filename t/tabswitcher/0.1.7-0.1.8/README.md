# Comparing `tmp/tabswitcher-0.1.7.tar.gz` & `tmp/tabswitcher-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabswitcher-0.1.7.tar", last modified: Wed May 29 19:52:57 2024, max compression
+gzip compressed data, was "tabswitcher-0.1.8.tar", last modified: Wed May 29 20:56:24 2024, max compression
```

## Comparing `tabswitcher-0.1.7.tar` & `tabswitcher-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.868142 tabswitcher-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.872142 tabswitcher-0.1.7/src/tabswitcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/NetworkImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/SearchInput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/TabList.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/VisibilityChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/src/tabswitcher/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/Icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/install.bat
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/sans.ttf
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/searchIcon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/assets/tabswitcher_service.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/brotab.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/focusWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/fuzzySearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/loadBookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/logTabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 19:52:53.000000 tabswitcher-0.1.7/src/tabswitcher/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:52:57.876142 tabswitcher-0.1.7/tabswitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 19:52:57.000000 tabswitcher-0.1.7/tabswitcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.205737 tabswitcher-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.209737 tabswitcher-0.1.8/src/tabswitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/NetworkImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/SearchInput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/TabList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/VisibilityChecker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/src/tabswitcher/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    76802 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/Icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/runLogger.vbs
+-rw-r--r--   0 runner    (1001) docker     (127)   529700 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/searchIcon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/assets/tabswitcher_service.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/brotab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/focusWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/fuzzySearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/loadBookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/logTabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 20:56:20.000000 tabswitcher-0.1.8/src/tabswitcher/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:56:24.213737 tabswitcher-0.1.8/tabswitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 20:56:24.000000 tabswitcher-0.1.8/tabswitcher.egg-info/top_level.txt
```

### Comparing `tabswitcher-0.1.7/LICENCE` & `tabswitcher-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/PKG-INFO` & `tabswitcher-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.1.7/README.md` & `tabswitcher-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/setup.py` & `tabswitcher-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tabswitcher',
-    version='0.1.7',
+    version='0.1.8',
     packages=['tabswitcher'],
     package_dir={'tabswitcher': 'src/tabswitcher'},
     package_data={'tabswitcher': ['assets/*']},
     description="A tool for efficient browser tab switching outside the browser",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='YukiGasai',
```

### Comparing `tabswitcher-0.1.7/src/tabswitcher/NetworkImage.py` & `tabswitcher-0.1.8/src/tabswitcher/NetworkImage.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/SearchInput.py` & `tabswitcher-0.1.8/src/tabswitcher/SearchInput.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/Settings.py` & `tabswitcher-0.1.8/src/tabswitcher/Settings.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/Tab.py` & `tabswitcher-0.1.8/src/tabswitcher/Tab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/TabList.py` & `tabswitcher-0.1.8/src/tabswitcher/TabList.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/VisibilityChecker.py` & `tabswitcher-0.1.8/src/tabswitcher/VisibilityChecker.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/__main__.py` & `tabswitcher-0.1.8/src/tabswitcher/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pickle
 
 import platform
+import shutil
 import sys
-from PyQt5.QtGui import QFont, QCursor, QDesktopServices, QIcon
-from PyQt5.QtCore import Qt, QUrl
+from PyQt5.QtGui import QFont, QCursor, QIcon
+from PyQt5.QtCore import Qt
 from PyQt5.QtWidgets import QApplication, QWidget, QVBoxLayout, QLabel
 from PyQt5.QtNetwork import QNetworkAccessManager
 import subprocess
 
 import pkg_resources
 
 from tabswitcher.Tab import Tab
@@ -313,17 +314,20 @@
     elif len(sys.argv) > 1 and sys.argv[1] == "--latest":
         if len(sys.argv) > 2:
             print_recent_tabs(sys.argv[2])
         else:
             print_recent_tabs()
     elif len(sys.argv) > 1 and sys.argv[1] == "--install":
         if platform.system() == "Windows":
-            batch_script = os.path.join(script_dir, "assets", "install.bat")
-            subprocess.run(["cmd", "/c", batch_script])
-
+            subprocess.run(["bt", "install"], check=True)
+            startup_script = os.path.join(script_dir, "assets", "runLogger.vbs")
+            startup_folder = os.path.join(os.environ["APPDATA"], r"Microsoft\Windows\Start Menu\Programs\Startup")
+            vbs_path = os.path.join(startup_folder, "runLogger.vbs")
+            shutil.copy2(startup_script, vbs_path)
+            subprocess.Popen(["cscript", vbs_path])
         else:
             batch_script = os.path.join(script_dir, "assets", "install.sh")
             subprocess.run(["sh", batch_script])
 
 
     elif len(sys.argv) > 1 and sys.argv[1] == "--version":
         version = pkg_resources.get_distribution("tabswitcher").version
```

### Comparing `tabswitcher-0.1.7/src/tabswitcher/actions.py` & `tabswitcher-0.1.8/src/tabswitcher/actions.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/assets/Icon.ico` & `tabswitcher-0.1.8/src/tabswitcher/assets/Icon.ico`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/assets/sans.ttf` & `tabswitcher-0.1.8/src/tabswitcher/assets/sans.ttf`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/assets/tabswitcher_service.xml` & `tabswitcher-0.1.8/src/tabswitcher/assets/tabswitcher_service.xml`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/brotab.py` & `tabswitcher-0.1.8/src/tabswitcher/brotab.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/colors.py` & `tabswitcher-0.1.8/src/tabswitcher/colors.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/focusWindow.py` & `tabswitcher-0.1.8/src/tabswitcher/focusWindow.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/fuzzySearch.py` & `tabswitcher-0.1.8/src/tabswitcher/fuzzySearch.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/loadBookmarks.py` & `tabswitcher-0.1.8/src/tabswitcher/loadBookmarks.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/src/tabswitcher/logTabs.py` & `tabswitcher-0.1.8/src/tabswitcher/logTabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import platform
 import subprocess
 import schedule
 import time
 from collections import deque
 import pickle
```

### Comparing `tabswitcher-0.1.7/src/tabswitcher/shortcuts.py` & `tabswitcher-0.1.8/src/tabswitcher/shortcuts.py`

 * *Files identical despite different names*

### Comparing `tabswitcher-0.1.7/tabswitcher.egg-info/PKG-INFO` & `tabswitcher-0.1.8/tabswitcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabswitcher
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for efficient browser tab switching outside the browser
 Home-page: https://github.com/YukiGasai/tabswitcher
 Author: YukiGasai
 Author-email: r.lindede@googlemail.com
 License: AGPL-3.0
 Keywords: tabswitcher,browsertool,tool
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tabswitcher-0.1.7/tabswitcher.egg-info/SOURCES.txt` & `tabswitcher-0.1.8/tabswitcher.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 src/tabswitcher/colors.py
 src/tabswitcher/focusWindow.py
 src/tabswitcher/fuzzySearch.py
 src/tabswitcher/loadBookmarks.py
 src/tabswitcher/logTabs.py
 src/tabswitcher/shortcuts.py
 src/tabswitcher/assets/Icon.ico
-src/tabswitcher/assets/install.bat
 src/tabswitcher/assets/install.sh
+src/tabswitcher/assets/runLogger.vbs
 src/tabswitcher/assets/sans.ttf
 src/tabswitcher/assets/searchIcon.svg
 src/tabswitcher/assets/tabswitcher_service.xml
 tabswitcher.egg-info/PKG-INFO
 tabswitcher.egg-info/SOURCES.txt
 tabswitcher.egg-info/dependency_links.txt
 tabswitcher.egg-info/entry_points.txt
```

