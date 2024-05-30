# Comparing `tmp/monday_code-0.0.5.tar.gz` & `tmp/monday_code-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monday_code-0.0.5.tar", last modified: Sun Apr 28 06:08:16 2024, max compression
+gzip compressed data, was "monday_code-0.0.6.tar", last modified: Thu May 30 07:50:38 2024, max compression
```

## Comparing `monday_code-0.0.5.tar` & `monday_code-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.777480 monday_code-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-28 06:08:10.000000 monday_code-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-28 06:08:16.777480 monday_code-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-28 06:08:10.000000 monday_code-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-28 06:08:10.000000 monday_code-0.0.5/README_FOR_PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.769481 monday_code-0.0.5/monday_code/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.773481 monday_code-0.0.5/monday_code/api/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10463 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/secret_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30735 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/secure_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    45643 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api/storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25779 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.773481 monday_code-0.0.5/monday_code/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/get_by_key_from_storage404_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/get_by_key_from_storage500_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/increment_counter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/json_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/period.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/publish_message_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/publish_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/secure_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/validate_secret_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/models/validate_secret_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-04-28 06:08:10.000000 monday_code-0.0.5/monday_code/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.777480 monday_code-0.0.5/monday_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-28 06:08:16.000000 monday_code-0.0.5/monday_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-28 06:08:10.000000 monday_code-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-28 06:08:16.777480 monday_code-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-28 06:08:10.000000 monday_code-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 06:08:16.777480 monday_code-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_get_by_key_from_storage404_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_get_by_key_from_storage500_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_increment_counter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_json_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_period.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_publish_message_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_publish_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_queue_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_secret_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_secure_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_secure_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_storage_data_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_validate_secret_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-28 06:08:10.000000 monday_code-0.0.5/test/test_validate_secret_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:38.048124 monday_code-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 07:50:33.000000 monday_code-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-30 07:50:38.048124 monday_code-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-30 07:50:33.000000 monday_code-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-30 07:50:33.000000 monday_code-0.0.6/README_FOR_PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:38.040125 monday_code-0.0.6/monday_code/
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:38.040125 monday_code-0.0.6/monday_code/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19808 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api/environment_variables_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api/logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21897 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19405 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api/secrets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api/secure_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45706 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api/storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25779 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:38.044124 monday_code-0.0.6/monday_code/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/get_by_key_from_storage404_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/get_by_key_from_storage500_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/increment_counter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/json_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/log_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/publish_message_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/publish_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/secure_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/validate_secret_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/validate_secret_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/write_log_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/models/write_log_request_body_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-05-30 07:50:33.000000 monday_code-0.0.6/monday_code/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:38.048124 monday_code-0.0.6/monday_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-30 07:50:38.000000 monday_code-0.0.6/monday_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-30 07:50:38.000000 monday_code-0.0.6/monday_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:50:38.000000 monday_code-0.0.6/monday_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 07:50:38.000000 monday_code-0.0.6/monday_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 07:50:38.000000 monday_code-0.0.6/monday_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-30 07:50:33.000000 monday_code-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 07:50:38.048124 monday_code-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-30 07:50:33.000000 monday_code-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:50:38.048124 monday_code-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_environment_variables_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_get_by_key_from_storage404_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_get_by_key_from_storage500_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_increment_counter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_json_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_log_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_publish_message_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_publish_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_secrets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_secure_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_secure_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_storage_data_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_validate_secret_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_validate_secret_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_write_log_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-30 07:50:33.000000 monday_code-0.0.6/test/test_write_log_request_body_error.py
```

### Comparing `monday_code-0.0.5/PKG-INFO` & `monday_code-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monday-code
-Version: 0.0.5
+Version: 0.0.6
 Summary: mcode-sdk-api
 Home-page: 
 Author: Monday.Com
 Author-email: support@monday.com
 License: MIT
 Keywords: monday-code
 Description-Content-Type: text/markdown
```

### Comparing `monday_code-0.0.5/README.md` & `monday_code-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,13 @@
 # monday-code
-No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
-
-This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
-
-- API version: 0.0.1
-- Package version: 0.0.1
-- Build package: org.openapitools.codegen.languages.PythonClientCodegen
-
-## Requirements.
-
-Python 3.7+
 
 ## Installation & Usage
-### pip install
-
-If the python package is hosted on a repository, you can install directly using:
-
-```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
-```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
-
-Then import the package:
-```python
-import monday_code
-```
-
-### Setuptools
-
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
-
 ```sh
-python setup.py install --user
+pip install monday-code
 ```
-(or `sudo python setup.py install` to install the package for all users)
-
-Then import the package:
-```python
-import monday_code
-```
-
-### Tests
-
-Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
@@ -61,63 +22,58 @@
 )
 
 
 
 # Enter a context with an instance of the API client
 with monday_code.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = monday_code.QueueApi(api_client)
-    publish_message_params = monday_code.PublishMessageParams() # PublishMessageParams | 
+    api_instance = monday_code.EnvironmentVariablesApi(api_client)
+    name = 'name_example' # str | 
 
     try:
-        api_response = api_instance.publish_message(publish_message_params)
-        print("The response of QueueApi->publish_message:\n")
+        api_response = api_instance.get_environment_variable(name)
+        print("The response of EnvironmentVariablesApi->get_environment_variable:\n")
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling QueueApi->publish_message: %s\n" % e)
+        print("Exception when calling EnvironmentVariablesApi->get_environment_variable: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost:59999*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*EnvironmentVariablesApi* | [**get_environment_variable**](docs/EnvironmentVariablesApi.md#get_environment_variable) | **GET** /environment-variables/{name} | 
+*EnvironmentVariablesApi* | [**get_environment_variable_keys**](docs/EnvironmentVariablesApi.md#get_environment_variable_keys) | **GET** /environment-variables | 
+*LogsApi* | [**write_log**](docs/LogsApi.md#write_log) | **POST** /logs | 
 *QueueApi* | [**publish_message**](docs/QueueApi.md#publish_message) | **POST** /queue | 
 *QueueApi* | [**validate_secret**](docs/QueueApi.md#validate_secret) | **POST** /queue/validate-secret | 
-*SecretApi* | [**get_secret**](docs/SecretApi.md#get_secret) | **GET** /secrets/{name} | 
+*SecretsApi* | [**get_secret**](docs/SecretsApi.md#get_secret) | **GET** /secrets/{name} | 
+*SecretsApi* | [**get_secret_keys**](docs/SecretsApi.md#get_secret_keys) | **GET** /secrets | 
 *SecureStorageApi* | [**delete_secure_storage**](docs/SecureStorageApi.md#delete_secure_storage) | **DELETE** /secure-storage/{key} | 
 *SecureStorageApi* | [**get_secure_storage**](docs/SecureStorageApi.md#get_secure_storage) | **GET** /secure-storage/{key} | 
 *SecureStorageApi* | [**put_secure_storage**](docs/SecureStorageApi.md#put_secure_storage) | **PUT** /secure-storage/{key} | 
 *StorageApi* | [**delete_by_key_from_storage**](docs/StorageApi.md#delete_by_key_from_storage) | **DELETE** /storage/{key} | 
 *StorageApi* | [**get_by_key_from_storage**](docs/StorageApi.md#get_by_key_from_storage) | **GET** /storage/{key} | 
-*StorageApi* | [**increment_counter**](docs/StorageApi.md#increment_counter) | **POST** /storage/counter/increment | 
+*StorageApi* | [**increment_counter**](docs/StorageApi.md#increment_counter) | **PUT** /storage/counter/increment | 
 *StorageApi* | [**upsert_by_key_from_storage**](docs/StorageApi.md#upsert_by_key_from_storage) | **PUT** /storage/{key} | 
 
 
 ## Documentation For Models
 
  - [GetByKeyFromStorage404Response](docs/GetByKeyFromStorage404Response.md)
  - [GetByKeyFromStorage500Response](docs/GetByKeyFromStorage500Response.md)
  - [IncrementCounterParams](docs/IncrementCounterParams.md)
  - [JsonValue](docs/JsonValue.md)
+ - [LogMethods](docs/LogMethods.md)
  - [Period](docs/Period.md)
  - [PublishMessageParams](docs/PublishMessageParams.md)
  - [PublishMessageResponse](docs/PublishMessageResponse.md)
  - [SecureStorageDataContract](docs/SecureStorageDataContract.md)
  - [StorageDataContract](docs/StorageDataContract.md)
  - [ValidateSecretParams](docs/ValidateSecretParams.md)
  - [ValidateSecretResponse](docs/ValidateSecretResponse.md)
-
-
-<a id="documentation-for-authorization"></a>
-## Documentation For Authorization
-
-Endpoints do not require authorization.
-
-
-## Author
-
-
-
+ - [WriteLogRequestBody](docs/WriteLogRequestBody.md)
+ - [WriteLogRequestBodyError](docs/WriteLogRequestBodyError.md)
```

### Comparing `monday_code-0.0.5/README_FOR_PYPI.md` & `monday_code-0.0.6/README_FOR_PYPI.md`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code/__init__.py` & `monday_code-0.0.6/monday_code/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,18 @@
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "0.0.1"
 
 # import apis into sdk package
+from monday_code.api.environment_variables_api import EnvironmentVariablesApi
+from monday_code.api.logs_api import LogsApi
 from monday_code.api.queue_api import QueueApi
-from monday_code.api.secret_api import SecretApi
+from monday_code.api.secrets_api import SecretsApi
 from monday_code.api.secure_storage_api import SecureStorageApi
 from monday_code.api.storage_api import StorageApi
 
 # import ApiClient
 from monday_code.api_response import ApiResponse
 from monday_code.api_client import ApiClient
 from monday_code.configuration import Configuration
@@ -34,14 +36,17 @@
 from monday_code.exceptions import ApiException
 
 # import models into sdk package
 from monday_code.models.get_by_key_from_storage404_response import GetByKeyFromStorage404Response
 from monday_code.models.get_by_key_from_storage500_response import GetByKeyFromStorage500Response
 from monday_code.models.increment_counter_params import IncrementCounterParams
 from monday_code.models.json_value import JsonValue
+from monday_code.models.log_methods import LogMethods
 from monday_code.models.period import Period
 from monday_code.models.publish_message_params import PublishMessageParams
 from monday_code.models.publish_message_response import PublishMessageResponse
 from monday_code.models.secure_storage_data_contract import SecureStorageDataContract
 from monday_code.models.storage_data_contract import StorageDataContract
 from monday_code.models.validate_secret_params import ValidateSecretParams
 from monday_code.models.validate_secret_response import ValidateSecretResponse
+from monday_code.models.write_log_request_body import WriteLogRequestBody
+from monday_code.models.write_log_request_body_error import WriteLogRequestBodyError
```

### Comparing `monday_code-0.0.5/monday_code/api/queue_api.py` & `monday_code-0.0.6/monday_code/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code/api/secret_api.py` & `monday_code-0.0.6/monday_code/api/logs_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,56 +12,56 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
+from monday_code.models.write_log_request_body import WriteLogRequestBody
 
 from monday_code.api_client import ApiClient, RequestSerialized
 from monday_code.api_response import ApiResponse
 from monday_code.rest import RESTResponseType
 
 
-class SecretApi:
+class LogsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def get_secret(
+    def write_log(
         self,
-        name: StrictStr,
+        write_log_request_body: WriteLogRequestBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> str:
-        """get_secret
+    ) -> None:
+        """write_log
 
 
-        :param name: (required)
-        :type name: str
+        :param write_log_request_body: (required)
+        :type write_log_request_body: WriteLogRequestBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -76,59 +76,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_secret_serialize(
-            name=name,
+        _param = self._write_log_serialize(
+            write_log_request_body=write_log_request_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "str",
-            '404': "GetByKeyFromStorage404Response",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_secret_with_http_info(
+    def write_log_with_http_info(
         self,
-        name: StrictStr,
+        write_log_request_body: WriteLogRequestBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[str]:
-        """get_secret
+    ) -> ApiResponse[None]:
+        """write_log
 
 
-        :param name: (required)
-        :type name: str
+        :param write_log_request_body: (required)
+        :type write_log_request_body: WriteLogRequestBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -143,59 +142,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_secret_serialize(
-            name=name,
+        _param = self._write_log_serialize(
+            write_log_request_body=write_log_request_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "str",
-            '404': "GetByKeyFromStorage404Response",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_secret_without_preload_content(
+    def write_log_without_preload_content(
         self,
-        name: StrictStr,
+        write_log_request_body: WriteLogRequestBody,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """get_secret
+        """write_log
 
 
-        :param name: (required)
-        :type name: str
+        :param write_log_request_body: (required)
+        :type write_log_request_body: WriteLogRequestBody
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -210,36 +208,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_secret_serialize(
-            name=name,
+        _param = self._write_log_serialize(
+            write_log_request_body=write_log_request_body,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "str",
-            '404': "GetByKeyFromStorage404Response",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_secret_serialize(
+    def _write_log_serialize(
         self,
-        name,
+        write_log_request_body,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -251,37 +248,44 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if name is not None:
-            _path_params['name'] = name
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if write_log_request_body is not None:
+            _body_params = write_log_request_body
 
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/secrets/{name}',
+            method='POST',
+            resource_path='/logs',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `monday_code-0.0.5/monday_code/api/secure_storage_api.py` & `monday_code-0.0.6/monday_code/api/secure_storage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import StrictStr
-from typing import Any
 from monday_code.models.secure_storage_data_contract import SecureStorageDataContract
 
 from monday_code.api_client import ApiClient, RequestSerialized
 from monday_code.api_response import ApiResponse
 from monday_code.rest import RESTResponseType
 
 
@@ -246,15 +245,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
+        _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if key is not None:
             _path_params['key'] = key
         # process the query parameters
         # process the header parameters
@@ -497,15 +496,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
+        _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if key is not None:
             _path_params['key'] = key
         # process the query parameters
         # process the header parameters
@@ -764,15 +763,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, Union[str, bytes]] = {}
+        _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if key is not None:
             _path_params['key'] = key
         # process the query parameters
         # process the header parameters
```

### Comparing `monday_code-0.0.5/monday_code/api/storage_api.py` & `monday_code-0.0.6/monday_code/api/storage_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictStr
+from typing import Optional
 from monday_code.models.increment_counter_params import IncrementCounterParams
 from monday_code.models.storage_data_contract import StorageDataContract
 
 from monday_code.api_client import ApiClient, RequestSerialized
 from monday_code.api_response import ApiResponse
 from monday_code.rest import RESTResponseType
 
@@ -854,15 +855,15 @@
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
+            method='PUT',
             resource_path='/storage/counter/increment',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
@@ -876,17 +877,17 @@
 
 
     @validate_call
     def upsert_by_key_from_storage(
         self,
         key: StrictStr,
         x_monday_access_token: StrictStr,
-        shared: StrictBool,
-        previous_version: StrictStr,
         storage_data_contract: StorageDataContract,
+        shared: Optional[StrictBool] = None,
+        previous_version: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -899,20 +900,20 @@
         """upsert_by_key_from_storage
 
 
         :param key: (required)
         :type key: str
         :param x_monday_access_token: (required)
         :type x_monday_access_token: str
-        :param shared: (required)
-        :type shared: bool
-        :param previous_version: (required)
-        :type previous_version: str
         :param storage_data_contract: (required)
         :type storage_data_contract: StorageDataContract
+        :param shared:
+        :type shared: bool
+        :param previous_version:
+        :type previous_version: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -930,17 +931,17 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upsert_by_key_from_storage_serialize(
             key=key,
             x_monday_access_token=x_monday_access_token,
+            storage_data_contract=storage_data_contract,
             shared=shared,
             previous_version=previous_version,
-            storage_data_contract=storage_data_contract,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -958,17 +959,17 @@
 
 
     @validate_call
     def upsert_by_key_from_storage_with_http_info(
         self,
         key: StrictStr,
         x_monday_access_token: StrictStr,
-        shared: StrictBool,
-        previous_version: StrictStr,
         storage_data_contract: StorageDataContract,
+        shared: Optional[StrictBool] = None,
+        previous_version: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -981,20 +982,20 @@
         """upsert_by_key_from_storage
 
 
         :param key: (required)
         :type key: str
         :param x_monday_access_token: (required)
         :type x_monday_access_token: str
-        :param shared: (required)
-        :type shared: bool
-        :param previous_version: (required)
-        :type previous_version: str
         :param storage_data_contract: (required)
         :type storage_data_contract: StorageDataContract
+        :param shared:
+        :type shared: bool
+        :param previous_version:
+        :type previous_version: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1012,17 +1013,17 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upsert_by_key_from_storage_serialize(
             key=key,
             x_monday_access_token=x_monday_access_token,
+            storage_data_contract=storage_data_contract,
             shared=shared,
             previous_version=previous_version,
-            storage_data_contract=storage_data_contract,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1040,17 +1041,17 @@
 
 
     @validate_call
     def upsert_by_key_from_storage_without_preload_content(
         self,
         key: StrictStr,
         x_monday_access_token: StrictStr,
-        shared: StrictBool,
-        previous_version: StrictStr,
         storage_data_contract: StorageDataContract,
+        shared: Optional[StrictBool] = None,
+        previous_version: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1063,20 +1064,20 @@
         """upsert_by_key_from_storage
 
 
         :param key: (required)
         :type key: str
         :param x_monday_access_token: (required)
         :type x_monday_access_token: str
-        :param shared: (required)
-        :type shared: bool
-        :param previous_version: (required)
-        :type previous_version: str
         :param storage_data_contract: (required)
         :type storage_data_contract: StorageDataContract
+        :param shared:
+        :type shared: bool
+        :param previous_version:
+        :type previous_version: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1094,17 +1095,17 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._upsert_by_key_from_storage_serialize(
             key=key,
             x_monday_access_token=x_monday_access_token,
+            storage_data_contract=storage_data_contract,
             shared=shared,
             previous_version=previous_version,
-            storage_data_contract=storage_data_contract,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1117,17 +1118,17 @@
         return response_data.response
 
 
     def _upsert_by_key_from_storage_serialize(
         self,
         key,
         x_monday_access_token,
+        storage_data_contract,
         shared,
         previous_version,
-        storage_data_contract,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
```

### Comparing `monday_code-0.0.5/monday_code/api_client.py` & `monday_code-0.0.6/monday_code/api_client.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code/api_response.py` & `monday_code-0.0.6/monday_code/api_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code/configuration.py` & `monday_code-0.0.6/monday_code/configuration.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code/exceptions.py` & `monday_code-0.0.6/monday_code/exceptions.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code/models/__init__.py` & `monday_code-0.0.6/monday_code/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 
 # import models into model package
 from monday_code.models.get_by_key_from_storage404_response import GetByKeyFromStorage404Response
 from monday_code.models.get_by_key_from_storage500_response import GetByKeyFromStorage500Response
 from monday_code.models.increment_counter_params import IncrementCounterParams
 from monday_code.models.json_value import JsonValue
+from monday_code.models.log_methods import LogMethods
 from monday_code.models.period import Period
 from monday_code.models.publish_message_params import PublishMessageParams
 from monday_code.models.publish_message_response import PublishMessageResponse
 from monday_code.models.secure_storage_data_contract import SecureStorageDataContract
 from monday_code.models.storage_data_contract import StorageDataContract
 from monday_code.models.validate_secret_params import ValidateSecretParams
 from monday_code.models.validate_secret_response import ValidateSecretResponse
+from monday_code.models.write_log_request_body import WriteLogRequestBody
+from monday_code.models.write_log_request_body_error import WriteLogRequestBodyError
```

### Comparing `monday_code-0.0.5/monday_code/models/get_by_key_from_storage404_response.py` & `monday_code-0.0.6/monday_code/models/get_by_key_from_storage500_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetByKeyFromStorage404Response(BaseModel):
+class GetByKeyFromStorage500Response(BaseModel):
     """
-    GetByKeyFromStorage404Response
+    GetByKeyFromStorage500Response
     """ # noqa: E501
-    reason: StrictStr
+    reason: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["reason"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetByKeyFromStorage404Response from a JSON string"""
+        """Create an instance of GetByKeyFromStorage500Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,15 +68,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetByKeyFromStorage404Response from a dict"""
+        """Create an instance of GetByKeyFromStorage500Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `monday_code-0.0.5/monday_code/models/get_by_key_from_storage500_response.py` & `monday_code-0.0.6/monday_code/models/get_by_key_from_storage404_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetByKeyFromStorage500Response(BaseModel):
+class GetByKeyFromStorage404Response(BaseModel):
     """
-    GetByKeyFromStorage500Response
+    GetByKeyFromStorage404Response
     """ # noqa: E501
-    reason: Optional[StrictStr] = None
+    reason: StrictStr
     __properties: ClassVar[List[str]] = ["reason"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetByKeyFromStorage500Response from a JSON string"""
+        """Create an instance of GetByKeyFromStorage404Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,15 +68,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetByKeyFromStorage500Response from a dict"""
+        """Create an instance of GetByKeyFromStorage404Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `monday_code-0.0.5/monday_code/models/increment_counter_params.py` & `monday_code-0.0.6/monday_code/models/increment_counter_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Union
 from monday_code.models.period import Period
 from typing import Optional, Set
 from typing_extensions import Self
 
 class IncrementCounterParams(BaseModel):
     """
@@ -30,19 +30,19 @@
     """ # noqa: E501
     renewal_date: datetime = Field(alias="renewalDate")
     kind: StrictStr
     increment_by: Union[StrictFloat, StrictInt] = Field(alias="incrementBy")
     period: Period
     __properties: ClassVar[List[str]] = ["renewalDate", "kind", "incrementBy", "period"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `monday_code-0.0.5/monday_code/models/json_value.py` & `monday_code-0.0.6/monday_code/models/json_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, ValidationError, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr, ValidationError, field_validator
 from typing import Dict, List, Optional, Union
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
 JSONVALUE_ANY_OF_SCHEMAS = ["Dict[str, JsonValue]", "List[JsonValue]", "bool", "float", "str"]
```

### Comparing `monday_code-0.0.5/monday_code/models/period.py` & `monday_code-0.0.6/monday_code/models/period.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code/models/publish_message_params.py` & `monday_code-0.0.6/monday_code/models/publish_message_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PublishMessageParams(BaseModel):
     """
     PublishMessageParams
     """ # noqa: E501
     message: StrictStr
     __properties: ClassVar[List[str]] = ["message"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `monday_code-0.0.5/monday_code/models/publish_message_response.py` & `monday_code-0.0.6/monday_code/models/validate_secret_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictBool
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PublishMessageResponse(BaseModel):
+class ValidateSecretResponse(BaseModel):
     """
-    PublishMessageResponse
+    ValidateSecretResponse
     """ # noqa: E501
-    id: StrictStr
-    __properties: ClassVar[List[str]] = ["id"]
+    valid: StrictBool
+    __properties: ClassVar[List[str]] = ["valid"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PublishMessageResponse from a JSON string"""
+        """Create an instance of ValidateSecretResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,20 +68,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PublishMessageResponse from a dict"""
+        """Create an instance of ValidateSecretResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id")
+            "valid": obj.get("valid")
         })
         return _obj
```

### Comparing `monday_code-0.0.5/monday_code/models/secure_storage_data_contract.py` & `monday_code-0.0.6/monday_code/models/secure_storage_data_contract.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SecureStorageDataContract(BaseModel):
     """
     SecureStorageDataContract
     """ # noqa: E501
     value: Optional[Any]
     __properties: ClassVar[List[str]] = ["value"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `monday_code-0.0.5/monday_code/models/storage_data_contract.py` & `monday_code-0.0.6/monday_code/models/storage_data_contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from monday_code.models.json_value import JsonValue
 from typing import Optional, Set
 from typing_extensions import Self
 
 class StorageDataContract(BaseModel):
     """
     StorageDataContract
     """ # noqa: E501
     version: StrictStr
     value: Optional[JsonValue]
     __properties: ClassVar[List[str]] = ["version", "value"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `monday_code-0.0.5/monday_code/models/validate_secret_params.py` & `monday_code-0.0.6/monday_code/models/validate_secret_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ValidateSecretParams(BaseModel):
     """
     ValidateSecretParams
     """ # noqa: E501
     secret: StrictStr
     __properties: ClassVar[List[str]] = ["secret"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `monday_code-0.0.5/monday_code/models/validate_secret_response.py` & `monday_code-0.0.6/monday_code/models/publish_message_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictBool
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ValidateSecretResponse(BaseModel):
+class PublishMessageResponse(BaseModel):
     """
-    ValidateSecretResponse
+    PublishMessageResponse
     """ # noqa: E501
-    valid: StrictBool
-    __properties: ClassVar[List[str]] = ["valid"]
+    id: StrictStr
+    __properties: ClassVar[List[str]] = ["id"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ValidateSecretResponse from a JSON string"""
+        """Create an instance of PublishMessageResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,20 +68,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ValidateSecretResponse from a dict"""
+        """Create an instance of PublishMessageResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "valid": obj.get("valid")
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `monday_code-0.0.5/monday_code/rest.py` & `monday_code-0.0.6/monday_code/rest.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/monday_code.egg-info/PKG-INFO` & `monday_code-0.0.6/monday_code.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monday-code
-Version: 0.0.5
+Version: 0.0.6
 Summary: mcode-sdk-api
 Home-page: 
 Author: Monday.Com
 Author-email: support@monday.com
 License: MIT
 Keywords: monday-code
 Description-Content-Type: text/markdown
```

### Comparing `monday_code-0.0.5/monday_code.egg-info/SOURCES.txt` & `monday_code-0.0.6/monday_code.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,38 +13,48 @@
 monday_code/rest.py
 monday_code.egg-info/PKG-INFO
 monday_code.egg-info/SOURCES.txt
 monday_code.egg-info/dependency_links.txt
 monday_code.egg-info/requires.txt
 monday_code.egg-info/top_level.txt
 monday_code/api/__init__.py
+monday_code/api/environment_variables_api.py
+monday_code/api/logs_api.py
 monday_code/api/queue_api.py
-monday_code/api/secret_api.py
+monday_code/api/secrets_api.py
 monday_code/api/secure_storage_api.py
 monday_code/api/storage_api.py
 monday_code/models/__init__.py
 monday_code/models/get_by_key_from_storage404_response.py
 monday_code/models/get_by_key_from_storage500_response.py
 monday_code/models/increment_counter_params.py
 monday_code/models/json_value.py
+monday_code/models/log_methods.py
 monday_code/models/period.py
 monday_code/models/publish_message_params.py
 monday_code/models/publish_message_response.py
 monday_code/models/secure_storage_data_contract.py
 monday_code/models/storage_data_contract.py
 monday_code/models/validate_secret_params.py
 monday_code/models/validate_secret_response.py
+monday_code/models/write_log_request_body.py
+monday_code/models/write_log_request_body_error.py
+test/test_environment_variables_api.py
 test/test_get_by_key_from_storage404_response.py
 test/test_get_by_key_from_storage500_response.py
 test/test_increment_counter_params.py
 test/test_json_value.py
+test/test_log_methods.py
+test/test_logs_api.py
 test/test_period.py
 test/test_publish_message_params.py
 test/test_publish_message_response.py
 test/test_queue_api.py
-test/test_secret_api.py
+test/test_secrets_api.py
 test/test_secure_storage_api.py
 test/test_secure_storage_data_contract.py
 test/test_storage_api.py
 test/test_storage_data_contract.py
 test/test_validate_secret_params.py
-test/test_validate_secret_response.py
+test/test_validate_secret_response.py
+test/test_write_log_request_body.py
+test/test_write_log_request_body_error.py
```

### Comparing `monday_code-0.0.5/pyproject.toml` & `monday_code-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/setup.py` & `monday_code-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "monday-code"
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `monday_code-0.0.5/test/test_get_by_key_from_storage404_response.py` & `monday_code-0.0.6/test/test_get_by_key_from_storage404_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_get_by_key_from_storage500_response.py` & `monday_code-0.0.6/test/test_get_by_key_from_storage500_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_increment_counter_params.py` & `monday_code-0.0.6/test/test_increment_counter_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_json_value.py` & `monday_code-0.0.6/test/test_json_value.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_period.py` & `monday_code-0.0.6/test/test_period.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_publish_message_params.py` & `monday_code-0.0.6/test/test_publish_message_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_publish_message_response.py` & `monday_code-0.0.6/test/test_publish_message_response.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_queue_api.py` & `monday_code-0.0.6/test/test_queue_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_secret_api.py` & `monday_code-0.0.6/test/test_secrets_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,34 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from monday_code.api.secret_api import SecretApi
+from monday_code.api.secrets_api import SecretsApi
 
 
-class TestSecretApi(unittest.TestCase):
-    """SecretApi unit test stubs"""
+class TestSecretsApi(unittest.TestCase):
+    """SecretsApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = SecretApi()
+        self.api = SecretsApi()
 
     def tearDown(self) -> None:
         pass
 
     def test_get_secret(self) -> None:
         """Test case for get_secret
 
         """
         pass
 
+    def test_get_secret_keys(self) -> None:
+        """Test case for get_secret_keys
+
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `monday_code-0.0.5/test/test_secure_storage_api.py` & `monday_code-0.0.6/test/test_secure_storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_secure_storage_data_contract.py` & `monday_code-0.0.6/test/test_secure_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_storage_api.py` & `monday_code-0.0.6/test/test_storage_api.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_storage_data_contract.py` & `monday_code-0.0.6/test/test_storage_data_contract.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_validate_secret_params.py` & `monday_code-0.0.6/test/test_validate_secret_params.py`

 * *Files identical despite different names*

### Comparing `monday_code-0.0.5/test/test_validate_secret_response.py` & `monday_code-0.0.6/test/test_validate_secret_response.py`

 * *Files identical despite different names*

