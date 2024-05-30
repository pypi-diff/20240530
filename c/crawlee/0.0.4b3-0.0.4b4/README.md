# Comparing `tmp/crawlee-0.0.4b3.tar.gz` & `tmp/crawlee-0.0.4b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.4b3.tar", max compression
+gzip compressed data, was "crawlee-0.0.4b4.tar", max compression
```

## Comparing `crawlee-0.0.4b3.tar` & `crawlee-0.0.4b4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    11355 2024-05-29 14:04:44.638610 crawlee-0.0.4b3/LICENSE
--rw-r--r--   0        0        0    20323 2024-05-29 14:04:44.638610 crawlee-0.0.4b3/README.md
--rw-r--r--   0        0        0     6790 2024-05-29 14:05:19.402664 crawlee-0.0.4b3/pyproject.toml
--rw-r--r--   0        0        0       31 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0      810 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/blocked.py
--rw-r--r--   0        0        0     3341 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1683 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     3503 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     5262 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/globs.py
--rw-r--r--   0        0        0     2056 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0      790 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/models.py
--rw-r--r--   0        0        0     1585 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      470 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/__init__.py
--rw-r--r--   0        0        0     9143 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_client.py
--rw-r--r--   0        0        0     1883 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_collection_client.py
--rw-r--r--   0        0        0     3486 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_client.py
--rw-r--r--   0        0        0     2025 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
--rw-r--r--   0        0        0     5622 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_client.py
--rw-r--r--   0        0        0     1992 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_collection_client.py
--rw-r--r--   0        0        0     2229 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/base_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/py.typed
--rw-r--r--   0        0        0      735 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/base_storage_client/types.py
--rw-r--r--   0        0        0      244 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    28954 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     4696 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2181 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/errors.py
--rw-r--r--   0        0        0     2279 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0     2820 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0      104 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     5574 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      524 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0      101 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/__init__.py
--rw-r--r--   0        0        0     1383 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/base_browser_plugin.py
--rw-r--r--   0        0        0     6184 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/browser_pool.py
--rw-r--r--   0        0        0     3104 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/playwright_browser_plugin.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/py.typed
--rw-r--r--   0        0        0      399 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/browsers/types.py
--rw-r--r--   0        0        0     1310 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/configuration.py
--rw-r--r--   0        0        0      182 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/consts.py
--rw-r--r--   0        0        0      308 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/enqueue_strategy.py
--rw-r--r--   0        0        0       91 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2682 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1556 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     2140 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     5085 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       77 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     2992 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/log_config.py
--rw-r--r--   0        0        0       55 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/__init__.py
--rw-r--r--   0        0        0    15666 2024-05-29 14:04:44.642610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/_creation_management.py
--rw-r--r--   0        0        0    15684 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_client.py
--rw-r--r--   0        0        0     2243 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_collection_client.py
--rw-r--r--   0        0        0    15914 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_client.py
--rw-r--r--   0        0        0     2333 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_collection_client.py
--rw-r--r--   0        0        0    11113 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/py.typed
--rw-r--r--   0        0        0    20944 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_client.py
--rw-r--r--   0        0        0     2316 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_collection_client.py
--rw-r--r--   0        0        0    13847 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/models.py
--rw-r--r--   0        0        0       95 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/playwright_crawler/__init__.py
--rw-r--r--   0        0        0     3076 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/playwright_crawler/playwright_crawler.py
--rw-r--r--   0        0        0      381 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/playwright_crawler/types.py
--rw-r--r--   0        0        0     7393 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/proxy_configuration.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/py.typed
--rw-r--r--   0        0        0       67 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8084 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/__init__.py
--rw-r--r--   0        0        0      980 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/error_tracker.py
--rw-r--r--   0        0        0     3646 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/models.py
--rw-r--r--   0        0        0    10880 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/statistics/statistics.py
--rw-r--r--   0        0        0     1520 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      150 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     8804 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/_creation_management.py
--rw-r--r--   0        0        0     1090 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15956 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     4994 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0        0 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2841 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2755 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25708 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-05-29 14:04:44.646610 crawlee-0.0.4b3/src/crawlee/types.py
--rw-r--r--   0        0        0    22484 1970-01-01 00:00:00.000000 crawlee-0.0.4b3/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-30 09:06:43.210505 crawlee-0.0.4b4/LICENSE
+-rw-r--r--   0        0        0    20669 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/README.md
+-rw-r--r--   0        0        0     6790 2024-05-30 09:07:23.770973 crawlee-0.0.4b4/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/blocked.py
+-rw-r--r--   0        0        0     3341 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1683 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     3503 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     5262 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/globs.py
+-rw-r--r--   0        0        0     2056 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0      790 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/models.py
+-rw-r--r--   0        0        0     1585 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      470 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/__init__.py
+-rw-r--r--   0        0        0     9143 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/base_dataset_client.py
+-rw-r--r--   0        0        0     1883 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/base_dataset_collection_client.py
+-rw-r--r--   0        0        0     3486 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/base_key_value_store_client.py
+-rw-r--r--   0        0        0     2025 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/base_key_value_store_collection_client.py
+-rw-r--r--   0        0        0     5622 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/base_request_queue_client.py
+-rw-r--r--   0        0        0     1992 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/base_request_queue_collection_client.py
+-rw-r--r--   0        0        0     2229 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/base_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/py.typed
+-rw-r--r--   0        0        0      735 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/base_storage_client/types.py
+-rw-r--r--   0        0        0      244 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    28954 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     4696 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2181 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/basic_crawler/errors.py
+-rw-r--r--   0        0        0     2279 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0     2820 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0      104 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     5574 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      524 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0      101 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/browsers/__init__.py
+-rw-r--r--   0        0        0     1383 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/browsers/base_browser_plugin.py
+-rw-r--r--   0        0        0     6184 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/browsers/browser_pool.py
+-rw-r--r--   0        0        0     3104 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/browsers/playwright_browser_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/browsers/py.typed
+-rw-r--r--   0        0        0      399 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/browsers/types.py
+-rw-r--r--   0        0        0     1310 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/configuration.py
+-rw-r--r--   0        0        0      182 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/consts.py
+-rw-r--r--   0        0        0      308 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/enqueue_strategy.py
+-rw-r--r--   0        0        0       91 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2682 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1556 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     2140 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     5085 2024-05-30 09:06:43.214505 crawlee-0.0.4b4/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       77 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     2992 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/log_config.py
+-rw-r--r--   0        0        0       55 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/__init__.py
+-rw-r--r--   0        0        0    15666 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/_creation_management.py
+-rw-r--r--   0        0        0    15684 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/dataset_client.py
+-rw-r--r--   0        0        0     2243 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/dataset_collection_client.py
+-rw-r--r--   0        0        0    15914 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/key_value_store_client.py
+-rw-r--r--   0        0        0     2333 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/key_value_store_collection_client.py
+-rw-r--r--   0        0        0    11113 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/py.typed
+-rw-r--r--   0        0        0    20944 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/request_queue_client.py
+-rw-r--r--   0        0        0     2316 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/memory_storage_client/request_queue_collection_client.py
+-rw-r--r--   0        0        0    13847 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/models.py
+-rw-r--r--   0        0        0       95 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/playwright_crawler/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/playwright_crawler/playwright_crawler.py
+-rw-r--r--   0        0        0      381 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/playwright_crawler/types.py
+-rw-r--r--   0        0        0     7393 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/proxy_configuration.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/py.typed
+-rw-r--r--   0        0        0       67 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8084 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/statistics/__init__.py
+-rw-r--r--   0        0        0      980 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/statistics/error_tracker.py
+-rw-r--r--   0        0        0     3646 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/statistics/models.py
+-rw-r--r--   0        0        0    10880 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/statistics/statistics.py
+-rw-r--r--   0        0        0     1520 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      150 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     8804 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/_creation_management.py
+-rw-r--r--   0        0        0     1090 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15956 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4994 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0        0 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2841 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2755 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25708 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-05-30 09:06:43.218505 crawlee-0.0.4b4/src/crawlee/types.py
+-rw-r--r--   0        0        0    22830 1970-01-01 00:00:00.000000 crawlee-0.0.4b4/PKG-INFO
```

### Comparing `crawlee-0.0.4b3/LICENSE` & `crawlee-0.0.4b4/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/README.md` & `crawlee-0.0.4b4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,32 @@
 
 If you plan to use `BeautifulSoupCrawler`, install `crawlee` with `beautifulsoup` extra:
 
 ```bash
 pip install 'crawlee[beautifulsoup]'
 ```
 
+If you plan to use `PlaywrightCrawler`, install `crawlee` with the `playwright` extra:
+
+```bash
+pip install 'crawlee[playwright]'
+```
+
+Then, install the Playwright dependencies:
+
+```bash
+playwright install
+```
+
+You can install multiple extras at once by using a comma as a separator:
+
+```bash
+pip install 'crawlee[beautifulsoup,playwright]'
+```
+
 ## Features
 
 - Unified interface for **HTTP and headless browser** crawling.
 - Persistent **queue** for URLs to crawl (breadth & depth-first).
 - Pluggable **storage** of both tabular data and files.
 - Automatic **scaling** with available system resources.
 - Integrated **proxy rotation** and session management.
```

#### html2text {}

```diff
@@ -8,58 +8,63 @@
 also have a TypeScript implementation of the Crawlee, which you can explore and
 utilize for your projects. Visit our GitHub repository for more information
 [Crawlee on GitHub](https://github.com/apify/crawlee). ## Installation Crawlee
 is available as the [`crawlee`](https://pypi.org/project/crawlee/) PyPI
 package. ```bash pip install crawlee ``` Additional, optional dependencies
 unlocking more features are shipped as package extras. If you plan to use
 `BeautifulSoupCrawler`, install `crawlee` with `beautifulsoup` extra: ```bash
-pip install 'crawlee[beautifulsoup]' ``` ## Features - Unified interface for
-**HTTP and headless browser** crawling. - Persistent **queue** for URLs to
-crawl (breadth & depth-first). - Pluggable **storage** of both tabular data and
-files. - Automatic **scaling** with available system resources. - Integrated
-**proxy rotation** and session management. - Configurable **request routing** -
-directing URLs to appropriate handlers. - Robust **error handling**. -
-Automatic **retries** when getting blocked. - Written in Python with **type
-hints**, which means better DX and fewer bugs. ## Introduction Crawlee covers
-your crawling and scraping end-to-end and helps you build reliable scrapers.
-Fast. Your crawlers will appear human-like and fly under the radar of modern
-bot protections even with the default configuration. Crawlee gives you the
-tools to crawl the web for links, scrape data and persistently store it in
-machine-readable formats, without having to worry about the technical details.
-And thanks to rich configuration options, you can tweak almost any aspect of
-Crawlee to suit your project's needs if the default settings don't cut it. ###
-Crawlers Crawlee offers a framework for parallel web crawling through a variety
-of crawler classes, each designed to meet different crawling needs. ####
-HttpCrawler [`HttpCrawler`](https://github.com/apify/crawlee-py/tree/master/
-src/crawlee/http_crawler) provides a framework for the parallel crawling of web
-pages using plain HTTP requests. The URLs to crawl are fed from a request
-provider. It enables the recursive crawling of websites. The parsing of
-obtained HTML is the user's responsibility. Since `HttpCrawler` uses raw HTTP
-requests to download web pages, it is very fast and efficient on data
-bandwidth. However, if the target website requires JavaScript to display the
-content, you might need to use some browser crawler instead, e.g.
-`PlaywrightCrawler`, because it loads the pages using a full-featured headless
-Chrome browser. `HttpCrawler` downloads each URL using a plain HTTP request,
-obtain the response and then invokes the user-provided request handler to
-extract page data. The source URLs are represented using the [`Request`](https:
-//github.com/apify/crawlee-py/blob/master/src/crawlee/models.py) objects that
-are fed from [`RequestList`](https://github.com/apify/crawlee-py/blob/master/
-src/crawlee/storages/request_list.py) or [`RequestQueue`](https://github.com/
-apify/crawlee-py/blob/master/src/crawlee/storages/request_queue.py) instances
-provided by the request provider option. The crawler finishes when there are no
-more Request objects to crawl. If you want to parse data using [BeautifulSoup]
-(https://pypi.org/project/beautifulsoup4/) see the `BeautifulSoupCrawler`
-section. Example usage: ```python import asyncio from crawlee.http_crawler
-import HttpCrawler, HttpCrawlingContext from crawlee.storages import Dataset,
-RequestQueue async def main() -> None: # Open a default request queue and add
-requests to it rq = await RequestQueue.open() await rq.add_request('https://
-crawlee.dev') # Open a default dataset for storing results dataset = await
-Dataset.open() # Create a HttpCrawler instance and provide a request provider
-crawler = HttpCrawler(request_provider=rq) # Define a handler for processing
-requests @crawler.router.default_handler async def request_handler(context:
+pip install 'crawlee[beautifulsoup]' ``` If you plan to use
+`PlaywrightCrawler`, install `crawlee` with the `playwright` extra: ```bash pip
+install 'crawlee[playwright]' ``` Then, install the Playwright dependencies:
+```bash playwright install ``` You can install multiple extras at once by using
+a comma as a separator: ```bash pip install 'crawlee[beautifulsoup,playwright]'
+``` ## Features - Unified interface for **HTTP and headless browser** crawling.
+- Persistent **queue** for URLs to crawl (breadth & depth-first). - Pluggable
+**storage** of both tabular data and files. - Automatic **scaling** with
+available system resources. - Integrated **proxy rotation** and session
+management. - Configurable **request routing** - directing URLs to appropriate
+handlers. - Robust **error handling**. - Automatic **retries** when getting
+blocked. - Written in Python with **type hints**, which means better DX and
+fewer bugs. ## Introduction Crawlee covers your crawling and scraping end-to-
+end and helps you build reliable scrapers. Fast. Your crawlers will appear
+human-like and fly under the radar of modern bot protections even with the
+default configuration. Crawlee gives you the tools to crawl the web for links,
+scrape data and persistently store it in machine-readable formats, without
+having to worry about the technical details. And thanks to rich configuration
+options, you can tweak almost any aspect of Crawlee to suit your project's
+needs if the default settings don't cut it. ### Crawlers Crawlee offers a
+framework for parallel web crawling through a variety of crawler classes, each
+designed to meet different crawling needs. #### HttpCrawler [`HttpCrawler`]
+(https://github.com/apify/crawlee-py/tree/master/src/crawlee/http_crawler)
+provides a framework for the parallel crawling of web pages using plain HTTP
+requests. The URLs to crawl are fed from a request provider. It enables the
+recursive crawling of websites. The parsing of obtained HTML is the user's
+responsibility. Since `HttpCrawler` uses raw HTTP requests to download web
+pages, it is very fast and efficient on data bandwidth. However, if the target
+website requires JavaScript to display the content, you might need to use some
+browser crawler instead, e.g. `PlaywrightCrawler`, because it loads the pages
+using a full-featured headless Chrome browser. `HttpCrawler` downloads each URL
+using a plain HTTP request, obtain the response and then invokes the user-
+provided request handler to extract page data. The source URLs are represented
+using the [`Request`](https://github.com/apify/crawlee-py/blob/master/src/
+crawlee/models.py) objects that are fed from [`RequestList`](https://
+github.com/apify/crawlee-py/blob/master/src/crawlee/storages/request_list.py)
+or [`RequestQueue`](https://github.com/apify/crawlee-py/blob/master/src/
+crawlee/storages/request_queue.py) instances provided by the request provider
+option. The crawler finishes when there are no more Request objects to crawl.
+If you want to parse data using [BeautifulSoup](https://pypi.org/project/
+beautifulsoup4/) see the `BeautifulSoupCrawler` section. Example usage:
+```python import asyncio from crawlee.http_crawler import HttpCrawler,
+HttpCrawlingContext from crawlee.storages import Dataset, RequestQueue async
+def main() -> None: # Open a default request queue and add requests to it rq =
+await RequestQueue.open() await rq.add_request('https://crawlee.dev') # Open a
+default dataset for storing results dataset = await Dataset.open() # Create a
+HttpCrawler instance and provide a request provider crawler = HttpCrawler
+(request_provider=rq) # Define a handler for processing requests
+@crawler.router.default_handler async def request_handler(context:
 HttpCrawlingContext) -> None: # Crawler will provide a HttpCrawlingContext
 instance, # from which you can access the request and response data record =
 { 'url': context.request.url, 'status_code': context.http_response.status_code,
 'headers': dict(context.http_response.headers), 'response':
 context.http_response.read().decode()[:1000], } # Extract the record and push
 it to the dataset await dataset.push_data(record) # Run the crawler await
 crawler.run() if __name__ == '__main__': asyncio.run(main()) ``` For further
```

### Comparing `crawlee-0.0.4b3/pyproject.toml` & `crawlee-0.0.4b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.4b3"
+version = "0.0.4b4"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/blocked.py` & `crawlee-0.0.4b4/src/crawlee/_utils/blocked.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.4b4/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/crypto.py` & `crawlee-0.0.4b4/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.4b4/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.4b4/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/file.py` & `crawlee-0.0.4b4/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/globs.py` & `crawlee-0.0.4b4/src/crawlee/_utils/globs.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.4b4/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/math.py` & `crawlee-0.0.4b4/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.4b4/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/models.py` & `crawlee-0.0.4b4/src/crawlee/_utils/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.4b4/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/requests.py` & `crawlee-0.0.4b4/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/system.py` & `crawlee-0.0.4b4/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/_utils/wait.py` & `crawlee-0.0.4b4/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.4b4/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.4b4/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.4b4/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/autoscaling/types.py` & `crawlee-0.0.4b4/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_client.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/base_dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_dataset_collection_client.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/base_dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_client.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/base_key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_key_value_store_collection_client.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/base_key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_client.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/base_request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_request_queue_collection_client.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/base_request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/base_storage_client.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/base_storage_client/types.py` & `crawlee-0.0.4b4/src/crawlee/base_storage_client/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.4b4/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.4b4/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/basic_crawler/errors.py` & `crawlee-0.0.4b4/src/crawlee/basic_crawler/errors.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.4b4/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/basic_crawler/types.py` & `crawlee-0.0.4b4/src/crawlee/basic_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.4b4/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/beautifulsoup_crawler/types.py` & `crawlee-0.0.4b4/src/crawlee/beautifulsoup_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/browsers/base_browser_plugin.py` & `crawlee-0.0.4b4/src/crawlee/browsers/base_browser_plugin.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/browsers/browser_pool.py` & `crawlee-0.0.4b4/src/crawlee/browsers/browser_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/browsers/playwright_browser_plugin.py` & `crawlee-0.0.4b4/src/crawlee/browsers/playwright_browser_plugin.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/configuration.py` & `crawlee-0.0.4b4/src/crawlee/configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/events/event_manager.py` & `crawlee-0.0.4b4/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.4b4/src/crawlee/events/local_event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/events/types.py` & `crawlee-0.0.4b4/src/crawlee/events/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.4b4/src/crawlee/http_clients/base_http_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/http_clients/httpx_client.py` & `crawlee-0.0.4b4/src/crawlee/http_clients/httpx_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.4b4/src/crawlee/http_crawler/http_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/log_config.py` & `crawlee-0.0.4b4/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/_creation_management.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/_creation_management.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_client.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/dataset_collection_client.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_client.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/key_value_store_collection_client.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/memory_storage_client.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_client.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/memory_storage_client/request_queue_collection_client.py` & `crawlee-0.0.4b4/src/crawlee/memory_storage_client/request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/models.py` & `crawlee-0.0.4b4/src/crawlee/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/playwright_crawler/playwright_crawler.py` & `crawlee-0.0.4b4/src/crawlee/playwright_crawler/playwright_crawler.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/proxy_configuration.py` & `crawlee-0.0.4b4/src/crawlee/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/sessions/models.py` & `crawlee-0.0.4b4/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/sessions/session.py` & `crawlee-0.0.4b4/src/crawlee/sessions/session.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.4b4/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/statistics/error_tracker.py` & `crawlee-0.0.4b4/src/crawlee/statistics/error_tracker.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/statistics/models.py` & `crawlee-0.0.4b4/src/crawlee/statistics/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/statistics/statistics.py` & `crawlee-0.0.4b4/src/crawlee/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storage_client_manager.py` & `crawlee-0.0.4b4/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storages/_creation_management.py` & `crawlee-0.0.4b4/src/crawlee/storages/_creation_management.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storages/base_storage.py` & `crawlee-0.0.4b4/src/crawlee/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storages/dataset.py` & `crawlee-0.0.4b4/src/crawlee/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.4b4/src/crawlee/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storages/request_list.py` & `crawlee-0.0.4b4/src/crawlee/storages/request_list.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storages/request_provider.py` & `crawlee-0.0.4b4/src/crawlee/storages/request_provider.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/storages/request_queue.py` & `crawlee-0.0.4b4/src/crawlee/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/src/crawlee/types.py` & `crawlee-0.0.4b4/src/crawlee/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.4b3/PKG-INFO` & `crawlee-0.0.4b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.4b3
+Version: 0.0.4b4
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -78,14 +78,32 @@
 
 If you plan to use `BeautifulSoupCrawler`, install `crawlee` with `beautifulsoup` extra:
 
 ```bash
 pip install 'crawlee[beautifulsoup]'
 ```
 
+If you plan to use `PlaywrightCrawler`, install `crawlee` with the `playwright` extra:
+
+```bash
+pip install 'crawlee[playwright]'
+```
+
+Then, install the Playwright dependencies:
+
+```bash
+playwright install
+```
+
+You can install multiple extras at once by using a comma as a separator:
+
+```bash
+pip install 'crawlee[beautifulsoup,playwright]'
+```
+
 ## Features
 
 - Unified interface for **HTTP and headless browser** crawling.
 - Persistent **queue** for URLs to crawl (breadth & depth-first).
 - Pluggable **storage** of both tabular data and files.
 - Automatic **scaling** with available system resources.
 - Integrated **proxy rotation** and session management.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlee Version: 0.0.4b3 Summary: Crawlee for
+Metadata-Version: 2.1 Name: crawlee Version: 0.0.4b4 Summary: Crawlee for
 Python License: Apache-2.0 Keywords:
 apify,automation,chrome,crawlee,crawler,headless,scraper,scraping Author: Apify
 Technologies s.r.o. Author-email: support@apify.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -37,58 +37,63 @@
 also have a TypeScript implementation of the Crawlee, which you can explore and
 utilize for your projects. Visit our GitHub repository for more information
 [Crawlee on GitHub](https://github.com/apify/crawlee). ## Installation Crawlee
 is available as the [`crawlee`](https://pypi.org/project/crawlee/) PyPI
 package. ```bash pip install crawlee ``` Additional, optional dependencies
 unlocking more features are shipped as package extras. If you plan to use
 `BeautifulSoupCrawler`, install `crawlee` with `beautifulsoup` extra: ```bash
-pip install 'crawlee[beautifulsoup]' ``` ## Features - Unified interface for
-**HTTP and headless browser** crawling. - Persistent **queue** for URLs to
-crawl (breadth & depth-first). - Pluggable **storage** of both tabular data and
-files. - Automatic **scaling** with available system resources. - Integrated
-**proxy rotation** and session management. - Configurable **request routing** -
-directing URLs to appropriate handlers. - Robust **error handling**. -
-Automatic **retries** when getting blocked. - Written in Python with **type
-hints**, which means better DX and fewer bugs. ## Introduction Crawlee covers
-your crawling and scraping end-to-end and helps you build reliable scrapers.
-Fast. Your crawlers will appear human-like and fly under the radar of modern
-bot protections even with the default configuration. Crawlee gives you the
-tools to crawl the web for links, scrape data and persistently store it in
-machine-readable formats, without having to worry about the technical details.
-And thanks to rich configuration options, you can tweak almost any aspect of
-Crawlee to suit your project's needs if the default settings don't cut it. ###
-Crawlers Crawlee offers a framework for parallel web crawling through a variety
-of crawler classes, each designed to meet different crawling needs. ####
-HttpCrawler [`HttpCrawler`](https://github.com/apify/crawlee-py/tree/master/
-src/crawlee/http_crawler) provides a framework for the parallel crawling of web
-pages using plain HTTP requests. The URLs to crawl are fed from a request
-provider. It enables the recursive crawling of websites. The parsing of
-obtained HTML is the user's responsibility. Since `HttpCrawler` uses raw HTTP
-requests to download web pages, it is very fast and efficient on data
-bandwidth. However, if the target website requires JavaScript to display the
-content, you might need to use some browser crawler instead, e.g.
-`PlaywrightCrawler`, because it loads the pages using a full-featured headless
-Chrome browser. `HttpCrawler` downloads each URL using a plain HTTP request,
-obtain the response and then invokes the user-provided request handler to
-extract page data. The source URLs are represented using the [`Request`](https:
-//github.com/apify/crawlee-py/blob/master/src/crawlee/models.py) objects that
-are fed from [`RequestList`](https://github.com/apify/crawlee-py/blob/master/
-src/crawlee/storages/request_list.py) or [`RequestQueue`](https://github.com/
-apify/crawlee-py/blob/master/src/crawlee/storages/request_queue.py) instances
-provided by the request provider option. The crawler finishes when there are no
-more Request objects to crawl. If you want to parse data using [BeautifulSoup]
-(https://pypi.org/project/beautifulsoup4/) see the `BeautifulSoupCrawler`
-section. Example usage: ```python import asyncio from crawlee.http_crawler
-import HttpCrawler, HttpCrawlingContext from crawlee.storages import Dataset,
-RequestQueue async def main() -> None: # Open a default request queue and add
-requests to it rq = await RequestQueue.open() await rq.add_request('https://
-crawlee.dev') # Open a default dataset for storing results dataset = await
-Dataset.open() # Create a HttpCrawler instance and provide a request provider
-crawler = HttpCrawler(request_provider=rq) # Define a handler for processing
-requests @crawler.router.default_handler async def request_handler(context:
+pip install 'crawlee[beautifulsoup]' ``` If you plan to use
+`PlaywrightCrawler`, install `crawlee` with the `playwright` extra: ```bash pip
+install 'crawlee[playwright]' ``` Then, install the Playwright dependencies:
+```bash playwright install ``` You can install multiple extras at once by using
+a comma as a separator: ```bash pip install 'crawlee[beautifulsoup,playwright]'
+``` ## Features - Unified interface for **HTTP and headless browser** crawling.
+- Persistent **queue** for URLs to crawl (breadth & depth-first). - Pluggable
+**storage** of both tabular data and files. - Automatic **scaling** with
+available system resources. - Integrated **proxy rotation** and session
+management. - Configurable **request routing** - directing URLs to appropriate
+handlers. - Robust **error handling**. - Automatic **retries** when getting
+blocked. - Written in Python with **type hints**, which means better DX and
+fewer bugs. ## Introduction Crawlee covers your crawling and scraping end-to-
+end and helps you build reliable scrapers. Fast. Your crawlers will appear
+human-like and fly under the radar of modern bot protections even with the
+default configuration. Crawlee gives you the tools to crawl the web for links,
+scrape data and persistently store it in machine-readable formats, without
+having to worry about the technical details. And thanks to rich configuration
+options, you can tweak almost any aspect of Crawlee to suit your project's
+needs if the default settings don't cut it. ### Crawlers Crawlee offers a
+framework for parallel web crawling through a variety of crawler classes, each
+designed to meet different crawling needs. #### HttpCrawler [`HttpCrawler`]
+(https://github.com/apify/crawlee-py/tree/master/src/crawlee/http_crawler)
+provides a framework for the parallel crawling of web pages using plain HTTP
+requests. The URLs to crawl are fed from a request provider. It enables the
+recursive crawling of websites. The parsing of obtained HTML is the user's
+responsibility. Since `HttpCrawler` uses raw HTTP requests to download web
+pages, it is very fast and efficient on data bandwidth. However, if the target
+website requires JavaScript to display the content, you might need to use some
+browser crawler instead, e.g. `PlaywrightCrawler`, because it loads the pages
+using a full-featured headless Chrome browser. `HttpCrawler` downloads each URL
+using a plain HTTP request, obtain the response and then invokes the user-
+provided request handler to extract page data. The source URLs are represented
+using the [`Request`](https://github.com/apify/crawlee-py/blob/master/src/
+crawlee/models.py) objects that are fed from [`RequestList`](https://
+github.com/apify/crawlee-py/blob/master/src/crawlee/storages/request_list.py)
+or [`RequestQueue`](https://github.com/apify/crawlee-py/blob/master/src/
+crawlee/storages/request_queue.py) instances provided by the request provider
+option. The crawler finishes when there are no more Request objects to crawl.
+If you want to parse data using [BeautifulSoup](https://pypi.org/project/
+beautifulsoup4/) see the `BeautifulSoupCrawler` section. Example usage:
+```python import asyncio from crawlee.http_crawler import HttpCrawler,
+HttpCrawlingContext from crawlee.storages import Dataset, RequestQueue async
+def main() -> None: # Open a default request queue and add requests to it rq =
+await RequestQueue.open() await rq.add_request('https://crawlee.dev') # Open a
+default dataset for storing results dataset = await Dataset.open() # Create a
+HttpCrawler instance and provide a request provider crawler = HttpCrawler
+(request_provider=rq) # Define a handler for processing requests
+@crawler.router.default_handler async def request_handler(context:
 HttpCrawlingContext) -> None: # Crawler will provide a HttpCrawlingContext
 instance, # from which you can access the request and response data record =
 { 'url': context.request.url, 'status_code': context.http_response.status_code,
 'headers': dict(context.http_response.headers), 'response':
 context.http_response.read().decode()[:1000], } # Extract the record and push
 it to the dataset await dataset.push_data(record) # Run the crawler await
 crawler.run() if __name__ == '__main__': asyncio.run(main()) ``` For further
```

