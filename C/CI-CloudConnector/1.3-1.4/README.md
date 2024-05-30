# Comparing `tmp/ci_cloudconnector-1.3.tar.gz` & `tmp/ci_cloudconnector-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-1.3.tar", last modified: Thu May 30 07:50:18 2024, max compression
+gzip compressed data, was "ci_cloudconnector-1.4.tar", last modified: Thu May 30 07:59:22 2024, max compression
```

## Comparing `ci_cloudconnector-1.3.tar` & `ci_cloudconnector-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:50:18.967574 ci_cloudconnector-1.3/
-drwxrwxrwx   0        0        0        0 2024-05-30 07:50:18.967574 ci_cloudconnector-1.3/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      357 2024-05-30 07:50:18.000000 ci_cloudconnector-1.3/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-30 07:50:18.000000 ci_cloudconnector-1.3/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:50:18.000000 ci_cloudconnector-1.3/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-30 07:50:18.000000 ci_cloudconnector-1.3/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      357 2024-05-30 07:50:18.967574 ci_cloudconnector-1.3/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.3/README.txt
--rw-rw-rw-   0        0        0    38751 2024-05-30 07:46:31.000000 ci_cloudconnector-1.3/logic.py
--rw-rw-rw-   0        0        0     8301 2024-05-30 07:45:13.000000 ci_cloudconnector-1.3/main.py
--rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.3/myservice.py
--rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.3/myservice_installer.py
--rw-rw-rw-   0        0        0       42 2024-05-30 07:50:18.967574 ci_cloudconnector-1.3/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-30 07:46:28.000000 ci_cloudconnector-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 07:59:22.190848 ci_cloudconnector-1.4/
+drwxrwxrwx   0        0        0        0 2024-05-30 07:59:22.183235 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-30 07:59:22.000000 ci_cloudconnector-1.4/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      357 2024-05-30 07:59:22.187525 ci_cloudconnector-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-1.4/README.txt
+-rw-rw-rw-   0        0        0    38751 2024-05-30 07:55:54.000000 ci_cloudconnector-1.4/logic.py
+-rw-rw-rw-   0        0        0     8301 2024-05-30 07:45:13.000000 ci_cloudconnector-1.4/main.py
+-rw-rw-rw-   0        0        0     3032 2024-05-30 05:59:53.000000 ci_cloudconnector-1.4/myservice.py
+-rw-rw-rw-   0        0        0      456 2024-05-30 06:06:07.000000 ci_cloudconnector-1.4/myservice_installer.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 07:59:22.191345 ci_cloudconnector-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-05-30 07:56:01.000000 ci_cloudconnector-1.4/setup.py
```

### Comparing `ci_cloudconnector-1.3/logic.py` & `ci_cloudconnector-1.4/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "1.3"
+VER = "1.4"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-1.3/main.py` & `ci_cloudconnector-1.4/main.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.3/myservice.py` & `ci_cloudconnector-1.4/myservice.py`

 * *Files identical despite different names*

### Comparing `ci_cloudconnector-1.3/setup.py` & `ci_cloudconnector-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="1.3",
+    version="1.4",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice", "myservice_installer"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

