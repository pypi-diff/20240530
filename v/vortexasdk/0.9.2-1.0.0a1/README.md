# Comparing `tmp/vortexasdk-0.9.2.tar.gz` & `tmp/vortexasdk-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vortexasdk-0.9.2.tar", last modified: Wed Dec 11 09:51:44 2019, max compression
+gzip compressed data, was "vortexasdk-1.0.0a1.tar", last modified: Fri Apr 26 16:36:22 2024, max compression
```

## Comparing `vortexasdk-0.9.2.tar` & `vortexasdk-1.0.0a1.tar`

### file list

```diff
@@ -1,115 +1,203 @@
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/
--rw-r--r--   0 kit        (501) staff       (20)    17832 2019-12-11 09:50:07.000000 vortexasdk-0.9.2/CHANGELOG.md
--rw-r--r--   0 kit        (501) staff       (20)     3370 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 kit        (501) staff       (20)     3031 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 kit        (501) staff       (20)       63 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/MANIFEST.in
--rw-r--r--   0 kit        (501) staff       (20)     8504 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/PKG-INFO
--rw-r--r--   0 kit        (501) staff       (20)     7259 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/README.md
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/docs/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/docs/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1875 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/docs/autogen.py
--rw-r--r--   0 kit        (501) staff       (20)      150 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/docs/utils.py
--rw-r--r--   0 kit        (501) staff       (20)      300 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/setup.cfg
--rw-r--r--   0 kit        (501) staff       (20)     1091 2019-12-11 09:48:27.000000 vortexasdk-0.9.2/setup.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/__init__.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/api/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/__init__.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/api/examples/
--rw-r--r--   0 kit        (501) staff       (20)      443 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/cargo_event_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     2318 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/cargo_movements.json
--rw-r--r--   0 kit        (501) staff       (20)      189 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/corporate_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)      168 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/corporate_entity2.json
--rw-r--r--   0 kit        (501) staff       (20)      599 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/corporations.json
--rw-r--r--   0 kit        (501) staff       (20)      170 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/geography_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     1768 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/geography_reference.json
--rw-r--r--   0 kit        (501) staff       (20)      192 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/product_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     1030 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/products.json
--rw-r--r--   0 kit        (501) staff       (20)      952 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessel_entity1.json
--rw-r--r--   0 kit        (501) staff       (20)     7818 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessel_movements.json
--rw-r--r--   0 kit        (501) staff       (20)     3322 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessels.json
--rw-r--r--   0 kit        (501) staff       (20)     2126 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/examples/vessels_reference.json
--rw-r--r--   0 kit        (501) staff       (20)     1121 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_cargo_event_entity.py
--rw-r--r--   0 kit        (501) staff       (20)     7820 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/api/test_cargo_movement.py
--rw-r--r--   0 kit        (501) staff       (20)      676 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_corporate_entity.py
--rw-r--r--   0 kit        (501) staff       (20)      352 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_from_dict_mixin.py
--rw-r--r--   0 kit        (501) staff       (20)      729 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_geography_entity.py
--rw-r--r--   0 kit        (501) staff       (20)     1042 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_product_entity.py
--rw-r--r--   0 kit        (501) staff       (20)     1362 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_vessel_entity.py
--rw-r--r--   0 kit        (501) staff       (20)    18110 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/api/test_vessel_movement.py
--rw-r--r--   0 kit        (501) staff       (20)       58 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/config.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/conversions/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/conversions/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1312 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/conversions/test_conversions.py
--rw-r--r--   0 kit        (501) staff       (20)     1432 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/conversions/test_convert_vessels.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/tests/endpoints/
--rw-r--r--   0 kit        (501) staff       (20)        0 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     4893 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/endpoints/test_cargo_movements_real.py
--rw-r--r--   0 kit        (501) staff       (20)      412 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_corporations_real.py
--rw-r--r--   0 kit        (501) staff       (20)      800 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_corporations_search_result.py
--rw-r--r--   0 kit        (501) staff       (20)      734 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/endpoints/test_geographies_real.py
--rw-r--r--   0 kit        (501) staff       (20)      271 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_products.py
--rw-r--r--   0 kit        (501) staff       (20)     2542 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_products_real.py
--rw-r--r--   0 kit        (501) staff       (20)      551 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_reference_endpoints_real.py
--rw-r--r--   0 kit        (501) staff       (20)     1797 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/tests/endpoints/test_vessel_movements_real.py
--rw-r--r--   0 kit        (501) staff       (20)      316 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_vessels.py
--rw-r--r--   0 kit        (501) staff       (20)     2439 2019-12-11 09:43:46.000000 vortexasdk-0.9.2/tests/endpoints/test_vessels_real.py
--rw-r--r--   0 kit        (501) staff       (20)     5483 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/endpoints/test_vessels_search_result.py
--rw-r--r--   0 kit        (501) staff       (20)     1306 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/mock_client.py
--rw-r--r--   0 kit        (501) staff       (20)     1234 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/test_id.py
--rw-r--r--   0 kit        (501) staff       (20)      434 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/test_to_ISODate.py
--rw-r--r--   0 kit        (501) staff       (20)      543 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/test_utils.py
--rw-r--r--   0 kit        (501) staff       (20)      469 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/testcases.py
--rw-r--r--   0 kit        (501) staff       (20)      660 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/tests/timer.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/
--rw-r--r--   0 kit        (501) staff       (20)      166 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)      375 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/abstract_client.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/api/
--rw-r--r--   0 kit        (501) staff       (20)      605 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1367 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/cargo_movement.py
--rw-r--r--   0 kit        (501) staff       (20)      693 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/corporation.py
--rw-r--r--   0 kit        (501) staff       (20)     3143 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/entity_flattening.py
--rw-r--r--   0 kit        (501) staff       (20)     1857 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/entity_serializing.py
--rw-r--r--   0 kit        (501) staff       (20)      989 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/api/geography.py
--rw-r--r--   0 kit        (501) staff       (20)      615 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/id.py
--rw-r--r--   0 kit        (501) staff       (20)      702 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/product.py
--rw-r--r--   0 kit        (501) staff       (20)      905 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/search_result.py
--rw-r--r--   0 kit        (501) staff       (20)      459 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/serdes.py
--rw-r--r--   0 kit        (501) staff       (20)     1917 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/api/shared_types.py
--rw-r--r--   0 kit        (501) staff       (20)     1688 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/vessel.py
--rw-r--r--   0 kit        (501) staff       (20)     1079 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/api/vessel_movement.py
--rw-r--r--   0 kit        (501) staff       (20)     4634 2019-12-11 09:43:46.000000 vortexasdk-0.9.2/vortexasdk/client.py
--rw-r--r--   0 kit        (501) staff       (20)      330 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/config.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/conversions/
--rw-r--r--   0 kit        (501) staff       (20)      322 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/conversions/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)     1129 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/conversions/conversions.py
--rw-r--r--   0 kit        (501) staff       (20)      501 2019-12-11 09:35:37.000000 vortexasdk-0.9.2/vortexasdk/conversions/corporations.py
--rw-r--r--   0 kit        (501) staff       (20)      668 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/conversions/geographies.py
--rw-r--r--   0 kit        (501) staff       (20)      479 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/conversions/products.py
--rw-r--r--   0 kit        (501) staff       (20)     1544 2019-12-11 09:35:37.000000 vortexasdk-0.9.2/vortexasdk/conversions/vessels.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk/endpoints/
--rw-r--r--   0 kit        (501) staff       (20)      371 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/__init__.py
--rw-r--r--   0 kit        (501) staff       (20)    10213 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/endpoints/cargo_movements.py
--rw-r--r--   0 kit        (501) staff       (20)    32511 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/cargo_movements_result.py
--rw-r--r--   0 kit        (501) staff       (20)     2598 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/endpoints/corporations.py
--rw-r--r--   0 kit        (501) staff       (20)     1247 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/corporations_result.py
--rw-r--r--   0 kit        (501) staff       (20)      330 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/endpoints.py
--rw-r--r--   0 kit        (501) staff       (20)     2383 2019-12-10 19:19:59.000000 vortexasdk-0.9.2/vortexasdk/endpoints/geographies.py
--rw-r--r--   0 kit        (501) staff       (20)     1223 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/geographies_result.py
--rw-r--r--   0 kit        (501) staff       (20)     3586 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/endpoints/products.py
--rw-r--r--   0 kit        (501) staff       (20)     1378 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/products_result.py
--rw-r--r--   0 kit        (501) staff       (20)     6836 2019-12-10 19:24:19.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessel_movements.py
--rw-r--r--   0 kit        (501) staff       (20)    21116 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessel_movements_result.py
--rw-r--r--   0 kit        (501) staff       (20)     4515 2019-12-11 09:43:46.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessels.py
--rw-r--r--   0 kit        (501) staff       (20)     1218 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/endpoints/vessels_result.py
--rw-r--r--   0 kit        (501) staff       (20)      121 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/exceptions.py
--rw-r--r--   0 kit        (501) staff       (20)      785 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/logger.py
--rw-r--r--   0 kit        (501) staff       (20)     2154 2019-12-10 19:19:35.000000 vortexasdk-0.9.2/vortexasdk/operations.py
--rw-r--r--   0 kit        (501) staff       (20)     1118 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/retry_session.py
--rw-r--r--   0 kit        (501) staff       (20)      399 2019-12-10 17:59:33.000000 vortexasdk-0.9.2/vortexasdk/utils.py
-drwxr-xr-x   0 kit        (501) staff       (20)        0 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/
--rw-r--r--   0 kit        (501) staff       (20)     8504 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/PKG-INFO
--rw-r--r--   0 kit        (501) staff       (20)     3231 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/SOURCES.txt
--rw-r--r--   0 kit        (501) staff       (20)        1 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/dependency_links.txt
--rw-r--r--   0 kit        (501) staff       (20)      184 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/requires.txt
--rw-r--r--   0 kit        (501) staff       (20)       22 2019-12-11 09:51:44.000000 vortexasdk-0.9.2/vortexasdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.459622 vortexasdk-1.0.0a1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38970 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/CHANGELOG.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3370 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5188 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12516 2024-04-26 16:36:22.459622 vortexasdk-1.0.0a1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11980 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.395621 vortexasdk-1.0.0a1/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/docs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1917 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/docs/autogen.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/docs/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.395621 vortexasdk-1.0.0a1/scripts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/scripts/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/scripts/validate_proposed_package_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      535 2024-04-26 16:36:22.459622 vortexasdk-1.0.0a1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1853 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.403621 vortexasdk-1.0.0a1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.407621 vortexasdk-1.0.0a1/tests/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.411621 vortexasdk-1.0.0a1/tests/api/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6169 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/asset_tanks.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/attributes.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2654 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/cargo_movements.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/cargo_time_series.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      168 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/corporate_entity2.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      573 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/corporations.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1768 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/geography_reference.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1159 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/products.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5296 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/storage_terminals.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4132 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/vessels.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2126 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/examples/vessels_reference.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1566 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_canal_transit_entity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_cargo_event_entity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8797 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_cargo_movement.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      491 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_corporate_entity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_geography_entity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      659 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_missing_keys.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      896 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_product_entity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1996 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/api/test_vessel_entity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.423622 vortexasdk-1.0.0a1/tests/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1429 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_asset_tanks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_attributes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1589 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_attributes_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2749 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_availability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      556 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_availability_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_availability_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_canal_transit_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_canal_transit_timeseries_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10699 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_cargo_movements_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1227 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_cargo_time_series.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6400 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_cargo_time_series_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      332 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_corporations_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      830 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_corporations_search_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3905 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_destination_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1397 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_eia_forecasts_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4803 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_freight_pricing_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1158 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_freight_pricing_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      964 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_geographies_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2019 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_movement_status_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1556 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_onshore_inventories_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3167 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_onshore_inventories_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3855 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_origin_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_parent_product_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1831 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_product_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1410 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_products.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2187 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_products_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_reference_endpoints_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1406 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_storage_terminals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1358 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_vessel_class_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      418 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_vessels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2585 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_vessels_real.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7191 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_vessels_search_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8566 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_voyage_events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4047 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_voyages_congestion_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6438 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_voyages_search_enriched.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2019 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_voyages_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3408 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/endpoints/test_voyages_top_hits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1970 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/mock_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1380 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1234 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1251 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_operations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_to_ISODate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      430 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_to_ISODate_Array.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7913 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_version_proposals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      332 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/test_versioning.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      469 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/testcases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/tests/timer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.427622 vortexasdk-1.0.0a1/vortexasdk/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2263 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.435622 vortexasdk-1.0.0a1/vortexasdk/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2617 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      772 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/aggregation_breakdown_item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1263 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/asset_tank.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/attribute.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      934 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/breakdown_item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2056 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/canal_transit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5615 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/cargo_movement.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      668 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/corporation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      359 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/eia_forecast.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2579 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/entity_flattening.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1857 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/entity_serializing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/fixture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/freight_pricing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/geography.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      906 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/onshore_inventory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1030 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/product.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/search_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4716 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/shared_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/storage_terminal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/timeseries_item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2784 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/vessel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2159 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/vessel_availability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      577 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/vessel_positions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/vessel_summary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6788 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/api/voyages.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2693 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/check_setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11363 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.459622 vortexasdk-1.0.0a1/vortexasdk/endpoints/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1744 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/aggregation_breakdown_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6937 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/asset_tanks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1492 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/asset_tanks_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5548 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/attributes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1296 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/attributes_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12178 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/canal_transit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/canal_transit_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13071 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/canal_transit_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18967 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/cargo_movements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33045 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/cargo_movements_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19073 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/cargo_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5846 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/corporations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1320 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/corporations_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16806 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/destination_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6688 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/eia_forecasts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1375 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/eia_forecasts_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2019 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/endpoints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11911 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4438 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/fixtures_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/freight_pricing_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5752 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/freight_pricing_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6020 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/freight_pricing_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5966 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/geographies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1280 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/geographies_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16095 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/movement_status_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3556 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/onshore_inventories_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9796 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/onshore_inventories_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9700 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/onshore_inventories_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16731 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/origin_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16264 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/parent_product_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16605 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/product_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6988 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/products.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1434 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/products_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2944 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/reference_breakdown_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5698 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/storage_terminals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1353 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/storage_terminals_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4007 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/timeseries_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13424 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_availability_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8317 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_availability_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13944 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_availability_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14031 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_availability_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15814 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_class_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7085 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_positions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1403 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_positions_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_summary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1506 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessel_summary_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9355 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessels.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1276 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/vessels_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4598 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_breakdown_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20334 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_congestion_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4453 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_congestion_breakdown_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22537 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_geography_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23177 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_product_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24954 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_routes_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29394 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_search_enriched.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2113 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_search_enriched_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26637 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_timeseries.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23495 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_timeseries_v2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20882 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_top_hits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22311 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/endpoints/voyages_vessel_class_breakdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      733 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5998 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/operations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1630 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/result_conversions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/retry_session.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/search_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3709 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      936 2024-04-26 16:35:38.000000 vortexasdk-1.0.0a1/vortexasdk/version_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 16:36:22.431622 vortexasdk-1.0.0a1/vortexasdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12516 2024-04-26 16:36:22.000000 vortexasdk-1.0.0a1/vortexasdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6977 2024-04-26 16:36:22.000000 vortexasdk-1.0.0a1/vortexasdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-26 16:36:22.000000 vortexasdk-1.0.0a1/vortexasdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2024-04-26 16:36:22.000000 vortexasdk-1.0.0a1/vortexasdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2024-04-26 16:36:22.000000 vortexasdk-1.0.0a1/vortexasdk.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vortexasdk-0.9.2/CODE_OF_CONDUCT.md` & `vortexasdk-1.0.0a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.2/docs/autogen.py` & `vortexasdk-1.0.0a1/docs/autogen.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 import six
 
 
 # From https://github.com/keras-team/keras/blob/0a0ac3fa5462cf4a72636ca4498a0a82ac91fc32/docs/autogen.py
 
 
-def get_module_docstring(filepath):
+def get_module_docstring(filepath: str) -> tuple[str, int]:
     """Extract the module docstring.
     Also finds the line at which the docstring ends.
     """
     co = compile(open(filepath, encoding="utf-8").read(), filepath, "exec")
     if co.co_consts and isinstance(co.co_consts[0], six.string_types):
         docstring = co.co_consts[0]
     else:
         print("Could not get the docstring from " + filepath)
         docstring = ""
     return docstring, co.co_firstlineno
 
 
-def copy_examples(examples_dir, destination_dir):
+def copy_examples(examples_dir: str, destination_dir: str) -> None:
     """Copy the examples directory in the documentation.
     Prettify files by extracting the docstrings written in Markdown.
     """
     pathlib.Path(destination_dir).mkdir(exist_ok=True)
     for file in os.listdir(examples_dir):
         if not file.endswith(".py"):
             continue
```

### Comparing `vortexasdk-0.9.2/tests/api/examples/cargo_movements.json` & `vortexasdk-1.0.0a1/tests/api/examples/vessels_reference.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('id', "*

 * *            "'48fca2ce4042e5e670a26f1ed2c9dbb8788bfd9bf763deb339791c3e818e2926'), ('name', "*

 * *            "'A.I.E.S.A. Boarding Pontoon'), ('layer', ['terminal']), ('leaf', True), "*

 * *            "('bounding_box', OrderedDict([('coordinates', [[[-6.922674179077148, "*

 * *            '37.17572267028018], [-6.922674179077148, 37.17812478494196], [-6.919476985931396, '*

 * *            '37.17812478494196], [-6.919476985931396, 37.17572267028018], [-6.922674179077148, '*

 * *            "37.17 […]*

```diff
@@ -1,77 +1,92 @@
-[
-    {
-        "cargo_movement_id": "00886b05a0747522b67322f50123ee60e61e219fc9a9c6011be1a1dade65f63e",
-        "events": [
-            {
-                "end_timestamp": "2019-10-20T16:41:49+0000",
-                "event_type": "cargo_port_load_event",
-                "location": [
-                    {
-                        "id": "2dfc3d43a21697c02ec3b2700b3b570a6ed1abb66d01c4fe6310ef362fcf6653",
-                        "label": "Netherlands",
-                        "layer": "country",
-                        "probability": 1,
-                        "source": "model"
-                    }
+{
+    "bounding_box": {
+        "coordinates": [
+            [
+                [
+                    -6.922674179077148,
+                    37.17572267028018
                 ],
-                "pos": [
-                    4.29914090037834,
-                    51.87936163368058
+                [
+                    -6.922674179077148,
+                    37.17812478494196
                 ],
-                "probability": 1,
-                "start_timestamp": "2019-10-18T21:38:34+0000"
-            }
-        ],
-        "product": [
-            {
-                "id": "b68cbb746f8b9098c50e2ba36bcad83001a53bd362e9031fb49085d02c36659c",
-                "label": "Clean products",
-                "layer": "group",
-                "probability": 0.4756425,
-                "source": "model"
-            },
-            {
-                "id": "a75fcc09bfc7d16496de3336551bc52b5891838bb7c22356d2cb65451587d1e5",
-                "label": "Biodiesel",
-                "layer": "group_product",
-                "probability": 0.4756425,
-                "source": "model"
-            },
-            {
-                "id": "9d52ede1cff0421a8cd7283b0171afe8d23f519dca5f4e489734522f9cdf804c",
-                "label": "Biodiesel Feedstock",
-                "layer": "grade",
-                "probability": 0.4756425,
-                "source": "model"
-            }
-        ],
-        "quantity": 4401,
-        "status": "unloaded_state",
-        "vessels": [
-            {
-                "corporate_entities": [
-                    {
-                        "id": "f9bd45e65e292909a7b751b0026dcf7795c6194b3c0712910a241caee32c99b8",
-                        "label": "Essberger J.T.",
-                        "layer": "commercial_owner",
-                        "probability": 1,
-                        "source": "external"
-                    }
+                [
+                    -6.919476985931396,
+                    37.17812478494196
                 ],
-                "cubic_capacity": 6100,
-                "dwt": 5260,
-                "end_timestamp": "2019-10-25T00:40:46+0000",
-                "fixture_fulfilled": false,
-                "id": "9cbf7c0fc6ccf1dfeacde02b87f3b6b1653030f560d4fc677bf1d7d0be8f8449",
-                "imo": 9480980,
-                "mmsi": 255804460,
-                "name": "JOHANN ESSBERGER",
-                "start_timestamp": "2019-10-18T21:38:34+0000",
-                "status": "vessel_status_laden_known",
-                "tags": [],
-                "vessel_class": "tiny_tanker",
-                "voyage_id": "401f0e74fc42401248a484aca2e9955dea885378796f7f4d0bc8e92c35ea270a"
-            }
-        ]
-    }
-]
+                [
+                    -6.919476985931396,
+                    37.17572267028018
+                ],
+                [
+                    -6.922674179077148,
+                    37.17572267028018
+                ]
+            ]
+        ],
+        "type": "Polygon"
+    },
+    "exclusion_rule": [
+        {
+            "id": "48fca2ce4042e5e670a26f1ed2c9dbb8788bfd9bf763deb339791c3e818e2926",
+            "layer": [
+                "terminal"
+            ],
+            "name": "A.I.E.S.A. Boarding Pontoon"
+        }
+    ],
+    "hierarchy": [
+        {
+            "id": "c1698979b983b265490545013156924518af07faf7f25905a78a1813054860d8",
+            "layer": "country"
+        },
+        {
+            "id": "d677e3a028e466356af42cacb5b8733fbc5367b99ee1075b68ea572868e55780",
+            "layer": "port"
+        },
+        {
+            "id": "f39d455f5d38907394d6da3a91da4e391f9a34bd6a17e826d6042761067e88f4",
+            "layer": "region"
+        },
+        {
+            "id": "676c3cff1dffd971ae51cd350f231394eeb0ab94eff981432f6ee55c5219b913",
+            "layer": "shipping_region"
+        },
+        {
+            "id": "a0a9eba4c7b8c1e853c207f32d67c4959b6197c39785e037abad42e90824c088",
+            "layer": "shipping_region"
+        },
+        {
+            "id": "6aa9a4fb76ca378e75eff85f458c90f7fd42778c26c957c417490c097161a3c5",
+            "layer": "trading_region"
+        },
+        {
+            "id": "9d18c3bff244a391b56d706cd85b3c304e875a54db5db556ad76e0be8df3329a",
+            "layer": "trading_subregion"
+        },
+        {
+            "id": "48fca2ce4042e5e670a26f1ed2c9dbb8788bfd9bf763deb339791c3e818e2926",
+            "layer": "terminal"
+        }
+    ],
+    "id": "48fca2ce4042e5e670a26f1ed2c9dbb8788bfd9bf763deb339791c3e818e2926",
+    "layer": [
+        "terminal"
+    ],
+    "leaf": true,
+    "name": "A.I.E.S.A. Boarding Pontoon",
+    "parent": [
+        {
+            "id": "d677e3a028e466356af42cacb5b8733fbc5367b99ee1075b68ea572868e55780",
+            "layer": [
+                "port"
+            ],
+            "name": "Huelva [ES]"
+        }
+    ],
+    "pos": [
+        -6.921049613576277,
+        37.17694070939973
+    ],
+    "ref_type": "geography"
+}
```

### Comparing `vortexasdk-0.9.2/tests/api/examples/geography_reference.json` & `vortexasdk-1.0.0a1/tests/api/examples/geography_reference.json`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.2/tests/api/examples/vessel_movements.json` & `vortexasdk-1.0.0a1/tests/endpoints/test_voyage_events.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,489 +1,536 @@
-00000000: 5b0a 2020 7b0a 2020 2020 2276 6573 7365  [.  {.    "vesse
-00000010: 6c5f 6d6f 7665 6d65 6e74 5f69 6422 3a20  l_movement_id": 
-00000020: 2237 6530 6662 3933 3165 6331 3131 3764  "7e0fb931ec1117d
-00000030: 3130 3266 3935 3730 3438 6136 6363 6534  102f957048a6cce4
-00000040: 3733 6137 6561 6633 6632 6239 3566 3662  73a7eaf3f2b95f6b
-00000050: 6363 6463 6337 6235 3064 6333 6438 6162  ccdcc7b50dc3d8ab
-00000060: 3722 2c0a 2020 2020 2273 7461 7274 5f74  7",.    "start_t
-00000070: 696d 6573 7461 6d70 223a 2022 3230 3137  imestamp": "2017
-00000080: 2d31 312d 3139 5430 363a 3539 3a30 352b  -11-19T06:59:05+
-00000090: 3030 3030 222c 0a20 2020 2022 656e 645f  0000",.    "end_
-000000a0: 7469 6d65 7374 616d 7022 3a20 2232 3031  timestamp": "201
-000000b0: 372d 3131 2d32 3954 3032 3a34 393a 3332  7-11-29T02:49:32
-000000c0: 2b30 3030 3022 2c0a 2020 2020 2276 6f79  +0000",.    "voy
-000000d0: 6167 655f 6964 223a 2022 3761 3239 6334  age_id": "7a29c4
-000000e0: 3838 3032 3736 6362 6264 6661 6465 3265  880276cbbdfade2e
-000000f0: 6336 6130 6565 3264 6262 6562 6639 6534  c6a0ee2dbbebf9e4
-00000100: 3162 6234 3762 3138 3635 3731 3936 6666  1bb47b18657196ff
-00000110: 6637 6364 3364 6333 3265 222c 0a20 2020  f7cd3dc32e",.   
-00000120: 2022 7665 7373 656c 223a 207b 0a20 2020   "vessel": {.   
-00000130: 2020 2022 6964 223a 2022 3664 3861 3866     "id": "6d8a8f
-00000140: 3038 3633 6361 3038 3732 3034 6464 3638  0863ca087204dd68
-00000150: 6535 6663 3362 3634 3639 6138 3739 3832  e5fc3b6469a87982
-00000160: 3965 3632 3632 3835 3665 3334 3835 3661  9e6262856e34856a
-00000170: 6561 3363 6132 3035 3039 222c 0a20 2020  ea3ca20509",.   
-00000180: 2020 2022 6d6d 7369 223a 2032 3438 3839     "mmsi": 24889
-00000190: 3630 3030 2c0a 2020 2020 2020 2269 6d6f  6000,.      "imo
-000001a0: 223a 2039 3338 3038 3933 2c0a 2020 2020  ": 9380893,.    
-000001b0: 2020 226e 616d 6522 3a20 2231 3720 4645    "name": "17 FE
-000001c0: 4252 5541 5259 222c 0a20 2020 2020 2022  BRUARY",.      "
-000001d0: 6477 7422 3a20 3136 3033 3931 2c0a 2020  dwt": 160391,.  
-000001e0: 2020 2020 2263 7562 6963 5f63 6170 6163      "cubic_capac
-000001f0: 6974 7922 3a20 3137 3230 3932 2c0a 2020  ity": 172092,.  
-00000200: 2020 2020 2276 6573 7365 6c5f 636c 6173      "vessel_clas
-00000210: 7322 3a20 2273 7565 7a6d 6178 222c 0a20  s": "suezmax",. 
-00000220: 2020 2020 2022 636f 7270 6f72 6174 655f       "corporate_
-00000230: 656e 7469 7469 6573 223a 205b 0a20 2020  entities": [.   
-00000240: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00000250: 2022 6964 223a 2022 3139 6231 6266 3339   "id": "19b1bf39
-00000260: 3266 3437 3463 6139 3432 6237 6232 3564  2f474ca942b7b25d
-00000270: 6463 6261 3336 3336 3338 3531 3662 3265  dcba363638516b2e
-00000280: 3430 3236 3865 6137 6137 3038 3838 3032  40268ea7a7088802
-00000290: 3135 3735 6134 6464 222c 0a20 2020 2020  1575a4dd",.     
-000002a0: 2020 2020 2022 6c61 7965 7222 3a20 2263       "layer": "c
-000002b0: 6861 7274 6572 6572 222c 0a20 2020 2020  harterer",.     
-000002c0: 2020 2020 2022 7072 6f62 6162 696c 6974       "probabilit
-000002d0: 7922 3a20 312c 0a20 2020 2020 2020 2020  y": 1,.         
-000002e0: 2022 736f 7572 6365 223a 2022 6578 7465   "source": "exte
-000002f0: 726e 616c 222c 0a20 2020 2020 2020 2020  rnal",.         
-00000300: 2022 6c61 6265 6c22 3a20 2256 4954 4f4c   "label": "VITOL
-00000310: 220a 2020 2020 2020 2020 7d2c 0a20 2020  ".        },.   
-00000320: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00000330: 2022 6964 223a 2022 3031 6563 3437 3465   "id": "01ec474e
-00000340: 3733 3234 6337 3633 3366 6661 6632 6135  7324c7633ffaf2a5
-00000350: 6339 3262 6237 3334 3863 6330 3261 6463  c92bb7348cc02adc
-00000360: 3464 3130 6238 3564 6161 3364 6432 6363  4d10b85daa3dd2cc
-00000370: 3534 3538 6466 3539 222c 0a20 2020 2020  5458df59",.     
-00000380: 2020 2020 2022 6c61 6265 6c22 3a20 2243       "label": "C
-00000390: 4f52 4520 5045 5452 4f4c 4555 4d22 2c0a  ORE PETROLEUM",.
-000003a0: 2020 2020 2020 2020 2020 226c 6179 6572            "layer
-000003b0: 223a 2022 636f 6d6d 6572 6369 616c 5f6f  ": "commercial_o
-000003c0: 776e 6572 222c 0a20 2020 2020 2020 2020  wner",.         
-000003d0: 2022 7072 6f62 6162 696c 6974 7922 3a20   "probability": 
-000003e0: 312c 0a20 2020 2020 2020 2020 2022 736f  1,.          "so
-000003f0: 7572 6365 223a 2022 6578 7465 726e 616c  urce": "external
-00000400: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-00000410: 2020 5d2c 0a20 2020 2020 2022 7461 6773    ],.      "tags
-00000420: 223a 205b 5d2c 0a20 2020 2020 2022 7374  ": [],.      "st
-00000430: 6174 7573 223a 2022 7665 7373 656c 5f73  atus": "vessel_s
-00000440: 7461 7475 735f 6261 6c6c 6173 7422 0a20  tatus_ballast". 
-00000450: 2020 207d 2c0a 2020 2020 226f 7269 6769     },.    "origi
-00000460: 6e22 3a20 7b0a 2020 2020 2020 2265 7665  n": {.      "eve
-00000470: 6e74 5f69 6422 3a20 2235 3736 3939 3935  nt_id": "5769995
-00000480: 6139 3332 6531 3532 6639 6465 6434 3237  a932e152f9ded427
-00000490: 3036 6365 6265 3930 3939 3262 6136 6363  06cebe90992ba6cc
-000004a0: 3036 3230 3865 3332 3833 3364 3239 6561  06208e32833d29ea
-000004b0: 3931 6533 3761 3638 6622 2c0a 2020 2020  91e37a68f",.    
-000004c0: 2020 226c 6f63 6174 696f 6e22 3a20 5b0a    "location": [.
-000004d0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000004e0: 2020 2020 2269 6422 3a20 2239 3334 6334      "id": "934c4
-000004f0: 3766 3336 6331 3661 3538 6436 3865 6635  7f36c16a58d68ef5
-00000500: 6530 3037 6536 3261 3233 6635 6630 3336  e007e62a23f5f036
-00000510: 6565 3366 3364 3166 3566 3835 6134 3863  ee3f3d1f5f85a48c
-00000520: 3537 3262 3930 6164 3862 3222 2c0a 2020  572b90ad8b2",.  
-00000530: 2020 2020 2020 2020 226c 6179 6572 223a          "layer":
-00000540: 2022 636f 756e 7472 7922 2c0a 2020 2020   "country",.    
-00000550: 2020 2020 2020 2270 726f 6261 6269 6c69        "probabili
-00000560: 7479 223a 2031 2c0a 2020 2020 2020 2020  ty": 1,.        
-00000570: 2020 2273 6f75 7263 6522 3a20 226d 6f64    "source": "mod
-00000580: 656c 222c 0a20 2020 2020 2020 2020 2022  el",.          "
-00000590: 6c61 6265 6c22 3a20 2243 6869 6e61 220a  label": "China".
-000005a0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000005b0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-000005c0: 6964 223a 2022 6339 3031 6363 3939 6137  id": "c901cc99a7
-000005d0: 3934 6166 6531 6137 6139 3134 3663 3435  94afe1a7a9146c45
-000005e0: 3733 3432 3065 3837 6336 3239 3731 3736  73420e87c6297176
-000005f0: 3531 6333 6130 6432 6565 3336 3238 6364  51c3a0d2ee3628cd
-00000600: 6166 3062 6335 222c 0a20 2020 2020 2020  af0bc5",.       
-00000610: 2020 2022 6c61 7965 7222 3a20 2270 6f72     "layer": "por
-00000620: 7422 2c0a 2020 2020 2020 2020 2020 2270  t",.          "p
-00000630: 726f 6261 6269 6c69 7479 223a 2031 2c0a  robability": 1,.
-00000640: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
-00000650: 6522 3a20 226d 6f64 656c 222c 0a20 2020  e": "model",.   
-00000660: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-00000670: 2242 6179 7571 7561 6e20 5b43 4e5d 220a  "Bayuquan [CN]".
-00000680: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000690: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-000006a0: 6964 223a 2022 6536 3935 3561 3263 3539  id": "e6955a2c59
-000006b0: 6463 3930 3833 3339 3836 6665 3038 3934  dc90833986fe0894
-000006c0: 6366 3637 3138 6464 6461 6137 3831 3662  cf6718dddaa7816b
-000006d0: 6235 3162 6339 3535 6364 6433 6562 3434  b51bc955cdd3eb44
-000006e0: 3730 6535 3534 222c 0a20 2020 2020 2020  70e554",.       
-000006f0: 2020 2022 6c61 7965 7222 3a20 2272 6567     "layer": "reg
-00000700: 696f 6e22 2c0a 2020 2020 2020 2020 2020  ion",.          
-00000710: 2270 726f 6261 6269 6c69 7479 223a 2031  "probability": 1
-00000720: 2c0a 2020 2020 2020 2020 2020 2273 6f75  ,.          "sou
-00000730: 7263 6522 3a20 226d 6f64 656c 222c 0a20  rce": "model",. 
-00000740: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00000750: 3a20 2241 7369 6122 0a20 2020 2020 2020  : "Asia".       
-00000760: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00000770: 2020 2020 2020 2020 2269 6422 3a20 2230          "id": "0
-00000780: 3761 6330 3230 6161 3038 3264 3564 3131  7ac020aa082d5d11
-00000790: 3666 3832 3965 6632 3861 3430 6539 3837  6f829ef28a40e987
-000007a0: 3663 3036 3434 6165 6234 6630 3438 3032  6c0644aeb4f04802
-000007b0: 3032 6331 6138 3662 6238 6164 6637 6622  02c1a86bb8adf7f"
-000007c0: 2c0a 2020 2020 2020 2020 2020 226c 6179  ,.          "lay
-000007d0: 6572 223a 2022 7368 6970 7069 6e67 5f72  er": "shipping_r
-000007e0: 6567 696f 6e22 2c0a 2020 2020 2020 2020  egion",.        
-000007f0: 2020 2270 726f 6261 6269 6c69 7479 223a    "probability":
-00000800: 2031 2c0a 2020 2020 2020 2020 2020 2273   1,.          "s
-00000810: 6f75 7263 6522 3a20 226d 6f64 656c 222c  ource": "model",
-00000820: 0a20 2020 2020 2020 2020 2022 6c61 6265  .          "labe
-00000830: 6c22 3a20 2246 6172 2045 6173 7422 0a20  l": "Far East". 
-00000840: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000850: 2020 7b0a 2020 2020 2020 2020 2020 2269    {.          "i
-00000860: 6422 3a20 2232 6233 3934 6234 3161 3766  d": "2b394b41a7f
-00000870: 6639 6534 3862 3430 6234 6261 3865 3661  f9e48b40b4ba8e6a
-00000880: 3662 3034 3533 3430 3236 3164 6663 3032  6b045340261dfc02
-00000890: 3133 3364 3034 6166 3133 6665 3735 3461  133d04af13fe754a
-000008a0: 3731 6134 3822 2c0a 2020 2020 2020 2020  71a48",.        
-000008b0: 2020 226c 6179 6572 223a 2022 7368 6970    "layer": "ship
-000008c0: 7069 6e67 5f72 6567 696f 6e22 2c0a 2020  ping_region",.  
-000008d0: 2020 2020 2020 2020 2270 726f 6261 6269          "probabi
-000008e0: 6c69 7479 223a 2031 2c0a 2020 2020 2020  lity": 1,.      
-000008f0: 2020 2020 2273 6f75 7263 6522 3a20 226d      "source": "m
-00000900: 6f64 656c 222c 0a20 2020 2020 2020 2020  odel",.         
-00000910: 2022 6c61 6265 6c22 3a20 2245 6173 7420   "label": "East 
-00000920: 4173 6961 220a 2020 2020 2020 2020 7d2c  Asia".        },
-00000930: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00000940: 2020 2020 2022 6964 223a 2022 6136 3338       "id": "a638
-00000950: 3930 3236 3065 3239 6438 3539 3339 3066  90260e29d859390f
-00000960: 6431 6132 3363 3639 3031 3831 6166 6434  d1a23c690181afd4
-00000970: 6264 3135 3239 3433 6130 3463 3030 6364  bd152943a04c00cd
-00000980: 3661 3565 6366 3366 3764 3165 222c 0a20  6a5ecf3f7d1e",. 
-00000990: 2020 2020 2020 2020 2022 6c61 7965 7222           "layer"
-000009a0: 3a20 2273 6869 7070 696e 675f 7265 6769  : "shipping_regi
-000009b0: 6f6e 222c 0a20 2020 2020 2020 2020 2022  on",.          "
-000009c0: 7072 6f62 6162 696c 6974 7922 3a20 312c  probability": 1,
-000009d0: 0a20 2020 2020 2020 2020 2022 736f 7572  .          "sour
-000009e0: 6365 223a 2022 6d6f 6465 6c22 2c0a 2020  ce": "model",.  
-000009f0: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00000a00: 2022 4e6f 7274 6820 4368 696e 6122 0a20   "North China". 
-00000a10: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000a20: 2020 7b0a 2020 2020 2020 2020 2020 2269    {.          "i
-00000a30: 6422 3a20 2262 3566 6166 6365 3665 3230  d": "b5fafce6e20
-00000a40: 6465 3264 6333 3037 6662 3765 3062 3839  de2dc307fb7e0b89
-00000a50: 3937 3865 6539 3161 3439 6137 6236 6563  978ee91a49a7b6ec
-00000a60: 3666 3534 3631 6461 6632 3633 3366 3363  6f5461daf2633f3c
-00000a70: 3536 3637 3422 2c0a 2020 2020 2020 2020  56674",.        
-00000a80: 2020 226c 6179 6572 223a 2022 7368 6970    "layer": "ship
-00000a90: 7069 6e67 5f72 6567 696f 6e22 2c0a 2020  ping_region",.  
-00000aa0: 2020 2020 2020 2020 2270 726f 6261 6269          "probabi
-00000ab0: 6c69 7479 223a 2031 2c0a 2020 2020 2020  lity": 1,.      
-00000ac0: 2020 2020 2273 6f75 7263 6522 3a20 226d      "source": "m
-00000ad0: 6f64 656c 222c 0a20 2020 2020 2020 2020  odel",.         
-00000ae0: 2022 6c61 6265 6c22 3a20 2243 6869 6e61   "label": "China
-00000af0: 2028 6578 636c 2e20 484b 2026 204d 6163   (excl. HK & Mac
-00000b00: 6175 2922 0a20 2020 2020 2020 207d 2c0a  au)".        },.
-00000b10: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000b20: 2020 2020 2269 6422 3a20 2239 3536 6230      "id": "956b0
-00000b30: 3335 3239 3531 3034 3539 6432 3938 6334  3529510459d298c4
-00000b40: 6535 3337 6432 3363 3666 6262 3232 6666  e537d23c6fbb22ff
-00000b50: 6438 3431 3461 6639 3333 6233 3437 3533  d8414af933b34753
-00000b60: 3130 6336 3631 6633 3337 6122 2c0a 2020  10c661f337a",.  
-00000b70: 2020 2020 2020 2020 226c 6179 6572 223a          "layer":
-00000b80: 2022 7472 6164 696e 675f 626c 6f63 6b22   "trading_block"
-00000b90: 2c0a 2020 2020 2020 2020 2020 2270 726f  ,.          "pro
-00000ba0: 6261 6269 6c69 7479 223a 2031 2c0a 2020  bability": 1,.  
-00000bb0: 2020 2020 2020 2020 2273 6f75 7263 6522          "source"
-00000bc0: 3a20 226d 6f64 656c 222c 0a20 2020 2020  : "model",.     
-00000bd0: 2020 2020 2022 6c61 6265 6c22 3a20 224e       "label": "N
-00000be0: 6f6e 2d4f 5045 4322 0a20 2020 2020 2020  on-OPEC".       
-00000bf0: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00000c00: 2020 2020 2020 2020 2269 6422 3a20 2232          "id": "2
-00000c10: 6233 3934 6234 3161 3766 6639 6534 3862  b394b41a7ff9e48b
-00000c20: 3430 6234 6261 3865 3661 3662 3034 3533  40b4ba8e6a6b0453
-00000c30: 3430 3236 3164 6663 3032 3133 3364 3034  40261dfc02133d04
-00000c40: 6166 3133 6665 3735 3461 3731 6134 3822  af13fe754a71a48"
-00000c50: 2c0a 2020 2020 2020 2020 2020 226c 6179  ,.          "lay
-00000c60: 6572 223a 2022 7472 6164 696e 675f 7265  er": "trading_re
-00000c70: 6769 6f6e 222c 0a20 2020 2020 2020 2020  gion",.         
-00000c80: 2022 7072 6f62 6162 696c 6974 7922 3a20   "probability": 
-00000c90: 312c 0a20 2020 2020 2020 2020 2022 736f  1,.          "so
-00000ca0: 7572 6365 223a 2022 6d6f 6465 6c22 2c0a  urce": "model",.
-00000cb0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00000cc0: 223a 2022 4561 7374 2041 7369 6122 0a20  ": "East Asia". 
-00000cd0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000ce0: 2020 7b0a 2020 2020 2020 2020 2020 2269    {.          "i
-00000cf0: 6422 3a20 2238 3766 3864 3035 3965 6432  d": "87f8d059ed2
-00000d00: 6635 3763 3166 3534 6464 3838 3363 6230  f57c1f54dd883cb0
-00000d10: 6663 3930 6638 3336 3333 6437 3336 6637  fc90f83633d736f7
-00000d20: 3633 3938 3266 3235 3033 6636 6638 3033  63982f2503f6f803
-00000d30: 6562 3333 3322 2c0a 2020 2020 2020 2020  eb333",.        
-00000d40: 2020 226c 6179 6572 223a 2022 7472 6164    "layer": "trad
-00000d50: 696e 675f 7375 6272 6567 696f 6e22 2c0a  ing_subregion",.
-00000d60: 2020 2020 2020 2020 2020 2270 726f 6261            "proba
-00000d70: 6269 6c69 7479 223a 2031 2c0a 2020 2020  bility": 1,.    
-00000d80: 2020 2020 2020 2273 6f75 7263 6522 3a20        "source": 
-00000d90: 226d 6f64 656c 222c 0a20 2020 2020 2020  "model",.       
-00000da0: 2020 2022 6c61 6265 6c22 3a20 224c 6961     "label": "Lia
-00000db0: 6f6e 696e 6720 5072 6f76 696e 6365 220a  oning Province".
-00000dc0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000dd0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-00000de0: 6964 223a 2022 3937 3735 3733 6533 3738  id": "977573e378
-00000df0: 3234 3238 3736 3365 6466 3538 3062 6535  2428763edf580be5
-00000e00: 3363 3733 6237 6430 3431 3732 3033 3765  3c73b7d04172037e
-00000e10: 3664 3662 6138 3238 3265 6131 6465 3636  6d6ba8282ea1de66
-00000e20: 6464 3336 6362 222c 0a20 2020 2020 2020  dd36cb",.       
-00000e30: 2020 2022 6c61 7965 7222 3a20 2274 6572     "layer": "ter
-00000e40: 6d69 6e61 6c22 2c0a 2020 2020 2020 2020  minal",.        
-00000e50: 2020 2270 726f 6261 6269 6c69 7479 223a    "probability":
-00000e60: 2031 2c0a 2020 2020 2020 2020 2020 2273   1,.          "s
-00000e70: 6f75 7263 6522 3a20 226d 6f64 656c 222c  ource": "model",
-00000e80: 0a20 2020 2020 2020 2020 2022 6c61 6265  .          "labe
-00000e90: 6c22 3a20 2258 6961 6e72 656e 6461 6f20  l": "Xianrendao 
-00000ea0: 4372 7564 6520 4f69 6c20 5465 726d 696e  Crude Oil Termin
-00000eb0: 616c 220a 2020 2020 2020 2020 7d0a 2020  al".        }.  
-00000ec0: 2020 2020 5d2c 0a20 2020 2020 2022 706f      ],.      "po
-00000ed0: 7322 3a20 5b0a 2020 2020 2020 2020 3132  s": [.        12
-00000ee0: 312e 3935 3237 3131 3033 3039 3034 3233  1.95271103090423
-00000ef0: 2c0a 2020 2020 2020 2020 3430 2e32 3039  ,.        40.209
-00000f00: 3633 3731 3532 3939 3831 320a 2020 2020  63715299812.    
-00000f10: 2020 5d2c 0a20 2020 2020 2022 7374 6172    ],.      "star
-00000f20: 745f 7469 6d65 7374 616d 7022 3a20 2232  t_timestamp": "2
-00000f30: 3031 372d 3131 2d31 3954 3036 3a35 393a  017-11-19T06:59:
-00000f40: 3035 2b30 3030 3022 2c0a 2020 2020 2020  05+0000",.      
-00000f50: 2265 6e64 5f74 696d 6573 7461 6d70 223a  "end_timestamp":
-00000f60: 2022 3230 3137 2d31 312d 3231 5430 303a   "2017-11-21T00:
-00000f70: 3030 3a30 382b 3030 3030 222c 0a20 2020  00:08+0000",.   
-00000f80: 2020 2022 6576 656e 745f 7479 7065 223a     "event_type":
-00000f90: 2022 6469 7363 6861 7267 6522 0a20 2020   "discharge".   
-00000fa0: 207d 2c0a 2020 2020 2264 6573 7469 6e61   },.    "destina
-00000fb0: 7469 6f6e 223a 207b 0a20 2020 2020 2022  tion": {.      "
-00000fc0: 6576 656e 745f 6964 223a 2022 3438 3764  event_id": "487d
-00000fd0: 3365 6261 3763 6332 3937 3234 6365 3662  3eba7cc29724ce6b
-00000fe0: 3861 6361 3338 3232 6466 6265 3835 6561  8aca3822dfbe85ea
-00000ff0: 6130 6136 3135 3030 6333 6364 3566 6135  a0a61500c3cd5fa5
-00001000: 6637 3035 6266 3935 6338 3332 222c 0a20  f705bf95c832",. 
-00001010: 2020 2020 2022 6c6f 6361 7469 6f6e 223a       "location":
-00001020: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
-00001030: 2020 2020 2020 2022 6964 223a 2022 3933         "id": "93
-00001040: 3463 3437 6633 3663 3136 6135 3864 3638  4c47f36c16a58d68
-00001050: 6566 3565 3030 3765 3632 6132 3366 3566  ef5e007e62a23f5f
-00001060: 3033 3665 6533 6633 6431 6635 6638 3561  036ee3f3d1f5f85a
-00001070: 3438 6335 3732 6239 3061 6438 6232 222c  48c572b90ad8b2",
-00001080: 0a20 2020 2020 2020 2020 2022 6c61 7965  .          "laye
-00001090: 7222 3a20 2263 6f75 6e74 7279 222c 0a20  r": "country",. 
-000010a0: 2020 2020 2020 2020 2022 7072 6f62 6162           "probab
-000010b0: 696c 6974 7922 3a20 312c 0a20 2020 2020  ility": 1,.     
-000010c0: 2020 2020 2022 736f 7572 6365 223a 2022       "source": "
-000010d0: 6d6f 6465 6c22 2c0a 2020 2020 2020 2020  model",.        
-000010e0: 2020 226c 6162 656c 223a 2022 4368 696e    "label": "Chin
-000010f0: 6122 0a20 2020 2020 2020 207d 2c0a 2020  a".        },.  
-00001100: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00001110: 2020 2269 6422 3a20 2230 3536 3035 3461    "id": "056054a
-00001120: 3036 6433 3231 6532 3161 6338 3638 3535  06d321e21ac86855
-00001130: 3861 3039 3937 3531 6233 3234 6236 3735  8a099751b324b675
-00001140: 6530 3563 3131 6466 3763 3034 3163 3861  e05c11df7c041c8a
-00001150: 6430 6564 6635 3434 3522 2c0a 2020 2020  d0edf5445",.    
-00001160: 2020 2020 2020 226c 6179 6572 223a 2022        "layer": "
-00001170: 706f 7274 222c 0a20 2020 2020 2020 2020  port",.         
-00001180: 2022 7072 6f62 6162 696c 6974 7922 3a20   "probability": 
-00001190: 312c 0a20 2020 2020 2020 2020 2022 736f  1,.          "so
-000011a0: 7572 6365 223a 2022 6d6f 6465 6c22 2c0a  urce": "model",.
-000011b0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-000011c0: 223a 2022 4461 6c69 616e 205b 434e 5d22  ": "Dalian [CN]"
-000011d0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-000011e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000011f0: 2269 6422 3a20 2265 3639 3535 6132 6335  "id": "e6955a2c5
-00001200: 3964 6339 3038 3333 3938 3666 6530 3839  9dc90833986fe089
-00001210: 3463 6636 3731 3864 6464 6161 3738 3136  4cf6718dddaa7816
-00001220: 6262 3531 6263 3935 3563 6464 3365 6234  bb51bc955cdd3eb4
-00001230: 3437 3065 3535 3422 2c0a 2020 2020 2020  470e554",.      
-00001240: 2020 2020 226c 6179 6572 223a 2022 7265      "layer": "re
-00001250: 6769 6f6e 222c 0a20 2020 2020 2020 2020  gion",.         
-00001260: 2022 7072 6f62 6162 696c 6974 7922 3a20   "probability": 
-00001270: 312c 0a20 2020 2020 2020 2020 2022 736f  1,.          "so
-00001280: 7572 6365 223a 2022 6d6f 6465 6c22 2c0a  urce": "model",.
-00001290: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-000012a0: 223a 2022 4173 6961 220a 2020 2020 2020  ": "Asia".      
-000012b0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-000012c0: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-000012d0: 3037 6163 3032 3061 6130 3832 6435 6431  07ac020aa082d5d1
-000012e0: 3136 6638 3239 6566 3238 6134 3065 3938  16f829ef28a40e98
-000012f0: 3736 6330 3634 3461 6562 3466 3034 3830  76c0644aeb4f0480
-00001300: 3230 3263 3161 3836 6262 3861 6466 3766  202c1a86bb8adf7f
-00001310: 222c 0a20 2020 2020 2020 2020 2022 6c61  ",.          "la
-00001320: 7965 7222 3a20 2273 6869 7070 696e 675f  yer": "shipping_
-00001330: 7265 6769 6f6e 222c 0a20 2020 2020 2020  region",.       
-00001340: 2020 2022 7072 6f62 6162 696c 6974 7922     "probability"
-00001350: 3a20 312c 0a20 2020 2020 2020 2020 2022  : 1,.          "
-00001360: 736f 7572 6365 223a 2022 6d6f 6465 6c22  source": "model"
-00001370: 2c0a 2020 2020 2020 2020 2020 226c 6162  ,.          "lab
-00001380: 656c 223a 2022 4661 7220 4561 7374 220a  el": "Far East".
-00001390: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000013a0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-000013b0: 6964 223a 2022 3262 3339 3462 3431 6137  id": "2b394b41a7
-000013c0: 6666 3965 3438 6234 3062 3462 6138 6536  ff9e48b40b4ba8e6
-000013d0: 6136 6230 3435 3334 3032 3631 6466 6330  a6b045340261dfc0
-000013e0: 3231 3333 6430 3461 6631 3366 6537 3534  2133d04af13fe754
-000013f0: 6137 3161 3438 222c 0a20 2020 2020 2020  a71a48",.       
-00001400: 2020 2022 6c61 7965 7222 3a20 2273 6869     "layer": "shi
-00001410: 7070 696e 675f 7265 6769 6f6e 222c 0a20  pping_region",. 
-00001420: 2020 2020 2020 2020 2022 7072 6f62 6162           "probab
-00001430: 696c 6974 7922 3a20 312c 0a20 2020 2020  ility": 1,.     
-00001440: 2020 2020 2022 736f 7572 6365 223a 2022       "source": "
-00001450: 6d6f 6465 6c22 2c0a 2020 2020 2020 2020  model",.        
-00001460: 2020 226c 6162 656c 223a 2022 4561 7374    "label": "East
-00001470: 2041 7369 6122 0a20 2020 2020 2020 207d   Asia".        }
-00001480: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
-00001490: 2020 2020 2020 2269 6422 3a20 2261 3633        "id": "a63
-000014a0: 3839 3032 3630 6532 3964 3835 3933 3930  890260e29d859390
-000014b0: 6664 3161 3233 6336 3930 3138 3161 6664  fd1a23c690181afd
-000014c0: 3462 6431 3532 3934 3361 3034 6330 3063  4bd152943a04c00c
-000014d0: 6436 6135 6563 6633 6637 6431 6522 2c0a  d6a5ecf3f7d1e",.
-000014e0: 2020 2020 2020 2020 2020 226c 6179 6572            "layer
-000014f0: 223a 2022 7368 6970 7069 6e67 5f72 6567  ": "shipping_reg
-00001500: 696f 6e22 2c0a 2020 2020 2020 2020 2020  ion",.          
-00001510: 2270 726f 6261 6269 6c69 7479 223a 2031  "probability": 1
-00001520: 2c0a 2020 2020 2020 2020 2020 2273 6f75  ,.          "sou
-00001530: 7263 6522 3a20 226d 6f64 656c 222c 0a20  rce": "model",. 
-00001540: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001550: 3a20 224e 6f72 7468 2043 6869 6e61 220a  : "North China".
-00001560: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00001570: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-00001580: 6964 223a 2022 6235 6661 6663 6536 6532  id": "b5fafce6e2
-00001590: 3064 6532 6463 3330 3766 6237 6530 6238  0de2dc307fb7e0b8
-000015a0: 3939 3738 6565 3931 6134 3961 3762 3665  9978ee91a49a7b6e
-000015b0: 6336 6635 3436 3164 6166 3236 3333 6633  c6f5461daf2633f3
-000015c0: 6335 3636 3734 222c 0a20 2020 2020 2020  c56674",.       
-000015d0: 2020 2022 6c61 7965 7222 3a20 2273 6869     "layer": "shi
-000015e0: 7070 696e 675f 7265 6769 6f6e 222c 0a20  pping_region",. 
-000015f0: 2020 2020 2020 2020 2022 7072 6f62 6162           "probab
-00001600: 696c 6974 7922 3a20 312c 0a20 2020 2020  ility": 1,.     
-00001610: 2020 2020 2022 736f 7572 6365 223a 2022       "source": "
-00001620: 6d6f 6465 6c22 2c0a 2020 2020 2020 2020  model",.        
-00001630: 2020 226c 6162 656c 223a 2022 4368 696e    "label": "Chin
-00001640: 6120 2865 7863 6c2e 2048 4b20 2620 4d61  a (excl. HK & Ma
-00001650: 6361 7529 220a 2020 2020 2020 2020 7d2c  cau)".        },
-00001660: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
-00001670: 2020 2020 2022 6964 223a 2022 3935 3662       "id": "956b
-00001680: 3033 3532 3935 3130 3435 3964 3239 3863  03529510459d298c
-00001690: 3465 3533 3764 3233 6336 6662 6232 3266  4e537d23c6fbb22f
-000016a0: 6664 3834 3134 6166 3933 3362 3334 3735  fd8414af933b3475
-000016b0: 3331 3063 3636 3166 3333 3761 222c 0a20  310c661f337a",. 
+00000000: 6672 6f6d 2076 6f72 7465 7861 7364 6b2e  from vortexasdk.
+00000010: 6170 692e 766f 7961 6765 7320 696d 706f  api.voyages impo
+00000020: 7274 2028 0a20 2020 2056 6f79 6167 6543  rt (.    VoyageC
+00000030: 6172 676f 4576 656e 742c 0a20 2020 2056  argoEvent,.    V
+00000040: 6f79 6167 6553 7461 7475 7345 7665 6e74  oyageStatusEvent
+00000050: 2c0a 2020 2020 566f 7961 6765 5665 7373  ,.    VoyageVess
+00000060: 656c 4576 656e 742c 0a29 0a0a 0a63 6c61  elEvent,.)...cla
+00000070: 7373 2054 6573 7456 6f79 6167 6545 7665  ss TestVoyageEve
+00000080: 6e74 733a 0a20 2020 2064 6566 2074 6573  nts:.    def tes
+00000090: 745f 7365 7269 616c 697a 655f 766f 7961  t_serialize_voya
+000000a0: 6765 5f76 6573 7365 6c5f 6576 656e 7428  ge_vessel_event(
+000000b0: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+000000c0: 2020 2020 2020 2056 6f79 6167 6556 6573         VoyageVes
+000000d0: 7365 6c45 7665 6e74 2e6d 6f64 656c 5f76  selEvent.model_v
+000000e0: 616c 6964 6174 6528 0a20 2020 2020 2020  alidate(.       
+000000f0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000100: 2020 2020 2020 2022 6576 656e 745f 6964         "event_id
+00000110: 223a 2022 3966 6435 3931 3764 6336 3162  ": "9fd5917dc61b
+00000120: 3135 6434 6433 6161 3735 3861 6336 6335  15d4d3aa758ac6c5
+00000130: 6637 3564 3664 6462 3732 3338 6666 3731  f75d6ddb7238ff71
+00000140: 3434 3065 6365 6434 6138 6131 3134 3133  440eced4a8a11413
+00000150: 3436 6637 222c 0a20 2020 2020 2020 2020  46f7",.         
+00000160: 2020 2020 2020 2022 7374 6172 745f 7469         "start_ti
+00000170: 6d65 7374 616d 7022 3a20 2232 3032 322d  mestamp": "2022-
+00000180: 3037 2d31 3354 3030 3a30 303a 3030 2e30  07-13T00:00:00.0
+00000190: 3030 5a22 2c0a 2020 2020 2020 2020 2020  00Z",.          
+000001a0: 2020 2020 2020 2265 6e64 5f74 696d 6573        "end_times
+000001b0: 7461 6d70 223a 2022 3230 3232 2d30 372d  tamp": "2022-07-
+000001c0: 3239 5430 303a 3030 3a30 302e 3030 305a  29T00:00:00.000Z
+000001d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000001e0: 2020 2022 6576 656e 745f 6772 6f75 7022     "event_group"
+000001f0: 3a20 2276 6573 7365 6c22 2c0a 2020 2020  : "vessel",.    
+00000200: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00000210: 6e74 5f74 7970 6522 3a20 2266 6978 7475  nt_type": "fixtu
+00000220: 7265 222c 0a20 2020 2020 2020 2020 2020  re",.           
+00000230: 2020 2020 2022 6163 7469 7669 7479 223a       "activity":
+00000240: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00000250: 2020 2020 2020 2022 6f64 6f6d 6574 6572         "odometer
+00000260: 5f73 7461 7274 223a 2034 3736 3636 3236  _start": 4766626
+00000270: 3835 2c0a 2020 2020 2020 2020 2020 2020  85,.            
+00000280: 2020 2020 226f 646f 6d65 7465 725f 656e      "odometer_en
+00000290: 6422 3a20 3437 3636 3632 3638 352c 0a20  d": 476662685,. 
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000002b0: 6c6f 6361 7469 6f6e 5f69 6422 3a20 2230  location_id": "0
+000002c0: 3031 3130 3031 3130 3031 3130 3031 3122  011001100110011"
+000002d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000002e0: 2020 226c 6f63 6174 696f 6e5f 6c61 7965    "location_laye
+000002f0: 7222 3a20 5b22 726f 6f74 225d 2c0a 2020  r": ["root"],.  
+00000300: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00000310: 6f63 6174 696f 6e5f 6465 7461 696c 7322  ocation_details"
+00000320: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+00000330: 2020 2020 2020 2263 6172 676f 5f6d 6f76        "cargo_mov
+00000340: 656d 656e 745f 6964 223a 205b 5d2c 0a20  ement_id": [],. 
+00000350: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000360: 7374 735f 6576 656e 745f 636f 756e 7465  sts_event_counte
+00000370: 7270 6172 7479 5f76 6573 7365 6c5f 6964  rparty_vessel_id
+00000380: 223a 204e 6f6e 652c 0a20 2020 2020 2020  ": None,.       
+00000390: 2020 2020 2020 2020 2022 7761 6974 696e           "waitin
+000003a0: 675f 6576 656e 745f 7461 7267 6574 5f67  g_event_target_g
+000003b0: 656f 6772 6170 6879 5f69 6422 3a20 4e6f  eography_id": No
+000003c0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+000003d0: 2020 2020 2277 6169 7469 6e67 5f65 7665      "waiting_eve
+000003e0: 6e74 5f74 6172 6765 745f 6765 6f67 7261  nt_target_geogra
+000003f0: 7068 795f 6465 7461 696c 7322 3a20 5b5d  phy_details": []
+00000400: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000410: 2020 2266 6978 7475 7265 5f65 7665 6e74    "fixture_event
+00000420: 5f66 6978 696e 675f 7469 6d65 7374 616d  _fixing_timestam
+00000430: 7022 3a20 2232 3032 322d 3037 2d31 3354  p": "2022-07-13T
+00000440: 3030 3a30 303a 3030 2e30 3030 5a22 2c0a  00:00:00.000Z",.
+00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000460: 2274 6167 7322 3a20 5b5d 2c0a 2020 2020  "tags": [],.    
+00000470: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
+00000480: 6261 6269 6c69 7479 223a 2031 2c0a 2020  bability": 1,.  
+00000490: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000004a0: 2020 2020 290a 0a20 2020 2064 6566 2074      )..    def t
+000004b0: 6573 745f 7365 7269 616c 697a 655f 766f  est_serialize_vo
+000004c0: 7961 6765 5f73 7461 7475 735f 6576 656e  yage_status_even
+000004d0: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
+000004e0: 0a20 2020 2020 2020 2056 6f79 6167 6553  .        VoyageS
+000004f0: 7461 7475 7345 7665 6e74 2e6d 6f64 656c  tatusEvent.model
+00000500: 5f76 616c 6964 6174 6528 0a20 2020 2020  _validate(.     
+00000510: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000520: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
+00000530: 6964 223a 2022 3762 6266 3561 6233 3664  id": "7bbf5ab36d
+00000540: 3933 6339 3935 222c 0a20 2020 2020 2020  93c995",.       
+00000550: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
+00000560: 6772 6f75 7022 3a20 2264 6572 6976 6564  group": "derived
+00000570: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000580: 2020 2022 6576 656e 745f 7479 7065 223a     "event_type":
+00000590: 2022 7374 6174 7573 222c 0a20 2020 2020   "status",.     
+000005a0: 2020 2020 2020 2020 2020 2022 6163 7469             "acti
+000005b0: 7669 7479 223a 2022 636f 6d6d 6974 6d65  vity": "commitme
+000005c0: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
+000005d0: 2020 2020 2022 7374 6172 745f 7469 6d65       "start_time
+000005e0: 7374 616d 7022 3a20 2232 3032 322d 3037  stamp": "2022-07
+000005f0: 2d31 3354 3030 3a30 303a 3030 2e30 3030  -13T00:00:00.000
+00000600: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
+00000610: 2020 2020 2265 6e64 5f74 696d 6573 7461      "end_timesta
+00000620: 6d70 223a 2022 3230 3232 2d30 372d 3239  mp": "2022-07-29
+00000630: 5430 303a 3030 3a30 302e 3030 305a 222c  T00:00:00.000Z",
+00000640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000650: 2022 6973 5f6f 7065 6e5f 6576 656e 7422   "is_open_event"
+00000660: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00000670: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+00000680: 3a20 2263 6f6d 6d69 7474 6564 222c 0a20  : "committed",. 
+00000690: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000006a0: 736f 7572 6365 5f65 7665 6e74 5f69 6422  source_event_id"
+000006b0: 3a20 2239 6664 3539 3137 6463 3631 6231  : "9fd5917dc61b1
+000006c0: 3564 3422 2c0a 2020 2020 2020 2020 2020  5d4",.          
+000006d0: 2020 7d0a 2020 2020 2020 2020 290a 0a20    }.        ).. 
+000006e0: 2020 2064 6566 2074 6573 745f 7365 7269     def test_seri
+000006f0: 616c 697a 655f 766f 7961 6765 5f63 6172  alize_voyage_car
+00000700: 676f 5f65 7665 6e74 2873 656c 6629 202d  go_event(self) -
+00000710: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00000720: 566f 7961 6765 4361 7267 6f45 7665 6e74  VoyageCargoEvent
+00000730: 2e6d 6f64 656c 5f76 616c 6964 6174 6528  .model_validate(
+00000740: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+00000750: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000760: 6576 656e 745f 6964 223a 2022 3238 3333  event_id": "2833
+00000770: 3037 6661 3836 3432 3962 6163 222c 0a20  07fa86429bac",. 
+00000780: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000790: 7374 6172 745f 7469 6d65 7374 616d 7022  start_timestamp"
+000007a0: 3a20 2232 3032 322d 3037 2d31 3354 3230  : "2022-07-13T20
+000007b0: 3a35 353a 3537 2e30 3030 5a22 2c0a 2020  :55:57.000Z",.  
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+000007d0: 6e64 5f74 696d 6573 7461 6d70 223a 2022  nd_timestamp": "
+000007e0: 3230 3232 2d30 382d 3234 5430 323a 3235  2022-08-24T02:25
+000007f0: 3a32 372e 3030 305a 222c 0a20 2020 2020  :27.000Z",.     
+00000800: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00000810: 745f 6772 6f75 7022 3a20 2264 6572 6976  t_group": "deriv
+00000820: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
+00000830: 2020 2020 2022 6576 656e 745f 7479 7065       "event_type
+00000840: 223a 2022 6361 7267 6f22 2c0a 2020 2020  ": "cargo",.    
+00000850: 2020 2020 2020 2020 2020 2020 226f 646f              "odo
+00000860: 6d65 7465 725f 7374 6172 7422 3a20 3436  meter_start": 46
+00000870: 3932 3830 3738 382c 0a20 2020 2020 2020  9280788,.       
+00000880: 2020 2020 2020 2020 2022 6f64 6f6d 6574           "odomet
+00000890: 6572 5f65 6e64 223a 2034 3833 3834 3031  er_end": 4838401
+000008a0: 3431 2c0a 2020 2020 2020 2020 2020 2020  41,.            
+000008b0: 2020 2020 2263 6172 676f 5f6d 6f76 656d      "cargo_movem
+000008c0: 656e 745f 6964 223a 2022 6164 6437 6331  ent_id": "add7c1
+000008d0: 6162 6666 3064 3764 3631 222c 0a20 2020  abff0d7d61",.   
+000008e0: 2020 2020 2020 2020 2020 2020 2022 6361               "ca
+000008f0: 7267 6f5f 6f72 6967 696e 5f69 6422 3a20  rgo_origin_id": 
+00000900: 2230 3164 6163 3262 6664 3533 6630 3565  "01dac2bfd53f05e
+00000910: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
+00000920: 2020 2020 2263 6172 676f 5f6f 7269 6769      "cargo_origi
+00000930: 6e5f 6465 7461 696c 7322 3a20 5b0a 2020  n_details": [.  
+00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000950: 2020 7b22 6c61 7965 7222 3a20 2262 6572    {"layer": "ber
+00000960: 7468 222c 2022 6964 223a 2022 3031 6461  th", "id": "01da
+00000970: 6332 6266 6435 3366 3035 6566 227d 2c0a  c2bfd53f05ef"},.
+00000980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000990: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+000009b0: 6422 3a20 2261 6332 6234 3964 3265 3532  d": "ac2b49d2e52
+000009c0: 6662 3331 6222 2c0a 2020 2020 2020 2020  fb31b",.        
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 226c 6179 6572 223a 2022 7465 726d 696e  "layer": "termin
+000009f0: 616c 222c 0a20 2020 2020 2020 2020 2020  al",.           
+00000a00: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
+00000a10: 6265 6c22 3a20 2254 7261 6e73 6e65 6674  bel": "Transneft
+00000a20: 202d 2050 6f72 7420 5072 696d 6f72 736b   - Port Primorsk
+00000a30: 2028 4372 7564 6529 2028 4578 2d42 616c   (Crude) (Ex-Bal
+00000a40: 7469 6320 5069 7065 6c69 6e65 2053 7973  tic Pipeline Sys
+00000a50: 7465 6d29 222c 0a20 2020 2020 2020 2020  tem)",.         
+00000a60: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00000a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a80: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00000a90: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00000aa0: 3a20 2234 3533 3463 6535 3236 3761 3436  : "4534ce5267a46
+00000ab0: 3830 3422 2c0a 2020 2020 2020 2020 2020  804",.          
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00000ad0: 6179 6572 223a 2022 706f 7274 222c 0a20  ayer": "port",. 
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00000b00: 2250 7269 6d6f 7273 6b20 284b 6f69 7669  "Primorsk (Koivi
+00000b10: 7374 6f29 205b 5255 5d22 2c0a 2020 2020  sto) [RU]",.    
+00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b30: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00000b40: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2022 6964 223a 2022 6239 3936 3532 3162   "id": "b996521b
+00000b70: 6539 6339 3936 6462 222c 0a20 2020 2020  e9c996db",.     
+00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b90: 2020 2022 6c61 7965 7222 3a20 2263 6f75     "layer": "cou
+00000ba0: 6e74 7279 222c 0a20 2020 2020 2020 2020  ntry",.         
+00000bb0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000bc0: 6c61 6265 6c22 3a20 2252 7573 7369 6122  label": "Russia"
+00000bd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000be0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000bf0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c10: 2020 2020 2020 2022 6964 223a 2022 3038         "id": "08
+00000c20: 3261 3839 3030 6633 3130 6661 3039 222c  2a8900f310fa09",
+00000c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c40: 2020 2020 2020 2020 2022 6c61 7965 7222           "layer"
+00000c50: 3a20 2273 6869 7070 696e 675f 7265 6769  : "shipping_regi
+00000c60: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+00000c70: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
+00000c80: 6265 6c22 3a20 2242 616c 7469 6322 2c0a  bel": "Baltic",.
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ca0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000cb0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cd0: 2020 2020 2022 6964 223a 2022 6239 3936       "id": "b996
+00000ce0: 3532 3162 6539 6339 3936 6462 222c 0a20  521be9c996db",. 
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d00: 2020 2020 2020 2022 6c61 7965 7222 3a20         "layer": 
+00000d10: 2272 6567 696f 6e22 2c0a 2020 2020 2020  "region",.      
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 2020 226c 6162 656c 223a 2022 5275 7373    "label": "Russ
+00000d40: 6961 222c 0a20 2020 2020 2020 2020 2020  ia",.           
+00000d50: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000d80: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+00000d90: 2261 3735 3336 6334 3837 3134 3134 3063  "a7536c48714140c
+00000da0: 3722 2c0a 2020 2020 2020 2020 2020 2020  7",.            
+00000db0: 2020 2020 2020 2020 2020 2020 226c 6179              "lay
+00000dc0: 6572 223a 2022 7472 6164 696e 675f 626c  er": "trading_bl
+00000dd0: 6f63 6b22 2c0a 2020 2020 2020 2020 2020  ock",.          
+00000de0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00000df0: 6162 656c 223a 2022 4f50 4543 202b 2052  abel": "OPEC + R
+00000e00: 7573 7369 6122 2c0a 2020 2020 2020 2020  ussia",.        
+00000e10: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000e40: 2020 2020 2020 2020 2020 2020 2022 6964               "id
+00000e50: 223a 2022 3163 3437 6530 3965 6266 3733  ": "1c47e09ebf73
+00000e60: 6362 6230 222c 0a20 2020 2020 2020 2020  cbb0",.         
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000e80: 6c61 7965 7222 3a20 2274 7261 6469 6e67  layer": "trading
+00000e90: 5f62 6c6f 636b 222c 0a20 2020 2020 2020  _block",.       
+00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000eb0: 2022 6c61 6265 6c22 3a20 224f 5045 432b   "label": "OPEC+
+00000ec0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000ed0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f00: 2020 2020 2020 2020 2269 6422 3a20 2263          "id": "c
+00000f10: 6534 3937 3861 3730 6635 3733 3936 6622  e4978a70f57396f"
+00000f20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000f30: 2020 2020 2020 2020 2020 226c 6179 6572            "layer
+00000f40: 223a 2022 7472 6164 696e 675f 626c 6f63  ": "trading_bloc
+00000f50: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
+00000f60: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+00000f70: 656c 223a 2022 4653 5522 2c0a 2020 2020  el": "FSU",.    
+00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f90: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00000fa0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fc0: 2022 6964 223a 2022 3935 3662 3033 3532   "id": "956b0352
+00000fd0: 3935 3130 3435 3964 222c 0a20 2020 2020  9510459d",.     
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ff0: 2020 2022 6c61 7965 7222 3a20 2274 7261     "layer": "tra
+00001000: 6469 6e67 5f62 6c6f 636b 222c 0a20 2020  ding_block",.   
+00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001020: 2020 2020 2022 6c61 6265 6c22 3a20 224e       "label": "N
+00001030: 6f6e 2d4f 5045 4322 2c0a 2020 2020 2020  on-OPEC",.      
+00001040: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00001050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001060: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001070: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001080: 6964 223a 2022 3634 3738 3130 3561 3832  id": "6478105a82
+00001090: 6664 3332 6531 222c 0a20 2020 2020 2020  fd32e1",.       
+000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010b0: 2022 6c61 7965 7222 3a20 2274 7261 6469   "layer": "tradi
+000010c0: 6e67 5f62 6c6f 636b 222c 0a20 2020 2020  ng_block",.     
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 2022 6c61 6265 6c22 3a20 2257 6573     "label": "Wes
+000010f0: 7420 6f66 2053 7565 7a22 2c0a 2020 2020  t of Suez",.    
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00001120: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001140: 2022 6964 223a 2022 3863 6161 3332 6162   "id": "8caa32ab
+00001150: 3735 6137 3066 3239 222c 0a20 2020 2020  75a70f29",.     
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 2022 6c61 7965 7222 3a20 2274 7261     "layer": "tra
+00001180: 6469 6e67 5f72 6567 696f 6e22 2c0a 2020  ding_region",.  
+00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011a0: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+000011b0: 4261 6c74 6963 7322 2c0a 2020 2020 2020  Baltics",.      
+000011c0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+000011d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011e0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001200: 6964 223a 2022 6334 3865 6335 3939 3433  id": "c48ec59943
+00001210: 3130 3237 6436 222c 0a20 2020 2020 2020  1027d6",.       
+00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001230: 2022 6c61 7965 7222 3a20 2274 7261 6469   "layer": "tradi
+00001240: 6e67 5f73 7562 7265 6769 6f6e 222c 0a20  ng_subregion",. 
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00001270: 2252 7573 7369 6120 4261 6c74 6963 7322  "Russia Baltics"
+00001280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001290: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000012a0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012c0: 2020 2020 2020 2022 6964 223a 2022 3435         "id": "45
+000012d0: 3334 6365 3532 3637 6134 3638 3034 222c  34ce5267a46804",
+000012e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000012f0: 2020 2020 2020 2020 2022 6c61 7965 7222           "layer"
+00001300: 3a20 2273 746f 7261 6765 222c 0a20 2020  : "storage",.   
+00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001320: 2020 2020 2022 6c61 6265 6c22 3a20 2250       "label": "P
+00001330: 7269 6d6f 7273 6b20 284b 6f69 7669 7374  rimorsk (Koivist
+00001340: 6f29 205b 5255 5d22 2c0a 2020 2020 2020  o) [RU]",.      
+00001350: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00001360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001370: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00001380: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001390: 6964 223a 2022 3561 3431 3865 3034 3537  id": "5a418e0457
+000013a0: 6335 6334 6663 222c 0a20 2020 2020 2020  c5c4fc",.       
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 2022 6c61 7965 7222 3a20 2266 7261 676d   "layer": "fragm
+000013d0: 656e 7422 2c0a 2020 2020 2020 2020 2020  ent",.          
+000013e0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+000013f0: 6162 656c 223a 2022 5275 7373 6961 2042  abel": "Russia B
+00001400: 616c 7469 6373 2028 4261 6c74 6963 2920  altics (Baltic) 
+00001410: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+00001420: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001430: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+00001440: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00001450: 6172 676f 5f64 6573 7469 6e61 7469 6f6e  argo_destination
+00001460: 5f69 6422 3a20 2234 3730 6163 3661 3830  _id": "470ac6a80
+00001470: 3737 6531 3438 3022 2c0a 2020 2020 2020  77e1480",.      
+00001480: 2020 2020 2020 2020 2020 2263 6172 676f            "cargo
+00001490: 5f64 6573 7469 6e61 7469 6f6e 5f64 6574  _destination_det
+000014a0: 6169 6c73 223a 205b 0a20 2020 2020 2020  ails": [.       
+000014b0: 2020 2020 2020 2020 2020 2020 207b 226c               {"l
+000014c0: 6179 6572 223a 2022 6265 7274 6822 2c20  ayer": "berth", 
+000014d0: 2269 6422 3a20 2234 3730 6163 3661 3830  "id": "470ac6a80
+000014e0: 3737 6531 3438 3022 7d2c 0a20 2020 2020  77e1480"},.     
+000014f0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00001500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001510: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+00001520: 3331 3038 6531 3165 6236 3138 6464 3533  3108e11eb618dd53
+00001530: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001540: 2020 2020 2020 2020 2020 2022 6c61 7965             "laye
+00001550: 7222 3a20 2274 6572 6d69 6e61 6c22 2c0a  r": "terminal",.
+00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001570: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
+00001580: 2022 4a61 6d6e 6167 6172 2052 656c 6961   "Jamnagar Relia
+00001590: 6e63 6520 5370 6d73 222c 0a20 2020 2020  nce Spms",.     
+000015a0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000015b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000015c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015e0: 2269 6422 3a20 2261 3037 6561 6130 3330  "id": "a07eaa030
+000015f0: 6266 6539 3235 6522 2c0a 2020 2020 2020  bfe925e",.      
+00001600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001610: 2020 226c 6179 6572 223a 2022 706f 7274    "layer": "port
+00001620: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001630: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+00001640: 6c22 3a20 2253 696b 6b61 205b 494e 5d22  l": "Sikka [IN]"
+00001650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001660: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001670: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001690: 2020 2020 2020 2022 6964 223a 2022 3730         "id": "70
+000016a0: 3432 3533 3733 6131 3833 3664 3664 222c  425373a1836d6d",
+000016b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000016c0: 2020 2020 2020 2020 2022 6c61 7965 7222           "layer"
-000016d0: 3a20 2274 7261 6469 6e67 5f62 6c6f 636b  : "trading_block
-000016e0: 222c 0a20 2020 2020 2020 2020 2022 7072  ",.          "pr
-000016f0: 6f62 6162 696c 6974 7922 3a20 312c 0a20  obability": 1,. 
-00001700: 2020 2020 2020 2020 2022 736f 7572 6365           "source
-00001710: 223a 2022 6d6f 6465 6c22 2c0a 2020 2020  ": "model",.    
-00001720: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
-00001730: 4e6f 6e2d 4f50 4543 220a 2020 2020 2020  Non-OPEC".      
-00001740: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00001750: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-00001760: 3262 3339 3462 3431 6137 6666 3965 3438  2b394b41a7ff9e48
-00001770: 6234 3062 3462 6138 6536 6136 6230 3435  b40b4ba8e6a6b045
-00001780: 3334 3032 3631 6466 6330 3231 3333 6430  340261dfc02133d0
-00001790: 3461 6631 3366 6537 3534 6137 3161 3438  4af13fe754a71a48
-000017a0: 222c 0a20 2020 2020 2020 2020 2022 6c61  ",.          "la
-000017b0: 7965 7222 3a20 2274 7261 6469 6e67 5f72  yer": "trading_r
-000017c0: 6567 696f 6e22 2c0a 2020 2020 2020 2020  egion",.        
-000017d0: 2020 2270 726f 6261 6269 6c69 7479 223a    "probability":
-000017e0: 2031 2c0a 2020 2020 2020 2020 2020 2273   1,.          "s
-000017f0: 6f75 7263 6522 3a20 226d 6f64 656c 222c  ource": "model",
-00001800: 0a20 2020 2020 2020 2020 2022 6c61 6265  .          "labe
-00001810: 6c22 3a20 2245 6173 7420 4173 6961 220a  l": "East Asia".
-00001820: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00001830: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-00001840: 6964 223a 2022 3837 6638 6430 3539 6564  id": "87f8d059ed
-00001850: 3266 3537 6331 6635 3464 6438 3833 6362  2f57c1f54dd883cb
-00001860: 3066 6339 3066 3833 3633 3364 3733 3666  0fc90f83633d736f
-00001870: 3736 3339 3832 6632 3530 3366 3666 3830  763982f2503f6f80
-00001880: 3365 6233 3333 222c 0a20 2020 2020 2020  3eb333",.       
-00001890: 2020 2022 6c61 7965 7222 3a20 2274 7261     "layer": "tra
-000018a0: 6469 6e67 5f73 7562 7265 6769 6f6e 222c  ding_subregion",
-000018b0: 0a20 2020 2020 2020 2020 2022 7072 6f62  .          "prob
-000018c0: 6162 696c 6974 7922 3a20 312c 0a20 2020  ability": 1,.   
-000018d0: 2020 2020 2020 2022 736f 7572 6365 223a         "source":
-000018e0: 2022 6d6f 6465 6c22 2c0a 2020 2020 2020   "model",.      
-000018f0: 2020 2020 226c 6162 656c 223a 2022 4c69      "label": "Li
-00001900: 616f 6e69 6e67 2050 726f 7669 6e63 6522  aoning Province"
-00001910: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00001920: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00001930: 2269 6422 3a20 2265 3436 3934 6162 6661  "id": "e4694abfa
-00001940: 6434 3866 3931 3335 6364 6436 3633 3465  d48f9135cdd6634e
-00001950: 6262 3036 3234 6333 6139 3130 3937 6663  bb0624c3a91097fc
-00001960: 3865 3833 6230 3834 3734 3764 3562 6462  8e83b084747d5bdb
-00001970: 6438 6332 6338 6522 2c0a 2020 2020 2020  d8c2c8e",.      
-00001980: 2020 2020 226c 6179 6572 223a 2022 7465      "layer": "te
-00001990: 726d 696e 616c 222c 0a20 2020 2020 2020  rminal",.       
-000019a0: 2020 2022 7072 6f62 6162 696c 6974 7922     "probability"
-000019b0: 3a20 312c 0a20 2020 2020 2020 2020 2022  : 1,.          "
-000019c0: 736f 7572 6365 223a 2022 6d6f 6465 6c22  source": "model"
-000019d0: 2c0a 2020 2020 2020 2020 2020 226c 6162  ,.          "lab
-000019e0: 656c 223a 2022 4461 6c69 616e 2058 696e  el": "Dalian Xin
-000019f0: 6761 6e67 204f 696c 2054 6572 6d69 6e61  gang Oil Termina
-00001a00: 6c22 0a20 2020 2020 2020 207d 0a20 2020  l".        }.   
-00001a10: 2020 205d 2c0a 2020 2020 2020 2270 6f73     ],.      "pos
-00001a20: 223a 205b 0a20 2020 2020 2020 2031 3231  ": [.        121
-00001a30: 2e39 3130 3732 3337 3135 3538 3931 2c0a  .9107237155891,.
-00001a40: 2020 2020 2020 2020 3338 2e39 3635 3137          38.96517
-00001a50: 3832 3133 3032 3632 3036 0a20 2020 2020  8213026206.     
-00001a60: 205d 2c0a 2020 2020 2020 2273 7461 7274   ],.      "start
-00001a70: 5f74 696d 6573 7461 6d70 223a 2022 3230  _timestamp": "20
-00001a80: 3137 2d31 312d 3237 5430 363a 3339 3a35  17-11-27T06:39:5
-00001a90: 302b 3030 3030 222c 0a20 2020 2020 2022  0+0000",.      "
-00001aa0: 656e 645f 7469 6d65 7374 616d 7022 3a20  end_timestamp": 
-00001ab0: 2232 3031 372d 3131 2d32 3954 3032 3a34  "2017-11-29T02:4
-00001ac0: 393a 3332 2b30 3030 3022 2c0a 2020 2020  9:32+0000",.    
-00001ad0: 2020 2265 7665 6e74 5f74 7970 6522 3a20    "event_type": 
-00001ae0: 2264 6973 6368 6172 6765 220a 2020 2020  "discharge".    
-00001af0: 7d2c 0a20 2020 2022 6361 7267 6f65 7322  },.    "cargoes"
-00001b00: 3a20 5b0a 2020 2020 2020 7b0a 2020 2020  : [.      {.    
-00001b10: 2020 2020 2263 6172 676f 5f6d 6f76 656d      "cargo_movem
-00001b20: 656e 745f 6964 223a 2022 3132 6264 3738  ent_id": "12bd78
-00001b30: 3437 3831 6363 3038 3264 3739 6236 6433  4781cc082d79b6d3
-00001b40: 6336 3530 3839 3539 3663 3338 3464 6131  c65089596c384da1
-00001b50: 3932 6166 3135 3438 3732 3665 6665 3230  92af1548726efe20
-00001b60: 3434 3530 6366 3938 3831 222c 0a20 2020  4450cf9881",.   
-00001b70: 2020 2020 2022 7175 616e 7469 7479 223a       "quantity":
-00001b80: 2032 3930 3639 322c 0a20 2020 2020 2020   290692,.       
-00001b90: 2022 7072 6f64 7563 7422 3a20 5b0a 2020   "product": [.  
-00001ba0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00001bb0: 2020 2020 2020 2269 6422 3a20 2236 6631        "id": "6f1
-00001bc0: 3162 3037 3234 6339 6134 6538 3566 6661  1b0724c9a4e85ffa
-00001bd0: 3766 3134 3435 6263 3736 3866 3035 3461  7f1445bc768f054a
-00001be0: 6637 3535 6130 3930 3131 3864 6366 3939  f755a090118dcf99
-00001bf0: 6631 3437 3435 6332 3631 3635 3322 2c0a  f14745c261653",.
-00001c00: 2020 2020 2020 2020 2020 2020 226c 6179              "lay
-00001c10: 6572 223a 2022 6772 6f75 7022 2c0a 2020  er": "group",.  
-00001c20: 2020 2020 2020 2020 2020 2270 726f 6261            "proba
-00001c30: 6269 6c69 7479 223a 2031 2c0a 2020 2020  bility": 1,.    
-00001c40: 2020 2020 2020 2020 2273 6f75 7263 6522          "source"
-00001c50: 3a20 2265 7874 6572 6e61 6c22 2c0a 2020  : "external",.  
-00001c60: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00001c70: 223a 2022 4372 7564 6522 0a20 2020 2020  ": "Crude".     
-00001c80: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001c90: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00001ca0: 2269 6422 3a20 2236 6631 3162 3037 3234  "id": "6f11b0724
-00001cb0: 6339 6134 6538 3566 6661 3766 3134 3435  c9a4e85ffa7f1445
-00001cc0: 6263 3736 3866 3035 3461 6637 3535 6130  bc768f054af755a0
-00001cd0: 3930 3131 3864 6366 3939 6631 3437 3435  90118dcf99f14745
-00001ce0: 6332 3631 3635 3322 2c0a 2020 2020 2020  c261653",.      
-00001cf0: 2020 2020 2020 226c 6179 6572 223a 2022        "layer": "
-00001d00: 6772 6f75 705f 7072 6f64 7563 7422 2c0a  group_product",.
-00001d10: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
-00001d20: 6261 6269 6c69 7479 223a 2031 2c0a 2020  bability": 1,.  
-00001d30: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
-00001d40: 6522 3a20 2265 7874 6572 6e61 6c22 2c0a  e": "external",.
-00001d50: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
-00001d60: 656c 223a 2022 4372 7564 6522 0a20 2020  el": "Crude".   
-00001d70: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00001d80: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00001d90: 2020 2269 6422 3a20 2261 3765 3236 3935    "id": "a7e2695
-00001da0: 3666 6262 3931 6437 3836 6231 6435 3535  6fbb91d786b1d555
-00001db0: 3832 3938 3162 3064 3139 3966 3732 6330  82981b0d199f72c0
-00001dc0: 3530 3935 3866 6433 3530 3162 3339 3931  50958fd3501b3991
-00001dd0: 6432 3465 6661 3264 3222 2c0a 2020 2020  d24efa2d2",.    
-00001de0: 2020 2020 2020 2020 226c 6179 6572 223a          "layer":
-00001df0: 2022 6361 7465 676f 7279 222c 0a20 2020   "category",.   
-00001e00: 2020 2020 2020 2020 2022 7072 6f62 6162           "probab
-00001e10: 696c 6974 7922 3a20 312c 0a20 2020 2020  ility": 1,.     
-00001e20: 2020 2020 2020 2022 736f 7572 6365 223a         "source":
-00001e30: 2022 6578 7465 726e 616c 222c 0a20 2020   "external",.   
-00001e40: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001e50: 3a20 224d 6564 6975 6d2d 536f 7572 220a  : "Medium-Sour".
-00001e60: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00001e70: 2020 2020 5d0a 2020 2020 2020 7d0a 2020      ].      }.  
-00001e80: 2020 5d0a 2020 7d0a 5d0a                   ].  }.].
+000016d0: 3a20 2263 6f75 6e74 7279 222c 0a20 2020  : "country",.   
+000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016f0: 2020 2020 2022 6c61 6265 6c22 3a20 2249       "label": "I
+00001700: 6e64 6961 222c 0a20 2020 2020 2020 2020  ndia",.         
+00001710: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001730: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00001740: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00001750: 3a20 2232 6632 3334 3231 3534 3564 6162  : "2f23421545dab
+00001760: 6631 3722 2c0a 2020 2020 2020 2020 2020  f17",.          
+00001770: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00001780: 6179 6572 223a 2022 7368 6970 7069 6e67  ayer": "shipping
+00001790: 5f72 6567 696f 6e22 2c0a 2020 2020 2020  _region",.      
+000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017b0: 2020 226c 6162 656c 223a 2022 5765 7374    "label": "West
+000017c0: 2043 6f61 7374 2049 6e64 6961 222c 0a20   Coast India",. 
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017e0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+000017f0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 2269 6422 3a20 2265 3639 3535      "id": "e6955
+00001820: 6132 6335 3964 6339 3038 3322 2c0a 2020  a2c59dc9083",.  
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 2020 2020 2020 226c 6179 6572 223a 2022        "layer": "
+00001850: 7265 6769 6f6e 222c 0a20 2020 2020 2020  region",.       
+00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001870: 2022 6c61 6265 6c22 3a20 2241 7369 6122   "label": "Asia"
+00001880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001890: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000018a0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 2020 2020 2022 6964 223a 2022 3935         "id": "95
+000018d0: 3662 3033 3532 3935 3130 3435 3964 222c  6b03529510459d",
+000018e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018f0: 2020 2020 2020 2020 2022 6c61 7965 7222           "layer"
+00001900: 3a20 2274 7261 6469 6e67 5f62 6c6f 636b  : "trading_block
+00001910: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001920: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+00001930: 6c22 3a20 224e 6f6e 2d4f 5045 4322 2c0a  l": "Non-OPEC",.
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00001960: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001980: 2020 2020 2022 6964 223a 2022 6663 3636       "id": "fc66
+00001990: 3934 3734 3265 6263 6534 3966 222c 0a20  94742ebce49f",. 
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 2020 2020 2022 6c61 7965 7222 3a20         "layer": 
+000019c0: 2274 7261 6469 6e67 5f62 6c6f 636b 222c  "trading_block",
+000019d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000019e0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+000019f0: 3a20 2245 6173 7420 6f66 2053 7565 7a22  : "East of Suez"
+00001a00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001a10: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001a20: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a40: 2020 2020 2020 2022 6964 223a 2022 3034         "id": "04
+00001a50: 3362 3362 3061 6362 3033 3935 3134 222c  3b3b0acb039514",
+00001a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a70: 2020 2020 2020 2020 2022 6c61 7965 7222           "layer"
+00001a80: 3a20 2274 7261 6469 6e67 5f72 6567 696f  : "trading_regio
+00001a90: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+00001aa0: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+00001ab0: 656c 223a 2022 496e 6469 616e 2053 7562  el": "Indian Sub
+00001ac0: 2d43 6f6e 7469 6e65 6e74 222c 0a20 2020  -Continent",.   
+00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ae0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00001af0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b10: 2020 2269 6422 3a20 2234 6537 3463 3164    "id": "4e74c1d
+00001b20: 3235 3265 3339 3231 6222 2c0a 2020 2020  252e3921b",.    
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 2020 2020 226c 6179 6572 223a 2022 7472      "layer": "tr
+00001b50: 6164 696e 675f 7375 6272 6567 696f 6e22  ading_subregion"
+00001b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001b70: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00001b80: 223a 2022 5765 7374 2043 6f61 7374 2049  ": "West Coast I
+00001b90: 6e64 6961 222c 0a20 2020 2020 2020 2020  ndia",.         
+00001ba0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bc0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00001bd0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00001be0: 3a20 2261 3037 6561 6130 3330 6266 6539  : "a07eaa030bfe9
+00001bf0: 3235 6522 2c0a 2020 2020 2020 2020 2020  25e",.          
+00001c00: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00001c10: 6179 6572 223a 2022 7374 6f72 6167 6522  ayer": "storage"
+00001c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001c30: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00001c40: 223a 2022 5369 6b6b 6120 5b49 4e5d 222c  ": "Sikka [IN]",
+00001c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c60: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001c70: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 2269 6422 3a20 2263 3766        "id": "c7f
+00001ca0: 6562 6135 6338 3831 3133 6134 6322 2c0a  eba5c88113a4c",.
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 2020 2020 2020 2020 226c 6179 6572 223a          "layer":
+00001cd0: 2022 6672 6167 6d65 6e74 222c 0a20 2020   "fragment",.   
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 2020 2020 2022 6c61 6265 6c22 3a20 2257       "label": "W
+00001d00: 6573 7420 436f 6173 7420 496e 6469 6120  est Coast India 
+00001d10: 2857 6573 7420 436f 6173 7420 496e 6469  (West Coast Indi
+00001d20: 6129 2032 222c 0a20 2020 2020 2020 2020  a) 2",.         
+00001d30: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00001d40: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+00001d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d60: 2022 7072 6f64 7563 745f 6964 223a 2022   "product_id": "
+00001d70: 6338 3830 3363 3037 3363 3239 3830 6439  c8803c073c2980d9
+00001d80: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001d90: 2020 2022 7072 6f64 7563 745f 6465 7461     "product_deta
+00001da0: 696c 7322 3a20 5b0a 2020 2020 2020 2020  ils": [.        
+00001db0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 2020 2269 6422 3a20 2261 3765        "id": "a7e
+00001de0: 3236 3935 3666 6262 3931 6437 3822 2c0a  26956fbb91d78",.
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 2020 2020 2020 2020 226c 6179 6572 223a          "layer":
+00001e10: 2022 6361 7465 676f 7279 222c 0a20 2020   "category",.   
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 2022 6c61 6265 6c22 3a20 224d       "label": "M
+00001e40: 6564 6975 6d2d 536f 7572 222c 0a20 2020  edium-Sour",.   
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00001e70: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e90: 2020 2269 6422 3a20 2236 6631 3162 3037    "id": "6f11b07
+00001ea0: 3234 6339 6134 6538 3522 2c0a 2020 2020  24c9a4e85",.    
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 2020 2020 226c 6179 6572 223a 2022 6772      "layer": "gr
+00001ed0: 6f75 705f 7072 6f64 7563 7422 2c0a 2020  oup_product",.  
+00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ef0: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00001f00: 4372 7564 6522 2c0a 2020 2020 2020 2020  Crude",.        
+00001f10: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f30: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00001f40: 2020 2020 2020 2020 2020 2020 2022 6964               "id
+00001f50: 223a 2022 3534 6166 3735 3561 3039 3031  ": "54af755a0901
+00001f60: 3138 6463 222c 0a20 2020 2020 2020 2020  18dc",.         
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001f80: 6c61 7965 7222 3a20 2267 726f 7570 222c  layer": "group",
+00001f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001fa0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00001fb0: 3a20 2243 7275 6465 2f43 6f6e 6465 6e73  : "Crude/Condens
+00001fc0: 6174 6573 222c 0a20 2020 2020 2020 2020  ates",.         
+00001fd0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ff0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00002000: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00002010: 3a20 2263 3838 3033 6330 3733 6332 3938  : "c8803c073c298
+00002020: 3064 3922 2c0a 2020 2020 2020 2020 2020  0d9",.          
+00002030: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00002040: 6179 6572 223a 2022 6772 6164 6522 2c0a  ayer": "grade",.
+00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002060: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
+00002070: 2022 5572 616c 7322 2c0a 2020 2020 2020   "Urals",.      
+00002080: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00002090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020a0: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+000020b0: 2020 2020 2271 7561 6e74 6974 795f 746f      "quantity_to
+000020c0: 6e6e 6573 223a 2031 3130 3931 302c 0a20  nnes": 110910,. 
+000020d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000020e0: 7175 616e 7469 7479 5f62 6172 7265 6c73  quantity_barrels
+000020f0: 223a 2037 3936 3235 312c 0a20 2020 2020  ": 796251,.     
+00002100: 2020 2020 2020 2020 2020 2022 7175 616e             "quan
+00002110: 7469 7479 5f63 7562 6963 5f6d 6574 7265  tity_cubic_metre
+00002120: 7322 3a20 3132 3635 3934 2c0a 2020 2020  s": 126594,.    
+00002130: 2020 2020 2020 2020 2020 2020 2274 6f6e              "ton
+00002140: 6e65 5f6d 696c 6573 223a 2038 3731 3931  ne_miles": 87191
+00002150: 3032 3831 2e34 3431 3638 3436 2c0a 2020  0281.4416846,.  
+00002160: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00002170: 2020 2020 290a                               ).
```

### Comparing `vortexasdk-0.9.2/tests/api/examples/vessels.json` & `vortexasdk-1.0.0a1/tests/api/examples/vessels.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809523%*

 * *Differences: {'0': "{'classes': [OrderedDict([('id', 'vlcc_plus'), ('label', 'VLCC+'), ('layer', 'legacy')]), "*

 * *      "OrderedDict([('id', 'oil'), ('label', 'Oil Tankers'), ('layer', 'group')]), "*

 * *      "OrderedDict([('id', 'oil_vlcc'), ('label', 'VLCC+'), ('layer', 'coarse')]), "*

 * *      "OrderedDict([('id', 'oil_vlcc'), ('label', 'VLCC+'), ('layer', 'granular')])]}",*

 * * '1': "{'classes': [OrderedDict([('id', 'vlcc_plus'), ('label', 'VLCC+'), ('layer', 'legacy')]), "*

 * *      "OrderedDict([('id', 'oil'), ('label', 'Oil Tanker […]*

```diff
@@ -1,10 +1,32 @@
 [
     {
         "call_sign": "3269",
+        "classes": [
+            {
+                "id": "vlcc_plus",
+                "label": "VLCC+",
+                "layer": "legacy"
+            },
+            {
+                "id": "oil",
+                "label": "Oil Tankers",
+                "layer": "group"
+            },
+            {
+                "id": "oil_vlcc",
+                "label": "VLCC+",
+                "layer": "coarse"
+            },
+            {
+                "id": "oil_vlcc",
+                "label": "VLCC+",
+                "layer": "granular"
+            }
+        ],
         "corporate_entities": [],
         "cubic_capacity": 7060,
         "current_product_type": [
             {
                 "active": false,
                 "cargo_movement_id": "12d2cbca522e5570ea988b30850ad5b762e16d1b710e920f26729f08fcfdca46",
                 "product_type": [
@@ -53,14 +75,36 @@
         "to_starboard": 5,
         "to_stern": 5,
         "vessel_class": "tiny_tanker",
         "vessel_status": "vessel_status_ballast"
     },
     {
         "call_sign": "839",
+        "classes": [
+            {
+                "id": "vlcc_plus",
+                "label": "VLCC+",
+                "layer": "legacy"
+            },
+            {
+                "id": "oil",
+                "label": "Oil Tankers",
+                "layer": "group"
+            },
+            {
+                "id": "oil_vlcc",
+                "label": "VLCC+",
+                "layer": "coarse"
+            },
+            {
+                "id": "oil_vlcc",
+                "label": "VLCC+",
+                "layer": "granular"
+            }
+        ],
         "corporate_entities": [],
         "cubic_capacity": 6318,
         "current_product_type": [
             {
                 "active": false,
                 "cargo_movement_id": "5b74c0aab0353cccb28a1bed34c04d7fa54120efb32de10f8f0429c00dd8d536",
                 "product_type": [
```

### Comparing `vortexasdk-0.9.2/tests/api/test_cargo_event_entity.py` & `vortexasdk-1.0.0a1/tests/api/test_cargo_event_entity.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from unittest import TestCase
 
-import jsons
-
-from vortexasdk.api.cargo_movement import CargoEvent
-from vortexasdk.api.geography import GeographyEntity
+from vortexasdk.api.cargo_movement import CargoPortUnloadEvent
 
 
 class TestCargoEventEntity(TestCase):
-    def test_serialize(self):
-        with open("tests/api/examples/cargo_event_entity1.json", "r") as f:
-            serialized = f.read()
-            deserialized = jsons.loads(serialized, CargoEvent)
-
-            expected = CargoEvent(
-                event_type="cargo_port_unload_event",
-                location=[
-                    GeographyEntity(
-                        id="2aaad41b89dfad19e5668918018ae02695d7710bcbe5f2dc689234e8da492de3",
-                        layer="country",
-                        label="United Kingdom",
-                        source="model",
-                        probability=1,
-                    )
+    def test_serialize(self) -> None:
+        CargoPortUnloadEvent.model_validate(
+            {
+                "event_type": "cargo_port_unload_event",
+                "location": [
+                    {
+                        "id": "2aaad41b89dfad19e5668918018ae02695d7710bcbe5f2dc689234e8da492de3",
+                        "layer": "country",
+                        "label": "United Kingdom",
+                        "source": "model",
+                        "probability": 1,
+                    }
                 ],
-                probability=1,
-                pos=[-0.256674902984994, 53.74191566386998],
-                start_timestamp="2019-10-24T13:16:43+0000",
-                end_timestamp="2019-10-25T00:40:46+0000",
-            )
-
-            assert expected == deserialized
+                "probability": 1,
+                "pos": [-0.256674902984994, 53.74191566386998],
+                "vessel_id": "c1dd5bcc5814a98afdd94bc90eeb6f2dcd1b30367dd08f112ca49e84db88876c",
+                "start_timestamp": "2019-10-24T13:16:43+0000",
+                "end_timestamp": "2019-10-25T00:40:46+0000",
+            }
+        )
```

### Comparing `vortexasdk-0.9.2/tests/api/test_cargo_movement.py` & `vortexasdk-1.0.0a1/tests/api/test_cargo_movement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,132 @@
-from typing import List
 from unittest import TestCase
 
-import jsons
+import json
 
 from vortexasdk.api import (
-    CargoEvent,
     CargoMovement,
-    CorporateEntity,
-    GeographyEntity,
-    ProductEntity,
-    VesselEntity,
 )
 from vortexasdk.api.entity_flattening import (
     convert_cargo_movement_to_flat_dict,
 )
-from vortexasdk.api.serdes import serialize_to_dict
-from vortexasdk.api import (
-    CargoEvent,
-    CargoMovement,
-    CorporateEntity,
-    GeographyEntity,
-    ProductEntity,
-    VesselEntity,
-)
 
 
 class TestCargoMovement(TestCase):
     dictionary = {
         "cargo_movement_id": "00886b05a0747522b67322f50123ee60e61e219fc9a9c6011be1a1dade65f63e",
         "quantity": 4401,
         "status": "unloaded_state",
         "vessels": [
-            VesselEntity(
-                **{
-                    "id": "9cbf7c0fc6ccf1dfeacde02b87f3b6b1653030f560d4fc677bf1d7d0be8f8449",
-                    "mmsi": 255804460,
-                    "imo": 9480980,
-                    "name": "JOHANN ESSBERGER",
-                    "dwt": 5260,
-                    "cubic_capacity": 6100,
-                    "vessel_class": "tiny_tanker",
-                    "corporate_entities": [
-                        CorporateEntity(
-                            **{
-                                "id": "f9bd45e65e292909a7b751b0026dcf7795c6194b3c0712910a241caee32c99b8",
-                                "label": "Essberger J.T.",
-                                "layer": "commercial_owner",
-                                "probability": 1,
-                                "source": "external",
-                            }
-                        )
-                    ],
-                    "start_timestamp": "2019-10-18T21:38:34+0000",
-                    "end_timestamp": "2019-10-25T00:40:46+0000",
-                    "fixture_fulfilled": False,
-                    "voyage_id": "401f0e74fc42401248a484aca2e9955dea885378796f7f4d0bc8e92c35ea270a",
-                    "tags": [],
-                    "status": "vessel_status_laden_known",
-                }
-            )
+            {
+                "id": "9cbf7c0fc6ccf1dfeacde02b87f3b6b1653030f560d4fc677bf1d7d0be8f8449",
+                "mmsi": 255804460,
+                "imo": 9480980,
+                "name": "JOHANN ESSBERGER",
+                "dwt": 5260,
+                "cubic_capacity": 6100,
+                "vessel_class": "tiny_tanker",
+                "classes": [
+                    {"id": "vlcc_plus", "label": "VLCC+", "layer": "legacy"},
+                    {"id": "oil", "label": "Oil Tankers", "layer": "group"},
+                    {"id": "oil_vlcc", "label": "VLCC+", "layer": "coarse"},
+                    {"id": "oil_vlcc", "label": "VLCC+", "layer": "granular"},
+                ],
+                "corporate_entities": [
+                    {
+                        "id": "f9bd45e65e292909a7b751b0026dcf7795c6194b3c0712910a241caee32c99b8",
+                        "label": "Essberger J.T.",
+                        "layer": "effective_controller",
+                        "probability": 1.0,
+                        "source": "external",
+                    }
+                ],
+                "start_timestamp": "2019-10-18T21:38:34+0000",
+                "end_timestamp": "2019-10-25T00:40:46+0000",
+                "fixture_fulfilled": False,
+                "voyage_id": "401f0e74fc42401248a484aca2e9955dea885378796f7f4d0bc8e92c35ea270a",
+                "tags": [],
+                "status": "vessel_status_laden_known",
+            }
         ],
         "product": [
-            ProductEntity(
-                **{
-                    "id": "b68cbb746f8b9098c50e2ba36bcad83001a53bd362e9031fb49085d02c36659c",
-                    "layer": "group",
-                    "probability": 0.4756425,
-                    "source": "model",
-                    "label": "Clean products",
-                }
-            ),
-            ProductEntity(
-                **{
-                    "id": "a75fcc09bfc7d16496de3336551bc52b5891838bb7c22356d2cb65451587d1e5",
-                    "layer": "group_product",
-                    "probability": 0.4756425,
-                    "source": "model",
-                    "label": "Biodiesel",
-                }
-            ),
-            ProductEntity(
-                **{
-                    "id": "9d52ede1cff0421a8cd7283b0171afe8d23f519dca5f4e489734522f9cdf804c",
-                    "layer": "grade",
-                    "probability": 0.4756425,
-                    "source": "model",
-                    "label": "Biodiesel Feedstock",
-                }
-            ),
+            {
+                "id": "b68cbb746f8b9098c50e2ba36bcad83001a53bd362e9031fb49085d02c36659c",
+                "layer": "group",
+                "probability": 0.4756425,
+                "source": "model",
+                "label": "Clean products",
+            },
+            {
+                "id": "a75fcc09bfc7d16496de3336551bc52b5891838bb7c22356d2cb65451587d1e5",
+                "layer": "group_product",
+                "probability": 0.4756425,
+                "source": "model",
+                "label": "Biodiesel",
+            },
+            {
+                "id": "9d52ede1cff0421a8cd7283b0171afe8d23f519dca5f4e489734522f9cdf804c",
+                "layer": "grade",
+                "probability": 0.4756425,
+                "source": "model",
+                "label": "Biodiesel Feedstock",
+            },
         ],
         "events": [
-            CargoEvent(
-                **{
-                    "event_type": "cargo_port_load_event",
-                    "location": [
-                        GeographyEntity(
-                            **{
-                                "id": "2dfc3d43a21697c02ec3b2700b3b570a6ed1abb66d01c4fe6310ef362fcf6653",
-                                "layer": "country",
-                                "label": "Netherlands",
-                                "source": "model",
-                                "probability": 1,
-                            }
-                        )
-                    ],
-                    "probability": 1,
-                    "pos": [4.29914090037834, 51.87936163368058],
-                    "start_timestamp": "2019-10-18T21:38:34+0000",
-                    "end_timestamp": "2019-10-20T16:41:49+0000",
-                }
-            )
+            {
+                "event_type": "cargo_port_load_event",
+                "location": [
+                    {
+                        "id": "2dfc3d43a21697c02ec3b2700b3b570a6ed1abb66d01c4fe6310ef362fcf6653",
+                        "layer": "country",
+                        "label": "Netherlands",
+                        "source": "model",
+                        "probability": 1.0,
+                    }
+                ],
+                "vessel_id": "9cbf7c0fc6ccf1dfeacde02b87f3b6b1653030f560d4fc677bf1d7d0be8f8449",
+                "probability": 1.0,
+                "pos": [4.29914090037834, 51.87936163368058],
+                "start_timestamp": "2019-10-18T21:38:34+0000",
+                "end_timestamp": "2019-10-20T16:41:49+0000",
+            }
+        ],
+        "parent_ids": [
+            {
+                "id": "9d52ede1cff0421a8cd7283b0171afe8d23f519dca5f4e489734522f9cdf804c",
+                "splinter_timestamp": "2019-10-20T16:41:49+0000",
+            }
         ],
     }
 
-    cm = CargoMovement(**dictionary)
+    cm = CargoMovement.model_validate(dictionary)
 
-    def test_serialize(self):
+    def test_serialize(self) -> None:
         with open("tests/api/examples/cargo_movements.json", "r") as f:
-            serialized = f.read()
-            deserialized = jsons.loads(serialized, List[CargoMovement])
+            serialized = json.load(f)[0]
+            deserialized = CargoMovement.model_validate(serialized)
 
-            assert [self.cm] == deserialized
+            assert self.cm == deserialized
 
-    def test_convert_to_flat_dict(self):
-        flat = convert_cargo_movement_to_flat_dict(serialize_to_dict(self.cm))
+    def test_convert_to_flat_dict(self) -> None:
+        flat = convert_cargo_movement_to_flat_dict(self.cm.dict())
 
         expected = {
             "cargo_movement_id": "00886b05a0747522b67322f50123ee60e61e219fc9a9c6011be1a1dade65f63e",
             "events.cargo_port_load_event.0.end_timestamp": "2019-10-20T16:41:49+0000",
             "events.cargo_port_load_event.0.event_type": "cargo_port_load_event",
             "events.cargo_port_load_event.0.location.country.id": "2dfc3d43a21697c02ec3b2700b3b570a6ed1abb66d01c4fe6310ef362fcf6653",
             "events.cargo_port_load_event.0.location.country.label": "Netherlands",
             "events.cargo_port_load_event.0.location.country.layer": "country",
-            "events.cargo_port_load_event.0.location.country.probability": 1,
+            "events.cargo_port_load_event.0.location.country.probability": 1.0,
             "events.cargo_port_load_event.0.location.country.source": "model",
             "events.cargo_port_load_event.0.pos.0": 4.29914090037834,
             "events.cargo_port_load_event.0.pos.1": 51.87936163368058,
-            "events.cargo_port_load_event.0.probability": 1,
+            "events.cargo_port_load_event.0.probability": 1.0,
             "events.cargo_port_load_event.0.start_timestamp": "2019-10-18T21:38:34+0000",
-            "events.cargo_port_load_event.0.vessel_id": None,
+            "events.cargo_port_load_event.0.vessel_id": "9cbf7c0fc6ccf1dfeacde02b87f3b6b1653030f560d4fc677bf1d7d0be8f8449",
             "product.group.id": "b68cbb746f8b9098c50e2ba36bcad83001a53bd362e9031fb49085d02c36659c",
             "product.group.label": "Clean products",
             "product.group.layer": "group",
             "product.group.probability": 0.4756425,
             "product.group.source": "model",
             "product.group_product.id": "a75fcc09bfc7d16496de3336551bc52b5891838bb7c22356d2cb65451587d1e5",
             "product.group_product.label": "Biodiesel",
@@ -152,28 +136,49 @@
             "product.grade.id": "9d52ede1cff0421a8cd7283b0171afe8d23f519dca5f4e489734522f9cdf804c",
             "product.grade.label": "Biodiesel Feedstock",
             "product.grade.layer": "grade",
             "product.grade.probability": 0.4756425,
             "product.grade.source": "model",
             "quantity": 4401,
             "status": "unloaded_state",
-            "vessels.0.corporate_entities.commercial_owner.id": "f9bd45e65e292909a7b751b0026dcf7795c6194b3c0712910a241caee32c99b8",
-            "vessels.0.corporate_entities.commercial_owner.label": "Essberger J.T.",
-            "vessels.0.corporate_entities.commercial_owner.layer": "commercial_owner",
-            "vessels.0.corporate_entities.commercial_owner.probability": 1,
-            "vessels.0.corporate_entities.commercial_owner.source": "external",
+            "vessels.0.corporate_entities.effective_controller.id": "f9bd45e65e292909a7b751b0026dcf7795c6194b3c0712910a241caee32c99b8",
+            "vessels.0.corporate_entities.effective_controller.label": "Essberger J.T.",
+            "vessels.0.corporate_entities.effective_controller.layer": "effective_controller",
+            "vessels.0.corporate_entities.effective_controller.probability": 1.0,
+            "vessels.0.corporate_entities.effective_controller.source": "external",
+            "vessels.0.corporate_entities.effective_controller.start_timestamp": None,
+            "vessels.0.corporate_entities.effective_controller.end_timestamp": None,
             "vessels.0.cubic_capacity": 6100,
-            "vessels.0.dwt": 5260,
             "vessels.0.end_timestamp": "2019-10-25T00:40:46+0000",
             "vessels.0.fixture_fulfilled": False,
             "vessels.0.fixture_id": None,
             "vessels.0.id": "9cbf7c0fc6ccf1dfeacde02b87f3b6b1653030f560d4fc677bf1d7d0be8f8449",
             "vessels.0.imo": 9480980,
             "vessels.0.mmsi": 255804460,
             "vessels.0.name": "JOHANN ESSBERGER",
+            "vessels.0.dwt": 5260,
+            "vessels.0.year": None,
+            "vessels.0.ice_class": None,
+            "vessels.0.propulsion": None,
             "vessels.0.start_timestamp": "2019-10-18T21:38:34+0000",
             "vessels.0.status": "vessel_status_laden_known",
             "vessels.0.vessel_class": "tiny_tanker",
+            "vessels.0.classes.0.id": "vlcc_plus",
+            "vessels.0.classes.0.layer": "legacy",
+            "vessels.0.classes.0.label": "VLCC+",
+            "vessels.0.classes.1.id": "oil",
+            "vessels.0.classes.1.layer": "group",
+            "vessels.0.classes.1.label": "Oil Tankers",
+            "vessels.0.classes.2.id": "oil_vlcc",
+            "vessels.0.classes.2.layer": "coarse",
+            "vessels.0.classes.2.label": "VLCC+",
+            "vessels.0.classes.3.id": "oil_vlcc",
+            "vessels.0.classes.3.layer": "granular",
+            "vessels.0.classes.3.label": "VLCC+",
+            "vessels.0.scrubber": None,
+            "vessels.0.flag": None,
             "vessels.0.voyage_id": "401f0e74fc42401248a484aca2e9955dea885378796f7f4d0bc8e92c35ea270a",
+            "parent_ids.0.id": "9d52ede1cff0421a8cd7283b0171afe8d23f519dca5f4e489734522f9cdf804c",
+            "parent_ids.0.splinter_timestamp": "2019-10-20T16:41:49+0000",
         }
 
         assert flat == expected
```

### Comparing `vortexasdk-0.9.2/tests/endpoints/test_corporations_search_result.py` & `vortexasdk-1.0.0a1/tests/endpoints/test_corporations_search_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import pandas as pd
 
 from tests.mock_client import example_corporations
 from vortexasdk.endpoints.corporations_result import CorporationsResult
 
 
 class TestCorporationsSearchResult(TestCase):
-    cr = CorporationsResult(example_corporations)
+    cr = CorporationsResult(records=example_corporations, reference={})
 
     def test_to_df(self):
         df = self.cr.to_df(["name", "corporate_entity_type"])
 
         expected = pd.DataFrame(
             {
                 "name": {0: "3J", 1: "5XJAPANESE"},
                 "corporate_entity_type": {
-                    0: ["commercial_owner"],
-                    1: ["commercial_owner"],
+                    0: ["effective_controller"],
+                    1: ["effective_controller"],
                 },
             }
         )
         assert expected.equals(df)
 
     def test_to_list(self):
         names = [x.name for x in self.cr.to_list()]
```

### Comparing `vortexasdk-0.9.2/tests/endpoints/test_geographies_real.py` & `vortexasdk-1.0.0a1/tests/endpoints/test_geographies_real.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from tests.testcases import TestCaseUsingRealAPI
-from docs.utils import to_markdown
 from vortexasdk import Geographies
+from itertools import chain
 
 
 class TestGeographiesReal(TestCaseUsingRealAPI):
-    def test_search(self):
-        geographies = Geographies().search(term=["Liverpool", "Southampton"])
-        names = [g["name"] for g in geographies]
-
-        assert "Liverpool [GB]" in names
-
     def test_load_all(self):
         all_geogs = Geographies().load_all()
 
         assert len(all_geogs) > 1000
 
     def test_search_empty_args(self):
         Geographies().search()
 
     def test_search_to_df(self):
+        Geographies().search(term=["Liverpool", "Southampton"]).to_df()
+
+    def test_search_to_list(self):
         geographies = (
-            Geographies().search(term=["Liverpool", "Southampton"]).to_df()
+            Geographies().search(term=["Liverpool", "Southampton"]).to_list()
         )
+        names = [g.name for g in geographies]
+        assert "Liverpool [GB]" in names
+
+    def test_search_with_filter_layer(self):
+        geoType = "port"
+        df = Geographies().search(filter_layer=geoType).to_list()
+        allLayers = [g.layer for g in df]
+        flatten_list = set(chain.from_iterable(allLayers))
 
-        print(to_markdown(geographies))
+        assert geoType in flatten_list
```

### Comparing `vortexasdk-0.9.2/tests/endpoints/test_vessel_movements_real.py` & `vortexasdk-1.0.0a1/tests/endpoints/test_movement_status_breakdown.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,66 @@
 from datetime import datetime
+from vortexasdk import MovementStatusBreakdown
 
 from tests.testcases import TestCaseUsingRealAPI
-from vortexasdk import VesselMovements
-from vortexasdk.endpoints import vessel_movements_result
 
+totalMovementStatusBreakdown = 6
 
-class TestVesselMovementsReal(TestCaseUsingRealAPI):
-    def test_search(self):
-        v = VesselMovements().search(
-            filter_time_min=datetime(2017, 10, 1, 0, 0),
-            filter_time_max=datetime(2017, 10, 1, 0, 10),
-            filter_origins="rotterdam",
+
+class TestMovementStatusBreakdownReal(TestCaseUsingRealAPI):
+    def test_search_returns_one_day(self):
+        date = datetime(2019, 1, 1)
+
+        result = MovementStatusBreakdown().search(
+            timestamp=date,
+            breakdown_unit="b",
+            filter_time_min=date,
+            filter_time_max=date,
         )
 
-        assert len(v) > 10
+        assert len(result) == totalMovementStatusBreakdown
 
-    def test_to_df_all_columns(self):
-        df = (
-            VesselMovements()
-            .search(
-                filter_time_min=datetime(2017, 10, 1, 0, 0),
-                filter_time_max=datetime(2017, 10, 1, 0, 10),
-                filter_origins="rotterdam",
-            )
-            .to_df(columns="all")
-            .head(2)
+    def test_search_returns_multiple_breakdowns(self):
+        filter_time_min = datetime(2022, 11, 10)
+        filter_time_max = datetime(2022, 11, 10)
+        timestamp = datetime(2022, 11, 10)
+
+        result = MovementStatusBreakdown().search(
+            filter_activity="loading_state",
+            timestamp=timestamp,
+            breakdown_unit="b",
+            filter_time_min=filter_time_min,
+            filter_time_max=filter_time_max,
+            breakdown_size=100,
         )
 
-        assert len(df) == 2
+        assert len(result) == totalMovementStatusBreakdown
+
+    def test_search_returns_any_activity(self):
+        date = datetime(2019, 11, 10)
 
-    def test_search_to_dataframe(self):
-        df = (
-            VesselMovements()
-            .search(
-                filter_time_min=datetime(2017, 10, 1, 0, 0),
-                filter_time_max=datetime(2017, 10, 1, 0, 10),
-                filter_origins="rotterdam",
-            )
-            .to_df()
-            .head(2)
+        result = MovementStatusBreakdown().search(
+            filter_activity="any_activity",
+            timestamp=date,
+            breakdown_unit="b",
+            filter_time_min=date,
+            filter_time_max=date,
         )
 
-        assert list(df.columns) == vessel_movements_result.DEFAULT_COLUMNS
-        assert len(df) == 2
+        assert len(result) == totalMovementStatusBreakdown
+
+    def test_search_returns_excluded_params(self):
+        date = datetime(2019, 11, 10)
+        rotterdam = (
+            "68faf65af1345067f11dc6723b8da32f00e304a6f33c000118fccd81947deb4e"
+        )
 
-    def test_search_to_dataframe_subset_of_columns(self):
-        cols = ["vessel.imo", "vessel.name"]
-        df = (
-            VesselMovements()
-            .search(
-                filter_time_min=datetime(2017, 10, 1, 0, 0),
-                filter_time_max=datetime(2017, 10, 1, 0, 10),
-                filter_origins="rotterdam",
-            )
-            .to_df(columns=cols)
-            .head(2)
+        result = MovementStatusBreakdown().search(
+            filter_activity="any_activity",
+            timestamp=date,
+            breakdown_unit="b",
+            filter_time_min=date,
+            filter_time_max=date,
+            exclude_origins=rotterdam,
         )
 
-        assert list(df.columns) == cols
-        assert len(df) == 2
+        assert len(result) == totalMovementStatusBreakdown
```

### Comparing `vortexasdk-0.9.2/tests/endpoints/test_vessels_real.py` & `vortexasdk-1.0.0a1/tests/endpoints/test_vessels_real.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from tests.testcases import TestCaseUsingRealAPI
 from tests.timer import Timer
+from vortexasdk import Products
 from vortexasdk.endpoints.vessels import Vessels
 
 
 class TestVesselsReal(TestCaseUsingRealAPI):
     def test_search_ids(self):
         ids = [
             "6d8a8f0863ca087204dd68e5fc3b6469a879829e6262856e34856aea3ca20509",
             "bf2b55bd31c709aa4cba91a3cc4111191c88c83753cbd285674c22150e42003e",
         ]
 
         vessels = Vessels().search(ids=ids).to_list()
         assert len(vessels) == 2
 
-        print([x.name for x in vessels])
-
     def test_search_filters_vessel_class(self):
-        vessel_classes = ["vlcc_plus", "aframax"]
+        vessel_classes = ["oil_vlcc", "oil_aframax"]
 
         vessels = Vessels().search(vessel_classes=vessel_classes).to_list()
 
         actual = {x.vessel_class for x in vessels}
 
         assert actual == set(vessel_classes)
 
     def test_search_terms_are_combined_with_AND(self):
         aframax = set(
-            v.id for v in Vessels().search(vessel_classes="aframax").to_list()
+            v.id
+            for v in Vessels().search(vessel_classes="oil_aframax").to_list()
         )
         aframax_called_zhen = set(
             v.id
             for v in Vessels()
-            .search(vessel_classes="aframax", term="zhen")
+            .search(vessel_classes="oil_aframax", term="zhen")
             .to_list()
         )
 
         assert aframax_called_zhen.issubset(aframax)
 
     def test_search_ids_dataframe(self):
         ids = [
@@ -44,15 +44,20 @@
         ]
 
         df = Vessels().search(ids=ids).to_df()
         assert list(df.columns) == ["id", "name", "imo", "vessel_class"]
         assert len(df) == 2
 
     def test_find_crude_vessels(self):
-        df = Vessels().search(vessel_product_types="crude").to_df()
+        crude = [
+            p.id
+            for p in Products().search("crude").to_list()
+            if "group" in p.layer
+        ]
+        df = Vessels().search(vessel_product_types=crude).to_df()
         assert len(df) > 1000
 
     def test_load_all(self):
         all_products = Vessels().load_all()
 
         assert len(all_products) > 1000
 
@@ -60,21 +65,22 @@
         with Timer("Search"):
             result = Vessels().search()
 
         with Timer("Serialize"):
             result.to_list()
 
         with Timer("Dataframe"):
-            df = result.to_df()
-            print(df.head())
+            result.to_df()
 
         assert len(result) >= 1_000
 
     def test_search_is_case_agnostic(self):
         uppercase = {
-            v.id for v in Vessels().search(vessel_classes="Suezmax").to_list()
+            v.id
+            for v in Vessels().search(vessel_classes="oil_suezmax").to_list()
         }
         lowercase = {
-            v.id for v in Vessels().search(vessel_classes="suezmax").to_list()
+            v.id
+            for v in Vessels().search(vessel_classes="oil_suezmax").to_list()
         }
 
         assert uppercase == lowercase
```

### Comparing `vortexasdk-0.9.2/tests/test_id.py` & `vortexasdk-1.0.0a1/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.2/tests/timer.py` & `vortexasdk-1.0.0a1/tests/timer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from typing import Any
 
 from vortexasdk.logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class Timer:
@@ -24,18 +25,18 @@
 
     "Hello"
     "Timer took 10 seconds"
     "Done"
 
     """
 
-    def __init__(self, name=None):
+    def __init__(self: "Timer", name: str | None = None) -> None:
         self.name = name
 
-    def __enter__(self):
+    def __enter__(self: "Timer") -> "Timer":
         self.start = time.time()
         return self
 
-    def __exit__(self, *args):
+    def __exit__(self: "Timer", *args: Any) -> None:
         self.end = time.time()
         self.interval = self.end - self.start
         logger.info(f"Timer {self.name} took: {self.interval} seconds")
```

### Comparing `vortexasdk-0.9.2/vortexasdk/api/corporation.py` & `vortexasdk-1.0.0a1/vortexasdk/api/corporation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from dataclasses import dataclass
-from typing import List
+from typing import List, Optional
 
-from vortexasdk.api.serdes import FromDictMixin
-from vortexasdk.api.shared_types import IDName, EntityWithProbability
 
+from vortexasdk.api.shared_types import (
+    EntityWithSingleLayerAndProbability,
+    IDName,
+)
 
-@dataclass(frozen=True)
-class Corporation(IDName, FromDictMixin):
+
+class Corporation(IDName):
     """Represent a Corporation reference record returned by the API."""
 
-    corporate_entity_type: List[str]
-    ref_type: str
-    leaf: bool
-    parent: List[str]
+    corporate_entity_type: Optional[List[str]] = None
+    ref_type: Optional[str] = None
+    leaf: Optional[bool] = None
+    parent: Optional[List[str]] = None
 
 
-@dataclass(frozen=True)
-class CorporateEntity(EntityWithProbability):
+class CorporateEntity(EntityWithSingleLayerAndProbability):
     """
     Represents a relationship between a corporation and another entity like a vessel.
 
     [Corporate Entity Further Documentation](https://docs.vortexa.com/reference/intro-corporate-entities)
 
 
     """
```

### Comparing `vortexasdk-0.9.2/vortexasdk/api/entity_flattening.py` & `vortexasdk-1.0.0a1/vortexasdk/api/entity_flattening.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from itertools import groupby
-from typing import Dict, List
+from typing import Dict, List, Union
+from typing_extensions import Literal
 
 # noinspection PyProtectedMember
 from flatten_dict import flatten
 import copy
 
 
 def flatten_dictionary(d: Dict) -> Dict:
@@ -15,66 +15,50 @@
     flat_with_formatted_keys = {}
     for k, v in dictionary.items():
         nice_path = ".".join([str(i) for i in k])
         flat_with_formatted_keys[nice_path] = v
     return flat_with_formatted_keys
 
 
-def convert_cargo_movement_to_flat_dict(cme: Dict, cols="all") -> Dict:
-    """Convert nested `CargoMovement` object to flat dictionary, keeping *cols*."""
-    as_dict = _group_cargo_movement_attributes_by_layer(cme)
+def convert_to_flat_dict(
+    va: Dict, columns: Union[Literal["all"], List[str]] = "all"
+) -> Dict:
+    """A generic function to convert nested object to flat dictionary, keeping *cols*."""
 
-    formatted = flatten_dictionary(as_dict)
+    formatted = flatten_dictionary(va)
 
-    if cols == "all":
+    if columns == "all":
         return formatted
     else:
-        return {k: v for k, v in formatted.items() if k in cols}
+        return {k: v for k, v in formatted.items() if k in columns}
 
 
-def convert_vessel_movement_to_flat_dict(vm: Dict, cols="all") -> Dict:
-    """Convert nested `VesselMovement` dict to flat dictionary, keeping *cols*."""
-    as_dict = _group_vessel_movement_attributes_by_layer(vm)
+def convert_cargo_movement_to_flat_dict(
+    cme: Dict, columns: Union[Literal["all"], List[str]] = "all"
+) -> Dict:
+    """Convert nested `CargoMovement` object to flat dictionary, keeping *cols*."""
+    as_dict = _group_cargo_movement_attributes_by_layer(cme)
 
     formatted = flatten_dictionary(as_dict)
 
-    if cols == "all":
+    if columns == "all":
         return formatted
     else:
-        return {k: v for k, v in formatted.items() if k in cols}
-
-
-def _group_vessel_movement_attributes_by_layer(vm: Dict) -> Dict:
-    """Group relevant `VesselMovement` attributes by `Entity.layer`."""
-    if "origin" in vm.keys():
-        flat_origin = _flatten_attributes(vm["origin"], "location")
-        vm["origin"] = flat_origin
-
-    if "destination" in vm.keys():
-        flat_destination = _flatten_attributes(vm["destination"], "location")
-        vm["destination"] = flat_destination
-
-    if "cargoes" in vm.keys():
-        flat_cargoes = [
-            _flatten_attributes(cargo, "product") for cargo in vm["cargoes"]
-        ]
-        vm["cargoes"] = flat_cargoes
-
-    vm["vessel"] = _flatten_vessel_entity(vm["vessel"])
-    return vm
+        return {k: v for k, v in formatted.items() if k in columns}
 
 
 def _group_cargo_movement_attributes_by_layer(cm: Dict) -> Dict:
     """Group relevant `CargoMovement` attributes by `Entity.layer`."""
     vessels = [_flatten_vessel_entity(ve) for ve in cm["vessels"]]
 
-    events = {
-        event_type: list(g)
-        for event_type, g in groupby(cm["events"], lambda x: x["event_type"])
-    }
+    events: Dict[str, list] = {}
+    for event in cm["events"]:
+        if event["event_type"] not in events:
+            events[event["event_type"]] = []
+        events[event["event_type"]].append(event)
 
     events_attributes = {
         event_type: [_flatten_attributes(ce, "location") for ce in es]
         for event_type, es in events.items()
     }
 
     cm = _flatten_attributes(cm, "product")
```

### Comparing `vortexasdk-0.9.2/vortexasdk/api/entity_serializing.py` & `vortexasdk-1.0.0a1/vortexasdk/api/entity_serializing.py`

 * *Files identical despite different names*

### Comparing `vortexasdk-0.9.2/vortexasdk/api/geography.py` & `vortexasdk-1.0.0a1/vortexasdk/api/geography.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-from dataclasses import dataclass
+from pydantic import BaseModel
 from typing import List, Optional, Tuple
 
-from vortexasdk.api.serdes import FromDictMixin
+
+from vortexasdk.api import ID
 from vortexasdk.api.shared_types import (
-    EntityWithProbability,
+    EntityWithSingleLayerAndProbability,
     IDLayer,
     IDNameLayer,
     Node,
 )
 
 Position = Tuple[float, float]
 
 
-@dataclass(frozen=True)
-class BoundingBox:
+class BoundingBox(BaseModel):
     """Polygon with list of bounding lon lat coords."""
 
-    type: str
-    coordinates: List[Position]
+    type: Optional[str] = None
+    coordinates: Optional[List[Position]] = None
 
 
-@dataclass(frozen=True)
-class Geography(Node, IDNameLayer, FromDictMixin):
+class Geography(Node):
     """Represent a Geography reference record returned by the API."""
 
-    bounding_box: Optional[BoundingBox]
-    centre_point: Optional[Position]
-    exclusion_rule: List[IDNameLayer]
-    hierarchy: List[IDLayer]
-    location: Optional[Position]
+    id: ID
+    name: Optional[str] = None
+    layer: List[str] = []
+    exclusion_rule: Optional[List[IDNameLayer]] = None
+    hierarchy: Optional[List[IDLayer]] = None
+    pos: Optional[List[float]] = None
 
 
-@dataclass(frozen=True)
-class GeographyEntity(EntityWithProbability):
+class GeographyEntity(EntityWithSingleLayerAndProbability):
     """
     Represents a hierarchy tree of locational data.
 
     [Geography Entities Further Documentation](https://docs.vortexa.com/reference/intro-geography-entries)
 
     """
```

### Comparing `vortexasdk-0.9.2/vortexasdk/api/id.py` & `vortexasdk-1.0.0a1/vortexasdk/api/id.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import List, Tuple
 
 ID = str
 
 
-def is_valid_id(potential_id) -> bool:
+def is_valid_id(potential_id: str) -> bool:
     """Check if argument is valid SHA256 hash."""
     return (
         isinstance(potential_id, str)
         and re.match("^[A-Fa-f0-9]{64}$", potential_id) is not None
     )
```

### Comparing `vortexasdk-0.9.2/vortexasdk/endpoints/cargo_movements_result.py` & `vortexasdk-1.0.0a1/vortexasdk/endpoints/cargo_movements_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 import functools
 import os
 from multiprocessing.pool import Pool
 from typing import List
+from typing_extensions import Literal
 
 import pandas as pd
 
-from vortexasdk.api import CargoMovement
+from vortexasdk.api.cargo_movement import CargoMovement
 from vortexasdk.api.entity_flattening import (
     convert_cargo_movement_to_flat_dict,
 )
 from vortexasdk.api.search_result import Result
+from vortexasdk.logger import get_logger
+from vortexasdk.result_conversions import create_dataframe, create_list
+
+logger = get_logger(__name__)
+
+DEFAULT_COLUMNS = [
+    "events.cargo_port_load_event.0.location.port.label",
+    "events.cargo_port_unload_event.0.location.port.label",
+    "product.group.label",
+    "product.grade.label",
+    "quantity",
+    "vessels.0.name",
+    "events.cargo_port_load_event.0.end_timestamp",
+    "events.cargo_port_unload_event.0.start_timestamp",
+]
 
 
 class CargoMovementsResult(Result):
     """
     Container class holdings search results returns from the cargo movements endpoint.
 
     This class has two methods, `to_list()`, and `to_df()`, allowing search results to be represented as a list of `CargoMovements`,
      or as a `pd.DataFrame` , respectively.
     """
 
     def to_list(self) -> List[CargoMovement]:
         """Represent cargo movements as a list of `CargoMovementEntity`s."""
-        list_of_dicts = super().to_list()
+        # noinspection PyTypeChecker
+        return create_list(super().to_list(), CargoMovement)
 
-        with Pool(os.cpu_count()) as pool:
-            return list(pool.map(CargoMovement.from_dict, list_of_dicts))
-
-    def to_df(self, columns=None) -> pd.DataFrame:
+    def to_df(
+        self: "CargoMovementsResult",
+        columns: Literal["all"] | List[str] | None = DEFAULT_COLUMNS,
+    ) -> pd.DataFrame:
         """
         Represent cargo movements as a `pd.DataFrame`.
 
         # Arguments
             columns: Output columns present in the `pd.DataFrame`.
             Enter `columns='all'` to return all available columns.
             Enter `columns=None` to use `cargo_movements.DEFAULT_COLUMNS`.
@@ -40,37 +57,37 @@
         `pd.DataFrame`, one row per cargo movement.
 
 
         ## Notes
 
         A cargo movement is a complicated, nested structure. Between it's point of loading and discharge, a cargo
          movement may be carried by _N_ or more vessels, with _N-1_ associated STS events. Each of these _N_ vessels
-         could have an associated corporate owner, charterer, time charterer... etc.
+         could have an associated effective controller, charterer, time charterer... etc.
 
          In order to represent a cargo movement as a flat (not nested) record in a dataframe, the sdk flattens the cargo
          movement, generating many columns in the process.
 
          The columns are logically named. Let's say that a cargo is transferred between 4 vessels en route from a load
          in Rotterdam to a discharge in New York. This is represented as 1 `cargo_port_unload_event`, followed by
           3 `cargo_sts_event`s, and finally 1 `cargo_port_unload_event`.
 
          In this example the name of the 1st vessel, is found in the `vessels.0.name` column (we're using zero-based
          numbering indexes). Likewise, the imo of the second vessel is found in the `vessels.1.imo` column.
 
-         To find the name of the country in which the second STS event occured, we'd use the
+         To find the name of the country in which the second STS event occurred, we'd use the
          `events.cargo_sts_event.1.location.country.layer` column.
 
          Similarly, to find out when the first vessel started
          loading the cargo from Rotterdam, we'd use the `events.cargo_port_load_event.0.start_timestamp` column.
 
         By default, the columns returned are something along the lines of.
         ```python
         DEFAULT_COLUMNS = [
-            'events.cargo_port_load_event.0.label',
-            'events.cargo_port_unload_event.0.label',
+            'events.cargo_port_load_event.0.location.port.label',
+            'events.cargo_port_unload_event.0.location.port.label',
             'product.group.label',
             'product.grade.label',
             'quantity',
             'vessels.0.name',
             'events.cargo_port_load_event.0.end_timestamp',
             'events.cargo_port_unload_event.0.start_timestamp',
         ]
@@ -420,19 +437,19 @@
             'quantity',
             'status',
             'vessels.0.corporate_entities.charterer.id',
             'vessels.0.corporate_entities.charterer.label',
             'vessels.0.corporate_entities.charterer.layer',
             'vessels.0.corporate_entities.charterer.probability',
             'vessels.0.corporate_entities.charterer.source',
-            'vessels.0.corporate_entities.commercial_owner.id',
-            'vessels.0.corporate_entities.commercial_owner.label',
-            'vessels.0.corporate_entities.commercial_owner.layer',
-            'vessels.0.corporate_entities.commercial_owner.probability',
-            'vessels.0.corporate_entities.commercial_owner.source',
+            'vessels.0.corporate_entities.effective_controller.id',
+            'vessels.0.corporate_entities.effective_controller.label',
+            'vessels.0.corporate_entities.effective_controller.layer',
+            'vessels.0.corporate_entities.effective_controller.probability',
+            'vessels.0.corporate_entities.effective_controller.source',
             'vessels.0.corporate_entities.time_charterer.end_timestamp',
             'vessels.0.corporate_entities.time_charterer.id',
             'vessels.0.corporate_entities.time_charterer.label',
             'vessels.0.corporate_entities.time_charterer.layer',
             'vessels.0.corporate_entities.time_charterer.probability',
             'vessels.0.corporate_entities.time_charterer.source',
             'vessels.0.corporate_entities.time_charterer.start_timestamp',
@@ -453,19 +470,19 @@
             'vessels.0.vessel_class',
             'vessels.0.voyage_id',
             'vessels.1.corporate_entities.charterer.id',
             'vessels.1.corporate_entities.charterer.label',
             'vessels.1.corporate_entities.charterer.layer',
             'vessels.1.corporate_entities.charterer.probability',
             'vessels.1.corporate_entities.charterer.source',
-            'vessels.1.corporate_entities.commercial_owner.id',
-            'vessels.1.corporate_entities.commercial_owner.label',
-            'vessels.1.corporate_entities.commercial_owner.layer',
-            'vessels.1.corporate_entities.commercial_owner.probability',
-            'vessels.1.corporate_entities.commercial_owner.source',
+            'vessels.1.corporate_entities.effective_controller.id',
+            'vessels.1.corporate_entities.effective_controller.label',
+            'vessels.1.corporate_entities.effective_controller.layer',
+            'vessels.1.corporate_entities.effective_controller.probability',
+            'vessels.1.corporate_entities.effective_controller.source',
             'vessels.1.corporate_entities.time_charterer.end_timestamp',
             'vessels.1.corporate_entities.time_charterer.id',
             'vessels.1.corporate_entities.time_charterer.label',
             'vessels.1.corporate_entities.time_charterer.layer',
             'vessels.1.corporate_entities.time_charterer.probability',
             'vessels.1.corporate_entities.time_charterer.source',
             'vessels.1.corporate_entities.time_charterer.start_timestamp',
@@ -485,19 +502,19 @@
             'vessels.1.vessel_class',
             'vessels.1.voyage_id',
             'vessels.2.corporate_entities.charterer.id',
             'vessels.2.corporate_entities.charterer.label',
             'vessels.2.corporate_entities.charterer.layer',
             'vessels.2.corporate_entities.charterer.probability',
             'vessels.2.corporate_entities.charterer.source',
-            'vessels.2.corporate_entities.commercial_owner.id',
-            'vessels.2.corporate_entities.commercial_owner.label',
-            'vessels.2.corporate_entities.commercial_owner.layer',
-            'vessels.2.corporate_entities.commercial_owner.probability',
-            'vessels.2.corporate_entities.commercial_owner.source',
+            'vessels.2.corporate_entities.effective_controller.id',
+            'vessels.2.corporate_entities.effective_controller.label',
+            'vessels.2.corporate_entities.effective_controller.layer',
+            'vessels.2.corporate_entities.effective_controller.probability',
+            'vessels.2.corporate_entities.effective_controller.source',
             'vessels.2.corporate_entities.time_charterer.end_timestamp',
             'vessels.2.corporate_entities.time_charterer.id',
             'vessels.2.corporate_entities.time_charterer.label',
             'vessels.2.corporate_entities.time_charterer.layer',
             'vessels.2.corporate_entities.time_charterer.probability',
             'vessels.2.corporate_entities.time_charterer.source',
             'vessels.2.corporate_entities.time_charterer.start_timestamp',
@@ -510,52 +527,44 @@
             'vessels.2.name',
             'vessels.2.start_timestamp',
             'vessels.2.status',
             'vessels.2.tags.0.start_timestamp',
             'vessels.2.tags.0.tag',
             'vessels.2.vessel_class',
             'vessels.2.voyage_id',
-            'vessels.3.corporate_entities.commercial_owner.id',
-            'vessels.3.corporate_entities.commercial_owner.label',
-            'vessels.3.corporate_entities.commercial_owner.layer',
-            'vessels.3.corporate_entities.commercial_owner.probability',
-            'vessels.3.corporate_entities.commercial_owner.source',
+            'vessels.3.corporate_entities.effective_controller.id',
+            'vessels.3.corporate_entities.effective_controller.label',
+            'vessels.3.corporate_entities.effective_controller.layer',
+            'vessels.3.corporate_entities.effective_controller.probability',
+            'vessels.3.corporate_entities.effective_controller.source',
             'vessels.3.cubic_capacity',
             'vessels.3.dwt',
             'vessels.3.id',
             'vessels.3.imo',
             'vessels.3.mmsi',
             'vessels.3.name',
             'vessels.3.start_timestamp',
             'vessels.3.status',
             'vessels.3.vessel_class',
             'vessels.3.voyage_id',
+            'parent_ids.0.id',
+            'parent_ids.0.splinter_timestamp',
+            'parent_ids.1.id',
+            'parent_ids.1.splinter_timestamp',
         ]
         ```
 
         """
-        if columns is None:
-            columns = DEFAULT_COLUMNS
 
         flatten = functools.partial(
-            convert_cargo_movement_to_flat_dict, cols=columns
+            convert_cargo_movement_to_flat_dict, columns=columns
         )
 
+        logger.debug("Converting each CargoMovement to a flat dictionary")
         with Pool(os.cpu_count()) as pool:
             records = pool.map(flatten, super().to_list())
 
-        if columns == "all":
-            return pd.DataFrame(data=records)
-        else:
-            return pd.DataFrame(data=records, columns=columns)
-
-
-DEFAULT_COLUMNS = [
-    "events.cargo_port_load_event.0.label",
-    "events.cargo_port_unload_event.0.label",
-    "product.group.label",
-    "product.grade.label",
-    "quantity",
-    "vessels.0.name",
-    "events.cargo_port_load_event.0.end_timestamp",
-    "events.cargo_port_unload_event.0.start_timestamp",
-]
+        return create_dataframe(
+            columns=columns,
+            data=records,
+            logger_description="CargoMovements",
+        )
```

### Comparing `vortexasdk-0.9.2/vortexasdk/endpoints/corporations_result.py` & `vortexasdk-1.0.0a1/vortexasdk/endpoints/corporations_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-import os
-from multiprocessing import Pool
 from typing import List
+from typing_extensions import Literal
 
 import pandas as pd
 
 from vortexasdk.api import Corporation
 from vortexasdk.api.search_result import Result
+from vortexasdk.logger import get_logger
+from vortexasdk.result_conversions import create_dataframe, create_list
+
+logger = get_logger(__name__)
+
+DEFAULT_COLUMNS = ["id", "name", "corporate_entity_type"]
 
 
 class CorporationsResult(Result):
     """Container class that holds the result obtained from calling the `Vessels` endpoint."""
 
     def to_list(self) -> List[Corporation]:
         """Represent vessels as a list."""
-        list_of_dicts = super().to_list()
-
-        with Pool(os.cpu_count()) as pool:
-            return list(pool.map(Corporation.from_dict, list_of_dicts))
+        # noinspection PyTypeChecker
+        return create_list(super().to_list(), Corporation)
 
-    def to_df(self, columns=None) -> pd.DataFrame:
+    def to_df(
+        self,
+        columns: List[str] | Literal["all"] | None = DEFAULT_COLUMNS,
+    ) -> pd.DataFrame:
         """
         Represent corporations as a `pd.DataFrame`.
 
         # Arguments
             columns: The corporation features we want in the dataframe. Enter `columns='all'` to include all features.
             Defaults to `columns = ['id', 'name', 'corporate_entity_type']`.
 
 
         # Returns
         `pd.DataFrame` of corporations.
 
         """
-        if columns is None:
-            columns = DEFAULT_COLUMNS
-
-        if columns == "all":
-            return pd.DataFrame(super().to_list())
-        else:
-            return pd.DataFrame(super().to_list(), columns=columns)
-
-
-DEFAULT_COLUMNS = ["id", "name", "corporate_entity_type"]
+        return create_dataframe(
+            columns=columns,
+            data=super().to_list(),
+            logger_description="Corporations",
+        )
```

### Comparing `vortexasdk-0.9.2/vortexasdk/endpoints/geographies_result.py` & `vortexasdk-1.0.0a1/vortexasdk/endpoints/geographies_result.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-import os
-from multiprocessing.pool import Pool
 from typing import List
-
+from typing_extensions import Literal
 import pandas as pd
 
 from vortexasdk.api import Geography
 from vortexasdk.api.search_result import Result
+from vortexasdk.logger import get_logger
+from vortexasdk.result_conversions import create_dataframe, create_list
+
+logger = get_logger(__name__)
+
+
+DEFAULT_COLUMNS = ["id", "name", "layer"]
 
 
 class GeographyResult(Result):
     """Container class that holds the result obtained from calling the `Geography` endpoint."""
 
     def to_list(self) -> List[Geography]:
         """Represent geographies as a list."""
-        list_of_dicts = super().to_list()
+        # noinspection PyTypeChecker
+        return create_list(super().to_list(), Geography)
 
-        with Pool(os.cpu_count()) as pool:
-            return list(pool.map(Geography.from_dict, list_of_dicts))
-
-    def to_df(self, columns=None) -> pd.DataFrame:
+    def to_df(
+        self,
+        columns: List[str] | Literal["all"] | None = DEFAULT_COLUMNS,
+    ) -> pd.DataFrame:
         """
         Represent geographies as a `pd.DataFrame`.
 
         # Arguments
             columns: The geography features we want in the dataframe. Enter `columns='all'` to include all features.
             Defaults to `columns = ['id', 'name', 'layer']`.
 
 
         # Returns
         `pd.DataFrame` of geographies.
 
         """
-        if columns is None:
-            columns = DEFAULT_COLUMNS
-
-        if columns == "all":
-            return pd.DataFrame(data=super().to_list())
-        else:
-            return pd.DataFrame(data=super().to_list(), columns=columns)
-
-
-DEFAULT_COLUMNS = ["id", "name", "layer"]
+        return create_dataframe(
+            data=super().to_list(),
+            columns=columns,
+            logger_description="Geographies",
+        )
```

### Comparing `vortexasdk-0.9.2/vortexasdk/endpoints/products_result.py` & `vortexasdk-1.0.0a1/vortexasdk/endpoints/products_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-import os
-from multiprocessing.pool import Pool
 from typing import List
-
+from typing_extensions import Literal
 import pandas as pd
 
 from vortexasdk.api import Product
 from vortexasdk.api.entity_flattening import flatten_dictionary
 from vortexasdk.api.search_result import Result
+from vortexasdk.logger import get_logger
+from vortexasdk.result_conversions import create_dataframe, create_list
+
+logger = get_logger(__name__)
+
+
+DEFAULT_COLUMNS = ["id", "name", "layer.0", "parent.0.name"]
 
 
 class ProductResult(Result):
     """Container class that holds the result obtained from calling the `Product` endpoint."""
 
     def to_list(self) -> List[Product]:
         """Represent products as a list."""
-        list_of_dicts = super().to_list()
+        # noinspection PyTypeChecker
+        return create_list(super().to_list(), Product)
 
-        with Pool(os.cpu_count()) as pool:
-            return list(pool.map(Product.from_dict, list_of_dicts))
-
-    def to_df(self, columns=None) -> pd.DataFrame:
+    def to_df(
+        self,
+        columns: List[str] | Literal["all"] | None = DEFAULT_COLUMNS,
+    ) -> pd.DataFrame:
         """
         Represent products as a `pd.DataFrame`.
 
         # Arguments
             columns: The product features we want in the dataframe. Enter `columns='all'` to include all features.
             Defaults to `columns = ['id', 'name', 'layer.0', 'parent.0.name']`.
 
 
         # Returns
         `pd.DataFrame` of products.
 
         """
-        if columns is None:
-            columns = DEFAULT_COLUMNS
-
         flattened_dicts = [flatten_dictionary(p) for p in super().to_list()]
 
-        if columns == "all":
-            return pd.DataFrame(data=flattened_dicts)
-        else:
-            return pd.DataFrame(data=flattened_dicts, columns=columns)
-
-
-DEFAULT_COLUMNS = ["id", "name", "layer.0", "parent.0.name"]
+        return create_dataframe(
+            columns=columns,
+            data=flattened_dicts,
+            logger_description="Products",
+        )
```

### Comparing `vortexasdk-0.9.2/vortexasdk/endpoints/vessels_result.py` & `vortexasdk-1.0.0a1/vortexasdk/endpoints/vessels_result.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-import os
-from multiprocessing import Pool
 from typing import List
+from typing_extensions import Literal
 
 import pandas as pd
 
+from vortexasdk.logger import get_logger
 from vortexasdk.api import Vessel
 from vortexasdk.api.search_result import Result
+from vortexasdk.result_conversions import create_dataframe, create_list
+
+logger = get_logger(__name__)
+
+DEFAULT_COLUMNS = ["id", "name", "imo", "vessel_class"]
 
 
 class VesselsResult(Result):
     """Container class that holds the result obtained from calling the `Vessels` endpoint."""
 
     def to_list(self) -> List[Vessel]:
         """Represent vessels as a list."""
-        list_of_dicts = super().to_list()
-
-        with Pool(os.cpu_count()) as pool:
-            return list(pool.map(Vessel.from_dict, list_of_dicts))
+        # noinspection PyTypeChecker
+        return create_list(super().to_list(), Vessel)
 
-    def to_df(self, columns=None) -> pd.DataFrame:
+    def to_df(
+        self,
+        columns: List[str] | Literal["all"] | None = DEFAULT_COLUMNS,
+    ) -> pd.DataFrame:
         """
         Represent vessels as a `pd.DataFrame`.
 
         # Arguments
             columns: The vessel features we want in the dataframe. Enter `columns='all'` to include all features.
             Defaults to `columns = ['id', 'name', 'imo', 'vessel_class']`.
 
 
         # Returns
         `pd.DataFrame` of vessels.
 
         """
-        if columns is None:
-            columns = DEFAULT_COLUMNS
-
-        if columns == "all":
-            return pd.DataFrame(data=super().to_list())
-        else:
-            return pd.DataFrame(data=super().to_list(), columns=columns)
-
-
-DEFAULT_COLUMNS = ["id", "name", "imo", "vessel_class"]
+        return create_dataframe(
+            columns=columns,
+            data=super().to_list(),
+            logger_description="Vessels",
+        )
```

### Comparing `vortexasdk-0.9.2/vortexasdk/logger.py` & `vortexasdk-1.0.0a1/vortexasdk/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,27 +5,22 @@
 from vortexasdk.config import LOG_FILE, LOG_LEVEL
 
 FORMATTER = logging.Formatter(
     "%(asctime)s %(name)s — %(levelname)s — %(message)s"
 )
 
 
-def get_console_handler():
+def get_logger(logger_name: str) -> logging.Logger:
+    logger = logging.getLogger(logger_name)
+    logger.setLevel(LOG_LEVEL)
+
     console_handler = logging.StreamHandler(sys.stdout)
     console_handler.setFormatter(FORMATTER)
-    return console_handler
-
+    logger.addHandler(console_handler)
 
-def get_file_handler():
-    file_handler = TimedRotatingFileHandler(LOG_FILE, when="midnight")
-    file_handler.setFormatter(FORMATTER)
-    return file_handler
+    if LOG_FILE is not None:
+        file_handler = TimedRotatingFileHandler(LOG_FILE, when="midnight")
+        file_handler.setFormatter(FORMATTER)
+        logger.addHandler(file_handler)
 
-
-def get_logger(logger_name):
-    logger = logging.getLogger(logger_name)
-
-    logger.setLevel(LOG_LEVEL)
-    logger.addHandler(get_console_handler())
-    logger.addHandler(get_file_handler())
     logger.propagate = False
     return logger
```

### Comparing `vortexasdk-0.9.2/vortexasdk/retry_session.py` & `vortexasdk-1.0.0a1/vortexasdk/retry_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from requests import Session, Response
+from requests import Response, Session
 from requests.adapters import HTTPAdapter
 from urllib3 import Retry
 
+_HEADERS = {"Content-Type": "application/json"}
+
 
 # Inspired by https://www.peterbe.com/plog/best-practice-with-retries-with-requests
 def _requests_retry_session(
     retries=6,
     backoff_factor=1,
-    status_forcelist=(500, 502, 504),
+    status_forcelist=(401, 500, 502, 504),
     session=None,
 ) -> Session:
     """Instantiate a session with Retry backoff."""
     session = session or Session()
 
     retry = Retry(
         raise_on_redirect=False,
         raise_on_status=False,
-        method_whitelist=["POST", "GET"],
+        allowed_methods=["POST", "GET"],
         status=retries,
         total=retries,
         read=retries,
         connect=retries,
         backoff_factor=backoff_factor,
         status_forcelist=status_forcelist,
     )
@@ -29,13 +31,13 @@
     session.mount("https://", adapter)
 
     return session
 
 
 def retry_get(*args, **kwargs) -> Response:
     with _requests_retry_session() as s:
-        return s.get(*args, **kwargs)
+        return s.get(headers=_HEADERS, *args, **kwargs)
 
 
 def retry_post(*args, **kwargs) -> Response:
     with _requests_retry_session() as s:
         return s.post(*args, **kwargs)
```

