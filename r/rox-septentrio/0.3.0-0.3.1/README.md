# Comparing `tmp/rox_septentrio-0.3.0.tar.gz` & `tmp/rox_septentrio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rox_septentrio-0.3.0.tar", last modified: Fri May 24 12:34:18 2024, max compression
+gzip compressed data, was "rox_septentrio-0.3.1.tar", last modified: Wed May 29 09:33:42 2024, max compression
```

## Comparing `rox_septentrio-0.3.0.tar` & `rox_septentrio-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.322800 rox_septentrio-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2994 2024-05-24 12:34:18.322800 rox_septentrio-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 12:34:18.322800 rox_septentrio-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.317800 rox_septentrio-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.319800 rox_septentrio-0.3.0/src/rox_septentrio/
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/converters.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/gps_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/nmea.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/src/rox_septentrio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.321800 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2994 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       87 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-24 12:34:18.000000 rox_septentrio-0.3.0/src/rox_septentrio.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:34:18.321800 rox_septentrio-0.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/tests/test_converter.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/tests/test_messages.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-24 12:33:55.000000 rox_septentrio-0.3.0/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:33:42.077894 rox_septentrio-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     3192 2024-05-29 09:33:42.077894 rox_septentrio-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 09:33:42.078894 rox_septentrio-0.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:33:42.072894 rox_septentrio-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:33:42.075893 rox_septentrio-0.3.1/src/rox_septentrio/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/converters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/gps_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/nmea.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/src/rox_septentrio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:33:42.077894 rox_septentrio-0.3.1/src/rox_septentrio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3192 2024-05-29 09:33:42.000000 rox_septentrio-0.3.1/src/rox_septentrio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2024-05-29 09:33:42.000000 rox_septentrio-0.3.1/src/rox_septentrio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 09:33:42.000000 rox_septentrio-0.3.1/src/rox_septentrio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-29 09:33:42.000000 rox_septentrio-0.3.1/src/rox_septentrio.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2024-05-29 09:33:42.000000 rox_septentrio-0.3.1/src/rox_septentrio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-29 09:33:42.000000 rox_septentrio-0.3.1/src/rox_septentrio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:33:42.077894 rox_septentrio-0.3.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/tests/test_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/tests/test_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-29 09:33:19.000000 rox_septentrio-0.3.1/tests/test_smoke.py
```

### Comparing `rox_septentrio-0.3.0/LICENCE` & `rox_septentrio-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.3.0/PKG-INFO` & `rox_septentrio-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox-septentrio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Driver for Septentrio GPS, posting messages to mqtt
 Author-email: Jev Kuznetsov <jev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/roxautomation/components/septentrio-gps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -51,14 +51,19 @@
 - **MQTT_DIRECTION_TOPIC**: MQTT topic for GPS directions (default: `"/gps/direction"`).
 
 ### GPS
 - **GPS_PORT**: Serial port for GPS (default: `"/dev/gps_nmea"`).
 - **GPS_BAUD**: Baud rate for GPS serial communication (default: `115200`).
 - **GPS_REF**: gps reference point, provide lat,lon, example: `GPS_REF="51.123,6.456"`
 
+## Precision
+ - **DIGITS_POSITION** : meter position accuracy, defaults to 3
+ - **DIGITS_LATLON** : digits latitude and longitude, defaults to 8
+ - **DIGITS_ANGLE** : angle accuracy, defaults to 4
+
 **Example launch with custom parameters**
 
     docker run \
     -e MQTT_HOST=192.168.1.100 \
     -e MQTT_PORT=8883 \
     -e GPS_PORT=/dev/ttyS0 \
     registry.gitlab.com/roxautomation/components/septentrio-gps:latest
```

### Comparing `rox_septentrio-0.3.0/README.md` & `rox_septentrio-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 - **MQTT_DIRECTION_TOPIC**: MQTT topic for GPS directions (default: `"/gps/direction"`).
 
 ### GPS
 - **GPS_PORT**: Serial port for GPS (default: `"/dev/gps_nmea"`).
 - **GPS_BAUD**: Baud rate for GPS serial communication (default: `115200`).
 - **GPS_REF**: gps reference point, provide lat,lon, example: `GPS_REF="51.123,6.456"`
 
+## Precision
+ - **DIGITS_POSITION** : meter position accuracy, defaults to 3
+ - **DIGITS_LATLON** : digits latitude and longitude, defaults to 8
+ - **DIGITS_ANGLE** : angle accuracy, defaults to 4
+
 **Example launch with custom parameters**
 
     docker run \
     -e MQTT_HOST=192.168.1.100 \
     -e MQTT_PORT=8883 \
     -e GPS_PORT=/dev/ttyS0 \
     registry.gitlab.com/roxautomation/components/septentrio-gps:latest
```

### Comparing `rox_septentrio-0.3.0/pyproject.toml` & `rox_septentrio-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #-----------------pyproject.toml configuration----------------
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rox-septentrio"
-version = "0.3.0"
+version = "0.3.1"
 description = "Driver for Septentrio GPS, posting messages to mqtt"
 authors = [
     {name = "Jev Kuznetsov", email = "jev@roxautomation.com"},
 ]
 license = {text = "MIT"}
 readme = "README.md"
 classifiers = [
```

### Comparing `rox_septentrio-0.3.0/src/rox_septentrio/config.py` & `rox_septentrio-0.3.1/src/rox_septentrio/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,7 +23,17 @@
 class GpsConfig(BaseSettings):
     """gps config"""
 
     model_config = SettingsConfigDict(env_prefix="gps_")
 
     port: str = "/dev/gps_nmea"
     baud: int = 115_200
+
+
+class PrecisionConfig(BaseSettings):
+    """precision settings"""
+
+    model_config = SettingsConfigDict(env_prefix="digits_")
+
+    position: int = 3
+    latlon: int = 8
+    angle: int = 4
```

### Comparing `rox_septentrio-0.3.0/src/rox_septentrio/converters.py` & `rox_septentrio-0.3.1/src/rox_septentrio/converters.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.3.0/src/rox_septentrio/gps_node.py` & `rox_septentrio-0.3.1/src/rox_septentrio/gps_node.py`

 * *Files identical despite different names*

### Comparing `rox_septentrio-0.3.0/src/rox_septentrio/nmea.py` & `rox_septentrio-0.3.1/src/rox_septentrio/nmea.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 
 Copyright (c) 2024 ROX Automation - Jev Kuznetsov
 """
 
 import time
 from typing import NamedTuple
 import pynmea2
+from rox_septentrio.config import PrecisionConfig
 from rox_septentrio.converters import GpsConverter, heading_to_theta
 
+
+pr_cfg = PrecisionConfig()
+
 gps_converter = GpsConverter()
 
 
 class SSN(pynmea2.ProprietarySentence):
     """proprietary message definition"""
 
     # docs: https://geodesy.noaa.gov/pub/abilich/antcalCorbin/Firmware%20User%20Manual.pdf
@@ -69,30 +73,30 @@
 def parse(txt: str) -> PositionData | HeadingData | None:
     """parse nmea message"""
 
     if txt.startswith("$PSSN"):
         msg = pynmea2.parse(txt)
 
         return HeadingData(
-            heading=round(msg.heading, 3),  # type: ignore
-            heading_stdev=msg.heading_stdev,  # type: ignore
-            theta=heading_to_theta(msg.heading),  # type: ignore
+            heading=round(msg.heading, pr_cfg.angle),  # type: ignore
+            heading_stdev=round(msg.heading_stdev, pr_cfg.angle),  # type: ignore
+            theta=round(heading_to_theta(msg.heading), pr_cfg.angle),  # type: ignore
             ts=timestamp(),
         )
 
     elif txt.startswith("$GPGGA"):
         msg = pynmea2.parse(txt)
 
         x, y = gps_converter.latlon_to_enu((msg.latitude, msg.longitude))  # type: ignore
 
         return PositionData(
-            lat=msg.latitude,  # type: ignore
-            lon=msg.longitude,  # type: ignore
-            x=round(x, 3),
-            y=round(y, 3),
+            lat=round(msg.latitude, pr_cfg.latlon),  # type: ignore
+            lon=round(msg.longitude, pr_cfg.latlon),  # type: ignore
+            x=round(x, pr_cfg.position),
+            y=round(y, pr_cfg.position),
             gps_qual=msg.gps_qual,  # type: ignore
             time=msg.timestamp.strftime("%H:%M:%S.%f"),  # type: ignore
             ts=timestamp(),
         )
 
     else:
         return None
```

### Comparing `rox_septentrio-0.3.0/src/rox_septentrio.egg-info/PKG-INFO` & `rox_septentrio-0.3.1/src/rox_septentrio.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rox-septentrio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Driver for Septentrio GPS, posting messages to mqtt
 Author-email: Jev Kuznetsov <jev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/roxautomation/components/septentrio-gps
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -51,14 +51,19 @@
 - **MQTT_DIRECTION_TOPIC**: MQTT topic for GPS directions (default: `"/gps/direction"`).
 
 ### GPS
 - **GPS_PORT**: Serial port for GPS (default: `"/dev/gps_nmea"`).
 - **GPS_BAUD**: Baud rate for GPS serial communication (default: `115200`).
 - **GPS_REF**: gps reference point, provide lat,lon, example: `GPS_REF="51.123,6.456"`
 
+## Precision
+ - **DIGITS_POSITION** : meter position accuracy, defaults to 3
+ - **DIGITS_LATLON** : digits latitude and longitude, defaults to 8
+ - **DIGITS_ANGLE** : angle accuracy, defaults to 4
+
 **Example launch with custom parameters**
 
     docker run \
     -e MQTT_HOST=192.168.1.100 \
     -e MQTT_PORT=8883 \
     -e GPS_PORT=/dev/ttyS0 \
     registry.gitlab.com/roxautomation/components/septentrio-gps:latest
```

### Comparing `rox_septentrio-0.3.0/src/rox_septentrio.egg-info/SOURCES.txt` & `rox_septentrio-0.3.1/src/rox_septentrio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

