# Comparing `tmp/ci_cloudconnector-1.7.tar.gz` & `tmp/ci_cloudconnector-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-1.7.tar", last modified: Thu May 30 08:24:06 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.8.tar", last modified: Thu May 30 08:37:50 2024, max compression
```

## Comparing `ci_cloudconnector-1.7.tar` & `ci_cloudconnector-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:24:06.983436 ci_cloudconnector-1.7/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:24:06.983436 ci_cloudconnector-1.7/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 08:24:06.000000 ci_cloudconnector-1.7/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 08:24:06.000000 ci_cloudconnector-1.7/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:24:06.000000 ci_cloudconnector-1.7/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 08:24:06.000000 ci_cloudconnector-1.7/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 08:24:06.983436 ci_cloudconnector-1.7/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.7/README.txt
--rw-rw-rw-   0        0        0    38793 2024-05-30 08:23:50.000000 ci_cloudconnector-1.7/logic.py
--rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-1.7/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.7/myservice.py
--rw-rw-rw-   0        0        0      964 2024-05-30 08:23:50.000000 ci_cloudconnector-1.7/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 08:24:06.983436 ci_cloudconnector-1.7/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-30 08:23:54.000000 ci_cloudconnector-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:37:50.244084 ci_cloudconnector-1.8/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:37:50.238695 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:37:50.241604 ci_cloudconnector-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.8/README.txt
+-rw-rw-rw-   0        0        0    39040 2024-05-30 08:37:23.000000 ci_cloudconnector-1.8/logic.py
+-rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-1.8/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.8/myservice.py
+-rw-rw-rw-   0        0        0      964 2024-05-30 08:23:50.000000 ci_cloudconnector-1.8/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:37:50.244084 ci_cloudconnector-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-30 08:37:27.000000 ci_cloudconnector-1.8/setup.py
```

### Comparing `ci_cloudconnector-1.7/logic.py` & `ci_cloudconnector-1.8/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "1.7"
+VER = "1.8"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -872,34 +872,43 @@
         return ans
     except Exception as inst:
         handleError("error reading modbus", inst)
         return fill_Invalids(tags_definitions, ans)
 
 
 # ============================
-def readSimulation_Tags(tagsDefinitions):
+def readSimulation_Tags(tags_definitions):
 
     ans = []
+    arranged_tags = arrange_tags_by_plc(tags_definitions)
+
     ci_print("Start Read readSimulation_Tags", "INFO")
 
+
     try:
-        for tag_def in tagsDefinitions:
-            try:
-                TagId = int(tag_def.get("TagId"))
-                value = random.uniform(-10, 10)
-                time = str(datetime.now(tzlocal.get_localzone()))
-                val = {
-                    "TagId": TagId,
-                    "time": time,
-                    "value": value,
-                    "status": TagStatus.Valid,
-                }
-                ans.append(val)
-            except (ValueError, TypeError) as e:
-                ci_print(f"Error processing tag definition: {e}")
+
+        for plc_address, tags_def_list in arranged_tags.items():
+            for index, tag_def in enumerate(tags_def_list):
+                try:
+                    TagId = int(tag_def.get("TagId"))
+                    value = random.uniform(-10, 10)
+                    time = str(datetime.now(tzlocal.get_localzone()))
+                    val = {
+                        "TagId": TagId,
+                        "time": time,
+                        "value": value,
+                        "status": TagStatus.Valid,
+                    }
+                    ans.append(val)
+                    ci_print(f"plc_address: {plc_address}, TagId: {TagId}, value: {value}")
+
+
+                except (ValueError, TypeError) as e:
+                    ci_print(f"Error processing tag definition: {e}")
+
 
         ci_print("End Read readSimulation_Tags", "INFO")
     except Exception as inst:
         handleError("Error in readSimulation_Tags", inst)
 
     return ans
 
@@ -1115,14 +1124,16 @@
 
         if currentToken == "":
             currentToken = get_cloud_token()
         # currently must get tags from cloud to init server before setting values
         tagsDefScanRatesAns = get_cloud_tags(currentToken)
         tagsDefScanRates = tagsDefScanRatesAns["Tags"]
 
+        ci_print(f'tagsDefScanRates: {tagsDefScanRates}')
+
         for scanRate in tagsDefScanRates:
 
             if scanRate in (None, 'null'):
                 continue
 
             scanRateInt = int(scanRate)
             scanRateStr = str(scanRate)
@@ -1157,19 +1168,17 @@
                                 values = readEtherNetIP_Tags(arranged_tags[connector_type])
                                 if values == []:
                                     time.sleep(1)
                                     ci_print("Ethernet Empty values ::2", "ERROR")
                                     values = readEtherNetIP_Tags(arranged_tags[connector_type])
 
                     if len(values) > 0:
-                        ci_print(f'Value: {values[0]["value"]}, TAGS: {len(values)}', 'INFO')
-                        print(f'ScanRate: {scanRate}, DIFF: {diff}')
+                        ci_print(f'ScanRate: {scanRate}, DIFF: {diff}, Values: {values}')
                     else:
-                        ci_print(f'No Values', 'ERROR')
-                        print(f'ScanRate: {scanRate}, DIFF: {diff}')
+                        ci_print(f'ScanRate: {scanRate}, DIFF: {diff}, No Values')
 
                     if values:
                         saveValuesToFile(values, "")
                         removeOldestFile()
 
                         now = datetime.now()
                         ScanRateLastRead[scanRateStr] = now
```

### Comparing `ci_cloudconnector-1.7/main.py` & `ci_cloudconnector-1.8/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.7/myservice.py` & `ci_cloudconnector-1.8/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.7/myservice_installer.py` & `ci_cloudconnector-1.8/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.7/setup.py` & `ci_cloudconnector-1.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="1.7",
+    version="1.8",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

