# Comparing `tmp/dwd_global_radiation-1.1.0rc1.tar.gz` & `tmp/dwd_global_radiation-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.1.0rc1.tar", last modified: Tue May 28 12:14:21 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.1.0rc2.tar", last modified: Wed May 29 21:12:15 2024, max compression
```

## Comparing `dwd_global_radiation-1.1.0rc1.tar` & `dwd_global_radiation-1.1.0rc2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.1.0rc1/LICENSE
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-21 10:47:19.000000 dwd_global_radiation-1.1.0rc1/README.md
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-27 15:10:26.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/__init__.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    27371 2024-05-28 11:59:54.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     7298 2024-05-28 11:57:05.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/global_radiation_printer.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    20227 2024-05-28 11:57:05.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation/utils.py
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      398 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-28 12:14:21.000000 dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-28 12:14:21.239580 dwd_global_radiation-1.1.0rc1/setup.cfg
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-28 11:57:22.000000 dwd_global_radiation-1.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:12:15.049955 dwd_global_radiation-1.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22430 2024-05-29 21:12:15.049955 dwd_global_radiation-1.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21423 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:12:15.047955 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27369 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation_printer.py
+-rw-r--r--   0 root         (0) root         (0)    20227 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:12:15.048955 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22430 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 21:12:15.049955 dwd_global_radiation-1.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1656 2024-05-29 21:10:36.000000 dwd_global_radiation-1.1.0rc2/setup.py
```

### Comparing `dwd_global_radiation-1.1.0rc1/LICENSE` & `dwd_global_radiation-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc1/PKG-INFO` & `dwd_global_radiation-1.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.1.0rc1/README.md` & `dwd_global_radiation-1.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc1/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         }
 
     def add_measurement_value(self, timestamp, sis):
         """Method for adding retrieved measurement values as SIS."""
         if not any(entry.timestamp == timestamp for entry in self.measurement_values):
             self.measurement_values.append(MeasurementEntry(timestamp, sis))
         else:
-            _LOGGER.warning(
+            _LOGGER.debug(
                 "Duplicate timestamp %s found. Measurement value not added.", timestamp
             )
 
     def get_measurement_values(self):
         """Method to retrieve all measurement values"""
         return self.measurement_values
```

### Comparing `dwd_global_radiation-1.1.0rc1/dwd_global_radiation/global_radiation_printer.py` & `dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation_printer.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc1/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.1.0rc2/dwd_global_radiation/utils.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc1/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.1.0rc1/setup.py` & `dwd_global_radiation-1.1.0rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dwd_global_radiation',
-    version='1.1.0rc1',
+    version='1.1.0rc2',
     packages=find_packages(),
     description='Access and analyze DWD global radiation data and forecasts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aschmere/dwd_global_radiation',
     author='Arno Schmerer',
     license='MIT',
```

