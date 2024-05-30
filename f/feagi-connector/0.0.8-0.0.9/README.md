# Comparing `tmp/feagi_connector-0.0.8.tar.gz` & `tmp/feagi_connector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feagi_connector-0.0.8.tar", last modified: Sun Apr 21 00:14:01 2024, max compression
+gzip compressed data, was "feagi_connector-0.0.9.tar", last modified: Tue Apr 23 00:26:10 2024, max compression
```

## Comparing `feagi_connector-0.0.8.tar` & `feagi_connector-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:14:01.174907 feagi_connector-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-21 00:14:01.174907 feagi_connector-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:14:01.174907 feagi_connector-0.0.8/feagi_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/PIL_retina.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/actuators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/feagi_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/pns_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    26080 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/retina.py
--rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:14:01.174907 feagi_connector-0.0.8/feagi_connector/sensorimotor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/sensorimotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/testing_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/feagi_connector/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 00:13:43.000000 feagi_connector-0.0.8/feagi_connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:14:01.174907 feagi_connector-0.0.8/feagi_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-21 00:14:01.000000 feagi_connector-0.0.8/feagi_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-21 00:14:01.000000 feagi_connector-0.0.8/feagi_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:14:01.000000 feagi_connector-0.0.8/feagi_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-21 00:14:01.000000 feagi_connector-0.0.8/feagi_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 00:14:01.000000 feagi_connector-0.0.8/feagi_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-21 00:13:42.000000 feagi_connector-0.0.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      784 2024-04-21 00:14:01.174907 feagi_connector-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:26:10.001754 feagi_connector-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-23 00:26:10.001754 feagi_connector-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:26:09.997754 feagi_connector-0.0.9/feagi_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/PIL_retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6091 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/actuators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/feagi_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20262 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/pns_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26080 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/retina.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:26:09.997754 feagi_connector-0.0.9/feagi_connector/sensorimotor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/sensorimotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/testing_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/feagi_connector/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 00:26:00.000000 feagi_connector-0.0.9/feagi_connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:26:10.001754 feagi_connector-0.0.9/feagi_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-23 00:26:09.000000 feagi_connector-0.0.9/feagi_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 00:26:09.000000 feagi_connector-0.0.9/feagi_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:26:09.000000 feagi_connector-0.0.9/feagi_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 00:26:09.000000 feagi_connector-0.0.9/feagi_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 00:26:09.000000 feagi_connector-0.0.9/feagi_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 00:25:59.000000 feagi_connector-0.0.9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      784 2024-04-23 00:26:10.001754 feagi_connector-0.0.9/setup.cfg
```

### Comparing `feagi_connector-0.0.8/LICENSE` & `feagi_connector-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/PKG-INFO` & `feagi_connector-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.8/README.md` & `feagi_connector-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/PIL_retina.py` & `feagi_connector-0.0.9/feagi_connector/PIL_retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/actuators.py` & `feagi_connector-0.0.9/feagi_connector/actuators.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/configuration.py` & `feagi_connector-0.0.9/feagi_connector/configuration.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/feagi_interface.py` & `feagi_connector-0.0.9/feagi_connector/feagi_interface.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/pns_gateway.py` & `feagi_connector-0.0.9/feagi_connector/pns_gateway.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/retina.py` & `feagi_connector-0.0.9/feagi_connector/retina.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/router.py` & `feagi_connector-0.0.9/feagi_connector/router.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/sensors.py` & `feagi_connector-0.0.9/feagi_connector/sensors.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/testing_mode.py` & `feagi_connector-0.0.9/feagi_connector/testing_mode.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector/trainer.py` & `feagi_connector-0.0.9/feagi_connector/trainer.py`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/feagi_connector.egg-info/PKG-INFO` & `feagi_connector-0.0.9/feagi_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feagi_connector
-Version: 0.0.8
+Version: 0.0.9
 Summary: Feagi agent to work with general and simulation robots
 Home-page: https://github.com/feagi/feagi-connector
 Author: Neuraville Inc.
 Author-email: info@feagi.org
 Project-URL: Bug Tracker, https://github.com/feagi/feagi/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `feagi_connector-0.0.8/feagi_connector.egg-info/SOURCES.txt` & `feagi_connector-0.0.9/feagi_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feagi_connector-0.0.8/setup.cfg` & `feagi_connector-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = feagi_connector
-version = 0.0.8
+version = 0.0.9
 author = Neuraville Inc.
 author_email = info@feagi.org
 description = Feagi agent to work with general and simulation robots
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/feagi/feagi-connector
 project_urls =
```

