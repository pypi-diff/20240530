# Comparing `tmp/aiocloudweather-2024.2.2.tar.gz` & `tmp/aiocloudweather-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocloudweather-2024.2.2.tar", last modified: Wed May 29 22:00:22 2024, max compression
+gzip compressed data, was "aiocloudweather-2024.5.0.tar", last modified: Thu May 30 20:37:36 2024, max compression
```

## Comparing `aiocloudweather-2024.2.2.tar` & `aiocloudweather-2024.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-29 22:00:22.881695 aiocloudweather-2024.2.2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11383 2024-05-20 09:40:32.000000 aiocloudweather-2024.2.2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      686 2024-05-29 22:00:22.881695 aiocloudweather-2024.2.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      119 2024-05-20 09:44:15.000000 aiocloudweather-2024.2.2/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-29 22:00:22.879695 aiocloudweather-2024.2.2/aiocloudweather/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      120 2024-05-26 16:06:10.000000 aiocloudweather-2024.2.2/aiocloudweather/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1605 2024-05-26 16:17:09.000000 aiocloudweather-2024.2.2/aiocloudweather/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1963 2024-05-20 11:00:26.000000 aiocloudweather-2024.2.2/aiocloudweather/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1401 2024-05-26 16:55:13.000000 aiocloudweather-2024.2.2/aiocloudweather/conversion.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-20 09:40:32.000000 aiocloudweather-2024.2.2/aiocloudweather/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10874 2024-05-26 17:12:45.000000 aiocloudweather-2024.2.2/aiocloudweather/sensor.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3731 2024-05-26 16:16:59.000000 aiocloudweather-2024.2.2/aiocloudweather/server.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-29 22:00:22.880695 aiocloudweather-2024.2.2/aiocloudweather.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      686 2024-05-29 22:00:22.000000 aiocloudweather-2024.2.2/aiocloudweather.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      565 2024-05-29 22:00:22.000000 aiocloudweather-2024.2.2/aiocloudweather.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-29 22:00:22.000000 aiocloudweather-2024.2.2/aiocloudweather.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       74 2024-05-29 22:00:22.000000 aiocloudweather-2024.2.2/aiocloudweather.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-29 22:00:22.000000 aiocloudweather-2024.2.2/aiocloudweather.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2024-05-29 22:00:22.000000 aiocloudweather-2024.2.2/aiocloudweather.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2024-05-29 22:00:22.000000 aiocloudweather-2024.2.2/aiocloudweather.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1488 2024-05-29 22:00:22.881695 aiocloudweather-2024.2.2/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2024-05-26 16:31:50.000000 aiocloudweather-2024.2.2/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-29 22:00:22.880695 aiocloudweather-2024.2.2/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1861 2024-05-26 16:54:12.000000 aiocloudweather-2024.2.2/tests/test_conversion.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2618 2024-05-26 17:10:47.000000 aiocloudweather-2024.2.2/tests/test_sensor.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1097 2024-05-26 18:18:41.000000 aiocloudweather-2024.2.2/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:37:36.083866 aiocloudweather-2024.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 20:37:36.083866 aiocloudweather-2024.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:37:36.079866 aiocloudweather-2024.5.0/aiocloudweather/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/aiocloudweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/aiocloudweather/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/aiocloudweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/aiocloudweather/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/aiocloudweather/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/aiocloudweather/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/aiocloudweather/station.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:37:36.083866 aiocloudweather-2024.5.0/aiocloudweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 20:37:36.000000 aiocloudweather-2024.5.0/aiocloudweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 20:37:36.000000 aiocloudweather-2024.5.0/aiocloudweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:37:36.000000 aiocloudweather-2024.5.0/aiocloudweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 20:37:36.000000 aiocloudweather-2024.5.0/aiocloudweather.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:37:36.000000 aiocloudweather-2024.5.0/aiocloudweather.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 20:37:36.000000 aiocloudweather-2024.5.0/aiocloudweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 20:37:36.000000 aiocloudweather-2024.5.0/aiocloudweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 20:37:36.083866 aiocloudweather-2024.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:37:36.083866 aiocloudweather-2024.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-30 20:37:27.000000 aiocloudweather-2024.5.0/tests/test_server.py
```

### Comparing `aiocloudweather-2024.2.2/LICENSE` & `aiocloudweather-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.2.2/PKG-INFO` & `aiocloudweather-2024.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.2.2
+Version: 2024.5.0
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.2.2/aiocloudweather/__main__.py` & `aiocloudweather-2024.5.0/aiocloudweather/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 from dataclasses import Field, fields
 import logging
 import sys
 from types import NoneType
 
 from aiocloudweather import CloudWeatherListener, WeatherStation
-from aiocloudweather.sensor import Sensor
+from aiocloudweather.station import Sensor
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def usage():
     """Print usage of the CLI."""
     print(f"Usage: {sys.argv[0]} port")
```

### Comparing `aiocloudweather-2024.2.2/aiocloudweather/const.py` & `aiocloudweather-2024.5.0/aiocloudweather/const.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.2.2/aiocloudweather/conversion.py` & `aiocloudweather-2024.5.0/aiocloudweather/conversion.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.2.2/aiocloudweather/sensor.py` & `aiocloudweather-2024.5.0/aiocloudweather/station.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """"""
 
 from dataclasses import dataclass, field, fields
 import logging
-from types import NoneType
 from typing import Final
 
 from aiocloudweather.conversion import (
     celsius_to_fahrenheit,
     fahrenheit_to_celsius,
     hpa_to_inhg,
     in_to_mm,
@@ -182,14 +181,16 @@
 class WeatherStation:
     """
     Represents a weather station with various sensor readings.
     """
 
     station_id: str
     station_key: str
+    update_time: float = field(default=None)
+
     date_utc: str = field(default=None)
 
     barometer: Sensor = field(default=None)
     temperature: Sensor = field(default=None)
     humidity: Sensor = field(default=None)
     indoor_temperature: Sensor = field(default=None)
     indoor_humidity: Sensor = field(default=None)
```

### Comparing `aiocloudweather-2024.2.2/aiocloudweather/server.py` & `aiocloudweather-2024.5.0/aiocloudweather/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """aioCloudWeather API server."""
 
 from __future__ import annotations
 
 import logging
+import time
 from typing import Callable
 from copy import deepcopy
 from dataclasses import fields
 
 from aiohttp import web
 
-from aiocloudweather.sensor import WundergroundRawSensor, WeathercloudRawSensor, WeatherStation
+from aiocloudweather.station import WundergroundRawSensor, WeathercloudRawSensor, WeatherStation
 
 _LOGGER = logging.getLogger(__name__)
 _CLOUDWEATHER_LISTEN_PORT = 49199
 
 
 class CloudWeatherListener:
     """CloudWeather Server API server."""
@@ -26,14 +27,15 @@
         # webserver
         self.server: None | web.Server = None
         self.runner: None | web.ServerRunner = None
         self.site: None | web.TCPSite = None
 
         # internal data
         self.last_values: dict[str, WeatherStation] = {}
+        self.last_updates: dict[str, float] = {}
         self.new_dataset_cb: list[Callable[[WeatherStation], None]] = []
 
         # storage
         self.stations: list[str] = []
 
     async def _new_dataset_cb(self, dataset: WeatherStation) -> None:
         """Internal new sensor callback
@@ -81,14 +83,17 @@
             dataset = await self.process_weathercloud(request.path)
             station_id = dataset.station_id
         
         if station_id not in self.stations:
             _LOGGER.debug("Found new station: %s", station_id)
             self.stations.append(station_id)
 
+        self.last_updates[station_id] = time.monotonic()
+        dataset.last_update = self.last_updates[station_id]
+
         try:
             await self._new_dataset_cb(dataset)
         except Exception as err:  # pylint: disable=broad-except
             _LOGGER.warning("CloudWeather new dataset callback error: %s", err)
 
         self.last_values[station_id] = deepcopy(dataset)
         return web.Response(text="OK")
```

### Comparing `aiocloudweather-2024.2.2/aiocloudweather.egg-info/PKG-INFO` & `aiocloudweather-2024.5.0/aiocloudweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.2.2
+Version: 2024.5.0
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.2.2/aiocloudweather.egg-info/SOURCES.txt` & `aiocloudweather-2024.5.0/aiocloudweather.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 setup.cfg
 setup.py
 aiocloudweather/__init__.py
 aiocloudweather/__main__.py
 aiocloudweather/const.py
 aiocloudweather/conversion.py
 aiocloudweather/py.typed
-aiocloudweather/sensor.py
 aiocloudweather/server.py
+aiocloudweather/station.py
 aiocloudweather.egg-info/PKG-INFO
 aiocloudweather.egg-info/SOURCES.txt
 aiocloudweather.egg-info/dependency_links.txt
 aiocloudweather.egg-info/entry_points.txt
 aiocloudweather.egg-info/not-zip-safe
 aiocloudweather.egg-info/requires.txt
 aiocloudweather.egg-info/top_level.txt
```

### Comparing `aiocloudweather-2024.2.2/setup.cfg` & `aiocloudweather-2024.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.2.2/setup.py` & `aiocloudweather-2024.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2024.2.2"
+VERSION = "2024.5.0"
 
 
 setup(
     name="aiocloudweather",
     version=VERSION,
     url="https://github.com/lhw/aiocloudweather",
     download_url="https://github.com/lhw/aiocloudweather",
```

### Comparing `aiocloudweather-2024.2.2/tests/test_conversion.py` & `aiocloudweather-2024.5.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.2.2/tests/test_sensor.py` & `aiocloudweather-2024.5.0/tests/test_sensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from aiocloudweather.sensor import WeatherStation, WundergroundRawSensor, WeathercloudRawSensor
+from aiocloudweather.station import WeatherStation, WundergroundRawSensor, WeathercloudRawSensor
 
 def test_weather_station_from_wunderground():
     raw_sensor_data = WundergroundRawSensor(
         station_id="12345",
         station_key="12345",
         barometer=29.92,
         temperature=72.5,
```

### Comparing `aiocloudweather-2024.2.2/tests/test_server.py` & `aiocloudweather-2024.5.0/tests/test_server.py`

 * *Files identical despite different names*

