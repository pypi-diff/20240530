# Comparing `tmp/datapools-1.0.64.tar.gz` & `tmp/datapools-1.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.64.tar", last modified: Tue May 28 10:48:13 2024, max compression
+gzip compressed data, was "datapools-1.0.65.tar", last modified: Thu May 30 17:36:34 2024, max compression
```

## Comparing `datapools-1.0.64.tar` & `datapools-1.0.65.tar`

### file list

```diff
@@ -1,93 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.828412 datapools-1.0.64/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 10:48:05.000000 datapools-1.0.64/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    21946 2024-05-28 10:48:05.000000 datapools-1.0.64/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-28 10:48:05.000000 datapools-1.0.64/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 10:48:05.000000 datapools-1.0.64/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-28 10:48:13.828412 datapools-1.0.64/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-28 10:48:05.000000 datapools-1.0.64/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.808412 datapools-1.0.64/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.812412 datapools-1.0.64/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-28 10:48:05.000000 datapools-1.0.64/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.828412 datapools-1.0.64/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 10:48:13.000000 datapools-1.0.64/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 10:48:13.828412 datapools-1.0.64/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-28 10:48:05.000000 datapools-1.0.64/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:13.816412 datapools-1.0.64/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 10:48:05.000000 datapools-1.0.64/tests/test_session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.455496 datapools-1.0.65/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-30 17:36:26.000000 datapools-1.0.65/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    22354 2024-05-30 17:36:26.000000 datapools-1.0.65/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-30 17:36:26.000000 datapools-1.0.65/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 17:36:26.000000 datapools-1.0.65/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-30 17:36:34.455496 datapools-1.0.65/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-30 17:36:26.000000 datapools-1.0.65/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.443496 datapools-1.0.65/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.443496 datapools-1.0.65/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.443496 datapools-1.0.65/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/ftp/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/ftp/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/ftp/ftp_dir_listing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20285 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.455496 datapools-1.0.65/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:36:34.455496 datapools-1.0.65/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 17:36:26.000000 datapools-1.0.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.455496 datapools-1.0.65/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/test_session_manager.py
```

### Comparing `datapools-1.0.64/HISTORY.md` & `datapools-1.0.65/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Linter + demo tag. [sergpsu]
+- Linter. [sergpsu]
+- Cleanup. [sergpsu]
+- Io operations instead of memory, FTP beta. [sergpsu]
+- Merge remote-tracking branch 'origin/master' into sergpsu-io-support.
+  [sergpsu]
+- Merge pull request #83 from torrentsai/sergpsu-delete-all-sessions.
+  [S]
+
+  Drive.google.com demo users bugfix
+
+
+1.0.64 (2024-05-28)
+-------------------
+- Release: version 1.0.64 🚀 [sergpsu]
 - Merge remote-tracking branch 'origin/master' into sergpsu-delete-all-
   sessions. [sergpsu]
 - Merge pull request #50 from
   torrentsai/dependabot/github_actions/codecov/codecov-action-4.
   [voldmr]
 
   Bump codecov/codecov-action from 3 to 4
```

### Comparing `datapools-1.0.64/LICENSE` & `datapools-1.0.65/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/PKG-INFO` & `datapools-1.0.65/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.64
+Version: 1.0.65
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
@@ -22,14 +22,15 @@
 Requires-Dist: azure-identity
 Requires-Dist: msgraph-sdk
 Requires-Dist: aio-pika
 Requires-Dist: dnspython
 Requires-Dist: pillow
 Requires-Dist: pytest-playwright
 Requires-Dist: bs4
+Requires-Dist: python-magic
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `datapools-1.0.64/README.md` & `datapools-1.0.65/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/api.py` & `datapools-1.0.65/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/cli.py` & `datapools-1.0.65/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/backend_api.py` & `datapools-1.0.65/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/queues/__init__.py` & `datapools-1.0.65/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/queues/rabbitmq.py` & `datapools-1.0.65/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/queues/types.py` & `datapools-1.0.65/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/session_manager.py` & `datapools-1.0.65/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/stoppable.py` & `datapools-1.0.65/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.65/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.65/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/common/types.py` & `datapools-1.0.65/datapools/common/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 class CrawlerContent(BaseCrawlerResult):
     tag_id: Optional[str] = None
     tag_keepout: Optional[bool] = False
     copyright_tag_id: Optional[str] = None
     copyright_tag_keepout: Optional[bool] = False
     platform_tag_id: Optional[str] = None
     platform_tag_keepout: Optional[bool] = False
-    type: DatapoolContentType
+    type: Optional[DatapoolContentType] = None
     # storage_id: Any
     url: Union[str, AnyUrl]
     priority_timestamp: Optional[int] = None
     content: Optional[Any] = None
 
     def to_dict(self):
         res = self.__dict__
```

### Comparing `datapools-1.0.64/datapools/producer/base_producer.py` & `datapools-1.0.65/datapools/producer/base_producer.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,16 +97,16 @@
                         if qm.type == QueueMessageType.Task:
                             task = qm.data
                             logger.info(f"Producer got: {task}")
 
                             # TODO: this storage must be associated with the worker!
                             #   For example, storage path or url can be formatted accordingly to worker id
                             worker_storage = WorkerFileStorage(self.cfg.WORKER_STORAGE_PATH, task["worker_id"])
-                            raw_data = await worker_storage.get(task["storage_id"])
-                            await self.process_content(session, raw_data, task)
+                            with worker_storage.get_reader(task["storage_id"]) as raw_data_reader:
+                                await self.process_content(session, raw_data_reader, task)
 
                             if not self.is_shared_storage():
                                 # tell worker that his storage item can be removed
                                 await self.topics_queue.push(
                                     QueueTopicMessage(
                                         get_storage_invalidation_topic(task["worker_id"]),
                                         {"storage_id": task["storage_id"]},
@@ -130,14 +130,15 @@
                         await self.eval_queue.reject(message, requeue=False)
 
         except Exception as e:
             logger.error(f"Catched: {traceback.format_exc()}")
             logger.error(f"!!!!!!! Exception in Datapools::router_loop() {e}")
 
     async def process_content(self, session: Session, raw_data, task):
+        logger.info(f"BaseProducer::process_content {type(raw_data)=}")
         # path = os.path.join(self.cfg.STORAGE_PATH, str(datapool_id))
         if not self.is_shared_storage():
             path = self.cfg.STORAGE_PATH
             if not os.path.exists(path):  # type: ignore
                 os.mkdir(path)  # type: ignore
             storage = FileStorage(path)
             # put data into persistent storage
```

### Comparing `datapools-1.0.64/datapools/scheduler/scheduler.py` & `datapools-1.0.65/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.65/datapools/worker/plugins/base_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import io
 import sys
 from abc import ABCMeta, abstractmethod
 from hashlib import md5
 from time import time
 from typing import AsyncGenerator, Union, Optional
 from urllib.parse import urljoin, urlparse
+import magic
 
 import dns.resolver
 import httpx
 from PIL import Image
 from PIL.ExifTags import Base as ExifTagsList
 
 from ...common.logger import logger
@@ -134,14 +135,25 @@
             async with httpx.AsyncClient(max_redirects=max_redirects) as client:
                 r = await client.get(url, follow_redirects=follow_redirects, headers=headers)
                 return r.content
 
         except Exception as e:
             logger.error(f"failed get content of {url}: {e}")
 
+    async def async_read_url(self, url, headers={}, follow_redirects=True, max_redirects=5):
+        logger.info(f"BasePlugin.async_read_url {url=}")
+        try:
+            async with httpx.AsyncClient(max_redirects=max_redirects) as client:
+                async with client.stream("GET", url, follow_redirects=follow_redirects, headers=headers) as stream:
+                    async for chunk in stream.aiter_bytes():
+                        yield chunk
+
+        except Exception as e:
+            logger.error(f"failed get content of {url}: {e}")
+
     @staticmethod
     def parse_url(url):
         return urlparse(url)
 
     @staticmethod
     @abstractmethod
     def is_supported(url):
@@ -254,33 +266,48 @@
             for elem in await elems.all():
                 c = await elem.text_content()
                 if c is not None:
                     return BasePlugin.parse_tag_in_str(c)
         return None
 
     @staticmethod
-    def get_content_type_by_mime_type(mime):
+    def get_content_type_by_mime_type(mime) -> DatapoolContentType:
         logger.info(f"{mime=}")
         parts = mime.split("/")
         if parts[0] == "image":
             return DatapoolContentType.Image
         if parts[0] == "video":
             return DatapoolContentType.Video
         if parts[0] == "audio":
             return DatapoolContentType.Audio
         if parts[0] == "text" or mime == "application/json":
             return DatapoolContentType.Text
 
         raise BasePluginException(f"not supported {mime=}")
 
+    @staticmethod
+    def get_content_type_by_content(content: Union[bytes, io.IOBase]) -> DatapoolContentType:
+        if isinstance(content, bytes):
+            buffer = content
+        elif isinstance(content, io.IOBase):
+            content.seek(0, 0)
+            buffer = content.read(512)  # TODO: enough?
+        mime = magic.from_buffer(buffer, mime=True)
+        if mime:
+            return BasePlugin.get_content_type_by_mime_type(mime)
+        raise BasePluginException(f"not supported content")
+
     @classmethod
-    def parse_image_tag(cls, content) -> Union[BaseTag, None]:
+    def parse_image_tag(cls, content: Union[bytes, io.IOBase]) -> Union[BaseTag, None]:
         # load image from bytes content, parse Copyright exif field for a license tag
         try:
-            image = Image.open(io.BytesIO(content))
+            if isinstance(content, bytes):
+                image = Image.open(io.BytesIO(content))
+            elif isinstance(content, io.IOBase):
+                image = Image.open(content)
             exifdata = image.getexif()
             cp = exifdata.get(ExifTagsList.Copyright)
             # logger.info( f'{cp=} {type(cp)=}')
 
             if type(cp) is str:
                 return cls.parse_tag_in_str(cp)
         except Exception as e:
@@ -352,7 +379,12 @@
     def make_text_storage_value(body, header=None, excerpt=None):
         data = (header + "\n" if header else "") + (excerpt + "\n" if excerpt else "") + body
         return data
 
     @staticmethod
     def gen_demo_tag(user_name):
         return "demo_" + md5(user_name.encode()).hexdigest()[-6:]
+
+
+class BaseReader:
+    @abstractmethod
+    def read_to(self, f: io.IOBase): ...
```

### Comparing `datapools-1.0.64/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/default/default.py` & `datapools-1.0.65/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.65/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import re
 from urllib.parse import urlparse, urlunparse
+from typing import Optional
+
 
 import requests
 from bs4 import BeautifulSoup, Comment
 from html2text import HTML2Text
 
 from ....common.logger import logger
 
@@ -14,16 +16,17 @@
 
 DOMAIN = "www.dw.com"
 
 
 class DeutscheWellePlugin(BasePlugin):
 
     base_url = f"https://{DOMAIN}/en/"
+    demo_tag: BaseTag
 
-    def __init__(self, ctx, demo_tag=None):
+    def __init__(self, ctx, demo_tag: Optional[str] = None):
         super().__init__(ctx)
         logger.info(f"{demo_tag=} ***************************************************")
         self.demo_tag = BaseTag(demo_tag)
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
```

### Comparing `datapools-1.0.64/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.65/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.65/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
                     async for msg in self.scan_folder(folder_id, drive):
                         yield msg
         except Exception as e:
             logger.error(f"GoogleDrivePlugin exception {e}")
             logger.error(traceback.format_exc())
 
     def _get_download_url(self, file_id):
-        # this url can be placed on site for preview
         return f"https://drive.google.com/uc?id={file_id}"
 
         # return f"https://www.googleapis.com/drive/v3/files/{file_id}?alt=media&key={self.creds.token}"
 
     async def find_license(self, folder_id, drive):
         try:
             files_res = (
@@ -178,64 +177,64 @@
                         yield yielded
                 else:
                     try:
                         datapool_content_type = BasePlugin.get_content_type_by_mime_type(item["mimeType"])
                     except BasePluginException:
                         logger.error(f'Not supported mime type {item["mimeType"]}')
 
-                    logger.info(f'downloading file {file_id} {item["name"]}')
+                    # logger.info(f'downloading file {file_id} {item["name"]}')
                     # TODO: this works too, but is getting blocked  when running from lsrv2
                     # fileRequest = drive.files().get_media(fileId=file_id)
                     # fh = io.BytesIO()
                     # downloader = MediaIoBaseDownload(fh, fileRequest)
                     # done = False
                     # while done is False:
                     #     status, done = downloader.next_chunk()
                     # fh.seek(0)
                     # content = fh.read()
                     # direct url seems to work better than API access
                     url = self._get_download_url(file_id)
-                    content = await self.download(url)
-                    if content is not None:
-                        logger.info(f"file size={len(content)}")
-
-                        author_tag = None
-                        if self.demo_mode:
-                            path = f"{parent_path}{item['name']}"
-                            logger.info(f"{path=}")
-
-                            # if file full path matches any structural rule,
-                            # then trying to create demo user from the match info
-                            match = self._match_structure_rules(path)
-                            if match and "user" in match:
-                                short_tag_id = BasePlugin.gen_demo_tag(match["user"])
-                                author_tag = BaseTag(short_tag_id)
-                                yield CrawlerDemoUser(
-                                    user_name=match["user"], short_tag_id=short_tag_id, platform="drive.google.com"
-                                )
-
-                        if not author_tag:
-                            if datapool_content_type == DatapoolContentType.Image:
-                                author_tag = BasePlugin.parse_image_tag(content)
-
-                        # obj_url = f'https://drive.google.com/file/d/{file_id}/view'
-                        obj_url = url
-                        # storage_id = self.ctx.storage.gen_id(obj_url)
-                        # await self.ctx.storage.put(storage_id, content)
-
-                        yield CrawlerContent(
-                            tag_id=str(author_tag) if author_tag is not None else None,
-                            tag_keepout=author_tag.is_keepout() if author_tag is not None else None,
-                            copyright_tag_id=str(self.tag_id),
-                            copyright_tag_keepout=self.tag_id.is_keepout(),
-                            type=datapool_content_type,
-                            # storage_id=storage_id,
-                            url=obj_url,
-                            content=content,
-                        )
+                    # content = await self.download(url)
+                    # if content is not None:
+                    #     logger.info(f"file size={len(content)}")
+
+                    author_tag = None
+                    if self.demo_mode:
+                        path = f"{parent_path}{item['name']}"
+                        logger.info(f"{path=}")
+
+                        # if file full path matches any structural rule,
+                        # then trying to create demo user from the match info
+                        match = self._match_structure_rules(path)
+                        if match and "user" in match:
+                            short_tag_id = BasePlugin.gen_demo_tag(match["user"])
+                            author_tag = BaseTag(short_tag_id)
+                            yield CrawlerDemoUser(
+                                user_name=match["user"], short_tag_id=short_tag_id, platform="drive.google.com"
+                            )
+
+                    # if not author_tag:
+                    #     if datapool_content_type == DatapoolContentType.Image:
+                    #         author_tag = BasePlugin.parse_image_tag(content)
+
+                    # obj_url = f'https://drive.google.com/file/d/{file_id}/view'
+                    obj_url = url
+                    # storage_id = self.ctx.storage.gen_id(obj_url)
+                    # await self.ctx.storage.put(storage_id, content)
+
+                    yield CrawlerContent(
+                        tag_id=str(author_tag) if author_tag is not None else None,
+                        tag_keepout=author_tag.is_keepout() if author_tag is not None else None,
+                        copyright_tag_id=str(self.tag_id),
+                        copyright_tag_keepout=self.tag_id.is_keepout(),
+                        type=datapool_content_type,
+                        # storage_id=storage_id,
+                        url=obj_url,
+                        # content=content,
+                    )
 
                 # baseImage = cv2.imdecode(np.fromstring(fhContents, dtype=np.uint8), cv2.IMREAD_COLOR)
             if page_token is None:
                 break
 
     def _match_structure_rules(self, path):
         # self.rules is [
```

### Comparing `datapools-1.0.64/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.65/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.65/datapools/worker/plugins/s3/s3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import os
+import io
 import tempfile
 import traceback
 
 import boto3
 import filetype
 from botocore import UNSIGNED
 from botocore.client import Config
 from botocore.exceptions import ClientError
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 
 # from ....common.types import CrawlerNop  # CrawlerBackTask,
 from ....common.types import CrawlerContent, DatapoolContentType
-from ..base_plugin import BasePlugin, BasePluginException
+from ..base_plugin import BasePlugin, BasePluginException, BaseReader
 from ...worker import WorkerTask
 
 
+class S3Reader(BaseReader):
+
+    def __init__(self, s3_client, bucket_name, key):
+        self.s3_client = s3_client
+        self.bucket_name = bucket_name
+        self.key = key
+
+    def read_to(self, f: io.IOBase):
+        self.s3_client.download_fileobj(self.bucket_name, self.key, f)
+
+
 class S3Exception(BasePluginException):
     pass
 
 
 class S3Plugin(BasePlugin):
     def __init__(self, ctx, aws_access_key_id=None, aws_secret_access_key=None):
         super().__init__(ctx)
@@ -101,46 +113,48 @@
             else:
                 # THIS IS DIRECT URL ( FOR PUBLIC BUCKETS )
                 # TODO: region?
                 obj_url = f"https://{self.bucket_name}.s3.amazonaws.com/{obj.key}"
 
             # storage_id = self.ctx.storage.gen_id(obj_url)
 
-            content = self._download(obj.key)
+            # content = self._download(obj.key)
 
             try:
-                content_type = self._get_datapool_content_type(content)
+                # content_type = self._get_datapool_content_type(content)
+                # content_type = BasePlugin.get_content_type_by_content(content)
 
-                tag = None
-                if content_type == DatapoolContentType.Image:
-                    tag = BasePlugin.parse_image_tag(content)
+                # tag = None
+                # if content_type == DatapoolContentType.Image:
+                #     tag = BasePlugin.parse_image_tag(content)
 
-                if tag is None and copyright_tag is None:
-                    continue
+                # if tag is None and copyright_tag is None:
+                #     continue
 
                 # await self.ctx.storage.put(storage_id, content)
 
                 yield CrawlerContent(
-                    tag_id=str(tag) if tag is not None else None,
-                    tag_keepout=tag.is_keepout() if tag is not None else False,
+                    # tag_id=str(tag) if tag is not None else None,
+                    # tag_keepout=tag.is_keepout() if tag is not None else False,
                     copyright_tag_id=str(copyright_tag) if copyright_tag is not None else None,
                     copyright_tag_keepout=copyright_tag.is_keepout() if copyright_tag is not None else False,
-                    type=content_type,
+                    # type=content_type,
                     # storage_id=storage_id,
                     url=obj_url,
-                    content=content,
+                    # content=content,
+                    content=S3Reader(self.s3_client, self.bucket_name, obj.key),
                 )
             except S3Exception as e:
                 logger.info(f"mime type not supported/detected: {e}")
 
     def _download(self, key):
         with tempfile.NamedTemporaryFile() as tmp:
             self.s3_client.download_fileobj(self.bucket_name, key, tmp)
 
             tmp.seek(0, 0)
             return tmp.read()
 
-    def _get_datapool_content_type(self, content):
-        type = filetype.guess(content)
-        if type is None:
-            raise S3Exception("unknown file type")
-        return BasePlugin.get_content_type_by_mime_type(type.mime)
+    # def _get_datapool_content_type(self, content):
+    #     type = filetype.guess(content)
+    #     if type is None:
+    #         raise S3Exception("unknown file type")
+    #     return BasePlugin.get_content_type_by_mime_type(type.mime)
```

### Comparing `datapools-1.0.64/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.65/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.65/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.65/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.65/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/datapools/worker/worker.py` & `datapools-1.0.65/datapools/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import importlib
+import tempfile
 import inspect
 import os
 import re
 import sys
 
 import traceback
 import uuid
@@ -23,15 +24,15 @@
     CrawlerHintURLStatus,
     CrawlerNop,
     DatapoolContentType,
     InvalidUsageException,
     WorkerSettings,
 )
 from .types import WorkerContext, WorkerTask
-from .plugins.base_plugin import BasePlugin
+from .plugins.base_plugin import BasePlugin, BaseReader
 from .utils import get_storage_invalidation_topic
 
 
 class WorkerFileStorage(FileStorage):
     def __init__(self, dstpath, worker_id):
         super().__init__(os.path.join(dstpath, worker_id))
 
@@ -319,69 +320,96 @@
         )
 
     async def _process_crawled_content(
         self, cc: CrawlerContent, session: Session, plugin: BasePlugin, task: WorkerTask
     ):
         no_tagged_content = True
         if not await session.has_content(cc.url):
-            if not cc.content:
-                logger.info("no content, downloading")
-                cc.content = await plugin.download(cc.url)
 
-            if cc.content:
-                if not cc.tag_id:
-                    # trying to parse author tag
-                    if cc.type == DatapoolContentType.Image:
-                        image_tag = BasePlugin.parse_image_tag(cc.content)
-                        cc.tag_id = str(image_tag) if image_tag is not None else None
-                        cc.tag_keepout = image_tag.is_keepout() if image_tag is not None else False
-                    # TODO: add video/audio parsing here
-
-                if cc.tag_id is not None or cc.copyright_tag_id is not None or cc.platform_tag_id is not None:
-                    no_tagged_content = False
-
-                    storage_id = self.storage.gen_id(cc.url)
-                    logger.info(f"putting to {storage_id=}")
-                    await self.storage.put(storage_id, cc.content)
-
-                    await session.add_content(cc.url)
-                    await session.inc_crawled_content()
-
-                    if cc.tag_id is not None:
-                        await session.inc_tag_usage(cc.tag_id, cc.tag_keepout)
-                    if cc.copyright_tag_id is not None:
-                        await session.inc_tag_usage(cc.copyright_tag_id, cc.copyright_tag_keepout)
-                    if cc.platform_tag_id is not None:
-                        await session.inc_tag_usage(cc.platform_tag_id, cc.platform_tag_keepout)
-
-                    # notifying producer about new crawled data
-                    await self.producer_queue.push(
-                        QueueMessage(
-                            session.id,
-                            QueueMessageType.Task,
-                            {
-                                "parent_url": task.url,
-                                "url": cc.url,
-                                "storage_id": storage_id,
-                                "tag_id": cc.tag_id,
-                                "tag_keepout": cc.tag_keepout,
-                                "copyright_tag_id": cc.copyright_tag_id,
-                                "copyright_tag_keepout": cc.copyright_tag_keepout,
-                                "platform_tag_id": cc.platform_tag_id,
-                                "platform_tag_keepout": cc.platform_tag_keepout,
-                                "type": DatapoolContentType(cc.type).value,
-                                "priority_timestamp": cc.priority_timestamp,
-                                "worker_id": self.id,
-                            },
-                        )
-                    )
+            async def process_content():
+                nonlocal no_tagged_content
+                logger.info(f"process_content {type(cc.content)=}")
+                if cc.content:
+                    if not cc.type:
+                        cc.type = BasePlugin.get_content_type_by_content(cc.content)
+
+                    logger.info(f"{cc.type=}")
+
+                    if cc.type:
+                        if not cc.tag_id:
+                            # trying to parse author tag
+                            if cc.type == DatapoolContentType.Image:
+                                image_tag = BasePlugin.parse_image_tag(cc.content)
+                                cc.tag_id = str(image_tag) if image_tag is not None else None
+                                cc.tag_keepout = image_tag.is_keepout() if image_tag is not None else False
+                            # TODO: add video/audio parsing here
+
+                        if cc.tag_id is not None or cc.copyright_tag_id is not None or cc.platform_tag_id is not None:
+                            no_tagged_content = False
+
+                            storage_id = self.storage.gen_id(cc.url)
+                            logger.info(f"putting to {storage_id=}")
+                            await self.storage.put(storage_id, cc.content)
+
+                            await session.add_content(cc.url)
+                            await session.inc_crawled_content()
+
+                            if cc.tag_id is not None:
+                                await session.inc_tag_usage(cc.tag_id, cc.tag_keepout)
+                            if cc.copyright_tag_id is not None:
+                                await session.inc_tag_usage(cc.copyright_tag_id, cc.copyright_tag_keepout)
+                            if cc.platform_tag_id is not None:
+                                await session.inc_tag_usage(cc.platform_tag_id, cc.platform_tag_keepout)
+
+                            # notifying producer about new crawled data
+                            await self.producer_queue.push(
+                                QueueMessage(
+                                    session.id,
+                                    QueueMessageType.Task,
+                                    {
+                                        "parent_url": task.url,
+                                        "url": cc.url,
+                                        "storage_id": storage_id,
+                                        "tag_id": cc.tag_id,
+                                        "tag_keepout": cc.tag_keepout,
+                                        "copyright_tag_id": cc.copyright_tag_id,
+                                        "copyright_tag_keepout": cc.copyright_tag_keepout,
+                                        "platform_tag_id": cc.platform_tag_id,
+                                        "platform_tag_keepout": cc.platform_tag_keepout,
+                                        "type": DatapoolContentType(cc.type).value,
+                                        "priority_timestamp": cc.priority_timestamp,
+                                        "worker_id": self.id,
+                                    },
+                                )
+                            )
+                        else:
+                            logger.info("no tag available")
+                    else:
+                        logger.info("unknown content type")
                 else:
-                    logger.info("no tag available")
+                    logger.info("no content")
+
+            if not cc.content:
+                logger.info("no content, downloading from url")
+                with tempfile.TemporaryFile("wb") as tmp:
+                    async for chunk in plugin.async_read_url(cc.url):
+                        tmp.write(chunk)
+                    cc.content = tmp
+                    await process_content()
+            elif isinstance(cc.content, BaseReader):
+                logger.info("content is BaseReader instance")
+                with tempfile.TemporaryFile("wb") as tmp:
+                    cc.content.read_to(tmp)
+                    cc.content = tmp
+                    await process_content()
             else:
-                logger.info("no content")
+                await process_content()
+
+        else:
+            logger.info(f"content url exists {cc.url}")
 
         # Stats for scheduler decision whether to continue crawling or not
         if no_tagged_content:
             logger.info("inc_since_last_tagged")
             await session.inc_since_last_tagged()
         else:
             logger.info("reset_since_last_tagged")
```

### Comparing `datapools-1.0.64/datapools.egg-info/PKG-INFO` & `datapools-1.0.65/datapools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.64
+Version: 1.0.65
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
@@ -22,14 +22,15 @@
 Requires-Dist: azure-identity
 Requires-Dist: msgraph-sdk
 Requires-Dist: aio-pika
 Requires-Dist: dnspython
 Requires-Dist: pillow
 Requires-Dist: pytest-playwright
 Requires-Dist: bs4
+Requires-Dist: python-magic
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `datapools-1.0.64/datapools.egg-info/SOURCES.txt` & `datapools-1.0.65/datapools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
 datapools/worker/plugins/default/__init__.py
 datapools/worker/plugins/default/default.py
 datapools/worker/plugins/deutsche_welle/__init__.py
 datapools/worker/plugins/deutsche_welle/deutsche_welle.py
 datapools/worker/plugins/freesound_org/__init__.py
 datapools/worker/plugins/freesound_org/freesound_org.py
+datapools/worker/plugins/ftp/__init__.py
+datapools/worker/plugins/ftp/ftp.py
+datapools/worker/plugins/ftp/ftp_dir_listing.py
 datapools/worker/plugins/google_drive/__init__.py
 datapools/worker/plugins/google_drive/google_drive.py
 datapools/worker/plugins/imageshack/__init__.py
 datapools/worker/plugins/imageshack/imageshack.py
 datapools/worker/plugins/s3/__init__.py
 datapools/worker/plugins/s3/s3.py
 datapools/worker/plugins/theguardian/__init__.py
```

### Comparing `datapools-1.0.64/setup.py` & `datapools-1.0.65/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/tests/test_base.py` & `datapools-1.0.65/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.64/tests/test_session_manager.py` & `datapools-1.0.65/tests/test_session_manager.py`

 * *Files identical despite different names*

