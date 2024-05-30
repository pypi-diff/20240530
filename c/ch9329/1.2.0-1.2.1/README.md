# Comparing `tmp/ch9329-1.2.0.tar.gz` & `tmp/ch9329-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.2.0.tar", last modified: Thu May 30 14:11:08 2024, max compression
+gzip compressed data, was "ch9329-1.2.1.tar", last modified: Thu May 30 16:21:58 2024, max compression
```

## Comparing `ch9329-1.2.0.tar` & `ch9329-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:08.961393 ch9329-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 14:11:03.000000 ch9329-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 14:11:03.000000 ch9329-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 14:11:08.961393 ch9329-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 14:11:03.000000 ch9329-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:08.961393 ch9329-1.2.0/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:08.961393 ch9329-1.2.0/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 14:11:03.000000 ch9329-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:11:08.961393 ch9329-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:58.886926 ch9329-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 16:21:54.000000 ch9329-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 16:21:54.000000 ch9329-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 16:21:58.886926 ch9329-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 16:21:54.000000 ch9329-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:58.886926 ch9329-1.2.1/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 16:21:54.000000 ch9329-1.2.1/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:21:58.886926 ch9329-1.2.1/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 16:21:58.000000 ch9329-1.2.1/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 16:21:58.000000 ch9329-1.2.1/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:21:58.000000 ch9329-1.2.1/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 16:21:58.000000 ch9329-1.2.1/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 16:21:58.000000 ch9329-1.2.1/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 16:21:54.000000 ch9329-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:21:58.886926 ch9329-1.2.1/setup.cfg
```

### Comparing `ch9329-1.2.0/LICENSE` & `ch9329-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.0/PKG-INFO` & `ch9329-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.2.0/README.md` & `ch9329-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.0/ch9329/config.py` & `ch9329-1.2.1/ch9329/config.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.0/ch9329/hid.py` & `ch9329-1.2.1/ch9329/hid.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.0/ch9329/keyboard.py` & `ch9329-1.2.1/ch9329/keyboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import time
+from random import uniform
 from typing import List
 from typing import Literal
 from typing import Tuple
 
 from serial import Serial
 
 from ch9329.exceptions import InvalidKey
@@ -95,20 +96,33 @@
 
 
 def release(ser: Serial) -> None:
     send(ser, ("", "", "", "", "", ""))
 
 
 def press_and_release(
-    ser: Serial, key: str, modifiers: List[Modifier] = []
+    ser: Serial,
+    key: str,
+    modifiers: List[Modifier] = [],
+    min_interval: float = 0.02,
+    max_interval: float = 0.05,
 ) -> None:
+    if key not in HID_MAPPING:
+        raise InvalidKey(key)
+    _, shift = HID_MAPPING[key]
+    if shift:
+        modifiers = modifiers.copy()
+        modifiers.append("shift")
     press(ser, key, modifiers)
+    time.sleep(uniform(min_interval, max_interval))
     release(ser)
 
 
-def write(ser: Serial, text: str, interval: float = 0.1) -> None:
+def write(
+    ser: Serial,
+    text: str,
+    min_interval: float = 0.02,
+    max_interval: float = 0.05,
+) -> None:
     for char in text:
-        if char not in HID_MAPPING:
-            raise InvalidKey(char)
-        _, shift = HID_MAPPING[char]
-        press_and_release(ser, char, ["shift"] if shift else [])
-        time.sleep(interval)
+        press_and_release(ser, char, [], min_interval, max_interval)
+        time.sleep(uniform(min_interval, max_interval))
```

### Comparing `ch9329-1.2.0/ch9329/mouse.py` & `ch9329-1.2.1/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.0/ch9329/utils.py` & `ch9329-1.2.1/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.2.0/ch9329.egg-info/PKG-INFO` & `ch9329-1.2.1/ch9329.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.2.0/pyproject.toml` & `ch9329-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.2.0"
+version = "1.2.1"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

