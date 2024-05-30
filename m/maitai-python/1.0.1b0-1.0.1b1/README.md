# Comparing `tmp/maitai_python-1.0.1b0.tar.gz` & `tmp/maitai_python-1.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai_python-1.0.1b0.tar", last modified: Wed May 29 18:14:18 2024, max compression
+gzip compressed data, was "maitai_python-1.0.1b1.tar", last modified: Thu May 30 21:32:37 2024, max compression
```

## Comparing `maitai_python-1.0.1b0.tar` & `maitai_python-1.0.1b1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.609357 maitai_python-1.0.1b0/
--rw-r--r--   0 ian        (501) staff       (20)     1726 2024-05-29 18:14:18.609127 maitai_python-1.0.1b0/PKG-INFO
--rw-r--r--   0 ian        (501) staff       (20)     1220 2024-05-29 18:12:26.000000 maitai_python-1.0.1b0/README.md
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.605946 maitai_python-1.0.1b0/maitai/
--rw-r--r--   0 ian        (501) staff       (20)      459 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai/__init__.py
--rw-r--r--   0 ian        (501) staff       (20)     2249 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai/_config.py
--rw-r--r--   0 ian        (501) staff       (20)      495 2024-05-22 20:55:51.000000 maitai_python-1.0.1b0/maitai/_config_listener_thread.py
--rw-r--r--   0 ian        (501) staff       (20)    12978 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai/_evaluator.py
--rw-r--r--   0 ian        (501) staff       (20)     4659 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai/_inference.py
--rw-r--r--   0 ian        (501) staff       (20)     1135 2024-05-22 20:55:51.000000 maitai_python-1.0.1b0/maitai/_maitai_client.py
--rw-r--r--   0 ian        (501) staff       (20)    16039 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai/_openai.py
--rw-r--r--   0 ian        (501) staff       (20)      236 2024-05-22 20:55:51.000000 maitai_python-1.0.1b0/maitai/_openai_types.py
--rw-r--r--   0 ian        (501) staff       (20)     1307 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai/_types.py
--rw-r--r--   0 ian        (501) staff       (20)     4243 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai/_utils.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.606121 maitai_python-1.0.1b0/maitai_common/
--rw-r--r--   0 ian        (501) staff       (20)        0 2024-05-22 20:55:51.000000 maitai_python-1.0.1b0/maitai_common/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.606563 maitai_python-1.0.1b0/maitai_common/processes/
--rw-r--r--   0 ian        (501) staff       (20)        0 2024-05-22 20:55:51.000000 maitai_python-1.0.1b0/maitai_common/processes/__init__.py
--rw-r--r--   0 ian        (501) staff       (20)     1977 2024-05-29 17:38:55.000000 maitai_python-1.0.1b0/maitai_common/processes/io_thread.py
--rw-r--r--   0 ian        (501) staff       (20)     3392 2024-05-22 20:55:51.000000 maitai_python-1.0.1b0/maitai_common/processes/websocket_listener_thread.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.606889 maitai_python-1.0.1b0/maitai_common/utils/
--rw-r--r--   0 ian        (501) staff       (20)        0 2024-05-28 20:03:48.000000 maitai_python-1.0.1b0/maitai_common/utils/__init__.py
--rw-r--r--   0 ian        (501) staff       (20)      407 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_common/utils/proto_utils.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.607011 maitai_python-1.0.1b0/maitai_gen/
--rw-r--r--   0 ian        (501) staff       (20)        0 2024-05-29 17:38:39.000000 maitai_python-1.0.1b0/maitai_gen/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.607123 maitai_python-1.0.1b0/maitai_gen/application/
--rw-r--r--   0 ian        (501) staff       (20)     1364 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/application/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.607268 maitai_python-1.0.1b0/maitai_gen/chat/
--rw-r--r--   0 ian        (501) staff       (20)     9847 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/chat/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.607581 maitai_python-1.0.1b0/maitai_gen/company/
--rw-r--r--   0 ian        (501) staff       (20)      641 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/company/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.607712 maitai_python-1.0.1b0/maitai_gen/inference/
--rw-r--r--   0 ian        (501) staff       (20)      600 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/inference/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.607847 maitai_python-1.0.1b0/maitai_gen/notification/
--rw-r--r--   0 ian        (501) staff       (20)     1198 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/notification/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.607978 maitai_python-1.0.1b0/maitai_gen/sandbox/
--rw-r--r--   0 ian        (501) staff       (20)     1460 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/sandbox/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.608100 maitai_python-1.0.1b0/maitai_gen/sentinel/
--rw-r--r--   0 ian        (501) staff       (20)     1518 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/sentinel/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.608234 maitai_python-1.0.1b0/maitai_gen/session/
--rw-r--r--   0 ian        (501) staff       (20)      886 2024-05-29 17:42:03.000000 maitai_python-1.0.1b0/maitai_gen/session/__init__.py
-drwxr-xr-x   0 ian        (501) staff       (20)        0 2024-05-29 18:14:18.608930 maitai_python-1.0.1b0/maitai_python.egg-info/
--rw-r--r--   0 ian        (501) staff       (20)     1726 2024-05-29 18:14:18.000000 maitai_python-1.0.1b0/maitai_python.egg-info/PKG-INFO
--rw-r--r--   0 ian        (501) staff       (20)      915 2024-05-29 18:14:18.000000 maitai_python-1.0.1b0/maitai_python.egg-info/SOURCES.txt
--rw-r--r--   0 ian        (501) staff       (20)        1 2024-05-29 18:14:18.000000 maitai_python-1.0.1b0/maitai_python.egg-info/dependency_links.txt
--rw-r--r--   0 ian        (501) staff       (20)       70 2024-05-29 18:14:18.000000 maitai_python-1.0.1b0/maitai_python.egg-info/requires.txt
--rw-r--r--   0 ian        (501) staff       (20)       32 2024-05-29 18:14:18.000000 maitai_python-1.0.1b0/maitai_python.egg-info/top_level.txt
--rw-r--r--   0 ian        (501) staff       (20)       38 2024-05-29 18:14:18.609401 maitai_python-1.0.1b0/setup.cfg
--rw-r--r--   0 ian        (501) staff       (20)      767 2024-05-29 18:13:28.000000 maitai_python-1.0.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1721 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     1215 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.664278 maitai_python-1.0.1b1/maitai/
+-rw-r--r--   0 runner    (1001) runner    (1001)      459 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/maitai/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2249 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/maitai/_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      495 2024-05-30 21:32:04.000000 maitai_python-1.0.1b1/maitai/_config_listener_thread.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12978 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_evaluator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4659 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_inference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1135 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_maitai_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    16039 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_openai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      236 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_openai_types.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1307 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_types.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4243 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai/_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.664278 maitai_python-1.0.1b1/maitai_common/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.664278 maitai_python-1.0.1b1/maitai_common/processes/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/processes/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1977 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/processes/io_thread.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3392 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/processes/websocket_listener_thread.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_common/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      407 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_common/utils/proto_utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/application/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1364 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/application/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/chat/
+-rw-r--r--   0 runner    (1001) runner    (1001)     9847 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/company/
+-rw-r--r--   0 runner    (1001) runner    (1001)      641 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/company/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/inference/
+-rw-r--r--   0 runner    (1001) runner    (1001)      600 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/notification/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1198 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/sandbox/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1460 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/sentinel/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1518 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/sentinel/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.668278 maitai_python-1.0.1b1/maitai_gen/session/
+-rw-r--r--   0 runner    (1001) runner    (1001)      886 2024-05-30 21:32:05.000000 maitai_python-1.0.1b1/maitai_gen/session/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/maitai_python.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1721 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      915 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       70 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       32 2024-05-30 21:32:37.000000 maitai_python-1.0.1b1/maitai_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-30 21:32:37.672278 maitai_python-1.0.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)      764 2024-05-30 21:32:24.000000 maitai_python-1.0.1b1/setup.py
```

### Comparing `maitai_python-1.0.1b0/PKG-INFO` & `maitai_python-1.0.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maitai-python
-Version: 1.0.1b0
+Version: 1.0.1b1
 Summary: MaiTai SDK for Python
 Home-page: https://docs.trymaitai.ai
 Author: Maitai
 Author-email: support@trymaitai.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: setuptools
 Requires-Dist: websocket-client
 
 # Quickstart
 
-Full documents can be found at https://docs.trymaitai.ai
+Full docs can be found at https://docs.trymaitai.ai
 
 ## Configure your application in the Maitai portal
 
 From the [Maitai Portal](https://portal.trymaitai.ai/), click the `+ New Application` button to create your first
 application.
 
 Fill out your application details, and note the `Application Reference` - you'll need that later
```

### Comparing `maitai_python-1.0.1b0/README.md` & `maitai_python-1.0.1b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Quickstart
 
-Full documents can be found at https://docs.trymaitai.ai
+Full docs can be found at https://docs.trymaitai.ai
 
 ## Configure your application in the Maitai portal
 
 From the [Maitai Portal](https://portal.trymaitai.ai/), click the `+ New Application` button to create your first
 application.
 
 Fill out your application details, and note the `Application Reference` - you'll need that later
```

### Comparing `maitai_python-1.0.1b0/maitai/_config.py` & `maitai_python-1.0.1b1/maitai/_config.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai/_evaluator.py` & `maitai_python-1.0.1b1/maitai/_evaluator.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai/_inference.py` & `maitai_python-1.0.1b1/maitai/_inference.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai/_maitai_client.py` & `maitai_python-1.0.1b1/maitai/_maitai_client.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai/_openai.py` & `maitai_python-1.0.1b1/maitai/_openai.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai/_types.py` & `maitai_python-1.0.1b1/maitai/_types.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai/_utils.py` & `maitai_python-1.0.1b1/maitai/_utils.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_common/processes/io_thread.py` & `maitai_python-1.0.1b1/maitai_common/processes/io_thread.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_common/processes/websocket_listener_thread.py` & `maitai_python-1.0.1b1/maitai_common/processes/websocket_listener_thread.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/application/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/application/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/chat/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/company/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/company/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/inference/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/notification/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/sandbox/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/sentinel/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/sentinel/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_gen/session/__init__.py` & `maitai_python-1.0.1b1/maitai_gen/session/__init__.py`

 * *Files identical despite different names*

### Comparing `maitai_python-1.0.1b0/maitai_python.egg-info/PKG-INFO` & `maitai_python-1.0.1b1/maitai_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maitai-python
-Version: 1.0.1b0
+Version: 1.0.1b1
 Summary: MaiTai SDK for Python
 Home-page: https://docs.trymaitai.ai
 Author: Maitai
 Author-email: support@trymaitai.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: setuptools
 Requires-Dist: websocket-client
 
 # Quickstart
 
-Full documents can be found at https://docs.trymaitai.ai
+Full docs can be found at https://docs.trymaitai.ai
 
 ## Configure your application in the Maitai portal
 
 From the [Maitai Portal](https://portal.trymaitai.ai/), click the `+ New Application` button to create your first
 application.
 
 Fill out your application details, and note the `Application Reference` - you'll need that later
```

### Comparing `maitai_python-1.0.1b0/maitai_python.egg-info/SOURCES.txt` & `maitai_python-1.0.1b1/maitai_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

