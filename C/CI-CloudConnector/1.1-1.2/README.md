# Comparing `tmp/ci_cloudconnector-1.1.tar.gz` & `tmp/ci_cloudconnector-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-1.1.tar", last modified: Thu May 30 07:38:04 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.2.tar", last modified: Thu May 30 07:43:49 2024, max compression
```

## Comparing `ci_cloudconnector-1.1.tar` & `ci_cloudconnector-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:38:04.394997 ci_cloudconnector-1.1/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:38:04.389582 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 07:38:04.391253 ci_cloudconnector-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.1/README.txt
--rw-rw-rw-   0        0        0    38752 2024-05-30 07:36:23.000000 ci_cloudconnector-1.1/logic.py
--rw-rw-rw-   0        0        0     8282 2024-05-30 07:36:04.000000 ci_cloudconnector-1.1/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.1/myservice.py
--rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.1/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 07:38:04.394997 ci_cloudconnector-1.1/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-05-30 07:36:12.000000 ci_cloudconnector-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:43:49.602096 ci_cloudconnector-1.2/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:43:49.598627 ci_cloudconnector-1.2/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:43:49.000000 ci_cloudconnector-1.2/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 07:43:49.000000 ci_cloudconnector-1.2/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:43:49.000000 ci_cloudconnector-1.2/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 07:43:49.000000 ci_cloudconnector-1.2/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:43:49.600597 ci_cloudconnector-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.2/README.txt
+-rw-rw-rw-   0        0        0    38751 2024-05-30 07:42:56.000000 ci_cloudconnector-1.2/logic.py
+-rw-rw-rw-   0        0        0     8283 2024-05-30 07:42:42.000000 ci_cloudconnector-1.2/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.2/myservice.py
+-rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.2/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:43:49.603097 ci_cloudconnector-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-30 07:42:56.000000 ci_cloudconnector-1.2/setup.py
```

### Comparing `ci_cloudconnector-1.1/logic.py` & `ci_cloudconnector-1.2/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "1.01"
+VER = "1.2"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-1.1/main.py` & `ci_cloudconnector-1.2/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     observer.start()
     return observer
 
 
 def init():
     logic.create_directories_if_missing()
     logic.initialize_config()
-    set_service_restart_delay("CloudConnectorService", 1000)
+    set_service_restart_delay("CloudConnectorService", 10000)
 
 
 
 def serviceStop():
     global service_stop
     service_stop = 1
     logic.ci_print("Service stop requested.")
```

### Comparing `ci_cloudconnector-1.1/myservice.py` & `ci_cloudconnector-1.2/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.1/setup.py` & `ci_cloudconnector-1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="1.01",
+    version="1.2",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

