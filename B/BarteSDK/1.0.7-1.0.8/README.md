# Comparing `tmp/BarteSDK-1.0.7.tar.gz` & `tmp/BarteSDK-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-1.0.7.tar", last modified: Thu May 30 11:43:05 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.8.tar", last modified: Thu May 30 11:58:06 2024, max compression
```

## Comparing `BarteSDK-1.0.7.tar` & `BarteSDK-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:43:05.487471 BarteSDK-1.0.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:43:05.483471 BarteSDK-1.0.7/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:43:05.000000 BarteSDK-1.0.7/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-30 11:43:05.000000 BarteSDK-1.0.7/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 11:43:05.000000 BarteSDK-1.0.7/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:43:05.000000 BarteSDK-1.0.7/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:43:05.000000 BarteSDK-1.0.7/BarteSDK.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:43:05.487471 BarteSDK-1.0.7/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:43:05.487471 BarteSDK-1.0.7/bartesdk/
--rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1892 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/base.py
--rwxrwxr-x   0 root         (0) root         (0)      533 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/buyers.py
--rwxrwxr-x   0 root         (0) root         (0)      535 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/charges.py
--rwxrwxr-x   0 root         (0) root         (0)      532 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/orders.py
--rwxrwxr-x   0 root         (0) root         (0)      552 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/paymentlinks.py
--rwxrwxr-x   0 root         (0) root         (0)      529 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/plans.py
--rwxrwxr-x   0 root         (0) root         (0)      553 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/subscriptions.py
--rwxrwxr-x   0 root         (0) root         (0)      555 2024-05-30 11:42:41.000000 BarteSDK-1.0.7/bartesdk/subseller.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 11:43:05.487471 BarteSDK-1.0.7/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 11:42:50.000000 BarteSDK-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:58:06.116604 BarteSDK-1.0.8/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2216 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/base.py
+-rwxrwxr-x   0 root         (0) root         (0)      198 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)      198 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)      196 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)      209 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)      194 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)      210 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)      210 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 11:57:51.000000 BarteSDK-1.0.8/setup.py
```

### Comparing `BarteSDK-1.0.7/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-1.0.8/BarteSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.7
+Version: 1.0.8
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.7/PKG-INFO` & `BarteSDK-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.7
+Version: 1.0.8
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.7/README.md` & `BarteSDK-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.7/bartesdk/__init__.py` & `BarteSDK-1.0.8/bartesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.7/setup.py` & `BarteSDK-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

