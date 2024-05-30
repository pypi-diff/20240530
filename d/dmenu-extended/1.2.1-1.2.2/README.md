# Comparing `tmp/dmenu_extended-1.2.1.tar.gz` & `tmp/dmenu_extended-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmenu_extended-1.2.1.tar", last modified: Wed Nov 23 07:03:22 2022, max compression
+gzip compressed data, was "dmenu_extended-1.2.2.tar", last modified: Thu May 30 12:34:24 2024, max compression
```

## Comparing `dmenu_extended-1.2.1.tar` & `dmenu_extended-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-23 07:03:22.217542 dmenu_extended-1.2.1/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1084 2021-09-28 06:34:32.000000 dmenu_extended-1.2.1/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)    18264 2022-11-23 07:03:22.217542 dmenu_extended-1.2.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)    16420 2022-11-20 20:53:41.000000 dmenu_extended-1.2.1/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      914 2022-11-23 06:52:00.000000 dmenu_extended-1.2.1/pyproject.toml
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2022-11-23 07:03:22.217542 dmenu_extended-1.2.1/setup.cfg
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-23 07:03:22.161499 dmenu_extended-1.2.1/src/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-23 07:03:22.217542 dmenu_extended-1.2.1/src/dmenu_extended/
--rw-rw-r--   0 mark      (1000) mark      (1000)       20 2022-11-05 09:29:11.000000 dmenu_extended-1.2.1/src/dmenu_extended/__init__.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)     6733 2022-11-05 09:29:11.000000 dmenu_extended-1.2.1/src/dmenu_extended/install_systemd_service.py
--rwxrwxr-x   0 mark      (1000) mark      (1000)    88848 2022-11-23 06:52:00.000000 dmenu_extended-1.2.1/src/dmenu_extended/main.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2022-11-23 07:03:22.217542 dmenu_extended-1.2.1/src/dmenu_extended.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)    18264 2022-11-23 07:03:22.000000 dmenu_extended-1.2.1/src/dmenu_extended.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      349 2022-11-23 07:03:22.000000 dmenu_extended-1.2.1/src/dmenu_extended.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2022-11-23 07:03:22.000000 dmenu_extended-1.2.1/src/dmenu_extended.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      208 2022-11-23 07:03:22.000000 dmenu_extended-1.2.1/src/dmenu_extended.egg-info/entry_points.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       15 2022-11-23 07:03:22.000000 dmenu_extended-1.2.1/src/dmenu_extended.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:34:24.027971 dmenu_extended-1.2.2/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1084 2024-04-30 21:06:12.000000 dmenu_extended-1.2.2/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)    18293 2024-05-30 12:34:24.026971 dmenu_extended-1.2.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)    16417 2024-05-30 10:50:15.000000 dmenu_extended-1.2.2/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)      950 2024-05-30 12:30:33.000000 dmenu_extended-1.2.2/pyproject.toml
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-30 12:34:24.027971 dmenu_extended-1.2.2/setup.cfg
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:34:24.024972 dmenu_extended-1.2.2/src/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:34:24.025972 dmenu_extended-1.2.2/src/dmenu_extended/
+-rw-rw-r--   0 mark      (1000) mark      (1000)       20 2024-04-30 21:06:12.000000 dmenu_extended-1.2.2/src/dmenu_extended/__init__.py
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     6733 2024-04-30 21:06:12.000000 dmenu_extended-1.2.2/src/dmenu_extended/install_systemd_service.py
+-rwxrwxr-x   0 mark      (1000) mark      (1000)    88848 2024-05-30 12:30:33.000000 dmenu_extended-1.2.2/src/dmenu_extended/main.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:34:24.026971 dmenu_extended-1.2.2/src/dmenu_extended.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    18293 2024-05-30 12:34:24.000000 dmenu_extended-1.2.2/src/dmenu_extended.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      447 2024-05-30 12:34:24.000000 dmenu_extended-1.2.2/src/dmenu_extended.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-30 12:34:24.000000 dmenu_extended-1.2.2/src/dmenu_extended.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      208 2024-05-30 12:34:24.000000 dmenu_extended-1.2.2/src/dmenu_extended.egg-info/entry_points.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       17 2024-05-30 12:34:24.000000 dmenu_extended-1.2.2/src/dmenu_extended.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       15 2024-05-30 12:34:24.000000 dmenu_extended-1.2.2/src/dmenu_extended.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-30 12:34:24.026971 dmenu_extended-1.2.2/tests/
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     2603 2024-04-30 21:06:12.000000 dmenu_extended-1.2.2/tests/test_install_systemd_service.py
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     2679 2024-04-30 21:06:12.000000 dmenu_extended-1.2.2/tests/test_main.py
```

### Comparing `dmenu_extended-1.2.1/LICENSE` & `dmenu_extended-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmenu_extended-1.2.1/PKG-INFO` & `dmenu_extended-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmenu_extended
-Version: 1.2.1
+Version: 1.2.2
 Summary: A wrapper for dmenu that implements plugins and fast file/folder searching
 Author-email: Mark Hedley Jones <markhedleyjones@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2013 Mark Hedley Jones
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -28,20 +28,21 @@
 Project-URL: Bug Tracker, https://github.com/MarkHedleyJones/dmenu-extended/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools>=61.0
 
 <img src="https://travis-ci.org/MarkHedleyJones/dmenu-extended.svg?branch=master" alt="build:passed">
 
 # dmenu-extended
 
-An extension to the original [dmenu](http://tools.suckless.org/dmenu/) allowing super fast access to your files, folders, and programs. dmenu-extended has support for plugins, command aliasing, file filtering, and customisation. You can also use dmenu-extended with [rofi](https://davedavenport.github.io/rofi/)!.
+An extension to the original [dmenu](http://tools.suckless.org/dmenu/) allowing super fast access to your files, folders, and programs. dmenu-extended has support for plugins, command aliasing, file filtering, and customisation. You can also use dmenu-extended with [rofi](https://davatorium.github.io/rofi/)!.
 
 ## See it in action
 
 <p align="center">
   <img src="https://raw.github.com/markhedleyjones/dmenu-extended/master/docs/demo.gif" alt="Dmenu-extended demo"/>
 </p>
```

### Comparing `dmenu_extended-1.2.1/README.md` & `dmenu_extended-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="https://travis-ci.org/MarkHedleyJones/dmenu-extended.svg?branch=master" alt="build:passed">
 
 # dmenu-extended
 
-An extension to the original [dmenu](http://tools.suckless.org/dmenu/) allowing super fast access to your files, folders, and programs. dmenu-extended has support for plugins, command aliasing, file filtering, and customisation. You can also use dmenu-extended with [rofi](https://davedavenport.github.io/rofi/)!.
+An extension to the original [dmenu](http://tools.suckless.org/dmenu/) allowing super fast access to your files, folders, and programs. dmenu-extended has support for plugins, command aliasing, file filtering, and customisation. You can also use dmenu-extended with [rofi](https://davatorium.github.io/rofi/)!.
 
 ## See it in action
 
 <p align="center">
   <img src="https://raw.github.com/markhedleyjones/dmenu-extended/master/docs/demo.gif" alt="Dmenu-extended demo"/>
 </p>
```

### Comparing `dmenu_extended-1.2.1/pyproject.toml` & `dmenu_extended-1.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmenu_extended"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Mark Hedley Jones", email="markhedleyjones@gmail.com" },
 ]
 description = "A wrapper for dmenu that implements plugins and fast file/folder searching"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = ["setuptools>=61.0"]
 
 [project.scripts]
 "dmenu_extended_run" = "dmenu_extended.main:run"
 "dmenu_extended_cache_build" = "dmenu_extended.main:build_cache"
 "dmenu_extended_install_systemd_service" = "dmenu_extended.install_systemd_service:run"
 
 [project.urls]
```

### Comparing `dmenu_extended-1.2.1/src/dmenu_extended/install_systemd_service.py` & `dmenu_extended-1.2.2/src/dmenu_extended/install_systemd_service.py`

 * *Files identical despite different names*

### Comparing `dmenu_extended-1.2.1/src/dmenu_extended/main.py` & `dmenu_extended-1.2.2/src/dmenu_extended/main.py`

 * *Files identical despite different names*

### Comparing `dmenu_extended-1.2.1/src/dmenu_extended.egg-info/PKG-INFO` & `dmenu_extended-1.2.2/src/dmenu_extended.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dmenu-extended
-Version: 1.2.1
+Name: dmenu_extended
+Version: 1.2.2
 Summary: A wrapper for dmenu that implements plugins and fast file/folder searching
 Author-email: Mark Hedley Jones <markhedleyjones@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2013 Mark Hedley Jones
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -28,20 +28,21 @@
 Project-URL: Bug Tracker, https://github.com/MarkHedleyJones/dmenu-extended/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools>=61.0
 
 <img src="https://travis-ci.org/MarkHedleyJones/dmenu-extended.svg?branch=master" alt="build:passed">
 
 # dmenu-extended
 
-An extension to the original [dmenu](http://tools.suckless.org/dmenu/) allowing super fast access to your files, folders, and programs. dmenu-extended has support for plugins, command aliasing, file filtering, and customisation. You can also use dmenu-extended with [rofi](https://davedavenport.github.io/rofi/)!.
+An extension to the original [dmenu](http://tools.suckless.org/dmenu/) allowing super fast access to your files, folders, and programs. dmenu-extended has support for plugins, command aliasing, file filtering, and customisation. You can also use dmenu-extended with [rofi](https://davatorium.github.io/rofi/)!.
 
 ## See it in action
 
 <p align="center">
   <img src="https://raw.github.com/markhedleyjones/dmenu-extended/master/docs/demo.gif" alt="Dmenu-extended demo"/>
 </p>
```

