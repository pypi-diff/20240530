# Comparing `tmp/node-1.2.1.tar.gz` & `tmp/node-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node-1.2.1.tar", last modified: Sun Apr 16 06:07:46 2023, max compression
+gzip compressed data, was "node-1.2.2.tar", last modified: Thu May 30 09:25:58 2024, max compression
```

## Comparing `node-1.2.1.tar` & `node-1.2.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17717 2023-04-16 06:07:46.000000 node-1.2.1/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2023-04-16 06:07:46.000000 node-1.2.1/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       64 2023-04-16 06:07:46.000000 node-1.2.1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)    37413 2023-04-16 06:07:46.274876 node-1.2.1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17494 2023-04-16 06:07:46.000000 node-1.2.1/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-04-16 06:07:46.274876 node-1.2.1/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1618 2023-04-16 06:07:46.000000 node-1.2.1/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.270876 node-1.2.1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.270876 node-1.2.1/src/node/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       76 2023-04-16 06:07:46.000000 node-1.2.1/src/node/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2193 2023-04-16 06:07:46.000000 node-1.2.1/src/node/base.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/behaviors/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3893 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1854 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/adopt.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4559 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/alias.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2230 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/attributes.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3108 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/cache.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2193 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/constraints.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1528 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/context.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9895 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6371 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/factories.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1979 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/fallback.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      767 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/filter.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2714 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/lifecycle.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6441 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/mapping.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4964 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/node.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/nodespace.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7223 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6127 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/reference.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9137 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/schema.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4009 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/sequence.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1939 2023-04-16 06:07:46.000000 node-1.2.1/src/node/behaviors/storage.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      594 2023-04-16 06:07:46.000000 node-1.2.1/src/node/compat.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1627 2023-04-16 06:07:46.000000 node-1.2.1/src/node/events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    26740 2023-04-16 06:07:46.000000 node-1.2.1/src/node/interfaces.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      776 2023-04-16 06:07:46.000000 node-1.2.1/src/node/locking.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/schema/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1615 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14949 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/fields.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      764 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/scope.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7638 2023-04-16 06:07:46.000000 node-1.2.1/src/node/schema/serializer.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9349 2023-04-16 06:07:46.000000 node-1.2.1/src/node/serializer.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       63 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2883 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/base.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      625 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/env.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     9562 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/fullmapping.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      290 2023-04-16 06:07:46.000000 node-1.2.1/src/node/testing/profiling.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.274876 node-1.2.1/src/node/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4603 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3656 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_adopt.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6280 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_alias.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2383 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_attributes.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15962 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_base.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7834 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_cache.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3497 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_common.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3990 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_constraints.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3077 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_context.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10023 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_events.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6101 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_factories.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7306 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_fallback.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1408 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_filter.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5454 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_lifecycle.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1565 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_locking.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8647 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_mapping.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2832 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_node.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2302 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_nodespace.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    32587 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    20996 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_reference.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    31709 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_schema.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6430 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_sequence.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18662 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_serializer.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3295 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_storage.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    39480 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_testing.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2864 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7312 2023-04-16 06:07:46.000000 node-1.2.1/src/node/tests/test_utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8033 2023-04-16 06:07:46.000000 node-1.2.1/src/node/utils.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-04-16 06:07:46.270876 node-1.2.1/src/node.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    37413 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2165 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/top_level.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-04-16 06:07:46.000000 node-1.2.1/src/node.egg-info/zip-safe
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.150216 node-1.2.2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17874 2024-05-30 09:25:57.000000 node-1.2.2/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2024-05-30 09:25:57.000000 node-1.2.2/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       64 2024-05-30 09:25:57.000000 node-1.2.2/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    37783 2024-05-30 09:25:58.150216 node-1.2.2/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17493 2024-05-30 09:25:57.000000 node-1.2.2/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2024-05-30 09:25:58.150216 node-1.2.2/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1618 2024-05-30 09:25:57.000000 node-1.2.2/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.146216 node-1.2.2/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.146216 node-1.2.2/src/node/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       76 2024-05-30 09:25:57.000000 node-1.2.2/src/node/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2193 2024-05-30 09:25:57.000000 node-1.2.2/src/node/base.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.146216 node-1.2.2/src/node/behaviors/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3893 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1854 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/adopt.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4559 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/alias.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2230 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/attributes.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3108 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/cache.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2193 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/constraints.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1528 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/context.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9895 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6371 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/factories.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1979 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/fallback.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      767 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/filter.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2714 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/lifecycle.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6441 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/mapping.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4964 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/node.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2213 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/nodespace.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7223 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6127 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/reference.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9137 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/schema.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4009 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/sequence.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1939 2024-05-30 09:25:57.000000 node-1.2.2/src/node/behaviors/storage.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      594 2024-05-30 09:25:57.000000 node-1.2.2/src/node/compat.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1627 2024-05-30 09:25:57.000000 node-1.2.2/src/node/events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    26740 2024-05-30 09:25:57.000000 node-1.2.2/src/node/interfaces.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      776 2024-05-30 09:25:57.000000 node-1.2.2/src/node/locking.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.150216 node-1.2.2/src/node/schema/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1615 2024-05-30 09:25:57.000000 node-1.2.2/src/node/schema/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14949 2024-05-30 09:25:57.000000 node-1.2.2/src/node/schema/fields.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      764 2024-05-30 09:25:57.000000 node-1.2.2/src/node/schema/scope.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7638 2024-05-30 09:25:57.000000 node-1.2.2/src/node/schema/serializer.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9349 2024-05-30 09:25:57.000000 node-1.2.2/src/node/serializer.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.150216 node-1.2.2/src/node/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       63 2024-05-30 09:25:57.000000 node-1.2.2/src/node/testing/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2883 2024-05-30 09:25:57.000000 node-1.2.2/src/node/testing/base.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      625 2024-05-30 09:25:57.000000 node-1.2.2/src/node/testing/env.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9562 2024-05-30 09:25:57.000000 node-1.2.2/src/node/testing/fullmapping.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      290 2024-05-30 09:25:57.000000 node-1.2.2/src/node/testing/profiling.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.150216 node-1.2.2/src/node/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4603 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3656 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_adopt.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6280 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_alias.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2383 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_attributes.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15962 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_base.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7834 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_cache.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3497 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_common.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3990 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_constraints.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3077 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_context.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10023 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_events.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6101 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_factories.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7306 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_fallback.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1408 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_filter.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5454 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_lifecycle.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1565 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_locking.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8647 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_mapping.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2832 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_node.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2302 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_nodespace.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    32587 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    20996 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_reference.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    31709 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_schema.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6430 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_sequence.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18662 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_serializer.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3295 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_storage.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    39480 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_testing.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2864 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7465 2024-05-30 09:25:57.000000 node-1.2.2/src/node/tests/test_utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8184 2024-05-30 09:25:57.000000 node-1.2.2/src/node/utils.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-30 09:25:58.150216 node-1.2.2/src/node.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    37783 2024-05-30 09:25:58.000000 node-1.2.2/src/node.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2165 2024-05-30 09:25:58.000000 node-1.2.2/src/node.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-30 09:25:58.000000 node-1.2.2/src/node.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-05-30 09:25:58.000000 node-1.2.2/src/node.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2024-05-30 09:25:58.000000 node-1.2.2/src/node.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-05-30 09:25:58.000000 node-1.2.2/src/node.egg-info/top_level.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-30 09:25:58.000000 node-1.2.2/src/node.egg-info/zip-safe
```

### Comparing `node-1.2.1/CHANGES.rst` & `node-1.2.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 
 Changes
 =======
 
+1.2.2 (2024-05-30)
+------------------
+
+- Make sure ``Unset`` class always returns the same instance in ``__new__``.
+  Fixes problems with pickle.
+  [rnix]
+
+
 1.2.1 (2023-04-16)
 ------------------
 
 - Replace deprecated import of ``Order`` with ``MappingOrder`` in ``node.base``.
   [rnix]
```

### Comparing `node-1.2.1/LICENSE.rst` & `node-1.2.2/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 License
 =======
 
 Copyright (c) 2009-2021, BlueDynamics Alliance, Austria
-Copyright (c) 2021-2022, Node Contributors
+Copyright (c) 2021-2024, Node Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `node-1.2.1/PKG-INFO` & `node-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node
-Version: 1.2.1
+Version: 1.2.2
 Summary: Building data structures as node trees
 Home-page: http://github.com/conestack/node
 Author: Node Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Keywords: node tree fullmapping dict
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,28 +15,35 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.rst
+Requires-Dist: odict>=1.9.0
+Requires-Dist: plumber>=1.5
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.deferredimport
+Requires-Dist: zope.deprecation
+Requires-Dist: zope.lifecycleevent
 
 Node
 ====
 
 .. image:: https://img.shields.io/pypi/v/node.svg
     :target: https://pypi.python.org/pypi/node
     :alt: Latest PyPI version
 
 .. image:: https://img.shields.io/pypi/dm/node.svg
     :target: https://pypi.python.org/pypi/node
     :alt: Number of PyPI downloads
 
 .. image:: https://github.com/conestack/node/actions/workflows/test.yaml/badge.svg
-    :target: https://github.com/conestack/node/actions/workflows/test.yaml
+    :target: https://github.com/conestack/node/actions/workflows/test.yml
     :alt: Test node
 
 
 Overview
 --------
 
 Node is a library to create nested data models and structures.
@@ -608,14 +615,22 @@
 - Jens Klein
 
 
 
 Changes
 =======
 
+1.2.2 (2024-05-30)
+------------------
+
+- Make sure ``Unset`` class always returns the same instance in ``__new__``.
+  Fixes problems with pickle.
+  [rnix]
+
+
 1.2.1 (2023-04-16)
 ------------------
 
 - Replace deprecated import of ``Order`` with ``MappingOrder`` in ``node.base``.
   [rnix]
 
 
@@ -1290,15 +1305,15 @@
 - Make it work [rnix, chaoflow, et al]
 
 
 License
 =======
 
 Copyright (c) 2009-2021, BlueDynamics Alliance, Austria
-Copyright (c) 2021-2022, Node Contributors
+Copyright (c) 2021-2024, Node Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `node-1.2.1/README.rst` & `node-1.2.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     :alt: Latest PyPI version
 
 .. image:: https://img.shields.io/pypi/dm/node.svg
     :target: https://pypi.python.org/pypi/node
     :alt: Number of PyPI downloads
 
 .. image:: https://github.com/conestack/node/actions/workflows/test.yaml/badge.svg
-    :target: https://github.com/conestack/node/actions/workflows/test.yaml
+    :target: https://github.com/conestack/node/actions/workflows/test.yml
     :alt: Test node
 
 
 Overview
 --------
 
 Node is a library to create nested data models and structures.
```

### Comparing `node-1.2.1/setup.py` & `node-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.2.1'
+version = '1.2.2'
 shortdesc = "Building data structures as node trees"
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `node-1.2.1/src/node/base.py` & `node-1.2.2/src/node/base.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/__init__.py` & `node-1.2.2/src/node/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/adopt.py` & `node-1.2.2/src/node/behaviors/adopt.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/alias.py` & `node-1.2.2/src/node/behaviors/alias.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/attributes.py` & `node-1.2.2/src/node/behaviors/attributes.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/cache.py` & `node-1.2.2/src/node/behaviors/cache.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/common.py` & `node-1.2.2/src/node/behaviors/common.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/constraints.py` & `node-1.2.2/src/node/behaviors/constraints.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/context.py` & `node-1.2.2/src/node/behaviors/context.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/events.py` & `node-1.2.2/src/node/behaviors/events.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/factories.py` & `node-1.2.2/src/node/behaviors/factories.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/fallback.py` & `node-1.2.2/src/node/behaviors/fallback.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/filter.py` & `node-1.2.2/src/node/behaviors/filter.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/lifecycle.py` & `node-1.2.2/src/node/behaviors/lifecycle.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/mapping.py` & `node-1.2.2/src/node/behaviors/mapping.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/node.py` & `node-1.2.2/src/node/behaviors/node.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/nodespace.py` & `node-1.2.2/src/node/behaviors/nodespace.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/order.py` & `node-1.2.2/src/node/behaviors/order.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/reference.py` & `node-1.2.2/src/node/behaviors/reference.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/schema.py` & `node-1.2.2/src/node/behaviors/schema.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/sequence.py` & `node-1.2.2/src/node/behaviors/sequence.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/behaviors/storage.py` & `node-1.2.2/src/node/behaviors/storage.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/compat.py` & `node-1.2.2/src/node/compat.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/events.py` & `node-1.2.2/src/node/events.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/interfaces.py` & `node-1.2.2/src/node/interfaces.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/locking.py` & `node-1.2.2/src/node/locking.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/schema/__init__.py` & `node-1.2.2/src/node/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/schema/fields.py` & `node-1.2.2/src/node/schema/fields.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/schema/scope.py` & `node-1.2.2/src/node/schema/scope.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/schema/serializer.py` & `node-1.2.2/src/node/schema/serializer.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/serializer.py` & `node-1.2.2/src/node/serializer.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/testing/base.py` & `node-1.2.2/src/node/testing/base.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/testing/env.py` & `node-1.2.2/src/node/testing/env.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/testing/fullmapping.py` & `node-1.2.2/src/node/testing/fullmapping.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/__init__.py` & `node-1.2.2/src/node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_adopt.py` & `node-1.2.2/src/node/tests/test_adopt.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_alias.py` & `node-1.2.2/src/node/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_attributes.py` & `node-1.2.2/src/node/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_base.py` & `node-1.2.2/src/node/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_cache.py` & `node-1.2.2/src/node/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_common.py` & `node-1.2.2/src/node/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_constraints.py` & `node-1.2.2/src/node/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_context.py` & `node-1.2.2/src/node/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_events.py` & `node-1.2.2/src/node/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_factories.py` & `node-1.2.2/src/node/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_fallback.py` & `node-1.2.2/src/node/tests/test_fallback.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_filter.py` & `node-1.2.2/src/node/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_lifecycle.py` & `node-1.2.2/src/node/tests/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_locking.py` & `node-1.2.2/src/node/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_mapping.py` & `node-1.2.2/src/node/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_node.py` & `node-1.2.2/src/node/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_nodespace.py` & `node-1.2.2/src/node/tests/test_nodespace.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_order.py` & `node-1.2.2/src/node/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_reference.py` & `node-1.2.2/src/node/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_schema.py` & `node-1.2.2/src/node/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_sequence.py` & `node-1.2.2/src/node/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_serializer.py` & `node-1.2.2/src/node/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_storage.py` & `node-1.2.2/src/node/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_testing.py` & `node-1.2.2/src/node/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_tests.py` & `node-1.2.2/src/node/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `node-1.2.1/src/node/tests/test_utils.py` & `node-1.2.2/src/node/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 from node.utils import logger
 from node.utils import node_by_path
 from node.utils import ReverseMapping
 from node.utils import safe_decode
 from node.utils import safe_encode
 from node.utils import StrCodec
 from node.utils import UNSET
+from node.utils import Unset
 from odict import odict
 import copy
 import logging
+import pickle
 
 
 class TestUtils(NodeTestCase):
 
     def test_UNSET(self):
         self.assertEqual(repr(UNSET), '<UNSET>')
         self.assertEqual(str(UNSET), '')
@@ -27,14 +29,16 @@
         self.assertEqual(len(UNSET), 0)
         self.assertTrue(copy.copy(UNSET) is UNSET)
         self.assertTrue(copy.deepcopy(UNSET) is UNSET)
         self.assertFalse(UNSET < UNSET)
         self.assertFalse(UNSET <= UNSET)
         self.assertFalse(UNSET > UNSET)
         self.assertFalse(UNSET >= UNSET)
+        self.assertTrue(Unset() is UNSET)
+        self.assertTrue(pickle.loads(pickle.dumps(UNSET)) is UNSET)
 
     def test_ReverseMapping(self):
         context = odict([
             ('foo', 'a'),
             ('bar', 'b')
         ])
         mapping = ReverseMapping(context)
```

### Comparing `node-1.2.1/src/node/utils.py` & `node-1.2.2/src/node/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 
 logger = logging.getLogger('node')
 
 
 class Unset(object):
     """Identify unset values in contrast to None."""
+    instance = None
+
+    def __new__(cls):
+        if cls.instance is None:
+            cls.instance = object.__new__(cls)
+        return cls.instance
 
     def __nonzero__(self):
         return False
 
     __bool__ = __nonzero__
 
     def __str__(self):
```

### Comparing `node-1.2.1/src/node.egg-info/PKG-INFO` & `node-1.2.2/src/node.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: node
-Version: 1.2.1
+Version: 1.2.2
 Summary: Building data structures as node trees
 Home-page: http://github.com/conestack/node
 Author: Node Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Keywords: node tree fullmapping dict
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,28 +15,35 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.rst
+Requires-Dist: odict>=1.9.0
+Requires-Dist: plumber>=1.5
+Requires-Dist: setuptools
+Requires-Dist: zope.component
+Requires-Dist: zope.deferredimport
+Requires-Dist: zope.deprecation
+Requires-Dist: zope.lifecycleevent
 
 Node
 ====
 
 .. image:: https://img.shields.io/pypi/v/node.svg
     :target: https://pypi.python.org/pypi/node
     :alt: Latest PyPI version
 
 .. image:: https://img.shields.io/pypi/dm/node.svg
     :target: https://pypi.python.org/pypi/node
     :alt: Number of PyPI downloads
 
 .. image:: https://github.com/conestack/node/actions/workflows/test.yaml/badge.svg
-    :target: https://github.com/conestack/node/actions/workflows/test.yaml
+    :target: https://github.com/conestack/node/actions/workflows/test.yml
     :alt: Test node
 
 
 Overview
 --------
 
 Node is a library to create nested data models and structures.
@@ -608,14 +615,22 @@
 - Jens Klein
 
 
 
 Changes
 =======
 
+1.2.2 (2024-05-30)
+------------------
+
+- Make sure ``Unset`` class always returns the same instance in ``__new__``.
+  Fixes problems with pickle.
+  [rnix]
+
+
 1.2.1 (2023-04-16)
 ------------------
 
 - Replace deprecated import of ``Order`` with ``MappingOrder`` in ``node.base``.
   [rnix]
 
 
@@ -1290,15 +1305,15 @@
 - Make it work [rnix, chaoflow, et al]
 
 
 License
 =======
 
 Copyright (c) 2009-2021, BlueDynamics Alliance, Austria
-Copyright (c) 2021-2022, Node Contributors
+Copyright (c) 2021-2024, Node Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `node-1.2.1/src/node.egg-info/SOURCES.txt` & `node-1.2.2/src/node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

