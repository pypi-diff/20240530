# Comparing `tmp/ci_cloudconnector-0.97.tar.gz` & `tmp/ci_cloudconnector-0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.97.tar", last modified: Thu May 30 05:19:05 2024, max compression
+gzip compressed data, was "ci_cloudconnector-0.98.tar", last modified: Thu May 30 05:34:12 2024, max compression
```

## Comparing `ci_cloudconnector-0.97.tar` & `ci_cloudconnector-0.98.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 05:19:05.304305 ci_cloudconnector-0.97/
-drwxrwxrwx   0        0        0        0 2024-05-30 05:19:05.300939 ci_cloudconnector-0.97/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      358 2024-05-30 05:19:05.000000 ci_cloudconnector-0.97/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-30 05:19:05.000000 ci_cloudconnector-0.97/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 05:19:05.000000 ci_cloudconnector-0.97/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 05:19:05.000000 ci_cloudconnector-0.97/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2024-05-30 05:19:05.304305 ci_cloudconnector-0.97/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.97/README.txt
--rw-rw-rw-   0        0        0    38752 2024-05-30 05:18:41.000000 ci_cloudconnector-0.97/logic.py
--rw-rw-rw-   0        0        0     7757 2024-05-29 19:17:55.000000 ci_cloudconnector-0.97/main.py
--rw-rw-rw-   0        0        0     3034 2024-05-30 05:16:55.000000 ci_cloudconnector-0.97/myservice.py
--rw-rw-rw-   0        0        0       42 2024-05-30 05:19:05.304305 ci_cloudconnector-0.97/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-05-30 05:18:35.000000 ci_cloudconnector-0.97/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 05:34:12.383466 ci_cloudconnector-0.98/
+drwxrwxrwx   0        0        0        0 2024-05-30 05:34:12.380678 ci_cloudconnector-0.98/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      358 2024-05-30 05:34:12.000000 ci_cloudconnector-0.98/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-30 05:34:12.000000 ci_cloudconnector-0.98/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 05:34:12.000000 ci_cloudconnector-0.98/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-30 05:34:12.000000 ci_cloudconnector-0.98/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2024-05-30 05:34:12.383466 ci_cloudconnector-0.98/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.98/README.txt
+-rw-rw-rw-   0        0        0    38752 2024-05-30 05:33:38.000000 ci_cloudconnector-0.98/logic.py
+-rw-rw-rw-   0        0        0     7757 2024-05-30 05:25:25.000000 ci_cloudconnector-0.98/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:33:29.000000 ci_cloudconnector-0.98/myservice.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 05:34:12.383466 ci_cloudconnector-0.98/setup.cfg
+-rw-rw-rw-   0        0        0      791 2024-05-30 05:33:44.000000 ci_cloudconnector-0.98/setup.py
```

### Comparing `ci_cloudconnector-0.97/logic.py` & `ci_cloudconnector-0.98/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "0.97"
+VER = "0.98"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-0.97/main.py` & `ci_cloudconnector-0.98/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-0.97/myservice.py` & `ci_cloudconnector-0.98/myservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import win32event
 import subprocess
 
 import logic
 import main
 
 class MyService(win32serviceutil.ServiceFramework):
-    _svc_name_ = "CloudConnectorService2"
-    _svc_display_name_ = "CloudConnectorService2"
+    _svc_name_ = "CloudConnectorService"
+    _svc_display_name_ = "CloudConnectorService"
     _svc_failure_actions_ = "restart/10000"  # Restart the service after 1 minute if it fails
 
     def __init__(self, args):
         win32serviceutil.ServiceFramework.__init__(self, args)
         self.stop_event = win32event.CreateEvent(None, 0, 0, None)
 
     def SvcDoRun(self):
```

### Comparing `ci_cloudconnector-0.97/setup.py` & `ci_cloudconnector-0.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="0.97",
+    version="0.98",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

