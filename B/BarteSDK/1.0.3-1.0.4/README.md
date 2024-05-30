# Comparing `tmp/BarteSDK-1.0.3.tar.gz` & `tmp/BarteSDK-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-1.0.3.tar", last modified: Thu May 30 10:28:44 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.4.tar", last modified: Thu May 30 10:37:00 2024, max compression
```

## Comparing `BarteSDK-1.0.3.tar` & `BarteSDK-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:28:44.649063 BarteSDK-1.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:28:44.649063 BarteSDK-1.0.3/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:28:44.000000 BarteSDK-1.0.3/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:28:44.000000 BarteSDK-1.0.3/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:28:44.000000 BarteSDK-1.0.3/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:28:44.000000 BarteSDK-1.0.3/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:28:44.000000 BarteSDK-1.0.3/BarteSDK.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:28:44.649063 BarteSDK-1.0.3/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:28:44.649063 BarteSDK-1.0.3/bartesdk/
--rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1949 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/buyers.py
--rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/charges.py
--rwxrwxr-x   0 root         (0) root         (0)     3049 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/orders.py
--rwxrwxr-x   0 root         (0) root         (0)     3002 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/paymentlinks.py
--rwxrwxr-x   0 root         (0) root         (0)     2451 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/plans.py
--rwxrwxr-x   0 root         (0) root         (0)     2631 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/subscriptions.py
--rwxrwxr-x   0 root         (0) root         (0)     2730 2024-05-30 10:28:19.000000 BarteSDK-1.0.3/bartesdk/subseller.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:28:44.649063 BarteSDK-1.0.3/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 10:28:27.000000 BarteSDK-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:37:00.152273 BarteSDK-1.0.4/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:37:00.000000 BarteSDK-1.0.4/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     1949 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)     2702 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)     3229 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)     2034 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)     2333 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)     1751 2024-05-30 10:36:34.000000 BarteSDK-1.0.4/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:37:00.156273 BarteSDK-1.0.4/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 10:36:43.000000 BarteSDK-1.0.4/setup.py
```

### Comparing `BarteSDK-1.0.3/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-1.0.4/BarteSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.3
+Version: 1.0.4
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.3/PKG-INFO` & `BarteSDK-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.3
+Version: 1.0.4
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.3/README.md` & `BarteSDK-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.3/bartesdk/__init__.py` & `BarteSDK-1.0.4/bartesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.3/bartesdk/buyers.py` & `BarteSDK-1.0.4/bartesdk/buyers.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.3/bartesdk/charges.py` & `BarteSDK-1.0.4/bartesdk/charges.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.3/bartesdk/orders.py` & `BarteSDK-1.0.4/bartesdk/orders.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,53 +9,45 @@
         if env == "prd":
             return f'https://api.barte.com/{api_version}/orders'
         elif env == "sandbox":
             return f'https://sandbox-api.barte.com/{api_version}/orders'
         else:
             raise ValueError("Invalid environment specified")
 
-    def create(self, start_date, value, installments, title, description, payment, uuid_buyer, idempotency_key):
+    def create(self, **kwargs):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
-            'x-idempotency-key': idempotency_key,
-            'accept': '*/*'
-        }
-        payload = {
-            "startDate": start_date,
-            "value": value,
-            "installments": installments,
-            "title": title,
-            "description": description,
-            "payment": payment,
-            "uuidBuyer": uuid_buyer
+            'accept': 'application/json'
         }
+        payload = kwargs
         response = requests.post(self.base_url, headers=headers, json=payload)
         return response.status_code, response.json() if response.ok else response.text
 
     def get(self, **params):
         headers = {
             'X-Token-Api': self.api_key
         }
         response = requests.get(self.base_url, headers=headers, params=params)
         return response.json()
 
-    def update(self, uuid, metadata, description):
+    def update(self, uuid, **kwargs):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
             'accept': '*/*'
         }
-        payload = {
-            "metadata": metadata,
-            "description": description
-        }
-        url = f"{self.base_url}/{uuid}/basic-value"
-        response = requests.patch(url, headers=headers, json=payload)
-        return response.status_code, response.json() if response.ok else response.text
+        url = f"{self.base_url}/{uuid}"
+        payload = kwargs
+        response = requests.put(url, headers=headers, json=payload)
+        try:
+            response_data = response.json() if response.ok else response.text
+        except ValueError:
+            response_data = response.text
+        return response.status_code, response_data
 
     def getByUuid(self, uuid):
         headers = {
             'X-Token-Api': self.api_key,
             'accept': 'application/json'
         }
         url = f"{self.base_url}/{uuid}"
```

### Comparing `BarteSDK-1.0.3/bartesdk/paymentlinks.py` & `BarteSDK-1.0.4/bartesdk/paymentlinks.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,28 @@
             'X-Token-Api': self.api_key,
             'accept': 'application/json'
         }
         url = f"{self.base_url}/{uuid}"
         response = requests.get(url, headers=headers)
         return response.status_code, response.json() if response.ok else response.text
 
-    def update(self, uuid, payload):
+    def update(self, uuid, **kwargs):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
             'accept': '*/*'
         }
         url = f"{self.base_url}/{uuid}"
+        payload = kwargs
         response = requests.put(url, headers=headers, json=payload)
-        return response.status_code, response.ok
+        try:
+            response_data = response.json() if response.ok else response.text
+        except ValueError:
+            response_data = response.text
+        return response.status_code, response_data
 
     def cancel(self, uuid):
         headers = {
             'X-Token-Api': self.api_key,
             'accept': '*/*'
         }
         url = f"{self.base_url}/{uuid}"
@@ -45,20 +50,21 @@
         headers = {
             'X-Token-Api': self.api_key,
             'accept': '*/*'
         }
         response = requests.get(self.base_url, headers=headers, params=params)
         return response.status_code, response.json() if response.ok else response.text
 
-    def create(self, payload):
+    def create(self, **kwargs):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
-            'accept': '*/*'
+            'accept': 'application/json'
         }
+        payload = kwargs
         response = requests.post(self.base_url, headers=headers, json=payload)
         return response.status_code, response.json() if response.ok else response.text
 
     def maxInstallments(self):
         headers = {
             'X-Token-Api': self.api_key,
             'accept': '*/*',
```

### Comparing `BarteSDK-1.0.3/bartesdk/plans.py` & `BarteSDK-1.0.4/bartesdk/subscriptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import requests
 
-class plansAPI:
+class subscriptionsAPI:
     def __init__(self, api_key, env="prd", api_version="v2"):
         self.api_key = api_key
         self.base_url = self._get_base_url(env, api_version)
 
     def _get_base_url(self, env, api_version):
         if env == "prd":
-            return f'https://api.barte.com/{api_version}/plans'
+            return f'https://api.barte.com/{api_version}/subscriptions'
         elif env == "sandbox":
-            return f'https://sandbox-api.barte.com/{api_version}/plans'
+            return f'https://sandbox-api.barte.com/{api_version}/subscriptions'
         else:
             raise ValueError("Invalid environment specified")
 
     def getByUuid(self, uuid):
         headers = {
-            'X-Token-Api': self.api_key,
-            'accept': 'application/json'
+            'X-Token-Api': self.api_key
         }
         url = f"{self.base_url}/{uuid}"
         response = requests.get(url, headers=headers)
-        return response.status_code, response.json() if response.ok else response.text
+        return response.json()
 
-    def get(self):
+    def create(self, **kwargs):
         headers = {
             'X-Token-Api': self.api_key,
+            'Content-Type': 'application/json',
             'accept': 'application/json'
         }
-        response = requests.get(self.base_url, headers=headers)
+        payload = kwargs
+        response = requests.post(self.base_url, headers=headers, json=payload)
         return response.status_code, response.json() if response.ok else response.text
 
-    def create(self, title, description, active, bullets, values, accept_payment_methods):
+    def updateBasicValue(self, subscription_id, uuid_plan, basic_value_type, value_per_month, bank_slip_description):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
-            'accept': 'application/json'
+            'accept': '*/*'
         }
         payload = {
-            "title": title,
-            "description": description,
-            "active": active,
-            "bullets": bullets,
-            "values": values,
-            "acceptPaymentMethods": accept_payment_methods
+            "uuidPlan": uuid_plan,
+            "basicValueRequest": {
+                "type": basic_value_type,
+                "valuePerMonth": value_per_month
+            },
+            "bankSlipDescription": bank_slip_description
         }
-        response = requests.post(self.base_url, headers=headers, json=payload)
-        return response.status_code, response.json() if response.ok else response.text
-        
-    def update(self, uuid, title, description, active, bullets, values, accept_payment_methods):
+        url = f"{self.base_url}/{subscription_id}/basic-value"
+        response = requests.patch(url, headers=headers, json=payload)
+        return response.status_code, response.ok
+
+    def cancel(self, uuid):
+
         headers = {
             'X-Token-Api': self.api_key,
-            'Content-Type': 'application/json',
-            'accept': 'application/json'
-        }
-        payload = {
-            "title": title,
-            "description": description,
-            "active": active,
-            "bullets": bullets,
-            "values": values,
-            "acceptPaymentMethods": accept_payment_methods
+            'accept': '*/*'
         }
         url = f"{self.base_url}/{uuid}"
-        response = requests.put(url, headers=headers, json=payload)
+        response = requests.delete(url, headers=headers)
         return response.status_code, response.ok
 
+    def get(self, **params):
+        headers = {
+            'X-Token-Api': self.api_key
+        }
+        response = requests.get(self.base_url, headers=headers, params=params)
+        return response.json()
```

### Comparing `BarteSDK-1.0.3/setup.py` & `BarteSDK-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

