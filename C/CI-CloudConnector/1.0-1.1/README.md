# Comparing `tmp/ci_cloudconnector-1.0.tar.gz` & `tmp/ci_cloudconnector-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-1.0.tar", last modified: Thu May 30 07:15:00 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.1.tar", last modified: Thu May 30 07:38:04 2024, max compression
```

## Comparing `ci_cloudconnector-1.0.tar` & `ci_cloudconnector-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:15:00.022626 ci_cloudconnector-1.0/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:15:00.009850 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 07:14:59.000000 ci_cloudconnector-1.0/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 07:15:00.018843 ci_cloudconnector-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.0/README.txt
--rw-rw-rw-   0        0        0    38752 2024-05-30 07:14:47.000000 ci_cloudconnector-1.0/logic.py
--rw-rw-rw-   0        0        0     7757 2024-05-30 05:59:53.000000 ci_cloudconnector-1.0/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.0/myservice.py
--rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.0/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 07:15:00.022927 ci_cloudconnector-1.0/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-05-30 07:14:41.000000 ci_cloudconnector-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:38:04.394997 ci_cloudconnector-1.1/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:38:04.389582 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 07:38:04.000000 ci_cloudconnector-1.1/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:38:04.391253 ci_cloudconnector-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.1/README.txt
+-rw-rw-rw-   0        0        0    38752 2024-05-30 07:36:23.000000 ci_cloudconnector-1.1/logic.py
+-rw-rw-rw-   0        0        0     8282 2024-05-30 07:36:04.000000 ci_cloudconnector-1.1/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.1/myservice.py
+-rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.1/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:38:04.394997 ci_cloudconnector-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-05-30 07:36:12.000000 ci_cloudconnector-1.1/setup.py
```

### Comparing `ci_cloudconnector-1.0/logic.py` & `ci_cloudconnector-1.1/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "1.00"
+VER = "1.01"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-1.0/main.py` & `ci_cloudconnector-1.1/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -229,24 +229,35 @@
     observer.start()
     return observer
 
 
 def init():
     logic.create_directories_if_missing()
     logic.initialize_config()
+    set_service_restart_delay("CloudConnectorService", 1000)
 
 
 
 def serviceStop():
     global service_stop
     service_stop = 1
     logic.ci_print("Service stop requested.")
 
 
 
+def set_service_restart_delay(service_name, delay_milliseconds):
+    command = f'sc failure {service_name} reset= 0 actions= restart/{delay_milliseconds}'
+    try:
+        subprocess.run(command, shell=True, check=True)
+        print(f"Restart delay for service '{service_name}' set to {delay_milliseconds} milliseconds.")
+    except subprocess.CalledProcessError as e:
+        print(f"Error setting restart delay for service '{service_name}': {e}")
+
+
+
 if __name__ == '__main__':
     init()
     args(sys.argv)
     #args([0, 'Start'])
     current_script_dir = os.path.dirname(os.path.abspath(__file__))
     main_file = os.path.join(current_script_dir, "logic.py")
     monitor_main_file(main_file)
```

### Comparing `ci_cloudconnector-1.0/myservice.py` & `ci_cloudconnector-1.1/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.0/setup.py` & `ci_cloudconnector-1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="1.00",
+    version="1.01",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

