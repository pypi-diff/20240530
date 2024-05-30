# Comparing `tmp/cloudflare-dns-1.3.0.tar.gz` & `tmp/cloudflare_dns-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare-dns-1.3.0.tar", last modified: Sat Aug 12 16:49:06 2023, max compression
+gzip compressed data, was "cloudflare_dns-1.3.1.tar", last modified: Thu May 30 17:50:46 2024, max compression
```

## Comparing `cloudflare-dns-1.3.0.tar` & `cloudflare_dns-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 taozen     (504) staff       (20)        0 2023-08-12 16:49:06.178452 cloudflare-dns-1.3.0/
--rw-r--r--   0 taozen     (504) staff       (20)     1064 2023-08-12 16:30:59.000000 cloudflare-dns-1.3.0/LICENSE
--rw-r--r--   0 taozen     (504) staff       (20)       78 2023-08-12 16:30:59.000000 cloudflare-dns-1.3.0/MANIFEST.in
--rw-r--r--   0 taozen     (504) staff       (20)     5877 2023-08-12 16:49:06.178312 cloudflare-dns-1.3.0/PKG-INFO
--rw-r--r--   0 taozen     (504) staff       (20)     4713 2023-08-12 16:46:24.000000 cloudflare-dns-1.3.0/README.md
-drwxr-xr-x   0 taozen     (504) staff       (20)        0 2023-08-12 16:49:06.176364 cloudflare-dns-1.3.0/cloudflare_dns/
--rw-r--r--   0 taozen     (504) staff       (20)     2423 2023-08-12 16:30:59.000000 cloudflare-dns-1.3.0/cloudflare_dns/__init__.py
-drwxr-xr-x   0 taozen     (504) staff       (20)        0 2023-08-12 16:49:06.177957 cloudflare-dns-1.3.0/cloudflare_dns/__pycache__/
--rw-r--r--   0 taozen     (504) staff       (20)     4807 2023-08-12 16:43:51.000000 cloudflare-dns-1.3.0/cloudflare_dns/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 taozen     (504) staff       (20)    12977 2023-08-12 16:45:59.000000 cloudflare-dns-1.3.0/cloudflare_dns/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0 taozen     (504) staff       (20)     9339 2023-08-12 16:45:53.000000 cloudflare-dns-1.3.0/cloudflare_dns/cli.py
-drwxr-xr-x   0 taozen     (504) staff       (20)        0 2023-08-12 16:49:06.177518 cloudflare-dns-1.3.0/cloudflare_dns.egg-info/
--rw-r--r--   0 taozen     (504) staff       (20)     5877 2023-08-12 16:49:06.000000 cloudflare-dns-1.3.0/cloudflare_dns.egg-info/PKG-INFO
--rw-r--r--   0 taozen     (504) staff       (20)      416 2023-08-12 16:49:06.000000 cloudflare-dns-1.3.0/cloudflare_dns.egg-info/SOURCES.txt
--rw-r--r--   0 taozen     (504) staff       (20)        1 2023-08-12 16:49:06.000000 cloudflare-dns-1.3.0/cloudflare_dns.egg-info/dependency_links.txt
--rw-r--r--   0 taozen     (504) staff       (20)       59 2023-08-12 16:49:06.000000 cloudflare-dns-1.3.0/cloudflare_dns.egg-info/entry_points.txt
--rw-r--r--   0 taozen     (504) staff       (20)       11 2023-08-12 16:49:06.000000 cloudflare-dns-1.3.0/cloudflare_dns.egg-info/requires.txt
--rw-r--r--   0 taozen     (504) staff       (20)       15 2023-08-12 16:49:06.000000 cloudflare-dns-1.3.0/cloudflare_dns.egg-info/top_level.txt
--rw-r--r--   0 taozen     (504) staff       (20)       38 2023-08-12 16:49:06.178493 cloudflare-dns-1.3.0/setup.cfg
--rw-r--r--   0 taozen     (504) staff       (20)     1625 2023-08-12 16:44:24.000000 cloudflare-dns-1.3.0/setup.py
+drwxr-xr-x   0 taozen     (504) staff       (20)        0 2024-05-30 17:50:46.195013 cloudflare_dns-1.3.1/
+-rw-r--r--   0 taozen     (504) staff       (20)     1064 2023-08-12 16:30:59.000000 cloudflare_dns-1.3.1/LICENSE
+-rw-r--r--   0 taozen     (504) staff       (20)       78 2023-08-12 16:30:59.000000 cloudflare_dns-1.3.1/MANIFEST.in
+-rw-r--r--   0 taozen     (504) staff       (20)     5911 2024-05-30 17:50:46.194757 cloudflare_dns-1.3.1/PKG-INFO
+-rw-r--r--   0 taozen     (504) staff       (20)     4713 2023-08-12 16:46:24.000000 cloudflare_dns-1.3.1/README.md
+drwxr-xr-x   0 taozen     (504) staff       (20)        0 2024-05-30 17:50:46.189335 cloudflare_dns-1.3.1/cloudflare_dns/
+-rw-r--r--   0 taozen     (504) staff       (20)     2423 2023-08-12 16:30:59.000000 cloudflare_dns-1.3.1/cloudflare_dns/__init__.py
+drwxr-xr-x   0 taozen     (504) staff       (20)        0 2024-05-30 17:50:46.191102 cloudflare_dns-1.3.1/cloudflare_dns/__pycache__/
+-rw-r--r--   0 taozen     (504) staff       (20)     4807 2023-08-12 16:43:51.000000 cloudflare_dns-1.3.1/cloudflare_dns/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 taozen     (504) staff       (20)    12977 2023-08-12 16:45:59.000000 cloudflare_dns-1.3.1/cloudflare_dns/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0 taozen     (504) staff       (20)     9339 2023-08-12 16:45:53.000000 cloudflare_dns-1.3.1/cloudflare_dns/cli.py
+drwxr-xr-x   0 taozen     (504) staff       (20)        0 2024-05-30 17:50:46.194330 cloudflare_dns-1.3.1/cloudflare_dns.egg-info/
+-rw-r--r--   0 taozen     (504) staff       (20)     5911 2024-05-30 17:50:46.000000 cloudflare_dns-1.3.1/cloudflare_dns.egg-info/PKG-INFO
+-rw-r--r--   0 taozen     (504) staff       (20)      416 2024-05-30 17:50:46.000000 cloudflare_dns-1.3.1/cloudflare_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 taozen     (504) staff       (20)        1 2024-05-30 17:50:46.000000 cloudflare_dns-1.3.1/cloudflare_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 taozen     (504) staff       (20)       59 2024-05-30 17:50:46.000000 cloudflare_dns-1.3.1/cloudflare_dns.egg-info/entry_points.txt
+-rw-r--r--   0 taozen     (504) staff       (20)       19 2024-05-30 17:50:46.000000 cloudflare_dns-1.3.1/cloudflare_dns.egg-info/requires.txt
+-rw-r--r--   0 taozen     (504) staff       (20)       15 2024-05-30 17:50:46.000000 cloudflare_dns-1.3.1/cloudflare_dns.egg-info/top_level.txt
+-rw-r--r--   0 taozen     (504) staff       (20)       38 2024-05-30 17:50:46.195070 cloudflare_dns-1.3.1/setup.cfg
+-rw-r--r--   0 taozen     (504) staff       (20)     1633 2024-05-30 17:46:01.000000 cloudflare_dns-1.3.1/setup.py
```

### Comparing `cloudflare-dns-1.3.0/LICENSE` & `cloudflare_dns-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare-dns-1.3.0/PKG-INFO` & `cloudflare_dns-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflare-dns
-Version: 1.3.0
+Version: 1.3.1
 Summary: CLI and Python tool for managing Cloudflare DNS
 Home-page: https://github.com/ZigZagT/cloudflare-dns
 Author: Tao Z
 Project-URL: Bug Tracker, https://github.com/ZigZagT/cloudflare-dns/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cloudflare==2.19.*
 
 # cloudflare-dns
 
 CLI and Python tool for managing Cloudflare DNS
 
 https://github.com/ZigZagT/cloudflare-dns
```

### Comparing `cloudflare-dns-1.3.0/README.md` & `cloudflare_dns-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudflare-dns-1.3.0/cloudflare_dns/__init__.py` & `cloudflare_dns-1.3.1/cloudflare_dns/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudflare-dns-1.3.0/cloudflare_dns/__pycache__/__init__.cpython-311.pyc` & `cloudflare_dns-1.3.1/cloudflare_dns/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cloudflare-dns-1.3.0/cloudflare_dns/__pycache__/cli.cpython-311.pyc` & `cloudflare_dns-1.3.1/cloudflare_dns/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `cloudflare-dns-1.3.0/cloudflare_dns/cli.py` & `cloudflare_dns-1.3.1/cloudflare_dns/cli.py`

 * *Files identical despite different names*

### Comparing `cloudflare-dns-1.3.0/cloudflare_dns.egg-info/PKG-INFO` & `cloudflare_dns-1.3.1/cloudflare_dns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflare-dns
-Version: 1.3.0
+Version: 1.3.1
 Summary: CLI and Python tool for managing Cloudflare DNS
 Home-page: https://github.com/ZigZagT/cloudflare-dns
 Author: Tao Z
 Project-URL: Bug Tracker, https://github.com/ZigZagT/cloudflare-dns/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cloudflare==2.19.*
 
 # cloudflare-dns
 
 CLI and Python tool for managing Cloudflare DNS
 
 https://github.com/ZigZagT/cloudflare-dns
```

### Comparing `cloudflare-dns-1.3.0/setup.py` & `cloudflare_dns-1.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cloudflare-dns',
-    version='1.3.0',
+    version='1.3.1',
     packages=find_packages(include=['cloudflare_dns']),
     install_requires=[
-        'cloudflare'
+        'cloudflare==2.19.*'
     ],
     entry_points={
         'console_scripts': {
             'cloudflare-dns=cloudflare_dns.cli:main',
         }
     },
     description='CLI and Python tool for managing Cloudflare DNS',
```

