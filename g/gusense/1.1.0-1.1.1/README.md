# Comparing `tmp/gusense-1.1.0.tar.gz` & `tmp/gusense-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gusense-1.1.0.tar", last modified: Wed May 29 15:16:37 2024, max compression
+gzip compressed data, was "dist\gusense-1.1.1.tar", last modified: Thu May 30 03:45:51 2024, max compression
```

## Comparing `gusense-1.1.0.tar` & `gusense-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 15:16:37.424334 gusense-1.1.0/
--rw-rw-rw-   0        0        0     1521 2024-03-27 03:33:12.000000 gusense-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      905 2024-05-29 15:16:37.424334 gusense-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-03-27 07:00:40.000000 gusense-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 15:16:37.408709 gusense-1.1.0/gusense/
--rw-rw-rw-   0        0        0      266 2024-03-27 02:06:09.000000 gusense-1.1.0/gusense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:16:37.408709 gusense-1.1.0/gusense/api/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:29:45.000000 gusense-1.1.0/gusense/api/__init__.py
--rw-rw-rw-   0        0        0     1407 2024-03-27 02:04:07.000000 gusense-1.1.0/gusense/api/client.py
--rw-rw-rw-   0        0        0      425 2024-03-27 02:15:39.000000 gusense-1.1.0/gusense/api/data_api.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:16:37.424334 gusense-1.1.0/gusense/common/
--rw-rw-rw-   0        0        0        0 2023-05-05 14:40:44.000000 gusense-1.1.0/gusense/common/__init__.py
--rw-rw-rw-   0        0        0      276 2024-05-29 14:23:24.000000 gusense-1.1.0/gusense/common/contant.py
--rw-rw-rw-   0        0        0     1725 2024-03-27 02:04:07.000000 gusense-1.1.0/gusense/common/credit.py
-drwxrwxrwx   0        0        0        0 2024-05-29 15:16:37.408709 gusense-1.1.0/gusense.egg-info/
--rw-rw-rw-   0        0        0      905 2024-05-29 15:16:37.000000 gusense-1.1.0/gusense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-05-29 15:16:37.000000 gusense-1.1.0/gusense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 15:16:37.000000 gusense-1.1.0/gusense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-29 15:16:37.000000 gusense-1.1.0/gusense.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-29 15:16:37.000000 gusense-1.1.0/gusense.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 15:16:37.424334 gusense-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1250 2024-05-29 15:16:33.000000 gusense-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:45:51.069930 gusense-1.1.1/
+-rw-rw-rw-   0        0        0     1521 2024-03-27 03:33:12.000000 gusense-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      905 2024-05-30 03:45:51.069930 gusense-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-03-27 07:00:40.000000 gusense-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 03:45:51.058426 gusense-1.1.1/gusense/
+-rw-rw-rw-   0        0        0      266 2024-03-27 02:06:09.000000 gusense-1.1.1/gusense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:45:51.058426 gusense-1.1.1/gusense/api/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:29:45.000000 gusense-1.1.1/gusense/api/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-05-30 03:14:42.000000 gusense-1.1.1/gusense/api/client.py
+-rw-rw-rw-   0        0        0      425 2024-03-27 02:15:39.000000 gusense-1.1.1/gusense/api/data_api.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:45:51.069930 gusense-1.1.1/gusense/common/
+-rw-rw-rw-   0        0        0        0 2023-05-05 14:40:44.000000 gusense-1.1.1/gusense/common/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-05-29 16:29:24.000000 gusense-1.1.1/gusense/common/contant.py
+-rw-rw-rw-   0        0        0     1957 2024-05-30 03:41:52.000000 gusense-1.1.1/gusense/common/credit.py
+drwxrwxrwx   0        0        0        0 2024-05-30 03:45:51.058426 gusense-1.1.1/gusense.egg-info/
+-rw-rw-rw-   0        0        0      905 2024-05-30 03:45:50.000000 gusense-1.1.1/gusense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-05-30 03:45:51.000000 gusense-1.1.1/gusense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 03:45:50.000000 gusense-1.1.1/gusense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-30 03:45:50.000000 gusense-1.1.1/gusense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-30 03:45:50.000000 gusense-1.1.1/gusense.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 03:45:51.069930 gusense-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2024-05-30 03:44:58.000000 gusense-1.1.1/setup.py
```

### Comparing `gusense-1.1.0/LICENSE` & `gusense-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gusense-1.1.0/PKG-INFO` & `gusense-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gusense
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is API util
 Home-page: https://www.python.org
 Author: wgp
 Author-email: 284250692@qq.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `gusense-1.1.0/gusense/api/client.py` & `gusense-1.1.1/gusense/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding:utf-8 -*-
 
 """
-数据接口
+数据公共接口
 Date: 2023.05.09
 author: wgp
 contact: 284250692@qq.com
 """
 
 import json
 import requests
 import pandas as pd
 from functools import partial
 from ..common import contant
 
-pd.set_option('display.max_columns', 500)
-pd.set_option('display.max_rows', 500)
-pd.set_option('max_colwidth', 1000)
-pd.set_option('display.width', 5000)
+# pd.set_option('display.max_columns', 500)
+# pd.set_option('display.max_rows', 500)
+# pd.set_option('max_colwidth', 1000)
+# pd.set_option('display.width', 5000)
 
 
 class HttpClient:
 
     def __init__(self, token=''):
         self.basic_url = contant.BASIC_URL
         self.token = token
```

### Comparing `gusense-1.1.0/gusense/common/credit.py` & `gusense-1.1.1/gusense/common/credit.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 """
 用户认证
 Date: 2023.05.09
 author: wgp
 contact: 284250692@qq.com
 """
 
-
 import json
 import pandas as pd
 import os
 import requests
 from ..common import contant
 
 user_path = os.path.expanduser('~')
 
+"""
+    用户认证方法，开发者ID和密匙来源Gusense数据中心
+"""
 
 def auth(app_id, app_secret):
     token = get_token(app_id, app_secret)
     if token is None or token == '':
         params = {
             "appId": app_id,
             "appSecret": app_secret
@@ -29,19 +31,25 @@
         code = json_res['code']
         if code == contant.REQ_SUCCESS_CODE:
             token = json_res['data']
             df = pd.DataFrame([[app_id, app_secret, token]], columns=['app_id', 'app_secret', 'token'])
             op = os.path.join(user_path, contant.USER_TOKEN_CN)
             df.to_csv(op, index=False)
         else:
-            os.remove(user_path + contant.SEPARATOR + contant.USER_TOKEN_CN)
+            path = user_path + contant.SEPARATOR + contant.USER_TOKEN_CN
+            if os.path.exists(path):
+                os.remove(user_path + contant.SEPARATOR + contant.USER_TOKEN_CN)
             msg = json_res['msg']
             raise Exception(msg)
 
 
+"""
+    获取token的方法
+"""
+
 def get_token(app_id=None, app_secret=None):
     credit_list = get_credit_list()
     if credit_list is None:
         return None
     if app_id is not None and app_secret is not None:
         oai = credit_list['app_id']
         oas = credit_list['app_secret']
@@ -56,8 +64,7 @@
     op = os.path.join(user_path, contant.USER_TOKEN_CN)
     if os.path.exists(op):
         df = pd.read_csv(op)
         credit_list = df.loc[0]
         return credit_list
     else:
         return None
-
```

### Comparing `gusense-1.1.0/gusense.egg-info/PKG-INFO` & `gusense-1.1.1/gusense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gusense
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is API util
 Home-page: https://www.python.org
 Author: wgp
 Author-email: 284250692@qq.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `gusense-1.1.0/setup.py` & `gusense-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # import re
 import setuptools
 
-version = "1.1.0"
+version = "1.1.1"
 # with open('gusense/__init__.py', 'r') as fd:
 #     version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
 #                         fd.read(), re.MULTILINE).group(1)
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="gusense",
```

