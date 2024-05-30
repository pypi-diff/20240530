# Comparing `tmp/ci_cloudconnector-0.95.tar.gz` & `tmp/ci_cloudconnector-0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.95.tar", last modified: Wed May 29 18:48:21 2024, max compression
+gzip compressed data, was "ci_cloudconnector-0.96.tar", last modified: Wed May 29 19:11:42 2024, max compression
```

## Comparing `ci_cloudconnector-0.95.tar` & `ci_cloudconnector-0.96.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 18:48:21.926079 ci_cloudconnector-0.95/
-drwxrwxrwx   0        0        0        0 2024-05-29 18:48:21.920328 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      358 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2024-05-29 18:48:21.922662 ci_cloudconnector-0.95/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.95/README.txt
--rw-rw-rw-   0        0        0    38752 2024-05-29 18:47:31.000000 ci_cloudconnector-0.95/logic.py
--rw-rw-rw-   0        0        0     7755 2024-05-29 18:47:17.000000 ci_cloudconnector-0.95/main.py
--rw-rw-rw-   0        0        0     2827 2024-05-29 18:43:18.000000 ci_cloudconnector-0.95/myservice.py
--rw-rw-rw-   0        0        0       42 2024-05-29 18:48:21.926079 ci_cloudconnector-0.95/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-05-29 18:47:40.000000 ci_cloudconnector-0.95/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 19:11:42.046716 ci_cloudconnector-0.96/
+drwxrwxrwx   0        0        0        0 2024-05-29 19:11:42.042794 ci_cloudconnector-0.96/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      358 2024-05-29 19:11:41.000000 ci_cloudconnector-0.96/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-29 19:11:41.000000 ci_cloudconnector-0.96/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 19:11:41.000000 ci_cloudconnector-0.96/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-29 19:11:41.000000 ci_cloudconnector-0.96/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2024-05-29 19:11:42.044677 ci_cloudconnector-0.96/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.96/README.txt
+-rw-rw-rw-   0        0        0    38752 2024-05-29 19:11:21.000000 ci_cloudconnector-0.96/logic.py
+-rw-rw-rw-   0        0        0     7757 2024-05-29 19:05:58.000000 ci_cloudconnector-0.96/main.py
+-rw-rw-rw-   0        0        0     3018 2024-05-29 19:08:55.000000 ci_cloudconnector-0.96/myservice.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 19:11:42.046716 ci_cloudconnector-0.96/setup.cfg
+-rw-rw-rw-   0        0        0      791 2024-05-29 19:11:26.000000 ci_cloudconnector-0.96/setup.py
```

### Comparing `ci_cloudconnector-0.95/logic.py` & `ci_cloudconnector-0.96/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "0.95"
+VER = "0.96"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-0.95/main.py` & `ci_cloudconnector-0.96/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
         self.main_file = main_file
         self.myService = service
 
     def on_modified(self, event):
         if event.src_path.endswith(self.main_file):
             logic.ci_print("Main file has been modified. Signaling service to restart...")
 
+
             # Stop the service
             self.myService.ServiceUpdated()
             logic.ci_print("Service stopped. You may restart it if necessary.")
 
 
 
 def monitor_main_file(main_file, service):
```

### Comparing `ci_cloudconnector-0.95/myservice.py` & `ci_cloudconnector-0.96/myservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,18 +50,24 @@
         if wait_result == win32event.WAIT_OBJECT_0:
             # Stop event has been signaled
             return
 
     def SvcStop(self):
         self.ReportServiceStatus(win32service.SERVICE_STOP_PENDING)
         main.serviceStop()
+
+
         logic.ci_print('Service stop requested.')
         time.sleep(2)  # Allow some time for the service to stop gracefully
         win32event.SetEvent(self.stop_event)
 
+        time.sleep(2)  # Allow some time for the service to stop gracefully
+        # Exit the service process with code -1
+        raise RuntimeError("stop the service with error")
+
 
         #time.sleep(20)
         #self.SvcTerminate()
 
     def ServiceUpdated(self):
         logic.ci_print('Service updated, stopping service...')
         self.SvcStop()
```

### Comparing `ci_cloudconnector-0.95/setup.py` & `ci_cloudconnector-0.96/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="0.95",
+    version="0.96",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

