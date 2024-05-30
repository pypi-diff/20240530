# Comparing `tmp/alibabacloud_videoenhan20200320-3.0.8.tar.gz` & `tmp/alibabacloud_videoenhan20200320-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_videoenhan20200320-3.0.8.tar", last modified: Fri Dec 16 05:26:56 2022, max compression
+gzip compressed data, was "dist/alibabacloud_videoenhan20200320-3.0.9.tar", last modified: Wed Jan 11 02:55:52 2023, max compression
```

## Comparing `alibabacloud_videoenhan20200320-3.0.8.tar` & `alibabacloud_videoenhan20200320-3.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/
--rw-r--r--   0 root         (0) root         (0)     1041 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   172331 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320/client.py
--rw-r--r--   0 root         (0) root         (0)   108612 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      359 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2888 2022-12-16 05:26:56.000000 alibabacloud_videoenhan20200320-3.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   172331 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320/client.py
+-rw-r--r--   0 root         (0) root         (0)   108612 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      359 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2888 2023-01-11 02:55:52.000000 alibabacloud_videoenhan20200320-3.0.9/setup.py
```

### Comparing `alibabacloud_videoenhan20200320-3.0.8/ChangeLog.md` & `alibabacloud_videoenhan20200320-3.0.9/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2022-12-16 Version: 3.0.8
+- Release MergeVideoModelFace.
+
 2022-12-14 Version: 3.0.7
 - Release MergeVideoModelFace.
 
 2022-12-02 Version: 3.0.6
 - Release MergeVideoModelFace.
 
 2022-11-30 Version: 3.0.5
```

### Comparing `alibabacloud_videoenhan20200320-3.0.8/LICENSE` & `alibabacloud_videoenhan20200320-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_videoenhan20200320-3.0.8/PKG-INFO` & `alibabacloud_videoenhan20200320-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_videoenhan20200320
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud videoenhan (20200320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_videoenhan20200320-3.0.8/README-CN.md` & `alibabacloud_videoenhan20200320-3.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_videoenhan20200320-3.0.8/README.md` & `alibabacloud_videoenhan20200320-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320/client.py` & `alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320/models.py` & `alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_videoenhan20200320-3.0.8/alibabacloud_videoenhan20200320.egg-info/PKG-INFO` & `alibabacloud_videoenhan20200320-3.0.9/alibabacloud_videoenhan20200320.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-videoenhan20200320
-Version: 3.0.8
+Version: 3.0.9
 Summary: Alibaba Cloud videoenhan (20200320) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_videoenhan20200320-3.0.8/setup.py` & `alibabacloud_videoenhan20200320-3.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_videoenhan20200320.
 
-Created on 16/12/2022
+Created on 11/01/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_videoenhan20200320"
 NAME = "alibabacloud_videoenhan20200320" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud videoenhan (20200320) SDK Library for Python"
@@ -40,15 +40,15 @@
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
     "alibabacloud_darabonba_number>=0.0.4, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

