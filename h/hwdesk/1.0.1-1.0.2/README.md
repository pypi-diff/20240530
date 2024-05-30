# Comparing `tmp/hwdesk-1.0.1.tar.gz` & `tmp/hwdesk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwdesk-1.0.1.tar", last modified: Wed May 29 18:40:22 2024, max compression
+gzip compressed data, was "hwdesk-1.0.2.tar", last modified: Wed May 29 18:47:46 2024, max compression
```

## Comparing `hwdesk-1.0.1.tar` & `hwdesk-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 18:40:16.000000 hwdesk-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 18:40:16.000000 hwdesk-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:40:22.812915 hwdesk-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 18:40:16.000000 hwdesk-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk/camera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/ms2109.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/ms2130.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/camera/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk/controls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/controls/ch9329.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/controls/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:16.000000 hwdesk-1.0.1/hwdesk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:40:22.812915 hwdesk-1.0.1/hwdesk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 18:40:22.000000 hwdesk-1.0.1/hwdesk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-29 18:40:16.000000 hwdesk-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:40:22.812915 hwdesk-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 18:47:42.000000 hwdesk-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-29 18:47:42.000000 hwdesk-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:47:46.360427 hwdesk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 18:47:42.000000 hwdesk-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/ms2109.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/ms2130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/camera/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk/controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/controls/ch9329.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/controls/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:42.000000 hwdesk-1.0.2/hwdesk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:47:46.360427 hwdesk-1.0.2/hwdesk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 18:47:46.000000 hwdesk-1.0.2/hwdesk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-29 18:47:42.000000 hwdesk-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:47:46.360427 hwdesk-1.0.2/setup.cfg
```

### Comparing `hwdesk-1.0.1/LICENSE` & `hwdesk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.1/PKG-INFO` & `hwdesk-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdesk
-Version: 1.0.1
+Version: 1.0.2
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `hwdesk-1.0.1/hwdesk/__main__.py` & `hwdesk-1.0.2/hwdesk/__main__.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.1/hwdesk/camera/base.py` & `hwdesk-1.0.2/hwdesk/camera/base.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.1/hwdesk/camera/prompt.py` & `hwdesk-1.0.2/hwdesk/camera/prompt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from tkinter.messagebox import showerror  # type:ignore
 from tkinter.simpledialog import askinteger
 
 from opencv_cam_idx.finder import find_cameras
 
 
 def ask_camera_idx() -> tuple[int, str]:
-    prompt = ""
-    prompt += "Please enter the index of camera you want to access: \n"
+    prompt: list[str] = []
+    prompt.append("Please enter the index of camera you want to access:")
     valid_idx: dict[int, tuple[int, str]] = {}
     for c in find_cameras():
         if "pid_2130" in c.device_path:
             valid_idx[c.idx] = c.idx, c.friendly_name
-            prompt += f"Index={c.idx}, Name={c.friendly_name}"
+            prompt.append(f"Index={c.idx}, Name={c.friendly_name}")
     if valid_idx == {}:
         showerror("HwDesk Error", "No MS2130 devices found.")
         return -1, ""
-    idx = askinteger("Camera Selection", prompt, initialvalue=0, minvalue=0)
+    idx = askinteger(
+        "Camera Selection", "\n".join(prompt), initialvalue=0, minvalue=0
+    )
     if idx not in valid_idx:
         showerror("HwDesk Error", "Please select a valid camera index.")
         return -1, ""
     return valid_idx[idx]
```

### Comparing `hwdesk-1.0.1/hwdesk/controls/ch9329.py` & `hwdesk-1.0.2/hwdesk/controls/ch9329.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.1/hwdesk/controls/prompt.py` & `hwdesk-1.0.2/hwdesk/controls/prompt.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 import serial.serialutil
 import serial.tools.list_ports
 from ch9329.config import get_serial_number
 from serial import Serial
 
 
 def ask_ch9329_port():
-    prompt = ""
-    prompt += "Please enter the index of CH9329 you want to access: \n"
+    prompt: list[str] = []
+    prompt.append("Please enter the index of CH9329 you want to access:")
     valid_ports: list[str] = []
     for i in serial.tools.list_ports.comports():
         try:
             if i.vid == 6790 and i.pid == 29987:
                 ser = Serial(i.name, 9600, timeout=0.05)
                 serial_number = get_serial_number(ser)
-                prompt += f"Port={i.name}, Serial={serial_number}"
+                prompt.append(f"Port={i.name}, Serial={serial_number}")
                 valid_ports.append(i.name)
         except serial.serialutil.SerialException:
             pass
     if valid_ports == []:
         showerror("HwDesk Error", "No CH9329 devices found.")
         return ""
-    port = askstring("CH9329 Selection", prompt, initialvalue=valid_ports[0])
+    port = askstring(
+        "CH9329 Selection", "\n".join(prompt), initialvalue=valid_ports[0]
+    )
     if port not in valid_ports:
         showerror("HwDesk Error", "Please select a valid CH9329 port.")
         return ""
     return port
```

### Comparing `hwdesk-1.0.1/hwdesk/gui.py` & `hwdesk-1.0.2/hwdesk/gui.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.1/hwdesk/logger.py` & `hwdesk-1.0.2/hwdesk/logger.py`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.1/hwdesk.egg-info/PKG-INFO` & `hwdesk-1.0.2/hwdesk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwdesk
-Version: 1.0.1
+Version: 1.0.2
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `hwdesk-1.0.1/hwdesk.egg-info/SOURCES.txt` & `hwdesk-1.0.2/hwdesk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hwdesk-1.0.1/pyproject.toml` & `hwdesk-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hwdesk"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
     "ch9329==1.1.2",
     "opencv-cam-idx==1.0.1",
     "opencv-python==4.9.0.80",
     "pydantic==2.6.4",
     "pillow==10.3.0",
 ]
```

