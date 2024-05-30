# Comparing `tmp/pyastroweatherio-0.50.2.tar.gz` & `tmp/pyastroweatherio-0.50.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.2.tar", last modified: Tue May 28 05:27:43 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.3.tar", last modified: Thu May 30 06:41:33 2024, max compression
```

## Comparing `pyastroweatherio-0.50.2.tar` & `pyastroweatherio-0.50.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-28 05:27:43.419647 pyastroweatherio-0.50.2/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.2/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-28 05:27:43.419647 pyastroweatherio-0.50.2/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1519 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-28 05:27:43.403646 pyastroweatherio-0.50.2/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      284 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    42587 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     6068 2024-05-27 17:28:04.000000 pyastroweatherio-0.50.2/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    24611 2024-05-28 05:26:46.000000 pyastroweatherio-0.50.2/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2024-05-25 14:57:18.000000 pyastroweatherio-0.50.2/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    50052 2024-05-28 05:27:01.000000 pyastroweatherio-0.50.2/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-28 05:27:43.415646 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       25 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-28 05:27:43.000000 pyastroweatherio-0.50.2/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-28 05:27:43.423647 pyastroweatherio-0.50.2/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1397 2024-05-28 05:27:15.000000 pyastroweatherio-0.50.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-30 06:41:33.737000 pyastroweatherio-0.50.3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1071 2024-05-29 21:14:23.000000 pyastroweatherio-0.50.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1112 2024-05-30 06:41:33.737000 pyastroweatherio-0.50.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1519 2024-05-29 21:14:23.000000 pyastroweatherio-0.50.3/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-30 06:41:33.735000 pyastroweatherio-0.50.3/pyastroweatherio/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      284 2024-05-29 21:14:23.000000 pyastroweatherio-0.50.3/pyastroweatherio/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    43453 2024-05-29 21:15:11.000000 pyastroweatherio-0.50.3/pyastroweatherio/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6068 2024-05-29 21:14:23.000000 pyastroweatherio-0.50.3/pyastroweatherio/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24611 2024-05-29 21:14:23.000000 pyastroweatherio-0.50.3/pyastroweatherio/dataclasses.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      337 2024-05-29 21:14:23.000000 pyastroweatherio-0.50.3/pyastroweatherio/errors.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    50108 2024-05-29 21:15:35.000000 pyastroweatherio-0.50.3/pyastroweatherio/helper_functions.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-30 06:41:33.736000 pyastroweatherio-0.50.3/pyastroweatherio.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1112 2024-05-30 06:41:33.000000 pyastroweatherio-0.50.3/pyastroweatherio.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      413 2024-05-30 06:41:33.000000 pyastroweatherio-0.50.3/pyastroweatherio.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-30 06:41:33.000000 pyastroweatherio-0.50.3/pyastroweatherio.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       25 2024-05-30 06:41:33.000000 pyastroweatherio-0.50.3/pyastroweatherio.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       17 2024-05-30 06:41:33.000000 pyastroweatherio-0.50.3/pyastroweatherio.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2024-05-30 06:41:33.738000 pyastroweatherio-0.50.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1397 2024-05-30 06:08:53.000000 pyastroweatherio-0.50.3/setup.py
```

### Comparing `pyastroweatherio-0.50.2/LICENSE` & `pyastroweatherio-0.50.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.2/PKG-INFO` & `pyastroweatherio-0.50.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.2
+Version: 0.50.3
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.2/README.md` & `pyastroweatherio-0.50.3/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.2/pyastroweatherio/client.py` & `pyastroweatherio-0.50.3/pyastroweatherio/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,14 +187,40 @@
 
         details_metno = (
             self._weather_data_metno[metno_index]
             .get("data", {})
             .get("instant", {})
             .get("details", {})
         )
+        details_metno_next_1_hours = (
+            self._weather_data_metno[metno_index]
+            .get("data", {})
+            .get("next_1_hours", {})
+        )
+        details_metno_next_6_hours = (
+            self._weather_data_metno[metno_index]
+            .get("data", {})
+            .get("next_6_hours", {})
+        )
+
+        # Break condition
+        if details_metno_next_1_hours is None:
+            # No more hourly data
+            _LOGGER.debug(
+                "No more hourly data at %s",
+                self._weather_data_metno[metno_index].get("time", {}),
+            )
+            return None
+        if details_metno_next_6_hours is None:
+            # No more 6-hourly data
+            _LOGGER.debug(
+                "No more 6-hourly data at %s",
+                self._weather_data_metno[metno_index].get("time", {}),
+            )
+            return None
 
         # 7Timer: Search for start index
         seventimer_init = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
         for row7 in self._weather_data_seventimer:
             if seventimer_init + timedelta(hours=row7["timepoint"]) > now:
                 break
             seventimer_index += 1
@@ -309,39 +335,32 @@
             ),
             "fog_area_fraction": details_metno.get("fog_area_fraction"),
             "rh2m": details_metno.get("relative_humidity"),
             "wind_speed": details_metno.get("wind_speed"),
             "wind_from_direction": details_metno.get("wind_from_direction"),
             "temp2m": details_metno.get("air_temperature"),
             "dewpoint2m": details_metno.get("dew_point_temperature"),
-            "weather": self._weather_data_metno[metno_index]
-            .get("data", {})
-            .get("next_1_hours", {})
-            .get("summary", {})
-            .get("symbol_code"),
-            "weather6": self._weather_data_metno[metno_index]
-            .get("data", {})
-            .get("next_6_hours", {})
-            .get("summary", {})
-            .get("symbol_code"),
-            "precipitation_amount": (
-                self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_1_hours", {})
-                .get("details", {})
-                .get("precipitation_amount")
+            "weather": details_metno_next_1_hours.get("summary", {}).get("symbol_code"),
+            "weather6": details_metno_next_6_hours.get("summary", {}).get(
+                "symbol_code"
+            ),
+            "precipitation_amount": details_metno_next_1_hours.get("details", {}).get(
+                "precipitation_amount"
             ),
             # Condition
             "condition_percentage": await self._calc_condition_percentage(
                 details_metno.get("cloud_area_fraction_high"),
                 details_metno.get("cloud_area_fraction_medium"),
                 details_metno.get("cloud_area_fraction_low"),
                 seeing,
                 transparency,
                 details_metno.get("wind_speed"),
+                details_metno_next_1_hours.get("details", {}).get(
+                    "precipitation_amount"
+                ),
             ),
             # Uptonight objects
             "uptonight": await self._get_deepsky_objects(),
         }
 
         items.append(LocationData(item))
 
@@ -392,26 +411,50 @@
                 datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"
             ) - last_forecast_time > timedelta(hours=1):
                 break
 
             last_forecast_time = datetime.strptime(
                 datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"
             )
-            details_metno = (
-                datapoint.get("data", {}).get("instant", {}).get("details", {})
-            )
+            details_metno = datapoint.get("data", {}).get("instant", {}).get("details")
 
             if details_metno.get("cloud_area_fraction") is None:
                 _LOGGER.error("Missing Met.no data")
                 break
 
             details_seventimer = self._get_data_seventimer_timer(
                 seventimer_init,
                 datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"),
             )
+            details_metno_next_1_hours = (
+                self._weather_data_metno[metno_index]
+                .get("data", {})
+                .get("next_1_hours")
+            )
+            details_metno_next_6_hours = (
+                self._weather_data_metno[metno_index]
+                .get("data", {})
+                .get("next_6_hours")
+            )
+
+            # Break condition
+            if details_metno_next_1_hours is None:
+                # No more hourly data
+                _LOGGER.debug(
+                    "No more hourly data at %s",
+                    self._weather_data_metno[metno_index].get("time", {}),
+                )
+                break
+            if details_metno_next_6_hours is None:
+                # No more 6-hourly data
+                _LOGGER.debug(
+                    "No more 6-hourly data at %s",
+                    self._weather_data_metno[metno_index].get("time", {}),
+                )
+                break
 
             item = {
                 "seventimer_init": init_ts,
                 "seventimer_timepoint": details_seventimer["timepoint"],
                 "forecast_time": datetime.strptime(
                     datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"
                 ),
@@ -480,70 +523,36 @@
             )
             item["fog_area_fraction"] = details_metno.get("fog_area_fraction")
             item["rh2m"] = details_metno.get("relative_humidity")
             item["wind_speed"] = details_metno.get("wind_speed")
             item["seeing"] = seeing
             item["transparency"] = transparency
             item["lifted_index"] = lifted_index
+            item["precipitation_amount"] = details_metno_next_1_hours.get(
+                "details", {}
+            ).get("precipitation_amount")
             item["condition_percentage"] = await self._calc_condition_percentage(
                 item["cloud_area_fraction_high"],
                 item["cloud_area_fraction_medium"],
                 item["cloud_area_fraction_low"],
                 seeing,
                 transparency,
                 item["wind_speed"],
+                details_metno_next_1_hours.get("details", {}).get(
+                    "precipitation_amount"
+                ),
             )
-
             item["wind_from_direction"] = details_metno.get("wind_from_direction")
             item["temp2m"] = details_metno.get("air_temperature")
             item["dewpoint2m"] = details_metno.get("dew_point_temperature")
-            if (
-                self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_1_hours")
-                is None
-            ):
-                # No more hourly data
-                _LOGGER.debug(
-                    "No more hourly data at %s",
-                    self._weather_data_metno[metno_index].get("time", {}),
-                )
-                break
-            if (
-                self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_6_hours")
-                is None
-            ):
-                # No more 6-hourly data
-                _LOGGER.debug(
-                    "No more 6-hourly data at %s",
-                    self._weather_data_metno[metno_index].get("time", {}),
-                )
-                break
-            item["weather"] = (
-                self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_1_hours", {})
-                .get("summary", {})
-                .get("symbol_code")
+            item["weather"] = details_metno_next_1_hours.get("summary", {}).get(
+                "symbol_code"
             )
-            item["weather6"] = (
-                self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_6_hours", {})
-                .get("summary", {})
-                .get("symbol_code")
-            )
-            item["precipitation_amount"] = (
-                self._weather_data_metno[metno_index]
-                .get("data", {})
-                .get("next_1_hours", {})
-                .get("details", {})
-                .get("precipitation_amount")
+            item["weather6"] = details_metno_next_6_hours.get("summary", {}).get(
+                "symbol_code"
             )
 
             items.append(ForecastData(item))
 
             item["seventimer_timepoint"] = item["seventimer_timepoint"] + 1
             item["forecast_time"] = item["forecast_time"] + timedelta(hours=1)
             item["hour"] = item["hour"] + 1
@@ -648,14 +657,15 @@
                         await self._calc_condition_percentage(
                             details_forecast.cloud_area_fraction_high_percentage,
                             details_forecast.cloud_area_fraction_medium_percentage,
                             details_forecast.cloud_area_fraction_low_percentage,
                             details_forecast.seeing,
                             details_forecast.transparency,
                             details_forecast.wind10m_speed,
+                            details_forecast.precipitation_amount,
                         )
                     )
 
                 if (
                     details_forecast.forecast_time.hour == sun_next_rising.hour
                     or index >= (forecast_data_len - 1)
                 ):
@@ -691,26 +701,28 @@
         self,
         cloudcover_high,
         cloudcover_medium,
         cloudcover_low,
         seeing,
         transparency,
         wind_speed,
+        precipitation_amount,
     ):
         """Return condition based on cloud cover, seeing, transparency, and wind speed."""
 
         if not all(
             v is not None
             for v in [
                 cloudcover_high,
                 cloudcover_medium,
                 cloudcover_low,
                 seeing,
                 transparency,
                 wind_speed,
+                precipitation_amount,
             ]
         ):
             return None
 
         # Seeing is something in between 0 and 2.5 arcsecs
         seeing = seeing * 100 / SEEING_MAX  # arcsecs up to 2.5
         # transparency = int(transparency * 40)  # mag degration up to 2.5
@@ -737,14 +749,15 @@
             )
             / (
                 self._cloudcover_weight
                 + self._seeing_weight
                 + self._transparency_weight
                 + self._calm_weight
             )
+            - precipitation_amount * 100
         )
 
         # _LOGGER.debug(
         #     "Cloudcover: %s %s, Seeing: %s %s, Transparency: %s %s, Calmness: %s %s, Conditions: %s",
         #     str(max(cloudcover)),
         #     str(self._cloudcover_weight),
         #     str(seeing),
@@ -752,14 +765,17 @@
         #     str(transparency),
         #     str(self._transparency_weight),
         #     str(wind_speed_value),
         #     str(self._calm_weight),
         #     condition,
         # )
 
+        # Ensure condition is within the valid range [0, 1]
+        condition = max(0, min(100, condition))
+
         return condition
 
     async def _get_deepsky_objects(self):
         """Return Deepsky Objects for today."""
 
         items = []
```

### Comparing `pyastroweatherio-0.50.2/pyastroweatherio/const.py` & `pyastroweatherio-0.50.3/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.2/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.3/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.2/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.3/pyastroweatherio/helper_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,29 +100,29 @@
         lifted_temp_500mb = (
             env_temp_500mb + (temperature - lcl) * 0.5
         )  # Assumption: 500 mb is halfway through the troposphere
 
         # Calculate Lifted Index
         lifted_index = env_temp_500mb - lifted_temp_500mb
 
-        _LOGGER.debug(
-            "Lifted Index (LI): {:.2f} °C (".format(lifted_index)
-            + "Air pressure at sea level (AP): {:.2f} mbar, ".format(
-                air_pressure_at_sea_level
-            )
-            + "Dew point(DP): {:.2f} °C, ".format(dew_point_temperature)
-            + "Temperature (T): {:.2f} °C, ".format(temperature)
-            + "Saturation vapor pressure at surface (ES): {:.2f} mbar, ".format(es)
-            + "Actual vapor pressure at surface (E): {:.2f} mbar, ".format(e)
-            + "Mixing ratio at surface (W): {:.2f} grams per kg, ".format(w)
-            + "Lifting Condensation Level (LCL): {:.2f} meters, ".format(lcl)
-            + "Temperature of the lifted parcel (T Parcel): {:.2f} °C)".format(
-                lifted_temp_500mb
-            )
-        )
+        # _LOGGER.debug(
+        #     "Lifted Index (LI): {:.2f} °C (".format(lifted_index)
+        #     + "Air pressure at sea level (AP): {:.2f} mbar, ".format(
+        #         air_pressure_at_sea_level
+        #     )
+        #     + "Dew point(DP): {:.2f} °C, ".format(dew_point_temperature)
+        #     + "Temperature (T): {:.2f} °C, ".format(temperature)
+        #     + "Saturation vapor pressure at surface (ES): {:.2f} mbar, ".format(es)
+        #     + "Actual vapor pressure at surface (E): {:.2f} mbar, ".format(e)
+        #     + "Mixing ratio at surface (W): {:.2f} grams per kg, ".format(w)
+        #     + "Lifting Condensation Level (LCL): {:.2f} meters, ".format(lcl)
+        #     + "Temperature of the lifted parcel (T Parcel): {:.2f} °C)".format(
+        #         lifted_temp_500mb
+        #     )
+        # )
 
         return lifted_index
 
     # #####################################################
     # Calculate magniture degradation based on transparency
     # #####################################################
     async def magnitude_degradation(
@@ -196,20 +196,20 @@
         )
 
         # Convert transparency to magnitude degradation
         magnitude_degradation = self._transparency_to_magnitude_degradation(
             transparency
         )
 
-        _LOGGER.debug(
-            "Magnitude Degradation: {:.2f} mag (".format(magnitude_degradation)
-            + "Lifted Index (LI): {:.2f} °C, ".format(lifted_index)
-            + "Seeing: {:.2f} arcsec, ".format(seeing)
-            + "Estimated Atmospheric Transparency: {:.2f})".format(transparency)
-        )
+        # _LOGGER.debug(
+        #     "Magnitude Degradation: {:.2f} mag (".format(magnitude_degradation)
+        #     + "Lifted Index (LI): {:.2f} °C, ".format(lifted_index)
+        #     + "Seeing: {:.2f} arcsec, ".format(seeing)
+        #     + "Estimated Atmospheric Transparency: {:.2f})".format(transparency)
+        # )
 
         return magnitude_degradation
 
     # #####################################################
     # Calculate atmospheric seeing
     # #####################################################
     # Modell 6:
@@ -285,21 +285,21 @@
             C
             * (water_vapor_pressure / 10) ** 0.25
             * (wind_speed / 10) ** 0.75
             * relative_pressure
         )
         seeing = 0.98 / seeing_factor
 
-        _LOGGER.debug(
-            "Seeing: {:.2f} arcsec (".format(seeing)
-            + "Water Vapor Pressure: {:.2f} mbar, ".format(water_vapor_pressure)
-            + "Wind Speed: {:.2f} m/s, ".format(wind_speed)
-            + "Relative Pressure: {:.2f} mbar, ".format(relative_pressure)
-            + "Seeing Factor: {:.2f})".format(seeing_factor)
-        )
+        # _LOGGER.debug(
+        #     "Seeing: {:.2f} arcsec (".format(seeing)
+        #     + "Water Vapor Pressure: {:.2f} mbar, ".format(water_vapor_pressure)
+        #     + "Wind Speed: {:.2f} m/s, ".format(wind_speed)
+        #     + "Relative Pressure: {:.2f} mbar, ".format(relative_pressure)
+        #     + "Seeing Factor: {:.2f})".format(seeing_factor)
+        # )
 
         if seeing > SEEING_MAX:
             seeing = SEEING_MAX  # max out seeing
 
         return seeing
 
     # #####################################################
```

### Comparing `pyastroweatherio-0.50.2/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.3/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.2
+Version: 0.50.3
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.2/setup.py` & `pyastroweatherio-0.50.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.2",
+    version="0.50.3",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

