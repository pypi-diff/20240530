# Comparing `tmp/pyrestcountries-2024.5.3.tar.gz` & `tmp/pyrestcountries-2024.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestcountries-2024.5.3.tar", last modified: Fri May  3 07:40:23 2024, max compression
+gzip compressed data, was "pyrestcountries-2024.5.30.tar", last modified: Thu May 30 05:41:34 2024, max compression
```

## Comparing `pyrestcountries-2024.5.3.tar` & `pyrestcountries-2024.5.30.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-03 07:40:23.662501 pyrestcountries-2024.5.3/
--rw-r--r--   0 gkoduri    (502) staff       (20)    34523 2024-04-29 10:32:24.000000 pyrestcountries-2024.5.3/LICENSE
--rw-r--r--   0 gkoduri    (502) staff       (20)     8347 2024-05-03 07:40:23.662218 pyrestcountries-2024.5.3/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)     7085 2024-05-03 07:39:17.000000 pyrestcountries-2024.5.3/README.md
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-03 07:40:23.659584 pyrestcountries-2024.5.3/pyrestcountries/
--rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-29 10:53:48.000000 pyrestcountries-2024.5.3/pyrestcountries/__init__.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     5264 2024-05-03 04:41:54.000000 pyrestcountries-2024.5.3/pyrestcountries/api.py
--rw-r--r--   0 gkoduri    (502) staff       (20)     2950 2024-04-29 11:33:15.000000 pyrestcountries-2024.5.3/pyrestcountries/data.py
-drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-03 07:40:23.661934 pyrestcountries-2024.5.3/pyrestcountries.egg-info/
--rw-r--r--   0 gkoduri    (502) staff       (20)     8347 2024-05-03 07:40:23.000000 pyrestcountries-2024.5.3/pyrestcountries.egg-info/PKG-INFO
--rw-r--r--   0 gkoduri    (502) staff       (20)      295 2024-05-03 07:40:23.000000 pyrestcountries-2024.5.3/pyrestcountries.egg-info/SOURCES.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-05-03 07:40:23.000000 pyrestcountries-2024.5.3/pyrestcountries.egg-info/dependency_links.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       35 2024-05-03 07:40:23.000000 pyrestcountries-2024.5.3/pyrestcountries.egg-info/requires.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       16 2024-05-03 07:40:23.000000 pyrestcountries-2024.5.3/pyrestcountries.egg-info/top_level.txt
--rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-05-03 07:40:23.662547 pyrestcountries-2024.5.3/setup.cfg
--rw-r--r--   0 gkoduri    (502) staff       (20)     1448 2024-05-03 07:40:03.000000 pyrestcountries-2024.5.3/setup.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-30 05:41:34.084689 pyrestcountries-2024.5.30/
+-rw-r--r--   0 gkoduri    (502) staff       (20)    34523 2024-04-29 10:32:24.000000 pyrestcountries-2024.5.30/LICENSE
+-rw-r--r--   0 gkoduri    (502) staff       (20)     8348 2024-05-30 05:41:34.084464 pyrestcountries-2024.5.30/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)     7085 2024-05-03 07:39:17.000000 pyrestcountries-2024.5.30/README.md
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-30 05:41:34.082416 pyrestcountries-2024.5.30/pyrestcountries/
+-rw-r--r--   0 gkoduri    (502) staff       (20)        0 2024-04-29 10:53:48.000000 pyrestcountries-2024.5.30/pyrestcountries/__init__.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     5453 2024-05-30 05:40:57.000000 pyrestcountries-2024.5.30/pyrestcountries/api.py
+-rw-r--r--   0 gkoduri    (502) staff       (20)     2950 2024-04-29 11:33:15.000000 pyrestcountries-2024.5.30/pyrestcountries/data.py
+drwxr-xr-x   0 gkoduri    (502) staff       (20)        0 2024-05-30 05:41:34.084189 pyrestcountries-2024.5.30/pyrestcountries.egg-info/
+-rw-r--r--   0 gkoduri    (502) staff       (20)     8348 2024-05-30 05:41:34.000000 pyrestcountries-2024.5.30/pyrestcountries.egg-info/PKG-INFO
+-rw-r--r--   0 gkoduri    (502) staff       (20)      295 2024-05-30 05:41:34.000000 pyrestcountries-2024.5.30/pyrestcountries.egg-info/SOURCES.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)        1 2024-05-30 05:41:34.000000 pyrestcountries-2024.5.30/pyrestcountries.egg-info/dependency_links.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       35 2024-05-30 05:41:34.000000 pyrestcountries-2024.5.30/pyrestcountries.egg-info/requires.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       16 2024-05-30 05:41:34.000000 pyrestcountries-2024.5.30/pyrestcountries.egg-info/top_level.txt
+-rw-r--r--   0 gkoduri    (502) staff       (20)       38 2024-05-30 05:41:34.084731 pyrestcountries-2024.5.30/setup.cfg
+-rw-r--r--   0 gkoduri    (502) staff       (20)     1448 2024-05-30 05:41:30.000000 pyrestcountries-2024.5.30/setup.py
```

### Comparing `pyrestcountries-2024.5.3/LICENSE` & `pyrestcountries-2024.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestcountries-2024.5.3/PKG-INFO` & `pyrestcountries-2024.5.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestcountries
-Version: 2024.5.3
+Version: 2024.5.30
 Summary: Pythonic wrapper around data served by restcountries API
 Home-page: https://github.com/musicmuni/pyrestcountries
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
 Project-URL: Documentation, https://github.com/musicmuni/pyrestcountries
 Project-URL: Source, https://github.com/musicmuni/pyrestcountries
 Project-URL: Tracker, https://github.com/musicmuni/pyrestcountries/issues
```

### Comparing `pyrestcountries-2024.5.3/README.md` & `pyrestcountries-2024.5.30/README.md`

 * *Files identical despite different names*

### Comparing `pyrestcountries-2024.5.3/pyrestcountries/api.py` & `pyrestcountries-2024.5.30/pyrestcountries/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
+import time
 
 import appdirs
 import requests
-from .data import *
 from diskcache import Cache
 from thefuzz import fuzz, process
 
+from .data import *
+
 
 class RestCountriesAPI:
     BASE_URL = "https://restcountries.com/v3.1"
 
     # caching to make sure we don't poll API for every request
     # declaring outside init so that this cache is shared across instances of this class
     cache_dir = appdirs.user_cache_dir("restcountries")
@@ -35,29 +37,29 @@
             all_names.update(translation.get("common", "").lower() for translation in country["translations"].values())
             all_names.update(
                 translation.get("official", "").lower() for translation in country["translations"].values()
             )
             self.country_iso2_to_names_map[iso2] = all_names
 
     def update_countries_cache(self):
-        """Fetches all country data from the API and caches it, using ETag to check for changes."""
-        headers = {}
-        etag = self.cache.get("etag")
-
-        if etag:
-            headers["If-None-Match"] = etag
-
-        response = requests.get(f"{self.BASE_URL}/all", headers=headers)
-
-        if response.status_code == 304:
-            print("Data has not changed since the last fetch. Using cached data...")
-            return  # Data in cache is still up to date
+        """Fetches all country data from the API and caches it, using max-age to determine expiration."""
+        cache_expiration = self.cache.get("cache_expiration")
+        current_time = time.time()
+
+        if cache_expiration and current_time < cache_expiration:
+            print("Using cached data...")
+            return  # Data in cache is still valid based on max-age
+
+        response = requests.get(f"{self.BASE_URL}/all")
         if response.status_code == 200:
-            print("Updating cache as data changed on remote...")
-            self.cache.set("etag", response.headers.get("ETag"))
+            print("Updating cache as data fetched from remote...")
+            # Calculate new expiration time based on max-age
+            max_age = int(response.headers.get("Cache-Control").split("max-age=")[1].split(",")[0])
+            cache_expiration = current_time + max_age
+            self.cache.set("cache_expiration", cache_expiration)
             self.cache.set("countries_data", response.json())
         else:
             response.raise_for_status()
 
     def close_cache(self):
         """Close the cache properly."""
         self.cache.close()
```

### Comparing `pyrestcountries-2024.5.3/pyrestcountries/data.py` & `pyrestcountries-2024.5.30/pyrestcountries/data.py`

 * *Files identical despite different names*

### Comparing `pyrestcountries-2024.5.3/pyrestcountries.egg-info/PKG-INFO` & `pyrestcountries-2024.5.30/pyrestcountries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestcountries
-Version: 2024.5.3
+Version: 2024.5.30
 Summary: Pythonic wrapper around data served by restcountries API
 Home-page: https://github.com/musicmuni/pyrestcountries
 Author: Gopala Krishna Koduri
 Author-email: gopal@riyazapp.com
 Project-URL: Documentation, https://github.com/musicmuni/pyrestcountries
 Project-URL: Source, https://github.com/musicmuni/pyrestcountries
 Project-URL: Tracker, https://github.com/musicmuni/pyrestcountries/issues
```

### Comparing `pyrestcountries-2024.5.3/setup.py` & `pyrestcountries-2024.5.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyrestcountries",
-    version="2024.05.03",
+    version="2024.05.30",
     description="Pythonic wrapper around data served by restcountries API",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Gopala Krishna Koduri",
     author_email="gopal@riyazapp.com",
     url="https://github.com/musicmuni/pyrestcountries",
     packages=find_packages(),
```

