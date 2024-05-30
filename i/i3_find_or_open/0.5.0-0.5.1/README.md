# Comparing `tmp/i3_find_or_open-0.5.0.tar.gz` & `tmp/i3_find_or_open-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i3_find_or_open-0.5.0.tar", max compression
+gzip compressed data, was "i3_find_or_open-0.5.1.tar", max compression
```

## Comparing `i3_find_or_open-0.5.0.tar` & `i3_find_or_open-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-11-21 13:29:02.922803 i3_find_or_open-0.5.0/LICENSE
--rw-r--r--   0        0        0     2415 2023-11-24 10:57:55.066202 i3_find_or_open-0.5.0/README.md
--rwxr-xr-x   0        0        0     2647 2023-11-24 11:08:20.556509 i3_find_or_open-0.5.0/i3_find_or_open/main.py
--rw-r--r--   0        0        0      543 2023-11-24 11:10:00.267545 i3_find_or_open-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 i3_find_or_open-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-01 21:50:10.472238 i3_find_or_open-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2415 2023-11-23 22:50:53.458219 i3_find_or_open-0.5.1/README.md
+-rwxr-xr-x   0        0        0     2634 2024-05-30 13:00:17.713149 i3_find_or_open-0.5.1/i3_find_or_open/main.py
+-rw-r--r--   0        0        0      543 2024-05-30 13:12:44.813701 i3_find_or_open-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 i3_find_or_open-0.5.1/PKG-INFO
```

### Comparing `i3_find_or_open-0.5.0/LICENSE` & `i3_find_or_open-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `i3_find_or_open-0.5.0/README.md` & `i3_find_or_open-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `i3_find_or_open-0.5.0/i3_find_or_open/main.py` & `i3_find_or_open-0.5.1/i3_find_or_open/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """A module that helps you bind keys to find and display, or open a window in i3wm."""
-#!/bin/python
+
 import argparse
 import importlib.metadata
 import re
 import subprocess as sp
 
 import i3ipc
```

### Comparing `i3_find_or_open-0.5.0/pyproject.toml` & `i3_find_or_open-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "i3_find_or_open"
-version = "0.5.0"
+version = "0.5.1"
 license = "GPL-3.0-only"
 description = "A command-line utility that helps you bind keys to find and display a window, or open it if there is no instance running in i3wm."
 authors = ["Hector Brown <hectorjbrown@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `i3_find_or_open-0.5.0/PKG-INFO` & `i3_find_or_open-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3_find_or_open
-Version: 0.5.0
+Version: 0.5.1
 Summary: A command-line utility that helps you bind keys to find and display a window, or open it if there is no instance running in i3wm.
 License: GPL-3.0-only
 Author: Hector Brown
 Author-email: hectorjbrown@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

