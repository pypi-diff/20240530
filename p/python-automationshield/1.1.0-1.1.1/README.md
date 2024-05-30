# Comparing `tmp/python_automationshield-1.1.0.tar.gz` & `tmp/python_automationshield-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_automationshield-1.1.0.tar", max compression
+gzip compressed data, was "python_automationshield-1.1.1.tar", max compression
```

## Comparing `python_automationshield-1.1.0.tar` & `python_automationshield-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1079 2024-05-30 14:40:47.235680 python_automationshield-1.1.0/LICENSE
--rw-r--r--   0        0        0     4590 2024-05-30 14:40:47.235680 python_automationshield-1.1.0/README.md
--rw-r--r--   0        0        0      812 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      656 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/__init__.py
--rw-r--r--   0        0        0     4473 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/arduino.py
--rw-r--r--   0        0        0      113 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
--rw-r--r--   0        0        0      115 2024-05-30 14:40:47.237680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/floatshield/floatshield.ino
--rw-r--r--   0        0        0      418 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
--rw-r--r--   0        0        0      447 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
--rw-r--r--   0        0        0     2481 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
--rw-r--r--   0        0        0      986 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
--rw-r--r--   0        0        0      356 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
--rw-r--r--   0        0        0      367 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
--rw-r--r--   0        0        0      122 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
--rw-r--r--   0        0        0      269 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
--rw-r--r--   0        0        0      119 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
--rw-r--r--   0        0        0       73 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/controller/__init__.py
--rw-r--r--   0        0        0     9561 2024-05-30 14:40:47.238680 python_automationshield-1.1.0/src/automationshield/controller/controller.py
--rw-r--r--   0        0        0     1037 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/controller/reference.py
--rw-r--r--   0        0        0       52 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/exception.py
--rw-r--r--   0        0        0       67 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/plotting/__init__.py
--rw-r--r--   0        0        0     6523 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/plotting/live_plotter.py
--rw-r--r--   0        0        0     7716 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/plotting/plotter.py
--rw-r--r--   0        0        0      187 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/__init__.py
--rw-r--r--   0        0        0      840 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/_dummyshield.py
--rw-r--r--   0        0        0     1973 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/aeroshield.py
--rw-r--r--   0        0        0    11517 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/baseshield.py
--rw-r--r--   0        0        0     1189 2024-05-30 14:40:47.239680 python_automationshield-1.1.0/src/automationshield/shields/floatshield.py
--rw-r--r--   0        0        0     6620 2024-05-30 14:40:47.240680 python_automationshield-1.1.0/src/automationshield/shields/magnetoshield.py
--rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 python_automationshield-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-30 15:09:38.905321 python_automationshield-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4590 2024-05-30 15:09:38.905321 python_automationshield-1.1.1/README.md
+-rw-r--r--   0        0        0      783 2024-05-30 15:09:38.907321 python_automationshield-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      656 2024-05-30 15:09:38.907321 python_automationshield-1.1.1/src/automationshield/__init__.py
+-rw-r--r--   0        0        0     4473 2024-05-30 15:09:38.907321 python_automationshield-1.1.1/src/automationshield/arduino.py
+-rw-r--r--   0        0        0      113 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
+-rw-r--r--   0        0        0      115 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/floatshield/floatshield.ino
+-rw-r--r--   0        0        0      418 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
+-rw-r--r--   0        0        0      447 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
+-rw-r--r--   0        0        0     2481 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
+-rw-r--r--   0        0        0      986 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
+-rw-r--r--   0        0        0      356 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
+-rw-r--r--   0        0        0      367 2024-05-30 15:09:38.908321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
+-rw-r--r--   0        0        0      122 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
+-rw-r--r--   0        0        0      269 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
+-rw-r--r--   0        0        0      119 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
+-rw-r--r--   0        0        0       73 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/controller/__init__.py
+-rw-r--r--   0        0        0     9561 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/controller/controller.py
+-rw-r--r--   0        0        0     1037 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/controller/reference.py
+-rw-r--r--   0        0        0       52 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/exception.py
+-rw-r--r--   0        0        0       67 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/plotting/__init__.py
+-rw-r--r--   0        0        0     6523 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/plotting/live_plotter.py
+-rw-r--r--   0        0        0     7716 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/plotting/plotter.py
+-rw-r--r--   0        0        0      187 2024-05-30 15:09:38.909321 python_automationshield-1.1.1/src/automationshield/shields/__init__.py
+-rw-r--r--   0        0        0      840 2024-05-30 15:09:38.910321 python_automationshield-1.1.1/src/automationshield/shields/_dummyshield.py
+-rw-r--r--   0        0        0     1973 2024-05-30 15:09:38.910321 python_automationshield-1.1.1/src/automationshield/shields/aeroshield.py
+-rw-r--r--   0        0        0    11517 2024-05-30 15:09:38.910321 python_automationshield-1.1.1/src/automationshield/shields/baseshield.py
+-rw-r--r--   0        0        0     1189 2024-05-30 15:09:38.910321 python_automationshield-1.1.1/src/automationshield/shields/floatshield.py
+-rw-r--r--   0        0        0     6620 2024-05-30 15:09:38.910321 python_automationshield-1.1.1/src/automationshield/shields/magnetoshield.py
+-rw-r--r--   0        0        0     5444 1970-01-01 00:00:00.000000 python_automationshield-1.1.1/PKG-INFO
```

### Comparing `python_automationshield-1.1.0/LICENSE` & `python_automationshield-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/README.md` & `python_automationshield-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/pyproject.toml` & `python_automationshield-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-automationshield"
-version = "1.1.0"
+version = "1.1.1"
 description = "A Python interface to AutomationShield's Arduino shields"
 authors = ["Bert Van den Abbeele"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/mrtreasurer/python-automationshield"
 documentation = "https://python-automationshield.readthedocs.io"
 packages = [
@@ -19,13 +19,12 @@
 multiprocess = ">=0.70.16"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 sphinx-autoapi = ">=3.0.0"
 myst-nb = ">=1.0.0"
-sphinx-rtd-theme = ">=2.0.0"
 sphinx-copybutton = ">=0.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_automationshield-1.1.0/src/automationshield/__init__.py` & `python_automationshield-1.1.1/src/automationshield/__init__.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/arduino.py` & `python_automationshield-1.1.1/src/automationshield/arduino.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp` & `python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h` & `python_automationshield-1.1.1/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/controller/controller.py` & `python_automationshield-1.1.1/src/automationshield/controller/controller.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/controller/reference.py` & `python_automationshield-1.1.1/src/automationshield/controller/reference.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/plotting/live_plotter.py` & `python_automationshield-1.1.1/src/automationshield/plotting/live_plotter.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/plotting/plotter.py` & `python_automationshield-1.1.1/src/automationshield/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/shields/_dummyshield.py` & `python_automationshield-1.1.1/src/automationshield/shields/_dummyshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/shields/aeroshield.py` & `python_automationshield-1.1.1/src/automationshield/shields/aeroshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/shields/baseshield.py` & `python_automationshield-1.1.1/src/automationshield/shields/baseshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/shields/floatshield.py` & `python_automationshield-1.1.1/src/automationshield/shields/floatshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/src/automationshield/shields/magnetoshield.py` & `python_automationshield-1.1.1/src/automationshield/shields/magnetoshield.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-1.1.0/PKG-INFO` & `python_automationshield-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automationshield
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python interface to AutomationShield's Arduino shields
 Home-page: https://gitlab.com/mrtreasurer/python-automationshield
 License: MIT
 Author: Bert Van den Abbeele
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

