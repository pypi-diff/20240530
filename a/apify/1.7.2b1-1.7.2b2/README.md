# Comparing `tmp/apify-1.7.2b1.tar.gz` & `tmp/apify-1.7.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.7.2b1.tar", last modified: Thu May 23 15:20:14 2024, max compression
+gzip compressed data, was "apify-1.7.2b2.tar", last modified: Thu May 30 08:43:56 2024, max compression
```

## Comparing `apify-1.7.2b1.tar` & `apify-1.7.2b2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.680984 apify-1.7.2b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-23 15:19:39.000000 apify-1.7.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 15:20:14.680984 apify-1.7.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-23 15:19:39.000000 apify-1.7.2b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-23 15:20:12.000000 apify-1.7.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:20:14.680984 apify-1.7.2b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.668983 apify-1.7.2b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.672984 apify-1.7.2b1/src/apify/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.672984 apify-1.7.2b1/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.676983 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    60423 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.676983 apify-1.7.2b1/src/apify/scrapy/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.676983 apify-1.7.2b1/src/apify/scrapy/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/middlewares/apify_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.676983 apify-1.7.2b1/src/apify/scrapy/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/pipelines/actor_dataset_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/scrapy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.676983 apify-1.7.2b1/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 15:19:39.000000 apify-1.7.2b1/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:20:14.676983 apify-1.7.2b1/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-23 15:20:14.000000 apify-1.7.2b1/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-23 15:20:14.000000 apify-1.7.2b1/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:20:14.000000 apify-1.7.2b1/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-23 15:20:14.000000 apify-1.7.2b1/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 15:20:14.000000 apify-1.7.2b1/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.208330 apify-1.7.2b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-05-30 08:43:10.000000 apify-1.7.2b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-30 08:43:56.208330 apify-1.7.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-30 08:43:10.000000 apify-1.7.2b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-30 08:43:54.000000 apify-1.7.2b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:43:56.212330 apify-1.7.2b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.196330 apify-1.7.2b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.200330 apify-1.7.2b2/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.204330 apify-1.7.2b2/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.204330 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60423 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.204330 apify-1.7.2b2/src/apify/scrapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.204330 apify-1.7.2b2/src/apify/scrapy/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/middlewares/apify_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.204330 apify-1.7.2b2/src/apify/scrapy/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/pipelines/actor_dataset_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/scrapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.208330 apify-1.7.2b2/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-30 08:43:10.000000 apify-1.7.2b2/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:43:56.208330 apify-1.7.2b2/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-30 08:43:56.000000 apify-1.7.2b2/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-30 08:43:56.000000 apify-1.7.2b2/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:43:56.000000 apify-1.7.2b2/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-30 08:43:56.000000 apify-1.7.2b2/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 08:43:56.000000 apify-1.7.2b2/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.7.2b1/LICENSE` & `apify-1.7.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/PKG-INFO` & `apify-1.7.2b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.2b1
+Version: 1.7.2b2
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
@@ -20,24 +20,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: apify-client~=1.6.2
-Requires-Dist: apify-shared~=1.1.1
+Requires-Dist: apify-client~=1.6.0
+Requires-Dist: apify-shared~=1.1.0
 Requires-Dist: aiofiles>=22.1.0
 Requires-Dist: aioshutil>=1.0
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: cryptography>=39.0.0
-Requires-Dist: httpx>=0.24.1
-Requires-Dist: psutil>=5.9.5
-Requires-Dist: pyee>=11.0.1
-Requires-Dist: sortedcollections>=2.0.1
+Requires-Dist: httpx>=0.24.0
+Requires-Dist: psutil>=5.9.0
+Requires-Dist: pyee>=11.0.0
+Requires-Dist: sortedcollections>=2.0.0
 Requires-Dist: typing-extensions>=4.1.0
 Requires-Dist: websockets>=10.1
 Provides-Extra: dev
 Requires-Dist: build~=1.2.0; extra == "dev"
 Requires-Dist: filelock~=3.14.0; extra == "dev"
 Requires-Dist: mypy~=1.10.0; extra == "dev"
 Requires-Dist: pre-commit~=3.5.0; extra == "dev"
@@ -46,14 +46,15 @@
 Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
 Requires-Dist: pytest-only~=2.1.0; extra == "dev"
 Requires-Dist: pytest-timeout~=2.3.0; extra == "dev"
 Requires-Dist: pytest-xdist~=3.6.0; extra == "dev"
 Requires-Dist: respx~=0.21.0; extra == "dev"
 Requires-Dist: ruff~=0.4.0; extra == "dev"
+Requires-Dist: setuptools~=70.0.0; extra == "dev"
 Requires-Dist: twine~=5.1.0; extra == "dev"
 Requires-Dist: types-aiofiles~=23.2.0.20240403; extra == "dev"
 Requires-Dist: types-colorama~=0.4.15.20240311; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5.20240516; extra == "dev"
 Provides-Extra: scrapy
 Requires-Dist: scrapy>=2.11.0; extra == "scrapy"
```

### Comparing `apify-1.7.2b1/README.md` & `apify-1.7.2b2/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/pyproject.toml` & `apify-1.7.2b2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apify"
-version = "1.7.2b1"
+version = "1.7.2b2"
 description = "Apify SDK for Python"
 readme = "README.md"
 license = { text = "Apache Software License" }
 authors = [{ name = "Apify Technologies s.r.o.", email = "support@apify.com" }]
 keywords = ["apify", "sdk", "actor", "scraping", "automation"]
 
 classifiers = [
@@ -22,24 +22,24 @@
 
 requires-python = ">=3.8"
 
 # We use inclusive ordered comparison clause for non-Apify packages intentionally in order to enhance the Apify SDK's
 # compatibility with a wide range of external packages. This decision was discussed in detail in the following PR:
 # https://github.com/apify/apify-sdk-python/pull/154
 dependencies = [
-    "apify-client ~= 1.6.2",
-    "apify-shared ~= 1.1.1",
+    "apify-client ~= 1.6.0",
+    "apify-shared ~= 1.1.0",
     "aiofiles >= 22.1.0",
     "aioshutil >= 1.0",
     "colorama >= 0.4.6",
     "cryptography >= 39.0.0",
-    "httpx >= 0.24.1",
-    "psutil >= 5.9.5",
-    "pyee >= 11.0.1",
-    "sortedcollections >= 2.0.1",
+    "httpx >= 0.24.0",
+    "psutil >= 5.9.0",
+    "pyee >= 11.0.0",
+    "sortedcollections >= 2.0.0",
     "typing-extensions >= 4.1.0",
     "websockets >= 10.1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "build ~= 1.2.0",
@@ -51,14 +51,15 @@
     "pytest-asyncio ~= 0.23.0",
     "pytest-cov ~= 5.0.0",
     "pytest-only ~= 2.1.0",
     "pytest-timeout ~= 2.3.0",
     "pytest-xdist ~= 3.6.0",
     "respx ~= 0.21.0",
     "ruff ~= 0.4.0",
+    "setuptools ~= 70.0.0",  # setuptools are used by pytest, but not explicitly required
     "twine ~= 5.1.0",
     "types-aiofiles ~= 23.2.0.20240403",
     "types-colorama ~= 0.4.15.20240311",
     "types-psutil ~= 5.9.5.20240516",
 ]
 scrapy = [
     "scrapy >= 2.11.0",
@@ -69,15 +70,15 @@
 "Documentation" = "https://docs.apify.com/sdk/python/"
 "Source" = "https://github.com/apify/apify-sdk-python"
 "Issue tracker" = "https://github.com/apify/apify-sdk-python/issues"
 "Changelog" = "https://github.com/apify/apify-sdk-python/blob/master/CHANGELOG.md"
 "Apify Homepage" = "https://apify.com"
 
 [build-system]
-requires = ["setuptools>=64.0.0", "wheel"]
+requires = ["setuptools ~= 70.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["apify*"]
 
 [tool.setuptools.package-data]
```

### Comparing `apify-1.7.2b1/src/apify/_crypto.py` & `apify-1.7.2b2/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.7.2b2/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.7.2b2/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.7.2b2/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/_utils.py` & `apify-1.7.2b2/src/apify/_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/actor.py` & `apify-1.7.2b2/src/apify/actor.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/config.py` & `apify-1.7.2b2/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/consts.py` & `apify-1.7.2b2/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/event_manager.py` & `apify-1.7.2b2/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/log.py` & `apify-1.7.2b2/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/proxy_configuration.py` & `apify-1.7.2b2/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/scrapy/middlewares/apify_proxy.py` & `apify-1.7.2b2/src/apify/scrapy/middlewares/apify_proxy.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/scrapy/pipelines/actor_dataset_push.py` & `apify-1.7.2b2/src/apify/scrapy/pipelines/actor_dataset_push.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/scrapy/requests.py` & `apify-1.7.2b2/src/apify/scrapy/requests.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/scrapy/scheduler.py` & `apify-1.7.2b2/src/apify/scrapy/scheduler.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/scrapy/utils.py` & `apify-1.7.2b2/src/apify/scrapy/utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/storages/base_storage.py` & `apify-1.7.2b2/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/storages/dataset.py` & `apify-1.7.2b2/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/storages/key_value_store.py` & `apify-1.7.2b2/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/storages/request_queue.py` & `apify-1.7.2b2/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify/storages/storage_client_manager.py` & `apify-1.7.2b2/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify.egg-info/PKG-INFO` & `apify-1.7.2b2/src/apify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.2b1
+Version: 1.7.2b2
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
@@ -20,24 +20,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: apify-client~=1.6.2
-Requires-Dist: apify-shared~=1.1.1
+Requires-Dist: apify-client~=1.6.0
+Requires-Dist: apify-shared~=1.1.0
 Requires-Dist: aiofiles>=22.1.0
 Requires-Dist: aioshutil>=1.0
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: cryptography>=39.0.0
-Requires-Dist: httpx>=0.24.1
-Requires-Dist: psutil>=5.9.5
-Requires-Dist: pyee>=11.0.1
-Requires-Dist: sortedcollections>=2.0.1
+Requires-Dist: httpx>=0.24.0
+Requires-Dist: psutil>=5.9.0
+Requires-Dist: pyee>=11.0.0
+Requires-Dist: sortedcollections>=2.0.0
 Requires-Dist: typing-extensions>=4.1.0
 Requires-Dist: websockets>=10.1
 Provides-Extra: dev
 Requires-Dist: build~=1.2.0; extra == "dev"
 Requires-Dist: filelock~=3.14.0; extra == "dev"
 Requires-Dist: mypy~=1.10.0; extra == "dev"
 Requires-Dist: pre-commit~=3.5.0; extra == "dev"
@@ -46,14 +46,15 @@
 Requires-Dist: pytest-asyncio~=0.23.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
 Requires-Dist: pytest-only~=2.1.0; extra == "dev"
 Requires-Dist: pytest-timeout~=2.3.0; extra == "dev"
 Requires-Dist: pytest-xdist~=3.6.0; extra == "dev"
 Requires-Dist: respx~=0.21.0; extra == "dev"
 Requires-Dist: ruff~=0.4.0; extra == "dev"
+Requires-Dist: setuptools~=70.0.0; extra == "dev"
 Requires-Dist: twine~=5.1.0; extra == "dev"
 Requires-Dist: types-aiofiles~=23.2.0.20240403; extra == "dev"
 Requires-Dist: types-colorama~=0.4.15.20240311; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5.20240516; extra == "dev"
 Provides-Extra: scrapy
 Requires-Dist: scrapy>=2.11.0; extra == "scrapy"
```

### Comparing `apify-1.7.2b1/src/apify.egg-info/SOURCES.txt` & `apify-1.7.2b2/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.7.2b1/src/apify.egg-info/requires.txt` & `apify-1.7.2b2/src/apify.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-apify-client~=1.6.2
-apify-shared~=1.1.1
+apify-client~=1.6.0
+apify-shared~=1.1.0
 aiofiles>=22.1.0
 aioshutil>=1.0
 colorama>=0.4.6
 cryptography>=39.0.0
-httpx>=0.24.1
-psutil>=5.9.5
-pyee>=11.0.1
-sortedcollections>=2.0.1
+httpx>=0.24.0
+psutil>=5.9.0
+pyee>=11.0.0
+sortedcollections>=2.0.0
 typing-extensions>=4.1.0
 websockets>=10.1
 
 [dev]
 build~=1.2.0
 filelock~=3.14.0
 mypy~=1.10.0
@@ -21,14 +21,15 @@
 pytest-asyncio~=0.23.0
 pytest-cov~=5.0.0
 pytest-only~=2.1.0
 pytest-timeout~=2.3.0
 pytest-xdist~=3.6.0
 respx~=0.21.0
 ruff~=0.4.0
+setuptools~=70.0.0
 twine~=5.1.0
 types-aiofiles~=23.2.0.20240403
 types-colorama~=0.4.15.20240311
 types-psutil~=5.9.5.20240516
 
 [scrapy]
 scrapy>=2.11.0
```

