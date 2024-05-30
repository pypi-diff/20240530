# Comparing `tmp/hwdesk-1.0.2.tar.gz` & `tmp/hwdesk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwdesk-1.0.2.tar", last modified: Wed May 29 18:47:46 2024, max compression
+gzip compressed data, was "hwdesk-1.0.3.tar", last modified: Thu May 30 14:57:57 2024, max compression
```

## Comparing `hwdesk-1.0.2.tar` & `hwdesk-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 18:47:42.000000 hwdesk-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 18:47:42.000000 hwdesk-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:47:46.360427 hwdesk-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 18:47:42.000000 hwdesk-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk/camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/ms2109.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/ms2130.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk/controls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/controls/ch9329.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/controls/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-29 18:47:42.000000 hwdesk-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:47:46.360427 hwdesk-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:57.268453 hwdesk-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 14:57:50.000000 hwdesk-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 14:57:50.000000 hwdesk-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-30 14:57:57.268453 hwdesk-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 14:57:50.000000 hwdesk-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:57.264454 hwdesk-1.0.3/hwdesk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:57.268453 hwdesk-1.0.3/hwdesk/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/camera/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/camera/ms2109.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/camera/ms2130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/camera/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:57.268453 hwdesk-1.0.3/hwdesk/controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/controls/ch9329.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/controls/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:50.000000 hwdesk-1.0.3/hwdesk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:57.268453 hwdesk-1.0.3/hwdesk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-30 14:57:57.000000 hwdesk-1.0.3/hwdesk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-30 14:57:57.000000 hwdesk-1.0.3/hwdesk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:57:57.000000 hwdesk-1.0.3/hwdesk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 14:57:57.000000 hwdesk-1.0.3/hwdesk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-30 14:57:57.000000 hwdesk-1.0.3/hwdesk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 14:57:57.000000 hwdesk-1.0.3/hwdesk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-30 14:57:50.000000 hwdesk-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:57:57.268453 hwdesk-1.0.3/setup.cfg
```

### Comparing `hwdesk-1.0.2/LICENSE` & `hwdesk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.2/PKG-INFO` & `hwdesk-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdesk
-Version: 1.0.2
+Version: 1.0.3
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,19 +24,20 @@
         
 Project-URL: Homepage, https://github.com/sandbox-pokhara/hwdesk
 Project-URL: Issues, https://github.com/sandbox-pokhara/hwdesk/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ch9329==1.1.2
+Requires-Dist: ch9329==1.2.0
+Requires-Dist: keyboard==0.13.5
 Requires-Dist: opencv-cam-idx==1.0.1
 Requires-Dist: opencv-python==4.9.0.80
-Requires-Dist: pydantic==2.6.4
 Requires-Dist: pillow==10.3.0
+Requires-Dist: pydantic==2.6.4
 
 # hwdesk
 
 ## Installation
 
 You can install the package via pip:
 
@@ -59,12 +60,11 @@
 ```
 
 To exit the program, press `alt+f4` or `esc`.
 
 ## Limitations
 
 - Mouse Drag
-- Alt+Tab, Alt+F4, Win+R, etc
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `hwdesk-1.0.2/hwdesk/__main__.py` & `hwdesk-1.0.3/hwdesk/__main__.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.2/hwdesk/camera/base.py` & `hwdesk-1.0.3/hwdesk/camera/base.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.2/hwdesk/camera/prompt.py` & `hwdesk-1.0.3/hwdesk/camera/prompt.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.2/hwdesk/controls/ch9329.py` & `hwdesk-1.0.3/hwdesk/controls/ch9329.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import time
 
 from ch9329 import keyboard
 from ch9329 import mouse
+from ch9329.keyboard import Modifier
 from serial import Serial
 
-MODIFIERS = {
-    0x0001: "shift",
-    0x0004: "ctrl",
-    0x0008: "alt_left",  # does not work
-    0x0080: "alt_right",  # does not work
-    0x20000: "alt",
-}
-
 KEY_MAP = {
+    "left windows": "win",
+    "right windows": "win",
+    "left shift": "shift",
+    "right shift": "shift",
+    "left ctrl": "ctrl",
+    "right ctrl": "ctrl",
     "space": " ",
+    "decimal": ".",
     "period": ".",
     "backspace": "backspace",
-    "enter": "\r",
+    "enter": "\n",
     "escape": "\x1b",
     "quotedbl": '"',
     "quote": "'",
     "grave": "`",
     "minus": "-",
     "equal": "=",
     "asciitilde": "~",
@@ -34,14 +34,15 @@
     "asterisk": "*",
     "parenleft": "(",
     "parenright": ")",
     "underscore": "_",
     "plus": "+",
     "tab": "\t",
     "caps_lock": "caps_lock",
+    "caps lock": "caps_lock",
     "bracketleft": "[",
     "bracketright": "]",
     "braceleft": "{",
     "braceright": "}",
     "semicolon": ";",
     "colon": ":",
     "apostrophe": "'",
@@ -51,14 +52,33 @@
     "less": "<",
     "greater": ">",
     "slash": "/",
     "question": "?",
     "return": "\n",
     "prior": "page_up",
     "next": "page_down",
+    "page up": "page_up",
+    "page down": "page_down",
+    "print screen": "print_screen",
+    "scroll lock": "scroll_lock",
+}
+
+MODIFIER_MAP: dict[str, Modifier] = {
+    "windows": "win",
+    "left windows": "win_left",
+    "right windows": "win_right",
+    "alt": "alt",
+    "left alt": "alt_left",
+    "right alt": "alt_right",
+    "ctrl": "ctrl",
+    "left ctrl": "ctrl_left",
+    "right shift": "shift_right",
+    "shift": "shift",
+    "left shift": "shift_left",
+    "right ctrl": "ctrl_right",
 }
 
 
 class CH9329:
     def __init__(self, port: str) -> None:
         self.port = port
         self.serial = Serial(port, 9600, timeout=0.05)
@@ -78,24 +98,20 @@
     def click(self, button: str = "left") -> None:
         mouse.press(self.serial, button)
         mouse.release(self.serial)
 
     def wheel(self, delta: int = 1) -> None:
         mouse.wheel(self.serial, delta)
 
-    def press(self, key: str, state: int) -> None:
-        """
-        :param key: keysym attribute of tkinter key event
-        :param state: state attribute of tkinter key event
-        """
-        modifiers = [v for k, v in MODIFIERS.items() if k & state]
-        modifier = modifiers[0] if modifiers else ""
+    def press(self, key: str, modifiers: list[Modifier] = []) -> None:
         key = key.lower()
         key = KEY_MAP.get(key, key)
-        keyboard.press(self.serial, key, modifier)
+        keyboard.press(self.serial, key, modifiers)
 
     def release(self) -> None:
         keyboard.release(self.serial)
 
-    def press_and_release(self, key: str, modifier: str = "") -> None:
-        keyboard.press(self.serial, key, modifier)
+    def press_and_release(
+        self, key: str, modifiers: list[Modifier] = []
+    ) -> None:
+        keyboard.press(self.serial, key, modifiers)
         keyboard.release(self.serial)
```

### Comparing `hwdesk-1.0.2/hwdesk/controls/prompt.py` & `hwdesk-1.0.3/hwdesk/controls/prompt.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.2/hwdesk/logger.py` & `hwdesk-1.0.3/hwdesk/logger.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.2/hwdesk.egg-info/PKG-INFO` & `hwdesk-1.0.3/hwdesk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdesk
-Version: 1.0.2
+Version: 1.0.3
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,19 +24,20 @@
         
 Project-URL: Homepage, https://github.com/sandbox-pokhara/hwdesk
 Project-URL: Issues, https://github.com/sandbox-pokhara/hwdesk/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ch9329==1.1.2
+Requires-Dist: ch9329==1.2.0
+Requires-Dist: keyboard==0.13.5
 Requires-Dist: opencv-cam-idx==1.0.1
 Requires-Dist: opencv-python==4.9.0.80
-Requires-Dist: pydantic==2.6.4
 Requires-Dist: pillow==10.3.0
+Requires-Dist: pydantic==2.6.4
 
 # hwdesk
 
 ## Installation
 
 You can install the package via pip:
 
@@ -59,12 +60,11 @@
 ```
 
 To exit the program, press `alt+f4` or `esc`.
 
 ## Limitations
 
 - Mouse Drag
-- Alt+Tab, Alt+F4, Win+R, etc
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `hwdesk-1.0.2/hwdesk.egg-info/SOURCES.txt` & `hwdesk-1.0.3/hwdesk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.2/pyproject.toml` & `hwdesk-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hwdesk"
-version = "1.0.2"
+version = "1.0.3"
 dependencies = [
-    "ch9329==1.1.2",
+    "ch9329==1.2.0",
+    "keyboard==0.13.5",
     "opencv-cam-idx==1.0.1",
     "opencv-python==4.9.0.80",
-    "pydantic==2.6.4",
     "pillow==10.3.0",
+    "pydantic==2.6.4",
 ]
 requires-python = ">=3.11"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = ""
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

