# Comparing `tmp/ch9329-1.1.2.tar.gz` & `tmp/ch9329-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.1.2.tar", last modified: Mon May 27 09:21:29 2024, max compression
+gzip compressed data, was "ch9329-1.2.0.tar", last modified: Thu May 30 14:11:08 2024, max compression
```

## Comparing `ch9329-1.1.2.tar` & `ch9329-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:28.999347 ch9329-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-27 09:21:24.000000 ch9329-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 09:21:24.000000 ch9329-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-27 09:21:28.999347 ch9329-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-27 09:21:24.000000 ch9329-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:28.999347 ch9329-1.1.2/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-27 09:21:24.000000 ch9329-1.1.2/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:21:28.999347 ch9329-1.1.2/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 09:21:28.000000 ch9329-1.1.2/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-27 09:21:24.000000 ch9329-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:21:28.999347 ch9329-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:08.961393 ch9329-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 14:11:03.000000 ch9329-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 14:11:03.000000 ch9329-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 14:11:08.961393 ch9329-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 14:11:03.000000 ch9329-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:08.961393 ch9329-1.2.0/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-30 14:11:03.000000 ch9329-1.2.0/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:11:08.961393 ch9329-1.2.0/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 14:11:08.000000 ch9329-1.2.0/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 14:11:03.000000 ch9329-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:11:08.961393 ch9329-1.2.0/setup.cfg
```

### Comparing `ch9329-1.1.2/LICENSE` & `ch9329-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.2/PKG-INFO` & `ch9329-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.1.2
+Version: 1.2.0
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -50,17 +50,17 @@
 
 from ch9329 import keyboard
 from ch9329 import mouse
 from ch9329.config import get_manufacturer
 from ch9329.config import get_product
 from ch9329.config import get_serial_number
 
-ser = Serial("COM3", 9600, timeout=1)
+ser = Serial("COM3", 9600, timeout=0.05)
 
-keyboard.press_and_release(ser, "a", modifier="ctrl")
+keyboard.press_and_release(ser, "a", modifiers=["ctrl"])
 keyboard.write(ser, "Hello World\n")
 keyboard.write(ser, "abcdefghijklmnopqrstuvwxyz\n")
 keyboard.write(ser, "ABCDEFGHIJKLMNOPQRSTUVWXYZ\n")
 keyboard.write(ser, "0123456789\n")
 keyboard.write(ser, "!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~\n")
 
 mouse.move(ser, x=500, y=500)
```

### Comparing `ch9329-1.1.2/README.md` & `ch9329-1.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 from ch9329 import keyboard
 from ch9329 import mouse
 from ch9329.config import get_manufacturer
 from ch9329.config import get_product
 from ch9329.config import get_serial_number
 
-ser = Serial("COM3", 9600, timeout=1)
+ser = Serial("COM3", 9600, timeout=0.05)
 
-keyboard.press_and_release(ser, "a", modifier="ctrl")
+keyboard.press_and_release(ser, "a", modifiers=["ctrl"])
 keyboard.write(ser, "Hello World\n")
 keyboard.write(ser, "abcdefghijklmnopqrstuvwxyz\n")
 keyboard.write(ser, "ABCDEFGHIJKLMNOPQRSTUVWXYZ\n")
 keyboard.write(ser, "0123456789\n")
 keyboard.write(ser, "!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~\n")
 
 mouse.move(ser, x=500, y=500)
```

### Comparing `ch9329-1.1.2/ch9329/config.py` & `ch9329-1.2.0/ch9329/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     data = ser.readall()
     if not data:
         return ""
     return data
 
 
 def get_usb_string(ser: Serial, descriptor: USBStringDescriptor):
+    ser.readall()  # clear old packets
     packet = get_packet(
         HEAD,
         ADDR,
         CMD_GET_USB_STRING,
         LEN_GET_USB_STRING,
         descriptor.value,
     )
```

### Comparing `ch9329-1.1.2/ch9329/mouse.py` & `ch9329-1.2.0/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.2/ch9329/utils.py` & `ch9329-1.2.0/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.1.2/ch9329.egg-info/PKG-INFO` & `ch9329-1.2.0/ch9329.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.1.2
+Version: 1.2.0
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -50,17 +50,17 @@
 
 from ch9329 import keyboard
 from ch9329 import mouse
 from ch9329.config import get_manufacturer
 from ch9329.config import get_product
 from ch9329.config import get_serial_number
 
-ser = Serial("COM3", 9600, timeout=1)
+ser = Serial("COM3", 9600, timeout=0.05)
 
-keyboard.press_and_release(ser, "a", modifier="ctrl")
+keyboard.press_and_release(ser, "a", modifiers=["ctrl"])
 keyboard.write(ser, "Hello World\n")
 keyboard.write(ser, "abcdefghijklmnopqrstuvwxyz\n")
 keyboard.write(ser, "ABCDEFGHIJKLMNOPQRSTUVWXYZ\n")
 keyboard.write(ser, "0123456789\n")
 keyboard.write(ser, "!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~\n")
 
 mouse.move(ser, x=500, y=500)
```

### Comparing `ch9329-1.1.2/pyproject.toml` & `ch9329-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.1.2"
+version = "1.2.0"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

