# Comparing `tmp/ci_cloudconnector-1.8.tar.gz` & `tmp/ci_cloudconnector-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-1.8.tar", last modified: Thu May 30 08:37:50 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.9.tar", last modified: Thu May 30 08:40:08 2024, max compression
```

## Comparing `ci_cloudconnector-1.8.tar` & `ci_cloudconnector-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:37:50.244084 ci_cloudconnector-1.8/
-drwxrwxrwx   0        0        0        0 2024-05-30 08:37:50.238695 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 08:37:50.000000 ci_cloudconnector-1.8/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 08:37:50.241604 ci_cloudconnector-1.8/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.8/README.txt
--rw-rw-rw-   0        0        0    39040 2024-05-30 08:37:23.000000 ci_cloudconnector-1.8/logic.py
--rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-1.8/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.8/myservice.py
--rw-rw-rw-   0        0        0      964 2024-05-30 08:23:50.000000 ci_cloudconnector-1.8/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 08:37:50.244084 ci_cloudconnector-1.8/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-30 08:37:27.000000 ci_cloudconnector-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:40:08.525670 ci_cloudconnector-1.9/
+drwxrwxrwx   0        0        0        0 2024-05-30 08:40:08.525670 ci_cloudconnector-1.9/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:40:08.000000 ci_cloudconnector-1.9/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 08:40:08.000000 ci_cloudconnector-1.9/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:40:08.000000 ci_cloudconnector-1.9/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 08:40:08.000000 ci_cloudconnector-1.9/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 08:40:08.525670 ci_cloudconnector-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.9/README.txt
+-rw-rw-rw-   0        0        0    39040 2024-05-30 08:39:35.000000 ci_cloudconnector-1.9/logic.py
+-rw-rw-rw-   0        0        0     8242 2024-05-30 08:03:29.000000 ci_cloudconnector-1.9/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.9/myservice.py
+-rw-rw-rw-   0        0        0      964 2024-05-30 08:23:50.000000 ci_cloudconnector-1.9/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 08:40:08.525670 ci_cloudconnector-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-30 08:40:00.000000 ci_cloudconnector-1.9/setup.py
```

### Comparing `ci_cloudconnector-1.8/logic.py` & `ci_cloudconnector-1.9/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "1.8"
+VER = "1.9"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-1.8/main.py` & `ci_cloudconnector-1.9/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.8/myservice.py` & `ci_cloudconnector-1.9/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.8/myservice_installer.py` & `ci_cloudconnector-1.9/myservice_installer.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.8/setup.py` & `ci_cloudconnector-1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="1.8",
+    version="1.9",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

