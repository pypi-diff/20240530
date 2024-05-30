# Comparing `tmp/crawlee-0.0.4b2.tar.gz` & `tmp/crawlee-0.0.4b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.4b2.tar", max compression
+gzip compressed data, was "crawlee-0.0.4b3.tar", max compression
```

## Comparing `crawlee-0.0.4b2.tar` & `crawlee-0.0.4b3.tar`

### file list

```diff
@@ -1,94 +1,103 @@
--rw-r--r--   0        0        0    11355 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/LICENSE
--rw-r--r--   0        0        0    16623 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/README.md
--rw-r--r--   0        0        0     6623 2024-05-24 18:44:17.299330 crawlee-0.0.4b2/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0      774 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/blocked.py
--rw-r--r--   0        0        0     3341 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1683 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     3503 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     5262 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/globs.py
--rw-r--r--   0        0        0     2056 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0      790 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/models.py
--rw-r--r--   0        0        0     1585 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      470 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/__init__.py
--rw-r--r--   0        0        0     9143 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_client.py
--rw-r--r--   0        0        0     1883 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_collection_client.py
--rw-r--r--   0        0        0     3486 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_client.py
--rw-r--r--   0        0        0     2025 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
--rw-r--r--   0        0        0     5622 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_client.py
--rw-r--r--   0        0        0     1992 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_collection_client.py
--rw-r--r--   0        0        0     2229 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/base_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/py.typed
--rw-r--r--   0        0        0      735 2024-05-24 18:43:54.503190 crawlee-0.0.4b2/src/crawlee/base_storage_client/types.py
--rw-r--r--   0        0        0      186 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    28317 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     4696 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2145 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/errors.py
--rw-r--r--   0        0        0     2279 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0     2820 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0       86 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     5574 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      524 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0     1310 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/configuration.py
--rw-r--r--   0        0        0      146 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/consts.py
--rw-r--r--   0        0        0      272 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/enqueue_strategy.py
--rw-r--r--   0        0        0       91 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2682 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1303 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     2140 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     5085 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       59 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     2992 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/log_config.py
--rw-r--r--   0        0        0       55 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/__init__.py
--rw-r--r--   0        0        0    15666 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/_creation_management.py
--rw-r--r--   0        0        0    15684 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_client.py
--rw-r--r--   0        0        0     2243 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_collection_client.py
--rw-r--r--   0        0        0    15914 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_client.py
--rw-r--r--   0        0        0     2333 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_collection_client.py
--rw-r--r--   0        0        0    11113 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/py.typed
--rw-r--r--   0        0        0    20944 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_client.py
--rw-r--r--   0        0        0     2316 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_collection_client.py
--rw-r--r--   0        0        0    13847 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/models.py
--rw-r--r--   0        0        0     7393 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/proxy_configuration.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/py.typed
--rw-r--r--   0        0        0       67 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8084 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/__init__.py
--rw-r--r--   0        0        0      980 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/error_tracker.py
--rw-r--r--   0        0        0     3646 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/models.py
--rw-r--r--   0        0        0    10880 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/statistics/statistics.py
--rw-r--r--   0        0        0     1520 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      150 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     8804 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/_creation_management.py
--rw-r--r--   0        0        0     1090 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15956 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     4994 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0        0 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2841 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2755 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25708 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-05-24 18:43:54.507190 crawlee-0.0.4b2/src/crawlee/types.py
--rw-r--r--   0        0        0    18689 1970-01-01 00:00:00.000000 crawlee-0.0.4b2/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-29 14:04:44.638610 crawlee-0.0.4b3/LICENSE
+-rw-r--r--   0        0        0    20323 2024-05-29 14:04:44.638610 crawlee-0.0.4b3/README.md
+-rw-r--r--   0        0        0     6790 2024-05-29 14:05:19.402664 crawlee-0.0.4b3/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/blocked.py
+-rw-r--r--   0        0        0     3341 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1683 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     3503 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     5262 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/globs.py
+-rw-r--r--   0        0        0     2056 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0      790 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/models.py
+-rw-r--r--   0        0        0     1585 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      470 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/__init__.py
+-rw-r--r--   0        0        0     9143 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_client.py
+-rw-r--r--   0        0        0     1883 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_collection_client.py
+-rw-r--r--   0        0        0     3486 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_client.py
+-rw-r--r--   0        0        0     2025 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
+-rw-r--r--   0        0        0     5622 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_client.py
+-rw-r--r--   0        0        0     1992 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_collection_client.py
+-rw-r--r--   0        0        0     2229 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/py.typed
+-rw-r--r--   0        0        0      735 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/types.py
+-rw-r--r--   0        0        0      244 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    28954 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     4696 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2181 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/errors.py
+-rw-r--r--   0        0        0     2279 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0     2820 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0      104 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     5574 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      524 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0      101 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/__init__.py
+-rw-r--r--   0        0        0     1383 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/base_browser_plugin.py
+-rw-r--r--   0        0        0     6184 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/browser_pool.py
+-rw-r--r--   0        0        0     3104 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/playwright_browser_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/py.typed
+-rw-r--r--   0        0        0      399 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/types.py
+-rw-r--r--   0        0        0     1310 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/configuration.py
+-rw-r--r--   0        0        0      182 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/consts.py
+-rw-r--r--   0        0        0      308 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/enqueue_strategy.py
+-rw-r--r--   0        0        0       91 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2682 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1556 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     2140 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     5085 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       77 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     2992 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/log_config.py
+-rw-r--r--   0        0        0       55 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/__init__.py
+-rw-r--r--   0        0        0    15666 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/_creation_management.py
+-rw-r--r--   0        0        0    15684 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_client.py
+-rw-r--r--   0        0        0     2243 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_collection_client.py
+-rw-r--r--   0        0        0    15914 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_client.py
+-rw-r--r--   0        0        0     2333 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_collection_client.py
+-rw-r--r--   0        0        0    11113 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/py.typed
+-rw-r--r--   0        0        0    20944 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_client.py
+-rw-r--r--   0        0        0     2316 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_collection_client.py
+-rw-r--r--   0        0        0    13847 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/models.py
+-rw-r--r--   0        0        0       95 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/playwright_crawler/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/playwright_crawler/playwright_crawler.py
+-rw-r--r--   0        0        0      381 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/playwright_crawler/types.py
+-rw-r--r--   0        0        0     7393 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/proxy_configuration.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/py.typed
+-rw-r--r--   0        0        0       67 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8084 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/__init__.py
+-rw-r--r--   0        0        0      980 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/error_tracker.py
+-rw-r--r--   0        0        0     3646 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/models.py
+-rw-r--r--   0        0        0    10880 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/statistics.py
+-rw-r--r--   0        0        0     1520 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      150 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     8804 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/_creation_management.py
+-rw-r--r--   0        0        0     1090 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15956 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4994 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2841 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2755 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25708 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/types.py
+-rw-r--r--   0        0        0    22484 1970-01-01 00:00:00.000000 crawlee-0.0.4b3/PKG-INFO
```

### Comparing `crawlee-0.0.4b2/LICENSE` & `crawlee-0.0.4b3/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/README.md` & `crawlee-0.0.4b3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -202,15 +202,116 @@
         }
 
         await dataset.push_data(record)
 ```
 
 #### PlaywrightCrawler
 
-- TODO
+[`PlaywrightCrawler`](https://github.com/apify/crawlee-py/tree/master/src/crawlee/playwright_crawler) extends
+the `BasicCrawler`. It provides the same features and on top of that, it uses
+[Playwright](https://playwright.dev/python) browser automation tool.
+
+This crawler provides a straightforward framework for parallel web page crawling using headless versions of Chromium,
+Firefox, and Webkit browsers through Playwright. URLs to be crawled are supplied by a request provider, which can be
+either a `RequestList` containing a static list of URLs or a dynamic `RequestQueue`.
+
+Using a headless browser to download web pages and extract data, `PlaywrightCrawler` is ideal for crawling
+websites that require JavaScript execution. For websites that do not require JavaScript, consider using
+the `BeautifulSoupCrawler`, which utilizes raw HTTP requests and will be much faster.
+
+Example usage:
+
+```python
+import asyncio
+
+from crawlee.playwright_crawler import PlaywrightCrawler, PlaywrightCrawlingContext
+from crawlee.storages import Dataset, RequestQueue
+
+
+async def main() -> None:
+    # Open a default request queue and add requests to it
+    rq = await RequestQueue.open()
+    await rq.add_request('https://crawlee.dev')
+
+    # Open a default dataset for storing results
+    dataset = await Dataset.open()
+
+    # Create a crawler instance and provide a request provider (and other optional arguments)
+    crawler = PlaywrightCrawler(
+        request_provider=rq,
+        # headless=False,
+        # browser_type='firefox',
+    )
+
+    @crawler.router.default_handler
+    async def request_handler(context: PlaywrightCrawlingContext) -> None:
+        record = {
+            'request_url': context.request.url,
+            'page_url': context.page.url,
+            'page_title': await context.page.title(),
+            'page_content': (await context.page.content())[:10000],
+        }
+        await dataset.push_data(record)
+
+    await crawler.run()
+
+
+if __name__ == '__main__':
+    asyncio.run(main())
+```
+
+Example usage with custom browser pool:
+
+```python
+import asyncio
+
+from crawlee.browsers import BrowserPool, PlaywrightBrowserPlugin
+from crawlee.playwright_crawler import PlaywrightCrawler, PlaywrightCrawlingContext
+from crawlee.storages import Dataset, RequestQueue
+
+
+async def main() -> None:
+    # Open a default request queue and add requests to it
+    rq = await RequestQueue.open()
+    await rq.add_request('https://crawlee.dev')
+    await rq.add_request('https://apify.com')
+
+    # Open a default dataset for storing results
+    dataset = await Dataset.open()
+
+    # Create a browser pool with a Playwright browser plugin
+    browser_pool = BrowserPool(
+        plugins=[
+            PlaywrightBrowserPlugin(
+                browser_type='firefox',
+                browser_options={'headless': False},
+                page_options={'viewport': {'width': 1920, 'height': 1080}},
+            )
+        ]
+    )
+
+    # Create a crawler instance and provide a browser pool and request provider
+    crawler = PlaywrightCrawler(request_provider=rq, browser_pool=browser_pool)
+
+    @crawler.router.default_handler
+    async def request_handler(context: PlaywrightCrawlingContext) -> None:
+        record = {
+            'request_url': context.request.url,
+            'page_url': context.page.url,
+            'page_title': await context.page.title(),
+            'page_content': (await context.page.content())[:10000],
+        }
+        await dataset.push_data(record)
+
+    await crawler.run()
+
+
+if __name__ == '__main__':
+    asyncio.run(main())
+```
 
 ### Storages
 
 Crawlee introduces several result storage types that are useful for specific tasks. The storing of underlying data
 is realized by the storage client. Currently, only a memory storage client is implemented. Using this, the data
 are stored either in the memory or persisted on the disk.
 
@@ -412,14 +513,22 @@
     crawler = HttpCrawler(session_pool=session_pool_v1, use_session_pool=True)
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
+<!--
+### Browser Management
+
+- TODO
+- Write once browser rotation and/or other features are ready
+- Update PlaywrightCrawler according to this
+-->
+
 ## Running on the Apify platform
 
 Crawlee is open-source and runs anywhere, but since it's developed by [Apify](https://apify.com), it's easy to set up on the Apify platform and run in the cloud. Visit the [Apify SDK website](https://sdk.apify.com) to learn more about deploying Crawlee to the Apify platform.
 
 ## Support
 
 If you find any bug or issue with Crawlee, please [submit an issue on GitHub](https://github.com/apify/crawlee-py/issues). For questions, you can ask on [Stack Overflow](https://stackoverflow.com/questions/tagged/apify), in GitHub Discussions or you can join our [Discord server](https://discord.com/invite/jyEM2PRvMU).
```

#### html2text {}

```diff
@@ -94,30 +94,73 @@
 example with the updated request handler: ```python from
 crawlee.enqueue_strategy import EnqueueStrategy # ...
 @crawler.router.default_handler async def request_handler(context:
 BeautifulSoupCrawlingContext) -> None: # Use enqueue links helper to enqueue
 all links from the page with the same domain await context.enqueue_links
 (strategy=EnqueueStrategy.SAME_DOMAIN) record = { 'title':
 context.soup.title.text, 'url': context.request.url, } await dataset.push_data
-(record) ``` #### PlaywrightCrawler - TODO ### Storages Crawlee introduces
-several result storage types that are useful for specific tasks. The storing of
-underlying data is realized by the storage client. Currently, only a memory
-storage client is implemented. Using this, the data are stored either in the
-memory or persisted on the disk. By default, the data are stored in the
-directory specified by the `CRAWLEE_STORAGE_DIR` environment variable. With
-default `.storage/`. #### Dataset A [`Dataset`](https://github.com/apify/
-crawlee-py/blob/master/src/crawlee/storages/dataset.py) is a type of storage
-mainly suitable for storing tabular data. Datasets are used to store structured
-data where each object stored has the same attributes, such as online store
-products or real estate offers. The dataset can be imagined as a table, where
-each object is a row and its attributes are columns. The dataset is an append-
-only storage - we can only add new records to it, but we cannot modify or
-remove existing records. Each Crawlee project run is associated with a default
-dataset. Typically, it is used to store crawling results specific to the
-crawler run. Its usage is optional. The data are persisted as follows: ```
+(record) ``` #### PlaywrightCrawler [`PlaywrightCrawler`](https://github.com/
+apify/crawlee-py/tree/master/src/crawlee/playwright_crawler) extends the
+`BasicCrawler`. It provides the same features and on top of that, it uses
+[Playwright](https://playwright.dev/python) browser automation tool. This
+crawler provides a straightforward framework for parallel web page crawling
+using headless versions of Chromium, Firefox, and Webkit browsers through
+Playwright. URLs to be crawled are supplied by a request provider, which can be
+either a `RequestList` containing a static list of URLs or a dynamic
+`RequestQueue`. Using a headless browser to download web pages and extract
+data, `PlaywrightCrawler` is ideal for crawling websites that require
+JavaScript execution. For websites that do not require JavaScript, consider
+using the `BeautifulSoupCrawler`, which utilizes raw HTTP requests and will be
+much faster. Example usage: ```python import asyncio from
+crawlee.playwright_crawler import PlaywrightCrawler, PlaywrightCrawlingContext
+from crawlee.storages import Dataset, RequestQueue async def main() -> None: #
+Open a default request queue and add requests to it rq = await
+RequestQueue.open() await rq.add_request('https://crawlee.dev') # Open a
+default dataset for storing results dataset = await Dataset.open() # Create a
+crawler instance and provide a request provider (and other optional arguments)
+crawler = PlaywrightCrawler( request_provider=rq, # headless=False, #
+browser_type='firefox', ) @crawler.router.default_handler async def
+request_handler(context: PlaywrightCrawlingContext) -> None: record =
+{ 'request_url': context.request.url, 'page_url': context.page.url,
+'page_title': await context.page.title(), 'page_content': (await
+context.page.content())[:10000], } await dataset.push_data(record) await
+crawler.run() if __name__ == '__main__': asyncio.run(main()) ``` Example usage
+with custom browser pool: ```python import asyncio from crawlee.browsers import
+BrowserPool, PlaywrightBrowserPlugin from crawlee.playwright_crawler import
+PlaywrightCrawler, PlaywrightCrawlingContext from crawlee.storages import
+Dataset, RequestQueue async def main() -> None: # Open a default request queue
+and add requests to it rq = await RequestQueue.open() await rq.add_request
+('https://crawlee.dev') await rq.add_request('https://apify.com') # Open a
+default dataset for storing results dataset = await Dataset.open() # Create a
+browser pool with a Playwright browser plugin browser_pool = BrowserPool
+( plugins=[ PlaywrightBrowserPlugin( browser_type='firefox', browser_options=
+{'headless': False}, page_options={'viewport': {'width': 1920, 'height':
+1080}}, ) ] ) # Create a crawler instance and provide a browser pool and
+request provider crawler = PlaywrightCrawler(request_provider=rq,
+browser_pool=browser_pool) @crawler.router.default_handler async def
+request_handler(context: PlaywrightCrawlingContext) -> None: record =
+{ 'request_url': context.request.url, 'page_url': context.page.url,
+'page_title': await context.page.title(), 'page_content': (await
+context.page.content())[:10000], } await dataset.push_data(record) await
+crawler.run() if __name__ == '__main__': asyncio.run(main()) ``` ### Storages
+Crawlee introduces several result storage types that are useful for specific
+tasks. The storing of underlying data is realized by the storage client.
+Currently, only a memory storage client is implemented. Using this, the data
+are stored either in the memory or persisted on the disk. By default, the data
+are stored in the directory specified by the `CRAWLEE_STORAGE_DIR` environment
+variable. With default `.storage/`. #### Dataset A [`Dataset`](https://
+github.com/apify/crawlee-py/blob/master/src/crawlee/storages/dataset.py) is a
+type of storage mainly suitable for storing tabular data. Datasets are used to
+store structured data where each object stored has the same attributes, such as
+online store products or real estate offers. The dataset can be imagined as a
+table, where each object is a row and its attributes are columns. The dataset
+is an append-only storage - we can only add new records to it, but we cannot
+modify or remove existing records. Each Crawlee project run is associated with
+a default dataset. Typically, it is used to store crawling results specific to
+the crawler run. Its usage is optional. The data are persisted as follows: ```
 {CRAWLEE_STORAGE_DIR}/datasets/{DATASET_ID}/{INDEX}.json ``` The following code
 demonstrates the basic operations of the dataset: ```python import asyncio from
 crawlee.storages import Dataset async def main() -> None: # Open a default
 dataset dataset = await Dataset.open() # Push a single record await
 dataset.push_data({'key1': 'value1'}) # Get records from the dataset data =
 await dataset.get_data() print(f'Dataset data: {data.items}') # Dataset data: [
 {'key1': 'value1'}] # Open a named dataset dataset_named = await Dataset.open
```

### Comparing `crawlee-0.0.4b2/pyproject.toml` & `crawlee-0.0.4b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.4b2"
+version = "0.0.4b3"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -51,14 +51,15 @@
 colorama = "^0.4.6"
 docutils = "^0.21.0"
 eval-type-backport = "^0.2.0"
 html5lib = { version = "^1.1", optional = true }
 httpx = "^0.27.0"
 lxml = { version = "^5.2.1", optional = true }
 more_itertools = "^10.2.0"
+playwright = { version = "^1.43.0", optional = true }
 psutil = "^5.9.8"
 pydantic = "^2.6.3"
 pydantic-settings = "^2.2.1"
 pyee = "^11.1.0"
 python-dateutil = "^2.9.0"
 sortedcollections = "^2.1.0"
 typing-extensions = "^4.1.0"
@@ -74,23 +75,25 @@
 pytest-asyncio = "~0.23.5"
 pytest-cov = "~5.0.0"
 pytest-only = "~2.1.0"
 pytest-timeout = "~2.3.0"
 pytest-xdist = "~3.6.0"
 respx = "~0.21.0"
 ruff = "~0.4.0"
+setuptools = "^70.0.0"  # setuptools are used by pytest, but not explicitly required
 types-aiofiles = "^23.2.0.20240106"
 types-beautifulsoup4 = "^4.12.0.20240229"
 types-colorama = "~0.4.15.20240106"
 types-psutil = "~5.9.5.20240205"
 types-python-dateutil = "^2.9.0.20240316"
 proxy-py = "^2.4.4"
 
 [tool.poetry.extras]
 beautifulsoup = ["beautifulsoup4", "lxml", "html5lib"]
+playwright = ["playwright"]
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
```

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/blocked.py` & `crawlee-0.0.4b3/src/crawlee/_utils/blocked.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 # Inspiration: https://github.com/apify/crawlee/blob/v3.9.2/packages/utils/src/internals/blocked.ts
 
 CLOUDFLARE_RETRY_CSS_SELECTORS = [
     '#turnstile-wrapper iframe[src^="https://challenges.cloudflare.com"]',
 ]
 
 RETRY_CSS_SELECTORS = [
```

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.4b3/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/crypto.py` & `crawlee-0.0.4b3/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.4b3/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.4b3/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/file.py` & `crawlee-0.0.4b3/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/globs.py` & `crawlee-0.0.4b3/src/crawlee/_utils/globs.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.4b3/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/math.py` & `crawlee-0.0.4b3/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.4b3/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/models.py` & `crawlee-0.0.4b3/src/crawlee/_utils/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.4b3/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/requests.py` & `crawlee-0.0.4b3/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/system.py` & `crawlee-0.0.4b3/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/_utils/wait.py` & `crawlee-0.0.4b3/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.4b3/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.4b3/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.4b3/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/autoscaling/types.py` & `crawlee-0.0.4b3/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_client.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_dataset_collection_client.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_client.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_key_value_store_collection_client.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_client.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_request_queue_collection_client.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/base_storage_client.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/base_storage_client/types.py` & `crawlee-0.0.4b3/src/crawlee/base_storage_client/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.4b3/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 )
 from crawlee.basic_crawler.router import Router
 from crawlee.basic_crawler.types import (
     BasicCrawlingContext,
     RequestHandlerRunResult,
     SendRequestFunction,
 )
+from crawlee.browsers import BrowserPool
 from crawlee.configuration import Configuration
 from crawlee.enqueue_strategy import EnqueueStrategy
 from crawlee.events.local_event_manager import LocalEventManager
 from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.models import BaseRequestData, Request, RequestState
 from crawlee.sessions import SessionPool
 from crawlee.statistics.statistics import Statistics
@@ -71,14 +72,16 @@
     configuration: NotRequired[Configuration]
     request_handler_timeout: NotRequired[timedelta]
     session_pool: NotRequired[SessionPool]
     use_session_pool: NotRequired[bool]
     retry_on_blocked: NotRequired[bool]
     proxy_configuration: NotRequired[ProxyConfiguration]
     statistics: NotRequired[Statistics[StatisticsState]]
+    browser_pool: NotRequired[BrowserPool]
+    use_browser_pool: NotRequired[bool]
     _context_pipeline: NotRequired[ContextPipeline[TCrawlingContext]]
 
 
 class BasicCrawler(Generic[TCrawlingContext]):
     """Provides a simple framework for parallel crawling of web pages.
 
     The URLs to crawl are fed either from a static list of URLs or from a dynamic queue of URLs enabling recursive
@@ -101,14 +104,16 @@
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta = timedelta(minutes=1),
         session_pool: SessionPool | None = None,
         use_session_pool: bool = True,
         retry_on_blocked: bool = True,
         proxy_configuration: ProxyConfiguration | None = None,
         statistics: Statistics | None = None,
+        browser_pool: BrowserPool | None = None,
+        use_browser_pool: bool = False,
         _context_pipeline: ContextPipeline[TCrawlingContext] | None = None,
     ) -> None:
         """Initialize the BasicCrawler.
 
         Args:
             request_provider: Provides requests to be processed
             request_handler: A callable to which request handling is delegated
@@ -121,14 +126,16 @@
             configuration: Crawler configuration
             request_handler_timeout: How long is a single request handler allowed to run
             use_session_pool: Enables using the session pool for crawling
             session_pool: A preconfigured `SessionPool` instance if you wish to use non-default configuration
             retry_on_blocked: If set to True, the crawler will try to automatically bypass any detected bot protection
             proxy_configuration: A HTTP proxy configuration to be used for making requests
             statistics: A preconfigured `Statistics` instance if you wish to use non-default configuration
+            browser_pool: A preconfigured `BrowserPool` instance for browser crawling.
+            use_browser_pool: Enables using the browser pool for crawling.
             _context_pipeline: Allows extending the request lifecycle and modifying the crawling context.
                 This parameter is meant to be used by child classes, not when BasicCrawler is instantiated directly.
         """
         self._router: Router[TCrawlingContext] | None = None
 
         if isinstance(cast(Router, request_handler), Router):
             self._router = cast(Router[TCrawlingContext], request_handler)
@@ -176,14 +183,18 @@
 
         self._proxy_configuration = proxy_configuration
         self._statistics = statistics or Statistics(
             event_manager=self._event_manager,
             log_message=f'{logger.name} request statistics',
         )
 
+        self._use_browser_pool = use_browser_pool
+        if self._use_browser_pool:
+            self._browser_pool = browser_pool or BrowserPool()
+
         self._running = False
         self._has_finished_before = False
 
     @property
     def router(self) -> Router[TCrawlingContext]:
         """The router used to handle each individual crawling request."""
         if self._router is None:
@@ -289,14 +300,17 @@
             await exit_stack.enter_async_context(self._event_manager)
             await exit_stack.enter_async_context(self._snapshotter)
             await exit_stack.enter_async_context(self._statistics)
 
             if self._use_session_pool:
                 await exit_stack.enter_async_context(self._session_pool)
 
+            if self._use_browser_pool:
+                await exit_stack.enter_async_context(self._browser_pool)
+
             await self._pool.run()
 
         if self._statistics.error_tracker.total > 0:
             logger.info(
                 'Error analysis:'
                 f' total_errors={self._statistics.error_tracker.total}'
                 f' unique_errors={self._statistics.error_tracker.unique_error_count}'
```

### Comparing `crawlee-0.0.4b2/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.4b3/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/basic_crawler/errors.py` & `crawlee-0.0.4b3/src/crawlee/basic_crawler/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Generic
 
 from typing_extensions import TypeVar
 
 from crawlee.basic_crawler.types import BasicCrawlingContext
```

### Comparing `crawlee-0.0.4b2/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.4b3/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/basic_crawler/types.py` & `crawlee-0.0.4b3/src/crawlee/basic_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/beautifulsoup_crawler/types.py` & `crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/configuration.py` & `crawlee-0.0.4b3/src/crawlee/configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/events/event_manager.py` & `crawlee-0.0.4b3/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.4b3/src/crawlee/events/local_event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.4b3/src/crawlee/http_clients/base_http_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/http_clients/httpx_client.py` & `crawlee-0.0.4b3/src/crawlee/http_clients/httpx_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.4b3/src/crawlee/http_crawler/http_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/log_config.py` & `crawlee-0.0.4b3/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/_creation_management.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/_creation_management.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_client.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/dataset_collection_client.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_client.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/key_value_store_collection_client.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/memory_storage_client.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_client.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/memory_storage_client/request_queue_collection_client.py` & `crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/models.py` & `crawlee-0.0.4b3/src/crawlee/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/proxy_configuration.py` & `crawlee-0.0.4b3/src/crawlee/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/sessions/models.py` & `crawlee-0.0.4b3/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/sessions/session.py` & `crawlee-0.0.4b3/src/crawlee/sessions/session.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.4b3/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/statistics/error_tracker.py` & `crawlee-0.0.4b3/src/crawlee/statistics/error_tracker.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/statistics/models.py` & `crawlee-0.0.4b3/src/crawlee/statistics/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/statistics/statistics.py` & `crawlee-0.0.4b3/src/crawlee/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storage_client_manager.py` & `crawlee-0.0.4b3/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storages/_creation_management.py` & `crawlee-0.0.4b3/src/crawlee/storages/_creation_management.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storages/base_storage.py` & `crawlee-0.0.4b3/src/crawlee/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storages/dataset.py` & `crawlee-0.0.4b3/src/crawlee/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.4b3/src/crawlee/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storages/request_list.py` & `crawlee-0.0.4b3/src/crawlee/storages/request_list.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storages/request_provider.py` & `crawlee-0.0.4b3/src/crawlee/storages/request_provider.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/storages/request_queue.py` & `crawlee-0.0.4b3/src/crawlee/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/src/crawlee/types.py` & `crawlee-0.0.4b3/src/crawlee/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b2/PKG-INFO` & `crawlee-0.0.4b3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.4b2
+Version: 0.0.4b3
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,24 +14,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: beautifulsoup
+Provides-Extra: playwright
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aioshutil (>=1.3,<2.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) ; extra == "beautifulsoup"
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: docutils (>=0.21.0,<0.22.0)
 Requires-Dist: eval-type-backport (>=0.2.0,<0.3.0)
 Requires-Dist: html5lib (>=1.1,<2.0) ; extra == "beautifulsoup"
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0) ; extra == "beautifulsoup"
 Requires-Dist: more_itertools (>=10.2.0,<11.0.0)
+Requires-Dist: playwright (>=1.43.0,<2.0.0) ; extra == "playwright"
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: sortedcollections (>=2.1.0,<3.0.0)
 Requires-Dist: tldextract (>=5.1.2,<6.0.0)
@@ -248,15 +250,116 @@
         }
 
         await dataset.push_data(record)
 ```
 
 #### PlaywrightCrawler
 
-- TODO
+[`PlaywrightCrawler`](https://github.com/apify/crawlee-py/tree/master/src/crawlee/playwright_crawler) extends
+the `BasicCrawler`. It provides the same features and on top of that, it uses
+[Playwright](https://playwright.dev/python) browser automation tool.
+
+This crawler provides a straightforward framework for parallel web page crawling using headless versions of Chromium,
+Firefox, and Webkit browsers through Playwright. URLs to be crawled are supplied by a request provider, which can be
+either a `RequestList` containing a static list of URLs or a dynamic `RequestQueue`.
+
+Using a headless browser to download web pages and extract data, `PlaywrightCrawler` is ideal for crawling
+websites that require JavaScript execution. For websites that do not require JavaScript, consider using
+the `BeautifulSoupCrawler`, which utilizes raw HTTP requests and will be much faster.
+
+Example usage:
+
+```python
+import asyncio
+
+from crawlee.playwright_crawler import PlaywrightCrawler, PlaywrightCrawlingContext
+from crawlee.storages import Dataset, RequestQueue
+
+
+async def main() -> None:
+    # Open a default request queue and add requests to it
+    rq = await RequestQueue.open()
+    await rq.add_request('https://crawlee.dev')
+
+    # Open a default dataset for storing results
+    dataset = await Dataset.open()
+
+    # Create a crawler instance and provide a request provider (and other optional arguments)
+    crawler = PlaywrightCrawler(
+        request_provider=rq,
+        # headless=False,
+        # browser_type='firefox',
+    )
+
+    @crawler.router.default_handler
+    async def request_handler(context: PlaywrightCrawlingContext) -> None:
+        record = {
+            'request_url': context.request.url,
+            'page_url': context.page.url,
+            'page_title': await context.page.title(),
+            'page_content': (await context.page.content())[:10000],
+        }
+        await dataset.push_data(record)
+
+    await crawler.run()
+
+
+if __name__ == '__main__':
+    asyncio.run(main())
+```
+
+Example usage with custom browser pool:
+
+```python
+import asyncio
+
+from crawlee.browsers import BrowserPool, PlaywrightBrowserPlugin
+from crawlee.playwright_crawler import PlaywrightCrawler, PlaywrightCrawlingContext
+from crawlee.storages import Dataset, RequestQueue
+
+
+async def main() -> None:
+    # Open a default request queue and add requests to it
+    rq = await RequestQueue.open()
+    await rq.add_request('https://crawlee.dev')
+    await rq.add_request('https://apify.com')
+
+    # Open a default dataset for storing results
+    dataset = await Dataset.open()
+
+    # Create a browser pool with a Playwright browser plugin
+    browser_pool = BrowserPool(
+        plugins=[
+            PlaywrightBrowserPlugin(
+                browser_type='firefox',
+                browser_options={'headless': False},
+                page_options={'viewport': {'width': 1920, 'height': 1080}},
+            )
+        ]
+    )
+
+    # Create a crawler instance and provide a browser pool and request provider
+    crawler = PlaywrightCrawler(request_provider=rq, browser_pool=browser_pool)
+
+    @crawler.router.default_handler
+    async def request_handler(context: PlaywrightCrawlingContext) -> None:
+        record = {
+            'request_url': context.request.url,
+            'page_url': context.page.url,
+            'page_title': await context.page.title(),
+            'page_content': (await context.page.content())[:10000],
+        }
+        await dataset.push_data(record)
+
+    await crawler.run()
+
+
+if __name__ == '__main__':
+    asyncio.run(main())
+```
 
 ### Storages
 
 Crawlee introduces several result storage types that are useful for specific tasks. The storing of underlying data
 is realized by the storage client. Currently, only a memory storage client is implemented. Using this, the data
 are stored either in the memory or persisted on the disk.
 
@@ -458,14 +561,22 @@
     crawler = HttpCrawler(session_pool=session_pool_v1, use_session_pool=True)
 
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
+<!--
+### Browser Management
+
+- TODO
+- Write once browser rotation and/or other features are ready
+- Update PlaywrightCrawler according to this
+-->
+
 ## Running on the Apify platform
 
 Crawlee is open-source and runs anywhere, but since it's developed by [Apify](https://apify.com), it's easy to set up on the Apify platform and run in the cloud. Visit the [Apify SDK website](https://sdk.apify.com) to learn more about deploying Crawlee to the Apify platform.
 
 ## Support
 
 If you find any bug or issue with Crawlee, please [submit an issue on GitHub](https://github.com/apify/crawlee-py/issues). For questions, you can ask on [Stack Overflow](https://stackoverflow.com/questions/tagged/apify), in GitHub Discussions or you can join our [Discord server](https://discord.com/invite/jyEM2PRvMU).
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: crawlee Version: 0.0.4b2 Summary: Crawlee for
+Metadata-Version: 2.1 Name: crawlee Version: 0.0.4b3 Summary: Crawlee for
 Python License: Apache-2.0 Keywords:
 apify,automation,chrome,crawlee,crawler,headless,scraper,scraping Author: Apify
 Technologies s.r.o. Author-email: support@apify.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Provides-Extra: beautifulsoup
-Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aioshutil
-(>=1.3,<2.0) Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) ; extra ==
-"beautifulsoup" Requires-Dist: colorama (>=0.4.6,<0.5.0) Requires-Dist:
-docutils (>=0.21.0,<0.22.0) Requires-Dist: eval-type-backport (>=0.2.0,<0.3.0)
-Requires-Dist: html5lib (>=1.1,<2.0) ; extra == "beautifulsoup" Requires-Dist:
-httpx (>=0.27.0,<0.28.0) Requires-Dist: lxml (>=5.2.1,<6.0.0) ; extra ==
-"beautifulsoup" Requires-Dist: more_itertools (>=10.2.0,<11.0.0) Requires-Dist:
-psutil (>=5.9.8,<6.0.0) Requires-Dist: pydantic (>=2.6.3,<3.0.0) Requires-Dist:
-pydantic-settings (>=2.2.1,<3.0.0) Requires-Dist: pyee (>=11.1.0,<12.0.0)
-Requires-Dist: python-dateutil (>=2.9.0,<3.0.0) Requires-Dist:
-sortedcollections (>=2.1.0,<3.0.0) Requires-Dist: tldextract (>=5.1.2,<6.0.0)
-Requires-Dist: typing-extensions (>=4.1.0,<5.0.0) Project-URL: Apify Homepage,
-https://apify.com Project-URL: Changelog, https://github.com/apify/crawlee-py/
-blob/master/CHANGELOG.md Project-URL: Documentation, https://todo.com/ Project-
-URL: Homepage, https://todo.com/ Project-URL: Issue Tracker, https://
-github.com/apify/crawlee-py/issues Project-URL: Repository, https://github.com/
-apify/crawlee-py Description-Content-Type: text/markdown
+Provides-Extra: playwright Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-
+Dist: aioshutil (>=1.3,<2.0) Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0) ;
+extra == "beautifulsoup" Requires-Dist: colorama (>=0.4.6,<0.5.0) Requires-
+Dist: docutils (>=0.21.0,<0.22.0) Requires-Dist: eval-type-backport
+(>=0.2.0,<0.3.0) Requires-Dist: html5lib (>=1.1,<2.0) ; extra ==
+"beautifulsoup" Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: lxml
+(>=5.2.1,<6.0.0) ; extra == "beautifulsoup" Requires-Dist: more_itertools
+(>=10.2.0,<11.0.0) Requires-Dist: playwright (>=1.43.0,<2.0.0) ; extra ==
+"playwright" Requires-Dist: psutil (>=5.9.8,<6.0.0) Requires-Dist: pydantic
+(>=2.6.3,<3.0.0) Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0) Requires-
+Dist: pyee (>=11.1.0,<12.0.0) Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
+Requires-Dist: sortedcollections (>=2.1.0,<3.0.0) Requires-Dist: tldextract
+(>=5.1.2,<6.0.0) Requires-Dist: typing-extensions (>=4.1.0,<5.0.0) Project-URL:
+Apify Homepage, https://apify.com Project-URL: Changelog, https://github.com/
+apify/crawlee-py/blob/master/CHANGELOG.md Project-URL: Documentation, https://
+todo.com/ Project-URL: Homepage, https://todo.com/ Project-URL: Issue Tracker,
+https://github.com/apify/crawlee-py/issues Project-URL: Repository, https://
+github.com/apify/crawlee-py Description-Content-Type: text/markdown
                                ************ _[[_CC_rr_aa_ww_ll_ee_ee_]]
              AA wweebb ssccrraappiinngg aanndd bbrroowwsseerr aauuttoommaattiioonn lliibbrraarryy ************
 Crawlee covers your crawling and scraping end-to-end and **helps you build
 reliable scrapers. Fast.** Your crawlers will appear almost human-like and fly
 under the radar of modern bot protections even with the default configuration.
 Crawlee gives you the tools to crawl the web for links, scrape data, and store
 it to disk or cloud while staying configurable to suit your project's needs. We
@@ -122,30 +123,73 @@
 example with the updated request handler: ```python from
 crawlee.enqueue_strategy import EnqueueStrategy # ...
 @crawler.router.default_handler async def request_handler(context:
 BeautifulSoupCrawlingContext) -> None: # Use enqueue links helper to enqueue
 all links from the page with the same domain await context.enqueue_links
 (strategy=EnqueueStrategy.SAME_DOMAIN) record = { 'title':
 context.soup.title.text, 'url': context.request.url, } await dataset.push_data
-(record) ``` #### PlaywrightCrawler - TODO ### Storages Crawlee introduces
-several result storage types that are useful for specific tasks. The storing of
-underlying data is realized by the storage client. Currently, only a memory
-storage client is implemented. Using this, the data are stored either in the
-memory or persisted on the disk. By default, the data are stored in the
-directory specified by the `CRAWLEE_STORAGE_DIR` environment variable. With
-default `.storage/`. #### Dataset A [`Dataset`](https://github.com/apify/
-crawlee-py/blob/master/src/crawlee/storages/dataset.py) is a type of storage
-mainly suitable for storing tabular data. Datasets are used to store structured
-data where each object stored has the same attributes, such as online store
-products or real estate offers. The dataset can be imagined as a table, where
-each object is a row and its attributes are columns. The dataset is an append-
-only storage - we can only add new records to it, but we cannot modify or
-remove existing records. Each Crawlee project run is associated with a default
-dataset. Typically, it is used to store crawling results specific to the
-crawler run. Its usage is optional. The data are persisted as follows: ```
+(record) ``` #### PlaywrightCrawler [`PlaywrightCrawler`](https://github.com/
+apify/crawlee-py/tree/master/src/crawlee/playwright_crawler) extends the
+`BasicCrawler`. It provides the same features and on top of that, it uses
+[Playwright](https://playwright.dev/python) browser automation tool. This
+crawler provides a straightforward framework for parallel web page crawling
+using headless versions of Chromium, Firefox, and Webkit browsers through
+Playwright. URLs to be crawled are supplied by a request provider, which can be
+either a `RequestList` containing a static list of URLs or a dynamic
+`RequestQueue`. Using a headless browser to download web pages and extract
+data, `PlaywrightCrawler` is ideal for crawling websites that require
+JavaScript execution. For websites that do not require JavaScript, consider
+using the `BeautifulSoupCrawler`, which utilizes raw HTTP requests and will be
+much faster. Example usage: ```python import asyncio from
+crawlee.playwright_crawler import PlaywrightCrawler, PlaywrightCrawlingContext
+from crawlee.storages import Dataset, RequestQueue async def main() -> None: #
+Open a default request queue and add requests to it rq = await
+RequestQueue.open() await rq.add_request('https://crawlee.dev') # Open a
+default dataset for storing results dataset = await Dataset.open() # Create a
+crawler instance and provide a request provider (and other optional arguments)
+crawler = PlaywrightCrawler( request_provider=rq, # headless=False, #
+browser_type='firefox', ) @crawler.router.default_handler async def
+request_handler(context: PlaywrightCrawlingContext) -> None: record =
+{ 'request_url': context.request.url, 'page_url': context.page.url,
+'page_title': await context.page.title(), 'page_content': (await
+context.page.content())[:10000], } await dataset.push_data(record) await
+crawler.run() if __name__ == '__main__': asyncio.run(main()) ``` Example usage
+with custom browser pool: ```python import asyncio from crawlee.browsers import
+BrowserPool, PlaywrightBrowserPlugin from crawlee.playwright_crawler import
+PlaywrightCrawler, PlaywrightCrawlingContext from crawlee.storages import
+Dataset, RequestQueue async def main() -> None: # Open a default request queue
+and add requests to it rq = await RequestQueue.open() await rq.add_request
+('https://crawlee.dev') await rq.add_request('https://apify.com') # Open a
+default dataset for storing results dataset = await Dataset.open() # Create a
+browser pool with a Playwright browser plugin browser_pool = BrowserPool
+( plugins=[ PlaywrightBrowserPlugin( browser_type='firefox', browser_options=
+{'headless': False}, page_options={'viewport': {'width': 1920, 'height':
+1080}}, ) ] ) # Create a crawler instance and provide a browser pool and
+request provider crawler = PlaywrightCrawler(request_provider=rq,
+browser_pool=browser_pool) @crawler.router.default_handler async def
+request_handler(context: PlaywrightCrawlingContext) -> None: record =
+{ 'request_url': context.request.url, 'page_url': context.page.url,
+'page_title': await context.page.title(), 'page_content': (await
+context.page.content())[:10000], } await dataset.push_data(record) await
+crawler.run() if __name__ == '__main__': asyncio.run(main()) ``` ### Storages
+Crawlee introduces several result storage types that are useful for specific
+tasks. The storing of underlying data is realized by the storage client.
+Currently, only a memory storage client is implemented. Using this, the data
+are stored either in the memory or persisted on the disk. By default, the data
+are stored in the directory specified by the `CRAWLEE_STORAGE_DIR` environment
+variable. With default `.storage/`. #### Dataset A [`Dataset`](https://
+github.com/apify/crawlee-py/blob/master/src/crawlee/storages/dataset.py) is a
+type of storage mainly suitable for storing tabular data. Datasets are used to
+store structured data where each object stored has the same attributes, such as
+online store products or real estate offers. The dataset can be imagined as a
+table, where each object is a row and its attributes are columns. The dataset
+is an append-only storage - we can only add new records to it, but we cannot
+modify or remove existing records. Each Crawlee project run is associated with
+a default dataset. Typically, it is used to store crawling results specific to
+the crawler run. Its usage is optional. The data are persisted as follows: ```
 {CRAWLEE_STORAGE_DIR}/datasets/{DATASET_ID}/{INDEX}.json ``` The following code
 demonstrates the basic operations of the dataset: ```python import asyncio from
 crawlee.storages import Dataset async def main() -> None: # Open a default
 dataset dataset = await Dataset.open() # Push a single record await
 dataset.push_data({'key1': 'value1'}) # Get records from the dataset data =
 await dataset.get_data() print(f'Dataset data: {data.items}') # Dataset data: [
 {'key1': 'value1'}] # Open a named dataset dataset_named = await Dataset.open
```

