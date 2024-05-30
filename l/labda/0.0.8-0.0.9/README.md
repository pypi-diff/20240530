# Comparing `tmp/labda-0.0.8.tar.gz` & `tmp/labda-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labda-0.0.8.tar", max compression
+gzip compressed data, was "labda-0.0.9.tar", max compression
```

## Comparing `labda-0.0.8.tar` & `labda-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      294 2024-05-27 07:21:21.966442 labda-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      219 2024-05-06 14:08:06.476463 labda-0.0.8/LICENSE.md
--rw-r--r--   0        0        0      949 2024-05-27 07:21:21.976442 labda-0.0.8/README.md
--rw-r--r--   0        0        0      183 2024-05-11 06:11:49.000349 labda-0.0.8/labda/__init__.py
--rw-r--r--   0        0        0      142 2024-04-17 03:56:15.837647 labda-0.0.8/labda/assets/__init__.py
--rw-r--r--   0        0        0     1195 2024-04-17 03:56:15.837647 labda-0.0.8/labda/assets/counts_cut_points.py
--rw-r--r--   0        0        0      808 2024-05-06 14:08:06.646463 labda-0.0.8/labda/assets/transportation_cut_points.py
--rw-r--r--   0        0        0      152 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/__init__.py
--rw-r--r--   0        0        0      656 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/accelerometer.py
--rw-r--r--   0        0        0      964 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/extras.py
--rw-r--r--   0        0        0     7377 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/spatial.py
--rw-r--r--   0        0        0     1238 2024-05-27 07:21:22.236442 labda-0.0.8/labda/logging.py
--rw-r--r--   0        0        0     1163 2024-05-09 08:50:19.212123 labda-0.0.8/labda/parallel.py
--rw-r--r--   0        0        0      201 2024-05-06 14:08:06.646463 labda-0.0.8/labda/parsers/__init__.py
--rw-r--r--   0        0        0     6852 2024-05-09 16:16:33.961740 labda-0.0.8/labda/parsers/actigraph.py
--rw-r--r--   0        0        0     1013 2024-05-09 08:47:40.902125 labda-0.0.8/labda/parsers/bulk.py
--rw-r--r--   0        0        0     6508 2024-04-17 03:56:15.837647 labda-0.0.8/labda/parsers/gadgetbridge.py
--rw-r--r--   0        0        0     2332 2024-04-17 03:56:15.837647 labda-0.0.8/labda/parsers/garmin.py
--rw-r--r--   0        0        0    10993 2024-05-09 16:26:39.781731 labda-0.0.8/labda/parsers/qstarz.py
--rw-r--r--   0        0        0     8566 2024-05-27 07:21:22.236442 labda-0.0.8/labda/parsers/sens.py
--rw-r--r--   0        0        0     9835 2024-05-27 07:21:22.236442 labda-0.0.8/labda/parsers/traccar.py
--rw-r--r--   0        0        0       37 2024-05-09 16:43:23.301717 labda-0.0.8/labda/processing/__init__.py
--rw-r--r--   0        0        0       88 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/__init__.py
--rw-r--r--   0        0        0     1580 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/activity_intensity.py
--rw-r--r--   0        0        0      616 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/steps.py
--rw-r--r--   0        0        0      913 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/wear.py
--rw-r--r--   0        0        0     2803 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/bouts.py
--rw-r--r--   0        0        0     2635 2024-05-11 12:15:33.238139 labda-0.0.8/labda/processing/context.py
--rw-r--r--   0        0        0      536 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/manipulations.py
--rw-r--r--   0        0        0      197 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/spatial/__init__.py
--rw-r--r--   0        0        0     6880 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/spatial/manipulations.py
--rw-r--r--   0        0        0     3277 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/spatial/timeline.py
--rw-r--r--   0        0        0     3797 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/spatial/transportation.py
--rw-r--r--   0        0        0    26484 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/spatial/trips.py
--rw-r--r--   0        0        0     2622 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/wear_validity.py
--rw-r--r--   0        0        0      252 2024-05-11 06:12:01.210349 labda-0.0.8/labda/structure/__init__.py
--rw-r--r--   0        0        0     5196 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/collection.py
--rw-r--r--   0        0        0     2595 2024-05-11 07:41:03.550336 labda-0.0.8/labda/structure/contexts.py
--rw-r--r--   0        0        0      600 2024-04-17 03:56:15.847647 labda-0.0.8/labda/structure/linkage.py
--rw-r--r--   0        0        0     8766 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/merging.py
--rw-r--r--   0        0        0     3435 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/resampling.py
--rw-r--r--   0        0        0    20115 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/subject.py
--rw-r--r--   0        0        0        0 2024-04-17 03:56:15.847647 labda-0.0.8/labda/structure/validation/__init__.py
--rw-r--r--   0        0        0     1337 2024-05-09 14:43:53.361819 labda-0.0.8/labda/structure/validation/context.py
--rw-r--r--   0        0        0      833 2024-04-17 03:56:15.847647 labda-0.0.8/labda/structure/validation/linkage.py
--rw-r--r--   0        0        0    11339 2024-05-11 12:15:54.098139 labda-0.0.8/labda/structure/validation/subject.py
--rw-r--r--   0        0        0     9961 2024-05-09 16:15:48.251740 labda-0.0.8/labda/utils.py
--rw-r--r--   0        0        0        0 2024-02-03 08:38:41.168015 labda-0.0.8/labda/visualisation/__init__.py
--rw-r--r--   0        0        0     3785 2024-05-11 09:52:34.810315 labda-0.0.8/labda/visualisation/spatial.py
--rw-r--r--   0        0        0     1697 2024-05-27 07:21:33.146442 labda-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 labda-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      294 2024-05-27 07:21:21.966442 labda-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      219 2024-05-06 14:08:06.476463 labda-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0      949 2024-05-27 07:21:21.976442 labda-0.0.9/README.md
+-rw-r--r--   0        0        0      183 2024-05-11 06:11:49.000349 labda-0.0.9/labda/__init__.py
+-rw-r--r--   0        0        0      142 2024-04-17 03:56:15.837647 labda-0.0.9/labda/assets/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-17 03:56:15.837647 labda-0.0.9/labda/assets/counts_cut_points.py
+-rw-r--r--   0        0        0      808 2024-05-06 14:08:06.646463 labda-0.0.9/labda/assets/transportation_cut_points.py
+-rw-r--r--   0        0        0      152 2024-04-17 03:56:15.837647 labda-0.0.9/labda/expanders/__init__.py
+-rw-r--r--   0        0        0      656 2024-04-17 03:56:15.837647 labda-0.0.9/labda/expanders/accelerometer.py
+-rw-r--r--   0        0        0      964 2024-04-17 03:56:15.837647 labda-0.0.9/labda/expanders/extras.py
+-rw-r--r--   0        0        0     7377 2024-04-17 03:56:15.837647 labda-0.0.9/labda/expanders/spatial.py
+-rw-r--r--   0        0        0     1238 2024-05-27 07:21:22.236442 labda-0.0.9/labda/logging.py
+-rw-r--r--   0        0        0     1163 2024-05-09 08:50:19.212123 labda-0.0.9/labda/parallel.py
+-rw-r--r--   0        0        0      201 2024-05-06 14:08:06.646463 labda-0.0.9/labda/parsers/__init__.py
+-rw-r--r--   0        0        0     6852 2024-05-09 16:16:33.961740 labda-0.0.9/labda/parsers/actigraph.py
+-rw-r--r--   0        0        0     1013 2024-05-09 08:47:40.902125 labda-0.0.9/labda/parsers/bulk.py
+-rw-r--r--   0        0        0     6508 2024-04-17 03:56:15.837647 labda-0.0.9/labda/parsers/gadgetbridge.py
+-rw-r--r--   0        0        0     2332 2024-04-17 03:56:15.837647 labda-0.0.9/labda/parsers/garmin.py
+-rw-r--r--   0        0        0    10993 2024-05-09 16:26:39.781731 labda-0.0.9/labda/parsers/qstarz.py
+-rw-r--r--   0        0        0     8848 2024-05-28 16:52:23.520237 labda-0.0.9/labda/parsers/sens.py
+-rw-r--r--   0        0        0    10531 2024-05-27 14:53:55.009940 labda-0.0.9/labda/parsers/traccar.py
+-rw-r--r--   0        0        0       37 2024-05-09 16:43:23.301717 labda-0.0.9/labda/processing/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-17 03:56:15.837647 labda-0.0.9/labda/processing/accelerometer/__init__.py
+-rw-r--r--   0        0        0     1580 2024-04-17 03:56:15.837647 labda-0.0.9/labda/processing/accelerometer/activity_intensity.py
+-rw-r--r--   0        0        0      616 2024-04-17 03:56:15.837647 labda-0.0.9/labda/processing/accelerometer/steps.py
+-rw-r--r--   0        0        0      913 2024-04-17 03:56:15.837647 labda-0.0.9/labda/processing/accelerometer/wear.py
+-rw-r--r--   0        0        0     2803 2024-04-17 03:56:15.837647 labda-0.0.9/labda/processing/bouts.py
+-rw-r--r--   0        0        0     2635 2024-05-11 12:15:33.238139 labda-0.0.9/labda/processing/context.py
+-rw-r--r--   0        0        0      536 2024-05-27 07:21:22.236442 labda-0.0.9/labda/processing/manipulations.py
+-rw-r--r--   0        0        0      197 2024-04-17 03:56:15.837647 labda-0.0.9/labda/processing/spatial/__init__.py
+-rw-r--r--   0        0        0     6880 2024-05-27 07:21:22.236442 labda-0.0.9/labda/processing/spatial/manipulations.py
+-rw-r--r--   0        0        0     3277 2024-04-17 03:56:15.837647 labda-0.0.9/labda/processing/spatial/timeline.py
+-rw-r--r--   0        0        0     3797 2024-05-27 07:21:22.236442 labda-0.0.9/labda/processing/spatial/transportation.py
+-rw-r--r--   0        0        0    26484 2024-05-27 07:21:22.236442 labda-0.0.9/labda/processing/spatial/trips.py
+-rw-r--r--   0        0        0     2622 2024-05-27 07:21:22.236442 labda-0.0.9/labda/processing/wear_validity.py
+-rw-r--r--   0        0        0      252 2024-05-11 06:12:01.210349 labda-0.0.9/labda/structure/__init__.py
+-rw-r--r--   0        0        0     5196 2024-05-27 07:21:22.236442 labda-0.0.9/labda/structure/collection.py
+-rw-r--r--   0        0        0     2595 2024-05-11 07:41:03.550336 labda-0.0.9/labda/structure/contexts.py
+-rw-r--r--   0        0        0      600 2024-04-17 03:56:15.847647 labda-0.0.9/labda/structure/linkage.py
+-rw-r--r--   0        0        0     8766 2024-05-27 07:21:22.236442 labda-0.0.9/labda/structure/merging.py
+-rw-r--r--   0        0        0     3435 2024-05-27 07:21:22.236442 labda-0.0.9/labda/structure/resampling.py
+-rw-r--r--   0        0        0    20200 2024-05-27 15:06:29.449949 labda-0.0.9/labda/structure/subject.py
+-rw-r--r--   0        0        0        0 2024-04-17 03:56:15.847647 labda-0.0.9/labda/structure/validation/__init__.py
+-rw-r--r--   0        0        0     1337 2024-05-09 14:43:53.361819 labda-0.0.9/labda/structure/validation/context.py
+-rw-r--r--   0        0        0      833 2024-04-17 03:56:15.847647 labda-0.0.9/labda/structure/validation/linkage.py
+-rw-r--r--   0        0        0    11339 2024-05-11 12:15:54.098139 labda-0.0.9/labda/structure/validation/subject.py
+-rw-r--r--   0        0        0     9961 2024-05-09 16:15:48.251740 labda-0.0.9/labda/utils.py
+-rw-r--r--   0        0        0        0 2024-02-03 08:38:41.168015 labda-0.0.9/labda/visualisation/__init__.py
+-rw-r--r--   0        0        0     3914 2024-05-27 15:07:51.509950 labda-0.0.9/labda/visualisation/spatial.py
+-rw-r--r--   0        0        0     1697 2024-05-28 18:41:23.510180 labda-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 labda-0.0.9/PKG-INFO
```

### Comparing `labda-0.0.8/README.md` & `labda-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/assets/counts_cut_points.py` & `labda-0.0.9/labda/assets/counts_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/assets/transportation_cut_points.py` & `labda-0.0.9/labda/assets/transportation_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/expanders/accelerometer.py` & `labda-0.0.9/labda/expanders/accelerometer.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/expanders/extras.py` & `labda-0.0.9/labda/expanders/extras.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/expanders/spatial.py` & `labda-0.0.9/labda/expanders/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/logging.py` & `labda-0.0.9/labda/logging.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/parallel.py` & `labda-0.0.9/labda/parallel.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/parsers/actigraph.py` & `labda-0.0.9/labda/parsers/actigraph.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/parsers/bulk.py` & `labda-0.0.9/labda/parsers/bulk.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/parsers/gadgetbridge.py` & `labda-0.0.9/labda/parsers/gadgetbridge.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/parsers/garmin.py` & `labda-0.0.9/labda/parsers/garmin.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/parsers/qstarz.py` & `labda-0.0.9/labda/parsers/qstarz.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/parsers/sens.py` & `labda-0.0.9/labda/parsers/sens.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,25 @@
             " activity/upright_walk/time": "boolean",
             " activity/upright_moderate/time": "boolean",
             " activity/upright_run/time": "boolean",
             " activity/cycling/time": "boolean",
         },
     )
 
-    df[Column.DATETIME] = pd.to_datetime(df[" unixts"], unit="ms", origin="unix")
+    # FIXME: Stupid thing to do, just remove whitespace from column names before anything.
+    if "utc" in df.columns and " local" in df.columns:
+        df.drop(columns=["utc", " local"], inplace=True)
+
+    if " unixts" in df.columns:
+        df.rename(columns={" unixts": "unixts"}, inplace=True)
+
+    df[Column.DATETIME] = pd.to_datetime(df["unixts"], unit="ms", origin="unix")
     df[Column.WEAR] = ~df[" general/nodata/time"]
-    df.drop(columns=["utc", " local", " unixts", " general/nodata/time"], inplace=True)
+
+    df.drop(columns=["unixts", " general/nodata/time"], inplace=True)
     df.set_index(Column.DATETIME, inplace=True)
 
     df.rename(
         columns={" activity/intensity/count": Column.ACTIVITY_VALUE}, inplace=True
     )
 
     return df
```

### Comparing `labda-0.0.8/labda/parsers/traccar.py` & `labda-0.0.9/labda/parsers/traccar.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,27 @@
     change_crs,
     change_timezone,
     get_crs,
     get_sampling_frequency,
     get_timezone,
 )
 
-# TODO: Environment determination based on GNSS_ACCURACY, not accurate points should be removed, others should be considered as indoor or outdoor points
-# (for example, remove points with accuracy over 1000 -> no signal, points with less -> 100 should be indoor, other outdoor), something like that, or actually option to specify the limit or to remove - multiple ways, but still one parameter.
-
 
 def _remove_not_accurate_points(df: pd.DataFrame, limit: int | float) -> pd.DataFrame:
     # Unit defaults to meters
     # TODO: Best value needs to be determined.
-    return df[df[Column.GNSS_ACCURACY] <= limit]
+    return df[df[Column.GNSS_ACCURACY] < limit]
+
+
+def _detect_environment(df: pd.DataFrame, limit: int | float) -> None:
+    # Unit defaults to meters
+    # TODO: Best value needs to be determined.
+    mask = df[Column.GNSS_ACCURACY].notna()
+    df.loc[mask, Column.ENVIRONMENT] = "outdoor"
+    df.loc[mask & (df[Column.GNSS_ACCURACY] > limit), Column.ENVIRONMENT] = "indoor"
 
 
 def _knots_to_kmh(knots):
     return knots * 1.852
 
 
 def _get_device(
@@ -168,15 +173,16 @@
     crs: str | None = "infer",
     timezone: str | None = "infer",
     sensor_id: str | None = None,
     vendor: Vendor = Vendor.TRACCAR,
     model: str | None = None,
     serial_number: str | None = None,
     firmware_version: str | None = None,
-    accuracy: int | float | None = None,
+    accuracy_limit: int | float | None = None,
+    environment_limit: int | float | None = None,
 ) -> Subject:
     """
     The Traccar API allows you to download data from a specific server (URL) using your login credentials (username and password). To obtain data for a particular device, you must specify a subject ID (which corresponds to the device identifier). Optionally, you can define a date and time range to download data for a specific timeframe. If no date range is provided (from/to), all data for the chosen device will be downloaded.
 
     The downloaded data will be parsed and validated according to the schema defined in the structure module.
 
     Args:
@@ -190,24 +196,26 @@
         timezone (str, optional): The timezone of the data. If set to "infer" it will be inferred from the data. If None it will be set to the local timezone. Otherwise, it will be set to the provided timezone.
         crs (str, optional): The coordinate reference system (CRS) of the data. If set to "infer" it will be inferred from the data. If None it will be set to "EPSG:4326". Otherwise, it will be set to the provided CRS.
         sensor_id (str, optional): The ID of the sensor to fetch data for. If not provided, unique device ID from Traccar server will be used (if available).
         vendor (Vendor, optional): The vendor of the device. Defaults to "Traccar".
         model (str, optional): The model of the device. If not provided, it will be fetched from the Traccar server (device - extra, phone + model) if available.
         serial_number (str, optional): The serial number of the device.
         firmware_version (str, optional): The firmware version of the device.
-        accuracy (int | float, optional): The maximum allowed GPS accuracy. If not provided, all points will be included, otherwise only points with accuracy less or equal to the provided value will be included.
+        accuracy_limit (int | float, optional): The maximum allowed GPS accuracy. If not provided, all points will be included, otherwise only points with accuracy less to the provided value will be included.
+        environment_limit (int | float, optional): The maximum allowed GPS accuracy to determine if the point is indoor or outdoor. If point accuracy is less to the provided value, the point will be marked as indoor, otherwise it will be marked as outdoor. If not provided, environment will not be detected.
 
     Returns:
         Subject: A Subject object containing the fetched and processed dataframe containing information: datetime, latitude, longitude, gps_accuracy, distance, elevation, and speed.
 
 
     Raises:
         HTTPError: HTTP request to the Traccar server failed.
         ValueError: No device is found for the specified subject ID.
         ValueError: No records are found for the specified device.
+        ValueError: Environment limit must be lower than accuracy limit.
 
     Examples:
         Here's how to call the function with just the minimum required parameters.
 
         ```python
         from labda.parsers import Traccar
 
@@ -252,16 +260,24 @@
         df = change_crs(df, origin_crs, crs)
 
     if not sampling_frequency:
         sampling_frequency = get_sampling_frequency(df)
 
     df = align_datetimes(df, sampling_frequency)
 
-    if accuracy:
-        df = _remove_not_accurate_points(df, accuracy)
+    if environment_limit and accuracy_limit and environment_limit >= accuracy_limit:
+        raise ValueError(
+            "Environment limit must be lower than accuracy limit. Please provide a lower value for environment limit."
+        )
+
+    if accuracy_limit:
+        df = _remove_not_accurate_points(df, accuracy_limit)
+
+    if environment_limit:
+        _detect_environment(df, environment_limit)
 
     # Order columns as defined in Column, remove extra columns
     records_columns = [col.value for col in Column]
     ordered_columns = [col for col in records_columns if col in df.columns]
     df = df[ordered_columns]
 
     df = SCHEMA.validate(df)
```

### Comparing `labda-0.0.8/labda/processing/accelerometer/activity_intensity.py` & `labda-0.0.9/labda/processing/accelerometer/activity_intensity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/accelerometer/steps.py` & `labda-0.0.9/labda/processing/accelerometer/steps.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/accelerometer/wear.py` & `labda-0.0.9/labda/processing/accelerometer/wear.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/bouts.py` & `labda-0.0.9/labda/processing/bouts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/context.py` & `labda-0.0.9/labda/processing/context.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/manipulations.py` & `labda-0.0.9/labda/processing/manipulations.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/spatial/manipulations.py` & `labda-0.0.9/labda/processing/spatial/manipulations.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/spatial/timeline.py` & `labda-0.0.9/labda/processing/spatial/timeline.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/spatial/transportation.py` & `labda-0.0.9/labda/processing/spatial/transportation.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/spatial/trips.py` & `labda-0.0.9/labda/processing/spatial/trips.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/processing/wear_validity.py` & `labda-0.0.9/labda/processing/wear_validity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/collection.py` & `labda-0.0.9/labda/structure/collection.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/contexts.py` & `labda-0.0.9/labda/structure/contexts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/linkage.py` & `labda-0.0.9/labda/structure/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/merging.py` & `labda-0.0.9/labda/structure/merging.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/resampling.py` & `labda-0.0.9/labda/structure/resampling.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/subject.py` & `labda-0.0.9/labda/structure/subject.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,15 +506,20 @@
             self.df,
             self.metadata.sampling_frequency,
             sampling_frequency,
             mapper,
         )
         self.metadata.sampling_frequency = sampling_frequency
 
-    def plot(self, kind: str) -> Any:
+    def plot(
+        self,
+        kind: str,
+        *,
+        path: Path | str | None = None,
+    ) -> Any:
         """
         Plots the subject's data based on the specified kind.
 
         The kind of plot to produce is specified by the 'kind' argument. The following kinds are supported:
         - 'gps': Plots the subject's raw GPS data.
         - 'timeline': Plots the subject's timeline data (trips with pauses and stationary points).
 
@@ -534,8 +539,8 @@
                 else:
                     raise ValueError("Timeline does not exist. Run 'detect_trips'.")
             case "gps":
                 df = self.df
             case _:
                 raise ValueError(f"Kind '{kind}' not supported.")
 
-        return plot(df, kind, crs=self.metadata.crs)
+        return plot(df, kind, crs=self.metadata.crs, path=path)
```

### Comparing `labda-0.0.8/labda/structure/validation/context.py` & `labda-0.0.9/labda/structure/validation/context.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/validation/linkage.py` & `labda-0.0.9/labda/structure/validation/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/structure/validation/subject.py` & `labda-0.0.9/labda/structure/validation/subject.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/utils.py` & `labda-0.0.9/labda/utils.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.8/labda/visualisation/spatial.py` & `labda-0.0.9/labda/visualisation/spatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Any, Dict, Tuple
 
 import geopandas as gpd
 import pandas as pd
 import pydeck as pdk
 from shapely.geometry import Point
 
@@ -43,15 +44,15 @@
 
     gdf.to_crs(epsg=4326, inplace=True)
 
     layer = pdk.Layer(
         "GeoJsonLayer",
         gdf,
         get_position="geometry.coordinates",
-        get_radius=10,  # Radius is in meters
+        get_radius=12,  # Radius is in meters
         get_fill_color="color",
         get_line_color="color",
         get_line_width=7.5,
         pickable=True,
         auto_highlight=True,
     )
 
@@ -83,15 +84,15 @@
 
     layer = pdk.Layer(
         "GeoJsonLayer",
         gdf,
         stroked=False,
         filled=True,
         get_position="geometry.coordinates",
-        get_radius=7.5,  # Radius is in meters
+        get_radius=8,  # Radius is in meters
         get_fill_color=[255, 0, 0],
         get_line_width=5,
         pickable=True,
         auto_highlight=True,
     )
 
     tooltip = {
@@ -105,15 +106,19 @@
 
 
 def plot(
     df: pd.DataFrame,
     kind: str,
     *,
     crs: str | None = None,
+    path: Path | str | None = None,
 ) -> str:
+    if isinstance(path, str):
+        path = Path(path)
+
     match kind:
         case "timeline":
             layer, tooltip, center = timeline_layer(df, crs)
         case "gps":
             layer, tooltip, center = gps_layer(df, crs)
         # case "context":
         #     layer, tooltip, center = context_layer(df, crs)
@@ -122,8 +127,8 @@
 
     # Set the viewport location
     view_state = pdk.ViewState(longitude=center.x, latitude=center.y, zoom=10)
 
     # Render
     r = pdk.Deck(layers=[layer], initial_view_state=view_state, tooltip=tooltip)  # type: ignore
 
-    return r.to_html()  # type: ignore
+    return r.to_html(filename=path)  # type: ignore
```

### Comparing `labda-0.0.8/pyproject.toml` & `labda-0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labda"
-version = "0.0.8"
+version = "0.0.9"
 description = "Library for Advanced Behavioural Data Analysis"
 authors = ["Josef Heidler <jheidler@health.sdu.dk>"]
 maintainers = ["Josef Heidler <jheidler@health.sdu.dk>"]
 
 readme = "README.md"
 license = "	CC-BY-SA-4.0"
 homepage = "https://labda.josefheidler.cz"
```

### Comparing `labda-0.0.8/PKG-INFO` & `labda-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labda
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for Advanced Behavioural Data Analysis
 Home-page: https://labda.josefheidler.cz
 License: 	CC-BY-SA-4.0
 Keywords: analysis,health,behaviour,data,spatial,temporal
 Author: Josef Heidler
 Author-email: jheidler@health.sdu.dk
 Maintainer: Josef Heidler
```

