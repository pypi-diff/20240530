# Comparing `tmp/ci_cloudconnector-0.99.tar.gz` & `tmp/ci_cloudconnector-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.99.tar", last modified: Thu May 30 05:59:42 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.0.tar", last modified: Thu May 30 07:15:00 2024, max compression
```

## Comparing `ci_cloudconnector-0.99.tar` & `ci_cloudconnector-1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 05:59:42.912712 ci_cloudconnector-0.99/
-drwxrwxrwx   0        0        0        0 2024-05-30 05:59:42.907946 ci_cloudconnector-0.99/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      358 2024-05-30 05:59:42.000000 ci_cloudconnector-0.99/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-30 05:59:42.000000 ci_cloudconnector-0.99/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 05:59:42.000000 ci_cloudconnector-0.99/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 05:59:42.000000 ci_cloudconnector-0.99/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2024-05-30 05:59:42.910357 ci_cloudconnector-0.99/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.99/README.txt
--rw-rw-rw-   0        0        0    38756 2024-05-30 05:59:23.000000 ci_cloudconnector-0.99/logic.py
--rw-rw-rw-   0        0        0     8423 2024-05-30 05:59:18.000000 ci_cloudconnector-0.99/main.py
--rw-rw-rw-   0        0        0     2937 2024-05-30 05:43:53.000000 ci_cloudconnector-0.99/myservice.py
--rw-rw-rw-   0        0        0       42 2024-05-30 05:59:42.913087 ci_cloudconnector-0.99/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-05-30 05:59:28.000000 ci_cloudconnector-0.99/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:15:00.022626 ci_cloudconnector-1.0/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:15:00.009850 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:15:00.018843 ci_cloudconnector-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.0/README.txt
+-rw-rw-rw-   0        0        0    38752 2024-05-30 07:14:47.000000 ci_cloudconnector-1.0/logic.py
+-rw-rw-rw-   0        0        0     7757 2024-05-30 05:59:53.000000 ci_cloudconnector-1.0/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.0/myservice.py
+-rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.0/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:15:00.022927 ci_cloudconnector-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-05-30 07:14:41.000000 ci_cloudconnector-1.0/setup.py
```

### Comparing `ci_cloudconnector-0.99/logic.py` & `ci_cloudconnector-1.0/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "0.99"
+VER = "1.00"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
@@ -28,16 +28,14 @@
 ScanRateLastRead = {}
 currentToken = ""
 g_connectorTypeName = ""
 g_lastGetTagsFromServer = None
 g_lastGetCloudVersionFromServer = None
 g_app_log = None
 
-
-
 def enum(**enums):
     return type("Enum", (), enums)
 
 TagStatus = enum(Invalid=10, Valid=20)
 
 def initialize_log(log_level=""):
```

### Comparing `ci_cloudconnector-0.99/main.py` & `ci_cloudconnector-1.0/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,42 +229,24 @@
     observer.start()
     return observer
 
 
 def init():
     logic.create_directories_if_missing()
     logic.initialize_config()
-    set_service_recovery_options(service_name, restart_delay)
 
 
 
 def serviceStop():
     global service_stop
     service_stop = 1
     logic.ci_print("Service stop requested.")
 
 
 
-def set_service_recovery_options(service_name, restart_delay):
-    try:
-        # Configure service recovery options
-        subprocess.run([
-            'sc', 'failure', service_name,
-            'reset=', '0',
-            f'actions=restart/{restart_delay}'
-        ], check=True)
-        logic.ci_print(f"Service recovery options for {service_name} configured successfully.")
-    except subprocess.CalledProcessError as e:
-        logic.ci_print(f"Error configuring service recovery options: {e}")
-
-# Usage
-service_name = "CloudConnectorService"
-restart_delay = 10000  # 10 seconds
-
-
 if __name__ == '__main__':
     init()
     args(sys.argv)
     #args([0, 'Start'])
     current_script_dir = os.path.dirname(os.path.abspath(__file__))
     main_file = os.path.join(current_script_dir, "logic.py")
     monitor_main_file(main_file)
```

### Comparing `ci_cloudconnector-0.99/myservice.py` & `ci_cloudconnector-1.0/myservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import logic
 import main
 
 class MyService(win32serviceutil.ServiceFramework):
     _svc_name_ = "CloudConnectorService"
     _svc_display_name_ = "CloudConnectorService"
+    _svc_failure_actions_ = "restart/10000"  # Restart the service after 1 minute if it fails
 
     def __init__(self, args):
         win32serviceutil.ServiceFramework.__init__(self, args)
         self.stop_event = win32event.CreateEvent(None, 0, 0, None)
 
     def SvcDoRun(self):
         try:
```

### Comparing `ci_cloudconnector-0.99/setup.py` & `ci_cloudconnector-1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="0.99",
+    version="1.00",
     packages=find_packages(),
-    py_modules=["logic", "main", "setup", "myservice"],
+    py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
     long_description=open("README.txt").read()  # Make sure you have README.txt in the same directory
 )
```

