# Comparing `tmp/BarteSDK-1.0.4.tar.gz` & `tmp/BarteSDK-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-1.0.4.tar", last modified: Thu May 30 10:37:00 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.5.tar", last modified: Thu May 30 11:03:37 2024, max compression
```

## Comparing `BarteSDK-1.0.4.tar` & `BarteSDK-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:37:00.152273 BarteSDK-1.0.4/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/bartesdk/
--rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1949 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/buyers.py
--rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/charges.py
--rwxrwxr-x   0 root         (0) root         (0)     2702 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/orders.py
--rwxrwxr-x   0 root         (0) root         (0)     3229 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/paymentlinks.py
--rwxrwxr-x   0 root         (0) root         (0)     2034 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/plans.py
--rwxrwxr-x   0 root         (0) root         (0)     2333 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/subscriptions.py
--rwxrwxr-x   0 root         (0) root         (0)     1751 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/subseller.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 10:36:43.000000 BarteSDK-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:37.951640 BarteSDK-1.0.5/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     1580 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/base.py
+-rwxrwxr-x   0 root         (0) root         (0)      533 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)      535 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)      532 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)      552 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)      529 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)      553 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)      555 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 11:03:23.000000 BarteSDK-1.0.5/setup.py
```

### Comparing `BarteSDK-1.0.4/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-1.0.5/BarteSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.4
+Version: 1.0.5
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.4/PKG-INFO` & `BarteSDK-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.4
+Version: 1.0.5
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.4/README.md` & `BarteSDK-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.4/bartesdk/__init__.py` & `BarteSDK-1.0.5/bartesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.4/bartesdk/buyers.py` & `BarteSDK-1.0.5/bartesdk/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 import requests
 
-class buyersAPI:
-    def __init__(self, api_key, env="prd", api_version="v2"):
+class BaseAPI:
+    def __init__(self, api_key, base_url):
         self.api_key = api_key
-        self.base_url = self._get_base_url(env, api_version)
-
-    def _get_base_url(self, env, api_version):
-        if env == "prd":
-            return f'https://api.barte.com/{api_version}/buyers'
-        elif env == "sandbox":
-            return f'https://sandbox-api.barte.com/{api_version}/buyers'
-        else:
-            raise ValueError("Invalid environment specified")
+        self.base_url = base_url
 
     def create(self, **kwargs):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
             'accept': 'application/json'
         }
         payload = kwargs
         response = requests.post(self.base_url, headers=headers, json=payload)
         return response.status_code, response.json() if response.ok else response.text
 
-
     def get(self, **params):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
             'accept': 'application/json'
         }
         response = requests.get(self.base_url, headers=headers, params=params)
@@ -51,8 +42,7 @@
         payload = kwargs
         response = requests.put(url, headers=headers, json=payload)
         try:
             response_data = response.json() if response.ok else response.text
         except ValueError:
             response_data = response.text
         return response.status_code, response_data
-
```

### Comparing `BarteSDK-1.0.4/setup.py` & `BarteSDK-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='1.0.4',
+    version='1.0.5',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

