# Comparing `tmp/juliang-1.0.1.tar.gz` & `tmp/juliang-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juliang-1.0.1.tar", last modified: Wed Aug  2 02:46:10 2023, max compression
+gzip compressed data, was "juliang-1.1.0.tar", last modified: Thu May 30 10:24:01 2024, max compression
```

## Comparing `juliang-1.0.1.tar` & `juliang-1.1.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.069491 juliang-1.0.1/
--rw-r--r--   0 symbol     (501) staff       (20)     1614 2023-08-02 02:46:10.069319 juliang-1.0.1/PKG-INFO
-drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.061731 juliang-1.0.1/juliang.egg-info/
--rw-r--r--   0 symbol     (501) staff       (20)     1614 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/PKG-INFO
--rw-r--r--   0 symbol     (501) staff       (20)     1155 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/SOURCES.txt
--rw-r--r--   0 symbol     (501) staff       (20)        1 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/dependency_links.txt
--rw-r--r--   0 symbol     (501) staff       (20)       10 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/top_level.txt
-drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.062124 juliang-1.0.1/juliangip/
--rw-r--r--   0 symbol     (501) staff       (20)     9786 2023-08-02 02:03:16.000000 juliang-1.0.1/juliangip/Juliang.py
--rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/__init__.py
-drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.068476 juliang-1.0.1/juliangip/common/
--rw-r--r--   0 symbol     (501) staff       (20)      409 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneGetIps.py
--rw-r--r--   0 symbol     (501) staff       (20)      196 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneGetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      349 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneReplaceWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      224 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneSetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      195 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicBalance.py
--rw-r--r--   0 symbol     (501) staff       (20)      227 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicCheck.py
--rw-r--r--   0 symbol     (501) staff       (20)      689 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicGetIps.py
--rw-r--r--   0 symbol     (501) staff       (20)      198 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicGetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      225 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicRemain.py
--rw-r--r--   0 symbol     (501) staff       (20)      351 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicReplaceWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      226 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicSetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      224 2023-08-02 01:37:44.000000 juliang-1.0.1/juliangip/common/PostPayCheck.py
--rw-r--r--   0 symbol     (501) staff       (20)      684 2023-08-02 01:27:29.000000 juliang-1.0.1/juliangip/common/PostPayGetIps.py
--rw-r--r--   0 symbol     (501) staff       (20)      196 2023-08-02 01:56:54.000000 juliang-1.0.1/juliangip/common/PostPayGetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      349 2023-08-02 02:01:33.000000 juliang-1.0.1/juliangip/common/PostPayReplaceWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      223 2023-08-02 01:50:34.000000 juliang-1.0.1/juliangip/common/PostPaySetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      484 2023-08-01 10:22:40.000000 juliang-1.0.1/juliangip/common/UnlimitedGetIps.py
--rw-r--r--   0 symbol     (501) staff       (20)      197 2023-08-01 10:28:08.000000 juliang-1.0.1/juliangip/common/UnlimitedGetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      351 2023-08-01 10:33:13.000000 juliang-1.0.1/juliangip/common/UnlimitedReplaceWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      228 2023-08-01 10:26:06.000000 juliang-1.0.1/juliangip/common/UnlimitedSetWhiteIp.py
--rw-r--r--   0 symbol     (501) staff       (20)      275 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/UsersGetAllOrders.py
--rw-r--r--   0 symbol     (501) staff       (20)      192 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/UsersGetBalance.py
--rw-r--r--   0 symbol     (501) staff       (20)      222 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/UsersGetCity.py
--rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/__init__.py
-drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.068861 juliang-1.0.1/juliangip/enums/
--rw-r--r--   0 symbol     (501) staff       (20)     2351 2023-08-02 02:03:12.000000 juliang-1.0.1/juliangip/enums/URL.py
--rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/enums/__init__.py
-drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.069120 juliang-1.0.1/juliangip/ext/
--rw-r--r--   0 symbol     (501) staff       (20)     1394 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/ext/StrKit.py
--rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/ext/__init__.py
--rw-r--r--   0 symbol     (501) staff       (20)       38 2023-08-02 02:46:10.069531 juliang-1.0.1/setup.cfg
--rw-r--r--   0 symbol     (501) staff       (20)     3823 2023-08-02 02:38:56.000000 juliang-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-30 10:24:01.706850 juliang-1.1.0/
+-rw-r--r--   0 root         (0) staff       (20)     1614 2024-05-30 10:24:01.706377 juliang-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-30 10:24:01.705834 juliang-1.1.0/juliang.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1614 2024-05-30 10:24:01.000000 juliang-1.1.0/juliang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1331 2024-05-30 10:24:01.000000 juliang-1.1.0/juliang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-30 10:24:01.000000 juliang-1.1.0/juliang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       10 2024-05-30 10:24:01.000000 juliang-1.1.0/juliang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-30 10:24:01.677148 juliang-1.1.0/juliangip/
+-rw-r--r--   0 root         (0) staff       (20)    11584 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/Juliang.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-30 10:24:01.703229 juliang-1.1.0/juliangip/common/
+-rw-r--r--   0 root         (0) staff       (20)      409 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/AloneGetIps.py
+-rw-r--r--   0 root         (0) staff       (20)      196 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/AloneGetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      349 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/AloneReplaceWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      224 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/AloneSetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      233 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/CompanyPostPayDelWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      577 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/CompanyPostPayGetIps.py
+-rw-r--r--   0 root         (0) staff       (20)      203 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/CompanyPostPayGetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      230 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/CompanyPostPaySetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      195 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/DynamicBalance.py
+-rw-r--r--   0 root         (0) staff       (20)      227 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/DynamicCheck.py
+-rw-r--r--   0 root         (0) staff       (20)      689 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/DynamicGetIps.py
+-rw-r--r--   0 root         (0) staff       (20)      198 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/DynamicGetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      225 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/DynamicRemain.py
+-rw-r--r--   0 root         (0) staff       (20)      351 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/DynamicReplaceWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      226 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/DynamicSetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      224 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/PostPayCheck.py
+-rw-r--r--   0 root         (0) staff       (20)      684 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/PostPayGetIps.py
+-rw-r--r--   0 root         (0) staff       (20)      196 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/PostPayGetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      349 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/PostPayReplaceWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      223 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/PostPaySetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      484 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/UnlimitedGetIps.py
+-rw-r--r--   0 root         (0) staff       (20)      197 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/UnlimitedGetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      351 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/UnlimitedReplaceWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      228 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/UnlimitedSetWhiteIp.py
+-rw-r--r--   0 root         (0) staff       (20)      275 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/UsersGetAllOrders.py
+-rw-r--r--   0 root         (0) staff       (20)      192 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/UsersGetBalance.py
+-rw-r--r--   0 root         (0) staff       (20)      222 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/common/UsersGetCity.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/common/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-30 10:24:01.704167 juliang-1.1.0/juliangip/enums/
+-rw-r--r--   0 root         (0) staff       (20)     2868 2024-05-30 09:51:29.000000 juliang-1.1.0/juliangip/enums/URL.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/enums/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-30 10:24:01.705403 juliang-1.1.0/juliangip/ext/
+-rw-r--r--   0 root         (0) staff       (20)     1394 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/ext/StrKit.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 07:23:55.000000 juliang-1.1.0/juliangip/ext/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-30 10:24:01.706949 juliang-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3823 2024-05-30 10:14:14.000000 juliang-1.1.0/setup.py
```

### Comparing `juliang-1.0.1/PKG-INFO` & `juliang-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juliang
-Version: 1.0.1
+Version: 1.1.0
 Summary: 巨量IP - API SDK for Python
 Home-page: https://gitee.com/juliangip/juliang-python-sdk
 Author: juliangip
 Author-email: juliangip@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `juliang-1.0.1/juliang.egg-info/PKG-INFO` & `juliang-1.1.0/juliang.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juliang
-Version: 1.0.1
+Version: 1.1.0
 Summary: 巨量IP - API SDK for Python
 Home-page: https://gitee.com/juliangip/juliang-python-sdk
 Author: juliangip
 Author-email: juliangip@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `juliang-1.0.1/juliang.egg-info/SOURCES.txt` & `juliang-1.1.0/juliang.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 juliang.egg-info/top_level.txt
 juliangip/Juliang.py
 juliangip/__init__.py
 juliangip/common/AloneGetIps.py
 juliangip/common/AloneGetWhiteIp.py
 juliangip/common/AloneReplaceWhiteIp.py
 juliangip/common/AloneSetWhiteIp.py
+juliangip/common/CompanyPostPayDelWhiteIp.py
+juliangip/common/CompanyPostPayGetIps.py
+juliangip/common/CompanyPostPayGetWhiteIp.py
+juliangip/common/CompanyPostPaySetWhiteIp.py
 juliangip/common/DynamicBalance.py
 juliangip/common/DynamicCheck.py
 juliangip/common/DynamicGetIps.py
 juliangip/common/DynamicGetWhiteIp.py
 juliangip/common/DynamicRemain.py
 juliangip/common/DynamicReplaceWhiteIp.py
 juliangip/common/DynamicSetWhiteIp.py
```

### Comparing `juliang-1.0.1/juliangip/Juliang.py` & `juliang-1.1.0/juliangip/Juliang.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 from .common.UnlimitedGetWhiteIp import UnlimitedGetWhiteIp
 from .common.UnlimitedReplaceWhiteIp import UnlimitedReplaceWhiteIp
 from .common.PostPayGetIps import PostPayGetIps
 from .common.PostPayCheck import PostPayCheck
 from .common.PostPaySetWhiteIp import PostPaySetWhiteIp
 from .common.PostPayGetWhiteIp import PostPayGetWhiteIp
 from .common.PostPayReplaceWhiteIp import PostPayReplaceWhiteIp
+from .common.CompanyPostPayGetIps import CompanyPostPayGetIps
+from .common.CompanyPostPaySetWhiteIp import CompanyPostPaySetWhiteIp
+from .common.CompanyPostPayGetWhiteIp import CompanyPostPayGetWhiteIp
+from .common.CompanyPostPayDelWhiteIp import CompanyPostPayDelWhiteIp
 from .enums.URL import URL
 from .ext.StrKit import get_params
 import urllib.request
 from urllib.parse import unquote
 
 
 # 动态代理 --提取动态代理
@@ -257,8 +261,48 @@
 def postPay_replace_white_ip(ip: PostPayReplaceWhiteIp) -> str:
     dic = ip.__dict__
     appkey = dic.get("key")
     params = get_params(dic,appkey)
     params = urllib.parse.quote(params,"?/&=")
     request = urllib.request.urlopen(URL.POSTPAY_REPLACEWHITEIP.value+params)
     result = unquote(request.read(),"utf-8")
+    return result
+
+# 按量付费(企业版) -- 提取ip
+def company_postpay_get_ips(ip: CompanyPostPayGetIps) -> str:
+    dic = ip.__dict__
+    appkey = dic.get("key")
+    params = get_params(dic,appkey)
+    params = urllib.parse.quote(params,"?/&=")
+    request = urllib.request.urlopen(URL.COMPANY_POSTPAY_GETIPS.value+params)
+    result = unquote(request.read(),"utf-8")
+    return result
+
+# 按量付费 -- 设置白名单
+def company_postpay_set_white_ip(ip:CompanyPostPaySetWhiteIp) -> str:
+    dic = ip.__dict__
+    appkey = dic.get("key")
+    params = get_params(dic,appkey)
+    params = urllib.parse.quote(params,"?/&=")
+    request = urllib.request.urlopen(URL.COMPANY_POSTPAY_SETWHITEIP.value+params)
+    result = unquote(request.read(),"utf-8")
+    return result
+
+# 按量付费 -- 获取白名单
+def company_postpay_get_white_ip(ip: CompanyPostPayGetWhiteIp) -> str:
+    dic = ip.__dict__
+    appkey = dic.get("key")
+    params = get_params(dic,appkey)
+    params = urllib.parse.quote(params,"?/&=")
+    request = urllib.request.urlopen(URL.COMPANY_POSTPAY_GETWHITEIP.value+params)
+    result = unquote(request.read(),"utf-8")
+    return result
+
+# 按量付费 -- 获取白名单
+def company_postpay_del_white_ip(ip: CompanyPostPayDelWhiteIp) -> str:
+    dic = ip.__dict__
+    appkey = dic.get("key")
+    params = get_params(dic,appkey)
+    params = urllib.parse.quote(params,"?/&=")
+    request = urllib.request.urlopen(URL.COMPANY_POSTPAY_DELWHITEIP.value+params)
+    result = unquote(request.read(),"utf-8")
     return result
```

### Comparing `juliang-1.0.1/juliangip/common/DynamicGetIps.py` & `juliang-1.1.0/juliangip/common/DynamicGetIps.py`

 * *Files identical despite different names*

### Comparing `juliang-1.0.1/juliangip/common/PostPayGetIps.py` & `juliang-1.1.0/juliangip/common/PostPayGetIps.py`

 * *Files identical despite different names*

### Comparing `juliang-1.0.1/juliangip/enums/URL.py` & `juliang-1.1.0/juliangip/enums/URL.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,13 +42,22 @@
     UNLIMITED_GETWHITEIP = DOMAIN + "/unlimited/getwhiteip"
     # 不限量 -- 替换白名单
     UNLIMITED_REPLACEWHITEIP = DOMAIN + "/unlimited/replaceWhiteIp"
     # 按量付费 -- 提取ip
     POSTPAY_GETIPS = DOMAIN + "/postpay/getips"
     # 按量付费 -- 检查ip有效性
     POSTPAY_CHECK = DOMAIN + "/postpay/check"
-    # 按量付费 -- 设置白名单
+    # 按量付费 -- 设置代理IP白名单
     POSTPAY_SETWHITEIP = DOMAIN + "/postpay/setwhiteip"
-    # 按量付费 -- 设置白名单
+    # 按量付费 -- 获取代理IP白名单
     POSTPAY_GETWHITEIP = DOMAIN + "/postpay/getwhiteip"
-    # 按量付费 -- 设置白名单
+    # 按量付费 -- 替换代理IP白名单
     POSTPAY_REPLACEWHITEIP = DOMAIN + "/postpay/replaceWhiteIp"
+
+    # 按量付费(企业版) -- 提取IP
+    COMPANY_POSTPAY_GETIPS = DOMAIN + "/company/postpay/getips"
+    # 按量付费(企业版) -- 设置代理IP白名单
+    COMPANY_POSTPAY_SETWHITEIP = DOMAIN + "/company/postpay/setwhiteip"
+    # 按量付费(企业版) -- 获取代理IP白名单
+    COMPANY_POSTPAY_GETWHITEIP = DOMAIN + "/company/postpay/getwhiteip"
+    # 按量付费(企业版) -- 删除代理IP白名单
+    COMPANY_POSTPAY_DELWHITEIP = DOMAIN + "/company/postpay/delwhiteip"
```

### Comparing `juliang-1.0.1/juliangip/ext/StrKit.py` & `juliang-1.1.0/juliangip/ext/StrKit.py`

 * *Files identical despite different names*

### Comparing `juliang-1.0.1/setup.py` & `juliang-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'juliang'
 DESCRIPTION = '巨量IP - API SDK for Python'
 URL = 'https://gitee.com/juliangip/juliang-python-sdk'
 EMAIL = 'juliangip@163.com'
 AUTHOR = 'juliangip'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '1.0.1'
+VERSION = '1.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

