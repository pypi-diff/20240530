# Comparing `tmp/oahspe-0.0.7.tar.gz` & `tmp/oahspe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oahspe-0.0.7.tar", last modified: Tue May 28 15:10:46 2024, max compression
+gzip compressed data, was "oahspe-0.0.8.tar", last modified: Wed May 29 11:57:43 2024, max compression
```

## Comparing `oahspe-0.0.7.tar` & `oahspe-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 15:10:46.608739 oahspe-0.0.7/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-26 13:20:10.000000 oahspe-0.0.7/LICENSE.txt
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 15:10:46.608739 oahspe-0.0.7/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-28 12:40:50.000000 oahspe-0.0.7/README.md
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 15:10:46.608739 oahspe-0.0.7/oahspe/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-26 16:33:26.000000 oahspe-0.0.7/oahspe/SSL.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    13322 2024-05-28 12:11:32.000000 oahspe-0.0.7/oahspe/crypt.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-26 15:35:40.000000 oahspe-0.0.7/oahspe/execute.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-26 13:20:10.000000 oahspe-0.0.7/oahspe/host.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8558 2024-05-28 15:06:17.000000 oahspe-0.0.7/oahspe/tool.py
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-28 15:10:46.608739 oahspe-0.0.7/oahspe.egg-info/
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/SOURCES.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/dependency_links.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-28 15:10:46.000000 oahspe-0.0.7/oahspe.egg-info/top_level.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-28 15:10:46.608739 oahspe-0.0.7/setup.cfg
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-28 15:10:16.000000 oahspe-0.0.7/setup.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:43.177650 oahspe-0.0.8/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-27 02:28:54.000000 oahspe-0.0.8/LICENSE.txt
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-29 11:57:43.177650 oahspe-0.0.8/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-28 10:32:43.000000 oahspe-0.0.8/README.md
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:43.177650 oahspe-0.0.8/oahspe/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3841 2024-05-27 02:28:54.000000 oahspe-0.0.8/oahspe/SSL.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    13322 2024-05-29 02:08:24.000000 oahspe-0.0.8/oahspe/crypt.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8461 2024-05-27 02:28:54.000000 oahspe-0.0.8/oahspe/execute.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-27 02:28:54.000000 oahspe-0.0.8/oahspe/host.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     8586 2024-05-29 05:08:22.000000 oahspe-0.0.8/oahspe/tool.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-29 11:57:43.177650 oahspe-0.0.8/oahspe.egg-info/
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      228 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/SOURCES.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/dependency_links.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-29 11:57:43.000000 oahspe-0.0.8/oahspe.egg-info/top_level.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-29 11:57:43.177650 oahspe-0.0.8/setup.cfg
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-29 11:57:29.000000 oahspe-0.0.8/setup.py
```

### Comparing `oahspe-0.0.7/LICENSE.txt` & `oahspe-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.7/PKG-INFO` & `oahspe-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.7/oahspe/SSL.py` & `oahspe-0.0.8/oahspe/SSL.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.7/oahspe/crypt.py` & `oahspe-0.0.8/oahspe/crypt.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.7/oahspe/execute.py` & `oahspe-0.0.8/oahspe/execute.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.7/oahspe/host.py` & `oahspe-0.0.8/oahspe/host.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.7/oahspe/tool.py` & `oahspe-0.0.8/oahspe/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime
 import os, hashlib, base64
 
 
 def tmp_write(content):
   tmp = gen_uuid()
   tmp = f'tmp/{tmp}'
+  os.system('mkdir -p tmp')
   if isinstance(content, str):
     mode = 'w'
   else:
     content = to_byte(content)
     mode = 'wb'
   with open(tmp, mode) as f:
     f.write(content)
```

### Comparing `oahspe-0.0.7/oahspe.egg-info/PKG-INFO` & `oahspe-0.0.8/oahspe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.7/setup.py` & `oahspe-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
   name = 'oahspe',
   packages = ['oahspe'],
   keywords = ['oahspe'],
-  version = '0.0.7',
+  version = '0.0.8',
   author = 'quangproo',
   license='MIT',
   description = 'Cloud DevOps',
   author_email = 'contact@quang.pro',
   url = 'https://github.com/quangproo/oahspe',
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',
   install_requires = [],
```

