# Comparing `tmp/BarteSDK-1.0.tar.gz` & `tmp/BarteSDK-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-1.0.tar", last modified: Thu May 30 10:08:57 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.1.tar", last modified: Thu May 30 10:18:23 2024, max compression
```

## Comparing `BarteSDK-1.0.tar` & `BarteSDK-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:57.136657 BarteSDK-1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:57.132657 BarteSDK-1.0/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9636 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:29.000000 BarteSDK-1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9636 2024-05-30 10:08:57.136657 BarteSDK-1.0/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:08:29.000000 BarteSDK-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:57.136657 BarteSDK-1.0/bartesdk/
--rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2003 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/buyers.py
--rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/charges.py
--rwxrwxr-x   0 root         (0) root         (0)     3049 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/orders.py
--rwxrwxr-x   0 root         (0) root         (0)     3002 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/paymentlinks.py
--rwxrwxr-x   0 root         (0) root         (0)     2451 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/plans.py
--rwxrwxr-x   0 root         (0) root         (0)     2631 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/subscriptions.py
--rwxrwxr-x   0 root         (0) root         (0)     2730 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/subseller.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:08:57.136657 BarteSDK-1.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      549 2024-05-30 10:08:39.000000 BarteSDK-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:18:23.856937 BarteSDK-1.0.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:18:23.852937 BarteSDK-1.0.1/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:18:23.852937 BarteSDK-1.0.1/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:18:23.852937 BarteSDK-1.0.1/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     1825 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)     3049 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)     3002 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)     2451 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)     2631 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)     2730 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:18:23.856937 BarteSDK-1.0.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 10:18:03.000000 BarteSDK-1.0.1/setup.py
```

### Comparing `BarteSDK-1.0/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-1.0.1/BarteSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0
+Version: 1.0.1
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0/PKG-INFO` & `BarteSDK-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0
+Version: 1.0.1
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0/README.md` & `BarteSDK-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0/bartesdk/__init__.py` & `BarteSDK-1.0.1/bartesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0/bartesdk/buyers.py` & `BarteSDK-1.0.1/bartesdk/orders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,84 @@
 import requests
 
-class buyersAPI:
+class ordersAPI:
     def __init__(self, api_key, env="prd", api_version="v2"):
         self.api_key = api_key
         self.base_url = self._get_base_url(env, api_version)
 
     def _get_base_url(self, env, api_version):
         if env == "prd":
-            return f'https://api.barte.com/{api_version}/buyers'
+            return f'https://api.barte.com/{api_version}/orders'
         elif env == "sandbox":
-            return f'https://sandbox-api.barte.com/{api_version}/buyers'
+            return f'https://sandbox-api.barte.com/{api_version}/orders'
         else:
             raise ValueError("Invalid environment specified")
 
-    def create(self, **kwargs):
+    def create(self, start_date, value, installments, title, description, payment, uuid_buyer, idempotency_key):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
-            'accept': 'application/json'
+            'x-idempotency-key': idempotency_key,
+            'accept': '*/*'
+        }
+        payload = {
+            "startDate": start_date,
+            "value": value,
+            "installments": installments,
+            "title": title,
+            "description": description,
+            "payment": payment,
+            "uuidBuyer": uuid_buyer
         }
-        payload = kwargs
         response = requests.post(self.base_url, headers=headers, json=payload)
         return response.status_code, response.json() if response.ok else response.text
 
-
     def get(self, **params):
         headers = {
-            'X-Token-Api': self.api_key,
-            'Content-Type': 'application/json',
-            'accept': 'application/json'
+            'X-Token-Api': self.api_key
         }
         response = requests.get(self.base_url, headers=headers, params=params)
         return response.json()
 
+    def update(self, uuid, metadata, description):
+        headers = {
+            'X-Token-Api': self.api_key,
+            'Content-Type': 'application/json',
+            'accept': '*/*'
+        }
+        payload = {
+            "metadata": metadata,
+            "description": description
+        }
+        url = f"{self.base_url}/{uuid}/basic-value"
+        response = requests.patch(url, headers=headers, json=payload)
+        return response.status_code, response.json() if response.ok else response.text
+
     def getByUuid(self, uuid):
         headers = {
-            'X-Token-Api': self.api_key
+            'X-Token-Api': self.api_key,
+            'accept': 'application/json'
         }
         url = f"{self.base_url}/{uuid}"
         response = requests.get(url, headers=headers)
-        return response.json()
+        return response.status_code, response.json() if response.ok else response.text
 
-    def update(self, uuid, name, email, countryCode, phone, alternativeEmail):
+    def cancel(self, uuid):
         headers = {
             'X-Token-Api': self.api_key,
-            'Content-Type': 'application/json',
             'accept': '*/*'
         }
         url = f"{self.base_url}/{uuid}"
-        payload = {
-            'name': name,
-            'email': email,
-            'countryCode': countryCode,
-            'phone': phone,
-            'alternativeEmail': alternativeEmail
+        response = requests.delete(url, headers=headers)
+        return response.status_code, response.json() if response.ok else response.text
+
+    def calculateInstallments(self, amount, max_installments):
+        headers = {
+            'X-Token-Api': self.api_key,
+            'accept': '*/*'
         }
-        response = requests.put(url, headers=headers, json=payload)
-        return response.status_code, response.ok
+        params = {
+            'amount': amount,
+            'maxInstallments': max_installments
+        }
+        response = requests.get(self.base_url, headers=headers, params=params)
+        return response.status_code, response.json() if response.ok else response.text
```

### Comparing `BarteSDK-1.0/bartesdk/charges.py` & `BarteSDK-1.0.1/bartesdk/charges.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0/bartesdk/orders.py` & `BarteSDK-1.0.1/bartesdk/subscriptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,74 @@
 import requests
 
-class ordersAPI:
+class subscriptionsAPI:
     def __init__(self, api_key, env="prd", api_version="v2"):
         self.api_key = api_key
         self.base_url = self._get_base_url(env, api_version)
 
     def _get_base_url(self, env, api_version):
         if env == "prd":
-            return f'https://api.barte.com/{api_version}/orders'
+            return f'https://api.barte.com/{api_version}/subscriptions'
         elif env == "sandbox":
-            return f'https://sandbox-api.barte.com/{api_version}/orders'
+            return f'https://sandbox-api.barte.com/{api_version}/subscriptions'
         else:
             raise ValueError("Invalid environment specified")
 
-    def create(self, start_date, value, installments, title, description, payment, uuid_buyer, idempotency_key):
+    def getByUuid(self, uuid):
+        headers = {
+            'X-Token-Api': self.api_key
+        }
+        url = f"{self.base_url}/{uuid}"
+        response = requests.get(url, headers=headers)
+        return response.json()
+
+    def create(self, uuid_plan, basic_value, additional_value, payment, uuid_buyer, start_date):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
-            'x-idempotency-key': idempotency_key,
-            'accept': '*/*'
+            'accept': 'application/json'
         }
         payload = {
-            "startDate": start_date,
-            "value": value,
-            "installments": installments,
-            "title": title,
-            "description": description,
+            "uuidPlan": uuid_plan,
+            "basicValue": basic_value,
+            "additionalValue": additional_value,
             "payment": payment,
-            "uuidBuyer": uuid_buyer
+            "uuidBuyer": uuid_buyer,
+            "startDate": start_date
         }
         response = requests.post(self.base_url, headers=headers, json=payload)
         return response.status_code, response.json() if response.ok else response.text
 
-    def get(self, **params):
-        headers = {
-            'X-Token-Api': self.api_key
-        }
-        response = requests.get(self.base_url, headers=headers, params=params)
-        return response.json()
-
-    def update(self, uuid, metadata, description):
+    def updateBasicValue(self, subscription_id, uuid_plan, basic_value_type, value_per_month, bank_slip_description):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
             'accept': '*/*'
         }
         payload = {
-            "metadata": metadata,
-            "description": description
+            "uuidPlan": uuid_plan,
+            "basicValueRequest": {
+                "type": basic_value_type,
+                "valuePerMonth": value_per_month
+            },
+            "bankSlipDescription": bank_slip_description
         }
-        url = f"{self.base_url}/{uuid}/basic-value"
+        url = f"{self.base_url}/{subscription_id}/basic-value"
         response = requests.patch(url, headers=headers, json=payload)
-        return response.status_code, response.json() if response.ok else response.text
-
-    def getByUuid(self, uuid):
-        headers = {
-            'X-Token-Api': self.api_key,
-            'accept': 'application/json'
-        }
-        url = f"{self.base_url}/{uuid}"
-        response = requests.get(url, headers=headers)
-        return response.status_code, response.json() if response.ok else response.text
+        return response.status_code, response.ok
 
     def cancel(self, uuid):
+
         headers = {
             'X-Token-Api': self.api_key,
             'accept': '*/*'
         }
         url = f"{self.base_url}/{uuid}"
         response = requests.delete(url, headers=headers)
-        return response.status_code, response.json() if response.ok else response.text
+        return response.status_code, response.ok
 
-    def calculateInstallments(self, amount, max_installments):
+    def get(self, **params):
         headers = {
-            'X-Token-Api': self.api_key,
-            'accept': '*/*'
-        }
-        params = {
-            'amount': amount,
-            'maxInstallments': max_installments
+            'X-Token-Api': self.api_key
         }
         response = requests.get(self.base_url, headers=headers, params=params)
-        return response.status_code, response.json() if response.ok else response.text
+        return response.json()
```

### Comparing `BarteSDK-1.0/bartesdk/paymentlinks.py` & `BarteSDK-1.0.1/bartesdk/paymentlinks.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0/bartesdk/plans.py` & `BarteSDK-1.0.1/bartesdk/plans.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0/bartesdk/subscriptions.py` & `BarteSDK-1.0.1/bartesdk/subseller.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 import requests
 
-class subscriptionsAPI:
+class subsellerAPI:
     def __init__(self, api_key, env="prd", api_version="v2"):
         self.api_key = api_key
         self.base_url = self._get_base_url(env, api_version)
 
     def _get_base_url(self, env, api_version):
         if env == "prd":
-            return f'https://api.barte.com/{api_version}/subscriptions'
+            return f'https://api.barte.com/{api_version}/seller/subseller'
         elif env == "sandbox":
-            return f'https://sandbox-api.barte.com/{api_version}/subscriptions'
+            return f'https://sandbox-api.barte.com/{api_version}/seller/subseller'
         else:
             raise ValueError("Invalid environment specified")
 
-    def getByUuid(self, uuid):
+    def getByID(self, id):
         headers = {
-            'X-Token-Api': self.api_key
+            'X-Token-Api': self.api_key,
+            'accept': '*/*'
         }
-        url = f"{self.base_url}/{uuid}"
+        url = f"{self.base_url}/{id}"
         response = requests.get(url, headers=headers)
-        return response.json()
+        return response.status_code, response.json() if response.ok else response.text
 
-    def create(self, uuid_plan, basic_value, additional_value, payment, uuid_buyer, start_date):
+    def update(self, subseller_id, name, document_type, document, alternative_email, owner_name, owner_document, birthdate, opening_date, payment_type, payment_value, description):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
-            'accept': 'application/json'
+            'accept': '*/*'
         }
         payload = {
-            "uuidPlan": uuid_plan,
-            "basicValue": basic_value,
-            "additionalValue": additional_value,
-            "payment": payment,
-            "uuidBuyer": uuid_buyer,
-            "startDate": start_date
+            "name": name,
+            "documentType": document_type,
+            "document": document,
+            "alternativeEmail": alternative_email,
+            "ownerName": owner_name,
+            "ownerDocument": owner_document,
+            "birthdate": birthdate,
+            "openingDate": opening_date,
+            "paymentType": payment_type,
+            "paymentValue": payment_value,
+            "description": description
         }
-        response = requests.post(self.base_url, headers=headers, json=payload)
+        url = f"{self.base_url}/{subseller_id}"
+        response = requests.patch(url, headers=headers, json=payload)
         return response.status_code, response.json() if response.ok else response.text
 
-    def updateBasicValue(self, subscription_id, uuid_plan, basic_value_type, value_per_month, bank_slip_description):
+    def create(self, name, document_type, document, phone, alternative_email, address, account, contact, payment_type, payment_value, description):
         headers = {
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
             'accept': '*/*'
         }
         payload = {
-            "uuidPlan": uuid_plan,
-            "basicValueRequest": {
-                "type": basic_value_type,
-                "valuePerMonth": value_per_month
-            },
-            "bankSlipDescription": bank_slip_description
+            "name": name,
+            "documentType": document_type,
+            "document": document,
+            "phone": phone,
+            "alternativeEmail": alternative_email,
+            "address": address,
+            "account": account,
+            "contact": contact,
+            "paymentType": payment_type,
+            "paymentValue": payment_value,
+            "description": description
         }
-        url = f"{self.base_url}/{subscription_id}/basic-value"
-        response = requests.patch(url, headers=headers, json=payload)
-        return response.status_code, response.ok
-
-    def cancel(self, uuid):
+        response = requests.post(self.base_url, headers=headers, json=payload)
+        return response.status_code, response.json() if response.ok else response.text
 
-        headers = {
-            'X-Token-Api': self.api_key,
-            'accept': '*/*'
-        }
-        url = f"{self.base_url}/{uuid}"
-        response = requests.delete(url, headers=headers)
-        return response.status_code, response.ok
 
-    def get(self, **params):
-        headers = {
-            'X-Token-Api': self.api_key
-        }
-        response = requests.get(self.base_url, headers=headers, params=params)
-        return response.json()
```

### Comparing `BarteSDK-1.0/setup.py` & `BarteSDK-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='1.0',
+    version='1.0.1',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

