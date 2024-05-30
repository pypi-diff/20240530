# Comparing `tmp/sensorbucket-1.0.1.tar.gz` & `tmp/sensorbucket-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensorbucket-1.0.1.tar", last modified: Wed May 10 11:19:10 2023, max compression
+gzip compressed data, was "sensorbucket-1.2.0rc1.tar", last modified: Thu May 30 13:59:07 2024, max compression
```

## Comparing `sensorbucket-1.0.1.tar` & `sensorbucket-1.2.0rc1.tar`

### file list

```diff
@@ -1,58 +1,102 @@
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      813 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/PKG-INFO
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     7260 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/README.md
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      675 2023-05-10 11:18:49.000000 sensorbucket-1.0.1/pyproject.toml
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.368483 sensorbucket-1.0.1/sensorbucket/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4036 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/__init__.py
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.368483 sensorbucket-1.0.1/sensorbucket/api/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      268 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/__init__.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    73852 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/devices_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    25482 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/measurements_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    41566 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/pipelines_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     8943 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/uplink_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    30473 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api_client.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      844 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    15678 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/configuration.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     5599 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/exceptions.py
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/sensorbucket/models/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3290 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/__init__.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2759 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_device201_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3030 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_device_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_device_sensor201_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2783 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2532 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_pipeline_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2970 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_sensor_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2943 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/datastream.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/delete_device_sensor200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3680 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/device.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2446 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/disable_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2735 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/get_device200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2759 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/get_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3495 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2919 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3495 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2919 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3447 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_devices200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2871 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_devices200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3471 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2895 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     6406 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/measurement.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2990 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/paginated_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2500 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/paginated_response_links.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2836 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/pipeline.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3515 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2939 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3067 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/sensor.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2422 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_device200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2965 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_device_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2783 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2807 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_pipeline_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    13243 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/rest.py
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.368483 sensorbucket-1.0.1/sensorbucket.egg-info/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      813 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/PKG-INFO
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2067 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/SOURCES.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)        1 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/dependency_links.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       58 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/requires.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       13 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/top_level.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       69 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/setup.cfg
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2131 2023-05-10 11:19:04.000000 sensorbucket-1.0.1/setup.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2024-05-30 13:59:07.375241 sensorbucket-1.2.0rc1/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      943 2024-05-30 13:59:07.375241 sensorbucket-1.2.0rc1/PKG-INFO
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    13604 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/README.md
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     1932 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/pyproject.toml
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2024-05-30 13:59:07.371908 sensorbucket-1.2.0rc1/sensorbucket/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     6819 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/__init__.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2024-05-30 13:59:07.371908 sensorbucket-1.2.0rc1/sensorbucket/api/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      477 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/__init__.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    47546 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/api_keys_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)   192012 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/devices_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    45709 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/measurements_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    63846 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/pipelines_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    53275 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/tenants_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    30960 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/tracing_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    13534 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/uplink_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    58079 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api/workers_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    25606 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api_client.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      652 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/api_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    16319 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/configuration.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     6418 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/exceptions.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2024-05-30 13:59:07.375241 sensorbucket-1.2.0rc1/sensorbucket/models/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     5860 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/__init__.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3020 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/add_sensor_to_sensor_group201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3073 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/add_sensor_to_sensor_group_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2992 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/add_tenant_member201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3048 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/add_tenant_member_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3123 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/api_error.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3360 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/api_key.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2913 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/api_key_created.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3659 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/archived_ingress.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3302 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_api_key_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3313 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_device201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3573 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_device_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3004 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_device_sensor201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3329 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3080 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_pipeline_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3354 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_sensor_group201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3082 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_sensor_group_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3460 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_sensor_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3614 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_user_worker_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3330 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/create_worker201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3401 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/datastream.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3004 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/delete_device_sensor200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3040 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/delete_sensor_from_sensor_group200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3000 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/delete_sensor_group200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4456 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/device.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2992 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/disable_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3408 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/get_datastream200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4420 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/get_datastream200_response_data.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3301 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/get_device200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3317 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/get_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3342 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/get_sensor_group200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3318 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/get_worker200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3147 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/get_worker_user_code200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3293 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/ingress_dto.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3925 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_api_keys200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3956 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_datastreams200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2919 2024-01-18 07:52:47.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_datastreams200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3948 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_device_sensors200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2919 2024-01-18 07:52:47.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_device_sensors200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3924 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_devices200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2871 2024-01-18 07:52:47.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_devices200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3969 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_ingresses200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3940 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_pipelines200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2895 2024-01-18 07:52:47.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_pipelines200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3965 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_sensor_groups200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3924 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_tenants200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3916 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_traces200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3941 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/list_workers200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     6772 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/measurement.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3486 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/paginated_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3062 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/paginated_response_links.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3435 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/pipeline.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3968 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/query_measurements200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2939 2024-01-18 07:52:47.000000 sensorbucket-1.2.0rc1/sensorbucket/models/query_measurements200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3004 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/remove_tenant_member200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2980 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/revoke_api_key200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3617 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/sensor.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3137 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/sensor_group.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3450 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/tenant.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3839 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/trace.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3390 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/trace_step.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2980 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_device200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3508 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_device_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3329 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3363 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_pipeline_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3000 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_sensor_group200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3082 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_sensor_group_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2983 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_tenant_member_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2980 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_worker200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3639 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/update_worker_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4236 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/models/user_worker.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)        0 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/py.typed
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     9676 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/sensorbucket/rest.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2024-05-30 13:59:07.375241 sensorbucket-1.2.0rc1/sensorbucket.egg-info/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      943 2024-05-30 13:59:07.000000 sensorbucket-1.2.0rc1/sensorbucket.egg-info/PKG-INFO
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4068 2024-05-30 13:59:07.000000 sensorbucket-1.2.0rc1/sensorbucket.egg-info/SOURCES.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)        1 2024-05-30 13:59:07.000000 sensorbucket-1.2.0rc1/sensorbucket.egg-info/dependency_links.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       76 2024-05-30 13:59:07.000000 sensorbucket-1.2.0rc1/sensorbucket.egg-info/requires.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       13 2024-05-30 13:59:07.000000 sensorbucket-1.2.0rc1/sensorbucket.egg-info/top_level.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       69 2024-05-30 13:59:07.375241 sensorbucket-1.2.0rc1/setup.cfg
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2218 2024-05-30 13:55:35.000000 sensorbucket-1.2.0rc1/setup.py
```

### Comparing `sensorbucket-1.0.1/PKG-INFO` & `sensorbucket-1.2.0rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: sensorbucket
-Version: 1.0.1
+Version: 1.2.0rc1
 Summary: Sensorbucket API
 Home-page: https://sensorbucket.nl
 Author: Tim van Osch
 Author-email: info@pollex.nl
 License: EUPLv1.2
 Keywords: OpenAPI,OpenAPI-Generator,Sensorbucket API
 Description-Content-Type: text/markdown
+Requires-Dist: urllib3<2.1.0,>=1.25.3
+Requires-Dist: python-dateutil
+Requires-Dist: pydantic>=2
+Requires-Dist: typing-extensions>=4.7.1
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex&#39;
```

### Comparing `sensorbucket-1.0.1/sensorbucket/api_client.py` & `sensorbucket-1.2.0rc1/sensorbucket/api_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
-import atexit
 import datetime
 from dateutil.parser import parse
 import json
 import mimetypes
-from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
+from typing import Tuple, Optional, List, Dict
 
 from sensorbucket.configuration import Configuration
-from sensorbucket.api_response import ApiResponse
+from sensorbucket.api_response import ApiResponse, T as ApiResponseT
 import sensorbucket.models
 from sensorbucket import rest
-from sensorbucket.exceptions import ApiValueError, ApiException
+from sensorbucket.exceptions import (
+    ApiValueError,
+    ApiException,
+    BadRequestException,
+    UnauthorizedException,
+    ForbiddenException,
+    NotFoundException,
+    ServiceException
+)
 
+RequestSerialized = Tuple[str, str, Dict[str, str], Optional[str], List[str]]
 
-class ApiClient(object):
+class ApiClient:
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
     the methods and models for each application are generated from the OpenAPI
     templates.
 
     :param configuration: .Configuration object for this client
     :param header_name: a header to pass when making calls to the API.
     :param header_value: a header value to pass when making calls to
         the API.
     :param cookie: a cookie to include in the header when making calls
         to the API
-    :param pool_threads: The number of threads to use for async requests
-        to the API. More threads means more concurrent API requests.
     """
 
     PRIMITIVE_TYPES = (float, bool, bytes, str, int)
     NATIVE_TYPES_MAPPING = {
         'int': int,
         'long': int, # TODO remove as only py3 is supported?
         'float': float,
@@ -59,54 +65,40 @@
         'bool': bool,
         'date': datetime.date,
         'datetime': datetime.datetime,
         'object': object,
     }
     _pool = None
 
-    def __init__(self, configuration=None, header_name=None, header_value=None,
-                 cookie=None, pool_threads=1):
+    def __init__(
+        self,
+        configuration=None,
+        header_name=None,
+        header_value=None,
+        cookie=None
+    ) -> None:
         # use default configuration if none is provided
         if configuration is None:
             configuration = Configuration.get_default()
         self.configuration = configuration
-        self.pool_threads = pool_threads
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.2.0-rc1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        self.close()
-
-    def close(self):
-        if self._pool:
-            self._pool.close()
-            self._pool.join()
-            self._pool = None
-            if hasattr(atexit, 'unregister'):
-                atexit.unregister(self.close)
-
-    @property
-    def pool(self):
-        """Create thread pool on first request
-         avoids instantiating unused threadpool for blocking clients.
-        """
-        if self._pool is None:
-            atexit.register(self.close)
-            self._pool = ThreadPool(self.pool_threads)
-        return self._pool
+        pass
 
     @property
     def user_agent(self):
         """User agent for this API client"""
         return self.default_headers['User-Agent']
 
     @user_agent.setter
@@ -139,59 +131,98 @@
 
         It stores default ApiClient.
 
         :param default: object of ApiClient.
         """
         cls._default = default
 
-    def __call_api(
-            self, resource_path, method, path_params=None,
-            query_params=None, header_params=None, body=None, post_params=None,
-            files=None, response_types_map=None, auth_settings=None,
-            _return_http_data_only=None, collection_formats=None,
-            _preload_content=True, _request_timeout=None, _host=None,
-            _request_auth=None):
+    def param_serialize(
+        self,
+        method,
+        resource_path,
+        path_params=None,
+        query_params=None,
+        header_params=None,
+        body=None,
+        post_params=None,
+        files=None, auth_settings=None,
+        collection_formats=None,
+        _host=None,
+        _request_auth=None
+    ) -> RequestSerialized:
+
+        """Builds the HTTP request params needed by the request.
+        :param method: Method to call.
+        :param resource_path: Path to method endpoint.
+        :param path_params: Path parameters in the url.
+        :param query_params: Query parameters in the url.
+        :param header_params: Header parameters to be
+            placed in the request header.
+        :param body: Request body.
+        :param post_params dict: Request post form parameters,
+            for `application/x-www-form-urlencoded`, `multipart/form-data`.
+        :param auth_settings list: Auth Settings names for the request.
+        :param files dict: key -> filename, value -> filepath,
+            for `multipart/form-data`.
+        :param collection_formats: dict of collection formats for path, query,
+            header, and post parameters.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :return: tuple of form (path, http_method, query_params, header_params,
+            body, post_params, files)
+        """
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
             header_params['Cookie'] = self.cookie
         if header_params:
             header_params = self.sanitize_for_serialization(header_params)
-            header_params = dict(self.parameters_to_tuples(header_params,
-                                                           collection_formats))
+            header_params = dict(
+                self.parameters_to_tuples(header_params,collection_formats)
+            )
 
         # path parameters
         if path_params:
             path_params = self.sanitize_for_serialization(path_params)
-            path_params = self.parameters_to_tuples(path_params,
-                                                    collection_formats)
+            path_params = self.parameters_to_tuples(
+                path_params,
+                collection_formats
+            )
             for k, v in path_params:
                 # specified safe chars, encode everything
                 resource_path = resource_path.replace(
                     '{%s}' % k,
                     quote(str(v), safe=config.safe_chars_for_path_param)
                 )
 
         # post parameters
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
-            post_params = self.parameters_to_tuples(post_params,
-                                                    collection_formats)
+            post_params = self.parameters_to_tuples(
+                post_params,
+                collection_formats
+            )
             post_params.extend(self.files_parameters(files))
 
         # auth setting
         self.update_params_for_auth(
-            header_params, query_params, auth_settings,
-            resource_path, method, body,
-            request_auth=_request_auth)
+            header_params,
+            query_params,
+            auth_settings,
+            resource_path,
+            method,
+            body,
+            request_auth=_request_auth
+        )
 
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
         # request url
         if _host is None:
@@ -199,64 +230,107 @@
         else:
             # use server/host defined in path or operation instead
             url = _host + resource_path
 
         # query parameters
         if query_params:
             query_params = self.sanitize_for_serialization(query_params)
-            url_query = self.parameters_to_url_query(query_params,
-                                                     collection_formats)
+            url_query = self.parameters_to_url_query(
+                query_params,
+                collection_formats
+            )
             url += "?" + url_query
 
+        return method, url, header_params, body, post_params
+
+
+    def call_api(
+        self,
+        method,
+        url,
+        header_params=None,
+        body=None,
+        post_params=None,
+        _request_timeout=None
+    ) -> rest.RESTResponse:
+        """Makes the HTTP request (synchronous)
+        :param method: Method to call.
+        :param url: Path to method endpoint.
+        :param header_params: Header parameters to be
+            placed in the request header.
+        :param body: Request body.
+        :param post_params dict: Request post form parameters,
+            for `application/x-www-form-urlencoded`, `multipart/form-data`.
+        :param _request_timeout: timeout setting for this request.
+        :return: RESTResponse
+        """
+
         try:
             # perform request and return response
-            response_data = self.request(
+            response_data = self.rest_client.request(
                 method, url,
-                query_params=query_params,
                 headers=header_params,
-                post_params=post_params, body=body,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout)
+                body=body, post_params=post_params,
+                _request_timeout=_request_timeout
+            )
+
         except ApiException as e:
-            if e.body:
-                e.body = e.body.decode('utf-8')
             raise e
 
-        self.last_response = response_data
+        return response_data
 
-        return_data = None # assuming derialization is not needed
-        # data needs deserialization or returns HTTP data (deserialized) only
-        if _preload_content or _return_http_data_only:
-          response_type = response_types_map.get(str(response_data.status), None)
-
-          if response_type == "bytearray":
-              response_data.data = response_data.data
-          else:
-              match = None
-              content_type = response_data.getheader('content-type')
-              if content_type is not None:
-                  match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
-              encoding = match.group(1) if match else "utf-8"
-              response_data.data = response_data.data.decode(encoding)
-
-          # deserialize response data
-          if response_type == "bytearray":
-              return_data = response_data.data
-          elif response_type:
-              return_data = self.deserialize(response_data, response_type)
-          else:
-              return_data = None
+    def response_deserialize(
+        self,
+        response_data: rest.RESTResponse,
+        response_types_map: Optional[Dict[str, ApiResponseT]]=None
+    ) -> ApiResponse[ApiResponseT]:
+        """Deserializes response into an object.
+        :param response_data: RESTResponse object to be deserialized.
+        :param response_types_map: dict of response types.
+        :return: ApiResponse
+        """
+
+        msg = "RESTResponse.read() must be called before passing it to response_deserialize()"
+        assert response_data.data is not None, msg
+
+        response_type = response_types_map.get(str(response_data.status), None)
+        if not response_type and isinstance(response_data.status, int) and 100 <= response_data.status <= 599:
+            # if not found, look for '1XX', '2XX', etc.
+            response_type = response_types_map.get(str(response_data.status)[0] + "XX", None)
+
+        # deserialize response data
+        response_text = None
+        return_data = None
+        try:
+            if response_type == "bytearray":
+                return_data = response_data.data
+            elif response_type == "file":
+                return_data = self.__deserialize_file(response_data)
+            elif response_type is not None:
+                match = None
+                content_type = response_data.getheader('content-type')
+                if content_type is not None:
+                    match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
+                encoding = match.group(1) if match else "utf-8"
+                response_text = response_data.data.decode(encoding)
+                return_data = self.deserialize(response_text, response_type)
+        finally:
+            if not 200 <= response_data.status <= 299:
+                raise ApiException.from_response(
+                    http_resp=response_data,
+                    body=response_text,
+                    data=return_data,
+                )
 
-        if _return_http_data_only:
-            return return_data
-        else:
-            return ApiResponse(status_code = response_data.status,
-                           data = return_data,
-                           headers = response_data.getheaders(),
-                           raw_data = response_data.data)
+        return ApiResponse(
+            status_code = response_data.status,
+            data = return_data,
+            headers = response_data.getheaders(),
+            raw_data = response_data.data
+        )
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
@@ -269,76 +343,80 @@
         :return: The serialized form of data.
         """
         if obj is None:
             return None
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
         elif isinstance(obj, list):
-            return [self.sanitize_for_serialization(sub_obj)
-                    for sub_obj in obj]
+            return [
+                self.sanitize_for_serialization(sub_obj) for sub_obj in obj
+            ]
         elif isinstance(obj, tuple):
-            return tuple(self.sanitize_for_serialization(sub_obj)
-                         for sub_obj in obj)
+            return tuple(
+                self.sanitize_for_serialization(sub_obj) for sub_obj in obj
+            )
         elif isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
 
-        if isinstance(obj, dict):
+        elif isinstance(obj, dict):
             obj_dict = obj
         else:
             # Convert model obj to dict except
             # attributes `openapi_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
             obj_dict = obj.to_dict()
 
-        return {key: self.sanitize_for_serialization(val)
-                for key, val in obj_dict.items()}
+        return {
+            key: self.sanitize_for_serialization(val)
+            for key, val in obj_dict.items()
+        }
 
-    def deserialize(self, response, response_type):
+    def deserialize(self, response_text, response_type):
         """Deserializes response into an object.
 
         :param response: RESTResponse object to be deserialized.
         :param response_type: class literal for
             deserialized object, or string of class name.
 
         :return: deserialized object.
         """
-        # handle file downloading
-        # save response body into a tmp file and return the instance
-        if response_type == "file":
-            return self.__deserialize_file(response)
 
         # fetch data from response object
         try:
-            data = json.loads(response.data)
+            data = json.loads(response_text)
         except ValueError:
-            data = response.data
+            data = response_text
 
         return self.__deserialize(data, response_type)
 
     def __deserialize(self, data, klass):
         """Deserializes dict, list, str into an object.
 
         :param data: dict, list or str.
         :param klass: class literal, or string of class name.
 
         :return: object.
         """
         if data is None:
             return None
 
-        if type(klass) == str:
+        if isinstance(klass, str):
             if klass.startswith('List['):
-                sub_kls = re.match(r'List\[(.*)]', klass).group(1)
+                m = re.match(r'List\[(.*)]', klass)
+                assert m is not None, "Malformed List type definition"
+                sub_kls = m.group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
             if klass.startswith('Dict['):
-                sub_kls = re.match(r'Dict\[([^,]*), (.*)]', klass).group(2)
+                m = re.match(r'Dict\[([^,]*), (.*)]', klass)
+                assert m is not None, "Malformed Dict type definition"
+                sub_kls = m.group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in data.items()}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -351,154 +429,25 @@
         elif klass == datetime.date:
             return self.__deserialize_date(data)
         elif klass == datetime.datetime:
             return self.__deserialize_datetime(data)
         else:
             return self.__deserialize_model(data, klass)
 
-    def call_api(self, resource_path, method,
-                 path_params=None, query_params=None, header_params=None,
-                 body=None, post_params=None, files=None,
-                 response_types_map=None, auth_settings=None,
-                 async_req=None, _return_http_data_only=None,
-                 collection_formats=None, _preload_content=True,
-                 _request_timeout=None, _host=None, _request_auth=None):
-        """Makes the HTTP request (synchronous) and returns deserialized data.
-
-        To make an async_req request, set the async_req parameter.
-
-        :param resource_path: Path to method endpoint.
-        :param method: Method to call.
-        :param path_params: Path parameters in the url.
-        :param query_params: Query parameters in the url.
-        :param header_params: Header parameters to be
-            placed in the request header.
-        :param body: Request body.
-        :param post_params dict: Request post form parameters,
-            for `application/x-www-form-urlencoded`, `multipart/form-data`.
-        :param auth_settings list: Auth Settings names for the request.
-        :param response: Response data type.
-        :param files dict: key -> filename, value -> filepath,
-            for `multipart/form-data`.
-        :param async_req bool: execute request asynchronously
-        :param _return_http_data_only: response data instead of ApiResponse
-                                       object with status code, headers, etc
-        :param _preload_content: if False, the ApiResponse.data will
-                                 be set to none and raw_data will store the
-                                 HTTP response body without reading/decoding.
-                                 Default is True.
-        :param collection_formats: dict of collection formats for path, query,
-            header, and post parameters.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_token: dict, optional
-        :return:
-            If async_req parameter is True,
-            the request will be called asynchronously.
-            The method will return the request thread.
-            If parameter async_req is False or missing,
-            then the method will return the response directly.
-        """
-        if not async_req:
-            return self.__call_api(resource_path, method,
-                                   path_params, query_params, header_params,
-                                   body, post_params, files,
-                                   response_types_map, auth_settings,
-                                   _return_http_data_only, collection_formats,
-                                   _preload_content, _request_timeout, _host,
-                                   _request_auth)
-
-        return self.pool.apply_async(self.__call_api, (resource_path,
-                                                       method, path_params,
-                                                       query_params,
-                                                       header_params, body,
-                                                       post_params, files,
-                                                       response_types_map,
-                                                       auth_settings,
-                                                       _return_http_data_only,
-                                                       collection_formats,
-                                                       _preload_content,
-                                                       _request_timeout,
-                                                       _host, _request_auth))
-
-    def request(self, method, url, query_params=None, headers=None,
-                post_params=None, body=None, _preload_content=True,
-                _request_timeout=None):
-        """Makes the HTTP request using RESTClient."""
-        if method == "GET":
-            return self.rest_client.get_request(url,
-                                        query_params=query_params,
-                                        _preload_content=_preload_content,
-                                        _request_timeout=_request_timeout,
-                                        headers=headers)
-        elif method == "HEAD":
-            return self.rest_client.head_request(url,
-                                         query_params=query_params,
-                                         _preload_content=_preload_content,
-                                         _request_timeout=_request_timeout,
-                                         headers=headers)
-        elif method == "OPTIONS":
-            return self.rest_client.options_request(url,
-                                            query_params=query_params,
-                                            headers=headers,
-                                            _preload_content=_preload_content,
-                                            _request_timeout=_request_timeout)
-        elif method == "POST":
-            return self.rest_client.post_request(url,
-                                         query_params=query_params,
-                                         headers=headers,
-                                         post_params=post_params,
-                                         _preload_content=_preload_content,
-                                         _request_timeout=_request_timeout,
-                                         body=body)
-        elif method == "PUT":
-            return self.rest_client.put_request(url,
-                                        query_params=query_params,
-                                        headers=headers,
-                                        post_params=post_params,
-                                        _preload_content=_preload_content,
-                                        _request_timeout=_request_timeout,
-                                        body=body)
-        elif method == "PATCH":
-            return self.rest_client.patch_request(url,
-                                          query_params=query_params,
-                                          headers=headers,
-                                          post_params=post_params,
-                                          _preload_content=_preload_content,
-                                          _request_timeout=_request_timeout,
-                                          body=body)
-        elif method == "DELETE":
-            return self.rest_client.delete_request(url,
-                                           query_params=query_params,
-                                           headers=headers,
-                                           _preload_content=_preload_content,
-                                           _request_timeout=_request_timeout,
-                                           body=body)
-        else:
-            raise ApiValueError(
-                "http method must be `GET`, `HEAD`, `OPTIONS`,"
-                " `POST`, `PATCH`, `PUT` or `DELETE`."
-            )
-
     def parameters_to_tuples(self, params, collection_formats):
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: Parameters as list of tuples, collections formatted
         """
-        new_params = []
+        new_params: List[Tuple[str, str]] = []
         if collection_formats is None:
             collection_formats = {}
-        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
+        for k, v in params.items() if isinstance(params, dict) else params:
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
                     new_params.extend((k, value) for value in v)
                 else:
                     if collection_format == 'ssv':
                         delimiter = ' '
@@ -517,40 +466,41 @@
     def parameters_to_url_query(self, params, collection_formats):
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: URL query string (e.g. a=Hello%20World&b=123)
         """
-        new_params = []
+        new_params: List[Tuple[str, str]] = []
         if collection_formats is None:
             collection_formats = {}
-        for k, v in params.items() if isinstance(params, dict) else params:  # noqa: E501
-            if isinstance(v, (int, float)):
-                v = str(v)
+        for k, v in params.items() if isinstance(params, dict) else params:
             if isinstance(v, bool):
                 v = str(v).lower()
+            if isinstance(v, (int, float)):
+                v = str(v)
             if isinstance(v, dict):
                 v = json.dumps(v)
 
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == 'multi':
-                    new_params.extend((k, value) for value in v)
+                    new_params.extend((k, str(value)) for value in v)
                 else:
                     if collection_format == 'ssv':
                         delimiter = ' '
                     elif collection_format == 'tsv':
                         delimiter = '\t'
                     elif collection_format == 'pipes':
                         delimiter = '|'
                     else:  # csv is the default
                         delimiter = ','
                     new_params.append(
-                        (k, delimiter.join(quote(str(value)) for value in v)))
+                        (k, delimiter.join(quote(str(value)) for value in v))
+                    )
             else:
                 new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(item) for item in new_params])
 
     def files_parameters(self, files=None):
         """Builds form parameters.
@@ -565,29 +515,32 @@
                 if not v:
                     continue
                 file_names = v if type(v) is list else [v]
                 for n in file_names:
                     with open(n, 'rb') as f:
                         filename = os.path.basename(f.name)
                         filedata = f.read()
-                        mimetype = (mimetypes.guess_type(filename)[0] or
-                                    'application/octet-stream')
+                        mimetype = (
+                            mimetypes.guess_type(filename)[0]
+                            or 'application/octet-stream'
+                        )
                         params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])]))
+                            tuple([k, tuple([filename, filedata, mimetype])])
+                        )
 
         return params
 
-    def select_header_accept(self, accepts):
+    def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
         """
         if not accepts:
-            return
+            return None
 
         for accept in accepts:
             if re.search('json', accept, re.IGNORECASE):
                 return accept
 
         return accepts[0]
 
@@ -602,17 +555,24 @@
 
         for content_type in content_types:
             if re.search('json', content_type, re.IGNORECASE):
                 return content_type
 
         return content_types[0]
 
-    def update_params_for_auth(self, headers, queries, auth_settings,
-                               resource_path, method, body,
-                               request_auth=None):
+    def update_params_for_auth(
+        self,
+        headers,
+        queries,
+        auth_settings,
+        resource_path,
+        method,
+        body,
+        request_auth=None
+    ) -> None:
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :resource_path: A string representation of the HTTP request resource path.
         :method: A string representation of the HTTP request method.
@@ -621,29 +581,44 @@
         :param request_auth: if set, the provided settings will
                              override the token in the configuration.
         """
         if not auth_settings:
             return
 
         if request_auth:
-            self._apply_auth_params(headers, queries,
-                                    resource_path, method, body,
-                                    request_auth)
-            return
-
-        for auth in auth_settings:
-            auth_setting = self.configuration.auth_settings().get(auth)
-            if auth_setting:
-                self._apply_auth_params(headers, queries,
-                                        resource_path, method, body,
-                                        auth_setting)
-
-    def _apply_auth_params(self, headers, queries,
-                           resource_path, method, body,
-                           auth_setting):
+            self._apply_auth_params(
+                headers,
+                queries,
+                resource_path,
+                method,
+                body,
+                request_auth
+            )
+        else:
+            for auth in auth_settings:
+                auth_setting = self.configuration.auth_settings().get(auth)
+                if auth_setting:
+                    self._apply_auth_params(
+                        headers,
+                        queries,
+                        resource_path,
+                        method,
+                        body,
+                        auth_setting
+                    )
+
+    def _apply_auth_params(
+        self,
+        headers,
+        queries,
+        resource_path,
+        method,
+        body,
+        auth_setting
+    ) -> None:
         """Updates the request parameters based on a single auth_setting
 
         :param headers: Header parameters dict to be updated.
         :param queries: Query parameters tuple list to be updated.
         :resource_path: A string representation of the HTTP request resource path.
         :method: A string representation of the HTTP request method.
         :body: A object representing the body of the HTTP request.
@@ -664,25 +639,32 @@
 
     def __deserialize_file(self, response):
         """Deserializes body to file
 
         Saves response body into a file in a temporary folder,
         using the filename from the `Content-Disposition` header if provided.
 
+        handle file downloading
+        save response body into a tmp file and return the instance
+
         :param response:  RESTResponse.
         :return: file path.
         """
         fd, path = tempfile.mkstemp(dir=self.configuration.temp_folder_path)
         os.close(fd)
         os.remove(path)
 
         content_disposition = response.getheader("Content-Disposition")
         if content_disposition:
-            filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
-                                 content_disposition).group(1)
+            m = re.search(
+                r'filename=[\'"]?([^\'"\s]+)[\'"]?',
+                content_disposition
+            )
+            assert m is not None, "Unexpected 'content-disposition' header value"
+            filename = m.group(1)
             path = os.path.join(os.path.dirname(path), filename)
 
         with open(path, "wb") as f:
             f.write(response.data)
 
         return path
```

### Comparing `sensorbucket-1.0.1/sensorbucket/configuration.py` & `sensorbucket-1.2.0rc1/sensorbucket/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 import copy
 import logging
+from logging import FileHandler
 import multiprocessing
 import sys
+from typing import Optional
 import urllib3
 
 import http.client as httplib
-from sensorbucket.exceptions import ApiValueError
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
-class Configuration(object):
+class Configuration:
     """This class contains various settings of the API client.
 
     :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
@@ -46,47 +47,51 @@
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
-      The validation of enums is performed for variables with defined enum values before.
+      The validation of enums is performed for variables with defined enum
+      values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format.
 
     :Example:
 
-    HTTP Basic Authentication Example.
+    API Key Authentication Example.
     Given the following security scheme in the OpenAPI specification:
       components:
         securitySchemes:
-          http_basic_auth:
-            type: http
-            scheme: basic
+          cookieAuth:         # name for the security scheme
+            type: apiKey
+            in: cookie
+            name: JSESSIONID  # cookie name
 
-    Configure API client with HTTP basic authentication:
+    You can programmatically set the cookie:
 
 conf = sensorbucket.Configuration(
-    username='the-user',
-    password='the-password',
+    api_key={'cookieAuth': 'abc123'}
+    api_key_prefix={'cookieAuth': 'JSESSIONID'}
 )
 
+    The following cookie will be added to the HTTP request:
+       Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
                  access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
-                 ):
+                 ) -> None:
         """Constructor
         """
         self._base_path = "https://sensorbucket.nl/api" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -129,15 +134,15 @@
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
-        self.logger_file_handler = None
+        self.logger_file_handler: Optional[FileHandler] = None
         """Log file handler
         """
         self.logger_file = None
         """Debug file location
         """
         self.debug = False
         """Debug switch
@@ -169,15 +174,15 @@
         """urllib3 connection pool's maximum number of connections saved
            per pool. urllib3 uses 1 connection as default value, but this is
            not the best value when you are making a lot of possibly parallel
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
-        self.proxy = None
+        self.proxy: Optional[str] = None
         """Proxy URL
         """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
@@ -371,48 +376,60 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
-        if self.username is not None and self.password is not None:
-            auth['basicAuth'] = {
-                'type': 'basic',
+        if 'CookieSession' in self.api_key:
+            auth['CookieSession'] = {
+                'type': 'api_key',
+                'in': 'cookie',
+                'key': 'SID',
+                'value': self.get_api_key_with_prefix(
+                    'CookieSession',
+                ),
+            }
+        if self.access_token is not None:
+            auth['APIKey'] = {
+                'type': 'bearer',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
+            }
+        if self.access_token is not None:
+            auth['Noop'] = {
+                'type': 'bearer',
                 'in': 'header',
                 'key': 'Authorization',
-                'value': self.get_basic_auth_token()
+                'value': 'Bearer ' + self.access_token
             }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0\n"\
-               "SDK Package Version: 1.0.0".\
+               "Version of the API: 1.2.0-rc1\n"\
+               "SDK Package Version: 1.2.0-rc1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
                 'url': "https://sensorbucket.nl/api",
                 'description': "Production",
-            },
-            {
-                'url': "http://localhost:3000/api",
-                'description': "Local docker environment",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
```

### Comparing `sensorbucket-1.0.1/sensorbucket/exceptions.py` & `sensorbucket-1.2.0rc1/sensorbucket/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
+from typing import Any, Optional
+from typing_extensions import Self
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
     def __init__(self, msg, path_to_item=None, valid_classes=None,
-                 key_type=None):
+                 key_type=None) -> None:
         """ Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list): a list of keys an indices to get to the
@@ -43,15 +45,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiTypeError, self).__init__(full_msg)
 
 
 class ApiValueError(OpenApiException, ValueError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list) the path to the exception in the
                 received_data dict. None if unset
@@ -61,15 +63,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiValueError, self).__init__(full_msg)
 
 
 class ApiAttributeError(OpenApiException, AttributeError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Raised when an attribute reference or assignment fails.
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
@@ -80,15 +82,15 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiAttributeError, self).__init__(full_msg)
 
 
 class ApiKeyError(OpenApiException, KeyError):
-    def __init__(self, msg, path_to_item=None):
+    def __init__(self, msg, path_to_item=None) -> None:
         """
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (None/list) the path to the exception in the
                 received_data dict
@@ -98,62 +100,97 @@
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
 class ApiException(OpenApiException):
 
-    def __init__(self, status=None, reason=None, http_resp=None):
+    def __init__(
+        self, 
+        status=None, 
+        reason=None, 
+        http_resp=None,
+        *,
+        body: Optional[str] = None,
+        data: Optional[Any] = None,
+    ) -> None:
+        self.status = status
+        self.reason = reason
+        self.body = body
+        self.data = data
+        self.headers = None
+
         if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
+            if self.status is None:
+                self.status = http_resp.status
+            if self.reason is None:
+                self.reason = http_resp.reason
+            if self.body is None:
+                try:
+                    self.body = http_resp.data.decode('utf-8')
+                except Exception:
+                    pass
             self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
+
+    @classmethod
+    def from_response(
+        cls, 
+        *, 
+        http_resp, 
+        body: Optional[str], 
+        data: Optional[Any],
+    ) -> Self:
+        if http_resp.status == 400:
+            raise BadRequestException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 401:
+            raise UnauthorizedException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 403:
+            raise ForbiddenException(http_resp=http_resp, body=body, data=data)
+
+        if http_resp.status == 404:
+            raise NotFoundException(http_resp=http_resp, body=body, data=data)
+
+        if 500 <= http_resp.status <= 599:
+            raise ServiceException(http_resp=http_resp, body=body, data=data)
+        raise ApiException(http_resp=http_resp, body=body, data=data)
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
                 self.headers)
 
-        if self.body:
-            error_message += "HTTP response body: {0}\n".format(self.body)
+        if self.data or self.body:
+            error_message += "HTTP response body: {0}\n".format(self.data or self.body)
 
         return error_message
 
 
-class NotFoundException(ApiException):
+class BadRequestException(ApiException):
+    pass
 
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
 
+class NotFoundException(ApiException):
+    pass
 
-class UnauthorizedException(ApiException):
 
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+class UnauthorizedException(ApiException):
+    pass
 
 
 class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
+    pass
 
 
 class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
+    pass
 
 
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/create_device201_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/get_sensor_group200_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,94 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
 from pydantic import BaseModel, StrictStr
-from sensorbucket.models.device import Device
+from typing import Any, ClassVar, Dict, List, Optional
+from sensorbucket.models.sensor_group import SensorGroup
+from typing import Optional, Set
+from typing_extensions import Self
 
-class CreateDevice201Response(BaseModel):
-    """
-    CreateDevice201Response
+class GetSensorGroup200Response(BaseModel):
     """
+    GetSensorGroup200Response
+    """ # noqa: E501
     message: Optional[StrictStr] = None
-    data: Optional[Device] = None
-    __properties = ["message", "data"]
+    data: Optional[SensorGroup] = None
+    __properties: ClassVar[List[str]] = ["message", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateDevice201Response:
-        """Create an instance of CreateDevice201Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of GetSensorGroup200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateDevice201Response:
-        """Create an instance of CreateDevice201Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of GetSensorGroup200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreateDevice201Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = CreateDevice201Response.parse_obj({
+        _obj = cls.model_validate({
             "message": obj.get("message"),
-            "data": Device.from_dict(obj.get("data")) if obj.get("data") is not None else None
+            "data": SensorGroup.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/create_device_request.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/create_pipeline_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, Dict, Optional, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-
-class CreateDeviceRequest(BaseModel):
+class CreatePipelineRequest(BaseModel):
     """
-    CreateDeviceRequest
-    """
-    code: StrictStr = Field(...)
+    CreatePipelineRequest
+    """ # noqa: E501
     description: Optional[StrictStr] = None
-    latitude: Optional[Union[StrictFloat, StrictInt]] = None
-    longitude: Optional[Union[StrictFloat, StrictInt]] = None
-    location_description: Optional[StrictStr] = None
-    properties: Optional[Dict[str, Any]] = None
-    __properties = ["code", "description", "latitude", "longitude", "location_description", "properties"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    steps: Optional[List[StrictStr]] = None
+    __properties: ClassVar[List[str]] = ["description", "steps"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateDeviceRequest:
-        """Create an instance of CreateDeviceRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreatePipelineRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateDeviceRequest:
-        """Create an instance of CreateDeviceRequest from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreatePipelineRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreateDeviceRequest.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = CreateDeviceRequest.parse_obj({
-            "code": obj.get("code"),
+        _obj = cls.model_validate({
             "description": obj.get("description"),
-            "latitude": obj.get("latitude"),
-            "longitude": obj.get("longitude"),
-            "location_description": obj.get("location_description"),
-            "properties": obj.get("properties")
+            "steps": obj.get("steps")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/create_device_sensor201_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/create_device_sensor201_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,88 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
 from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
 class CreateDeviceSensor201Response(BaseModel):
     """
     CreateDeviceSensor201Response
-    """
+    """ # noqa: E501
     message: Optional[StrictStr] = None
-    __properties = ["message"]
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateDeviceSensor201Response:
+    def from_json(cls, json_str: str) -> Optional[Self]:
         """Create an instance of CreateDeviceSensor201Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateDeviceSensor201Response:
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of CreateDeviceSensor201Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreateDeviceSensor201Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = CreateDeviceSensor201Response.parse_obj({
+        _obj = cls.model_validate({
             "message": obj.get("message")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/create_pipeline200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/list_pipelines200_response_all_of.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, conlist
 from sensorbucket.models.pipeline import Pipeline
 
-class CreatePipeline200Response(BaseModel):
+class ListPipelines200ResponseAllOf(BaseModel):
     """
-    CreatePipeline200Response
+    ListPipelines200ResponseAllOf
     """
-    message: Optional[StrictStr] = None
-    data: Optional[Pipeline] = None
-    __properties = ["message", "data"]
+    data: Optional[conlist(Pipeline)] = None
+    __properties = ["data"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,37 +40,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreatePipeline200Response:
-        """Create an instance of CreatePipeline200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> ListPipelines200ResponseAllOf:
+        """Create an instance of ListPipelines200ResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of data
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
         if self.data:
-            _dict['data'] = self.data.to_dict()
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreatePipeline200Response:
-        """Create an instance of CreatePipeline200Response from a dict"""
+    def from_dict(cls, obj: dict) -> ListPipelines200ResponseAllOf:
+        """Create an instance of ListPipelines200ResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreatePipeline200Response.parse_obj(obj)
+            return ListPipelines200ResponseAllOf.parse_obj(obj)
 
-        _obj = CreatePipeline200Response.parse_obj({
-            "message": obj.get("message"),
-            "data": Pipeline.from_dict(obj.get("data")) if obj.get("data") is not None else None
+        _obj = ListPipelines200ResponseAllOf.parse_obj({
+            "data": [Pipeline.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/create_pipeline_request.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/add_tenant_member_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,90 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List, Optional
-from pydantic import BaseModel, StrictStr, conlist
-
-class CreatePipelineRequest(BaseModel):
+class AddTenantMemberRequest(BaseModel):
     """
-    CreatePipelineRequest
-    """
-    description: Optional[StrictStr] = None
-    steps: Optional[conlist(StrictStr)] = None
-    __properties = ["description", "steps"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    AddTenantMemberRequest
+    """ # noqa: E501
+    user_id: StrictStr
+    permissions: List[StrictStr]
+    __properties: ClassVar[List[str]] = ["user_id", "permissions"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreatePipelineRequest:
-        """Create an instance of CreatePipelineRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of AddTenantMemberRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreatePipelineRequest:
-        """Create an instance of CreatePipelineRequest from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of AddTenantMemberRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreatePipelineRequest.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = CreatePipelineRequest.parse_obj({
-            "description": obj.get("description"),
-            "steps": obj.get("steps")
+        _obj = cls.model_validate({
+            "user_id": obj.get("user_id"),
+            "permissions": obj.get("permissions")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/create_sensor_request.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/get_worker_user_code200_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, Dict, Optional, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-
-class CreateSensorRequest(BaseModel):
+class GetWorkerUserCode200Response(BaseModel):
     """
-    CreateSensorRequest
-    """
-    code: StrictStr = Field(...)
-    description: Optional[StrictStr] = None
-    external_id: StrictStr = Field(...)
-    brand: Optional[StrictStr] = None
-    properties: Optional[Dict[str, Any]] = None
-    archive_time: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties = ["code", "description", "external_id", "brand", "properties", "archive_time"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    GetWorkerUserCode200Response
+    """ # noqa: E501
+    message: Optional[StrictStr] = None
+    data: Optional[StrictStr] = Field(default=None, description="The usercode base64 encoded")
+    __properties: ClassVar[List[str]] = ["message", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreateSensorRequest:
-        """Create an instance of CreateSensorRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of GetWorkerUserCode200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreateSensorRequest:
-        """Create an instance of CreateSensorRequest from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of GetWorkerUserCode200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreateSensorRequest.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = CreateSensorRequest.parse_obj({
-            "code": obj.get("code"),
-            "description": obj.get("description"),
-            "external_id": obj.get("external_id"),
-            "brand": obj.get("brand"),
-            "properties": obj.get("properties"),
-            "archive_time": obj.get("archive_time")
+        _obj = cls.model_validate({
+            "message": obj.get("message"),
+            "data": obj.get("data")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/datastream.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/update_pipeline_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,92 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-
-class Datastream(BaseModel):
+class UpdatePipelineRequest(BaseModel):
     """
-    Datastream
-    """
-    id: Optional[StrictStr] = None
+    UpdatePipelineRequest
+    """ # noqa: E501
     description: Optional[StrictStr] = None
-    sensor_id: Optional[Union[StrictFloat, StrictInt]] = None
-    observed_property: Optional[StrictStr] = None
-    unit_of_measurement: Optional[StrictStr] = None
-    created_at: Optional[StrictStr] = None
-    __properties = ["id", "description", "sensor_id", "observed_property", "unit_of_measurement", "created_at"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    steps: Optional[List[StrictStr]] = None
+    status: Optional[StrictStr] = Field(default=None, description="Used to change a pipeline from inactive to active or vice-versa.  Moving from active to inactive can also be achieve by `DELETE`ing the pipeline resource. ")
+    __properties: ClassVar[List[str]] = ["description", "steps", "status"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Datastream:
-        """Create an instance of Datastream from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of UpdatePipelineRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Datastream:
-        """Create an instance of Datastream from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of UpdatePipelineRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Datastream.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = Datastream.parse_obj({
-            "id": obj.get("id"),
+        _obj = cls.model_validate({
             "description": obj.get("description"),
-            "sensor_id": obj.get("sensor_id"),
-            "observed_property": obj.get("observed_property"),
-            "unit_of_measurement": obj.get("unit_of_measurement"),
-            "created_at": obj.get("created_at")
+            "steps": obj.get("steps"),
+            "status": obj.get("status")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/delete_device_sensor200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/list_devices200_response_all_of.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, conlist
+from sensorbucket.models.device import Device
 
-class DeleteDeviceSensor200Response(BaseModel):
+class ListDevices200ResponseAllOf(BaseModel):
     """
-    DeleteDeviceSensor200Response
+    ListDevices200ResponseAllOf
     """
-    message: Optional[StrictStr] = None
-    __properties = ["message"]
+    data: Optional[conlist(Device)] = None
+    __properties = ["data"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,33 +40,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DeleteDeviceSensor200Response:
-        """Create an instance of DeleteDeviceSensor200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> ListDevices200ResponseAllOf:
+        """Create an instance of ListDevices200ResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
+        if self.data:
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DeleteDeviceSensor200Response:
-        """Create an instance of DeleteDeviceSensor200Response from a dict"""
+    def from_dict(cls, obj: dict) -> ListDevices200ResponseAllOf:
+        """Create an instance of ListDevices200ResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DeleteDeviceSensor200Response.parse_obj(obj)
+            return ListDevices200ResponseAllOf.parse_obj(obj)
 
-        _obj = DeleteDeviceSensor200Response.parse_obj({
-            "message": obj.get("message")
+        _obj = ListDevices200ResponseAllOf.parse_obj({
+            "data": [Device.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/device.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/create_sensor_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,98 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, Dict, List, Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, conlist
-from sensorbucket.models.sensor import Sensor
-
-class Device(BaseModel):
+class CreateSensorRequest(BaseModel):
     """
-    Device
-    """
-    id: Optional[Union[StrictFloat, StrictInt]] = None
-    code: Optional[StrictStr] = None
+    CreateSensorRequest
+    """ # noqa: E501
+    code: StrictStr
     description: Optional[StrictStr] = None
-    organisation: Optional[StrictStr] = None
+    external_id: StrictStr
+    brand: Optional[StrictStr] = None
     properties: Optional[Dict[str, Any]] = None
-    latitude: Optional[Union[StrictFloat, StrictInt]] = None
-    longitude: Optional[Union[StrictFloat, StrictInt]] = None
-    location_description: Optional[StrictStr] = None
-    sensors: Optional[conlist(Sensor)] = None
-    __properties = ["id", "code", "description", "organisation", "properties", "latitude", "longitude", "location_description", "sensors"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    archive_time: Optional[StrictInt] = None
+    __properties: ClassVar[List[str]] = ["code", "description", "external_id", "brand", "properties", "archive_time"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Device:
-        """Create an instance of Device from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreateSensorRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in sensors (list)
-        _items = []
-        if self.sensors:
-            for _item in self.sensors:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sensors'] = _items
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Device:
-        """Create an instance of Device from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreateSensorRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Device.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = Device.parse_obj({
-            "id": obj.get("id"),
+        _obj = cls.model_validate({
             "code": obj.get("code"),
             "description": obj.get("description"),
-            "organisation": obj.get("organisation"),
+            "external_id": obj.get("external_id"),
+            "brand": obj.get("brand"),
             "properties": obj.get("properties"),
-            "latitude": obj.get("latitude"),
-            "longitude": obj.get("longitude"),
-            "location_description": obj.get("location_description"),
-            "sensors": [Sensor.from_dict(_item) for _item in obj.get("sensors")] if obj.get("sensors") is not None else None
+            "archive_time": obj.get("archive_time")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/disable_pipeline200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/list_device_sensors200_response_all_of.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, conlist
+from sensorbucket.models.sensor import Sensor
 
-class DisablePipeline200Response(BaseModel):
+class ListDeviceSensors200ResponseAllOf(BaseModel):
     """
-    DisablePipeline200Response
+    ListDeviceSensors200ResponseAllOf
     """
-    message: Optional[StrictStr] = None
-    __properties = ["message"]
+    data: Optional[conlist(Sensor)] = None
+    __properties = ["data"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,33 +40,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DisablePipeline200Response:
-        """Create an instance of DisablePipeline200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> ListDeviceSensors200ResponseAllOf:
+        """Create an instance of ListDeviceSensors200ResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
+        if self.data:
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DisablePipeline200Response:
-        """Create an instance of DisablePipeline200Response from a dict"""
+    def from_dict(cls, obj: dict) -> ListDeviceSensors200ResponseAllOf:
+        """Create an instance of ListDeviceSensors200ResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return DisablePipeline200Response.parse_obj(obj)
+            return ListDeviceSensors200ResponseAllOf.parse_obj(obj)
 
-        _obj = DisablePipeline200Response.parse_obj({
-            "message": obj.get("message")
+        _obj = ListDeviceSensors200ResponseAllOf.parse_obj({
+            "data": [Sensor.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/get_device200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/disable_pipeline200_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
 from pydantic import BaseModel, StrictStr
-from sensorbucket.models.device import Device
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-class GetDevice200Response(BaseModel):
-    """
-    GetDevice200Response
+class DisablePipeline200Response(BaseModel):
     """
+    DisablePipeline200Response
+    """ # noqa: E501
     message: Optional[StrictStr] = None
-    data: Optional[Device] = None
-    __properties = ["message", "data"]
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetDevice200Response:
-        """Create an instance of GetDevice200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of DisablePipeline200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of data
-        if self.data:
-            _dict['data'] = self.data.to_dict()
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetDevice200Response:
-        """Create an instance of GetDevice200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of DisablePipeline200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return GetDevice200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = GetDevice200Response.parse_obj({
-            "message": obj.get("message"),
-            "data": Device.from_dict(obj.get("data")) if obj.get("data") is not None else None
+        _obj = cls.model_validate({
+            "message": obj.get("message")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/get_pipeline200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/create_device201_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,94 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
 from pydantic import BaseModel, StrictStr
-from sensorbucket.models.pipeline import Pipeline
+from typing import Any, ClassVar, Dict, List, Optional
+from sensorbucket.models.device import Device
+from typing import Optional, Set
+from typing_extensions import Self
 
-class GetPipeline200Response(BaseModel):
-    """
-    GetPipeline200Response
+class CreateDevice201Response(BaseModel):
     """
+    CreateDevice201Response
+    """ # noqa: E501
     message: Optional[StrictStr] = None
-    data: Optional[Pipeline] = None
-    __properties = ["message", "data"]
+    data: Optional[Device] = None
+    __properties: ClassVar[List[str]] = ["message", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetPipeline200Response:
-        """Create an instance of GetPipeline200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreateDevice201Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetPipeline200Response:
-        """Create an instance of GetPipeline200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreateDevice201Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return GetPipeline200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = GetPipeline200Response.parse_obj({
+        _obj = cls.model_validate({
             "message": obj.get("message"),
-            "data": Pipeline.from_dict(obj.get("data")) if obj.get("data") is not None else None
+            "data": Device.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/list_api_keys200_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,106 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import List
-from pydantic import BaseModel, Field, StrictInt, conlist
-from sensorbucket.models.datastream import Datastream
+from pydantic import BaseModel, StrictInt
+from typing import Any, ClassVar, Dict, List
+from sensorbucket.models.api_key import ApiKey
 from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
+from typing import Optional, Set
+from typing_extensions import Self
 
-class ListDatastreams200Response(BaseModel):
+class ListApiKeys200Response(BaseModel):
     """
-    ListDatastreams200Response
-    """
-    links: PaginatedResponseLinks = Field(...)
-    page_size: StrictInt = Field(...)
-    total_count: StrictInt = Field(...)
-    data: conlist(Datastream) = Field(...)
-    __properties = ["links", "page_size", "total_count", "data"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    ListApiKeys200Response
+    """ # noqa: E501
+    links: PaginatedResponseLinks
+    page_size: StrictInt
+    total_count: StrictInt
+    data: List[ApiKey]
+    __properties: ClassVar[List[str]] = ["links", "page_size", "total_count", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListDatastreams200Response:
-        """Create an instance of ListDatastreams200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of ListApiKeys200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         # override the default output from pydantic by calling `to_dict()` of links
         if self.links:
             _dict['links'] = self.links.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in data (list)
         _items = []
         if self.data:
             for _item in self.data:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListDatastreams200Response:
-        """Create an instance of ListDatastreams200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of ListApiKeys200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ListDatastreams200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = ListDatastreams200Response.parse_obj({
-            "links": PaginatedResponseLinks.from_dict(obj.get("links")) if obj.get("links") is not None else None,
+        _obj = cls.model_validate({
+            "links": PaginatedResponseLinks.from_dict(obj["links"]) if obj.get("links") is not None else None,
             "page_size": obj.get("page_size"),
             "total_count": obj.get("total_count"),
-            "data": [Datastream.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+            "data": [ApiKey.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response_all_of.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/list_datastreams200_response_all_of.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/get_device200_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from sensorbucket.models.device import Device
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List
-from pydantic import BaseModel, Field, StrictInt, conlist
-from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
-from sensorbucket.models.sensor import Sensor
-
-class ListDeviceSensors200Response(BaseModel):
+class GetDevice200Response(BaseModel):
     """
-    ListDeviceSensors200Response
-    """
-    links: PaginatedResponseLinks = Field(...)
-    page_size: StrictInt = Field(...)
-    total_count: StrictInt = Field(...)
-    data: conlist(Sensor) = Field(...)
-    __properties = ["links", "page_size", "total_count", "data"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    GetDevice200Response
+    """ # noqa: E501
+    message: Optional[StrictStr] = None
+    data: Optional[Device] = None
+    __properties: ClassVar[List[str]] = ["message", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListDeviceSensors200Response:
-        """Create an instance of ListDeviceSensors200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of GetDevice200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of links
-        if self.links:
-            _dict['links'] = self.links.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
+        # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListDeviceSensors200Response:
-        """Create an instance of ListDeviceSensors200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of GetDevice200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ListDeviceSensors200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = ListDeviceSensors200Response.parse_obj({
-            "links": PaginatedResponseLinks.from_dict(obj.get("links")) if obj.get("links") is not None else None,
-            "page_size": obj.get("page_size"),
-            "total_count": obj.get("total_count"),
-            "data": [Sensor.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = cls.model_validate({
+            "message": obj.get("message"),
+            "data": Device.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response_all_of.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/query_measurements200_response_all_of.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from sensorbucket.models.sensor import Sensor
+from sensorbucket.models.measurement import Measurement
 
-class ListDeviceSensors200ResponseAllOf(BaseModel):
+class QueryMeasurements200ResponseAllOf(BaseModel):
     """
-    ListDeviceSensors200ResponseAllOf
+    QueryMeasurements200ResponseAllOf
     """
-    data: Optional[conlist(Sensor)] = None
+    data: Optional[conlist(Measurement)] = None
     __properties = ["data"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
@@ -40,16 +40,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListDeviceSensors200ResponseAllOf:
-        """Create an instance of ListDeviceSensors200ResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> QueryMeasurements200ResponseAllOf:
+        """Create an instance of QueryMeasurements200ResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -60,20 +60,20 @@
             for _item in self.data:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListDeviceSensors200ResponseAllOf:
-        """Create an instance of ListDeviceSensors200ResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> QueryMeasurements200ResponseAllOf:
+        """Create an instance of QueryMeasurements200ResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ListDeviceSensors200ResponseAllOf.parse_obj(obj)
+            return QueryMeasurements200ResponseAllOf.parse_obj(obj)
 
-        _obj = ListDeviceSensors200ResponseAllOf.parse_obj({
-            "data": [Sensor.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = QueryMeasurements200ResponseAllOf.parse_obj({
+            "data": [Measurement.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_devices200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/delete_sensor_from_sensor_group200_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,88 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List
-from pydantic import BaseModel, Field, StrictInt, conlist
-from sensorbucket.models.device import Device
-from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
-
-class ListDevices200Response(BaseModel):
+class DeleteSensorFromSensorGroup200Response(BaseModel):
     """
-    ListDevices200Response
-    """
-    links: PaginatedResponseLinks = Field(...)
-    page_size: StrictInt = Field(...)
-    total_count: StrictInt = Field(...)
-    data: conlist(Device) = Field(...)
-    __properties = ["links", "page_size", "total_count", "data"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    DeleteSensorFromSensorGroup200Response
+    """ # noqa: E501
+    message: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListDevices200Response:
-        """Create an instance of ListDevices200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of DeleteSensorFromSensorGroup200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of links
-        if self.links:
-            _dict['links'] = self.links.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
-        if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListDevices200Response:
-        """Create an instance of ListDevices200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of DeleteSensorFromSensorGroup200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ListDevices200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = ListDevices200Response.parse_obj({
-            "links": PaginatedResponseLinks.from_dict(obj.get("links")) if obj.get("links") is not None else None,
-            "page_size": obj.get("page_size"),
-            "total_count": obj.get("total_count"),
-            "data": [Device.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = cls.model_validate({
+            "message": obj.get("message")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_devices200_response_all_of.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/api_error.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,92 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List, Optional
-from pydantic import BaseModel, conlist
-from sensorbucket.models.device import Device
-
-class ListDevices200ResponseAllOf(BaseModel):
-    """
-    ListDevices200ResponseAllOf
+class ApiError(BaseModel):
     """
-    data: Optional[conlist(Device)] = None
-    __properties = ["data"]
+    ApiError
+    """ # noqa: E501
+    message: Optional[StrictStr] = None
+    code: Optional[StrictStr] = None
+    http_status: Optional[StrictInt] = None
+    __properties: ClassVar[List[str]] = ["message", "code", "http_status"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListDevices200ResponseAllOf:
-        """Create an instance of ListDevices200ResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of ApiError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
-        if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListDevices200ResponseAllOf:
-        """Create an instance of ListDevices200ResponseAllOf from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of ApiError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ListDevices200ResponseAllOf.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = ListDevices200ResponseAllOf.parse_obj({
-            "data": [Device.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = cls.model_validate({
+            "message": obj.get("message"),
+            "code": obj.get("code"),
+            "http_status": obj.get("http_status")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/create_sensor_group201_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from sensorbucket.models.sensor_group import SensorGroup
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List
-from pydantic import BaseModel, Field, StrictInt, conlist
-from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
-from sensorbucket.models.pipeline import Pipeline
-
-class ListPipelines200Response(BaseModel):
+class CreateSensorGroup201Response(BaseModel):
     """
-    ListPipelines200Response
-    """
-    links: PaginatedResponseLinks = Field(...)
-    page_size: StrictInt = Field(...)
-    total_count: StrictInt = Field(...)
-    data: conlist(Pipeline) = Field(...)
-    __properties = ["links", "page_size", "total_count", "data"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    CreateSensorGroup201Response
+    """ # noqa: E501
+    message: Optional[StrictStr] = None
+    data: Optional[SensorGroup] = None
+    __properties: ClassVar[List[str]] = ["message", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListPipelines200Response:
-        """Create an instance of ListPipelines200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreateSensorGroup201Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of links
-        if self.links:
-            _dict['links'] = self.links.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
+        # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListPipelines200Response:
-        """Create an instance of ListPipelines200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreateSensorGroup201Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ListPipelines200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = ListPipelines200Response.parse_obj({
-            "links": PaginatedResponseLinks.from_dict(obj.get("links")) if obj.get("links") is not None else None,
-            "page_size": obj.get("page_size"),
-            "total_count": obj.get("total_count"),
-            "data": [Pipeline.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = cls.model_validate({
+            "message": obj.get("message"),
+            "data": SensorGroup.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response_all_of.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/api_key_created.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,88 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List, Optional
-from pydantic import BaseModel, conlist
-from sensorbucket.models.pipeline import Pipeline
-
-class ListPipelines200ResponseAllOf(BaseModel):
-    """
-    ListPipelines200ResponseAllOf
+class ApiKeyCreated(BaseModel):
     """
-    data: Optional[conlist(Pipeline)] = None
-    __properties = ["data"]
+    ApiKeyCreated
+    """ # noqa: E501
+    api_key: StrictStr
+    __properties: ClassVar[List[str]] = ["api_key"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListPipelines200ResponseAllOf:
-        """Create an instance of ListPipelines200ResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of ApiKeyCreated from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
-        if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListPipelines200ResponseAllOf:
-        """Create an instance of ListPipelines200ResponseAllOf from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of ApiKeyCreated from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ListPipelines200ResponseAllOf.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = ListPipelines200ResponseAllOf.parse_obj({
-            "data": [Pipeline.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = cls.model_validate({
+            "api_key": obj.get("api_key")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/measurement.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/measurement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,102 +1,119 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Any, Dict, Optional, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
+from datetime import datetime
+from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
+from typing import Optional, Set
+from typing_extensions import Self
 
 class Measurement(BaseModel):
     """
     Measurement
-    """
-    uplink_message_id: StrictStr = Field(...)
-    device_id: Union[StrictFloat, StrictInt] = Field(...)
-    device_code: StrictStr = Field(...)
+    """ # noqa: E501
+    uplink_message_id: StrictStr
+    device_id: StrictInt
+    device_code: StrictStr
     device_description: Optional[StrictStr] = None
     device_latitude: Optional[Union[StrictFloat, StrictInt]] = None
     device_longitude: Optional[Union[StrictFloat, StrictInt]] = None
     device_altitude: Optional[Union[StrictFloat, StrictInt]] = None
     device_location_description: Optional[StrictStr] = None
     device_properties: Optional[Dict[str, Any]] = None
-    device_state: Union[StrictFloat, StrictInt] = Field(...)
-    sensor_id: Union[StrictFloat, StrictInt] = Field(...)
-    sensor_code: StrictStr = Field(...)
+    device_state: StrictInt
+    sensor_id: StrictInt
+    sensor_code: StrictStr
     sensor_description: Optional[StrictStr] = None
-    sensor_external_id: StrictStr = Field(...)
+    sensor_external_id: StrictStr
     sensor_properties: Optional[Dict[str, Any]] = None
     sensor_brand: Optional[StrictStr] = None
-    sensor_archive_time: Optional[Union[StrictFloat, StrictInt]] = None
-    datastream_id: StrictStr = Field(...)
+    sensor_archive_time: Optional[StrictInt] = None
+    datastream_id: StrictStr
     datastream_description: Optional[StrictStr] = None
-    datastream_observed_property: StrictStr = Field(...)
-    datastream_unit_of_measurement: StrictStr = Field(...)
-    measurement_timestamp: StrictStr = Field(...)
-    measurement_value: Union[StrictFloat, StrictInt] = Field(...)
+    datastream_observed_property: StrictStr
+    datastream_unit_of_measurement: StrictStr
+    measurement_timestamp: datetime
+    measurement_value: Union[StrictFloat, StrictInt]
     measurement_latitude: Optional[Union[StrictFloat, StrictInt]] = None
     measurement_longitude: Optional[Union[StrictFloat, StrictInt]] = None
     measurement_altitude: Optional[Union[StrictFloat, StrictInt]] = None
     measurement_properties: Optional[Dict[str, Any]] = None
-    measurement_expiration: StrictStr = Field(...)
-    created_at: Optional[StrictStr] = None
-    __properties = ["uplink_message_id", "device_id", "device_code", "device_description", "device_latitude", "device_longitude", "device_altitude", "device_location_description", "device_properties", "device_state", "sensor_id", "sensor_code", "sensor_description", "sensor_external_id", "sensor_properties", "sensor_brand", "sensor_archive_time", "datastream_id", "datastream_description", "datastream_observed_property", "datastream_unit_of_measurement", "measurement_timestamp", "measurement_value", "measurement_latitude", "measurement_longitude", "measurement_altitude", "measurement_properties", "measurement_expiration", "created_at"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    measurement_expiration: datetime
+    created_at: Optional[datetime] = None
+    __properties: ClassVar[List[str]] = ["uplink_message_id", "device_id", "device_code", "device_description", "device_latitude", "device_longitude", "device_altitude", "device_location_description", "device_properties", "device_state", "sensor_id", "sensor_code", "sensor_description", "sensor_external_id", "sensor_properties", "sensor_brand", "sensor_archive_time", "datastream_id", "datastream_description", "datastream_observed_property", "datastream_unit_of_measurement", "measurement_timestamp", "measurement_value", "measurement_latitude", "measurement_longitude", "measurement_altitude", "measurement_properties", "measurement_expiration", "created_at"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Measurement:
+    def from_json(cls, json_str: str) -> Optional[Self]:
         """Create an instance of Measurement from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Measurement:
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of Measurement from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Measurement.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = Measurement.parse_obj({
+        _obj = cls.model_validate({
             "uplink_message_id": obj.get("uplink_message_id"),
             "device_id": obj.get("device_id"),
             "device_code": obj.get("device_code"),
             "device_description": obj.get("device_description"),
             "device_latitude": obj.get("device_latitude"),
             "device_longitude": obj.get("device_longitude"),
             "device_altitude": obj.get("device_altitude"),
@@ -121,7 +138,8 @@
             "measurement_altitude": obj.get("measurement_altitude"),
             "measurement_properties": obj.get("measurement_properties"),
             "measurement_expiration": obj.get("measurement_expiration"),
             "created_at": obj.get("created_at")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/paginated_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/sensor_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,94 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, List
-from pydantic import BaseModel, Field, StrictInt, conlist
-from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
-
-class PaginatedResponse(BaseModel):
+class SensorGroup(BaseModel):
     """
-    PaginatedResponse
-    """
-    links: PaginatedResponseLinks = Field(...)
-    page_size: StrictInt = Field(...)
-    total_count: StrictInt = Field(...)
-    data: conlist(Any) = Field(...)
-    __properties = ["links", "page_size", "total_count", "data"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    SensorGroup
+    """ # noqa: E501
+    id: StrictInt
+    name: StrictStr
+    description: StrictStr
+    sensors: List[StrictInt]
+    __properties: ClassVar[List[str]] = ["id", "name", "description", "sensors"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PaginatedResponse:
-        """Create an instance of PaginatedResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of SensorGroup from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of links
-        if self.links:
-            _dict['links'] = self.links.to_dict()
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PaginatedResponse:
-        """Create an instance of PaginatedResponse from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of SensorGroup from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PaginatedResponse.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = PaginatedResponse.parse_obj({
-            "links": PaginatedResponseLinks.from_dict(obj.get("links")) if obj.get("links") is not None else None,
-            "page_size": obj.get("page_size"),
-            "total_count": obj.get("total_count"),
-            "data": obj.get("data")
+        _obj = cls.model_validate({
+            "id": obj.get("id"),
+            "name": obj.get("name"),
+            "description": obj.get("description"),
+            "sensors": obj.get("sensors")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/paginated_response_links.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/update_tenant_member_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,88 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
 from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List
+from typing import Optional, Set
+from typing_extensions import Self
 
-class PaginatedResponseLinks(BaseModel):
+class UpdateTenantMemberRequest(BaseModel):
     """
-    PaginatedResponseLinks
-    """
-    previous: Optional[StrictStr] = None
-    next: Optional[StrictStr] = None
-    __properties = ["previous", "next"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    UpdateTenantMemberRequest
+    """ # noqa: E501
+    permissions: List[StrictStr]
+    __properties: ClassVar[List[str]] = ["permissions"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PaginatedResponseLinks:
-        """Create an instance of PaginatedResponseLinks from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of UpdateTenantMemberRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PaginatedResponseLinks:
-        """Create an instance of PaginatedResponseLinks from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of UpdateTenantMemberRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PaginatedResponseLinks.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = PaginatedResponseLinks.parse_obj({
-            "previous": obj.get("previous"),
-            "next": obj.get("next")
+        _obj = cls.model_validate({
+            "permissions": obj.get("permissions")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/pipeline.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/tenant.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,100 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List, Optional
-from pydantic import BaseModel, StrictStr, conlist
-
-class Pipeline(BaseModel):
+class Tenant(BaseModel):
     """
-    Pipeline
-    """
-    id: Optional[StrictStr] = None
-    description: Optional[StrictStr] = None
-    steps: Optional[conlist(StrictStr)] = None
-    status: Optional[StrictStr] = None
-    last_status_change: Optional[StrictStr] = None
-    created_at: Optional[StrictStr] = None
-    __properties = ["id", "description", "steps", "status", "last_status_change", "created_at"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    Tenant
+    """ # noqa: E501
+    id: StrictInt
+    name: StrictStr
+    address: StrictStr
+    zip_code: StrictStr
+    city: StrictStr
+    chamber_of_commerce_id: Optional[StrictStr] = None
+    headquarter_id: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "address", "zip_code", "city", "chamber_of_commerce_id", "headquarter_id"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Pipeline:
-        """Create an instance of Pipeline from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of Tenant from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Pipeline:
-        """Create an instance of Pipeline from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of Tenant from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Pipeline.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = Pipeline.parse_obj({
+        _obj = cls.model_validate({
             "id": obj.get("id"),
-            "description": obj.get("description"),
-            "steps": obj.get("steps"),
-            "status": obj.get("status"),
-            "last_status_change": obj.get("last_status_change"),
-            "created_at": obj.get("created_at")
+            "name": obj.get("name"),
+            "address": obj.get("address"),
+            "zip_code": obj.get("zip_code"),
+            "city": obj.get("city"),
+            "chamber_of_commerce_id": obj.get("chamber_of_commerce_id"),
+            "headquarter_id": obj.get("headquarter_id")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/query_measurements200_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,106 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import List
-from pydantic import BaseModel, Field, StrictInt, conlist
+from pydantic import BaseModel, StrictInt
+from typing import Any, ClassVar, Dict, List
 from sensorbucket.models.measurement import Measurement
 from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
+from typing import Optional, Set
+from typing_extensions import Self
 
 class QueryMeasurements200Response(BaseModel):
     """
     QueryMeasurements200Response
-    """
-    links: PaginatedResponseLinks = Field(...)
-    page_size: StrictInt = Field(...)
-    total_count: StrictInt = Field(...)
-    data: conlist(Measurement) = Field(...)
-    __properties = ["links", "page_size", "total_count", "data"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    """ # noqa: E501
+    links: PaginatedResponseLinks
+    page_size: StrictInt
+    total_count: StrictInt
+    data: List[Measurement]
+    __properties: ClassVar[List[str]] = ["links", "page_size", "total_count", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QueryMeasurements200Response:
+    def from_json(cls, json_str: str) -> Optional[Self]:
         """Create an instance of QueryMeasurements200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         # override the default output from pydantic by calling `to_dict()` of links
         if self.links:
             _dict['links'] = self.links.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in data (list)
         _items = []
         if self.data:
             for _item in self.data:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QueryMeasurements200Response:
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of QueryMeasurements200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return QueryMeasurements200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = QueryMeasurements200Response.parse_obj({
-            "links": PaginatedResponseLinks.from_dict(obj.get("links")) if obj.get("links") is not None else None,
+        _obj = cls.model_validate({
+            "links": PaginatedResponseLinks.from_dict(obj["links"]) if obj.get("links") is not None else None,
             "page_size": obj.get("page_size"),
             "total_count": obj.get("total_count"),
-            "data": [Measurement.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+            "data": [Measurement.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response_all_of.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/create_api_key_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,95 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from datetime import datetime
+from pydantic import BaseModel, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import List, Optional
-from pydantic import BaseModel, conlist
-from sensorbucket.models.measurement import Measurement
-
-class QueryMeasurements200ResponseAllOf(BaseModel):
-    """
-    QueryMeasurements200ResponseAllOf
+class CreateApiKeyRequest(BaseModel):
     """
-    data: Optional[conlist(Measurement)] = None
-    __properties = ["data"]
+    CreateApiKeyRequest
+    """ # noqa: E501
+    name: StrictStr
+    tenant_id: StrictInt
+    permissions: Optional[List[StrictStr]] = None
+    expiration_date: Optional[datetime] = None
+    __properties: ClassVar[List[str]] = ["name", "tenant_id", "permissions", "expiration_date"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QueryMeasurements200ResponseAllOf:
-        """Create an instance of QueryMeasurements200ResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreateApiKeyRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
-        if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QueryMeasurements200ResponseAllOf:
-        """Create an instance of QueryMeasurements200ResponseAllOf from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreateApiKeyRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return QueryMeasurements200ResponseAllOf.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = QueryMeasurements200ResponseAllOf.parse_obj({
-            "data": [Measurement.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = cls.model_validate({
+            "name": obj.get("name"),
+            "tenant_id": obj.get("tenant_id"),
+            "permissions": obj.get("permissions"),
+            "expiration_date": obj.get("expiration_date")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/sensor.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/delete_sensor_group200_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,88 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, Dict, Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-
-class Sensor(BaseModel):
+class DeleteSensorGroup200Response(BaseModel):
     """
-    Sensor
-    """
-    id: Optional[Union[StrictFloat, StrictInt]] = None
-    code: Optional[StrictStr] = None
-    description: Optional[StrictStr] = None
-    external_id: Optional[StrictStr] = None
-    brand: Optional[StrictStr] = None
-    archive_time: Optional[Union[StrictFloat, StrictInt]] = None
-    properties: Optional[Dict[str, Any]] = None
-    created_at: Optional[StrictStr] = None
-    __properties = ["id", "code", "description", "external_id", "brand", "archive_time", "properties", "created_at"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    DeleteSensorGroup200Response
+    """ # noqa: E501
+    message: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Sensor:
-        """Create an instance of Sensor from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of DeleteSensorGroup200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Sensor:
-        """Create an instance of Sensor from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of DeleteSensorGroup200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Sensor.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = Sensor.parse_obj({
-            "id": obj.get("id"),
-            "code": obj.get("code"),
-            "description": obj.get("description"),
-            "external_id": obj.get("external_id"),
-            "brand": obj.get("brand"),
-            "archive_time": obj.get("archive_time"),
-            "properties": obj.get("properties"),
-            "created_at": obj.get("created_at")
+        _obj = cls.model_validate({
+            "message": obj.get("message")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/update_device200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/remove_tenant_member200_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,88 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
 from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-class UpdateDevice200Response(BaseModel):
-    """
-    UpdateDevice200Response
+class RemoveTenantMember200Response(BaseModel):
     """
+    RemoveTenantMember200Response
+    """ # noqa: E501
     message: Optional[StrictStr] = None
-    __properties = ["message"]
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateDevice200Response:
-        """Create an instance of UpdateDevice200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of RemoveTenantMember200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateDevice200Response:
-        """Create an instance of UpdateDevice200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of RemoveTenantMember200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdateDevice200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = UpdateDevice200Response.parse_obj({
+        _obj = cls.model_validate({
             "message": obj.get("message")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/update_device_request.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/update_worker_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,104 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
+from pydantic import BaseModel, Field, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
+from typing import Optional, Set
+from typing_extensions import Self
 
-from typing import Any, Dict, Optional, Union
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-
-class UpdateDeviceRequest(BaseModel):
+class UpdateWorkerRequest(BaseModel):
     """
-    UpdateDeviceRequest
-    """
-    description: Optional[Union[StrictFloat, StrictInt]] = None
-    latitude: Optional[Union[StrictFloat, StrictInt]] = None
-    longitude: Optional[Union[StrictFloat, StrictInt]] = None
-    location_description: Optional[StrictStr] = None
-    properties: Optional[Dict[str, Any]] = None
-    __properties = ["description", "latitude", "longitude", "location_description", "properties"]
-
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
+    UpdateWorkerRequest
+    """ # noqa: E501
+    name: Optional[StrictStr] = None
+    description: Optional[StrictStr] = None
+    state: Optional[StrictStr] = None
+    user_code: Optional[StrictStr] = Field(default=None, description="base64 encoded user code")
+    __properties: ClassVar[List[str]] = ["name", "description", "state", "user_code"]
+
+    @field_validator('state')
+    def state_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('enabled', 'disabled'):
+            raise ValueError("must be one of enum values ('enabled', 'disabled')")
+        return value
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
+
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateDeviceRequest:
-        """Create an instance of UpdateDeviceRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of UpdateWorkerRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateDeviceRequest:
-        """Create an instance of UpdateDeviceRequest from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of UpdateWorkerRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdateDeviceRequest.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = UpdateDeviceRequest.parse_obj({
+        _obj = cls.model_validate({
+            "name": obj.get("name"),
             "description": obj.get("description"),
-            "latitude": obj.get("latitude"),
-            "longitude": obj.get("longitude"),
-            "location_description": obj.get("location_description"),
-            "properties": obj.get("properties")
+            "state": obj.get("state"),
+            "user_code": obj.get("user_code")
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket/models/update_pipeline200_response.py` & `sensorbucket-1.2.0rc1/sensorbucket/models/create_pipeline200_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,94 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import Optional
 from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from sensorbucket.models.pipeline import Pipeline
+from typing import Optional, Set
+from typing_extensions import Self
 
-class UpdatePipeline200Response(BaseModel):
-    """
-    UpdatePipeline200Response
+class CreatePipeline200Response(BaseModel):
     """
+    CreatePipeline200Response
+    """ # noqa: E501
     message: Optional[StrictStr] = None
     data: Optional[Pipeline] = None
-    __properties = ["message", "data"]
+    __properties: ClassVar[List[str]] = ["message", "data"]
+
+    model_config = {
+        "populate_by_name": True,
+        "validate_assignment": True,
+        "protected_namespaces": (),
+    }
 
-    class Config:
-        """Pydantic configuration"""
-        allow_population_by_field_name = True
-        validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
+        return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
+        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdatePipeline200Response:
-        """Create an instance of UpdatePipeline200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> Optional[Self]:
+        """Create an instance of CreatePipeline200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True,
-                          exclude={
-                          },
-                          exclude_none=True)
+    def to_dict(self) -> Dict[str, Any]:
+        """Return the dictionary representation of the model using alias.
+
+        This has the following differences from calling pydantic's
+        `self.model_dump(by_alias=True)`:
+
+        * `None` is only added to the output dict for nullable fields that
+          were set at model initialization. Other fields with value `None`
+          are ignored.
+        """
+        excluded_fields: Set[str] = set([
+        ])
+
+        _dict = self.model_dump(
+            by_alias=True,
+            exclude=excluded_fields,
+            exclude_none=True,
+        )
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdatePipeline200Response:
-        """Create an instance of UpdatePipeline200Response from a dict"""
+    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
+        """Create an instance of CreatePipeline200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdatePipeline200Response.parse_obj(obj)
+            return cls.model_validate(obj)
 
-        _obj = UpdatePipeline200Response.parse_obj({
+        _obj = cls.model_validate({
             "message": obj.get("message"),
-            "data": Pipeline.from_dict(obj.get("data")) if obj.get("data") is not None else None
+            "data": Pipeline.from_dict(obj["data"]) if obj.get("data") is not None else None
         })
         return _obj
 
+
```

### Comparing `sensorbucket-1.0.1/sensorbucket.egg-info/PKG-INFO` & `sensorbucket-1.2.0rc1/sensorbucket.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: sensorbucket
-Version: 1.0.1
+Version: 1.2.0rc1
 Summary: Sensorbucket API
 Home-page: https://sensorbucket.nl
 Author: Tim van Osch
 Author-email: info@pollex.nl
 License: EUPLv1.2
 Keywords: OpenAPI,OpenAPI-Generator,Sensorbucket API
 Description-Content-Type: text/markdown
+Requires-Dist: urllib3<2.1.0,>=1.25.3
+Requires-Dist: python-dateutil
+Requires-Dist: pydantic>=2
+Requires-Dist: typing-extensions>=4.7.1
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex&#39;
```

### Comparing `sensorbucket-1.0.1/setup.py` & `sensorbucket-1.2.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
     Sensorbucket API
 
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex' 
 
-    The version of the OpenAPI document: 1.0
+    The version of the OpenAPI document: 1.2.0-rc1
     Contact: info@pollex.nl
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
-"""
+"""  # noqa: E501
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "sensorbucket"
-VERSION = "1.0.1"
+VERSION = "1.2.0-rc1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
-    "urllib3 >= 1.25.3",
+    "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
-    "pydantic >= 1.10.5, < 2",
-    "aenum"
+    "pydantic >= 2",
+    "typing-extensions >= 4.7.1",
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Sensorbucket API",
     author="Tim van Osch",
@@ -41,10 +41,11 @@
     keywords=["OpenAPI", "OpenAPI-Generator", "Sensorbucket API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     license="EUPLv1.2",
     long_description_content_type='text/markdown',
     long_description="""\
-    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex   # noqa: E501
-    """
+    SensorBucket processes data from different sources and devices into a single standardized format.  An applications connected to SensorBucket, can use all devices SensorBucket supports.  Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker that receives data from an AMQP source, process said data and output in the expected worker output format.  Find out more at: https://developer.sensorbucket.nl/  Developed and designed by Provincie Zeeland and Pollex&#39; 
+    """,  # noqa: E501
+    package_data={"sensorbucket": ["py.typed"]},
 )
```

