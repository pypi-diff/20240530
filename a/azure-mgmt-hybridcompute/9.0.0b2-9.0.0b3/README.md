# Comparing `tmp/azure-mgmt-hybridcompute-9.0.0b2.tar.gz` & `tmp/azure-mgmt-hybridcompute-9.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-hybridcompute-9.0.0b2.tar", last modified: Wed Apr 24 04:41:19 2024, max compression
+gzip compressed data, was "azure-mgmt-hybridcompute-9.0.0b3.tar", last modified: Thu May 30 07:14:05 2024, max compression
```

## Comparing `azure-mgmt-hybridcompute-9.0.0b2.tar` & `azure-mgmt-hybridcompute-9.0.0b3.tar`

### file list

```diff
@@ -1,70 +1,78 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15626 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      219 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18574 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2045 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      636 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      928 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3461 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8017 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_hybrid_compute_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1347 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.077571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3509 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8229 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.081571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1778 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9159 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10447 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33666 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24342 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machine_run_commands_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29433 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4617 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5639 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24188 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9146 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35542 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.081571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11969 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10220 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   215695 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1778 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11883 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11974 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41526 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30384 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37220 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machines_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6068 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_network_profile_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6322 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30433 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11925 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46177 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18574 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2878 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-24 04:41:18.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-24 04:41:19.000000 azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-24 04:41:19.089571 azure-mgmt-hybridcompute-9.0.0b2/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2780 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-24 04:41:19.085571 azure-mgmt-hybridcompute-9.0.0b2/tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/tests/conftest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1711 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/tests/disable_test_hybridcompute.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      977 2024-04-24 04:39:52.000000 azure-mgmt-hybridcompute-9.0.0b2/tests/test_mgmt_hybridcompute.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.786925 azure-mgmt-hybridcompute-9.0.0b3/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16012 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      219 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18960 2024-05-30 07:14:05.786925 azure-mgmt-hybridcompute-9.0.0b3/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2045 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      640 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.774925 azure-mgmt-hybridcompute-9.0.0b3/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.774925 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.778925 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      928 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3461 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9304 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_hybrid_compute_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1347 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.778925 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      875 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3509 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9532 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.782925 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2187 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9443 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31647 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_gateways_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10686 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33274 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_licenses_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34088 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34389 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_machine_run_commands_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29901 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4855 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9846 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_network_security_perimeter_configurations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5877 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24564 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9430 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36102 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19503 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_settings_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.782925 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12859 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10736 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   232961 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.786925 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2187 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12167 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39431 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_gateways_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12213 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40934 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_licenses_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41948 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42093 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37688 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_machines_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6306 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_network_profile_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12790 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_network_security_perimeter_configurations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6560 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30809 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12209 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    46737 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25931 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_settings_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.786925 azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18960 2024-05-30 07:14:05.000000 azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3440 2024-05-30 07:14:05.000000 azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-30 07:14:05.000000 azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-30 07:14:05.000000 azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-05-30 07:14:05.000000 azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-30 07:14:05.000000 azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-30 07:14:05.786925 azure-mgmt-hybridcompute-9.0.0b3/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2780 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-30 07:14:05.786925 azure-mgmt-hybridcompute-9.0.0b3/tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2616 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/tests/conftest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1711 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/tests/disable_test_hybridcompute.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      977 2024-05-30 07:12:14.000000 azure-mgmt-hybridcompute-9.0.0b3/tests/test_mgmt_hybridcompute.py
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/CHANGELOG.md` & `azure-mgmt-hybridcompute-9.0.0b3/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Release History
 
+## 9.0.0b3 (2024-05-30)
+
+### Features Added
+
+  - Added operation MachineRunCommandsOperations.begin_update
+  - Added operation group GatewaysOperations
+  - Added operation group LicensesOperations
+  - Added operation group NetworkSecurityPerimeterConfigurationsOperations
+  - Added operation group SettingsOperations
+  - Model LicenseDetails has a new parameter volume_license_details
+
 ## 9.0.0b2 (2024-04-22)
 
 ### Features Added
 
   - Added operation group MachineRunCommandsOperations
   - Model LicenseProfile has a new parameter billing_start_date
   - Model LicenseProfile has a new parameter disenrollment_date
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/LICENSE` & `azure-mgmt-hybridcompute-9.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/PKG-INFO` & `azure-mgmt-hybridcompute-9.0.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-hybridcompute
-Version: 9.0.0b2
+Version: 9.0.0b3
 Summary: Microsoft Azure Hybrid Compute Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,25 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 9.0.0b3 (2024-05-30)
+
+### Features Added
+
+  - Added operation MachineRunCommandsOperations.begin_update
+  - Added operation group GatewaysOperations
+  - Added operation group LicensesOperations
+  - Added operation group NetworkSecurityPerimeterConfigurationsOperations
+  - Added operation group SettingsOperations
+  - Model LicenseDetails has a new parameter volume_license_details
+
 ## 9.0.0b2 (2024-04-22)
 
 ### Features Added
 
   - Added operation group MachineRunCommandsOperations
   - Model LicenseProfile has a new parameter billing_start_date
   - Model LicenseProfile has a new parameter disenrollment_date
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/README.md` & `azure-mgmt-hybridcompute-9.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/_meta.json` & `azure-mgmt-hybridcompute-9.0.0b3/_meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6944444444444443%*

 * *Differences: {"'autorest'": "'3.10.2'",*

 * * "'autorest_command'": "'autorest specification/hybridcompute/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.16 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.10.2 --version-tolerant=False'",*

 * * "'commit'": "'34f8f3fa251276229e64680c29a […]*

```diff
@@ -1,11 +1,11 @@
 {
-    "autorest": "3.9.7",
-    "autorest_command": "autorest specification/hybridcompute/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
-    "commit": "71a0c7adf2a6e169ab9a33c7cf36bb93db083e86",
+    "autorest": "3.10.2",
+    "autorest_command": "autorest specification/hybridcompute/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.16 --use=@autorest/modelerfour@4.27.0 --version=3.10.2 --version-tolerant=False",
+    "commit": "34f8f3fa251276229e64680c29abe1d194559661",
     "readme": "specification/hybridcompute/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.13.7",
+        "@autorest/python@6.13.16",
         "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_configuration.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
+from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
-from ._version import VERSION
+from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials import TokenCredential
+    from azure.core.credentials_async import AsyncTokenCredential
 
 
 class HybridComputeManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HybridComputeManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials.TokenCredential
+    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-10-03-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-03-31-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2023-10-03-preview")
+    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        api_version: str = kwargs.pop("api_version", "2024-03-31-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,14 +52,14 @@
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = ARMChallengeAuthenticationPolicy(
+            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_serialization.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/_vendor.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_configuration.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.pipeline import policies
-from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
+from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
-from .._version import VERSION
+from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
-    from azure.core.credentials_async import AsyncTokenCredential
+    from azure.core.credentials import TokenCredential
 
 
 class HybridComputeManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for HybridComputeManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
-    :type credential: ~azure.core.credentials_async.AsyncTokenCredential
+    :type credential: ~azure.core.credentials.TokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-10-03-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-03-31-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        api_version: str = kwargs.pop("api_version", "2023-10-03-preview")
+    def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
+        api_version: str = kwargs.pop("api_version", "2024-03-31-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
@@ -52,14 +52,14 @@
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
-            self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
+            self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,35 +15,41 @@
 from azure.mgmt.core.policies import AsyncARMAutoResourceProviderRegistrationPolicy
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import HybridComputeManagementClientConfiguration
 from .operations import (
     ExtensionMetadataOperations,
+    GatewaysOperations,
     HybridComputeManagementClientOperationsMixin,
+    LicensesOperations,
     MachineExtensionsOperations,
     MachineRunCommandsOperations,
     MachinesOperations,
     NetworkProfileOperations,
+    NetworkSecurityPerimeterConfigurationsOperations,
     Operations,
     PrivateEndpointConnectionsOperations,
     PrivateLinkResourcesOperations,
     PrivateLinkScopesOperations,
+    SettingsOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class HybridComputeManagementClient(
     HybridComputeManagementClientOperationsMixin
 ):  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """The Hybrid Compute Management Client.
 
+    :ivar licenses: LicensesOperations operations
+    :vartype licenses: azure.mgmt.hybridcompute.aio.operations.LicensesOperations
     :ivar machines: MachinesOperations operations
     :vartype machines: azure.mgmt.hybridcompute.aio.operations.MachinesOperations
     :ivar machine_extensions: MachineExtensionsOperations operations
     :vartype machine_extensions:
      azure.mgmt.hybridcompute.aio.operations.MachineExtensionsOperations
     :ivar extension_metadata: ExtensionMetadataOperations operations
     :vartype extension_metadata:
@@ -51,30 +57,38 @@
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.hybridcompute.aio.operations.Operations
     :ivar network_profile: NetworkProfileOperations operations
     :vartype network_profile: azure.mgmt.hybridcompute.aio.operations.NetworkProfileOperations
     :ivar machine_run_commands: MachineRunCommandsOperations operations
     :vartype machine_run_commands:
      azure.mgmt.hybridcompute.aio.operations.MachineRunCommandsOperations
+    :ivar gateways: GatewaysOperations operations
+    :vartype gateways: azure.mgmt.hybridcompute.aio.operations.GatewaysOperations
+    :ivar settings: SettingsOperations operations
+    :vartype settings: azure.mgmt.hybridcompute.aio.operations.SettingsOperations
     :ivar private_link_scopes: PrivateLinkScopesOperations operations
     :vartype private_link_scopes:
      azure.mgmt.hybridcompute.aio.operations.PrivateLinkScopesOperations
     :ivar private_link_resources: PrivateLinkResourcesOperations operations
     :vartype private_link_resources:
      azure.mgmt.hybridcompute.aio.operations.PrivateLinkResourcesOperations
     :ivar private_endpoint_connections: PrivateEndpointConnectionsOperations operations
     :vartype private_endpoint_connections:
      azure.mgmt.hybridcompute.aio.operations.PrivateEndpointConnectionsOperations
+    :ivar network_security_perimeter_configurations:
+     NetworkSecurityPerimeterConfigurationsOperations operations
+    :vartype network_security_perimeter_configurations:
+     azure.mgmt.hybridcompute.aio.operations.NetworkSecurityPerimeterConfigurationsOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :param subscription_id: The ID of the target subscription. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-10-03-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2024-03-31-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
      Retry-After header is present.
     """
 
     def __init__(
@@ -107,35 +121,41 @@
             ]
         self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
+        self.licenses = LicensesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machines = MachinesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machine_extensions = MachineExtensionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.extension_metadata = ExtensionMetadataOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.network_profile = NetworkProfileOperations(self._client, self._config, self._serialize, self._deserialize)
         self.machine_run_commands = MachineRunCommandsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.gateways = GatewaysOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.settings = SettingsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.private_link_scopes = PrivateLinkScopesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.private_link_resources = PrivateLinkResourcesOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.private_endpoint_connections = PrivateEndpointConnectionsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
+        self.network_security_perimeter_configurations = NetworkSecurityPerimeterConfigurationsOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
 
     def _send_request(
         self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
     ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/_vendor.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,44 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._licenses_operations import LicensesOperations
 from ._machines_operations import MachinesOperations
 from ._machine_extensions_operations import MachineExtensionsOperations
 from ._hybrid_compute_management_client_operations import HybridComputeManagementClientOperationsMixin
 from ._extension_metadata_operations import ExtensionMetadataOperations
 from ._operations import Operations
 from ._network_profile_operations import NetworkProfileOperations
 from ._machine_run_commands_operations import MachineRunCommandsOperations
+from ._gateways_operations import GatewaysOperations
+from ._settings_operations import SettingsOperations
 from ._private_link_scopes_operations import PrivateLinkScopesOperations
 from ._private_link_resources_operations import PrivateLinkResourcesOperations
 from ._private_endpoint_connections_operations import PrivateEndpointConnectionsOperations
+from ._network_security_perimeter_configurations_operations import NetworkSecurityPerimeterConfigurationsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "LicensesOperations",
     "MachinesOperations",
     "MachineExtensionsOperations",
     "HybridComputeManagementClientOperationsMixin",
     "ExtensionMetadataOperations",
     "Operations",
     "NetworkProfileOperations",
     "MachineRunCommandsOperations",
+    "GatewaysOperations",
+    "SettingsOperations",
     "PrivateLinkScopesOperations",
     "PrivateLinkResourcesOperations",
     "PrivateEndpointConnectionsOperations",
+    "NetworkSecurityPerimeterConfigurationsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -27,14 +28,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._extension_metadata_operations import build_get_request, build_list_request
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class ExtensionMetadataOperations:
     """
     .. warning::
@@ -68,15 +73,15 @@
         :type extension_type: str
         :param version: The version of the Extension being received. Required.
         :type version: str
         :return: ExtensionValue or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.ExtensionValue
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -137,15 +142,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ExtensionValueListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -27,29 +28,34 @@
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._hybrid_compute_management_client_operations import build_upgrade_extensions_request
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class HybridComputeManagementClientOperationsMixin(  # pylint: disable=name-too-long
     HybridComputeManagementClientMixinABC
 ):
+
     async def _upgrade_extensions_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         machine_name: str,
         extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO[bytes]],
         **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -36,14 +37,18 @@
     build_delete_request,
     build_get_request,
     build_list_request,
     build_update_request,
 )
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MachineExtensionsOperations:
     """
     .. warning::
@@ -67,15 +72,15 @@
         self,
         resource_group_name: str,
         machine_name: str,
         extension_name: str,
         extension_parameters: Union[_models.MachineExtension, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.MachineExtension]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -274,15 +279,15 @@
         self,
         resource_group_name: str,
         machine_name: str,
         extension_name: str,
         extension_parameters: Union[_models.MachineExtensionUpdate, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.MachineExtension]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -485,15 +490,15 @@
         return AsyncLROPoller[_models.MachineExtension](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -608,15 +613,15 @@
         :type machine_name: str
         :param extension_name: The name of the machine extension. Required.
         :type extension_name: str
         :return: MachineExtension or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.MachineExtension
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -677,15 +682,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineExtensionsListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machine_run_commands_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_machine_run_commands_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -32,17 +33,22 @@
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._machine_run_commands_operations import (
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_request,
+    build_update_request,
 )
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MachineRunCommandsOperations:
     """
     .. warning::
@@ -66,15 +72,15 @@
         self,
         resource_group_name: str,
         machine_name: str,
         run_command_name: str,
         run_command_properties: Union[_models.MachineRunCommand, IO[bytes]],
         **kwargs: Any
     ) -> _models.MachineRunCommand:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -272,18 +278,229 @@
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return AsyncLROPoller[_models.MachineRunCommand](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
+    async def _update_initial(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: Union[_models.MachineRunCommandUpdate, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.MachineRunCommand]:
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.MachineRunCommand]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(run_command_properties, (IOBase, bytes)):
+            _content = run_command_properties
+        else:
+            _json = self._serialize.body(run_command_properties, "MachineRunCommandUpdate")
+
+        _request = build_update_request(
+            resource_group_name=resource_group_name,
+            machine_name=machine_name,
+            run_command_name=run_command_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("MachineRunCommand", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: _models.MachineRunCommandUpdate,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.MachineRunCommand]:
+        """The operation to update the run command.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Required.
+        :type run_command_properties: ~azure.mgmt.hybridcompute.models.MachineRunCommandUpdate
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.MachineRunCommand]:
+        """The operation to update the run command.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Required.
+        :type run_command_properties: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of AsyncLROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def begin_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: Union[_models.MachineRunCommandUpdate, IO[bytes]],
+        **kwargs: Any
+    ) -> AsyncLROPoller[_models.MachineRunCommand]:
+        """The operation to update the run command.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Is either a
+         MachineRunCommandUpdate type or a IO[bytes] type. Required.
+        :type run_command_properties: ~azure.mgmt.hybridcompute.models.MachineRunCommandUpdate or
+         IO[bytes]
+        :return: An instance of AsyncLROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MachineRunCommand] = kwargs.pop("cls", None)
+        polling: Union[bool, AsyncPollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = await self._update_initial(
+                resource_group_name=resource_group_name,
+                machine_name=machine_name,
+                run_command_name=run_command_name,
+                run_command_properties=run_command_properties,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("MachineRunCommand", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
+
+        if polling is True:
+            polling_method: AsyncPollingMethod = cast(AsyncPollingMethod, AsyncARMPolling(lro_delay, **kwargs))
+        elif polling is False:
+            polling_method = cast(AsyncPollingMethod, AsyncNoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return AsyncLROPoller[_models.MachineRunCommand].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return AsyncLROPoller[_models.MachineRunCommand](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
+
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, machine_name: str, run_command_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -400,15 +617,15 @@
         :type machine_name: str
         :param run_command_name: The name of the run command. Required.
         :type run_command_name: str
         :return: MachineRunCommand or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.MachineRunCommand
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -469,15 +686,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineRunCommandsListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_machines_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -37,14 +38,18 @@
     build_get_request,
     build_install_patches_request,
     build_list_by_resource_group_request,
     build_list_by_subscription_request,
 )
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class MachinesOperations:
     """
     .. warning::
@@ -75,15 +80,15 @@
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -132,15 +137,15 @@
         :type machine_name: str
         :param expand: The expand expression to apply on the operation. Default value is None.
         :type expand: str
         :return: Machine or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.Machine
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -180,15 +185,15 @@
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     async def _assess_patches_initial(
         self, resource_group_name: str, name: str, **kwargs: Any
     ) -> Optional[_models.MachineAssessPatchesResult]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -298,15 +303,15 @@
     async def _install_patches_initial(
         self,
         resource_group_name: str,
         name: str,
         install_patches_input: Union[_models.MachineInstallPatchesParameters, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.MachineInstallPatchesResult]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -512,15 +517,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -592,15 +597,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -24,14 +25,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._network_profile_operations import build_get_request
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class NetworkProfileOperations:
     """
     .. warning::
@@ -60,15 +65,15 @@
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
         :return: NetworkProfile or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.NetworkProfile
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -26,14 +27,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._operations import build_list_request
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class Operations:
     """
     .. warning::
@@ -64,15 +69,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -35,14 +36,18 @@
     build_create_or_update_request,
     build_delete_request,
     build_get_request,
     build_list_by_private_link_scope_request,
 )
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class PrivateEndpointConnectionsOperations:
     """
     .. warning::
@@ -75,15 +80,15 @@
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -128,15 +133,15 @@
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
         parameters: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.PrivateEndpointConnection]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -327,15 +332,15 @@
         return AsyncLROPoller[_models.PrivateEndpointConnection](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -456,15 +461,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnectionListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -27,14 +28,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
 from ...operations._private_link_resources_operations import build_get_request, build_list_by_private_link_scope_request
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class PrivateLinkResourcesOperations:
     """
     .. warning::
@@ -72,15 +77,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -154,15 +159,15 @@
         :type scope_name: str
         :param group_name: The name of the private link resource. Required.
         :type group_name: str
         :return: PrivateLinkResource or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -39,14 +40,18 @@
     build_get_validation_details_request,
     build_list_by_resource_group_request,
     build_list_request,
     build_update_tags_request,
 )
 from .._vendor import HybridComputeManagementClientMixinABC
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class PrivateLinkScopesOperations:
     """
     .. warning::
@@ -78,15 +83,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.HybridComputePrivateLinkScopeListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -162,15 +167,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.HybridComputePrivateLinkScopeListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -229,15 +234,15 @@
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
     async def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -344,15 +349,15 @@
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -470,15 +475,15 @@
          Servers and Clusters PrivateLinkScope. Is either a HybridComputePrivateLinkScope type or a
          IO[bytes] type. Required.
         :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -611,15 +616,15 @@
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
          instance. Is either a TagsResource type or a IO[bytes] type. Required.
         :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -682,15 +687,15 @@
         :param private_link_scope_id: The id (Guid) of the Azure Arc PrivateLinkScope resource.
          Required.
         :type private_link_scope_id: str
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -742,15 +747,15 @@
         :param machine_name: The name of the target machine to get the private link scope validation
          details for. Required.
         :type machine_name: str
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,25 @@
 from ._models_py3 import AgentVersionsList
 from ._models_py3 import AvailablePatchCountByClassification
 from ._models_py3 import CloudMetadata
 from ._models_py3 import ConfigurationExtension
 from ._models_py3 import ConnectionDetail
 from ._models_py3 import ErrorAdditionalInfo
 from ._models_py3 import ErrorDetail
+from ._models_py3 import ErrorDetailAutoGenerated
 from ._models_py3 import ErrorResponse
+from ._models_py3 import ErrorResponseAutoGenerated
 from ._models_py3 import EsuKey
 from ._models_py3 import ExtensionTargetProperties
 from ._models_py3 import ExtensionValue
 from ._models_py3 import ExtensionValueListResult
 from ._models_py3 import ExtensionsResourceStatus
+from ._models_py3 import Gateway
+from ._models_py3 import GatewayUpdate
+from ._models_py3 import GatewaysListResult
 from ._models_py3 import HybridComputePrivateLinkScope
 from ._models_py3 import HybridComputePrivateLinkScopeListResult
 from ._models_py3 import HybridComputePrivateLinkScopeProperties
 from ._models_py3 import HybridIdentityMetadata
 from ._models_py3 import HybridIdentityMetadataList
 from ._models_py3 import Identity
 from ._models_py3 import IpAddress
@@ -88,38 +93,44 @@
 from ._models_py3 import PrivateLinkScopeValidationDetails
 from ._models_py3 import PrivateLinkScopesResource
 from ._models_py3 import PrivateLinkServiceConnectionStateProperty
 from ._models_py3 import ProductFeature
 from ._models_py3 import ProductFeatureUpdate
 from ._models_py3 import ProvisioningIssue
 from ._models_py3 import ProxyResource
+from ._models_py3 import ProxyResourceAutoGenerated
 from ._models_py3 import Resource
 from ._models_py3 import ResourceAssociation
+from ._models_py3 import ResourceAutoGenerated
 from ._models_py3 import ResourceUpdate
 from ._models_py3 import RunCommandInputParameter
 from ._models_py3 import RunCommandManagedIdentity
 from ._models_py3 import ServiceStatus
 from ._models_py3 import ServiceStatuses
+from ._models_py3 import Settings
 from ._models_py3 import Subnet
 from ._models_py3 import SystemData
 from ._models_py3 import TagsResource
 from ._models_py3 import TrackedResource
+from ._models_py3 import TrackedResourceAutoGenerated
+from ._models_py3 import VolumeLicenseDetails
 from ._models_py3 import WindowsParameters
 
 from ._hybrid_compute_management_client_enums import AccessMode
 from ._hybrid_compute_management_client_enums import AccessRuleDirection
 from ._hybrid_compute_management_client_enums import AgentConfigurationMode
 from ._hybrid_compute_management_client_enums import ArcKindEnum
 from ._hybrid_compute_management_client_enums import AssessmentModeTypes
 from ._hybrid_compute_management_client_enums import CreatedByType
 from ._hybrid_compute_management_client_enums import EsuEligibility
 from ._hybrid_compute_management_client_enums import EsuKeyState
 from ._hybrid_compute_management_client_enums import EsuServerType
 from ._hybrid_compute_management_client_enums import ExecutionState
 from ._hybrid_compute_management_client_enums import ExtensionsStatusLevelTypes
+from ._hybrid_compute_management_client_enums import GatewayType
 from ._hybrid_compute_management_client_enums import LastAttemptStatusEnum
 from ._hybrid_compute_management_client_enums import LicenseAssignmentState
 from ._hybrid_compute_management_client_enums import LicenseCoreType
 from ._hybrid_compute_management_client_enums import LicenseEdition
 from ._hybrid_compute_management_client_enums import LicenseProfileProductType
 from ._hybrid_compute_management_client_enums import LicenseProfileSubscriptionStatus
 from ._hybrid_compute_management_client_enums import LicenseProfileSubscriptionStatusUpdate
@@ -128,14 +139,15 @@
 from ._hybrid_compute_management_client_enums import LicenseTarget
 from ._hybrid_compute_management_client_enums import LicenseType
 from ._hybrid_compute_management_client_enums import OsType
 from ._hybrid_compute_management_client_enums import PatchModeTypes
 from ._hybrid_compute_management_client_enums import PatchOperationStartedBy
 from ._hybrid_compute_management_client_enums import PatchOperationStatus
 from ._hybrid_compute_management_client_enums import PatchServiceUsed
+from ._hybrid_compute_management_client_enums import ProgramYear
 from ._hybrid_compute_management_client_enums import ProvisioningIssueSeverity
 from ._hybrid_compute_management_client_enums import ProvisioningIssueType
 from ._hybrid_compute_management_client_enums import ProvisioningState
 from ._hybrid_compute_management_client_enums import PublicNetworkAccessType
 from ._hybrid_compute_management_client_enums import StatusLevelTypes
 from ._hybrid_compute_management_client_enums import StatusTypes
 from ._hybrid_compute_management_client_enums import VMGuestPatchClassificationLinux
@@ -154,20 +166,25 @@
     "AgentVersionsList",
     "AvailablePatchCountByClassification",
     "CloudMetadata",
     "ConfigurationExtension",
     "ConnectionDetail",
     "ErrorAdditionalInfo",
     "ErrorDetail",
+    "ErrorDetailAutoGenerated",
     "ErrorResponse",
+    "ErrorResponseAutoGenerated",
     "EsuKey",
     "ExtensionTargetProperties",
     "ExtensionValue",
     "ExtensionValueListResult",
     "ExtensionsResourceStatus",
+    "Gateway",
+    "GatewayUpdate",
+    "GatewaysListResult",
     "HybridComputePrivateLinkScope",
     "HybridComputePrivateLinkScopeListResult",
     "HybridComputePrivateLinkScopeProperties",
     "HybridIdentityMetadata",
     "HybridIdentityMetadataList",
     "Identity",
     "IpAddress",
@@ -229,37 +246,43 @@
     "PrivateLinkScopeValidationDetails",
     "PrivateLinkScopesResource",
     "PrivateLinkServiceConnectionStateProperty",
     "ProductFeature",
     "ProductFeatureUpdate",
     "ProvisioningIssue",
     "ProxyResource",
+    "ProxyResourceAutoGenerated",
     "Resource",
     "ResourceAssociation",
+    "ResourceAutoGenerated",
     "ResourceUpdate",
     "RunCommandInputParameter",
     "RunCommandManagedIdentity",
     "ServiceStatus",
     "ServiceStatuses",
+    "Settings",
     "Subnet",
     "SystemData",
     "TagsResource",
     "TrackedResource",
+    "TrackedResourceAutoGenerated",
+    "VolumeLicenseDetails",
     "WindowsParameters",
     "AccessMode",
     "AccessRuleDirection",
     "AgentConfigurationMode",
     "ArcKindEnum",
     "AssessmentModeTypes",
     "CreatedByType",
     "EsuEligibility",
     "EsuKeyState",
     "EsuServerType",
     "ExecutionState",
     "ExtensionsStatusLevelTypes",
+    "GatewayType",
     "LastAttemptStatusEnum",
     "LicenseAssignmentState",
     "LicenseCoreType",
     "LicenseEdition",
     "LicenseProfileProductType",
     "LicenseProfileSubscriptionStatus",
     "LicenseProfileSubscriptionStatusUpdate",
@@ -268,14 +291,15 @@
     "LicenseTarget",
     "LicenseType",
     "OsType",
     "PatchModeTypes",
     "PatchOperationStartedBy",
     "PatchOperationStatus",
     "PatchServiceUsed",
+    "ProgramYear",
     "ProvisioningIssueSeverity",
     "ProvisioningIssueType",
     "ProvisioningState",
     "PublicNetworkAccessType",
     "StatusLevelTypes",
     "StatusTypes",
     "VMGuestPatchClassificationLinux",
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,20 @@
     """The level code."""
 
     INFO = "Info"
     WARNING = "Warning"
     ERROR = "Error"
 
 
+class GatewayType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """The type of the Gateway resource."""
+
+    PUBLIC = "Public"
+
+
 class LastAttemptStatusEnum(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Specifies the status of Agent Upgrade."""
 
     SUCCESS = "Success"
     FAILED = "Failed"
 
 
@@ -237,14 +243,22 @@
     WU = "WU"
     WU_WSUS = "WU_WSUS"
     YUM = "YUM"
     APT = "APT"
     ZYPPER = "Zypper"
 
 
+class ProgramYear(str, Enum, metaclass=CaseInsensitiveEnumMeta):
+    """Describes the program year the volume license is for."""
+
+    YEAR1 = "Year 1"
+    YEAR2 = "Year 2"
+    YEAR3 = "Year 3"
+
+
 class ProvisioningIssueSeverity(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Severity of the provisioning issue."""
 
     WARNING = "Warning"
     """Warnings can cause connectivity issues after provisioning succeeds."""
     ERROR = "Error"
     """Errors will cause association provisioning to fail."""
@@ -283,14 +297,17 @@
 
     ENABLED = "Enabled"
     """Allows Azure Arc agents to communicate with Azure Arc services over both public (internet) and
     private endpoints."""
     DISABLED = "Disabled"
     """Does not allow Azure Arc agents to communicate with Azure Arc services over public (internet)
     endpoints. The agents must use the private link."""
+    SECURED_BY_PERIMETER = "SecuredByPerimeter"
+    """Azure Arc agent communication with Azure Arc services over public (internet) is enforced by
+    Network Security Perimeter (NSP)"""
 
 
 class StatusLevelTypes(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The level code."""
 
     INFO = "Info"
     WARNING = "Warning"
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_models_py3.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/_models_py3.py`

 * *Files 3% similar despite different names*

```diff
@@ -470,14 +470,57 @@
         self.code = None
         self.message = None
         self.target = None
         self.details = None
         self.additional_info = None
 
 
+class ErrorDetailAutoGenerated(_serialization.Model):
+    """The error detail.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar code: The error code.
+    :vartype code: str
+    :ivar message: The error message.
+    :vartype message: str
+    :ivar target: The error target.
+    :vartype target: str
+    :ivar details: The error details.
+    :vartype details: list[~azure.mgmt.hybridcompute.models.ErrorDetailAutoGenerated]
+    :ivar additional_info: The error additional info.
+    :vartype additional_info: list[~azure.mgmt.hybridcompute.models.ErrorAdditionalInfo]
+    """
+
+    _validation = {
+        "code": {"readonly": True},
+        "message": {"readonly": True},
+        "target": {"readonly": True},
+        "details": {"readonly": True},
+        "additional_info": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "code": {"key": "code", "type": "str"},
+        "message": {"key": "message", "type": "str"},
+        "target": {"key": "target", "type": "str"},
+        "details": {"key": "details", "type": "[ErrorDetailAutoGenerated]"},
+        "additional_info": {"key": "additionalInfo", "type": "[ErrorAdditionalInfo]"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.code = None
+        self.message = None
+        self.target = None
+        self.details = None
+        self.additional_info = None
+
+
 class ErrorResponse(_serialization.Model):
     """Common error response for all Azure Resource Manager APIs to return error details for failed
     operations. (This also follows the OData error response format.).
 
     :ivar error: The error object.
     :vartype error: ~azure.mgmt.hybridcompute.models.ErrorDetail
     """
@@ -491,34 +534,57 @@
         :keyword error: The error object.
         :paramtype error: ~azure.mgmt.hybridcompute.models.ErrorDetail
         """
         super().__init__(**kwargs)
         self.error = error
 
 
+class ErrorResponseAutoGenerated(_serialization.Model):
+    """Common error response for all Azure Resource Manager APIs to return error details for failed
+    operations. (This also follows the OData error response format.).
+
+    :ivar error: The error object.
+    :vartype error: ~azure.mgmt.hybridcompute.models.ErrorDetailAutoGenerated
+    """
+
+    _attribute_map = {
+        "error": {"key": "error", "type": "ErrorDetailAutoGenerated"},
+    }
+
+    def __init__(self, *, error: Optional["_models.ErrorDetailAutoGenerated"] = None, **kwargs: Any) -> None:
+        """
+        :keyword error: The error object.
+        :paramtype error: ~azure.mgmt.hybridcompute.models.ErrorDetailAutoGenerated
+        """
+        super().__init__(**kwargs)
+        self.error = error
+
+
 class EsuKey(_serialization.Model):
     """ESU key.
 
     :ivar sku: SKU number.
     :vartype sku: str
-    :ivar license_status: The current status of the license profile key.
-    :vartype license_status: str
+    :ivar license_status: The current status of the license profile key. Represented by the same
+     integer value that is presented on the machine itself when querying the license key status.
+    :vartype license_status: int
     """
 
     _attribute_map = {
         "sku": {"key": "sku", "type": "str"},
-        "license_status": {"key": "licenseStatus", "type": "str"},
+        "license_status": {"key": "licenseStatus", "type": "int"},
     }
 
-    def __init__(self, *, sku: Optional[str] = None, license_status: Optional[str] = None, **kwargs: Any) -> None:
+    def __init__(self, *, sku: Optional[str] = None, license_status: Optional[int] = None, **kwargs: Any) -> None:
         """
         :keyword sku: SKU number.
         :paramtype sku: str
-        :keyword license_status: The current status of the license profile key.
-        :paramtype license_status: str
+        :keyword license_status: The current status of the license profile key. Represented by the same
+         integer value that is presented on the machine itself when querying the license key status.
+        :paramtype license_status: int
         """
         super().__init__(**kwargs)
         self.sku = sku
         self.license_status = license_status
 
 
 class ExtensionsResourceStatus(_serialization.Model):
@@ -590,21 +656,21 @@
         :keyword target_version: Properties for the specified Extension to Upgrade.
         :paramtype target_version: str
         """
         super().__init__(**kwargs)
         self.target_version = target_version
 
 
-class Resource(_serialization.Model):
+class ResourceAutoGenerated(_serialization.Model):
     """Common fields that are returned in the response for all Azure Resource Manager resources.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -631,22 +697,22 @@
         super().__init__(**kwargs)
         self.id = None
         self.name = None
         self.type = None
         self.system_data = None
 
 
-class ProxyResource(Resource):
+class ProxyResource(ResourceAutoGenerated):
     """The resource model definition for a Azure Resource Manager proxy resource. It will not have
     tags and a location.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -656,16 +722,16 @@
 
 
 class ExtensionValue(ProxyResource):
     """Describes a Extension Metadata.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
-    :ivar id: Fully qualified resource ID for the resource. Ex -
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
     :vartype id: str
     :ivar name: The name of the resource.
     :vartype name: str
     :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
      "Microsoft.Storage/storageAccounts".
     :vartype type: str
     :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
@@ -726,14 +792,237 @@
 
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.value = None
 
 
+class TrackedResourceAutoGenerated(ResourceAutoGenerated):
+    """The resource model definition for an Azure Resource Manager tracked top level resource which
+    has 'tags' and a 'location'.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+    }
+
+    def __init__(self, *, location: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
+        self.location = location
+
+
+class Gateway(TrackedResourceAutoGenerated):  # pylint: disable=too-many-instance-attributes
+    """Describes an Arc Gateway.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar id: Fully qualified resource ID for the resource. E.g.
+     "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}".  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar location: The geo-location where the resource lives. Required.
+    :vartype location: str
+    :ivar provisioning_state: The provisioning state, which only appears in the response. Known
+     values are: "Creating", "Updating", "Deleting", "Succeeded", "Failed", "Accepted", "Canceled",
+     and "Deleted".
+    :vartype provisioning_state: str or ~azure.mgmt.hybridcompute.models.ProvisioningState
+    :ivar gateway_id: A unique, immutable, identifier for the Gateway.
+    :vartype gateway_id: str
+    :ivar gateway_type: The type of the Gateway resource. "Public"
+    :vartype gateway_type: str or ~azure.mgmt.hybridcompute.models.GatewayType
+    :ivar gateway_endpoint: The endpoint fqdn for the Gateway.
+    :vartype gateway_endpoint: str
+    :ivar allowed_features: Specifies the list of features that are enabled for this Gateway.
+    :vartype allowed_features: list[str]
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "location": {"required": True},
+        "provisioning_state": {"readonly": True},
+        "gateway_id": {"readonly": True},
+        "gateway_endpoint": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tags": {"key": "tags", "type": "{str}"},
+        "location": {"key": "location", "type": "str"},
+        "provisioning_state": {"key": "properties.provisioningState", "type": "str"},
+        "gateway_id": {"key": "properties.gatewayId", "type": "str"},
+        "gateway_type": {"key": "properties.gatewayType", "type": "str"},
+        "gateway_endpoint": {"key": "properties.gatewayEndpoint", "type": "str"},
+        "allowed_features": {"key": "properties.allowedFeatures", "type": "[str]"},
+    }
+
+    def __init__(
+        self,
+        *,
+        location: str,
+        tags: Optional[Dict[str, str]] = None,
+        gateway_type: Optional[Union[str, "_models.GatewayType"]] = None,
+        allowed_features: Optional[List[str]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword location: The geo-location where the resource lives. Required.
+        :paramtype location: str
+        :keyword gateway_type: The type of the Gateway resource. "Public"
+        :paramtype gateway_type: str or ~azure.mgmt.hybridcompute.models.GatewayType
+        :keyword allowed_features: Specifies the list of features that are enabled for this Gateway.
+        :paramtype allowed_features: list[str]
+        """
+        super().__init__(tags=tags, location=location, **kwargs)
+        self.provisioning_state = None
+        self.gateway_id = None
+        self.gateway_type = gateway_type
+        self.gateway_endpoint = None
+        self.allowed_features = allowed_features
+
+
+class GatewaysListResult(_serialization.Model):
+    """The List license operation response.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar value: The list of Gateways. Required.
+    :vartype value: list[~azure.mgmt.hybridcompute.models.Gateway]
+    :ivar next_link: The URI to fetch the next page of Gateways. Call ListNext() with this URI to
+     fetch the next page of Gateways.
+    :vartype next_link: str
+    """
+
+    _validation = {
+        "value": {"required": True},
+    }
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "[Gateway]"},
+        "next_link": {"key": "nextLink", "type": "str"},
+    }
+
+    def __init__(self, *, value: List["_models.Gateway"], next_link: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword value: The list of Gateways. Required.
+        :paramtype value: list[~azure.mgmt.hybridcompute.models.Gateway]
+        :keyword next_link: The URI to fetch the next page of Gateways. Call ListNext() with this URI
+         to fetch the next page of Gateways.
+        :paramtype next_link: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+        self.next_link = next_link
+
+
+class ResourceUpdate(_serialization.Model):
+    """The Update Resource model definition.
+
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    """
+
+    _attribute_map = {
+        "tags": {"key": "tags", "type": "{str}"},
+    }
+
+    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        """
+        super().__init__(**kwargs)
+        self.tags = tags
+
+
+class GatewayUpdate(ResourceUpdate):
+    """Describes a License Update.
+
+    :ivar tags: Resource tags.
+    :vartype tags: dict[str, str]
+    :ivar allowed_features: Specifies the list of features that are enabled for this Gateway.
+    :vartype allowed_features: list[str]
+    """
+
+    _attribute_map = {
+        "tags": {"key": "tags", "type": "{str}"},
+        "allowed_features": {"key": "properties.allowedFeatures", "type": "[str]"},
+    }
+
+    def __init__(
+        self, *, tags: Optional[Dict[str, str]] = None, allowed_features: Optional[List[str]] = None, **kwargs: Any
+    ) -> None:
+        """
+        :keyword tags: Resource tags.
+        :paramtype tags: dict[str, str]
+        :keyword allowed_features: Specifies the list of features that are enabled for this Gateway.
+        :paramtype allowed_features: list[str]
+        """
+        super().__init__(tags=tags, **kwargs)
+        self.allowed_features = allowed_features
+
+
 class PrivateLinkScopesResource(_serialization.Model):
     """An azure resource object.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to server.
 
@@ -879,15 +1168,16 @@
 
 class HybridComputePrivateLinkScopeProperties(_serialization.Model):
     """Properties that define a Azure Arc PrivateLinkScope resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar public_network_access: Indicates whether machines associated with the private link scope
-     can also use public Azure Arc service endpoints. Known values are: "Enabled" and "Disabled".
+     can also use public Azure Arc service endpoints. Known values are: "Enabled", "Disabled", and
+     "SecuredByPerimeter".
     :vartype public_network_access: str or ~azure.mgmt.hybridcompute.models.PublicNetworkAccessType
     :ivar provisioning_state: Current state of this PrivateLinkScope: whether or not is has been
      provisioned within the resource group it is defined. Users cannot change this value but are
      able to read from it. Values will include Provisioning ,Succeeded, Canceled and Failed.
     :vartype provisioning_state: str
     :ivar private_link_scope_id: The Guid id of the private link scope.
     :vartype private_link_scope_id: str
@@ -913,27 +1203,88 @@
     }
 
     def __init__(
         self, *, public_network_access: Union[str, "_models.PublicNetworkAccessType"] = "Disabled", **kwargs: Any
     ) -> None:
         """
         :keyword public_network_access: Indicates whether machines associated with the private link
-         scope can also use public Azure Arc service endpoints. Known values are: "Enabled" and
-         "Disabled".
+         scope can also use public Azure Arc service endpoints. Known values are: "Enabled", "Disabled",
+         and "SecuredByPerimeter".
         :paramtype public_network_access: str or
          ~azure.mgmt.hybridcompute.models.PublicNetworkAccessType
         """
         super().__init__(**kwargs)
         self.public_network_access = public_network_access
         self.provisioning_state = None
         self.private_link_scope_id = None
         self.private_endpoint_connections = None
 
 
-class HybridIdentityMetadata(ProxyResource):
+class Resource(_serialization.Model):
+    """Common fields that are returned in the response for all Azure Resource Manager resources.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+    }
+
+    def __init__(self, **kwargs: Any) -> None:
+        """ """
+        super().__init__(**kwargs)
+        self.id = None
+        self.name = None
+        self.type = None
+        self.system_data = None
+
+
+class ProxyResourceAutoGenerated(Resource):
+    """The resource model definition for a Azure Resource Manager proxy resource. It will not have
+    tags and a location.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
+    """
+
+
+class HybridIdentityMetadata(ProxyResourceAutoGenerated):
     """Defines the HybridIdentityMetadata.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
@@ -1310,14 +1661,16 @@
     :vartype type: str or ~azure.mgmt.hybridcompute.models.LicenseCoreType
     :ivar processors: Describes the number of processors.
     :vartype processors: int
     :ivar assigned_licenses: Describes the number of assigned licenses.
     :vartype assigned_licenses: int
     :ivar immutable_id: Describes the immutable id.
     :vartype immutable_id: str
+    :ivar volume_license_details: A list of volume license details.
+    :vartype volume_license_details: list[~azure.mgmt.hybridcompute.models.VolumeLicenseDetails]
     """
 
     _validation = {
         "assigned_licenses": {"readonly": True},
         "immutable_id": {"readonly": True},
     }
 
@@ -1325,24 +1678,26 @@
         "state": {"key": "state", "type": "str"},
         "target": {"key": "target", "type": "str"},
         "edition": {"key": "edition", "type": "str"},
         "type": {"key": "type", "type": "str"},
         "processors": {"key": "processors", "type": "int"},
         "assigned_licenses": {"key": "assignedLicenses", "type": "int"},
         "immutable_id": {"key": "immutableId", "type": "str"},
+        "volume_license_details": {"key": "volumeLicenseDetails", "type": "[VolumeLicenseDetails]"},
     }
 
     def __init__(
         self,
         *,
         state: Optional[Union[str, "_models.LicenseState"]] = None,
         target: Optional[Union[str, "_models.LicenseTarget"]] = None,
         edition: Optional[Union[str, "_models.LicenseEdition"]] = None,
         type: Optional[Union[str, "_models.LicenseCoreType"]] = None,
         processors: Optional[int] = None,
+        volume_license_details: Optional[List["_models.VolumeLicenseDetails"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword state: Describes the state of the license. Known values are: "Activated" and
          "Deactivated".
         :paramtype state: str or ~azure.mgmt.hybridcompute.models.LicenseState
         :keyword target: Describes the license target server. Known values are: "Windows Server 2012"
@@ -1352,23 +1707,26 @@
          Datacenter. Known values are: "Standard" and "Datacenter".
         :paramtype edition: str or ~azure.mgmt.hybridcompute.models.LicenseEdition
         :keyword type: Describes the license core type (pCore or vCore). Known values are: "pCore" and
          "vCore".
         :paramtype type: str or ~azure.mgmt.hybridcompute.models.LicenseCoreType
         :keyword processors: Describes the number of processors.
         :paramtype processors: int
+        :keyword volume_license_details: A list of volume license details.
+        :paramtype volume_license_details: list[~azure.mgmt.hybridcompute.models.VolumeLicenseDetails]
         """
         super().__init__(**kwargs)
         self.state = state
         self.target = target
         self.edition = edition
         self.type = type
         self.processors = processors
         self.assigned_licenses = None
         self.immutable_id = None
+        self.volume_license_details = volume_license_details
 
 
 class LicenseProfile(TrackedResource):  # pylint: disable=too-many-instance-attributes
     """Describes a license profile in a hybrid machine.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -1830,34 +2188,14 @@
         :paramtype next_link: str
         """
         super().__init__(**kwargs)
         self.value = value
         self.next_link = next_link
 
 
-class ResourceUpdate(_serialization.Model):
-    """The Update Resource model definition.
-
-    :ivar tags: Resource tags.
-    :vartype tags: dict[str, str]
-    """
-
-    _attribute_map = {
-        "tags": {"key": "tags", "type": "{str}"},
-    }
-
-    def __init__(self, *, tags: Optional[Dict[str, str]] = None, **kwargs: Any) -> None:
-        """
-        :keyword tags: Resource tags.
-        :paramtype tags: dict[str, str]
-        """
-        super().__init__(**kwargs)
-        self.tags = tags
-
-
 class LicenseProfileUpdate(ResourceUpdate):
     """Describes a License Profile Update.
 
     :ivar tags: Resource tags.
     :vartype tags: dict[str, str]
     :ivar subscription_status: Indicates the subscription status of the product. Known values are:
      "Enable" and "Disable".
@@ -3550,15 +3888,15 @@
         self.os_profile = os_profile
         self.cloud_metadata = cloud_metadata
         self.agent_upgrade = agent_upgrade
         self.parent_cluster_resource_id = parent_cluster_resource_id
         self.private_link_scope_resource_id = private_link_scope_resource_id
 
 
-class NetworkConfiguration(ProxyResource):
+class NetworkConfiguration(ProxyResourceAutoGenerated):
     """NetworkConfiguration.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
@@ -3814,36 +4152,36 @@
     """Network Security Perimeter profile.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar name: Name of the resource.
     :vartype name: str
     :ivar access_rules_version: Access rules version number.
-    :vartype access_rules_version: str
+    :vartype access_rules_version: int
     :ivar access_rules: Collection of access rules for the profile.
     :vartype access_rules: list[~azure.mgmt.hybridcompute.models.AccessRule]
     :ivar diagnostic_settings_version: Diagnostic settings version number.
-    :vartype diagnostic_settings_version: str
+    :vartype diagnostic_settings_version: int
     :ivar enabled_log_categories: Collection of enabled log categories for the profile.
     :vartype enabled_log_categories: list[str]
     """
 
     _validation = {
         "name": {"readonly": True},
         "access_rules_version": {"readonly": True},
         "access_rules": {"readonly": True},
         "diagnostic_settings_version": {"readonly": True},
         "enabled_log_categories": {"readonly": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
-        "access_rules_version": {"key": "accessRulesVersion", "type": "str"},
+        "access_rules_version": {"key": "accessRulesVersion", "type": "int"},
         "access_rules": {"key": "accessRules", "type": "[AccessRule]"},
-        "diagnostic_settings_version": {"key": "diagnosticSettingsVersion", "type": "str"},
+        "diagnostic_settings_version": {"key": "diagnosticSettingsVersion", "type": "int"},
         "enabled_log_categories": {"key": "enabledLogCategories", "type": "[str]"},
     }
 
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.name = None
@@ -4065,15 +4403,15 @@
         :paramtype patch_mode: str or ~azure.mgmt.hybridcompute.models.PatchModeTypes
         """
         super().__init__(**kwargs)
         self.assessment_mode = assessment_mode
         self.patch_mode = patch_mode
 
 
-class PrivateEndpointConnection(ProxyResource):
+class PrivateEndpointConnection(ProxyResourceAutoGenerated):
     """A private endpoint connection.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
@@ -4255,15 +4593,15 @@
         :keyword id: Resource id of the private endpoint.
         :paramtype id: str
         """
         super().__init__(**kwargs)
         self.id = id
 
 
-class PrivateLinkResource(ProxyResource):
+class PrivateLinkResource(ProxyResourceAutoGenerated):
     """A private link resource.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Fully qualified resource ID for the resource. Ex -
      /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
     :vartype id: str
@@ -4368,15 +4706,16 @@
     """PrivateLinkScopeValidationDetails.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     :ivar id: Azure resource Id.
     :vartype id: str
     :ivar public_network_access: Indicates whether machines associated with the private link scope
-     can also use public Azure Arc service endpoints. Known values are: "Enabled" and "Disabled".
+     can also use public Azure Arc service endpoints. Known values are: "Enabled", "Disabled", and
+     "SecuredByPerimeter".
     :vartype public_network_access: str or ~azure.mgmt.hybridcompute.models.PublicNetworkAccessType
     :ivar connection_details: List of Private Endpoint Connection details.
     :vartype connection_details: list[~azure.mgmt.hybridcompute.models.ConnectionDetail]
     """
 
     _validation = {
         "id": {"readonly": True},
@@ -4393,16 +4732,16 @@
         *,
         public_network_access: Union[str, "_models.PublicNetworkAccessType"] = "Disabled",
         connection_details: Optional[List["_models.ConnectionDetail"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword public_network_access: Indicates whether machines associated with the private link
-         scope can also use public Azure Arc service endpoints. Known values are: "Enabled" and
-         "Disabled".
+         scope can also use public Azure Arc service endpoints. Known values are: "Enabled", "Disabled",
+         and "SecuredByPerimeter".
         :paramtype public_network_access: str or
          ~azure.mgmt.hybridcompute.models.PublicNetworkAccessType
         :keyword connection_details: List of Private Endpoint Connection details.
         :paramtype connection_details: list[~azure.mgmt.hybridcompute.models.ConnectionDetail]
         """
         super().__init__(**kwargs)
         self.id = None
@@ -4747,14 +5086,63 @@
         :paramtype guest_configuration_service: ~azure.mgmt.hybridcompute.models.ServiceStatus
         """
         super().__init__(**kwargs)
         self.extension_service = extension_service
         self.guest_configuration_service = guest_configuration_service
 
 
+class Settings(ProxyResourceAutoGenerated):
+    """Settings.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    :ivar id: Fully qualified resource ID for the resource. Ex -
+     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}.  # pylint: disable=line-too-long
+    :vartype id: str
+    :ivar name: The name of the resource.
+    :vartype name: str
+    :ivar type: The type of the resource. E.g. "Microsoft.Compute/virtualMachines" or
+     "Microsoft.Storage/storageAccounts".
+    :vartype type: str
+    :ivar system_data: Azure Resource Manager metadata containing createdBy and modifiedBy
+     information.
+    :vartype system_data: ~azure.mgmt.hybridcompute.models.SystemData
+    :ivar tenant_id: Azure resource tenant Id.
+    :vartype tenant_id: str
+    :ivar gateway_resource_id: Associated Gateway Resource Id.
+    :vartype gateway_resource_id: str
+    """
+
+    _validation = {
+        "id": {"readonly": True},
+        "name": {"readonly": True},
+        "type": {"readonly": True},
+        "system_data": {"readonly": True},
+        "tenant_id": {"readonly": True},
+    }
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "name": {"key": "name", "type": "str"},
+        "type": {"key": "type", "type": "str"},
+        "system_data": {"key": "systemData", "type": "SystemData"},
+        "tenant_id": {"key": "properties.tenantId", "type": "str"},
+        "gateway_resource_id": {"key": "properties.gatewayProperties.gatewayResourceId", "type": "str"},
+    }
+
+    def __init__(self, *, gateway_resource_id: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword gateway_resource_id: Associated Gateway Resource Id.
+        :paramtype gateway_resource_id: str
+        """
+        super().__init__(**kwargs)
+        self.tenant_id = None
+        self.gateway_resource_id = gateway_resource_id
+
+
 class Subnet(_serialization.Model):
     """Describes the subnet.
 
     :ivar address_prefix: Represents address prefix.
     :vartype address_prefix: str
     """
 
@@ -4852,14 +5240,48 @@
         :keyword tags: Resource tags.
         :paramtype tags: dict[str, str]
         """
         super().__init__(**kwargs)
         self.tags = tags
 
 
+class VolumeLicenseDetails(_serialization.Model):
+    """VolumeLicenseDetails.
+
+    :ivar program_year: Describes the program year the volume license is for. Known values are:
+     "Year 1", "Year 2", and "Year 3".
+    :vartype program_year: str or ~azure.mgmt.hybridcompute.models.ProgramYear
+    :ivar invoice_id: The invoice id for the volume license.
+    :vartype invoice_id: str
+    """
+
+    _attribute_map = {
+        "program_year": {"key": "programYear", "type": "str"},
+        "invoice_id": {"key": "invoiceId", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        program_year: Optional[Union[str, "_models.ProgramYear"]] = None,
+        invoice_id: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword program_year: Describes the program year the volume license is for. Known values are:
+         "Year 1", "Year 2", and "Year 3".
+        :paramtype program_year: str or ~azure.mgmt.hybridcompute.models.ProgramYear
+        :keyword invoice_id: The invoice id for the volume license.
+        :paramtype invoice_id: str
+        """
+        super().__init__(**kwargs)
+        self.program_year = program_year
+        self.invoice_id = invoice_id
+
+
 class WindowsParameters(_serialization.Model):
     """Input for InstallPatches on a Windows VM, as directly received by the API.
 
     :ivar classifications_to_include: The update classifications to select when installing patches
      for Windows.
     :vartype classifications_to_include: list[str or
      ~azure.mgmt.hybridcompute.models.VMGuestPatchClassificationWindows]
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/models/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/__init__.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,36 +2,44 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._licenses_operations import LicensesOperations
 from ._machines_operations import MachinesOperations
 from ._machine_extensions_operations import MachineExtensionsOperations
 from ._hybrid_compute_management_client_operations import HybridComputeManagementClientOperationsMixin
 from ._extension_metadata_operations import ExtensionMetadataOperations
 from ._operations import Operations
 from ._network_profile_operations import NetworkProfileOperations
 from ._machine_run_commands_operations import MachineRunCommandsOperations
+from ._gateways_operations import GatewaysOperations
+from ._settings_operations import SettingsOperations
 from ._private_link_scopes_operations import PrivateLinkScopesOperations
 from ._private_link_resources_operations import PrivateLinkResourcesOperations
 from ._private_endpoint_connections_operations import PrivateEndpointConnectionsOperations
+from ._network_security_perimeter_configurations_operations import NetworkSecurityPerimeterConfigurationsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "LicensesOperations",
     "MachinesOperations",
     "MachineExtensionsOperations",
     "HybridComputeManagementClientOperationsMixin",
     "ExtensionMetadataOperations",
     "Operations",
     "NetworkProfileOperations",
     "MachineRunCommandsOperations",
+    "GatewaysOperations",
+    "SettingsOperations",
     "PrivateLinkScopesOperations",
     "PrivateLinkResourcesOperations",
     "PrivateEndpointConnectionsOperations",
+    "NetworkSecurityPerimeterConfigurationsOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Iterable, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -25,28 +26,32 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(
     location: str, publisher: str, extension_type: str, version: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions/{version}",
     )  # pylint: disable=line-too-long
@@ -71,15 +76,15 @@
 
 def build_list_request(
     location: str, publisher: str, extension_type: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/publishers/{publisher}/extensionTypes/{extensionType}/versions",
     )  # pylint: disable=line-too-long
@@ -134,15 +139,15 @@
         :type extension_type: str
         :param version: The version of the Extension being received. Required.
         :type version: str
         :return: ExtensionValue or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.ExtensionValue
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -202,15 +207,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ExtensionValueListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Optional, Type, TypeVar, Union, cast, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -26,28 +27,32 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_upgrade_extensions_request(
     resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/upgradeExtensions",
@@ -74,22 +79,23 @@
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class HybridComputeManagementClientOperationsMixin(  # pylint: disable=name-too-long
     HybridComputeManagementClientMixinABC
 ):
+
     def _upgrade_extensions_initial(  # pylint: disable=inconsistent-return-statements
         self,
         resource_group_name: str,
         machine_name: str,
         extension_upgrade_parameters: Union[_models.MachineExtensionUpgrade, IO[bytes]],
         **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -28,28 +29,32 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_or_update_request(
     resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
@@ -80,15 +85,15 @@
 
 def build_update_request(
     resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
@@ -119,15 +124,15 @@
 
 def build_delete_request(
     resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
     )  # pylint: disable=line-too-long
@@ -155,15 +160,15 @@
 
 def build_get_request(
     resource_group_name: str, machine_name: str, extension_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions/{extensionName}",
     )  # pylint: disable=line-too-long
@@ -191,15 +196,15 @@
 
 def build_list_request(
     resource_group_name: str, machine_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/extensions",
     )  # pylint: disable=line-too-long
@@ -249,15 +254,15 @@
         self,
         resource_group_name: str,
         machine_name: str,
         extension_name: str,
         extension_parameters: Union[_models.MachineExtension, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.MachineExtension]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -456,15 +461,15 @@
         self,
         resource_group_name: str,
         machine_name: str,
         extension_name: str,
         extension_parameters: Union[_models.MachineExtensionUpdate, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.MachineExtension]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -667,15 +672,15 @@
         return LROPoller[_models.MachineExtension](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, machine_name: str, extension_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -790,15 +795,15 @@
         :type machine_name: str
         :param extension_name: The name of the machine extension. Required.
         :type extension_name: str
         :return: MachineExtension or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.MachineExtension
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -858,15 +863,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineExtensionsListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -28,28 +29,32 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_create_or_update_request(
     resource_group_name: str, machine_name: str, run_command_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands/{runCommandName}",
@@ -72,21 +77,58 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
+def build_update_request(
+    resource_group_name: str, machine_name: str, run_command_name: str, subscription_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands/{runCommandName}",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "resourceGroupName": _SERIALIZER.url(
+            "resource_group_name", resource_group_name, "str", max_length=90, min_length=1
+        ),
+        "machineName": _SERIALIZER.url("machine_name", machine_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "runCommandName": _SERIALIZER.url("run_command_name", run_command_name, "str", pattern=r"[a-zA-Z0-9-_\.]+"),
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
+
+
 def build_delete_request(
     resource_group_name: str, machine_name: str, run_command_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands/{runCommandName}",
     )  # pylint: disable=line-too-long
@@ -112,15 +154,15 @@
 
 def build_get_request(
     resource_group_name: str, machine_name: str, run_command_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands/{runCommandName}",
     )  # pylint: disable=line-too-long
@@ -146,15 +188,15 @@
 
 def build_list_request(
     resource_group_name: str, machine_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/runCommands",
     )  # pylint: disable=line-too-long
@@ -202,15 +244,15 @@
         self,
         resource_group_name: str,
         machine_name: str,
         run_command_name: str,
         run_command_properties: Union[_models.MachineRunCommand, IO[bytes]],
         **kwargs: Any
     ) -> _models.MachineRunCommand:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -407,18 +449,229 @@
                 client=self._client,
                 deserialization_callback=get_long_running_output,
             )
         return LROPoller[_models.MachineRunCommand](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
+    def _update_initial(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: Union[_models.MachineRunCommandUpdate, IO[bytes]],
+        **kwargs: Any
+    ) -> Optional[_models.MachineRunCommand]:
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[Optional[_models.MachineRunCommand]] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(run_command_properties, (IOBase, bytes)):
+            _content = run_command_properties
+        else:
+            _json = self._serialize.body(run_command_properties, "MachineRunCommandUpdate")
+
+        _request = build_update_request(
+            resource_group_name=resource_group_name,
+            machine_name=machine_name,
+            run_command_name=run_command_name,
+            subscription_id=self._config.subscription_id,
+            api_version=api_version,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            _request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 202]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
+            raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
+
+        deserialized = None
+        response_headers = {}
+        if response.status_code == 200:
+            deserialized = self._deserialize("MachineRunCommand", pipeline_response)
+
+        if response.status_code == 202:
+            response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
+            response_headers["Retry-After"] = self._deserialize("int", response.headers.get("Retry-After"))
+            response_headers["Azure-AsyncOperation"] = self._deserialize(
+                "str", response.headers.get("Azure-AsyncOperation")
+            )
+
+        if cls:
+            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
+
+        return deserialized  # type: ignore
+
+    @overload
+    def begin_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: _models.MachineRunCommandUpdate,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.MachineRunCommand]:
+        """The operation to update the run command.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Required.
+        :type run_command_properties: ~azure.mgmt.hybridcompute.models.MachineRunCommandUpdate
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def begin_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> LROPoller[_models.MachineRunCommand]:
+        """The operation to update the run command.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Required.
+        :type run_command_properties: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: An instance of LROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def begin_update(
+        self,
+        resource_group_name: str,
+        machine_name: str,
+        run_command_name: str,
+        run_command_properties: Union[_models.MachineRunCommandUpdate, IO[bytes]],
+        **kwargs: Any
+    ) -> LROPoller[_models.MachineRunCommand]:
+        """The operation to update the run command.
+
+        :param resource_group_name: The name of the resource group. The name is case insensitive.
+         Required.
+        :type resource_group_name: str
+        :param machine_name: The name of the hybrid machine. Required.
+        :type machine_name: str
+        :param run_command_name: The name of the run command. Required.
+        :type run_command_name: str
+        :param run_command_properties: Parameters supplied to the Create Run Command. Is either a
+         MachineRunCommandUpdate type or a IO[bytes] type. Required.
+        :type run_command_properties: ~azure.mgmt.hybridcompute.models.MachineRunCommandUpdate or
+         IO[bytes]
+        :return: An instance of LROPoller that returns either MachineRunCommand or the result of
+         cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.hybridcompute.models.MachineRunCommand]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+        api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.MachineRunCommand] = kwargs.pop("cls", None)
+        polling: Union[bool, PollingMethod] = kwargs.pop("polling", True)
+        lro_delay = kwargs.pop("polling_interval", self._config.polling_interval)
+        cont_token: Optional[str] = kwargs.pop("continuation_token", None)
+        if cont_token is None:
+            raw_result = self._update_initial(
+                resource_group_name=resource_group_name,
+                machine_name=machine_name,
+                run_command_name=run_command_name,
+                run_command_properties=run_command_properties,
+                api_version=api_version,
+                content_type=content_type,
+                cls=lambda x, y, z: x,
+                headers=_headers,
+                params=_params,
+                **kwargs
+            )
+        kwargs.pop("error_map", None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize("MachineRunCommand", pipeline_response)
+            if cls:
+                return cls(pipeline_response, deserialized, {})  # type: ignore
+            return deserialized
+
+        if polling is True:
+            polling_method: PollingMethod = cast(PollingMethod, ARMPolling(lro_delay, **kwargs))
+        elif polling is False:
+            polling_method = cast(PollingMethod, NoPolling())
+        else:
+            polling_method = polling
+        if cont_token:
+            return LROPoller[_models.MachineRunCommand].from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output,
+            )
+        return LROPoller[_models.MachineRunCommand](
+            self._client, raw_result, get_long_running_output, polling_method  # type: ignore
+        )
+
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, machine_name: str, run_command_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -535,15 +788,15 @@
         :type machine_name: str
         :param run_command_name: The name of the run command. Required.
         :type run_command_name: str
         :return: MachineRunCommand or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.MachineRunCommand
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -603,15 +856,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineRunCommandsListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_machines_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_machines_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -28,28 +29,32 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_delete_request(
     resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}",
     )  # pylint: disable=line-too-long
@@ -76,15 +81,15 @@
 
 def build_get_request(
     resource_group_name: str, machine_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}",
     )  # pylint: disable=line-too-long
@@ -113,15 +118,15 @@
 
 def build_assess_patches_request(
     resource_group_name: str, name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/assessPatches",
     )  # pylint: disable=line-too-long
@@ -144,15 +149,15 @@
 
 def build_install_patches_request(
     resource_group_name: str, name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{name}/installPatches",
@@ -178,15 +183,15 @@
 
 def build_list_by_resource_group_request(
     resource_group_name: str, subscription_id: str, *, expand: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines",
     )  # pylint: disable=line-too-long
@@ -210,15 +215,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_subscription_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/machines")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str", min_length=1),
     }
@@ -264,15 +269,15 @@
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
         :return: None or the result of cls(response)
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -321,15 +326,15 @@
         :type machine_name: str
         :param expand: The expand expression to apply on the operation. Default value is None.
         :type expand: str
         :return: Machine or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.Machine
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -369,15 +374,15 @@
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
     def _assess_patches_initial(
         self, resource_group_name: str, name: str, **kwargs: Any
     ) -> Optional[_models.MachineAssessPatchesResult]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -487,15 +492,15 @@
     def _install_patches_initial(
         self,
         resource_group_name: str,
         name: str,
         install_patches_input: Union[_models.MachineInstallPatchesParameters, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.MachineInstallPatchesResult]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -701,15 +706,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -781,15 +786,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MachineListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_network_profile_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_network_profile_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Optional, Type, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
@@ -23,26 +24,30 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/networkProfile",
     )  # pylint: disable=line-too-long
@@ -95,15 +100,15 @@
         :type resource_group_name: str
         :param machine_name: The name of the hybrid machine. Required.
         :type machine_name: str
         :return: NetworkProfile or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.NetworkProfile
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Iterable, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -25,26 +26,30 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/providers/Microsoft.HybridCompute/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
@@ -84,15 +89,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.OperationListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_patch.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -28,14 +29,18 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -45,15 +50,15 @@
     private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
@@ -85,15 +90,15 @@
     private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}",
@@ -128,15 +133,15 @@
     private_endpoint_connection_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections/{privateEndpointConnectionName}",
     )  # pylint: disable=line-too-long
@@ -164,15 +169,15 @@
 
 def build_list_by_private_link_scope_request(
     resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateEndpointConnections",
     )  # pylint: disable=line-too-long
@@ -227,15 +232,15 @@
         :type scope_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection. Required.
         :type private_endpoint_connection_name: str
         :return: PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateEndpointConnection
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -280,15 +285,15 @@
         self,
         resource_group_name: str,
         scope_name: str,
         private_endpoint_connection_name: str,
         parameters: Union[_models.PrivateEndpointConnection, IO[bytes]],
         **kwargs: Any
     ) -> Optional[_models.PrivateEndpointConnection]:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -479,15 +484,15 @@
         return LROPoller[_models.PrivateEndpointConnection](
             self._client, raw_result, get_long_running_output, polling_method  # type: ignore
         )
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, private_endpoint_connection_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -608,15 +613,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateEndpointConnectionListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+import sys
+from typing import Any, Callable, Dict, Iterable, Optional, Type, TypeVar
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -25,28 +26,32 @@
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_by_private_link_scope_request(
     resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateLinkResources",
     )  # pylint: disable=line-too-long
@@ -71,15 +76,15 @@
 
 def build_get_request(
     resource_group_name: str, scope_name: str, group_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}/privateLinkResources/{groupName}",
     )  # pylint: disable=line-too-long
@@ -139,15 +144,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.PrivateLinkResourceListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -221,15 +226,15 @@
         :type scope_name: str
         :param group_name: The name of the private link resource. Required.
         :type group_name: str
         :return: PrivateLinkResource or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkResource
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py` & `azure-mgmt-hybridcompute-9.0.0b3/azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, cast, overload
+import sys
+from typing import Any, Callable, Dict, IO, Iterable, Optional, Type, TypeVar, Union, cast, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -28,26 +29,30 @@
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
 from .. import models as _models
 from .._serialization import Serializer
 from .._vendor import HybridComputeManagementClientMixinABC, _convert_request
 
+if sys.version_info >= (3, 9):
+    from collections.abc import MutableMapping
+else:
+    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/privateLinkScopes"
     )
     path_format_arguments = {
@@ -65,15 +70,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_by_resource_group_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes",
     )  # pylint: disable=line-too-long
@@ -95,15 +100,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_request(resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
     )  # pylint: disable=line-too-long
@@ -126,15 +131,15 @@
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
     )  # pylint: disable=line-too-long
@@ -159,15 +164,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
@@ -195,15 +200,15 @@
 
 def build_update_tags_request(
     resource_group_name: str, scope_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/privateLinkScopes/{scopeName}",
@@ -231,15 +236,15 @@
 
 def build_get_validation_details_request(
     location: str, private_link_scope_id: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.HybridCompute/locations/{location}/privateLinkScopes/{privateLinkScopeId}",
     )  # pylint: disable=line-too-long
@@ -262,15 +267,15 @@
 
 def build_get_validation_details_for_machine_request(  # pylint: disable=name-too-long
     resource_group_name: str, machine_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-03-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2024-03-31-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HybridCompute/machines/{machineName}/privateLinkScopes/current",
     )  # pylint: disable=line-too-long
@@ -324,15 +329,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.HybridComputePrivateLinkScopeListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -408,15 +413,15 @@
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.HybridComputePrivateLinkScopeListResult] = kwargs.pop("cls", None)
 
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -475,15 +480,15 @@
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
     def _delete_initial(  # pylint: disable=inconsistent-return-statements
         self, resource_group_name: str, scope_name: str, **kwargs: Any
     ) -> None:
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -588,15 +593,15 @@
         :type resource_group_name: str
         :param scope_name: The name of the Azure Arc PrivateLinkScope resource. Required.
         :type scope_name: str
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -714,15 +719,15 @@
          Servers and Clusters PrivateLinkScope. Is either a HybridComputePrivateLinkScope type or a
          IO[bytes] type. Required.
         :type parameters: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -855,15 +860,15 @@
         :param private_link_scope_tags: Updated tag information to set into the PrivateLinkScope
          instance. Is either a TagsResource type or a IO[bytes] type. Required.
         :type private_link_scope_tags: ~azure.mgmt.hybridcompute.models.TagsResource or IO[bytes]
         :return: HybridComputePrivateLinkScope or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.HybridComputePrivateLinkScope
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -926,15 +931,15 @@
         :param private_link_scope_id: The id (Guid) of the Azure Arc PrivateLinkScope resource.
          Required.
         :type private_link_scope_id: str
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
@@ -986,15 +991,15 @@
         :param machine_name: The name of the target machine to get the private link scope validation
          details for. Required.
         :type machine_name: str
         :return: PrivateLinkScopeValidationDetails or the result of cls(response)
         :rtype: ~azure.mgmt.hybridcompute.models.PrivateLinkScopeValidationDetails
         :raises ~azure.core.exceptions.HttpResponseError:
         """
-        error_map = {
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/PKG-INFO` & `azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-hybridcompute
-Version: 9.0.0b2
+Version: 9.0.0b3
 Summary: Microsoft Azure Hybrid Compute Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -82,14 +82,25 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 9.0.0b3 (2024-05-30)
+
+### Features Added
+
+  - Added operation MachineRunCommandsOperations.begin_update
+  - Added operation group GatewaysOperations
+  - Added operation group LicensesOperations
+  - Added operation group NetworkSecurityPerimeterConfigurationsOperations
+  - Added operation group SettingsOperations
+  - Model LicenseDetails has a new parameter volume_license_details
+
 ## 9.0.0b2 (2024-04-22)
 
 ### Features Added
 
   - Added operation group MachineRunCommandsOperations
   - Model LicenseProfile has a new parameter billing_start_date
   - Model LicenseProfile has a new parameter disenrollment_date
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/azure_mgmt_hybridcompute.egg-info/SOURCES.txt` & `azure-mgmt-hybridcompute-9.0.0b3/azure_mgmt_hybridcompute.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,40 +17,48 @@
 azure/mgmt/hybridcompute/aio/__init__.py
 azure/mgmt/hybridcompute/aio/_configuration.py
 azure/mgmt/hybridcompute/aio/_hybrid_compute_management_client.py
 azure/mgmt/hybridcompute/aio/_patch.py
 azure/mgmt/hybridcompute/aio/_vendor.py
 azure/mgmt/hybridcompute/aio/operations/__init__.py
 azure/mgmt/hybridcompute/aio/operations/_extension_metadata_operations.py
+azure/mgmt/hybridcompute/aio/operations/_gateways_operations.py
 azure/mgmt/hybridcompute/aio/operations/_hybrid_compute_management_client_operations.py
+azure/mgmt/hybridcompute/aio/operations/_licenses_operations.py
 azure/mgmt/hybridcompute/aio/operations/_machine_extensions_operations.py
 azure/mgmt/hybridcompute/aio/operations/_machine_run_commands_operations.py
 azure/mgmt/hybridcompute/aio/operations/_machines_operations.py
 azure/mgmt/hybridcompute/aio/operations/_network_profile_operations.py
+azure/mgmt/hybridcompute/aio/operations/_network_security_perimeter_configurations_operations.py
 azure/mgmt/hybridcompute/aio/operations/_operations.py
 azure/mgmt/hybridcompute/aio/operations/_patch.py
 azure/mgmt/hybridcompute/aio/operations/_private_endpoint_connections_operations.py
 azure/mgmt/hybridcompute/aio/operations/_private_link_resources_operations.py
 azure/mgmt/hybridcompute/aio/operations/_private_link_scopes_operations.py
+azure/mgmt/hybridcompute/aio/operations/_settings_operations.py
 azure/mgmt/hybridcompute/models/__init__.py
 azure/mgmt/hybridcompute/models/_hybrid_compute_management_client_enums.py
 azure/mgmt/hybridcompute/models/_models_py3.py
 azure/mgmt/hybridcompute/models/_patch.py
 azure/mgmt/hybridcompute/operations/__init__.py
 azure/mgmt/hybridcompute/operations/_extension_metadata_operations.py
+azure/mgmt/hybridcompute/operations/_gateways_operations.py
 azure/mgmt/hybridcompute/operations/_hybrid_compute_management_client_operations.py
+azure/mgmt/hybridcompute/operations/_licenses_operations.py
 azure/mgmt/hybridcompute/operations/_machine_extensions_operations.py
 azure/mgmt/hybridcompute/operations/_machine_run_commands_operations.py
 azure/mgmt/hybridcompute/operations/_machines_operations.py
 azure/mgmt/hybridcompute/operations/_network_profile_operations.py
+azure/mgmt/hybridcompute/operations/_network_security_perimeter_configurations_operations.py
 azure/mgmt/hybridcompute/operations/_operations.py
 azure/mgmt/hybridcompute/operations/_patch.py
 azure/mgmt/hybridcompute/operations/_private_endpoint_connections_operations.py
 azure/mgmt/hybridcompute/operations/_private_link_resources_operations.py
 azure/mgmt/hybridcompute/operations/_private_link_scopes_operations.py
+azure/mgmt/hybridcompute/operations/_settings_operations.py
 azure_mgmt_hybridcompute.egg-info/PKG-INFO
 azure_mgmt_hybridcompute.egg-info/SOURCES.txt
 azure_mgmt_hybridcompute.egg-info/dependency_links.txt
 azure_mgmt_hybridcompute.egg-info/not-zip-safe
 azure_mgmt_hybridcompute.egg-info/requires.txt
 azure_mgmt_hybridcompute.egg-info/top_level.txt
 tests/conftest.py
```

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/setup.py` & `azure-mgmt-hybridcompute-9.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/tests/conftest.py` & `azure-mgmt-hybridcompute-9.0.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/tests/disable_test_hybridcompute.py` & `azure-mgmt-hybridcompute-9.0.0b3/tests/disable_test_hybridcompute.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-hybridcompute-9.0.0b2/tests/test_mgmt_hybridcompute.py` & `azure-mgmt-hybridcompute-9.0.0b3/tests/test_mgmt_hybridcompute.py`

 * *Files identical despite different names*

