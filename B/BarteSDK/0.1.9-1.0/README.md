# Comparing `tmp/bartesdk-0.1.9.tar.gz` & `tmp/BarteSDK-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bartesdk-0.1.9.tar", last modified: Tue May 21 10:36:14 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.tar", last modified: Thu May 30 10:08:57 2024, max compression
```

## Comparing `bartesdk-0.1.9.tar` & `BarteSDK-1.0.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:36:14.240140 bartesdk-0.1.9/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-21 10:23:50.000000 bartesdk-0.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:36:14.240140 bartesdk-0.1.9/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-21 10:23:50.000000 bartesdk-0.1.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:36:14.236140 bartesdk-0.1.9/bartesdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:36:14.240140 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 10:36:14.240140 bartesdk-0.1.9/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      612 2024-05-21 10:36:02.000000 bartesdk-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:57.136657 BarteSDK-1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:57.132657 BarteSDK-1.0/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9636 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 10:08:57.000000 BarteSDK-1.0/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:29.000000 BarteSDK-1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9636 2024-05-30 10:08:57.136657 BarteSDK-1.0/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 10:08:29.000000 BarteSDK-1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 10:08:57.136657 BarteSDK-1.0/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2003 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)     1638 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)     3049 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)     3002 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)     2451 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)     2631 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)     2730 2024-05-30 10:08:29.000000 BarteSDK-1.0/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 10:08:57.136657 BarteSDK-1.0/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      549 2024-05-30 10:08:39.000000 BarteSDK-1.0/setup.py
```

### Comparing `bartesdk-0.1.9/setup.py` & `BarteSDK-1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# setup.py
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='bartesdk',
-    version='0.1.9',
-    packages=find_packages(where='bartesdk'),
-    package_dir={'': 'bartesdk'},
+    name='BarteSDK',
+    version='1.0',
+    packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
     license='MIT',
```

