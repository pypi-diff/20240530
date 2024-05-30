# Comparing `tmp/consmodel-0.1.6.tar.gz` & `tmp/consmodel-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consmodel-0.1.6.tar", last modified: Wed Feb 14 13:55:35 2024, max compression
+gzip compressed data, was "consmodel-0.1.7.tar", last modified: Thu May 30 10:14:39 2024, max compression
```

## Comparing `consmodel-0.1.6.tar` & `consmodel-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-02-14 13:55:35.345398 consmodel-0.1.6/
-drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-02-14 13:55:35.344825 consmodel-0.1.6/ConsModel.egg-info/
--rw-r--r--   0 blazdobravec   (501) staff       (20)     4969 2024-02-14 13:55:35.000000 consmodel-0.1.6/ConsModel.egg-info/PKG-INFO
--rw-r--r--   0 blazdobravec   (501) staff       (20)      651 2024-02-14 13:55:35.000000 consmodel-0.1.6/ConsModel.egg-info/SOURCES.txt
--rw-r--r--   0 blazdobravec   (501) staff       (20)        1 2024-02-14 13:55:35.000000 consmodel-0.1.6/ConsModel.egg-info/dependency_links.txt
--rw-r--r--   0 blazdobravec   (501) staff       (20)      182 2024-02-14 13:55:35.000000 consmodel-0.1.6/ConsModel.egg-info/requires.txt
--rw-r--r--   0 blazdobravec   (501) staff       (20)       10 2024-02-14 13:55:35.000000 consmodel-0.1.6/ConsModel.egg-info/top_level.txt
--rw-r--r--   0 blazdobravec   (501) staff       (20)     1068 2023-09-29 00:56:26.000000 consmodel-0.1.6/LICENCE.txt
--rw-r--r--   0 blazdobravec   (501) staff       (20)     4969 2024-02-14 13:55:35.345163 consmodel-0.1.6/PKG-INFO
--rw-r--r--   0 blazdobravec   (501) staff       (20)     4063 2023-11-15 07:55:03.000000 consmodel-0.1.6/README.md
-drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-02-14 13:55:35.340421 consmodel-0.1.6/consmodel/
--rw-r--r--   0 blazdobravec   (501) staff       (20)      163 2024-01-03 10:16:03.000000 consmodel-0.1.6/consmodel/__init__.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)      164 2023-12-27 13:30:02.000000 consmodel-0.1.6/consmodel/ac_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)     6315 2024-02-14 13:53:48.000000 consmodel-0.1.6/consmodel/base_model.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)    18853 2024-01-26 10:01:29.000000 consmodel-0.1.6/consmodel/bs_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)    10258 2023-12-27 15:10:43.000000 consmodel-0.1.6/consmodel/cons_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)       96 2023-12-27 13:30:02.000000 consmodel-0.1.6/consmodel/ev_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)     3888 2024-02-14 12:23:15.000000 consmodel-0.1.6/consmodel/hp_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)    22142 2024-02-14 13:50:27.000000 consmodel-0.1.6/consmodel/pv_sim.py
-drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-02-14 13:55:35.342389 consmodel-0.1.6/consmodel/utils/
--rw-r--r--   0 blazdobravec   (501) staff       (20)        0 2023-10-01 21:46:56.000000 consmodel-0.1.6/consmodel/utils/__init__.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)     5007 2024-02-14 11:20:48.000000 consmodel-0.1.6/consmodel/utils/st_types.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)      267 2023-11-06 22:49:00.000000 consmodel-0.1.6/pyproject.toml
--rw-r--r--   0 blazdobravec   (501) staff       (20)       38 2024-02-14 13:55:35.345440 consmodel-0.1.6/setup.cfg
--rw-r--r--   0 blazdobravec   (501) staff       (20)     1094 2024-02-14 13:55:06.000000 consmodel-0.1.6/setup.py
-drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-02-14 13:55:35.344294 consmodel-0.1.6/tests/
--rw-r--r--   0 blazdobravec   (501) staff       (20)     3372 2024-02-02 06:34:51.000000 consmodel-0.1.6/tests/test_bs_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)     2431 2024-01-03 11:02:23.000000 consmodel-0.1.6/tests/test_cons_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)      516 2024-02-14 13:43:03.000000 consmodel-0.1.6/tests/test_hp_sim.py
--rw-r--r--   0 blazdobravec   (501) staff       (20)     1272 2024-02-14 12:46:13.000000 consmodel-0.1.6/tests/test_pv_sim.py
+drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-05-30 10:14:39.010872 consmodel-0.1.7/
+drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-05-30 10:14:39.010132 consmodel-0.1.7/ConsModel.egg-info/
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     4969 2024-05-30 10:14:38.000000 consmodel-0.1.7/ConsModel.egg-info/PKG-INFO
+-rw-r--r--   0 blazdobravec   (501) staff       (20)      651 2024-05-30 10:14:39.000000 consmodel-0.1.7/ConsModel.egg-info/SOURCES.txt
+-rw-r--r--   0 blazdobravec   (501) staff       (20)        1 2024-05-30 10:14:38.000000 consmodel-0.1.7/ConsModel.egg-info/dependency_links.txt
+-rw-r--r--   0 blazdobravec   (501) staff       (20)      182 2024-05-30 10:14:38.000000 consmodel-0.1.7/ConsModel.egg-info/requires.txt
+-rw-r--r--   0 blazdobravec   (501) staff       (20)       10 2024-05-30 10:14:38.000000 consmodel-0.1.7/ConsModel.egg-info/top_level.txt
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     1068 2023-09-29 00:56:26.000000 consmodel-0.1.7/LICENCE.txt
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     4969 2024-05-30 10:14:39.010440 consmodel-0.1.7/PKG-INFO
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     4063 2023-11-15 07:55:03.000000 consmodel-0.1.7/README.md
+drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-05-30 10:14:39.007251 consmodel-0.1.7/consmodel/
+-rw-r--r--   0 blazdobravec   (501) staff       (20)      163 2024-01-03 10:16:03.000000 consmodel-0.1.7/consmodel/__init__.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)      164 2023-12-27 13:30:02.000000 consmodel-0.1.7/consmodel/ac_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     6600 2024-05-30 10:13:06.000000 consmodel-0.1.7/consmodel/base_model.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)    18853 2024-01-26 10:01:29.000000 consmodel-0.1.7/consmodel/bs_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)    10258 2023-12-27 15:10:43.000000 consmodel-0.1.7/consmodel/cons_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)       96 2023-12-27 13:30:02.000000 consmodel-0.1.7/consmodel/ev_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     3888 2024-02-14 12:23:15.000000 consmodel-0.1.7/consmodel/hp_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)    22142 2024-02-14 13:50:27.000000 consmodel-0.1.7/consmodel/pv_sim.py
+drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-05-30 10:14:39.008703 consmodel-0.1.7/consmodel/utils/
+-rw-r--r--   0 blazdobravec   (501) staff       (20)        0 2023-10-01 21:46:56.000000 consmodel-0.1.7/consmodel/utils/__init__.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     5007 2024-02-14 11:20:48.000000 consmodel-0.1.7/consmodel/utils/st_types.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)      267 2023-11-06 22:49:00.000000 consmodel-0.1.7/pyproject.toml
+-rw-r--r--   0 blazdobravec   (501) staff       (20)       38 2024-05-30 10:14:39.010937 consmodel-0.1.7/setup.cfg
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     1094 2024-05-30 10:14:31.000000 consmodel-0.1.7/setup.py
+drwxr-xr-x   0 blazdobravec   (501) staff       (20)        0 2024-05-30 10:14:39.009787 consmodel-0.1.7/tests/
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     3372 2024-02-02 06:34:51.000000 consmodel-0.1.7/tests/test_bs_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     2431 2024-01-03 11:02:23.000000 consmodel-0.1.7/tests/test_cons_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)      516 2024-05-30 10:12:56.000000 consmodel-0.1.7/tests/test_hp_sim.py
+-rw-r--r--   0 blazdobravec   (501) staff       (20)     1272 2024-02-14 12:46:13.000000 consmodel-0.1.7/tests/test_pv_sim.py
```

### Comparing `consmodel-0.1.6/ConsModel.egg-info/PKG-INFO` & `consmodel-0.1.7/ConsModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consmodel
-Version: 0.1.6
+Version: 0.1.7
 Summary: The library aims to provide a simple way to create individual consumer loads, generation.
 Home-page: https://github.com/blazdob/consmodel
 Author: Blaž Dobravec
 Author-email: blaz@dobravec.si
 Project-URL: Bug Tracker, https://github.com/blazdob/consmodel/issue
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `consmodel-0.1.6/ConsModel.egg-info/SOURCES.txt` & `consmodel-0.1.7/ConsModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/LICENCE.txt` & `consmodel-0.1.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/PKG-INFO` & `consmodel-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consmodel
-Version: 0.1.6
+Version: 0.1.7
 Summary: The library aims to provide a simple way to create individual consumer loads, generation.
 Home-page: https://github.com/blazdob/consmodel
 Author: Blaž Dobravec
 Author-email: blaz@dobravec.si
 Project-URL: Bug Tracker, https://github.com/blazdob/consmodel/issue
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `consmodel-0.1.6/README.md` & `consmodel-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/consmodel/base_model.py` & `consmodel-0.1.7/consmodel/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,22 @@
                 coco ... The weather condition code
         """
         # round the start to the nearest hour
         start = start.replace(minute=0, second=0, microsecond=0)
 
         # if end is over an hour then round up to the next hour
         if end.minute > 0 or end.second > 0 or end.microsecond > 0:
-            end = end.replace(hour=end.hour + 1,
+            if end.hour == 23:
+                end = end.replace(hour=0,
+                                  minute=0,
+                                  second=0,
+                                  microsecond=0)
+                end = end.replace(year=end.year + 1)
+            else:
+                end = end.replace(hour=end.hour + 1,
                               minute=0,
                               second=0,
                               microsecond=0)
 
         location = Point(self.lat, self.lon, self.alt)
         weather_data = Hourly(location, start, end, self.tz)
         weather_data = weather_data.fetch()
```

### Comparing `consmodel-0.1.6/consmodel/bs_sim.py` & `consmodel-0.1.7/consmodel/bs_sim.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/consmodel/cons_sim.py` & `consmodel-0.1.7/consmodel/cons_sim.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/consmodel/hp_sim.py` & `consmodel-0.1.7/consmodel/hp_sim.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/consmodel/pv_sim.py` & `consmodel-0.1.7/consmodel/pv_sim.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/consmodel/utils/st_types.py` & `consmodel-0.1.7/consmodel/utils/st_types.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/setup.py` & `consmodel-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="consmodel",
-    version="0.1.6",
+    version="0.1.7",
     author="Blaž Dobravec",
     author_email="blaz@dobravec.si",
     description=
     "The library aims to provide a simple way to create individual consumer loads, generation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/blazdob/consmodel",
```

### Comparing `consmodel-0.1.6/tests/test_bs_sim.py` & `consmodel-0.1.7/tests/test_bs_sim.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/tests/test_cons_sim.py` & `consmodel-0.1.7/tests/test_cons_sim.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/tests/test_hp_sim.py` & `consmodel-0.1.7/tests/test_hp_sim.py`

 * *Files identical despite different names*

### Comparing `consmodel-0.1.6/tests/test_pv_sim.py` & `consmodel-0.1.7/tests/test_pv_sim.py`

 * *Files identical despite different names*

