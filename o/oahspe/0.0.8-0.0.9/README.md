# Comparing `tmp/oahspe-0.0.8.tar.gz` & `tmp/oahspe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oahspe-0.0.8.tar", last modified: Wed May 29 11:57:43 2024, max compression
+gzip compressed data, was "oahspe-0.0.9.tar", last modified: Thu May 30 02:33:07 2024, max compression
```

## Comparing `oahspe-0.0.8.tar` & `oahspe-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,58 @@
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:43.177650 oahspe-0.0.8/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-27 02:28:54.000000 oahspe-0.0.8/LICENSE.txt
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-29 11:57:43.177650 oahspe-0.0.8/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-28 10:32:43.000000 oahspe-0.0.8/README.md
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:43.177650 oahspe-0.0.8/oahspe/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-27 02:28:54.000000 oahspe-0.0.8/oahspe/SSL.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    13322 2024-05-29 02:08:24.000000 oahspe-0.0.8/oahspe/crypt.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-27 02:28:54.000000 oahspe-0.0.8/oahspe/execute.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-27 02:28:54.000000 oahspe-0.0.8/oahspe/host.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8586 2024-05-29 05:08:22.000000 oahspe-0.0.8/oahspe/tool.py
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:43.177650 oahspe-0.0.8/oahspe.egg-info/
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/SOURCES.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/dependency_links.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/top_level.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-29 11:57:43.177650 oahspe-0.0.8/setup.cfg
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-29 11:57:29.000000 oahspe-0.0.8/setup.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 02:08:24.675270 oahspe-0.0.9/oahspe/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/SSL.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 05:08:27.249728 oahspe-0.0.9/oahspe/__pycache__/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    23192 2024-05-29 03:50:20.116461 oahspe-0.0.9/oahspe/__pycache__/crypt.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    18113 2024-05-29 05:08:27.249728 oahspe-0.0.9/oahspe/__pycache__/tool.cpython-312.pyc
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:01.564253 oahspe-0.0.9/oahspe/ali/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1444 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/ALB.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1638 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/CAS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     2141 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/CDN.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/CMS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    10077 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/ECS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      833 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/EOS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      499 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/ESS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1387 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/KMS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     4073 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/NAS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     2386 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/OSS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1999 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/RAM.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      499 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/SAS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     5790 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/ali/VPC.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:01.564253 oahspe-0.0.9/oahspe/ali/__init__.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 12:29:23.265403 oahspe-0.0.9/oahspe/ali/__pycache__/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     2388 2024-05-29 03:15:29.366310 oahspe-0.0.9/oahspe/ali/__pycache__/ALB.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3117 2024-05-29 03:15:29.346310 oahspe-0.0.9/oahspe/ali/__pycache__/CAS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3409 2024-05-29 03:15:29.350310 oahspe-0.0.9/oahspe/ali/__pycache__/CDN.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1192 2024-05-29 03:15:29.374310 oahspe-0.0.9/oahspe/ali/__pycache__/CMS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    17033 2024-05-29 03:15:29.322309 oahspe-0.0.9/oahspe/ali/__pycache__/ECS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1608 2024-05-29 11:32:35.075049 oahspe-0.0.9/oahspe/ali/__pycache__/EOS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1125 2024-05-29 03:15:29.426312 oahspe-0.0.9/oahspe/ali/__pycache__/ESS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     6841 2024-05-29 03:15:29.362310 oahspe-0.0.9/oahspe/ali/__pycache__/NAS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     5024 2024-05-29 03:15:29.430312 oahspe-0.0.9/oahspe/ali/__pycache__/OSS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     4231 2024-05-29 03:15:29.350310 oahspe-0.0.9/oahspe/ali/__pycache__/RAM.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1125 2024-05-29 03:15:29.394311 oahspe-0.0.9/oahspe/ali/__pycache__/SAS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    10126 2024-05-29 03:15:29.290308 oahspe-0.0.9/oahspe/ali/__pycache__/VPC.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      158 2024-05-29 12:29:23.265403 oahspe-0.0.9/oahspe/ali/__pycache__/__init__.cpython-312.pyc
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:08.984502 oahspe-0.0.9/oahspe/aws/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3937 2024-05-29 02:08:24.675270 oahspe-0.0.9/oahspe/aws/S3.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:08.984502 oahspe-0.0.9/oahspe/aws/__init__.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 03:12:30.107091 oahspe-0.0.9/oahspe/aws/__pycache__/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     5983 2024-05-28 03:12:30.107091 oahspe-0.0.9/oahspe/aws/__pycache__/S3.cpython-312.pyc
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:16.496755 oahspe-0.0.9/oahspe/clf/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      878 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/clf/DNS.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:16.496755 oahspe-0.0.9/oahspe/clf/__init__.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 03:15:29.362310 oahspe-0.0.9/oahspe/clf/__pycache__/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     2350 2024-05-29 03:15:29.362310 oahspe-0.0.9/oahspe/clf/__pycache__/DNS.cpython-312.pyc
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    13322 2024-05-29 02:08:24.675270 oahspe-0.0.9/oahspe/crypt.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/execute.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-27 02:28:54.408364 oahspe-0.0.9/oahspe/host.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8586 2024-05-29 05:08:22.269561 oahspe-0.0.9/oahspe/tool.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-30 02:33:07.693863 oahspe-0.0.9/oahspe.egg-info/
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-30 02:33:07.693863 oahspe-0.0.9/oahspe.egg-info/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      238 2024-05-30 02:33:07.709864 oahspe-0.0.9/oahspe.egg-info/SOURCES.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-30 02:33:07.693863 oahspe-0.0.9/oahspe.egg-info/dependency_links.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-30 02:33:07.693863 oahspe-0.0.9/oahspe.egg-info/top_level.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-27 02:28:54.408364 oahspe-0.0.9/LICENSE.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-30 02:11:46.306869 oahspe-0.0.9/README.md
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      696 2024-05-30 02:27:26.862428 oahspe-0.0.9/setup.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-30 02:23:40.774842 oahspe-0.0.9/setup.cfg
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-30 02:33:07.693863 oahspe-0.0.9/PKG-INFO
```

### Comparing `oahspe-0.0.8/LICENSE.txt` & `oahspe-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.8/PKG-INFO` & `oahspe-0.0.9/oahspe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.8/oahspe/SSL.py` & `oahspe-0.0.9/oahspe/SSL.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.8/oahspe/crypt.py` & `oahspe-0.0.9/oahspe/crypt.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.8/oahspe/execute.py` & `oahspe-0.0.9/oahspe/execute.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.8/oahspe/host.py` & `oahspe-0.0.9/oahspe/host.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.8/oahspe/tool.py` & `oahspe-0.0.9/oahspe/tool.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.8/oahspe.egg-info/PKG-INFO` & `oahspe-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.8/setup.py` & `oahspe-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from distutils.core import setup
 
+with open('version.txt', 'r') as f: version = f.read()
+
 setup(
   name = 'oahspe',
   packages = ['oahspe'],
   keywords = ['oahspe'],
-  version = '0.0.8',
+  version = version,
   author = 'quangproo',
   license='MIT',
   description = 'Cloud DevOps',
   author_email = 'contact@quang.pro',
   url = 'https://github.com/quangproo/oahspe',
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',
   install_requires = [],
```

