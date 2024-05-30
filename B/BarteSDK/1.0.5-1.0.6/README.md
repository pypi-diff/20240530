# Comparing `tmp/BarteSDK-1.0.5.tar.gz` & `tmp/BarteSDK-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-1.0.5.tar", last modified: Thu May 30 11:03:37 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.6.tar", last modified: Thu May 30 11:31:47 2024, max compression
```

## Comparing `BarteSDK-1.0.5.tar` & `BarteSDK-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:37.951640 BarteSDK-1.0.5/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:03:37.000000 BarteSDK-1.0.5/BarteSDK.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/bartesdk/
--rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1580 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/base.py
--rwxrwxr-x   0 root         (0) root         (0)      533 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/buyers.py
--rwxrwxr-x   0 root         (0) root         (0)      535 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/charges.py
--rwxrwxr-x   0 root         (0) root         (0)      532 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/orders.py
--rwxrwxr-x   0 root         (0) root         (0)      552 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/paymentlinks.py
--rwxrwxr-x   0 root         (0) root         (0)      529 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/plans.py
--rwxrwxr-x   0 root         (0) root         (0)      553 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/subscriptions.py
--rwxrwxr-x   0 root         (0) root         (0)      555 2024-05-30 11:03:14.000000 BarteSDK-1.0.5/bartesdk/subseller.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 11:03:37.955640 BarteSDK-1.0.5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 11:03:23.000000 BarteSDK-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:31:47.569648 BarteSDK-1.0.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:31:47.561648 BarteSDK-1.0.6/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:31:47.000000 BarteSDK-1.0.6/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-30 11:31:47.000000 BarteSDK-1.0.6/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 11:31:47.000000 BarteSDK-1.0.6/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:31:47.000000 BarteSDK-1.0.6/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:31:47.000000 BarteSDK-1.0.6/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 11:31:24.000000 BarteSDK-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:31:47.565648 BarteSDK-1.0.6/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 11:31:24.000000 BarteSDK-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:31:47.565648 BarteSDK-1.0.6/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 11:31:24.000000 BarteSDK-1.0.6/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     1854 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/base.py
+-rwxrwxr-x   0 root         (0) root         (0)      533 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)      535 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)      532 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)      552 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)      529 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)      553 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)      555 2024-05-30 11:31:25.000000 BarteSDK-1.0.6/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 11:31:47.569648 BarteSDK-1.0.6/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 11:31:33.000000 BarteSDK-1.0.6/setup.py
```

### Comparing `BarteSDK-1.0.5/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-1.0.6/BarteSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.5
+Version: 1.0.6
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.5/PKG-INFO` & `BarteSDK-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.5
+Version: 1.0.6
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.5/README.md` & `BarteSDK-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/__init__.py` & `BarteSDK-1.0.6/bartesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/base.py` & `BarteSDK-1.0.6/bartesdk/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,7 +42,16 @@
         payload = kwargs
         response = requests.put(url, headers=headers, json=payload)
         try:
             response_data = response.json() if response.ok else response.text
         except ValueError:
             response_data = response.text
         return response.status_code, response_data
+
+    def cancel(self, uuid):
+        headers = {
+            'X-Token-Api': self.api_key,
+            'accept': '*/*'
+        }
+        url = f"{self.base_url}/{uuid}"
+        response = requests.delete(url, headers=headers)
+        return response.status_code, response.ok
```

### Comparing `BarteSDK-1.0.5/bartesdk/buyers.py` & `BarteSDK-1.0.6/bartesdk/buyers.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/charges.py` & `BarteSDK-1.0.6/bartesdk/charges.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/orders.py` & `BarteSDK-1.0.6/bartesdk/orders.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/paymentlinks.py` & `BarteSDK-1.0.6/bartesdk/paymentlinks.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/plans.py` & `BarteSDK-1.0.6/bartesdk/plans.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/subscriptions.py` & `BarteSDK-1.0.6/bartesdk/subscriptions.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/bartesdk/subseller.py` & `BarteSDK-1.0.6/bartesdk/subseller.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.5/setup.py` & `BarteSDK-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

