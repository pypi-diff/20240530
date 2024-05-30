# Comparing `tmp/clipassman-0.5.0.tar.gz` & `tmp/clipassman-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipassman-0.5.0.tar", last modified: Thu May 30 12:32:41 2024, max compression
+gzip compressed data, was "clipassman-0.5.1.tar", last modified: Thu May 30 12:44:41 2024, max compression
```

## Comparing `clipassman-0.5.0.tar` & `clipassman-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-30 12:32:41.281866 clipassman-0.5.0/
--rw-r--r--   0 smart     (1000) smart     (1000)     1499 2024-05-24 03:21:47.000000 clipassman-0.5.0/LICENSE
--rw-r--r--   0 smart     (1000) smart     (1000)      184 2024-05-30 11:54:54.000000 clipassman-0.5.0/MANIFEST.in
--rw-r--r--   0 smart     (1000) smart     (1000)     5506 2024-05-30 12:32:41.281866 clipassman-0.5.0/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)     4120 2024-05-30 12:29:00.000000 clipassman-0.5.0/README.md
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-30 12:32:41.281866 clipassman-0.5.0/clipassman/
--rw-r--r--   0 smart     (1000) smart     (1000)      443 2024-05-30 12:25:51.000000 clipassman-0.5.0/clipassman/__init__.py
--rw-r--r--   0 smart     (1000) smart     (1000)      701 2024-05-30 12:10:17.000000 clipassman-0.5.0/clipassman/app.py
--rw-r--r--   0 smart     (1000) smart     (1000)     6894 2024-05-30 12:14:21.000000 clipassman-0.5.0/clipassman/commander.py
--rw-r--r--   0 smart     (1000) smart     (1000)      767 2024-05-30 12:29:00.000000 clipassman-0.5.0/clipassman/manager.py
--rw-r--r--   0 smart     (1000) smart     (1000)     5056 2024-05-30 12:12:11.000000 clipassman-0.5.0/clipassman/passman.py
-drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-30 12:32:41.281866 clipassman-0.5.0/clipassman.egg-info/
--rw-r--r--   0 smart     (1000) smart     (1000)     5506 2024-05-30 12:32:41.000000 clipassman-0.5.0/clipassman.egg-info/PKG-INFO
--rw-r--r--   0 smart     (1000) smart     (1000)      421 2024-05-30 12:32:41.000000 clipassman-0.5.0/clipassman.egg-info/SOURCES.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-30 12:32:41.000000 clipassman-0.5.0/clipassman.egg-info/dependency_links.txt
--rw-r--r--   0 smart     (1000) smart     (1000)       50 2024-05-30 12:32:41.000000 clipassman-0.5.0/clipassman.egg-info/entry_points.txt
--rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-30 12:32:41.000000 clipassman-0.5.0/clipassman.egg-info/not-zip-safe
--rw-r--r--   0 smart     (1000) smart     (1000)       52 2024-05-30 12:32:41.000000 clipassman-0.5.0/clipassman.egg-info/requires.txt
--rw-r--r--   0 smart     (1000) smart     (1000)       11 2024-05-30 12:32:41.000000 clipassman-0.5.0/clipassman.egg-info/top_level.txt
--rw-r--r--   0 smart     (1000) smart     (1000)       51 2024-05-30 12:05:06.000000 clipassman-0.5.0/requirements.txt
--rw-r--r--   0 smart     (1000) smart     (1000)     1553 2024-05-30 12:32:41.281866 clipassman-0.5.0/setup.cfg
--rw-r--r--   0 smart     (1000) smart     (1000)      479 2024-05-30 12:30:55.000000 clipassman-0.5.0/setup.py
--rw-r--r--   0 smart     (1000) smart     (1000)      139 2024-05-30 11:57:25.000000 clipassman-0.5.0/tox.ini
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-30 12:44:41.619809 clipassman-0.5.1/
+-rw-r--r--   0 smart     (1000) smart     (1000)     1499 2024-05-24 03:21:47.000000 clipassman-0.5.1/LICENSE
+-rw-r--r--   0 smart     (1000) smart     (1000)      184 2024-05-30 11:54:54.000000 clipassman-0.5.1/MANIFEST.in
+-rw-r--r--   0 smart     (1000) smart     (1000)     6279 2024-05-30 12:44:41.619809 clipassman-0.5.1/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)     4893 2024-05-30 12:43:54.000000 clipassman-0.5.1/README.md
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-30 12:44:41.616475 clipassman-0.5.1/clipassman/
+-rw-r--r--   0 smart     (1000) smart     (1000)      443 2024-05-30 12:43:54.000000 clipassman-0.5.1/clipassman/__init__.py
+-rw-r--r--   0 smart     (1000) smart     (1000)      701 2024-05-30 12:10:17.000000 clipassman-0.5.1/clipassman/app.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     6894 2024-05-30 12:14:21.000000 clipassman-0.5.1/clipassman/commander.py
+-rw-r--r--   0 smart     (1000) smart     (1000)      767 2024-05-30 12:29:00.000000 clipassman-0.5.1/clipassman/manager.py
+-rw-r--r--   0 smart     (1000) smart     (1000)     5056 2024-05-30 12:12:11.000000 clipassman-0.5.1/clipassman/passman.py
+drwxr-xr-x   0 smart     (1000) smart     (1000)        0 2024-05-30 12:44:41.616475 clipassman-0.5.1/clipassman.egg-info/
+-rw-r--r--   0 smart     (1000) smart     (1000)     6279 2024-05-30 12:44:41.000000 clipassman-0.5.1/clipassman.egg-info/PKG-INFO
+-rw-r--r--   0 smart     (1000) smart     (1000)      421 2024-05-30 12:44:41.000000 clipassman-0.5.1/clipassman.egg-info/SOURCES.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-30 12:44:41.000000 clipassman-0.5.1/clipassman.egg-info/dependency_links.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)       50 2024-05-30 12:44:41.000000 clipassman-0.5.1/clipassman.egg-info/entry_points.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)        1 2024-05-30 12:44:41.000000 clipassman-0.5.1/clipassman.egg-info/not-zip-safe
+-rw-r--r--   0 smart     (1000) smart     (1000)       52 2024-05-30 12:44:41.000000 clipassman-0.5.1/clipassman.egg-info/requires.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)       11 2024-05-30 12:44:41.000000 clipassman-0.5.1/clipassman.egg-info/top_level.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)       51 2024-05-30 12:05:06.000000 clipassman-0.5.1/requirements.txt
+-rw-r--r--   0 smart     (1000) smart     (1000)     1553 2024-05-30 12:44:41.619809 clipassman-0.5.1/setup.cfg
+-rw-r--r--   0 smart     (1000) smart     (1000)      479 2024-05-30 12:30:55.000000 clipassman-0.5.1/setup.py
+-rw-r--r--   0 smart     (1000) smart     (1000)      139 2024-05-30 11:57:25.000000 clipassman-0.5.1/tox.ini
```

### Comparing `clipassman-0.5.0/LICENSE` & `clipassman-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clipassman-0.5.0/PKG-INFO` & `clipassman-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipassman
-Version: 0.5.0
+Version: 0.5.1
 Summary: Cross-platform console smart password generator and manager.
 Home-page: https://github.com/smartlegionlab/clipassman/
 Author: A.A. Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/clipassman/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/clipassman/releases
@@ -28,14 +28,26 @@
 Requires-Dist: smartcliapp~=0.4.0
 Requires-Dist: smartpasslib~=0.4.2
 
 # clipassman
 
 ***
 
+***
+
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/clipassman)](https://github.com/smartlegionlab/clipassman/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/clipassman?label=pypi%20downloads)](https://pypi.org/project/clipassman/)
+![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/clipassman)
+[![PyPI](https://img.shields.io/pypi/v/clipassman)](https://pypi.org/project/clipassman)
+[![GitHub](https://img.shields.io/github/license/smartlegionlab/clipassman)](https://github.com/smartlegionlab/clipassman/blob/master/LICENSE)
+[![PyPI - Format](https://img.shields.io/pypi/format/clipassman)](https://pypi.org/project/clipassman)
+
+
+***
+
 
 ## Short description:
 
 ___clipassman___ - Cross-platform console smart password generator and manager.
 
 - Passwords are not stored anywhere, neither in open nor in encrypted form, they are generated on the fly.
 - Complex passwords up to 1000 characters.
@@ -52,17 +64,25 @@
 
 - Linux: All.
 - Windows: 7/8/10.
 - Termux (Android).
 
 ***
 
+## Help:
+
+`pip install clipassman`
+
+`clipassman`
+
+***
+
 ## What is news:
 
-__clipassman v0.5.0__
+__clipassman v0.5.1__
 
 ***
 
 ## Images:
 
 ![LOGO](https://github.com/smartlegionlab/clipassman/raw/master/data/images/clipassman.png)
```

### Comparing `clipassman-0.5.0/clipassman/app.py` & `clipassman-0.5.1/clipassman/app.py`

 * *Files identical despite different names*

### Comparing `clipassman-0.5.0/clipassman/commander.py` & `clipassman-0.5.1/clipassman/commander.py`

 * *Files identical despite different names*

### Comparing `clipassman-0.5.0/clipassman/manager.py` & `clipassman-0.5.1/clipassman/manager.py`

 * *Files identical despite different names*

### Comparing `clipassman-0.5.0/clipassman/passman.py` & `clipassman-0.5.1/clipassman/passman.py`

 * *Files identical despite different names*

### Comparing `clipassman-0.5.0/clipassman.egg-info/PKG-INFO` & `clipassman-0.5.1/clipassman.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipassman
-Version: 0.5.0
+Version: 0.5.1
 Summary: Cross-platform console smart password generator and manager.
 Home-page: https://github.com/smartlegionlab/clipassman/
 Author: A.A. Suvorov
 Author-email: smartlegiondev@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://github.com/smartlegionlab/clipassman/blob/master/README.md
 Project-URL: Release notes, https://github.com/smartlegionlab/clipassman/releases
@@ -28,14 +28,26 @@
 Requires-Dist: smartcliapp~=0.4.0
 Requires-Dist: smartpasslib~=0.4.2
 
 # clipassman
 
 ***
 
+***
+
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/smartlegionlab/clipassman)](https://github.com/smartlegionlab/clipassman/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/clipassman?label=pypi%20downloads)](https://pypi.org/project/clipassman/)
+![GitHub top language](https://img.shields.io/github/languages/top/smartlegionlab/clipassman)
+[![PyPI](https://img.shields.io/pypi/v/clipassman)](https://pypi.org/project/clipassman)
+[![GitHub](https://img.shields.io/github/license/smartlegionlab/clipassman)](https://github.com/smartlegionlab/clipassman/blob/master/LICENSE)
+[![PyPI - Format](https://img.shields.io/pypi/format/clipassman)](https://pypi.org/project/clipassman)
+
+
+***
+
 
 ## Short description:
 
 ___clipassman___ - Cross-platform console smart password generator and manager.
 
 - Passwords are not stored anywhere, neither in open nor in encrypted form, they are generated on the fly.
 - Complex passwords up to 1000 characters.
@@ -52,17 +64,25 @@
 
 - Linux: All.
 - Windows: 7/8/10.
 - Termux (Android).
 
 ***
 
+## Help:
+
+`pip install clipassman`
+
+`clipassman`
+
+***
+
 ## What is news:
 
-__clipassman v0.5.0__
+__clipassman v0.5.1__
 
 ***
 
 ## Images:
 
 ![LOGO](https://github.com/smartlegionlab/clipassman/raw/master/data/images/clipassman.png)
```

### Comparing `clipassman-0.5.0/setup.cfg` & `clipassman-0.5.1/setup.cfg`

 * *Files identical despite different names*

