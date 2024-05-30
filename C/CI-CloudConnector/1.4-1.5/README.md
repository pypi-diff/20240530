# Comparing `tmp/ci_cloudconnector-1.4.tar.gz` & `tmp/ci_cloudconnector-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-1.4.tar", last modified: Thu May 30 07:59:22 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.5.tar", last modified: Thu May 30 08:08:05 2024, max compression
```

## Comparing `ci_cloudconnector-1.4.tar` & `ci_cloudconnector-1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:59:22.190848 ci_cloudconnector-1.4/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:59:22.183235 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 07:59:22.187525 ci_cloudconnector-1.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.4/README.txt
--rw-rw-rw-   0        0        0    38751 2024-05-30 07:55:54.000000 ci_cloudconnector-1.4/logic.py
--rw-rw-rw-   0        0        0     8301 2024-05-30 07:45:13.000000 ci_cloudconnector-1.4/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.4/myservice.py
--rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.4/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 07:59:22.191345 ci_cloudconnector-1.4/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-30 07:56:01.000000 ci_cloudconnector-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:08:05.755113 ci_cloudconnector-1.5/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:08:05.748658 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 08:08:05.000000 ci_cloudconnector-1.5/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:08:05.751436 ci_cloudconnector-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.5/README.txt
+-rw-rw-rw-   0        0        0    38737 2024-05-30 08:04:41.000000 ci_cloudconnector-1.5/logic.py
+-rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-1.5/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.5/myservice.py
+-rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.5/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:08:05.755113 ci_cloudconnector-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-30 08:04:47.000000 ci_cloudconnector-1.5/setup.py
```

### Comparing `ci_cloudconnector-1.4/logic.py` & `ci_cloudconnector-1.5/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "1.4"
+VER = "1.5"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -201,14 +201,15 @@
 
             initialize_log(log_level)
 
             ci_print(f"Server Address: {cfg_server_address}", "INFO")
             ci_print(f"Username: {cfg_username}", "INFO")
             ci_print(f"Password: {cfg_password}", "INFO")
             ci_print(f"Max Files: {cfg_max_files}", "INFO")
+            ci_print(f"VERSION: {getLocalVersion()}")
 
         else:
             ci_print(f"Config not found or overwrite is True, creating new one in {file_path}", "INFO")
             config = configparser.ConfigParser()
             config.add_section("Server")
             config.add_section("Logging")
 
@@ -224,14 +225,15 @@
 
             config.set("Server", "Address", cfg_server_address)
             config.set("Server", "username", cfg_username)
             config.set("Server", "password", cfg_password)
             config.set("Server", "maxFiles", cfg_max_files)
             config.set("Logging", "Level", cfg_log_level)
 
+
             with open(file_path, "w") as configfile:
                 config.write(configfile)
 
             initialize_config()  # Reload the config after updating
 
     except Exception as inst:
         handleError("Error in initialize_config", inst)
@@ -958,15 +960,15 @@
 # ============================
 def getTagsValuesFromFile(fileName):
 
     try:
         f2 = open(fileName, "r")
         vals = json.load(f2)
         f2.close()
-        ci_print("Got " + str(len(vals)) + " Values From File", "INFO")
+
         return vals
     except Exception as inst:
         handleError("Error in getTagsValuesFromFile", inst)
 
 
 # ============================
 def saveValuesToFile(values, fileName):
```

### Comparing `ci_cloudconnector-1.4/main.py` & `ci_cloudconnector-1.5/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
 def MainLoopTimer():
     print(f"MainLoopTimer: {str(datetime.now())}")
     global repeating_timer
 
     if repeating_timer:
         repeating_timer.stop()
 
-    logic.ci_print(f"VERSION: {logic.getLocalVersion()}")
     if service_stop == 1:
         repeating_timer = None
         return
 
     try:
         MainLoop()
     except Exception as e:
```

### Comparing `ci_cloudconnector-1.4/myservice.py` & `ci_cloudconnector-1.5/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.4/setup.py` & `ci_cloudconnector-1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="1.4",
+    version="1.5",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

