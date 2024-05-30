# Comparing `tmp/alibabacloud_slb20140515-3.3.26.tar.gz` & `tmp/alibabacloud_slb20140515-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_slb20140515-3.3.26.tar", last modified: Thu May 30 12:43:14 2024, max compression
+gzip compressed data, was "dist/alibabacloud_slb20140515-3.3.9.tar", last modified: Wed Dec 29 10:09:58 2021, max compression
```

## Comparing `alibabacloud_slb20140515-3.3.26.tar` & `alibabacloud_slb20140515-3.3.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 12:43:14.000000 alibabacloud_slb20140515-3.3.26/
--rw-r--r--   0 root         (0) root         (0)     1591 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2419 2024-05-30 12:43:14.000000 alibabacloud_slb20140515-3.3.26/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 12:43:14.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   620458 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515/client.py
--rw-r--r--   0 root         (0) root         (0)  1090704 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 12:43:14.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2419 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-30 12:43:14.000000 alibabacloud_slb20140515-3.3.26/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2628 2024-05-30 12:43:13.000000 alibabacloud_slb20140515-3.3.26/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/
+-rw-r--r--   0 root         (0) root         (0)      305 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2345 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   431433 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/client.py
+-rw-r--r--   0 root         (0) root         (0)   695669 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2345 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2627 2021-12-29 10:09:58.000000 alibabacloud_slb20140515-3.3.9/setup.py
```

### Comparing `alibabacloud_slb20140515-3.3.26/LICENSE` & `alibabacloud_slb20140515-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_slb20140515-3.3.26/PKG-INFO` & `alibabacloud_slb20140515-3.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_slb20140515
-Version: 3.3.26
+Version: 3.3.9
 Summary: Alibaba Cloud Server Load Balancer (20140515) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/slb-20140515/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_slb20140515-3.3.26/README-CN.md` & `alibabacloud_slb20140515-3.3.9/README-CN.md`

 * *Files 16% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/slb-20140515/ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_slb20140515-3.3.26/README.md` & `alibabacloud_slb20140515-3.3.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/slb-20140515/ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_slb20140515-3.3.26/alibabacloud_slb20140515.egg-info/PKG-INFO` & `alibabacloud_slb20140515-3.3.9/alibabacloud_slb20140515.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-slb20140515
-Version: 3.3.26
+Version: 3.3.9
 Summary: Alibaba Cloud Server Load Balancer (20140515) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/slb-20140515/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_slb20140515-3.3.26/setup.py` & `alibabacloud_slb20140515-3.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_slb20140515.
 
-Created on 30/05/2024
+Created on 29/12/2021
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_slb20140515"
 NAME = "alibabacloud_slb20140515" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Server Load Balancer (20140515) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.12, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

