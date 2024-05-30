# Comparing `tmp/geoglows-1.6.2.tar.gz` & `tmp/geoglows-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.6.2.tar", last modified: Wed May 22 20:18:39 2024, max compression
+gzip compressed data, was "geoglows-1.6.3.tar", last modified: Thu May 30 17:41:33 2024, max compression
```

## Comparing `geoglows-1.6.2.tar` & `geoglows-1.6.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:18:39.047987 geoglows-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-22 20:18:30.000000 geoglows-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 20:18:30.000000 geoglows-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-22 20:18:39.047987 geoglows-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-22 20:18:30.000000 geoglows-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:18:39.047987 geoglows-1.6.2/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_download_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:18:39.047987 geoglows-1.6.2/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/streamflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-22 20:18:30.000000 geoglows-1.6.2/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:18:39.047987 geoglows-1.6.2/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-22 20:18:39.000000 geoglows-1.6.2/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-22 20:18:39.000000 geoglows-1.6.2/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:18:39.000000 geoglows-1.6.2/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 20:18:39.000000 geoglows-1.6.2/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 20:18:39.000000 geoglows-1.6.2/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-22 20:18:30.000000 geoglows-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:18:39.047987 geoglows-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-22 20:18:30.000000 geoglows-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:33.370298 geoglows-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-30 17:41:29.000000 geoglows-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 17:41:29.000000 geoglows-1.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 17:41:33.370298 geoglows-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-30 17:41:29.000000 geoglows-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:33.370298 geoglows-1.6.3/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_download_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:33.370298 geoglows-1.6.3/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16447 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11330 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15778 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/streamflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-30 17:41:29.000000 geoglows-1.6.3/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:41:33.370298 geoglows-1.6.3/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 17:41:33.000000 geoglows-1.6.3/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-30 17:41:33.000000 geoglows-1.6.3/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:41:33.000000 geoglows-1.6.3/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-30 17:41:33.000000 geoglows-1.6.3/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 17:41:33.000000 geoglows-1.6.3/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 17:41:29.000000 geoglows-1.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:41:33.370298 geoglows-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-30 17:41:29.000000 geoglows-1.6.3/setup.py
```

### Comparing `geoglows-1.6.2/LICENSE` & `geoglows-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/PKG-INFO` & `geoglows-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.6.2
+Version: 1.6.3
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.6.2/README.md` & `geoglows-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_constants.py` & `geoglows-1.6.3/geoglows/_constants.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_download_decorators.py` & `geoglows-1.6.3/geoglows/_download_decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,30 +23,22 @@
 __all__ = [
     '_forecast',
     '_retrospective',
 ]
 
 
 def _forecast(function):
-    def _river_id_is_iterable(river_id):
-        return bool(
-                isinstance(river_id, list) or
-                isinstance(river_id, tuple) or
-                isinstance(river_id, set) or
-                isinstance(river_id, np.ndarray)
-        )
-
     def from_aws(*args, **kwargs):
         product_name = function.__name__.replace("_", "").lower()
         if product_name == 'forecastrecords':
             warnings.warn('forecast_records are not available from the AWS Open Data Program.')
             return from_rest(*args, **kwargs)
 
         river_id = args[0] if len(args) > 0 else kwargs.get('river_id', None)
-        if river_id is None:
+        if river_id is None and product_name != 'dates':
             raise ValueError('River ID must be provided to retrieve forecast data.')
 
         return_format = kwargs.get('format', 'df')
         assert return_format in ('df', 'xarray'), f'Unsupported return format requested: {return_format}'
 
         if kwargs.get('skip_log', False):
             requests.post(f'{DEFAULT_REST_ENDPOINT}{DEFAULT_REST_ENDPOINT_VERSION}/log',
@@ -122,15 +114,15 @@
 
         version = kwargs.get('version', DEFAULT_REST_ENDPOINT_VERSION)
         assert version in ('v2',), ValueError(f'Unrecognized model version parameter: {version}')
 
         product_name = function.__name__.replace("_", "").lower()
 
         river_id = args[0] if len(args) > 0 else kwargs.get('river_id', None)
-        if river_id is None:
+        if river_id is None and product_name != 'dates':
             raise ValueError('River ID must be provided to retrieve forecast data.')
         if not isinstance(river_id, (int, np.int64, )):
             raise ValueError('Multiple river_ids are not available via REST API. Provide a single 9 digit integer.')
         if river_id and version == 'v2':
             assert 1_000_000_000 > river_id >= 110_000_000, ValueError('River ID must be a 9 digit integer')
 
         # request parameter validation before submitting
```

### Comparing `geoglows-1.6.2/geoglows/_plots/__init__.py` & `geoglows-1.6.3/geoglows/_plots/__init__.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_plots/format_tools.py` & `geoglows-1.6.3/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.6.3/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.6.3/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_plots/plotly_helpers.py` & `geoglows-1.6.3/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.6.3/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/_plots/plots.py` & `geoglows-1.6.3/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/analyze.py` & `geoglows-1.6.3/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/bias.py` & `geoglows-1.6.3/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/data.py` & `geoglows-1.6.3/geoglows/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import warnings
 
 import pandas as pd
 import xarray as xr
 
 from ._constants import get_metadata_table_path
-from ._download_decorators import _forecast, _retrospective
+from ._download_decorators import _forecast, _retrospective, DEFAULT_REST_ENDPOINT, DEFAULT_REST_ENDPOINT_VERSION
 
 from .analyze import (
     daily_averages as calc_daily_averages,
     monthly_averages as calc_monthly_averages,
     annual_averages as calc_annual_averages,
 )
 
@@ -23,14 +23,17 @@
     'retrospective',
     'daily_averages',
     'monthly_averages',
     'annual_averages',
     'return_periods',
 
     'metadata_tables',
+
+    'DEFAULT_REST_ENDPOINT',
+    'DEFAULT_REST_ENDPOINT_VERSION',
 ]
 
 
 # Forecast data and derived products
 @_forecast
 def dates(**kwargs) -> dict or str:
     """
```

### Comparing `geoglows-1.6.2/geoglows/streamflow.py` & `geoglows-1.6.3/geoglows/streamflow.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/streams.py` & `geoglows-1.6.3/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows/tables.py` & `geoglows-1.6.3/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/geoglows.egg-info/PKG-INFO` & `geoglows-1.6.3/geoglows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.6.2
+Version: 1.6.3
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.6.2/geoglows.egg-info/SOURCES.txt` & `geoglows-1.6.3/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.6.2/setup.py` & `geoglows-1.6.3/setup.py`

 * *Files identical despite different names*

