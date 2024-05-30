# Comparing `tmp/corebridge-0.2.7.tar.gz` & `tmp/corebridge-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.2.7.tar", last modified: Thu May 30 10:01:43 2024, max compression
+gzip compressed data, was "corebridge-0.2.8.tar", last modified: Thu May 30 10:19:36 2024, max compression
```

## Comparing `corebridge-0.2.7.tar` & `corebridge-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:01:43.245618 corebridge-0.2.7/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.7/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.7/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-30 10:01:43.245618 corebridge-0.2.7/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)     2417 2024-05-27 09:35:23.000000 corebridge-0.2.7/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:01:43.245618 corebridge-0.2.7/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     5133 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     4377 2024-05-30 10:01:32.000000 corebridge-0.2.7/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:01:43.245618 corebridge-0.2.7/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.7/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      287 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-30 10:01:43.000000 corebridge-0.2.7/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1208 2024-05-30 09:54:45.000000 corebridge-0.2.7/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-30 10:01:43.245618 corebridge-0.2.7/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.7/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:19:36.098584 corebridge-0.2.8/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.8/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.8/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-30 10:19:36.098584 corebridge-0.2.8/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     2417 2024-05-27 09:35:23.000000 corebridge-0.2.8/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:19:36.098584 corebridge-0.2.8/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-30 10:19:06.000000 corebridge-0.2.8/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-30 10:19:06.000000 corebridge-0.2.8/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     5133 2024-05-30 10:19:06.000000 corebridge-0.2.8/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4181 2024-05-30 10:19:06.000000 corebridge-0.2.8/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-30 10:19:36.098584 corebridge-0.2.8/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     3185 2024-05-30 10:19:36.000000 corebridge-0.2.8/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-30 10:19:36.000000 corebridge-0.2.8/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-30 10:19:36.000000 corebridge-0.2.8/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-30 10:19:36.000000 corebridge-0.2.8/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.8/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      287 2024-05-30 10:19:36.000000 corebridge-0.2.8/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-30 10:19:36.000000 corebridge-0.2.8/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1208 2024-05-30 10:18:45.000000 corebridge-0.2.8/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-30 10:19:36.098584 corebridge-0.2.8/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.8/setup.py
```

### Comparing `corebridge-0.2.7/LICENSE` & `corebridge-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.7/PKG-INFO` & `corebridge-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.7
+Version: 0.2.8
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.7/README.md` & `corebridge-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.7/corebridge/_modidx.py` & `corebridge-0.2.8/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.7/corebridge/aicorebridge.py` & `corebridge-0.2.8/corebridge/aicorebridge.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.7/corebridge/core.py` & `corebridge-0.2.8/corebridge/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['timeseries_dataframe', 'set_time_index_zone', 'timeseries_dataframe_from_datadict',
+__all__ = ['set_time_index_zone', 'timeseries_dataframe', 'timeseries_dataframe_from_datadict',
            'timeseries_dataframe_to_datadict']
 
 # %% ../nbs/00_core.ipynb 3
 import typing
 import os
 import numpy as np
 import pandas as pd
@@ -13,14 +13,26 @@
 # %% ../nbs/00_core.ipynb 4
 try:
     print(f"Loading {__name__} from {__file__}")
 except:
     pass
 
 # %% ../nbs/00_core.ipynb 6
+def set_time_index_zone(df:pd.DataFrame, timezone):
+
+    df.index.name = 'time'
+    if not hasattr(df.index, 'tz'):
+        df.index = df.index.tz_localize('UTC').tz_convert(timezone)
+    elif str(df.index.tz) != timezone:
+        df.index = df.index.tz_convert(timezone)
+
+    return df
+
+
+# %% ../nbs/00_core.ipynb 7
 def timeseries_dataframe(
         data:typing.Union[pd.DataFrame, pd.Series, dict, np.ndarray, np.recarray], 
         timezone='UTC', 
         columnnames=None):
     
     """Convert various data formats to timeseries DataFrame"""
 
@@ -58,34 +70,16 @@
                 data=data[:, 1:],
                 index=pd.DatetimeIndex(data[:,0]*1e9),
                 columns=columns
             )
         else:
             return pd.DataFrame()
 
-    df.index.name = 'time'
-    if not df.index.tz:
-        df.index = df.index.tz_localize('UTC').tz_convert(timezone)
-    elif str(df.index.tz) != timezone:
-        df.index = df.index.tz_convert(timezone)
-
     return set_time_index_zone(df, timezone)
 
-# %% ../nbs/00_core.ipynb 7
-def set_time_index_zone(df:pd.DataFrame, timezone):
-
-    df.index.name = 'time'
-    if not df.index.tz:
-        df.index = df.index.tz_localize('UTC').tz_convert(timezone)
-    elif str(df.index.tz) != timezone:
-        df.index = df.index.tz_convert(timezone)
-
-    return df
-
-
 # %% ../nbs/00_core.ipynb 8
 def timeseries_dataframe_from_datadict(
         data:dict, 
         timecolumns,
         recordformat='records'):
         
     "Convert data dict to dataframe"
```

### Comparing `corebridge-0.2.7/corebridge.egg-info/PKG-INFO` & `corebridge-0.2.8/corebridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.7
+Version: 0.2.8
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.7/settings.ini` & `corebridge-0.2.8/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.2.7
+version = 0.2.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
```

### Comparing `corebridge-0.2.7/setup.py` & `corebridge-0.2.8/setup.py`

 * *Files identical despite different names*

