# Comparing `tmp/th2_grpc_lw_data_provider-2.4.0.dev9065606558.tar.gz` & `tmp/th2_grpc_lw_data_provider-2.4.0.dev9065635110.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_lw_data_provider-2.4.0.dev9065606558.tar", last modified: Mon May 13 15:29:04 2024, max compression
+gzip compressed data, was "dist/th2_grpc_lw_data_provider-2.4.0.dev9065635110.tar", last modified: Mon May 13 15:30:44 2024, max compression
```

## Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558.tar` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:29:04.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 15:29:04.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-13 15:27:30.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 15:27:30.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:29:04.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-13 15:27:30.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:29:04.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-13 15:28:41.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/data_provider_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-13 15:27:30.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider.proto
--rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32690 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-13 15:27:30.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-13 15:28:41.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:29:04.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-13 15:29:04.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 15:29:03.000000 th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-13 15:29:15.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-13 15:29:16.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-13 15:29:15.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-13 15:30:22.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/data_provider_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-13 15:29:15.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    12077 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32690 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-13 15:29:15.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-13 15:30:22.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 15:30:44.000000 th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/top_level.txt
```

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/PKG-INFO` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_lw_data_provider
-Version: 2.4.0.dev9065606558
+Version: 2.4.0.dev9065635110
 Summary: th2_grpc_lw_data_provider
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for lw-data-provider (2.3.0)
```

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/setup.py` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/data_provider_service.py` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/data_provider_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider.proto` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider_pb2.py` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/lw_data_provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider.proto` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_pb2.py` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider/queue_data_provider_service.py` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider/queue_data_provider_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/PKG-INFO` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-lw-data-provider
-Version: 2.4.0.dev9065606558
+Version: 2.4.0.dev9065635110
 Summary: th2_grpc_lw_data_provider
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for lw-data-provider (2.3.0)
```

### Comparing `th2_grpc_lw_data_provider-2.4.0.dev9065606558/th2_grpc_lw_data_provider.egg-info/SOURCES.txt` & `th2_grpc_lw_data_provider-2.4.0.dev9065635110/th2_grpc_lw_data_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

