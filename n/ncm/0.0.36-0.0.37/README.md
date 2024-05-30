# Comparing `tmp/ncm-0.0.36.tar.gz` & `tmp/ncm-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.36.tar", last modified: Wed May 22 18:32:34 2024, max compression
+gzip compressed data, was "ncm-0.0.37.tar", last modified: Thu May 30 21:43:06 2024, max compression
```

## Comparing `ncm-0.0.36.tar` & `ncm-0.0.37.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:34.727606 ncm-0.0.36/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 18:32:22.000000 ncm-0.0.36/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-22 18:32:34.727606 ncm-0.0.36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-22 18:32:22.000000 ncm-0.0.36/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:34.723606 ncm-0.0.36/ncm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:22.000000 ncm-0.0.36/ncm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   149360 2024-05-22 18:32:22.000000 ncm-0.0.36/ncm/ncm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:34.723606 ncm-0.0.36/ncm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:32:34.727606 ncm-0.0.36/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      602 2024-05-22 18:32:32.000000 ncm-0.0.36/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:43:06.953964 ncm-0.0.37/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-30 21:42:56.000000 ncm-0.0.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-30 21:43:06.953964 ncm-0.0.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-30 21:42:56.000000 ncm-0.0.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:43:06.949964 ncm-0.0.37/ncm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:42:56.000000 ncm-0.0.37/ncm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149021 2024-05-30 21:42:56.000000 ncm-0.0.37/ncm/ncm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:43:06.953964 ncm-0.0.37/ncm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-30 21:43:06.000000 ncm-0.0.37/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 21:43:06.000000 ncm-0.0.37/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:43:06.000000 ncm-0.0.37/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 21:43:06.000000 ncm-0.0.37/ncm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 21:43:06.000000 ncm-0.0.37/ncm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:43:06.953964 ncm-0.0.37/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      602 2024-05-30 21:43:04.000000 ncm-0.0.37/setup.py
```

### Comparing `ncm-0.0.36/LICENSE` & `ncm-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.36/PKG-INFO` & `ncm-0.0.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.36
+Version: 0.0.37
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.36/README.md` & `ncm-0.0.37/README.md`

 * *Files identical despite different names*

### Comparing `ncm-0.0.36/ncm/ncm.py` & `ncm-0.0.37/ncm/ncm.py`

 * *Files 1% similar despite different names*

```diff
@@ -2474,46 +2474,41 @@
                           'fields',
                           'limit',
                           'sort']
 
         params = self.__parse_kwargs(kwargs, allowed_params)
         return self.__get_json(get_url, call_type, params=params)
     
-    def regrade(self, subscription_id, mac_or_serial_number, action="UPGRADE"):
+    def regrade(self, subscription_id, mac, action="UPGRADE"):
         """ 
         Applies a subscription to an asset.
         :param subscription_id: ID of the subscription to apply. See https://developer.cradlepoint.com/ for list of subscriptions.
-        :param mac_or_serial_number: MAC address or serial number of the asset to apply the subscription to. Can also be a list.
+        :param mac: MAC address of the asset to apply the subscription to. Can also be a list.
         :param action: Action to take. Default is "UPGRADE". Can also be "DOWNGRADE".
         """
 
         call_type = 'Subscription'
         post_url = f'{self.base_url}/asset_endpoints/regrades'
 
         payload = {
             "atomic:operations": []
         }
-        mac_or_serial_number = mac_or_serial_number if isinstance(mac_or_serial_number, list) else [mac_or_serial_number]
-        for smac in mac_or_serial_number:
+        mac = mac if isinstance(mac, list) else [mac]
+        for smac in mac:
             data = {
                 "op": "add",
                 "data": {
                     "type": "regrades",
                     "attributes": {
                         "action": action,
-                        "subscription_type": subscription_id
+                        "subscription_type": subscription_id,
+                        "mac_address": smac.replace(':','') if len(smac) == 17 else smac
                     }
                 }
             }
-            if len(smac) == 17:
-                data['data']['attributes']['mac_address'] = smac.replace(':','')
-            elif len(smac) == 12:
-                data['data']['attributes']['mac_address'] = smac
-            else:
-                data['data']['attributes']['serial_number'] = smac
             payload["atomic:operations"].append(data)
 
         ncm = self.session.post(post_url, json=payload)
         result = self._return_handler(ncm.status_code, ncm.json(), call_type)
         return result
 
     def get_regrades(self, **kwargs):
@@ -3854,15 +3849,15 @@
     """
     This NCM Client class provides functions for interacting with =
     the Cradlepoint NCM API. Full documentation of the Cradlepoint API can be
     found at: https://developer.cradlepoint.com
     """
 
     def __new__(cls, api_keys=None, api_key=None, **kwargs):
-        api_keys = api_keys or {}
+        api_keys = {**api_keys} or {}
         apiv3_key = api_keys.pop('token', None) or api_key
         v2 = bool(api_keys)
         v3 = bool(apiv3_key)
         if v2 and v3:
             return NcmClientv2v3(api_keys=api_keys, api_key=apiv3_key, **kwargs)
         if v2 or not (v2 or v3):
             return NcmClientv2(api_keys=api_keys, **kwargs)
```

### Comparing `ncm-0.0.36/ncm.egg-info/PKG-INFO` & `ncm-0.0.37/ncm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.36
+Version: 0.0.37
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.36/setup.py` & `ncm-0.0.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.36",
+    version="0.0.37",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cradlepoint/api-samples/tree/master/ncm",
     packages=find_packages(),
```

