# Comparing `tmp/dwd_global_radiation-1.1.0rc2.tar.gz` & `tmp/dwd_global_radiation-1.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.1.0rc2.tar", last modified: Wed May 29 21:12:15 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.1.0rc3.tar", last modified: Wed May 29 22:25:11 2024, max compression
```

## Comparing `dwd_global_radiation-1.1.0rc2.tar` & `dwd_global_radiation-1.1.0rc3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:12:15.049955 dwd_global_radiation-1.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22430 2024-05-29 21:12:15.049955 dwd_global_radiation-1.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21423 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:12:15.047955 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27369 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 root         (0) root         (0)     7298 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation_printer.py
--rw-r--r--   0 root         (0) root         (0)    20227 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 21:12:15.048955 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22430 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      128 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 21:12:15.000000 dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 21:12:15.049955 dwd_global_radiation-1.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1656 2024-05-29 21:10:36.000000 dwd_global_radiation-1.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:25:11.924302 dwd_global_radiation-1.1.0rc3/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22371 2024-05-29 22:25:11.924302 dwd_global_radiation-1.1.0rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21423 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:25:11.922302 dwd_global_radiation-1.1.0rc3/dwd_global_radiation/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27369 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation/global_radiation_printer.py
+-rw-r--r--   0 root         (0) root         (0)    20227 2024-05-29 20:29:12.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 22:25:11.923303 dwd_global_radiation-1.1.0rc3/dwd_global_radiation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22371 2024-05-29 22:25:11.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-29 22:25:11.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 22:25:11.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-29 22:25:11.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 22:25:11.000000 dwd_global_radiation-1.1.0rc3/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      977 2024-05-29 22:25:11.924302 dwd_global_radiation-1.1.0rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-29 22:16:46.000000 dwd_global_radiation-1.1.0rc3/setup.py
```

### Comparing `dwd_global_radiation-1.1.0rc2/LICENSE` & `dwd_global_radiation-1.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc2/PKG-INFO` & `dwd_global_radiation-1.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,16 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: netCDF4>=1.6.5
-Requires-Dist: numpy>=1.26.0
 Requires-Dist: pytz>=2024.1
 Requires-Dist: requests>=2.31.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tzlocal>=5.2
 Requires-Dist: xarray>=2024.3.0
 
 DISCLAIMER: This project is a private open source project and is not affiliated with the German public meteorology service institute "Deutscher Wetterdienst" (DWD). However, it uses its publicly available data interfaces.
```

### Comparing `dwd_global_radiation-1.1.0rc2/README.md` & `dwd_global_radiation-1.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.1.0rc3/dwd_global_radiation/global_radiation.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc2/dwd_global_radiation/global_radiation_printer.py` & `dwd_global_radiation-1.1.0rc3/dwd_global_radiation/global_radiation_printer.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc2/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.1.0rc3/dwd_global_radiation/utils.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc2/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.1.0rc3/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.1.0rc2
+Version: 1.1.0rc3
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,16 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: beautifulsoup4>=4.12.3
-Requires-Dist: netCDF4>=1.6.5
-Requires-Dist: numpy>=1.26.0
 Requires-Dist: pytz>=2024.1
 Requires-Dist: requests>=2.31.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tzlocal>=5.2
 Requires-Dist: xarray>=2024.3.0
 
 DISCLAIMER: This project is a private open source project and is not affiliated with the German public meteorology service institute "Deutscher Wetterdienst" (DWD). However, it uses its publicly available data interfaces.
```

