# Comparing `tmp/youless_api-1.1.1.tar.gz` & `tmp/youless_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youless_api-1.1.1.tar", last modified: Mon May 13 07:13:24 2024, max compression
+gzip compressed data, was "youless_api-2.0.0.tar", last modified: Thu May 30 15:15:08 2024, max compression
```

## Comparing `youless_api-1.1.1.tar` & `youless_api-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-13 07:13:24.811150 youless_api-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-13 07:13:20.000000 youless_api-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:13:24.811150 youless_api-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 07:13:20.000000 youless_api-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api/
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api/device/
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/LS110.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/LS120.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/LS120_pv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api/test/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_LS110.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_LS120.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_LS120_pv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/test/test_youless_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-13 07:13:20.000000 youless_api-1.1.1/youless_api/youless_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:13:24.811150 youless_api-1.1.1/youless_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 07:13:24.000000 youless_api-1.1.1/youless_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:15:08.311471 youless_api-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-30 15:15:08.311471 youless_api-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-30 15:15:04.000000 youless_api-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:15:08.311471 youless_api-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-30 15:15:04.000000 youless_api-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:15:08.307470 youless_api-2.0.0/youless_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:15:08.311471 youless_api-2.0.0/youless_api/device/
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:15:08.311471 youless_api-2.0.0/youless_api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:15:08.311471 youless_api-2.0.0/youless_api/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/test/test_gateway_enelogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/test/test_gateway_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/test/test_youless_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-30 15:15:04.000000 youless_api-2.0.0/youless_api/youless_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:15:08.311471 youless_api-2.0.0/youless_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-30 15:15:08.000000 youless_api-2.0.0/youless_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-30 15:15:08.000000 youless_api-2.0.0/youless_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:15:08.000000 youless_api-2.0.0/youless_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:15:08.000000 youless_api-2.0.0/youless_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 15:15:08.000000 youless_api-2.0.0/youless_api.egg-info/top_level.txt
```

### Comparing `youless_api-1.1.1/PKG-INFO` & `youless_api-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youless_api
-Version: 1.1.1
+Version: 2.0.0
 Summary: A bridge for python to the YouLess sensor
 Home-page: https://github.com/gjong/youless-python-bridge
 Author: G. Jongerius
 License: MIT
 Description-Content-Type: text/markdown
 
 # YouLess Python Data Bridge
```

### Comparing `youless_api-1.1.1/README.md` & `youless_api-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `youless_api-1.1.1/youless_api/test/__init__.py` & `youless_api-2.0.0/youless_api/test/__init__.py`

 * *Files identical despite different names*

### Comparing `youless_api-1.1.1/youless_api/youless_sensor.py` & `youless_api-2.0.0/youless_api/youless_sensor.py`

 * *Files identical despite different names*

### Comparing `youless_api-1.1.1/youless_api.egg-info/PKG-INFO` & `youless_api-2.0.0/youless_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youless_api
-Version: 1.1.1
+Version: 2.0.0
 Summary: A bridge for python to the YouLess sensor
 Home-page: https://github.com/gjong/youless-python-bridge
 Author: G. Jongerius
 License: MIT
 Description-Content-Type: text/markdown
 
 # YouLess Python Data Bridge
```

