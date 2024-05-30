# Comparing `tmp/qase_api_v2_client-1.0.0b1.tar.gz` & `tmp/qase_api_v2_client-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_api_v2_client-1.0.0b1.tar", last modified: Mon May  6 08:21:28 2024, max compression
+gzip compressed data, was "qase_api_v2_client-1.0.0b2.tar", last modified: Mon May  6 16:09:42 2024, max compression
```

## Comparing `qase_api_v2_client-1.0.0b1.tar` & `qase_api_v2_client-1.0.0b2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.369780 qase_api_v2_client-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-06 08:21:28.369780 qase_api_v2_client-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:21:28.369780 qase_api_v2_client-1.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.361780 qase_api_v2_client-1.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.361780 qase_api_v2_client-1.0.0b1/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.361780 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.361780 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api/results_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25548 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.365780 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/base_error_field_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/base_error_field_response_error_fields_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/base_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/create_result_v2422_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/create_results_request_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/relation_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/relation_suite_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_steps_type.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.369780 qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-06 08:21:28.000000 qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-06 08:21:28.000000 qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:21:28.000000 qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 08:21:28.000000 qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:21:28.000000 qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:21:28.369780 qase_api_v2_client-1.0.0b1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_base_error_field_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_base_error_field_response_error_fields_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_base_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_create_result_v2422_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_create_results_request_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_relation_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_relation_suite_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_step_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_step_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_step_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_result_steps_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-06 08:21:18.000000 qase_api_v2_client-1.0.0b1/test/test_results_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.769496 qase_api_v2_client-1.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-06 16:09:42.769496 qase_api_v2_client-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:09:42.769496 qase_api_v2_client-1.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.757496 qase_api_v2_client-1.0.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.761496 qase_api_v2_client-1.0.0b2/src/qase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.761496 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.761496 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25963 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api/results_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25619 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15323 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.765496 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/base_error_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/base_error_field_response_error_fields_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/base_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/create_result_v2422_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/create_results_request_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/relation_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/relation_suite_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_steps_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.769496 qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-06 16:09:42.000000 qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-06 16:09:42.000000 qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:09:42.000000 qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 16:09:42.000000 qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 16:09:42.000000 qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:09:42.765496 qase_api_v2_client-1.0.0b2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_base_error_field_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_base_error_field_response_error_fields_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_base_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_create_result_v2422_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_create_results_request_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_relation_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_relation_suite_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_step_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_step_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_step_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_result_steps_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-06 16:09:36.000000 qase_api_v2_client-1.0.0b2/test/test_results_api.py
```

### Comparing `qase_api_v2_client-1.0.0b1/PKG-INFO` & `qase_api_v2_client-1.0.0b2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-api-v2-client
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Qase TestOps API V2 client for Python
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python
 Keywords: OpenAPI,OpenAPI-Generator,Qase.io TestOps API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -47,15 +47,15 @@
 
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 
 ```python
 
-import qase
+import qase.api_client_v2
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
@@ -64,32 +64,32 @@
 
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 
 ```python
 
-import qase
+import qase.api_client_v2
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from qase.rest import ApiException
+from qase.api_client_v2.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.qase.io/v2
 # See configuration.py for a list of all supported configuration parameters.
-configuration = qase.Configuration(
+configuration = qase.api_client_v2.Configuration(
     host="https://api.qase.io/v2"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
@@ -98,20 +98,20 @@
 configuration.api_key['TokenAuth'] = os.environ["API_KEY"]
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['TokenAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
-with qase.ApiClient(configuration) as api_client:
+with qase.api_client_v2.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = qase.ResultsApi(api_client)
+    api_instance = qase.api_client_v2.ResultsApi(api_client)
     project_code = 'project_code_example'  # str | 
     run_id = 56  # int | 
-    result_create = qase.ResultCreate()  # ResultCreate | 
+    result_create = qase.api_client_v2.ResultCreate()  # ResultCreate | 
 
     try:
         # (Beta) Create test run result
         api_instance.create_result_v2(project_code, run_id, result_create)
     except ApiException as e:
         print("Exception when calling ResultsApi->create_result_v2: %s\n" % e)
```

### Comparing `qase_api_v2_client-1.0.0b1/README.md` & `qase_api_v2_client-1.0.0b2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 
 ```python
 
-import qase
+import qase.api_client_v2
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
@@ -43,32 +43,32 @@
 
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 
 ```python
 
-import qase
+import qase.api_client_v2
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from qase.rest import ApiException
+from qase.api_client_v2.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.qase.io/v2
 # See configuration.py for a list of all supported configuration parameters.
-configuration = qase.Configuration(
+configuration = qase.api_client_v2.Configuration(
     host="https://api.qase.io/v2"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
@@ -77,20 +77,20 @@
 configuration.api_key['TokenAuth'] = os.environ["API_KEY"]
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['TokenAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
-with qase.ApiClient(configuration) as api_client:
+with qase.api_client_v2.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = qase.ResultsApi(api_client)
+    api_instance = qase.api_client_v2.ResultsApi(api_client)
     project_code = 'project_code_example'  # str | 
     run_id = 56  # int | 
-    result_create = qase.ResultCreate()  # ResultCreate | 
+    result_create = qase.api_client_v2.ResultCreate()  # ResultCreate | 
 
     try:
         # (Beta) Create test run result
         api_instance.create_result_v2(project_code, run_id, result_create)
     except ApiException as e:
         print("Exception when calling ResultsApi->create_result_v2: %s\n" % e)
```

### Comparing `qase_api_v2_client-1.0.0b1/pyproject.toml` & `qase_api_v2_client-1.0.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-api-v2-client"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "Qase TestOps API V2 client for Python"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api/results_api.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api/results_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 """  # noqa: E501
 
 from pydantic import validate_call, Field, StrictFloat
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import StrictInt, StrictStr
-from src.qase.api_client_v2.models.create_results_request_v2 import CreateResultsRequestV2
-from src.qase.api_client_v2.models.result_create import ResultCreate
+from qase.api_client_v2.models.create_results_request_v2 import CreateResultsRequestV2
+from qase.api_client_v2.models.result_create import ResultCreate
 
-from src.qase.api_client_v2.api_client import ApiClient, RequestSerialized
-from src.qase.api_client_v2.api_response import ApiResponse
-from src.qase.api_client_v2.rest import RESTResponseType
+from qase.api_client_v2.api_client import ApiClient, RequestSerialized
+from qase.api_client_v2.api_response import ApiResponse
+from qase.api_client_v2.rest import RESTResponseType
 
 
 class ResultsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api_client.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 from typing import Tuple, Optional, List, Dict
 
-from .configuration import Configuration
-from .api_response import ApiResponse, T as ApiResponseT
-from . import rest
-from .exceptions import (
+from qase.api_client_v2.configuration import Configuration
+from qase.api_client_v2.api_response import ApiResponse, T as ApiResponseT
+from qase.api_client_v2 import rest
+from qase.api_client_v2.exceptions import (
     ApiValueError,
     ApiException
 )
 
 RequestSerialized = Tuple[str, str, Dict[str, str], Optional[str], List[str]]
 
 class ApiClient:
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/api_response.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/api_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/configuration.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/configuration.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/exceptions.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/exceptions.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/base_error_field_response.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/base_error_field_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
-from .base_error_field_response_error_fields_inner import BaseErrorFieldResponseErrorFieldsInner
+from qase.api_client_v2.models.base_error_field_response_error_fields_inner import BaseErrorFieldResponseErrorFieldsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class BaseErrorFieldResponse(BaseModel):
     """
     BaseErrorFieldResponse
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/base_error_field_response_error_fields_inner.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/base_error_field_response_error_fields_inner.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/base_error_response.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/base_error_response.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/create_result_v2422_response.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/create_result_v2422_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List
-from .base_error_field_response_error_fields_inner import BaseErrorFieldResponseErrorFieldsInner
+from qase.api_client_v2.models.base_error_field_response_error_fields_inner import BaseErrorFieldResponseErrorFieldsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateResultV2422Response(BaseModel):
     """
     CreateResultV2422Response
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/create_results_request_v2.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/create_results_request_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from .result_create import ResultCreate
+from qase.api_client_v2.models.result_create import ResultCreate
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateResultsRequestV2(BaseModel):
     """
     CreateResultsRequestV2
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/relation_suite.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/relation_suite.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from .relation_suite_item import RelationSuiteItem
+from qase.api_client_v2.models.relation_suite_item import RelationSuiteItem
 from typing import Optional, Set
 from typing_extensions import Self
 
 class RelationSuite(BaseModel):
     """
     RelationSuite
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/relation_suite_item.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/relation_suite_item.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_create.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Union
-from .result_execution import ResultExecution
-from .result_relations import ResultRelations
-from .result_step import ResultStep
-from .result_steps_type import ResultStepsType
+from qase.api_client_v2.models.result_execution import ResultExecution
+from qase.api_client_v2.models.result_relations import ResultRelations
+from qase.api_client_v2.models.result_step import ResultStep
+from qase.api_client_v2.models.result_steps_type import ResultStepsType
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultCreate(BaseModel):
     """
     ResultCreate
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_execution.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_execution.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_relations.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from .relation_suite import RelationSuite
+from qase.api_client_v2.models.relation_suite import RelationSuite
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultRelations(BaseModel):
     """
     ResultRelations
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing import Any, ClassVar, Dict, List
-from .result_step_data import ResultStepData
-from .result_step_execution import ResultStepExecution
+from qase.api_client_v2.models.result_step_data import ResultStepData
+from qase.api_client_v2.models.result_step_execution import ResultStepExecution
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultStep(BaseModel):
     """
     ResultStep
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step_data.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step_data.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step_execution.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Union
-from .result_step_status import ResultStepStatus
+from qase.api_client_v2.models.result_step_status import ResultStepStatus
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ResultStepExecution(BaseModel):
     """
     ResultStepExecution
     """ # noqa: E501
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_step_status.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_step_status.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/models/result_steps_type.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/models/result_steps_type.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/src/qase/api_client_v2/rest.py` & `qase_api_v2_client-1.0.0b2/src/qase/api_client_v2/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import io
 import json
 import re
 import ssl
 
 import urllib3
 
-from .exceptions import ApiException, ApiValueError
+from qase.api_client_v2.exceptions import ApiException, ApiValueError
 
 SUPPORTED_SOCKS_PROXIES = {"socks5", "socks5h", "socks4", "socks4a"}
 RESTResponseType = urllib3.HTTPResponse
 
 
 def is_socks_proxy_url(url):
     if url is None:
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/PKG-INFO` & `qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-api-v2-client
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Qase TestOps API V2 client for Python
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python
 Keywords: OpenAPI,OpenAPI-Generator,Qase.io TestOps API
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -47,15 +47,15 @@
 
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 
 ```python
 
-import qase
+import qase.api_client_v2
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
@@ -64,32 +64,32 @@
 
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 
 ```python
 
-import qase
+import qase.api_client_v2
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
-from qase.rest import ApiException
+from qase.api_client_v2.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://api.qase.io/v2
 # See configuration.py for a list of all supported configuration parameters.
-configuration = qase.Configuration(
+configuration = qase.api_client_v2.Configuration(
     host="https://api.qase.io/v2"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
@@ -98,20 +98,20 @@
 configuration.api_key['TokenAuth'] = os.environ["API_KEY"]
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['TokenAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
-with qase.ApiClient(configuration) as api_client:
+with qase.api_client_v2.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = qase.ResultsApi(api_client)
+    api_instance = qase.api_client_v2.ResultsApi(api_client)
     project_code = 'project_code_example'  # str | 
     run_id = 56  # int | 
-    result_create = qase.ResultCreate()  # ResultCreate | 
+    result_create = qase.api_client_v2.ResultCreate()  # ResultCreate | 
 
     try:
         # (Beta) Create test run result
         api_instance.create_result_v2(project_code, run_id, result_create)
     except ApiException as e:
         print("Exception when calling ResultsApi->create_result_v2: %s\n" % e)
```

### Comparing `qase_api_v2_client-1.0.0b1/src/qase_api_v2_client.egg-info/SOURCES.txt` & `qase_api_v2_client-1.0.0b2/src/qase_api_v2_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.md
 pyproject.toml
+src/qase/__init__.py
 src/qase/api_client_v2/__init__.py
 src/qase/api_client_v2/api_client.py
 src/qase/api_client_v2/api_response.py
 src/qase/api_client_v2/configuration.py
 src/qase/api_client_v2/exceptions.py
 src/qase/api_client_v2/py.typed
 src/qase/api_client_v2/rest.py
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_base_error_field_response.py` & `qase_api_v2_client-1.0.0b2/test/test_base_error_field_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.base_error_field_response import BaseErrorFieldResponse
+from qase.api_client_v2.models.base_error_field_response import BaseErrorFieldResponse
 
 class TestBaseErrorFieldResponse(unittest.TestCase):
     """BaseErrorFieldResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_base_error_field_response_error_fields_inner.py` & `qase_api_v2_client-1.0.0b2/test/test_base_error_field_response_error_fields_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.base_error_field_response_error_fields_inner import BaseErrorFieldResponseErrorFieldsInner
+from qase.api_client_v2.models.base_error_field_response_error_fields_inner import BaseErrorFieldResponseErrorFieldsInner
 
 class TestBaseErrorFieldResponseErrorFieldsInner(unittest.TestCase):
     """BaseErrorFieldResponseErrorFieldsInner unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_base_error_response.py` & `qase_api_v2_client-1.0.0b2/test/test_base_error_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.base_error_response import BaseErrorResponse
+from qase.api_client_v2.models.base_error_response import BaseErrorResponse
 
 class TestBaseErrorResponse(unittest.TestCase):
     """BaseErrorResponse unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_create_result_v2422_response.py` & `qase_api_v2_client-1.0.0b2/test/test_create_result_v2422_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.create_result_v2422_response import CreateResultV2422Response
+from qase.api_client_v2.models.create_result_v2422_response import CreateResultV2422Response
 
 class TestCreateResultV2422Response(unittest.TestCase):
     """CreateResultV2422Response unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_create_results_request_v2.py` & `qase_api_v2_client-1.0.0b2/test/test_create_results_request_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.create_results_request_v2 import CreateResultsRequestV2
+from qase.api_client_v2.models.create_results_request_v2 import CreateResultsRequestV2
 
 class TestCreateResultsRequestV2(unittest.TestCase):
     """CreateResultsRequestV2 unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_relation_suite.py` & `qase_api_v2_client-1.0.0b2/test/test_relation_suite.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.relation_suite import RelationSuite
+from qase.api_client_v2.models.relation_suite import RelationSuite
 
 class TestRelationSuite(unittest.TestCase):
     """RelationSuite unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_relation_suite_item.py` & `qase_api_v2_client-1.0.0b2/test/test_relation_suite_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.relation_suite_item import RelationSuiteItem
+from qase.api_client_v2.models.relation_suite_item import RelationSuiteItem
 
 class TestRelationSuiteItem(unittest.TestCase):
     """RelationSuiteItem unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_create.py` & `qase_api_v2_client-1.0.0b2/test/test_result_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.result_create import ResultCreate
+from qase.api_client_v2.models.result_create import ResultCreate
 
 class TestResultCreate(unittest.TestCase):
     """ResultCreate unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_execution.py` & `qase_api_v2_client-1.0.0b2/test/test_result_execution.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.result_execution import ResultExecution
+from qase.api_client_v2.models.result_execution import ResultExecution
 
 class TestResultExecution(unittest.TestCase):
     """ResultExecution unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_relations.py` & `qase_api_v2_client-1.0.0b2/test/test_result_relations.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.result_relations import ResultRelations
+from qase.api_client_v2.models.result_relations import ResultRelations
 
 class TestResultRelations(unittest.TestCase):
     """ResultRelations unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_step.py` & `qase_api_v2_client-1.0.0b2/test/test_result_step.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.result_step import ResultStep
+from qase.api_client_v2.models.result_step import ResultStep
 
 class TestResultStep(unittest.TestCase):
     """ResultStep unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_step_data.py` & `qase_api_v2_client-1.0.0b2/test/test_result_step_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.result_step_data import ResultStepData
+from qase.api_client_v2.models.result_step_data import ResultStepData
 
 class TestResultStepData(unittest.TestCase):
     """ResultStepData unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_step_execution.py` & `qase_api_v2_client-1.0.0b2/test/test_result_step_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.models.result_step_execution import ResultStepExecution
+from qase.api_client_v2.models.result_step_execution import ResultStepExecution
 
 class TestResultStepExecution(unittest.TestCase):
     """ResultStepExecution unit test stubs"""
 
     def setUp(self):
         pass
```

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_step_status.py` & `qase_api_v2_client-1.0.0b2/test/test_result_step_status.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/test/test_result_steps_type.py` & `qase_api_v2_client-1.0.0b2/test/test_result_steps_type.py`

 * *Files identical despite different names*

### Comparing `qase_api_v2_client-1.0.0b1/test/test_results_api.py` & `qase_api_v2_client-1.0.0b2/test/test_results_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from src.qase.api_client_v2.api import ResultsApi
+from qase.api_client_v2.api import ResultsApi
 
 
 class TestResultsApi(unittest.TestCase):
     """ResultsApi unit test stubs"""
 
     def setUp(self) -> None:
         self.api = ResultsApi()
```

