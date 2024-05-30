# Comparing `tmp/ct_tcpchat-0.0.1.tar.gz` & `tmp/ct_tcpchat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ct_tcpchat-0.0.1.tar", last modified: Thu May 30 01:40:57 2024, max compression
+gzip compressed data, was "ct_tcpchat-0.1.0.tar", last modified: Thu May 30 01:43:28 2024, max compression
```

## Comparing `ct_tcpchat-0.0.1.tar` & `ct_tcpchat-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-30 01:40:57.328030 ct_tcpchat-0.0.1/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1067 2024-05-28 21:40:14.000000 ct_tcpchat-0.0.1/LICENSE
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     5904 2024-05-30 01:40:57.327804 ct_tcpchat-0.0.1/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     5390 2024-05-30 01:23:06.000000 ct_tcpchat-0.0.1/README.md
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-30 01:40:57.326698 ct_tcpchat-0.0.1/ct_tcpchat/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       45 2024-05-30 00:57:48.000000 ct_tcpchat-0.0.1/ct_tcpchat/__init__.py
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     8941 2024-05-30 00:57:31.000000 ct_tcpchat-0.0.1/ct_tcpchat/tcpchat.py
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-30 01:40:57.327440 ct_tcpchat-0.0.1/ct_tcpchat.egg-info/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     5904 2024-05-30 01:40:57.000000 ct_tcpchat-0.0.1/ct_tcpchat.egg-info/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      207 2024-05-30 01:40:57.000000 ct_tcpchat-0.0.1/ct_tcpchat.egg-info/SOURCES.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)        1 2024-05-30 01:40:57.000000 ct_tcpchat-0.0.1/ct_tcpchat.egg-info/dependency_links.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       11 2024-05-30 01:40:57.000000 ct_tcpchat-0.0.1/ct_tcpchat.egg-info/top_level.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       38 2024-05-30 01:40:57.328175 ct_tcpchat-0.0.1/setup.cfg
--rw-rw-r--   0 ricovanderhallen   (501) staff       (20)      697 2024-05-30 01:39:37.000000 ct_tcpchat-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:43:28.169111 ct_tcpchat-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 01:43:22.000000 ct_tcpchat-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-30 01:43:28.169111 ct_tcpchat-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-30 01:43:22.000000 ct_tcpchat-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:43:28.169111 ct_tcpchat-0.1.0/ct_tcpchat/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 01:43:22.000000 ct_tcpchat-0.1.0/ct_tcpchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-30 01:43:22.000000 ct_tcpchat-0.1.0/ct_tcpchat/tcpchat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:43:28.169111 ct_tcpchat-0.1.0/ct_tcpchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-30 01:43:28.000000 ct_tcpchat-0.1.0/ct_tcpchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 01:43:28.000000 ct_tcpchat-0.1.0/ct_tcpchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:43:28.000000 ct_tcpchat-0.1.0/ct_tcpchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 01:43:28.000000 ct_tcpchat-0.1.0/ct_tcpchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:43:28.169111 ct_tcpchat-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-30 01:43:22.000000 ct_tcpchat-0.1.0/setup.py
```

### Comparing `ct_tcpchat-0.0.1/LICENSE` & `ct_tcpchat-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ct_tcpchat-0.0.1/PKG-INFO` & `ct_tcpchat-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ct-tcpchat
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/TcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ct_tcpchat-0.0.1/README.md` & `ct_tcpchat-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ct_tcpchat-0.0.1/ct_tcpchat/tcpchat.py` & `ct_tcpchat-0.1.0/ct_tcpchat/tcpchat.py`

 * *Files identical despite different names*

### Comparing `ct_tcpchat-0.0.1/ct_tcpchat.egg-info/PKG-INFO` & `ct_tcpchat-0.1.0/ct_tcpchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ct-tcpchat
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/TcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ct_tcpchat-0.0.1/setup.py` & `ct_tcpchat-0.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ct-tcpchat",
-    version="0.0.1",
+    version="0.1.0",
     packages=find_packages(),
     install_requires=[],
     author="Clevrthings",
     author_email="info@clevrthings.com",
     description="A simple Python module for creating a TCP chat connection between two computers to send commands or information.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

