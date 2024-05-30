# Comparing `tmp/tesla_fleet_api-0.5.8.tar.gz` & `tmp/tesla_fleet_api-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla_fleet_api-0.5.8.tar", last modified: Sat May 11 22:08:03 2024, max compression
+gzip compressed data, was "tesla_fleet_api-0.5.9.tar", last modified: Sun May 12 01:55:13 2024, max compression
```

## Comparing `tesla_fleet_api-0.5.8.tar` & `tesla_fleet_api-0.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:08:03.728330 tesla_fleet_api-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-11 22:08:03.728330 tesla_fleet_api-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:08:03.728330 tesla_fleet_api-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:08:03.728330 tesla_fleet_api-0.5.8/tesla_fleet_api/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/charging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/energyspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/teslafleetapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/teslafleetoauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/teslemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/tessie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    32835 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-05-11 22:07:51.000000 tesla_fleet_api-0.5.8/tesla_fleet_api/vehiclespecific.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:08:03.728330 tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-11 22:08:03.000000 tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 22:08:03.000000 tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:08:03.000000 tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 22:08:03.000000 tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 22:08:03.000000 tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:13.127649 tesla_fleet_api-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-12 01:55:13.127649 tesla_fleet_api-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 01:55:13.127649 tesla_fleet_api-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:13.127649 tesla_fleet_api-0.5.9/tesla_fleet_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/charging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/energyspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/teslafleetapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/teslafleetoauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/teslemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/tessie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32835 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-05-12 01:55:06.000000 tesla_fleet_api-0.5.9/tesla_fleet_api/vehiclespecific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 01:55:13.127649 tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-12 01:55:13.000000 tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-12 01:55:13.000000 tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 01:55:13.000000 tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 01:55:13.000000 tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 01:55:13.000000 tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/top_level.txt
```

### Comparing `tesla_fleet_api-0.5.8/LICENSE` & `tesla_fleet_api-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/PKG-INFO` & `tesla_fleet_api-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla_fleet_api
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tesla Fleet API library for Python
 Home-page: https://github.com/Teslemetry/tesla_fleet_api
 Author: Brett Adams
 Author-email: admin@teslemetry.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tesla_fleet_api-0.5.8/README.md` & `tesla_fleet_api-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/setup.py` & `tesla_fleet_api-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tesla_fleet_api",
-    version="0.5.8",
+    version="0.5.9",
     author="Brett Adams",
     author_email="admin@teslemetry.com",
     description="Tesla Fleet API library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Teslemetry/tesla_fleet_api",
     packages=setuptools.find_packages(),
```

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/__init__.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/charging.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/charging.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/const.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tesla Fleet API constants."""
 
 from enum import Enum
 import logging
 
-VERSION = "0.5.8"
+VERSION = "0.5.9"
 LOGGER = logging.getLogger(__package__)
 SERVERS = {
     "na": "https://fleet-api.prd.na.vn.cloud.tesla.com",
     "eu": "https://fleet-api.prd.eu.vn.cloud.tesla.com",
     "cn": "https://fleet-api.prd.cn.vn.cloud.tesla.cn",
 }
```

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/energy.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/energy.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/energyspecific.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/energyspecific.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/exceptions.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/partner.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/partner.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/teslafleetapi.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/teslafleetapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,24 @@
         user_scope: bool = True,
         vehicle_scope: bool = True,
     ):
         """Initialize the Tesla Fleet API."""
 
         self.session = session
         self.access_token = access_token
+        self.raise_for_status = raise_for_status
 
-        if region is not None:
-            if not server and region not in SERVERS:
+        if server is not None:
+            self.server = server
+        elif region is not None:
+            if region not in SERVERS:
                 raise ValueError(f"Region must be one of {', '.join(SERVERS.keys())}")
-            self.server = server or SERVERS.get(region)
-        self.raise_for_status = raise_for_status
+            self.server = SERVERS.get(region)
+        else:
+            raise ValueError("Either server or region must be provided.")
 
         LOGGER.debug("Using server %s", self.server)
 
         if charging_scope:
             self.charging = Charging(self)
         if energy_scope:
             self.energy = Energy(self)
```

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/teslafleetoauth.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/teslafleetoauth.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/teslemetry.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/teslemetry.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/tessie.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/tessie.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/user.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/user.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/vehicle.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/vehicle.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api/vehiclespecific.py` & `tesla_fleet_api-0.5.9/tesla_fleet_api/vehiclespecific.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/PKG-INFO` & `tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla_fleet_api
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tesla Fleet API library for Python
 Home-page: https://github.com/Teslemetry/tesla_fleet_api
 Author: Brett Adams
 Author-email: admin@teslemetry.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tesla_fleet_api-0.5.8/tesla_fleet_api.egg-info/SOURCES.txt` & `tesla_fleet_api-0.5.9/tesla_fleet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

