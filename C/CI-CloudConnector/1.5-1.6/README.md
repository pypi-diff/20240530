# Comparing `tmp/ci_cloudconnector-1.5.tar.gz` & `tmp/ci_cloudconnector-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-1.5.tar", last modified: Thu May 30 08:08:05 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.6.tar", last modified: Thu May 30 08:13:14 2024, max compression
```

## Comparing `ci_cloudconnector-1.5.tar` & `ci_cloudconnector-1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:08:05.755113 ci_cloudconnector-1.5/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:08:05.748658 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 08:08:05.751436 ci_cloudconnector-1.5/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.5/README.txt
--rw-rw-rw-   0        0        0    38737 2024-05-30 08:04:41.000000 ci_cloudconnector-1.5/logic.py
--rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-1.5/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.5/myservice.py
--rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.5/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 08:08:05.755113 ci_cloudconnector-1.5/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-30 08:04:47.000000 ci_cloudconnector-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:13:14.319944 ci_cloudconnector-1.6/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:13:14.312420 ci_cloudconnector-1.6/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:13:14.000000 ci_cloudconnector-1.6/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 08:13:14.000000 ci_cloudconnector-1.6/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:13:14.000000 ci_cloudconnector-1.6/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 08:13:14.000000 ci_cloudconnector-1.6/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:13:14.312420 ci_cloudconnector-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.6/README.txt
+-rw-rw-rw-   0        0        0    38793 2024-05-30 08:12:49.000000 ci_cloudconnector-1.6/logic.py
+-rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-1.6/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.6/myservice.py
+-rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.6/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:13:14.319944 ci_cloudconnector-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-30 08:13:00.000000 ci_cloudconnector-1.6/setup.py
```

### Comparing `ci_cloudconnector-1.5/logic.py` & `ci_cloudconnector-1.6/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "1.5"
+VER = "1.6"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -875,14 +875,15 @@
         return fill_Invalids(tags_definitions, ans)
 
 
 # ============================
 def readSimulation_Tags(tagsDefinitions):
 
     ans = []
+    ci_print("Start Read readSimulation_Tags", "INFO")
 
     try:
         for tag_def in tagsDefinitions:
             try:
                 TagId = int(tag_def.get("TagId"))
                 value = random.uniform(-10, 10)
                 time = str(datetime.now(tzlocal.get_localzone()))
@@ -1156,18 +1157,18 @@
                                 values = readEtherNetIP_Tags(arranged_tags[connector_type])
                                 if values == []:
                                     time.sleep(1)
                                     ci_print("Ethernet Empty values ::2", "ERROR")
                                     values = readEtherNetIP_Tags(arranged_tags[connector_type])
 
                     if len(values) > 0:
-                        ci_print(f'VALUE: {values[0]["value"]}, TAGS: {len(values)}', 'INFO')
+                        ci_print(f'Value: {values[0]["value"]}, TAGS: {len(values)}', 'INFO')
                         print(f'ScanRate: {scanRate}, DIFF: {diff}')
                     else:
-                        ci_print(f'NO VALUES', 'ERROR')
+                        ci_print(f'No Values', 'ERROR')
                         print(f'ScanRate: {scanRate}, DIFF: {diff}')
 
                     if values:
                         saveValuesToFile(values, "")
                         removeOldestFile()
 
                         now = datetime.now()
```

### Comparing `ci_cloudconnector-1.5/main.py` & `ci_cloudconnector-1.6/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.5/myservice.py` & `ci_cloudconnector-1.6/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.5/setup.py` & `ci_cloudconnector-1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="1.5",
+    version="1.6",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

