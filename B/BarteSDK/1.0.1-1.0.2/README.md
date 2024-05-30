# Comparing `tmp/BarteSDK-1.0.1.tar.gz` & `tmp/BarteSDK-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-1.0.1.tar", last modified: Thu May 30 10:18:23 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.2.tar", last modified: Thu May 30 10:26:15 2024, max compression
```

## Comparing `BarteSDK-1.0.1.tar` & `BarteSDK-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:18:23.856937 BarteSDK-1.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:18:23.852937 BarteSDK-1.0.1/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:18:23.000000 BarteSDK-1.0.1/BarteSDK.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:18:23.852937 BarteSDK-1.0.1/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:18:23.852937 BarteSDK-1.0.1/bartesdk/
--rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1825 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/buyers.py
--rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/charges.py
--rwxrwxr-x   0 root         (0) root         (0)     3049 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/orders.py
--rwxrwxr-x   0 root         (0) root         (0)     3002 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/paymentlinks.py
--rwxrwxr-x   0 root         (0) root         (0)     2451 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/plans.py
--rwxrwxr-x   0 root         (0) root         (0)     2631 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/subscriptions.py
--rwxrwxr-x   0 root         (0) root         (0)     2730 2024-05-30 10:17:53.000000 BarteSDK-1.0.1/bartesdk/subseller.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:18:23.856937 BarteSDK-1.0.1/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 10:18:03.000000 BarteSDK-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:26:15.670892 BarteSDK-1.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:26:15.666891 BarteSDK-1.0.2/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:26:15.000000 BarteSDK-1.0.2/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:26:15.000000 BarteSDK-1.0.2/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:26:15.000000 BarteSDK-1.0.2/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:26:15.000000 BarteSDK-1.0.2/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:26:15.000000 BarteSDK-1.0.2/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 10:26:15.670892 BarteSDK-1.0.2/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:26:15.670892 BarteSDK-1.0.2/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     1809 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)     3049 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)     3002 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)     2451 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)     2631 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)     2730 2024-05-30 10:25:48.000000 BarteSDK-1.0.2/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:26:15.670892 BarteSDK-1.0.2/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 10:25:57.000000 BarteSDK-1.0.2/setup.py
```

### Comparing `BarteSDK-1.0.1/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-1.0.2/BarteSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.1/PKG-INFO` & `BarteSDK-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.1
+Version: 1.0.2
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.1/README.md` & `BarteSDK-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/bartesdk/__init__.py` & `BarteSDK-1.0.2/bartesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/bartesdk/buyers.py` & `BarteSDK-1.0.2/bartesdk/buyers.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,9 +46,9 @@
             'X-Token-Api': self.api_key,
             'Content-Type': 'application/json',
             'accept': '*/*'
         }
         url = f"{self.base_url}/{uuid}"
         payload = kwargs
         response = requests.put(url, headers=headers, json=payload)
-        return response.status_code, response.json() if response.ok else response.text
+        return response.status_code, if response.ok else response.text
```

### Comparing `BarteSDK-1.0.1/bartesdk/charges.py` & `BarteSDK-1.0.2/bartesdk/charges.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/bartesdk/orders.py` & `BarteSDK-1.0.2/bartesdk/orders.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/bartesdk/paymentlinks.py` & `BarteSDK-1.0.2/bartesdk/paymentlinks.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/bartesdk/plans.py` & `BarteSDK-1.0.2/bartesdk/plans.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/bartesdk/subscriptions.py` & `BarteSDK-1.0.2/bartesdk/subscriptions.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/bartesdk/subseller.py` & `BarteSDK-1.0.2/bartesdk/subseller.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.1/setup.py` & `BarteSDK-1.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

