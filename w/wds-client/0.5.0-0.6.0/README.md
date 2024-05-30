# Comparing `tmp/wds_client-0.5.0.tar.gz` & `tmp/wds_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wds_client-0.5.0.tar", last modified: Mon May 20 14:27:27 2024, max compression
+gzip compressed data, was "wds_client-0.6.0.tar", last modified: Thu May 30 19:48:20 2024, max compression
```

## Comparing `wds_client-0.5.0.tar` & `wds_client-0.6.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:27.238600 wds_client-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 14:27:27.238600 wds_client-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-20 14:26:05.000000 wds_client-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 14:27:27.238600 wds_client-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-20 14:26:05.000000 wds_client-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:27.226601 wds_client-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_attribute_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_attribute_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_backup_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_backup_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_batch_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-20 14:26:04.000000 wds_client-0.5.0/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_capabilities_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_clone_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_clone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_generic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_generic_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_import_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_instances_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_job_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_job_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_record_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-20 14:26:05.000000 wds_client-0.5.0/test/test_version_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:27.226601 wds_client-0.5.0/wds_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:27.230600 wds_client-0.5.0/wds_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/capabilities_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/cloning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/general_wds_information_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/instances_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/job_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    61562 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/records_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    34758 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26209 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:27.238600 wds_client-0.5.0/wds_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/attribute_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/attribute_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/attribute_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/backup_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/backup_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/backup_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/backup_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/batch_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/batch_record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/batch_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-20 14:26:04.000000 wds_client-0.5.0/wds_client/models/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/clone_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/clone_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/clone_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/generic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/generic_job_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/import_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/job_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/record_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/record_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/record_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/record_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/search_sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/tsv_upload_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/models/version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-20 14:26:05.000000 wds_client-0.5.0/wds_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:27.238600 wds_client-0.5.0/wds_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 14:27:27.000000 wds_client-0.5.0/wds_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-20 14:27:27.000000 wds_client-0.5.0/wds_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:27:27.000000 wds_client-0.5.0/wds_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 14:27:27.000000 wds_client-0.5.0/wds_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 14:27:27.000000 wds_client-0.5.0/wds_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:20.610327 wds_client-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 19:48:20.610327 wds_client-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-30 19:46:24.000000 wds_client-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 19:48:20.610327 wds_client-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-30 19:46:24.000000 wds_client-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:20.602327 wds_client-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_attribute_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_attribute_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_capabilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_generic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_generic_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_import_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_job_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-30 19:46:24.000000 wds_client-0.6.0/test/test_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:20.602327 wds_client-0.6.0/wds_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:20.606327 wds_client-0.6.0/wds_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/capabilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/cloning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/general_wds_information_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17329 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/instances_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/job_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61562 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/records_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34758 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26209 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:20.610327 wds_client-0.6.0/wds_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/attribute_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/attribute_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/attribute_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/backup_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/backup_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/backup_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/batch_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/batch_record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/batch_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/clone_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/clone_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/clone_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/generic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/generic_job_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/import_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/job_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/record_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/record_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/record_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/record_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/search_sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/tsv_upload_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/models/version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-05-30 19:46:24.000000 wds_client-0.6.0/wds_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:48:20.610327 wds_client-0.6.0/wds_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 19:48:20.000000 wds_client-0.6.0/wds_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-30 19:48:20.000000 wds_client-0.6.0/wds_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:48:20.000000 wds_client-0.6.0/wds_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 19:48:20.000000 wds_client-0.6.0/wds_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 19:48:20.000000 wds_client-0.6.0/wds_client.egg-info/top_level.txt
```

### Comparing `wds_client-0.5.0/README.md` & `wds_client-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This page lists current APIs.
 As of v0.2, all APIs are subject to change without notice.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v0.2
-- Package version: 0.5.0
+- Package version: 0.6.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `wds_client-0.5.0/setup.py` & `wds_client-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "wds-client"
-VERSION = "0.5.0"
+VERSION = "0.6.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `wds_client-0.5.0/test/test_app.py` & `wds_client-0.6.0/test/test_app.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_attribute_data_type.py` & `wds_client-0.6.0/test/test_attribute_data_type.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_attribute_schema.py` & `wds_client-0.6.0/test/test_attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_attribute_schema_update.py` & `wds_client-0.6.0/test/test_attribute_schema_update.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_backup_job.py` & `wds_client-0.6.0/test/test_backup_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_backup_job_all_of.py` & `wds_client-0.6.0/test/test_backup_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_backup_response.py` & `wds_client-0.6.0/test/test_backup_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_backup_restore_request.py` & `wds_client-0.6.0/test/test_backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_batch_operation.py` & `wds_client-0.6.0/test/test_batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_batch_record_request.py` & `wds_client-0.6.0/test/test_batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_batch_response.py` & `wds_client-0.6.0/test/test_batch_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_build.py` & `wds_client-0.6.0/test/test_build.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_capabilities.py` & `wds_client-0.6.0/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_capabilities_api.py` & `wds_client-0.6.0/test/test_capabilities_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_clone_job.py` & `wds_client-0.6.0/test/test_clone_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_clone_job_all_of.py` & `wds_client-0.6.0/test/test_clone_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_clone_response.py` & `wds_client-0.6.0/test/test_clone_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_cloning_api.py` & `wds_client-0.6.0/test/test_cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_commit.py` & `wds_client-0.6.0/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_error_response.py` & `wds_client-0.6.0/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_general_wds_information_api.py` & `wds_client-0.6.0/test/test_general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_generic_job.py` & `wds_client-0.6.0/test/test_generic_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_generic_job_all_of.py` & `wds_client-0.6.0/test/test_generic_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_git.py` & `wds_client-0.6.0/test/test_git.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_import_api.py` & `wds_client-0.6.0/test/test_import_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_import_request.py` & `wds_client-0.6.0/test/test_import_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_inline_object.py` & `wds_client-0.6.0/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_instances_api.py` & `wds_client-0.6.0/test/test_instances_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_job.py` & `wds_client-0.6.0/test/test_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_job_api.py` & `wds_client-0.6.0/test/test_job_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_job_v1.py` & `wds_client-0.6.0/test/test_job_v1.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_record_query_response.py` & `wds_client-0.6.0/test/test_record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_record_request.py` & `wds_client-0.6.0/test/test_record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_record_response.py` & `wds_client-0.6.0/test/test_record_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_record_type_schema.py` & `wds_client-0.6.0/test/test_record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_records_api.py` & `wds_client-0.6.0/test/test_records_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_schema_api.py` & `wds_client-0.6.0/test/test_schema_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_search_filter.py` & `wds_client-0.6.0/test/test_search_filter.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_search_request.py` & `wds_client-0.6.0/test/test_search_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_search_sort_direction.py` & `wds_client-0.6.0/test/test_search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_status_response.py` & `wds_client-0.6.0/test/test_status_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_tsv_upload_response.py` & `wds_client-0.6.0/test/test_tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/test/test_version_response.py` & `wds_client-0.6.0/test/test_version_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/__init__.py` & `wds_client-0.6.0/wds_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v0.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 # import apis into sdk package
 from wds_client.api.capabilities_api import CapabilitiesApi
 from wds_client.api.cloning_api import CloningApi
 from wds_client.api.general_wds_information_api import GeneralWDSInformationApi
 from wds_client.api.import_api import ImportApi
 from wds_client.api.instances_api import InstancesApi
```

### Comparing `wds_client-0.5.0/wds_client/api/__init__.py` & `wds_client-0.6.0/wds_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/capabilities_api.py` & `wds_client-0.6.0/wds_client/api/capabilities_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/cloning_api.py` & `wds_client-0.6.0/wds_client/api/cloning_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/general_wds_information_api.py` & `wds_client-0.6.0/wds_client/api/general_wds_information_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/import_api.py` & `wds_client-0.6.0/wds_client/api/import_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/instances_api.py` & `wds_client-0.6.0/wds_client/api/instances_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/job_api.py` & `wds_client-0.6.0/wds_client/api/job_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/records_api.py` & `wds_client-0.6.0/wds_client/api/records_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api/schema_api.py` & `wds_client-0.6.0/wds_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/api_client.py` & `wds_client-0.6.0/wds_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'wds-client/0.5.0/python'
+        self.user_agent = 'wds-client/0.6.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `wds_client-0.5.0/wds_client/configuration.py` & `wds_client-0.6.0/wds_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v0.2\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.6.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `wds_client-0.5.0/wds_client/exceptions.py` & `wds_client-0.6.0/wds_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/__init__.py` & `wds_client-0.6.0/wds_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/app.py` & `wds_client-0.6.0/wds_client/models/app.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/attribute_data_type.py` & `wds_client-0.6.0/wds_client/models/attribute_data_type.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/attribute_schema.py` & `wds_client-0.6.0/wds_client/models/attribute_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/attribute_schema_update.py` & `wds_client-0.6.0/wds_client/models/attribute_schema_update.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/backup_job.py` & `wds_client-0.6.0/wds_client/models/backup_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/backup_job_all_of.py` & `wds_client-0.6.0/wds_client/models/backup_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/backup_response.py` & `wds_client-0.6.0/wds_client/models/backup_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/backup_restore_request.py` & `wds_client-0.6.0/wds_client/models/backup_restore_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/batch_operation.py` & `wds_client-0.6.0/wds_client/models/batch_operation.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/batch_record_request.py` & `wds_client-0.6.0/wds_client/models/batch_record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/batch_response.py` & `wds_client-0.6.0/wds_client/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/build.py` & `wds_client-0.6.0/wds_client/models/build.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/capabilities.py` & `wds_client-0.6.0/wds_client/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/clone_job.py` & `wds_client-0.6.0/wds_client/models/clone_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/clone_job_all_of.py` & `wds_client-0.6.0/wds_client/models/clone_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/clone_response.py` & `wds_client-0.6.0/wds_client/models/clone_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/commit.py` & `wds_client-0.6.0/wds_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/error_response.py` & `wds_client-0.6.0/wds_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/generic_job.py` & `wds_client-0.6.0/wds_client/models/generic_job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/generic_job_all_of.py` & `wds_client-0.6.0/wds_client/models/generic_job_all_of.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/git.py` & `wds_client-0.6.0/wds_client/models/git.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/import_request.py` & `wds_client-0.6.0/wds_client/models/import_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/inline_object.py` & `wds_client-0.6.0/wds_client/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/job.py` & `wds_client-0.6.0/wds_client/models/job.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/job_v1.py` & `wds_client-0.6.0/wds_client/models/job_v1.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/record_query_response.py` & `wds_client-0.6.0/wds_client/models/record_query_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/record_request.py` & `wds_client-0.6.0/wds_client/models/record_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/record_response.py` & `wds_client-0.6.0/wds_client/models/record_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/record_type_schema.py` & `wds_client-0.6.0/wds_client/models/record_type_schema.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/search_filter.py` & `wds_client-0.6.0/wds_client/models/search_filter.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/search_request.py` & `wds_client-0.6.0/wds_client/models/search_request.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/search_sort_direction.py` & `wds_client-0.6.0/wds_client/models/search_sort_direction.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/status_response.py` & `wds_client-0.6.0/wds_client/models/status_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/tsv_upload_response.py` & `wds_client-0.6.0/wds_client/models/tsv_upload_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/models/version_response.py` & `wds_client-0.6.0/wds_client/models/version_response.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client/rest.py` & `wds_client-0.6.0/wds_client/rest.py`

 * *Files identical despite different names*

### Comparing `wds_client-0.5.0/wds_client.egg-info/SOURCES.txt` & `wds_client-0.6.0/wds_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

