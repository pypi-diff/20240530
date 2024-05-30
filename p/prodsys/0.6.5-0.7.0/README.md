# Comparing `tmp/prodsys-0.6.5.tar.gz` & `tmp/prodsys-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.6.5.tar", max compression
+gzip compressed data, was "prodsys-0.7.0.tar", max compression
```

## Comparing `prodsys-0.6.5.tar` & `prodsys-0.7.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.6.5/LICENSE
--rw-r--r--   0        0        0      405 2024-05-08 06:54:32.238837 prodsys-0.6.5/prodsys/__init__.py
--rw-r--r--   0        0        0     1289 2024-05-01 05:54:38.231436 prodsys-0.6.5/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    56359 2024-05-05 08:37:15.084888 prodsys-0.6.5/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     8854 2024-05-04 15:39:44.446374 prodsys-0.6.5/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.6.5/prodsys/conf/__init__.py
--rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.6.5/prodsys/conf/logging.ini
--rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.6.5/prodsys/conf/logging_config.py
--rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.6.5/prodsys/control/__init__.py
--rw-r--r--   0        0        0     9030 2024-05-04 15:39:44.446374 prodsys-0.6.5/prodsys/control/routing_control_env.py
--rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.6.5/prodsys/control/sequencing_control_env.py
--rw-r--r--   0        0        0     2307 2024-05-06 07:36:03.343941 prodsys-0.6.5/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.6.5/prodsys/express/core.py
--rw-r--r--   0        0        0     1589 2024-05-04 15:39:44.446374 prodsys-0.6.5/prodsys/express/node.py
--rw-r--r--   0        0        0    11649 2024-05-04 15:39:44.446374 prodsys-0.6.5/prodsys/express/process.py
--rw-r--r--   0        0        0     2477 2024-05-04 15:39:44.457893 prodsys-0.6.5/prodsys/express/product.py
--rw-r--r--   0        0        0     7129 2024-05-04 15:39:44.457893 prodsys-0.6.5/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8295 2024-05-04 15:39:44.457893 prodsys-0.6.5/prodsys/express/resources.py
--rw-r--r--   0        0        0     2573 2024-05-04 15:39:44.464082 prodsys-0.6.5/prodsys/express/sink.py
--rw-r--r--   0        0        0     3413 2024-05-04 15:39:44.464082 prodsys-0.6.5/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2024-05-01 07:15:45.742369 prodsys-0.6.5/prodsys/express/state.py
--rw-r--r--   0        0        0     9374 2024-05-06 07:36:03.343941 prodsys-0.6.5/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.6.5/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     3382 2024-05-08 06:17:55.371995 prodsys-0.6.5/prodsys/factories/link_transport_process_updater.py
--rw-r--r--   0        0        0     1745 2024-05-04 15:39:44.464082 prodsys-0.6.5/prodsys/factories/node_factory.py
--rw-r--r--   0        0        0     3752 2024-05-04 15:39:44.464082 prodsys-0.6.5/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.6.5/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.6.5/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    11157 2024-05-04 15:39:44.464082 prodsys-0.6.5/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.6.5/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.6.5/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.6.5/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2024-05-06 07:18:41.418213 prodsys-0.6.5/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1583 2024-05-04 15:39:44.464082 prodsys-0.6.5/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.6.5/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     1233 2024-05-04 15:39:44.473598 prodsys-0.6.5/prodsys/models/node_data.py
--rw-r--r--   0        0        0     3963 2024-05-05 08:37:15.084888 prodsys-0.6.5/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2024-04-19 09:06:03.048928 prodsys-0.6.5/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0    14397 2024-05-04 15:39:44.476967 prodsys-0.6.5/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     6357 2024-05-04 14:20:57.302536 prodsys-0.6.5/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1931 2024-05-04 14:20:57.303890 prodsys-0.6.5/prodsys/models/queue_data.py
--rw-r--r--   0        0        0    12335 2024-05-04 15:39:44.476967 prodsys-0.6.5/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10745 2024-05-05 05:55:40.858758 prodsys-0.6.5/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     2846 2024-05-04 14:20:57.305926 prodsys-0.6.5/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     4059 2024-05-04 14:20:57.312957 prodsys-0.6.5/prodsys/models/source_data.py
--rw-r--r--   0        0        0    13852 2024-05-04 14:20:57.312957 prodsys-0.6.5/prodsys/models/state_data.py
--rw-r--r--   0        0        0    13285 2024-05-06 07:36:03.343941 prodsys-0.6.5/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.6.5/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    12423 2024-05-05 08:37:15.084888 prodsys-0.6.5/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    28142 2024-05-05 08:37:15.084888 prodsys-0.6.5/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4642 2024-05-04 14:20:57.321008 prodsys-0.6.5/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    46203 2024-05-04 15:39:44.483548 prodsys-0.6.5/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     9523 2024-05-05 08:37:15.091916 prodsys-0.6.5/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    11829 2024-05-05 08:37:15.091916 prodsys-0.6.5/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.6.5/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    31006 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6855 2024-05-01 15:14:08.116047 prodsys-0.6.5/prodsys/simulation/logger.py
--rw-r--r--   0        0        0      459 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/node.py
--rw-r--r--   0        0        0     3765 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9599 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0    11900 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/process.py
--rw-r--r--   0        0        0    10255 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/product.py
--rw-r--r--   0        0        0     5716 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/request.py
--rw-r--r--   0        0        0    18086 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/resources.py
--rw-r--r--   0        0        0     9958 2024-05-06 07:36:03.343941 prodsys-0.6.5/prodsys/simulation/route_finder.py
--rw-r--r--   0        0        0    15942 2024-05-04 15:39:44.489571 prodsys-0.6.5/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3202 2024-05-05 08:37:15.091916 prodsys-0.6.5/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     2260 2024-05-04 14:20:57.328996 prodsys-0.6.5/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     4139 2024-05-06 07:36:03.343941 prodsys-0.6.5/prodsys/simulation/source.py
--rw-r--r--   0        0        0    29728 2024-05-04 15:39:44.505331 prodsys-0.6.5/prodsys/simulation/state.py
--rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.6.5/prodsys/simulation/store.py
--rw-r--r--   0        0        0    14403 2024-05-06 07:36:03.343941 prodsys-0.6.5/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.6.5/prodsys/util/__init__.py
--rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.6.5/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    30349 2024-05-04 14:20:57.328996 prodsys-0.6.5/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    12939 2024-05-06 07:36:03.343941 prodsys-0.6.5/prodsys/util/runner.py
--rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.6.5/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4390 2024-05-04 15:39:44.505331 prodsys-0.6.5/prodsys/util/util.py
--rw-r--r--   0        0        0     1631 2024-05-08 06:54:31.294012 prodsys-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     7237 2024-05-05 08:37:14.995920 prodsys-0.6.5/README.md
--rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 prodsys-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.7.0/LICENSE
+-rw-r--r--   0        0        0      407 2024-05-30 11:41:44.798793 prodsys-0.7.0/prodsys/__init__.py
+-rw-r--r--   0        0        0     1288 2024-05-30 11:41:44.801327 prodsys-0.7.0/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    58496 2024-05-30 11:41:44.803233 prodsys-0.7.0/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     8916 2024-05-30 11:41:44.803811 prodsys-0.7.0/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.7.0/prodsys/conf/__init__.py
+-rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.7.0/prodsys/conf/logging.ini
+-rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.7.0/prodsys/conf/logging_config.py
+-rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.7.0/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9030 2024-05-23 17:55:37.315762 prodsys-0.7.0/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.7.0/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2355 2024-05-30 11:41:44.805577 prodsys-0.7.0/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      469 2024-05-30 11:41:44.807510 prodsys-0.7.0/prodsys/express/core.py
+-rw-r--r--   0        0        0     1568 2024-05-30 11:41:44.809047 prodsys-0.7.0/prodsys/express/node.py
+-rw-r--r--   0        0        0    11370 2024-05-30 11:41:44.809823 prodsys-0.7.0/prodsys/express/process.py
+-rw-r--r--   0        0        0     2543 2024-05-30 11:41:44.811476 prodsys-0.7.0/prodsys/express/product.py
+-rw-r--r--   0        0        0     7136 2024-05-30 11:41:44.811476 prodsys-0.7.0/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8361 2024-05-30 11:41:44.815151 prodsys-0.7.0/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2651 2024-05-30 11:41:44.817046 prodsys-0.7.0/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3424 2024-05-30 11:41:44.817046 prodsys-0.7.0/prodsys/express/source.py
+-rw-r--r--   0        0        0     7622 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/express/state.py
+-rw-r--r--   0        0        0     9338 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.7.0/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     3572 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/link_transport_process_updater.py
+-rw-r--r--   0        0        0     1736 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/node_factory.py
+-rw-r--r--   0        0        0     3807 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6347 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     2006 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    11218 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3261 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5050 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     3006 2024-05-30 11:41:44.819625 prodsys-0.7.0/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2017 2024-05-30 11:41:44.835278 prodsys-0.7.0/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1583 2024-05-23 17:55:37.335415 prodsys-0.7.0/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      578 2024-05-30 11:41:44.835278 prodsys-0.7.0/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     1142 2024-05-30 11:41:44.839363 prodsys-0.7.0/prodsys/models/node_data.py
+-rw-r--r--   0        0        0     3717 2024-05-30 11:41:44.839363 prodsys-0.7.0/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     8544 2024-05-30 11:41:44.839363 prodsys-0.7.0/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0    13869 2024-05-30 11:41:44.846581 prodsys-0.7.0/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     6249 2024-05-30 11:41:44.847357 prodsys-0.7.0/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1883 2024-05-30 11:41:44.851246 prodsys-0.7.0/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0    12223 2024-05-30 11:41:44.852394 prodsys-0.7.0/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10661 2024-05-30 11:41:44.852394 prodsys-0.7.0/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     2772 2024-05-30 11:41:44.852394 prodsys-0.7.0/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     3974 2024-05-30 11:41:44.852394 prodsys-0.7.0/prodsys/models/source_data.py
+-rw-r--r--   0        0        0    13358 2024-05-30 11:41:44.852394 prodsys-0.7.0/prodsys/models/state_data.py
+-rw-r--r--   0        0        0    12776 2024-05-30 11:41:44.852394 prodsys-0.7.0/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.7.0/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    12396 2024-05-30 11:41:44.864391 prodsys-0.7.0/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    28135 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4642 2024-05-04 14:20:57.321008 prodsys-0.7.0/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    46233 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     9562 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    11811 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.7.0/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    30978 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2024-05-01 15:14:08.116047 prodsys-0.7.0/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0      421 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/simulation/node.py
+-rw-r--r--   0        0        0     3727 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9561 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0    12232 2024-05-30 11:41:44.866905 prodsys-0.7.0/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    10164 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     5652 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    17882 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0     9958 2024-05-28 19:49:30.684043 prodsys-0.7.0/prodsys/simulation/route_finder.py
+-rw-r--r--   0        0        0    15942 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3202 2024-05-23 17:55:37.365082 prodsys-0.7.0/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     2242 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     4075 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    29824 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.7.0/prodsys/simulation/store.py
+-rw-r--r--   0        0        0    14378 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.7.0/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.7.0/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    30387 2024-05-30 11:41:44.883447 prodsys-0.7.0/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    12588 2024-05-30 11:41:44.902905 prodsys-0.7.0/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.7.0/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4396 2024-05-30 11:41:44.902905 prodsys-0.7.0/prodsys/util/util.py
+-rw-r--r--   0        0        0     1625 2024-05-30 11:41:44.902905 prodsys-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7237 2024-05-23 17:55:37.194724 prodsys-0.7.0/README.md
+-rw-r--r--   0        0        0     9299 1970-01-01 00:00:00.000000 prodsys-0.7.0/PKG-INFO
```

### Comparing `prodsys-0.6.5/LICENSE` & `prodsys-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/adapters/__init__.py` & `prodsys-0.7.0/prodsys/adapters/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 This module contains the adapters for the production system which are data containers for the data models defined in `prodsys.models`. The adapters are used in all algorithms that analyze or optimize a production system. 
 The data structure of the adapter can also be used to integrate new algorithms into prodsys by utilizing its defined data structure. 
 The adapters is the `prodsys.models` equivalent to the `prodsys.express.ProductionSystem` class and can be created from the express object. In contrast to the adapter, the express class nests the objects in a tree structure, which makes it easier to work with when instantiating a production system, but more complicated when reviewing the data itself.
 The adapter comes with a data validation that ensures that entered data is syntatically, semantically and logically valid. 
 """
-
 from prodsys.adapters.adapter import (
-    ProductionSystemAdapter,
     get_default_queues_for_resource,
     get_default_queue_for_sink,
     get_default_queue_for_source,
     get_machines,
     get_transport_resources,
     get_set_of_IDs,
     get_possible_production_processes_IDs,
     add_default_queues_to_adapter,
-    check_for_clean_compound_processes
+    check_for_clean_compound_processes,
+    ProductionSystemAdapter,
 )
 from prodsys.adapters.json_adapter import JsonProductionSystemAdapter
```

### Comparing `prodsys-0.6.5/prodsys/adapters/adapter.py` & `prodsys-0.7.0/prodsys/adapters/adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from hashlib import md5
-import warnings
 from typing import List, Any, Set, Optional, Tuple, Union
-from numpy import isin
-from pydantic import BaseModel, validator, ValidationError
+from pydantic import BaseModel, ConfigDict, field_validator, ValidationError, ValidationInfo
 
 import logging
 logger = logging.getLogger(__name__)
 
-from prodsys.models import (
-    product_data,
-    queue_data,
-    resource_data,
-    node_data,
-    time_model_data,
-    state_data,
-    processes_data,
-    sink_data,
-    source_data,
-    scenario_data,
-)
+# from prodsys.models import (
+#     time_model_data,
+#     node_data,
+#     product_data,
+#     queue_data,
+#     resource_data,
+#     state_data,
+#     processes_data,
+#     sink_data,
+#     source_data,
+#     scenario_data,
+# )
+from prodsys.models import time_model_data as time_model_data_module
+from prodsys.models import state_data as state_data_module
+from prodsys.models import processes_data as processes_data_module
+from prodsys.models import sink_data as sink_data_module
+from prodsys.models import source_data as source_data_module
+from prodsys.models import resource_data as resource_data_module
+from prodsys.models import product_data as product_data_module
+from prodsys.models import queue_data as queue_data_module
+from prodsys.models import node_data as node_data_module
+from prodsys.models import scenario_data as scenario_data_module
+
+
+
+
 from prodsys.util import util
 
 
-def get_machines(adapter: ProductionSystemAdapter) -> List[resource_data.ProductionResourceData]:
+def get_machines(adapter: ProductionSystemAdapter) -> List[resource_data_module.ProductionResourceData]:
     """
     Returns a list of all machines in the adapter.
 
     Args:
         adapter (ProductionSystemAdapter): ProductionSystemAdapter object
 
     Returns:
-        List[resource_data.ProductionResourceData]: List of all machines in the adapter
+        List[resource_data_module.ProductionResourceData]: List of all machines in the adapter
     """
     return [
         resource
         for resource in adapter.resource_data
-        if isinstance(resource, resource_data.ProductionResourceData)
+        if isinstance(resource, resource_data_module.ProductionResourceData)
     ]
 
 
 def get_transport_resources(
     adapter: ProductionSystemAdapter,
-) -> List[resource_data.TransportResourceData]:
+) -> List[resource_data_module.TransportResourceData]:
     """
     Returns a list of all transport resources in the adapter.
 
     Args:
         adapter (ProductionSystemAdapter): ProductionSystemAdapter object
 
     Returns:
-        List[resource_data.TransportResourceData]: List of all transport resources in the adapter
+        List[resource_data_module.TransportResourceData]: List of all transport resources in the adapter
     """
     return [
         resource
         for resource in adapter.resource_data
-        if isinstance(resource, resource_data.TransportResourceData)
+        if isinstance(resource, resource_data_module.TransportResourceData)
     ]
 
 
 def get_set_of_IDs(list_of_objects: List[Any]) -> Set[str]:
     """
     Returns a set of all IDs of the objects in the list, by utilizing the ID attribute of the objects.
 
@@ -71,46 +83,46 @@
     Returns:
         Set[str]: Set of all IDs of the objects in the list
     """
     return set([obj.ID for obj in list_of_objects])
 
 
 def get_default_queues_for_resource(
-    resource: resource_data.ProductionResourceData,
+    resource: resource_data_module.ProductionResourceData,
     queue_capacity: Union[float, int] = 0.0,
-) -> Tuple[List[queue_data.QueueData], List[queue_data.QueueData]]:
+) -> Tuple[List[queue_data_module.QueueData], List[queue_data_module.QueueData]]:
     """
     Returns a tuple of two lists of default queues for the given resource. The first list contains the default input queues and the second list contains the default output queues.
 
     Args:
-        resource (resource_data.ProductionResourceData): Resource for which the default queues should be returned
+        resource (resource_data_module.ProductionResourceData): Resource for which the default queues should be returned
         queue_capacity (Union[float, int], optional): Capacity of the default queues. Defaults to 0.0 (infinite queue).
 
     Returns:
-        Tuple[List[queue_data.QueueData], List[queue_data.QueueData]]: Tuple of two lists of default queues for the given resource
+        Tuple[List[queue_data_module.QueueData], List[queue_data_module.QueueData]]: Tuple of two lists of default queues for the given resource
     """
     input_queues = [
-        queue_data.QueueData(
+        queue_data_module.QueueData(
             ID=resource.ID + "_default_input_queue",
             description="Default input queue of " + resource.ID,
             capacity=queue_capacity,
         )
     ]
     output_queues = [
-        queue_data.QueueData(
+        queue_data_module.QueueData(
             ID=resource.ID + "_default_output_queue",
             description="Default output queue of " + resource.ID,
             capacity=queue_capacity,
         )
     ]
     return input_queues, output_queues
 
 
 def remove_queues_from_resource(
-    machine: resource_data.ProductionResourceData, adapter: ProductionSystemAdapter
+    machine: resource_data_module.ProductionResourceData, adapter: ProductionSystemAdapter
 ) -> ProductionSystemAdapter:
     if machine.input_queues or machine.output_queues:
         for queue_ID in machine.input_queues + machine.output_queues:
             for queue in adapter.queue_data:
                 if queue.ID == queue_ID:
                     adapter.queue_data.remove(queue)
                     break
@@ -157,27 +169,27 @@
         machine.input_queues = list(get_set_of_IDs(input_queues))
         machine.output_queues = list(get_set_of_IDs(output_queues))
         adapter.queue_data += input_queues + output_queues
     return adapter
 
 
 def get_default_queue_for_source(
-    source: source_data.SourceData, queue_capacity=0.0
-) -> queue_data.QueueData:
+    source: source_data_module.SourceData, queue_capacity=0.0
+) -> queue_data_module.QueueData:
     """
     Returns a default queue for the given source.
 
     Args:
-        source (source_data.SourceData): Source for which the default queue should be returned
+        source (source_data_module.SourceData): Source for which the default queue should be returned
         queue_capacity (float, optional): Capacity of the default queue. Defaults to 0.0 (infinite queue).
 
     Returns:
-        queue_data.QueueData: Default queue for the given source
+        queue_data_module.QueueData: Default queue for the given source
     """
-    return queue_data.QueueData(
+    return queue_data_module.QueueData(
         ID=source.ID + "_default_output_queue",
         description="Default output queue of " + source.ID,
         capacity=queue_capacity,
     )
 
 
 def add_default_queues_to_sources(
@@ -198,27 +210,27 @@
             output_queues = [get_default_queue_for_source(source, queue_capacity)]
             source.output_queues = list(get_set_of_IDs(output_queues))
             adapter.queue_data += output_queues
     return adapter
 
 
 def get_default_queue_for_sink(
-    sink: sink_data.SinkData, queue_capacity=0.0
-) -> queue_data.QueueData:
+    sink: sink_data_module.SinkData, queue_capacity=0.0
+) -> queue_data_module.QueueData:
     """
     Returns a default queue for the given sink.
 
     Args:
-        sink (sink_data.SinkData): Sink for which the default queue should be returned
+        sink (sink_data_module.SinkData): Sink for which the default queue should be returned
         queue_capacity (float, optional): Capacity of the default queue. Defaults to 0.0 (infinite queue).
 
     Returns:
-        queue_data.QueueData: Default queue for the given sink
+        queue_data_module.QueueData: Default queue for the given sink
     """
-    return queue_data.QueueData(
+    return queue_data_module.QueueData(
         ID=sink.ID + "_default_input_queue",
         description="Default input queue of " + sink.ID,
         capacity=queue_capacity,
     )
 
 
 def add_default_queues_to_sinks(
@@ -268,49 +280,49 @@
     Thereby, it is assured that the expected data is used for simulation and optimization. If the data is not valid, an error is raised with information about the reasons for invalidity.
     The adapter targets easy integration of algorithms with each other in different environments. 
     Therefore, the adapter can even be used for integration of new algorithms by serving as a defined data interface. 
 
     Args:
         ID (str, optional): ID of the production system. Defaults to "".
         seed (int, optional): Seed for the random number generator used in simulation. Defaults to 0.
-        time_model_data (List[time_model_data.TIME_MODEL_DATA], optional): List of time models used by the entities in the production system. Defaults to [].
-        state_data (List[state_data.STATE_DATA_UNION], optional): List of states used by the resources in the production system. Defaults to [].
-        process_data (List[processes_data.PROCESS_DATA_UNION], optional): List of processes required by products and provided by resources in the production system. Defaults to [].
-        queue_data (List[queue_data.QueueData], optional): List of queues used by the resources, sources and sinks in the production system. Defaults to [].
-        node_data (List[resource_data.NodeData], optional): List of nodes in the production system. Defaults to [].
-        resource_data (List[resource_data.RESOURCE_DATA_UNION], optional): List of resources in the production system. Defaults to [].
-        product_data (List[product_data.ProductData], optional): List of products in the production system. Defaults to []
-        sink_data (List[sink_data.SinkData], optional): List of sinks in the production system. Defaults to [].
-        source_data (List[source_data.SourceData], optional): List of sources in the production system. Defaults to [].
-        scenario_data (Optional[scenario_data.ScenarioData], optional): Scenario data of the production system used for optimization. Defaults to None.
+        time_model_data (List[time_model_data_module.TIME_MODEL_DATA], optional): List of time models used by the entities in the production system. Defaults to [].
+        state_data (List[state_data_module.STATE_DATA_UNION], optional): List of states used by the resources in the production system. Defaults to [].
+        process_data (List[processes_data_module.PROCESS_DATA_UNION], optional): List of processes required by products and provided by resources in the production system. Defaults to [].
+        queue_data (List[queue_data_module.QueueData], optional): List of queues used by the resources, sources and sinks in the production system. Defaults to [].
+        node_data (List[resource_data_module.NodeData], optional): List of nodes in the production system. Defaults to [].
+        resource_data (List[resource_data_module.RESOURCE_DATA_UNION], optional): List of resources in the production system. Defaults to [].
+        product_data (List[product_data_module.ProductData], optional): List of products in the production system. Defaults to []
+        sink_data (List[sink_data_module.SinkData], optional): List of sinks in the production system. Defaults to [].
+        source_data (List[source_data_module.SourceData], optional): List of sources in the production system. Defaults to [].
+        scenario_data (Optional[scenario_data_module.ScenarioData], optional): Scenario data of the production system used for optimization. Defaults to None.
         valid_configuration (bool, optional): Indicates if the configuration is valid. Defaults to True.
         reconfiguration_cost (float, optional): Cost of reconfiguration in a optimization scenario. Defaults to 0.
     """
     # TODO: add check, that throws an error, if items have the same ID!
     ID: str = ""
     seed: int = 0
-    time_model_data: List[time_model_data.TIME_MODEL_DATA] = []
-    state_data: List[state_data.STATE_DATA_UNION] = []
-    process_data: List[processes_data.PROCESS_DATA_UNION] = []
-    queue_data: List[queue_data.QueueData] = []
-    node_data: List[node_data.NodeData] = []
-    resource_data: List[resource_data.RESOURCE_DATA_UNION] = []
-    product_data: List[product_data.ProductData] = []
-    sink_data: List[sink_data.SinkData] = []
-    source_data: List[source_data.SourceData] = []
-    scenario_data: Optional[scenario_data.ScenarioData] = None
+    time_model_data: List[time_model_data_module.TIME_MODEL_DATA] = []
+    state_data: List[state_data_module.STATE_DATA_UNION] = []
+    process_data: List[processes_data_module.PROCESS_DATA_UNION] = []
+    queue_data: List[queue_data_module.QueueData] = []
+    node_data: List[node_data_module.NodeData] = []
+    resource_data: List[resource_data_module.RESOURCE_DATA_UNION] = []
+    product_data: List[product_data_module.ProductData] = []
+    sink_data: List[sink_data_module.SinkData] = []
+    source_data: List[source_data_module.SourceData] = []
+    scenario_data: Optional[scenario_data_module.ScenarioData] = None
 
 
     valid_configuration: bool = True
     reconfiguration_cost: float = 0
 
-    class Config:
-        validate = True
-        validate_assignment = True
-        schema_extra = {
+
+    model_config = ConfigDict(
+        validate_assignment=True,
+        json_schema_extra={
             "examples": [{
                 "ID": "Example Adapter",
                 "valid_configuration": True,
                 "reconfiguration_cost": 0,
                 "seed": 24,
                 "time_model_data": [
                     {
@@ -673,14 +685,15 @@
                         "output_queues": ["SourceQueue"],
                     },
                 ],
                 "scenario_data": None,
             }
             ]
         }
+    )
 
     def hash(self) -> str:
         """
         Generates a hash of the adapter based on the hash of all contained entities. Only information describing the physical structure and functionality of the production system is considered. Can be used to compare two production systems of adapters for functional equality.
 
         Returns:
             str: Hash of the adapter
@@ -697,146 +710,158 @@
                 *sorted([product.hash(self) for product in self.product_data]),
                 *sorted([sink.hash(self) for sink in self.sink_data]),
                 *sorted([source.hash(self) for source in self.source_data])
                 ]
             )).encode("utf-8")
             ).hexdigest()
 
-    @validator("state_data", each_item=True)
-    def check_states(cls, state: state_data.STATE_DATA_UNION, values):
-        time_models = get_set_of_IDs(values["time_model_data"])
-        if state.time_model_id not in time_models:
-            raise ValueError(
-                f"The time model {state.time_model_id} of state {state.ID} is not a valid time model of {time_models}."
-            )
-        return state
-
-    @validator("process_data", each_item=True)
-    def check_processes(cls, process: processes_data.PROCESS_DATA_UNION, values):
-        if isinstance(process, processes_data.CompoundProcessData) or isinstance(process, processes_data.RequiredCapabilityProcessData):
-            return process
-        time_models = get_set_of_IDs(values["time_model_data"])
-        if process.time_model_id not in time_models:
-            raise ValueError(
-                f"The time model {process.time_model_id} of process {process.ID} is not a valid time model of {time_models}."
-            )
-        return process
+    @field_validator("state_data")
+    def check_states(cls, states: List[state_data_module.STATE_DATA_UNION], info: ValidationInfo):
+        values = info.data
+        for state in states:
+            time_models = get_set_of_IDs(values["time_model_data"])
+            if state.time_model_id not in time_models:
+                raise ValueError(
+                    f"The time model {state.time_model_id} of state {state.ID} is not a valid time model of {time_models}."
+                )
+        return states
 
-    @validator("resource_data", each_item=True)
-    def check_resources(cls, resource: resource_data.RESOURCE_DATA_UNION, values):
-        processes = get_set_of_IDs(values["process_data"])
-        for process in resource.process_ids:
-            if process not in processes:
+    @field_validator("process_data")
+    def check_processes(cls, processes: List[processes_data_module.PROCESS_DATA_UNION], info: ValidationInfo):
+        values = info.data
+        for process in processes:
+            if isinstance(process, processes_data_module.CompoundProcessData) or isinstance(process, processes_data_module.RequiredCapabilityProcessData):
+                continue
+            time_models = get_set_of_IDs(values["time_model_data"])
+            if process.time_model_id not in time_models:
                 raise ValueError(
-                    f"The process {process} of resource {resource.ID} is not a valid process of {processes}."
+                    f"The time model {process.time_model_id} of process {process.ID} is not a valid time model of {time_models}."
                 )
-        states = get_set_of_IDs(values["state_data"])
-        for state in resource.state_ids:
-            if state not in states:
+        return processes
+
+    @field_validator("resource_data")
+    def check_resources(cls, resources: List[resource_data_module.RESOURCE_DATA_UNION], info: ValidationInfo):
+        values = info.data
+        for resource in resources:
+            processes = get_set_of_IDs(values["process_data"])
+            for process in resource.process_ids:
+                if process not in processes:
+                    raise ValueError(
+                        f"The process {process} of resource {resource.ID} is not a valid process of {processes}."
+                    )
+            states = get_set_of_IDs(values["state_data"])
+            for state in resource.state_ids:
+                if state not in states:
+                    raise ValueError(
+                        f"The state {state} of resource {resource.ID} is not a valid state of {states}."
+                    )
+            if isinstance(resource, resource_data_module.ProductionResourceData):
+                queues = get_set_of_IDs(values["queue_data"])
+                if resource.input_queues and resource.output_queues:
+                    for queue in resource.input_queues + resource.output_queues:
+                        if queue not in queues:
+                            raise ValueError(
+                                f"The queue {queue} of resource {resource.ID} is not a valid queue of {queues}."
+                            )
+                else:
+                    input_queues, output_queues = get_default_queues_for_resource(resource)
+                    resource.input_queues = list(get_set_of_IDs(input_queues))
+                    resource.output_queues = list(get_set_of_IDs(output_queues))
+                    values["queue_data"] += input_queues + output_queues
+
+        return resources
+
+    @field_validator("product_data")
+    def check_products(cls, products: List[product_data_module.ProductData], info: ValidationInfo):
+        values = info.data
+        for product in products:
+            all_processes = get_set_of_IDs(values["process_data"])
+            if product.transport_process not in all_processes:
+                raise ValidationError(
+                    f"The transport process {product.transport_process} of product {product.ID} is not a valid process of {all_processes}."
+                )
+            required_processes = set()
+            if isinstance(product.processes, list) and isinstance(
+                product.processes[0], str
+            ):
+                required_processes = set(product.processes)
+            elif isinstance(product.processes, list) and isinstance(
+                product.processes[0], list
+            ):
+                required_processes = set(util.flatten(product.processes))
+            elif isinstance(product.processes, dict):
+                required_processes = set(product.processes.keys())
+            if required_processes - all_processes != set():
                 raise ValueError(
-                    f"The state {state} of resource {resource.ID} is not a valid state of {states}."
+                    f"The processes {required_processes - all_processes} of product {product.ID} are not a valid processes of {all_processes}."
                 )
-        if isinstance(resource, resource_data.ProductionResourceData):
-            queues = get_set_of_IDs(values["queue_data"])
-            if resource.input_queues and resource.output_queues:
-                for queue in resource.input_queues + resource.output_queues:
-                    if queue not in queues:
-                        raise ValueError(
-                            f"The queue {queue} of resource {resource.ID} is not a valid queue of {queues}."
-                        )
-            else:
-                input_queues, output_queues = get_default_queues_for_resource(resource)
-                resource.input_queues = list(get_set_of_IDs(input_queues))
-                resource.output_queues = list(get_set_of_IDs(output_queues))
-                values["queue_data"] += input_queues + output_queues
-
-        return resource
-
-    @validator("product_data", each_item=True)
-    def check_products(cls, product: product_data.ProductData, values):
-        all_processes = get_set_of_IDs(values["process_data"])
-        if product.transport_process not in all_processes:
-            raise ValidationError(
-                f"The transport process {product.transport_process} of product {product.ID} is not a valid process of {all_processes}."
-            )
-        required_processes = set()
-        if isinstance(product.processes, list) and isinstance(
-            product.processes[0], str
-        ):
-            required_processes = set(product.processes)
-        elif isinstance(product.processes, list) and isinstance(
-            product.processes[0], list
-        ):
-            required_processes = set(util.flatten(product.processes))
-        elif isinstance(product.processes, dict):
-            required_processes = set(product.processes.keys())
-        if required_processes - all_processes != set():
-            raise ValueError(
-                f"The processes {required_processes - all_processes} of product {product.ID} are not a valid processes of {all_processes}."
-            )
 
-        return product
+        return products
 
-    @validator("sink_data", each_item=True)
-    def check_sinks(cls, sink: sink_data.SinkData, values):
-        try:
-            products = get_set_of_IDs(values["product_data"])
-        except KeyError:
-            raise ValueError("Product data is missing or faulty.")
-        if sink.product_type not in products:
-            raise ValueError(
-                f"The product type {sink.product_type} of sink {sink.ID} is not a valid product of {products}."
-            )
-        if not sink.input_queues:
-            input_queue = get_default_queue_for_sink(sink)
-            sink.input_queues = list(get_set_of_IDs([input_queue]))
-            values["queue_data"] += [input_queue]
-            return sink
-        queues = get_set_of_IDs(values["queue_data"])
-        for q in sink.input_queues:
-            if q not in queues:
+    @field_validator("sink_data")
+    def check_sinks(cls, sinks: List[sink_data_module.SinkData], info: ValidationInfo):
+        values = info.data
+        for sink in sinks:
+            try:
+                products = get_set_of_IDs(values["product_data"])
+            except KeyError:
+                raise ValueError("Product data is missing or faulty.")
+            if sink.product_type not in products:
                 raise ValueError(
-                    f"The queue {q} of sink {sink.ID} is not a valid queue of {queues}."
+                    f"The product type {sink.product_type} of sink {sink.ID} is not a valid product of {products}."
                 )
-            for queue in values["queue_data"]:
-                if queue.ID == q:
-                    if queue.capacity != 0:
-                        logger.warning(
-                            f"The capacity of the queue {queue.ID} of sink {sink.ID} is limited. This might lead to unexpected behavior so it was changed to infinity."
-                        )
-                        queue.capacity = 0
-        return sink
-
-    @validator("source_data", each_item=True)
-    def check_sources(cls, source: source_data.SourceData, values):
-        time_models = get_set_of_IDs(values["time_model_data"])
-        if source.time_model_id not in time_models:
-            raise ValueError(
-                f"The time model {source.time_model_id} of source {source.ID} is not a valid time model of {time_models}."
-            )
-        try:
-            products = get_set_of_IDs(values["product_data"])
-        except KeyError:
-            raise ValueError("Product data is missing or faulty.")
-        if source.product_type not in products:
-            raise ValueError(
-                f"The product type {source.product_type} of source {source.ID} is not a valid product of {products}."
-            )
-        if not source.output_queues:
-            output_queue = get_default_queue_for_source(source)
-            source.output_queues = list(get_set_of_IDs([output_queue]))
-            values["queue_data"] += [output_queue]
-            return source
-        queues = get_set_of_IDs(values["queue_data"])
-        for q in source.output_queues:
-            if q not in queues:
+            if not sink.input_queues:
+                input_queue = get_default_queue_for_sink(sink)
+                sink.input_queues = list(get_set_of_IDs([input_queue]))
+                values["queue_data"] += [input_queue]
+                continue
+            queues = get_set_of_IDs(values["queue_data"])
+            for q in sink.input_queues:
+                if q not in queues:
+                    raise ValueError(
+                        f"The queue {q} of sink {sink.ID} is not a valid queue of {queues}."
+                    )
+                for queue in values["queue_data"]:
+                    if queue.ID == q:
+                        if queue.capacity != 0:
+                            logger.warning(
+                                f"The capacity of the queue {queue.ID} of sink {sink.ID} is limited. This might lead to unexpected behavior so it was changed to infinity."
+                            )
+                            queue.capacity = 0
+        return sinks
+
+    @field_validator("source_data")
+    def check_sources(cls, sources: List[source_data_module.SourceData], info: ValidationInfo):
+        values = info.data
+        for source in sources:
+            time_models = get_set_of_IDs(values["time_model_data"])
+            if source.time_model_id not in time_models:
+                raise ValueError(
+                    f"The time model {source.time_model_id} of source {source.ID} is not a valid time model of {time_models}."
+                )
+            try:
+                products = get_set_of_IDs(values["product_data"])
+            except KeyError:
+                raise ValueError("Product data is missing or faulty.")
+            if source.product_type not in products:
                 raise ValueError(
-                    f"The queue {q} of source {source.ID} is not a valid queue of {queues}."
+                    f"The product type {source.product_type} of source {source.ID} is not a valid product of {products}."
                 )
-        return source
+            if not source.output_queues:
+                output_queue = get_default_queue_for_source(source)
+                source.output_queues = list(get_set_of_IDs([output_queue]))
+                values["queue_data"] += [output_queue]
+                continue
+            queues = get_set_of_IDs(values["queue_data"])
+            for q in source.output_queues:
+                if q not in queues:
+                    raise ValueError(
+                        f"The queue {q} of source {source.ID} is not a valid queue of {queues}."
+                    )
+        return sources
 
     @abstractmethod
     def read_data(self, file_path: str, scenario_file_path: Optional[str] = None):
         """
         Reads the data from the given file path and scenario file path.
 
         Args:
@@ -852,15 +877,15 @@
 
         Args:
             file_path (str): File path for the production system configuration
         """
         pass
 
     def read_scenario(self, scenario_file_path: str):
-        self.scenario_data = scenario_data.ScenarioData.parse_file(scenario_file_path)
+        self.scenario_data = scenario_data_module.ScenarioData.parse_file(scenario_file_path)
 
     def validate_proceses_available(self):
         required_processes = set(
             util.flatten([product.processes for product in self.product_data])
         )
         available_processes = set()
         for resource in self.resource_data:
@@ -917,15 +942,15 @@
 
     Args:
         adapter (ProductionSystemAdapter): Production system configuration
 
     Raises:
         ValueError: If the start or target of a link is not a valid location.
     """
-    link_transport_processes = [process for process in adapter.process_data if isinstance(process, processes_data.LinkTransportProcessData)]
+    link_transport_processes = [process for process in adapter.process_data if isinstance(process, processes_data_module.LinkTransportProcessData)]
     if not link_transport_processes:
         return 
     nodes = get_set_of_IDs(adapter.node_data)
     resources = get_set_of_IDs(adapter.resource_data)
     sources = get_set_of_IDs(adapter.source_data)
     sinks = get_set_of_IDs(adapter.sink_data)
     all_location_ids = nodes | resources | sources | sinks
@@ -974,16 +999,16 @@
 
     Args:
         adapter_object (ProductionSystemAdapter): Production system configuration
 
     Returns:
         Union[List[str], List[Tuple[str, ...]]]: List of production process IDs
     """
-    possible_processes = [process for process in adapter_object.process_data if not isinstance(process, processes_data.TransportProcessData) and not isinstance(process, processes_data.RequiredCapabilityProcessData)]  
-    compund_processes = [process for process in adapter_object.process_data if isinstance(process, processes_data.CompoundProcessData)]
+    possible_processes = [process for process in adapter_object.process_data if not isinstance(process, processes_data_module.TransportProcessData) and not isinstance(process, processes_data_module.RequiredCapabilityProcessData)]  
+    compund_processes = [process for process in adapter_object.process_data if isinstance(process, processes_data_module.CompoundProcessData)]
     compound_process_id_tuples = [tuple(compound_process.process_ids) for compound_process in compund_processes]
 
     compound_processes_ids = set([compound_process.ID for compound_process in compund_processes])
     compound_processes_contained_process_ids = set(util.flatten(compound_process_id_tuples))
     individual_processes_ids = [process.ID for process in possible_processes if process.ID not in compound_processes_contained_process_ids and process.ID not in compound_processes_ids]
     
     return individual_processes_ids + compound_process_id_tuples
@@ -992,169 +1017,169 @@
 def get_possible_transport_processes_IDs(
     adapter_object: ProductionSystemAdapter,
 ) -> List[str]:
     possible_processes = adapter_object.process_data
     return [
         process.ID
         for process in possible_processes
-        if isinstance(process, processes_data.TransportProcessData)
+        if isinstance(process, processes_data_module.TransportProcessData)
     ]
 
 
 def get_production_processes_from_ids(
     adapter_object: ProductionSystemAdapter, process_ids: List[str]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
-            if process.ID == process_id and isinstance(process, processes_data.ProductionProcessData):
+            if process.ID == process_id and isinstance(process, processes_data_module.ProductionProcessData):
                 processes.append(process)
                 break
     return processes
 
 
 def get_transport_processes_from_ids(
     adapter_object: ProductionSystemAdapter, process_ids: List[str]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
-            if process.ID == process_id and isinstance(process, processes_data.TransportProcessData) and not (hasattr(process, "capability") and getattr(process, "capability")):
+            if process.ID == process_id and isinstance(process, processes_data_module.TransportProcessData) and not (hasattr(process, "capability") and getattr(process, "capability")):
                 processes.append(process)
                 break
     return processes
 
 def get_capability_processes_from_ids(
         adapter_object: ProductionSystemAdapter, process_ids: List[str]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
-            if process.ID == process_id and (isinstance(process, processes_data.CapabilityProcessData) or (hasattr(process, "capability") and getattr(process, "capability"))):
+            if process.ID == process_id and (isinstance(process, processes_data_module.CapabilityProcessData) or (hasattr(process, "capability") and getattr(process, "capability"))):
                 processes.append(process)
                 break
     return processes
 
 
 def get_compound_processes_from_ids(
     adapter_object: ProductionSystemAdapter, process_ids: List[str]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
-            if process.ID == process_id and isinstance(process, processes_data.CompoundProcessData):
+            if process.ID == process_id and isinstance(process, processes_data_module.CompoundProcessData):
                 processes.append(process)
     return processes
 
 
 def get_required_capability_processes_from_ids(
     adapter_object: ProductionSystemAdapter, process_ids: List[str]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for process_id in process_ids:
         for process in adapter_object.process_data:
-            if process.ID == process_id and isinstance(process, processes_data.RequiredCapabilityProcessData):
+            if process.ID == process_id and isinstance(process, processes_data_module.RequiredCapabilityProcessData):
                 processes.append(process)
     return processes
 
 def get_contained_production_processes_from_compound_processes(
-    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data.CompoundProcessData]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data_module.CompoundProcessData]
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for compound_process in compound_processes:
         for process_id in compound_process.process_ids:
             processes = get_production_processes_from_ids(adapter_object, [process_id])
             if len(processes) > 1:
                 raise ValueError(f"Multiple processes with ID {process_id} found.")
             if processes:
                 process = processes[0]
                 processes.append(process)
     return processes
 
 def get_contained_capability_processes_from_compound_processes(
-    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data.CompoundProcessData]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data_module.CompoundProcessData]
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for compound_process in compound_processes:
         for process_id in compound_process.process_ids:
             processes = get_capability_processes_from_ids(adapter_object, [process_id])
             if len(processes) > 1:
                 raise ValueError(f"Multiple processes with ID {process_id} found.")
             if processes:
                 process = processes[0]
                 processes.append(process)
     return processes
 
 def get_contained_transport_processes_from_compound_processes(
-    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data.CompoundProcessData]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data_module.CompoundProcessData]
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for compound_process in compound_processes:
         for process_id in compound_process.process_ids:
             processes = get_transport_processes_from_ids(adapter_object, [process_id])
             if len(processes) > 1:
                 raise ValueError(f"Multiple processes with ID {process_id} found.")
             if processes:
                 process = processes[0]
                 processes.append(process)
     return processes
     
 
 def get_contained_required_capability_processes_from_compound_processes(
-    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data.CompoundProcessData]
-) -> List[processes_data.PROCESS_DATA_UNION]:
+    adapter_object: ProductionSystemAdapter, compound_processes: List[processes_data_module.CompoundProcessData]
+) -> List[processes_data_module.PROCESS_DATA_UNION]:
     processes = []
     for compound_process in compound_processes:
         for process_id in compound_process.process_ids:
             processes = get_required_capability_processes_from_ids(adapter_object, [process_id])
             if len(processes) > 1:
                 raise ValueError(f"Multiple processes with ID {process_id} found.")
             process = processes[0]
             processes.append(process)
     return processes
 
 
-def assert_production_processes_available(available: List[processes_data.ProductionProcessData], required: List[processes_data.ProductionProcessData]):
+def assert_production_processes_available(available: List[processes_data_module.ProductionProcessData], required: List[processes_data_module.ProductionProcessData]):
     """
     Checks if all required production processes are available.
 
     Args:
-        available (List[processes_data.ProductionProcessData]): production processes that are available in the production system resources
-        required (List[processes_data.ProductionProcessData]): production processes that are required from the products
+        available (List[processes_data_module.ProductionProcessData]): production processes that are available in the production system resources
+        required (List[processes_data_module.ProductionProcessData]): production processes that are required from the products
     Raises:
         ValueError: If required production processes are not available
     """
     available = set([process.ID for process in available])
     required = set([process.ID for process in required])
     if required - available != set():
         raise ValueError(f"Required production processes {required - available} are not available.")
 
-def assert_transport_processes_available(available: List[processes_data.TransportProcessData], required: List[processes_data.TransportProcessData]):
+def assert_transport_processes_available(available: List[processes_data_module.TransportProcessData], required: List[processes_data_module.TransportProcessData]):
     """
     Checks if all required transport processes are available.
 
     Args:
-        available (List[processes_data.TransportProcessData]): transport processes that are available in the production system resources
-        required (List[processes_data.TransportProcessData]): transport processes that are required from the products
+        available (List[processes_data_module.TransportProcessData]): transport processes that are available in the production system resources
+        required (List[processes_data_module.TransportProcessData]): transport processes that are required from the products
 
     Raises:
         ValueError: If required transport processes are not available
     """
     available = set([process.ID for process in available])
     required = set([process.ID for process in required])
     if required - available != set():
         raise ValueError(f"Required transport processes {required - available} are not available.")
 
-def assert_capability_processes_available(available: List[processes_data.CapabilityProcessData], required: List[processes_data.CapabilityProcessData]):
+def assert_capability_processes_available(available: List[processes_data_module.CapabilityProcessData], required: List[processes_data_module.CapabilityProcessData]):
     """
     Checks if all required capability processes are available.
 
     Args:
-        available (List[processes_data.CapabilityProcessData]): capability processes that are available in the production system resources
-        required (List[processes_data.CapabilityProcessData]): capability processes that are required from the products
+        available (List[processes_data_module.CapabilityProcessData]): capability processes that are available in the production system resources
+        required (List[processes_data_module.CapabilityProcessData]): capability processes that are required from the products
 
     Raises:
         ValueError: If required capability processes are not available
     """
     available = set([process.capability for process in available])
     required = set([process.capability for process in required])
     if required - available != set():
```

### Comparing `prodsys-0.6.5/prodsys/adapters/json_adapter.py` & `prodsys-0.7.0/prodsys/adapters/json_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import json
 from abc import ABC, abstractmethod
 from typing import List, Dict, Any, Optional
-from pydantic import parse_obj_as, BaseModel
+from pydantic import BaseModel
+from pydantic import TypeAdapter
 from warnings import warn
 
 
 from prodsys.adapters import adapter
 
 from prodsys.models import (
     product_data,
@@ -113,23 +114,23 @@
     
     def create_objects_from_configuration_data_old(
         self, configuration_data: Dict[str, Any], type
     ):  
         warn("This method is deprecated. Use create_objects_from_configuration_data instead.", DeprecationWarning)
         objects = []
         for values in configuration_data.values():
-            objects.append(parse_obj_as(type, values))
+            objects.append(TypeAdapter(type).validate_python(values))
         return objects
     
     def create_objects_from_configuration_data(
         self, configuration_data: List[Any], type
     ):  
         objects = []
         for values in configuration_data:
-            objects.append(parse_obj_as(type, values))
+            objects.append(TypeAdapter(type).validate_python(values))
         return objects
 
     def write_data(self, file_path: str):
         """
         Writes the data to the given file path.
 
         Args:
@@ -159,13 +160,13 @@
     def write_scenario_data(self, file_path: str) -> None:
         """
         Writes the scenario data to the given file path.
 
         Args:
             file_path (str): File path for the scenario data.
         """
-        data = self.scenario_data.dict()
+        data = self.scenario_data.model_dump()
         with open(file_path, "w") as json_file:
             json.dump(data, json_file)
 
     def get_list_of_dict_objects(self, values: List[BaseModel]) -> List[dict]:
-        return  [data.dict() for data in values]
+        return  [data.model_dump() for data in values]
```

### Comparing `prodsys-0.6.5/prodsys/conf/logging.ini` & `prodsys-0.7.0/prodsys/conf/logging.ini`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/conf/logging_config.py` & `prodsys-0.7.0/prodsys/conf/logging_config.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/control/routing_control_env.py` & `prodsys-0.7.0/prodsys/control/routing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/control/sequencing_control_env.py` & `prodsys-0.7.0/prodsys/control/sequencing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/express/__init__.py` & `prodsys-0.7.0/prodsys/express/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 - `prodsys.express.resources`: Contains classes to specify resources.
 - `prodsys.express.sink`: Contains classes to specify sinks.
 - `prodsys.express.source`: Contains classes to specify sources.
 - `prodsys.express.state`: Contains classes to specify states.
 - `prodsys.express.time_model`: Contains classes to specify time models.
 
 """
+from prodsys.express.core import ExpressObject
 from prodsys.express.time_model import (
     SampleTimeModel,
     ScheduledTimeModel,
     FunctionTimeModel,
     DistanceTimeModel,
     SequentialTimeModel,
     ManhattanDistanceTimeModel,
 )
+from prodsys.express.state import SetupState, BreakDownState, ProcessBreakdownState
+from prodsys.express.node import Node
 from prodsys.express.process import (
     ProductionProcess,
     CapabilityProcess,
     RequiredCapabilityProcess,
     TransportProcess,
     LinkTransportProcess,
 )
-from prodsys.express.state import SetupState, BreakDownState, ProcessBreakdownState
 from prodsys.express.resources import ProductionResource, TransportResource
-from prodsys.express.node import Node
 from prodsys.express.product import Product
 from prodsys.express.source import Source
 from prodsys.express.sink import Sink
 from prodsys.express.production_system import ProductionSystem
```

### Comparing `prodsys-0.6.5/prodsys/express/node.py` & `prodsys-0.7.0/prodsys/express/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,41 @@
 A Node is the express object for a NodeData object in the models API. It represents a location in the production system layout, 
 used for LinkTransportProcesses to specify crossroads or specific locations for transport.
 """
 from typing import Optional
 from uuid import uuid1
 
 
-from pydantic import Field, conlist
+from pydantic import ConfigDict, Field, conlist
 from pydantic.dataclasses import dataclass
 
-from prodsys.models import node_data
-
 from prodsys.express import core
 
+from prodsys.models import node_data
+
 @dataclass
 class Node(core.ExpressObject):
         """
         Represents a node data object of a link, which is just a location in the production system layout. 
 
         Attributes:
                 location (List[float]): Location of the node. It has to be a list of length 2.
         """
-        location: conlist(float, min_items=2, max_items=2) # type: ignore
+        location: conlist(float, min_length=2, max_length=2) # type: ignore
         ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
-        class Config:
-                schema_extra = {
-                "example": {
-                        "summary": "Node",
-                        "value": {
-                        "ID": "N1",
-                        "description": "Node 1",
-                        "location": [0.0, 0.0],
-                        },
-                }
-            }
+        model_config=ConfigDict(json_schema_extra= {
+                "examples": [
+                        {
+                                "ID": "N1",
+                                "description": "Node 1",
+                                "location": [0.0, 0.0],
+                        }
+                ]
+        })
                 
         def to_model(self) -> node_data.NodeData:
              """
              Function returns a NodeData object from the Node object.
              """
              return node_data.NodeData(
                   ID = self.ID,
```

### Comparing `prodsys-0.6.5/prodsys/express/process.py` & `prodsys-0.7.0/prodsys/express/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,14 @@
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from prodsys.express import core, time_model
 from prodsys.models import processes_data
 
-if TYPE_CHECKING:
-    from prodsys.express.resources import Resource
-    from prodsys.express.source import Source
-    from prodsys.express.sink import Sink
-    from prodsys.express.node import Node
-
 @dataclass
 class Process(ABC):
     """
     Abstract base class to represents a process.
 
     Args:
         time_model (time_model.TIME_MODEL_UNION): Time model of the process.
@@ -194,14 +188,15 @@
         return processes_data.TransportProcessData(
             time_model_id=self.time_model.ID,
             ID=self.ID,
             description="",
             type=self.type
         )
 
+
 @dataclass
 class LinkTransportProcess(TransportProcess):
     """
     Represents a link transport process. They include a list or dict of links.
 
     Attributes:
         type (processes_data.ProcessTypeEnum): The type of the process.
@@ -215,38 +210,35 @@
             mapping from a key (which can be a ProductionResource, NodeData, Source, or Sink) to a list of these objects.
         capability (Optional[str]): The capability of the process.
     """
 
     type: processes_data.ProcessTypeEnum = Field(
         init=False, default=processes_data.ProcessTypeEnum.LinkTransportProcesses
     )
-    links: Union[List[List[Union[Resource, Node, Source, Sink]]], 
-                 Dict[Union[Resource, Node, Source, Sink], 
-                      List[Union[Resource, Node, Source, Sink]]]] = Field(default_factory=list)
+    links: Union[List[List[Union[resources.Resource, sink.Sink, source.Source, node.Node]]], 
+                 Dict[Union[resources.Resource, sink.Sink, source.Source, node.Node], 
+                      List[Union[resources.Resource, sink.Sink, source.Source, node.Node]]]] = Field(default_factory=list)
     capability: Optional[str] = Field(default_factory=str)
 
-    def __post_init__(self):
-        self.__pydantic_model__.update_forward_refs(**globals())
-
-    def add_link(self, link: List[Union[Resource, Node, Source, Sink]]) -> None:
+    def add_link(self, link: List[Union[resources.Resource, sink.Sink, source.Source, node.Node]]) -> None:
         """
         Adds a link to the LinkTransportProcess object.
 
         Args:
             link (Union[Resource, Node, Source, Sink]): The link to add.
             link_list (List[Union[Resource, Node, Source, Sink]]): The list of links to add the link to.
         """
         if isinstance(self.links, list):
             self.links.append(link)
         else:
             if not link in self.links:
                 self.links[link] = []
             self.links[link[0]] = link[1]
 
-    def set_links(self, links: List[List[Union[Resource, Node, Source, Sink]]]) -> None:
+    def set_links(self, links: List[List[Union[resources.Resource, node.Node, source.Source, sink.Sink]]]) -> None:
         """
         Sets the links of the LinkTransportProcess object.
 
         Args:
             links (List[List[Union[Resource, Node, Source, Sink]]]): The links to set.
         """
         self.links = links
@@ -270,15 +262,15 @@
             time_model_id=self.time_model.ID,
             ID=self.ID,
             description="",
             type=self.type,
             links=return_links,
             capability=self.capability,
         )
-    
+
 
 @dataclass
 class RequiredCapabilityProcess(core.ExpressObject):
     """
     Represents a required capability process. A capability which can be matched with the capability of a linktransportprocess.
 
     Attributes:
@@ -311,11 +303,8 @@
 PROCESS_UNION = Union[
     ProductionProcess,
     CapabilityProcess,
     TransportProcess,
     RequiredCapabilityProcess,
     LinkTransportProcess,
 ]
-from prodsys.express.resources import Resource
-from prodsys.express.source import Source
-from prodsys.express.sink import Sink
-from prodsys.express.node import Node
+from prodsys.express import resources, sink, source, node
```

### Comparing `prodsys-0.6.5/prodsys/express/product.py` & `prodsys-0.7.0/prodsys/express/product.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from __future__ import annotations
+
 from typing import List, Optional, Union
 from uuid import uuid1
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
 from prodsys.models import product_data
 
-from prodsys.express import core, process
+from prodsys.express import core
 
 @dataclass
 class Product(core.ExpressObject):
     """
     Class that represents a product.
 
     Args:
@@ -59,7 +61,9 @@
         """
         return product_data.ProductData(
             ID=self.ID,
             description="",
             processes=[process.ID for process in self.processes],
             transport_process=self.transport_process.ID,
         )
+
+from prodsys.express import process
```

### Comparing `prodsys-0.6.5/prodsys/express/production_system.py` & `prodsys-0.7.0/prodsys/express/production_system.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 from typing import List, Optional, Union
 
 
-from pydantic import Field
+from pydantic import Field, PrivateAttr
 from pydantic.dataclasses import dataclass
 
-import prodsys
 from prodsys.util import util
+from prodsys.util import runner
+from prodsys.adapters import adapter, json_adapter
 
 from prodsys.express import (
-    core,
-    node,
-    product,
-    resources,
-    source,
-    sink,
-    process,
-    time_model,
-    state,
-    process
+    core, node, resources, source, time_model, state, process, product, sink
 )
 
 
 def remove_duplicate_items(
     items: List[
         Union[
             resources.Resource,
@@ -52,37 +44,36 @@
     for item in items:
         if item.ID in id_set:
             continue
         id_set.add(item.ID)
         filtered_items.append(item)
     return filtered_items
 
-
 @dataclass
 class ProductionSystem(core.ExpressObject):
     """
     Class that represents a production system. A production system containts of resources, products, sources and sinks.
     It is the `prodsys.express` equivalent to the 'ProductionSystemAdapter' of the `prodsys.adapters` module and
     can be converted to this data object. In contrast to the adapter,
     this class nests the objects in a tree structure, which makes it easier to work with when instantiating
     a production system, but more complicated when reviewing the data itself.
 
     Args:
         resources (List[resources.Resource]): Resources of the production system.
         sources (List[source.Source]): Sources of the production system.
         sinks (List[sink.Sink]): Sinks of the production system.
     """
-
     resources: List[Union[resources.ProductionResource, resources.TransportResource]]
     sources: List[source.Source]
     sinks: List[sink.Sink]
 
-    _runner: Optional[prodsys.runner.Runner] = Field(default=None, init=False)
+    def __post_init__(self):
+        self._runner: Optional[runner.Runner] = None
 
-    def to_model(self) -> prodsys.adapters.ProductionSystemAdapter:
+    def to_model(self) -> adapter.ProductionSystemAdapter:
         """
         Converts the `prodsys.express` object to a data object from `prodsys.models`.
 
         Returns:
             prodsys.adapters.Adapter: An instance of the data object.
         """
         products = [source.product for source in self.sources] + [
@@ -147,15 +138,15 @@
                     r._output_queues
                     for r in self.resources
                     if isinstance(r, resources.ProductionResource)
                 ]
                 + [s._input_queues for s in self.sinks]
             )
         )
-        return prodsys.adapters.JsonProductionSystemAdapter(
+        return json_adapter.JsonProductionSystemAdapter(
             time_model_data=time_model_data,
             process_data=process_data,
             state_data=state_data,
             node_data=nodes_data,
             product_data=product_data,
             nodes_data=nodes_data,
             resource_data=resource_data,
@@ -168,15 +159,15 @@
         """
         Runs the simulation of the production system.
         
         Args:
             time_range (float, optional): The time range of the simulation. Defaults to 2880.
             seed (int, optional): The seed of the simulation. Defaults to 0.
         """
-        self._runner = prodsys.runner.Runner(adapter=self.to_model())
+        self._runner = runner.Runner(adapter=self.to_model())
         self._runner.adapter.seed = seed
         self._runner.initialize_simulation()
         self._runner.run(time_range)
 
     def validate(self):
         """
         Validates the production system. Checks if the production system is valid.
```

### Comparing `prodsys-0.6.5/prodsys/express/resources.py` & `prodsys-0.7.0/prodsys/express/resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,59 +2,60 @@
 In `prodsys` exist two different types of resources: production resources and transport resources. Production resources are resources that can perform processes on products. Transport resources are resources that can transport products from one location to another. Both types of resources are represented by the `Resource` class. The `Resource` class is an abstract base class and cannot be instantiated. Instead, the `ProductionResource` and `TransportResource` classes can be used to represent production resources and transport resources, respectively.
 
 The following resources are available:
 
 - `ProductionResource`: Class that represents a production resource.
 - `TransportResource`: Class that represents a transport resource.
 """
+from __future__ import annotations
+
 from typing import List, Optional, Union
 from uuid import uuid1
 
 from abc import ABC
 
 from pydantic import Field, conlist
 from pydantic.dataclasses import dataclass
 
+from prodsys.express import core
+
 from prodsys.models import resource_data, queue_data
 import prodsys
 
-from prodsys.express import core, process, state
-
-
 @dataclass
 class Resource(ABC):
     """
     Abstract base class to represents a resource.
 
     Args:
         processes (List[process.PROCESS_UNION]): Processes of the resource.
-        location (conlist(float, min_items=2, max_items=2)): Location of the resource.
+        location (conlist(float, min_length=2, max_length=2)): Location of the resource.
         capacity (int): Capacity of the resource. Defaults to 1.
         states (Optional[List[state.STATE_UNION]], optional): States of the resource. Defaults to None.
         controller (resource_data.ControllerEnum, optional): Controller of the resource. Defaults to resource_data.ControllerEnum.PipelineController.
         control_policy (resource_data.ResourceControlPolicy, optional): Control policy of the resource. Defaults to resource_data.ResourceControlPolicy.FIFO.
         ID (str): ID of the resource.
     """
     processes: List[process.PROCESS_UNION]
-    location: conlist(float, min_items=2, max_items=2) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) # type: ignore
     capacity: int = 1
     states: Optional[List[state.STATE_UNION]] = Field(default_factory=list)
     controller: resource_data.ControllerEnum = resource_data.ControllerEnum.PipelineController
     control_policy: Union[resource_data.ResourceControlPolicy, resource_data.TransportControlPolicy] = resource_data.ResourceControlPolicy.FIFO
     ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
 
 @dataclass
 class ProductionResource(Resource, core.ExpressObject):
     """
     Class that represents a production resource.
 
     Args:
         processes (List[process.ProductionProcess]): Processes of the resource.
-        location (conlist(float, min_items=2, max_items=2)): Location of the resource.
+        location (conlist(float, min_length=2, max_length=2)): Location of the resource.
         capacity (int): Capacity of the resource. Defaults to 1.
         states (Optional[List[state.STATE_UNION]], optional): States of the resource. Defaults to None.
         controller (resource_data.ControllerEnum, optional): Controller of the resource. Defaults to resource_data.ControllerEnum.PipelineController.
         control_policy (resource_data.ResourceControlPolicy, optional): Control policy of the resource. Defaults to resource_data.ResourceControlPolicy.FIFO.
         queue_size (Optional[int], optional): Queue size of the resource. Defaults to 0 (infinte queue).
         ID (str): ID of the resource.
 
@@ -102,30 +103,30 @@
             ID=self.ID,
             description="",
             process_ids=[process.ID for process in self.processes],
             location=self.location,
             capacity=self.capacity,
             state_ids=[state.ID for state in self.states],
             controller=self.controller,
-            control_policy=self.control_policy,
+            control_policy=self.control_policy
         )
         self._input_queues, self._output_queues = prodsys.adapters.get_default_queues_for_resource(resource, self.queue_size)
         resource.input_queues = [q.ID for q in self._input_queues]
         resource.output_queues = [q.ID for q in self._output_queues]
         return resource   
 
 
 @dataclass
 class TransportResource(Resource, core.ExpressObject):
     """
     Class that represents a transport resource.
 
     Args:
         processes (List[process.TransportProcess]): Processes of the resource.
-        location (conlist(float, min_items=2, max_items=2)): Location of the resource.
+        location (conlist(float, min_length=2, max_length=2)): Location of the resource.
         capacity (int): Capacity of the resource. Defaults to 1.
         states (Optional[List[state.STATE_UNION]], optional): States of the resource. Defaults to None.
         controller (resource_data.ControllerEnum, optional): Controller of the resource. Defaults to resource_data.ControllerEnum.TransportController.
         control_policy (resource_data.TransportControlPolicy, optional): Control policy of the resource. Defaults to resource_data.TransportControlPolicy.FIFO.
         ID (str): ID of the resource.
 
     Examples:
@@ -142,22 +143,22 @@
         psx.TransportResource(
             processes=[transport_process],
             location=[10.0, 10.0]
         )
         ```
     """
     processes: List[process.TransportProcess]
-    location: conlist(float, min_items=2, max_items=2) = Field(default_factory=list) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) = Field(default_factory=list) # type: ignore
     # capacity: int = 1
     # states: Optional[List[state.STATE_UNION]] = Field(default_factory=list)
     controller: resource_data.ControllerEnum = resource_data.ControllerEnum.TransportController
     control_policy: resource_data.TransportControlPolicy = resource_data.TransportControlPolicy.FIFO
     # ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
-    def __post_init_post_parse__(self):
+    def __post_init__(self):
         if not self.location:
             self.location = [0.0, 0.0]
 
     def to_model(self) -> resource_data.TransportResourceData:
         """
         Converts the `prodsys.express` object to a data object from `prodsys.models`.
 
@@ -169,8 +170,10 @@
             description="",
             process_ids=[process.ID for process in self.processes],
             location=self.location,
             capacity=self.capacity,
             state_ids=[state.ID for state in self.states],
             controller=self.controller,
             control_policy=self.control_policy,
-        )
+        )
+
+from prodsys.express import state, process
```

### Comparing `prodsys-0.6.5/prodsys/express/sink.py` & `prodsys-0.7.0/prodsys/express/sink.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+from __future__ import annotations
+
 from typing import List, Optional
 from uuid import uuid1
 
 
 from pydantic import Field, conlist
 from pydantic.dataclasses import dataclass
 
+from prodsys.express import core
+
 from prodsys.models import sink_data, queue_data
 import prodsys
 
-from prodsys.express import core, product
 
 @dataclass
 class Sink(core.ExpressObject):
     """
     Class that represents a sink.
 
     Args:
         product (product.Product): Product of the sink.
-        location (conlist(float, min_items=2, max_items=2)): Location of the sink.
+        location (conlist(float, min_length=2, max_length=2)): Location of the sink.
         ID (str): ID of the sink.
     
     Attributes:
         _input_queues (List[queue_data.QueueData]): Input queues of the sink.
     
     Examples:
         Creation of a sink with a product and a location:
@@ -52,15 +55,15 @@
         psx.Sink(
             product=product,
             location=[0.0, 0.0],
         )
         ```
     """
     product: product.Product
-    location: conlist(float, min_items=2, max_items=2) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) # type: ignore
     ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
     _input_queues: List[queue_data.QueueData] = Field(default_factory=list, init=False)
 
     def to_model(self) -> sink_data.SinkData:
         """
         Converts the `prodsys.express` object to a data object from `prodsys.models`.
@@ -73,7 +76,9 @@
             description="",
             location=self.location,
             product_type=self.product.ID,
         )
         self._input_queues = [prodsys.adapters.get_default_queue_for_sink(sink)]
         sink.input_queues = [q.ID for q in self._input_queues]
         return sink
+    
+from prodsys.express import product
```

### Comparing `prodsys-0.6.5/prodsys/express/source.py` & `prodsys-0.7.0/prodsys/express/source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+from __future__ import annotations
+
 from typing import List, Optional
 from uuid import uuid1
 
 
 from pydantic import Field, conlist
 from pydantic.dataclasses import dataclass
 
+from prodsys.express import core, time_model
+
 from prodsys.models import source_data, queue_data
 import prodsys
 
-from prodsys.express import core, product, time_model
-
 @dataclass
 class Source(core.ExpressObject):
     """
     Class that represents a source.
 
     Args:
         product (product.Product): Product of the source.
         time_model (time_model.TIME_MODEL_UNION): Time model of the source that determines the inter-arrival time of products.
-        location (conlist(float, min_items=2, max_items=2)): Location of the source.
+        location (conlist(float, min_length=2, max_length=2)): Location of the source.
         routing_heuristic (source_data.RoutingHeuristic, optional): Routing heuristic of the source. Defaults to source_data.RoutingHeuristic.random.
         ID (str): ID of the source.
     
     Attributes:
         _output_queues (List[queue_data.QueueData]): Output queues of the source.
 
     Examples:
@@ -60,24 +62,20 @@
             time_model=arrival_time_model,
             location=[0.0, 0.0],
         )
         ```
     """
     product: product.Product
     time_model: time_model.TIME_MODEL_UNION
-    location: conlist(float, min_items=2, max_items=2) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) # type: ignore
     routing_heuristic: source_data.RoutingHeuristic = source_data.RoutingHeuristic.random
     ID: Optional[str] = Field(default_factory=lambda: str(uuid1()))
 
     _output_queues: List[queue_data.QueueData] = Field(default_factory=list, init=False)
 
-
-    def __post_init_post_parse__(self):
-        pass
-
     def to_model(self) -> source_data.SourceData:
         """
         Converts the `prodsys.express` object to a data object from `prodsys.models`.
 
         Returns:
             source_data.SourceData: An instance of the data object.
         """
@@ -88,7 +86,9 @@
             product_type=self.product.ID,
             time_model_id=self.time_model.ID,
             routing_heuristic=self.routing_heuristic,
         )
         self._output_queues = [prodsys.adapters.get_default_queue_for_source(source)]
         source.output_queues = [q.ID for q in self._output_queues]
         return source
+
+from prodsys.express import product
```

### Comparing `prodsys-0.6.5/prodsys/express/state.py` & `prodsys-0.7.0/prodsys/express/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 The following states are possible:
 
 - `Breakdown`: A state that makes a resource unavailable for a certain time.
 - `ProcessBreakdown`: A state that makes a process unavailable for a certain time but other processes can still be performed.
 - `Setup`: A state that represents the time needed to change the process of a resource.	    
 
 """
+from __future__ import annotations
+
 from typing import List, Optional, Union
 from uuid import uuid1
 
 from abc import ABC
 
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
+from prodsys.express import core, time_model
+
 from prodsys.models import state_data
 
-from prodsys.express import time_model, core, process
 
 
 @dataclass
 class State(ABC):
     """
     Abstract base class to represents a state.
 
@@ -208,8 +211,9 @@
             description="",
             time_model_id=self.time_model.ID,
             type=self.type,
             origin_setup=self.origin_setup.ID,
             target_setup=self.target_setup.ID
         )
     
-STATE_UNION = Union[BreakDownState, ProcessBreakdownState, SetupState]
+STATE_UNION = Union[BreakDownState, ProcessBreakdownState, SetupState]
+from prodsys.express import process
```

### Comparing `prodsys-0.6.5/prodsys/express/time_model.py` & `prodsys-0.7.0/prodsys/express/time_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 of products, performance of processes and the duration of states.
 
 The following time models are possible:
 - `SequentialTimeModel`: A time model that is based on a sequence of values.
 - `FunctionTimeModel`: A time model that is based on a distribution function which gets sampled.
 - `ManhattanDistanceTimeModel`: A time model that is based on the manhattan distance between two nodes and a constant velocity.
 """
-from __future__ import annotations
-
 from typing import List, Literal, Optional, Union
 from typing_extensions import deprecated
 from uuid import uuid1
 
 from pydantic.dataclasses import dataclass
 from pydantic import Field
 
-from prodsys.models import time_model_data
 from prodsys.express import core
 
+from prodsys.models import time_model_data
+
 @deprecated(
     "The SequentialTimeModel is deprecated and will be removed in the next version. Please use the SampleTimeModel instead.",
     category=None
 )
 @dataclass
 class SequentialTimeModel(core.ExpressObject):
     """
```

### Comparing `prodsys-0.6.5/prodsys/factories/__init__.py` & `prodsys-0.7.0/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/factories/link_transport_process_updater.py` & `prodsys-0.7.0/prodsys/factories/link_transport_process_updater.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING, Union
 
-from pydantic import BaseModel
 
 from prodsys.factories import process_factory, source_factory, sink_factory, resource_factory, node_factory
 from prodsys.simulation import process
 
 if TYPE_CHECKING:
     from prodsys.simulation import resources, sink, source, node
 
 
-class LinkTransportProcessUpdater(BaseModel):
+class LinkTransportProcessUpdater:
     """
     Updater class that updates the links of `prodsys.simulation` LinkTransportProcess objects in the process factory based on the created node, resource, source and sink objects.
 
     Args:
         process_factory (process_factory.ProcessFactory): Factory that contains alll process objects.
         source_factory (source_factory.SourceFactory): Factory that contains all source objects.
         sink_factory (sink_factory.SinkFactory): Factory that contains all sink objects.
         resource_factory (resource_factory.ResourceFactory): Factory that contains all resource objects.
         node_factory (node_factory.NodeFactory): Factory that contains all node objects.
     """
-    process_factory: process_factory.ProcessFactory
-    source_factory: source_factory.SourceFactory
-    sink_factory: sink_factory.SinkFactory
-    resource_factory: resource_factory.ResourceFactory
-    node_factory: node_factory.NodeFactory
+    def __init__(self, process_factory: process_factory.ProcessFactory, source_factory: source_factory.SourceFactory, sink_factory: sink_factory.SinkFactory, resource_factory: resource_factory.ResourceFactory, node_factory: node_factory.NodeFactory):
+        self.process_factory = process_factory
+        self.source_factory = source_factory
+        self.sink_factory = sink_factory
+        self.resource_factory = resource_factory
+        self.node_factory = node_factory
 
     def update_links_with_objects(self):
         """
         The method updates the links of the LinkTransportProcess objects in the process factory with the created node, resource, source and sink objects from the respective factories.
         """
         for process_instance in self.process_factory.processes:
             if isinstance(process_instance, process.LinkTransportProcess):
```

### Comparing `prodsys-0.6.5/prodsys/factories/node_factory.py` & `prodsys-0.7.0/prodsys/factories/node_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from __future__ import annotations
 
 from typing import List, TYPE_CHECKING
 
-from pydantic import BaseModel, parse_obj_as
+from pydantic import BaseModel, ConfigDict, TypeAdapter
 
-from prodsys.simulation import sim
 
 from prodsys.models.node_data import NodeData
 from prodsys.simulation import node
 
 if TYPE_CHECKING:
     from prodsys.adapters import adapter
+    from prodsys.simulation import sim
 
-class NodeFactory(BaseModel):
+class NodeFactory:
     """
     Factory class that creates and stores `prodsys.simulation` resource objects from `prodsys.models` node objects.
 
     Args:
         env (sim.Environment): prodsys simulation environment.
     """
-    env: sim.Environment
-    nodes: List[node.Node] = []
-    
 
-    class Config:
-        arbitrary_types_allowed = True
+    def __init__(self, env: sim.Environment):
+        self.env = env
+        self.nodes = []
 
     def create_nodes(self, adapter: adapter.ProductionSystemAdapter):
         """
         Creates node objects based on the given adapter.
 
         Args:
             adapter (adapter.ProductionSystemAdapter): Adapter that contains the node data.
@@ -41,15 +39,15 @@
         Creates a node object based on the given node data.
 
         Args:
             node_data (NodeData): Node data that is used to create the node object.
         """
         values = {}
         values.update({"data": node_data})
-        self.nodes.append(parse_obj_as(node.Node, values))
+        self.nodes.append(TypeAdapter(node.Node).validate_python(values))
 
     def get_node(self, ID: str) -> node.Node:
         """
         Method returns a node object with the given ID.
 
         Args:
             ID (str): ID of the node object.
```

### Comparing `prodsys-0.6.5/prodsys/factories/process_factory.py` & `prodsys-0.7.0/prodsys/factories/process_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import List, Optional, TYPE_CHECKING
 
-from pydantic import BaseModel, parse_obj_as
+from pydantic import BaseModel, TypeAdapter
 
 from prodsys.factories import time_model_factory
 from prodsys.models import processes_data
 
 if TYPE_CHECKING:
     from prodsys.adapters import adapter
     from prodsys.simulation import process
@@ -34,23 +34,25 @@
             self.add_processes(process_data, adapter)
 
     def add_processes(self, process_data: processes_data.PROCESS_DATA_UNION, adapter: adapter.ProductionSystemAdapter):
         values = {}
         if not (isinstance(process_data, processes_data.CompoundProcessData) or isinstance(process_data, processes_data.RequiredCapabilityProcessData)):
             time_model = self.time_model_factory.get_time_model(process_data.time_model_id)
             values.update({"time_model": time_model})
+        else:
+            values.update({"time_model": None})
         values.update({"process_data": process_data})
         if isinstance(process_data, processes_data.CompoundProcessData):
             contained_processes_data = [other_process_data for other_process_data in adapter.process_data if other_process_data.ID in process_data.process_ids]
             values.update({"contained_processes_data": contained_processes_data})
         if isinstance(process_data, processes_data.LinkTransportProcessData):
             values.update({"links": [[]]})
-            self.processes.append(parse_obj_as(process.LinkTransportProcess, values))
+            self.processes.append(TypeAdapter(process.LinkTransportProcess).validate_python(values))
         else:
-            self.processes.append(parse_obj_as(process.PROCESS_UNION, values))
+            self.processes.append(TypeAdapter(process.PROCESS_UNION).validate_python(values))
 
     def get_processes_in_order(self, IDs: List[str]) -> List[process.PROCESS_UNION]:
         """
         Returns a list of process objects in the order of the given IDs.
 
         Args:
             IDs (List[str]): List of IDs that is used to sort the process objects.
@@ -81,9 +83,8 @@
         """
         pr = [pr for pr in self.processes if pr.process_data.ID in ID]
         if not pr:
             raise ValueError(f"Process with ID {ID} not found")
         return pr.pop()
 
 
-from prodsys.simulation import process
-ProcessFactory.update_forward_refs()
+from prodsys.simulation import process
```

### Comparing `prodsys-0.6.5/prodsys/factories/product_factory.py` & `prodsys-0.7.0/prodsys/factories/product_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 from __future__ import annotations
 
-from typing import List, Dict
+from typing import TYPE_CHECKING, List, Dict
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 
-from prodsys.simulation import router, sim
-from prodsys.models import product_data
-from prodsys.factories import process_factory
-from prodsys.simulation import logger, proces_models, process
+from prodsys.models.product_data import ProductData
+from prodsys.simulation import proces_models
+from prodsys.simulation import process
 
+if TYPE_CHECKING:
+    from prodsys.factories import process_factory
+    from prodsys.simulation import sim, router, product
 
-class ProductFactory(BaseModel):
+
+
+class ProductFactory:
     """
     Factory class that creates and stores `prodsys.simulation` product objects from `prodsys.models` product objects.
 
     Args:
         env (sim.Environment): prodsys simulation environment.
         process_factory (process_factory.ProcessFactory): Factory that creates process objects.
     """
 
-    env: sim.Environment
-    process_factory: process_factory.ProcessFactory
-    products: List[product.Product] = []
-    finished_products: List[product.Product] = []
-    event_logger: logger.EventLogger = Field(default=False, init=False)
-    product_counter = 0
-
-    class Config:
-        arbitrary_types_allowed = True
+    def __init__(
+        self, env: sim.Environment, process_factory: process_factory.ProcessFactory
+    ):
+        self.env = env
+        self.process_factory = process_factory
+        self.products = []
+        self.finished_products = []
+        self.event_logger = False
+        self.product_counter = 0
 
     def create_product(
-        self, product_data: product_data.ProductData, router: router.Router
+        self, product_data: ProductData, router: router.Router
     ) -> product.Product:
         """
         Creates a product object based on the given product data and router.
 
         Args:
-            product_data (product_data.ProductData): Product data that is used to create the product object.
+            product_data (ProductData): Product data that is used to create the product object.
             router (router.Router): Router that is used to route the product object.
 
         Raises:
             ValueError: If the transport process is not found.
 
         Returns:
             product.Product: Created product object.
         """
-        product_data = product_data.copy()
+        product_data = product_data.model_copy()
         product_data.ID = (
             str(product_data.product_type) + "_" + str(self.product_counter)
         )
         process_model = self.create_process_model(product_data)
         transport_processes = self.process_factory.get_process(
             product_data.transport_process
         )
@@ -91,21 +95,21 @@
                 self.process_factory.get_process(predecessor_id)
                 for predecessor_id in predecessor_ids
             ]
             precedence_graph.add_node(process, successors, predecessors)
         return precedence_graph
 
     def create_process_model(
-        self, product_data: product_data.ProductData
+        self, product_data: ProductData
     ) -> proces_models.ProcessModel:
         """
         Creates a process model based on the given product data.
 
         Args:
-            product_data (product_data.ProductData): Product data that is used to create the process model.
+            product_data (ProductData): Product data that is used to create the process model.
 
         Raises:
             ValueError: If the process model is not recognized.
 
         Returns:
             proces_models.ProcessModel: Created process model.
         """
@@ -161,11 +165,8 @@
 
         Args:
             product (product.Product): Product object that is registered as a finished product object.
         """
         self.finished_products.append(product)
         self.remove_product(product)
 
-
 from prodsys.simulation import product
-
-product.Product.update_forward_refs()
```

### Comparing `prodsys-0.6.5/prodsys/factories/queue_factory.py` & `prodsys-0.7.0/prodsys/factories/queue_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import List, TYPE_CHECKING
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from prodsys.simulation import sim, store
 
 if TYPE_CHECKING:
     from prodsys.adapters import adapter
     from prodsys.models import queue_data
 
@@ -21,16 +21,15 @@
     Returns:
         _type_: _description_
     """
     env: sim.Environment
 
     queues: List[store.Queue] = []
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def create_queues(self, adapter: adapter.ProductionSystemAdapter):
         """
         Creates queue objects based on the given adapter.
 
         Args:
             adapter (adapter.ProductionSystemAdapter): _description_
```

### Comparing `prodsys-0.6.5/prodsys/factories/resource_factory.py` & `prodsys-0.7.0/prodsys/factories/resource_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import copy
 from typing import Dict, List, Optional, Union, Tuple, TYPE_CHECKING
 
-from pydantic import BaseModel, parse_obj_as
+from pydantic import BaseModel, ConfigDict, TypeAdapter
 
 from prodsys.simulation import sim
 from prodsys.simulation import process, state
 from prodsys.util.util import get_class_from_str
 
 
 from prodsys.models.resource_data import (
@@ -15,14 +15,15 @@
     ProductionResourceData,
     ControllerEnum,
     ResourceControlPolicy, TransportControlPolicy
 )
 from prodsys.factories import process_factory, state_factory, queue_factory
 
 from prodsys.simulation import control, resources
+from prodsys.simulation.resources import RESOURCE_UNION
 
 if TYPE_CHECKING:
     from prodsys.simulation import store
     from prodsys.adapters import adapter
 
 
 CONTROLLER_DICT: Dict = {
@@ -112,31 +113,30 @@
     """
     env: sim.Environment
     process_factory: process_factory.ProcessFactory
     state_factory: state_factory.StateFactory
     queue_factory: queue_factory.QueueFactory
 
     resource_data: List[RESOURCE_DATA_UNION] = []
-    resources: List[resources.RESOURCE_UNION] = []
+    resources: List[RESOURCE_UNION] = []
     controllers: List[
         Union[control.ProductionController, control.TransportController]
     ] = []
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def create_resources(self, adapter: adapter.ProductionSystemAdapter):
         """
         Creates resource objects based on the given adapter.
 
         Args:
             adapter (adapter.ProductionSystemAdapter): Adapter that contains the resource data.
         """
         for resource_data in adapter.resource_data:
-            self.add_resource(resource_data.copy(deep=True))
+            self.add_resource(resource_data.model_copy(deep=True))
 
     def get_queues_for_resource(
         self, resource_data: ProductionResourceData
     ) -> Tuple[List[store.Queue], List[store.Queue]]:
         input_queues = []
         output_queues = []
         if resource_data.input_queues:
@@ -169,15 +169,15 @@
         values.update({"controller": controller})
 
         if isinstance(resource_data, ProductionResourceData):
             input_queues, output_queues = self.get_queues_for_resource(resource_data)
             values.update(
                 {"input_queues": input_queues, "output_queues": output_queues}
             )
-        resource_object = parse_obj_as(resources.RESOURCE_UNION, values)
+        resource_object = TypeAdapter(RESOURCE_UNION).validate_python(values)
         # print(resource_object._env)
         controller.set_resource(resource_object)
 
         states = self.state_factory.get_states(resource_data.state_ids)
         register_states(resource_object, states, self.env)
         register_production_states_for_processes(
             resource_object, self.state_factory, self.env
@@ -191,15 +191,15 @@
         """
         for _resource in self.resources:
             _resource.start_states()
 
         for controller in self.controllers:
             self.env.process(controller.control_loop())  # type: ignore
 
-    def get_resource(self, ID: str) -> resources.RESOURCE_UNION:
+    def get_resource(self, ID: str) -> RESOURCE_UNION:
         """
         Method returns a resource object with the given ID.
 
         Args:
             ID (str): ID of the resource object.
 
         Returns:
```

### Comparing `prodsys-0.6.5/prodsys/factories/sink_factory.py` & `prodsys-0.7.0/prodsys/factories/sink_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, Any, TYPE_CHECKING
 
-from pydantic import BaseModel, Field, parse_obj_as
+from pydantic import BaseModel, ConfigDict, Field, TypeAdapter
 
 from prodsys.simulation import sim, sink
 from prodsys.models import sink_data
 if TYPE_CHECKING:
     from prodsys.factories import product_factory, queue_factory
     from prodsys.adapters import adapter
 
@@ -23,16 +23,15 @@
     """
     env: sim.Environment
     product_factory: product_factory.ProductFactory
     queue_factory: queue_factory.QueueFactory
 
     sinks: List[sink.Sink] = Field(default_factory=list, init=False)
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def create_sinks(self, adapter: adapter.ProductionSystemAdapter):
         """
         Creates sink objects based on the given adapter.
 
         Args:
             adapter (adapter.ProductionSystemAdapter): Adapter that contains the sink data.
@@ -42,15 +41,15 @@
 
     def add_sink(self, sink_data: sink_data.SinkData):
         values = {
             "env": self.env,
             "data": sink_data,
             "product_factory": self.product_factory,
         }
-        sink_object = parse_obj_as(sink.Sink, values)
+        sink_object = TypeAdapter(sink.Sink).validate_python(values)
         self.add_queues_to_sink(sink_object)
         self.sinks.append(sink_object)
 
     def add_queues_to_sink(self, _sink: sink.Sink):
         input_queues = self.queue_factory.get_queues(_sink.data.input_queues)
         _sink.add_input_queues(input_queues)
 
@@ -85,9 +84,8 @@
             __product_type (str): Product type that is used to sort the sink objects.
 
         Returns:
             List[sink.Sink]: List of sink objects with the given product type.
         """
         return [s for s in self.sinks if __product_type == s.data.product_type]
 
-from prodsys.factories import product_factory, queue_factory   
-SinkFactory.update_forward_refs()
+from prodsys.factories import product_factory, queue_factory
```

### Comparing `prodsys-0.6.5/prodsys/factories/source_factory.py` & `prodsys-0.7.0/prodsys/factories/source_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, TYPE_CHECKING
 
-from pydantic import BaseModel, parse_obj_as, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 
 from prodsys.simulation import router, sim, source
-from prodsys.models import source_data, product_data
+from prodsys.models.product_data import ProductData
+from prodsys.models.source_data import SourceData
 
 
 if TYPE_CHECKING:
     from prodsys.factories import (
         resource_factory,
         queue_factory,
         time_model_factory,
         sink_factory,
     )
     from prodsys.adapters import adapter
 
 
 class SourceFactory(BaseModel):
     """
-    Factory class that creates and stores `prodsys.simulation` source objects based on the given source data according to `prodsys.models.source_data.SourceData`.
+    Factory class that creates and stores `prodsys.simulation` source objects based on the given source data according to `prodsys.models.SourceData`.
 
     Args:
         env (sim.Environment): prodsys simulation environment.
         product_factory (product_factory.ProductFactory): Factory that creates product objects.
         time_model_factory (time_model_factory.TimeModelFactory): Factory that creates time model objects.
         queue_factory (queue_factory.QueueFactory): Factory that creates queue objects.
         resource_factory (resource_factory.ResourceFactory): Factory that creates resource objects.
@@ -35,21 +36,20 @@
     env: sim.Environment
     product_factory: product_factory.ProductFactory
     time_model_factory: time_model_factory.TimeModelFactory
     queue_factory: queue_factory.QueueFactory
     resource_factory: resource_factory.ResourceFactory
     sink_factory: sink_factory.SinkFactory
 
-    product_data: List[product_data.ProductData] = Field(
+    product_data: List[ProductData] = Field(
         default_factory=list, init=False
     )
     sources: List[source.Source] = Field(default_factory=list, init=False)
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def create_sources(self, adapter: adapter.ProductionSystemAdapter):
         """
         Creates source objects based on the given adapter.
 
         Args:
             adapter (adapter.ProductionSystemAdapter): Adapter that contains the source data.
@@ -64,16 +64,16 @@
             self.resource_factory,
             self.sink_factory,
             router.ROUTING_HEURISTIC[routing_heuristic],
         )
 
     def add_source(
         self,
-        source_data: source_data.SourceData,
-        product_data_of_source: product_data.ProductData,
+        source_data: SourceData,
+        product_data_of_source: ProductData,
     ):
         router = self.get_router(source_data.routing_heuristic)
 
         time_model = self.time_model_factory.get_time_model(source_data.time_model_id)
 
         source_object = source.Source(
             env=self.env,
@@ -137,9 +137,7 @@
 from prodsys.factories import (
     product_factory,
     resource_factory,
     queue_factory,
     time_model_factory,
     sink_factory,
 )
-
-SourceFactory.update_forward_refs()
```

### Comparing `prodsys-0.6.5/prodsys/factories/state_factory.py` & `prodsys-0.7.0/prodsys/factories/state_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 from __future__ import annotations
 
 from dataclasses import field
 from typing import List, TYPE_CHECKING
 
-from pydantic import parse_obj_as, BaseModel
+from pydantic import ConfigDict, BaseModel, TypeAdapter
 
 from prodsys.simulation import sim
 from prodsys.factories import time_model_factory
 from prodsys.models import state_data
 from prodsys.simulation import state
 
 
 if TYPE_CHECKING:
     from prodsys.adapters import adapter
 
 
-class StateFactory(BaseModel):
+class StateFactory:
     """
     Factory class that creates and stores `prodsys.simulation` state objects from `prodsys.models` state objects.
 
     Args:
         env (sim.Environment): prodsys simulation environment.
         time_model_factory (time_model_factory.TimeModelFactory): Factory that creates time model objects.
     """
-    env: sim.Environment
-    time_model_factory: time_model_factory.TimeModelFactory
 
-    state_data: List[state_data.STATE_DATA_UNION] = []
-    states: List[state.STATE_UNION] = []
-
-    class Config:
-        arbitrary_types_allowed = True
+    def __init__(self, env: sim.Environment, time_model_factory: time_model_factory.TimeModelFactory):
+        self.env = env
+        self.time_model_factory = time_model_factory
+        self.state_data: List[state_data.STATE_DATA_UNION] = []
+        self.states: List[state.STATE_UNION] = []
 
     def create_states_from_configuration_data(self, configuration_data: dict):
         for cls_name, items in configuration_data.items():
             for values in items.values():
                 values.update({"type": cls_name})
                 self.state_data.append(
-                    parse_obj_as(state_data.STATE_DATA_UNION, values)
+                    TypeAdapter(state_data.STATE_DATA_UNION).validate_python(values)
                 )
                 self.add_state(self.state_data[-1])
 
     def add_state(self, state_data: state_data.STATE_DATA_UNION):
         values = {}
         values.update({"state_data": state_data})
         time_model = self.time_model_factory.get_time_model(
             values["state_data"].time_model_id
         )
         values.update({"time_model": time_model, "env": self.env})
-        if "repair_time_model_id" in state_data.dict():
+        if "repair_time_model_id" in state_data.model_dump():
             repair_time_model = self.time_model_factory.get_time_model(
                 state_data.repair_time_model_id
             )
             values.update({"repair_time_model": repair_time_model})
-        self.states.append(parse_obj_as(state.STATE_UNION, values))
+        # FIXME: resolve bug when importing simulation types
+        self.states.append(TypeAdapter(state.STATE_UNION).validate_python(values))
 
     def create_states(self, adapter: adapter.ProductionSystemAdapter):
         """
         Creates state objects based on the given adapter.
 
         Args:
             adapter (adapter.ProductionSystemAdapter): Adapter that contains the state data.
```

### Comparing `prodsys-0.6.5/prodsys/factories/time_model_factory.py` & `prodsys-0.7.0/prodsys/factories/time_model_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 from __future__ import annotations
 
 from typing import List, TYPE_CHECKING
 
-from pydantic import BaseModel, parse_obj_as
-
-from prodsys.models import time_model_data
-from prodsys.simulation import time_model
+from pydantic import BaseModel, TypeAdapter
+from prodsys.models.time_model_data import TIME_MODEL_DATA
+from prodsys.simulation.time_model import TIME_MODEL, TimeModel
 
 if TYPE_CHECKING:
     from prodsys.adapters import adapter
 
 class TimeModelFactory(BaseModel):
     """
     Factory class that creates and stores `prodsys.simulation` time model objects based on the given time model data according to `prodsys.models.time_model_data.TIME_MODEL_DATA`.
 
     Returns:
         _type_: _description_
     """
-    time_model_data: List[time_model_data.TIME_MODEL_DATA] = []
-    time_models: List[time_model.TIME_MODEL] = []
+    time_model_data: List[TIME_MODEL_DATA] = []
+    time_models: List[TIME_MODEL] = []
 
     def create_time_models(self, adapter: adapter.ProductionSystemAdapter):
         """
         Creates time model objects based on the given adapter.
 
         Args:
             adapter (adapter.ProductionSystemAdapter): Adapter that contains the time model data.
         """
         for time_model_data in adapter.time_model_data:
-            self.time_models.append(
-                parse_obj_as(time_model.TIME_MODEL, {"time_model_data": time_model_data})
+            self.time_models.append(TypeAdapter(TIME_MODEL).validate_python({"time_model_data": time_model_data})
             )
 
-    def get_time_models(self, IDs: List[str]) -> List[time_model.TimeModel]:
+    def get_time_models(self, IDs: List[str]) -> List[TimeModel]:
         """
         Returns a list of time model objects with the given IDs.
 
         Args:
             IDs (List[str]): List of IDs that is used to filter the time model objects.
 
         Returns:
             List[time_model.TimeModel]: List of time model objects with the given IDs.
         """
         return [tm for tm in self.time_models if tm.time_model_data.ID in IDs]
 
-    def get_time_model(self, ID: str) -> time_model.TimeModel:
+    def get_time_model(self, ID: str) -> TimeModel:
         """
         Returns a time model object with the given ID.
 
         Args:
             ID (str): ID that is used to filter the time model objects.
 
         Returns:
```

### Comparing `prodsys-0.6.5/prodsys/models/__init__.py` & `prodsys-0.7.0/prodsys/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/models/node_data.py` & `prodsys-0.7.0/prodsys/models/node_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 """
 NodeData objects are used in prodsys to represent Locations in the production system that serve as nodes in a link. They are used in the 
 `LinkTransportProcess` class to represent locations where routes can cross.
 """
-
-from __future__ import annotations
-
 from hashlib import md5
 from typing import List
 
-from pydantic import conlist
+from pydantic import ConfigDict, conlist
 
 from prodsys.models.core_asset import CoreAsset
 
 class NodeData(CoreAsset):
     """
     Represents a node data object of a link.
 
     Attributes:
             location (List[float]): Location of the node. It has to be a list of length 2.
     """
 
-    location: conlist(float, min_items=2, max_items=2) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) # type: ignore
 
     def hash(self) -> str:
         """
         Hashes the node data object.
 
         Returns:
             str: Hash of the node data object.
         """
         return md5("".join([*map(str, self.location)]).encode("utf-8")).hexdigest()
-
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Node",
-                "value": {
-                    "ID": "N1",
-                    "description": "Node 1",
-                    "location": [0.0, 0.0],
-                },
+    
+    model_config = ConfigDict(json_schema_extra= {
+        "examples": [
+            {
+                "ID": "N1",
+                "description": "Node 1",
+                "location": [0.0, 0.0],
             }
-        }
+        ]
+    })
```

### Comparing `prodsys-0.6.5/prodsys/models/performance_data.py` & `prodsys-0.7.0/prodsys/models/performance_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from __future__ import annotations
-
 from enum import Enum
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from typing import Literal, Union, Optional, List, Tuple, TYPE_CHECKING
 
 from prodsys.models.performance_indicators import (
     KPIEnum,
     KPILevelEnum,
     KPI_UNION,
 )
 
-if TYPE_CHECKING:
-    from prodsys.simulation import state
-
 
 class Event(BaseModel):
     """
     Class that represents an event in the event log.
 
     Args:
         time (float): Time of the event.
@@ -34,75 +29,74 @@
     state: str
     state_type: str
     activity: str
     product: Optional[str] = None
     expected_end_time: Optional[float] = None
     target_location: Optional[str] = None
 
-    class Config:
-        schema_extra = {
-            "examples": [
-                {
-                    "time": 12.0,
-                    "resource": "R1",
-                    "state": "P1",
-                    "state_type": "Production",
-                    "activity": "start state",
-                    "product": "Product_1_12",
-                    "expected_end_time": 24.3,
-                    "target_location": None,
-                }, 
-                {
-                    "time": 24.3,
-                    "resource": "R1",
-                    "state": "P1",
-                    "state_type": "Production",
-                    "activity": "end state",
-                    "product": "Product_1_12",
-                    "expected_end_time": None,
-                    "target_location": "L1",
-                },
-            ]
-        }
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "time": 12.0,
+                "resource": "R1",
+                "state": "P1",
+                "state_type": "Production",
+                "activity": "start state",
+                "product": "Product_1_12",
+                "expected_end_time": 24.3,
+                "target_location": None,
+            }, 
+            {
+                "time": 24.3,
+                "resource": "R1",
+                "state": "P1",
+                "state_type": "Production",
+                "activity": "end state",
+                "product": "Product_1_12",
+                "expected_end_time": None,
+                "target_location": "L1",
+            },
+        ]
+    })
 
 
 class Performance(BaseModel):
     """
     Class that represents the performance of a simulation run.
 
     Args:
         event_log (List[Event]): Event log of the simulation run.
         kpis (List[KPI_UNION]): List of KPIs of the simulation run.
     """
 
-    class Config:
-        schema_extra = {
-            "examples": [{               
-                    "event_log": Event.Config.schema_extra["examples"],
-                    "kpis": [
-                        {
-                            "name": "throughput",
-                            "target": "max",
-                            "weight": 1,
-                            "value": 4.32,
-                            "context": ["system", "product_type"],
-                            "product_type": "ProductType_1",
-                        },
-                        {
-                            "name": "WIP",
-                            "target": "min",
-                            "weight": 1,
-                            "value": 121,
-                            "context": ["system", "product_type"],
-                            "product_type": "ProductType_1",
-                        },
-                    ],
-                }
-            ]
-        }
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "event_log": Event.model_config["json_schema_extra"]["examples"],
+                "kpis": [
+                    {
+                        "name": "throughput",
+                        "target": "max",
+                        "weight": 1,
+                        "value": 4.32,
+                        "context": ["system", "product_type"],
+                        "product_type": "ProductType_1",
+                    },
+                    {
+                        "name": "WIP",
+                        "target": "min",
+                        "weight": 1,
+                        "value": 121,
+                        "context": ["system", "product_type"],
+                        "product_type": "ProductType_1",
+                    },
+                ],
+            }
+        ]
+    })
 
     event_log: List[Event]
     kpis: List[KPI_UNION]
 
     def get_kpi_for_context(self, context: Tuple[KPILevelEnum, ...]) -> List[KPI_UNION]:
         return [kpi for kpi in self.kpis if context == kpi.context]
```

### Comparing `prodsys-0.6.5/prodsys/models/performance_indicators.py` & `prodsys-0.7.0/prodsys/models/performance_indicators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import annotations
-
 from enum import Enum
 from typing import Literal, List, Optional, Union, Tuple
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, ConfigDict, field_validator
 
 
 class KPIEnum(str, Enum):
     """
     Enum that represents the different kind of KPIs.
     """
 
@@ -59,15 +57,15 @@
     target: Literal["min", "max"]
     weight: Optional[float] = 1
     value: Optional[float] = None
     context: Optional[Tuple[KPILevelEnum, ...]] = None
     resource: Optional[str] = None
     product_type: Optional[str] = None
 
-    @validator("context")
+    @field_validator("context", mode="before")
     def sort_context(cls, v):
         return tuple(sorted(v))
 
 
 class DynamicKPI(KPI):
     """
     Class that represents a dynamic KPI. Not intended for usage but only inheritance.
@@ -79,251 +77,236 @@
     process: Optional[str] = None
 
 
 class Output(KPI):
     name: Literal[KPIEnum.OUTPUT] = KPIEnum.OUTPUT
     target: Literal["max"] = "max"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Output KPI",
-                "value": {
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
                     "name": "output",
                     "target": "max",
                     "weight": 1,
                     "value": 34,
                     "context": ["system", "product_type"],
                     "product_type": "ProductType_1",
-                },
-            }
+                }
+            ]
         }
+    )
 
 
 class Throughput(KPI):
     name: Literal[KPIEnum.THROUGHPUT]
     target: Literal["max"] = "max"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Throughput KPI",
-                "value": {
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
                     "name": "throughput",
                     "target": "max",
                     "weight": 1,
                     "value": 4.32,
                     "context": ["system", "product_type"],
                     "product_type": "ProductType_1",
-                },
-            }
+                }
+            ]
         }
-
+    )
 
 class Cost(KPI):
     name: Literal[KPIEnum.COST]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Cost KPI",
-                "value": {
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
                     "name": "cost",
                     "target": "min",
                     "weight": 0.5,
                     "value": 36000,
                     "context": ["system"],
-                },
-            }
+                }
+            ]
         }
+    )
 
 
 class WIP(KPI):
     name: Literal[KPIEnum.WIP]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "WIP KPI",
-                "value": {
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
                     "name": "WIP",
                     "target": "min",
                     "weight": 1,
                     "value": 121,
                     "context": ["system", "product_type"],
                     "product_type": "ProductType_1",
-                },
-            }
+                }
+            ]
         }
+    )
 
 
 class DynamicWIP(DynamicKPI, WIP):
     name: Literal[KPIEnum.DYNAMIC_WIP]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Dynamic WIP KPI",
-                "value": {
-                    "name": "dynamic_WIP",
-                    "target": "min",
-                    "weight": 1,
-                    "value": 121,
-                    "context": ["system", "product"],
-                    "product_type": "ProductType_1",
-                    "start_time": 21.2,
-                    "end_time": 23.4,
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "dynamic_WIP",
+                "target": "min",
+                "weight": 1,
+                "value": 121,
+                "context": ["system", "product"],
+                "product_type": "ProductType_1",
+                "start_time": 21.2,
+                "end_time": 23.4,
             }
-        }
+        ]
+    })
 
 
 class ThroughputTime(KPI):
     name: Literal[KPIEnum.TRHOUGHPUT_TIME]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Throughput time KPI",
-                "value": {
-                    "name": "throughput_time",
-                    "target": "min",
-                    "weight": 1,
-                    "value": 221.1,
-                    "context": ["system", "product_type"],
-                    "product_type": "ProductType_1",
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "throughput_time",
+                "target": "min",
+                "weight": 1,
+                "value": 221.1,
+                "context": ["system", "product_type"],
+                "product_type": "ProductType_1",
             }
-        }
+        ]
+    })
 
 
 class DynamicThroughputTime(DynamicKPI, ThroughputTime):
     name: Literal[KPIEnum.DYNAMIC_THROUGHPUT_TIME]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Dynamic throughput time KPI",
-                "value": {
-                    "name": "throughput_time",
-                    "target": "min",
-                    "weight": 1,
-                    "value": 201.3,
-                    "context": ["system", "product"],
-                    "product_type": "ProductType_1",
-                    "product": "Product_1_23",
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "dynamic_throughput_time",
+                "target": "min",
+                "weight": 1,
+                "value": 221.1,
+                "context": ["system", "product"],
+                "product_type": "ProductType_1",
+                "product": "Product_1_23",
+                "start_time": 21.2,
+                "end_time": 23.4,
             }
-        }
+        ]
+    })
 
 
 class ProcessingTime(KPI):
     name: Literal[KPIEnum.PROCESSING_TIME]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Processing time KPI",
-                "value": {
-                    "name": "processing_time",
-                    "target": "min",
-                    "weight": 1,
-                    "value": 1.2,
-                    "context": ["resource", "process"],
-                    "resource": "Resource_1",
-                    "process": "P1",
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "processing_time",
+                "target": "min",
+                "weight": 1,
+                "value": 1.2,
+                "context": ["resource", "process"],
+                "resource": "Resource_1",
+                "process": "P1",
             }
-        }
+        ]
+    })
 
 
 class ProductiveTime(KPI):
     name: Literal[KPIEnum.PRODUCTIVE_TIME]
     target: Literal["max"] = "max"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Productive time KPI",
-                "value": {
-                    "name": "productive_time",
-                    "target": "max",
-                    "weight": 1,
-                    "value": 0.65,
-                    "context": ["resource"],
-                    "resource": "Resource_1",
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "productive_time",
+                "target": "max",
+                "weight": 1,
+                "value": 0.65,
+                "context": ["resource"],
+                "resource": "Resource_1",
             }
-        }
+        ]
+    })
 
 
 class StandbyTime(KPI):
     name: Literal[KPIEnum.STANDBY_TIME]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Standby time KPI",
-                "value": {
-                    "name": "standby_time",
-                    "target": "min",
-                    "weight": 1,
-                    "value": 0.12,
-                    "context": ["resource"],
-                    "resource": "Resource_1",
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "standby_time",
+                "target": "min",
+                "weight": 1,
+                "value": 0.12,
+                "context": ["resource"],
+                "resource": "Resource_1",
             }
-        }
+        ]
+    })
 
 
 class SetupTime(KPI):
     name: Literal[KPIEnum.SETUP_TIME]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Setup time KPI",
-                "value": {
-                    "name": "setup_time",
-                    "target": "min",
-                    "weight": 1,
-                    "value": 0.08,
-                    "context": ["resource"],
-                    "resource": "Resource_1",
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "setup_time",
+                "target": "min",
+                "weight": 1,
+                "value": 0.08,
+                "context": ["resource"],
+                "resource": "Resource_1",
             }
-        }
+        ]
+    })
 
 
 class UnscheduledDowntime(KPI):
     name: Literal[KPIEnum.UNSCHEDULED_DOWNTIME]
     target: Literal["min"] = "min"
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Unscheduled downtime KPI",
-                "value": {
-                    "name": "unscheduled_downtime",
-                    "target": "min",
-                    "weight": 1,
-                    "value": 0.1,
-                    "context": ["resource"],
-                    "resource": "Resource_1",
-                },
+    model_config = ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": "unscheduled_downtime",
+                "target": "min",
+                "weight": 1,
+                "value": 0.1,
+                "context": ["resource"],
+                "resource": "Resource_1",
             }
-        }
+        ]
+    })
 
 
 KPI_UNION = Union[
     Output,
     Throughput,
     Cost,
     WIP,
```

### Comparing `prodsys-0.6.5/prodsys/models/processes_data.py` & `prodsys-0.7.0/prodsys/models/processes_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 """
 
 from __future__ import annotations
 from hashlib import md5
 from enum import Enum
 from typing import Literal, Union, Optional, List, TYPE_CHECKING
 
-from pydantic import Field
+from pydantic import ConfigDict, Field
 
 from prodsys.models.core_asset import CoreAsset
 
 if TYPE_CHECKING:
     from prodsys.adapters.adapter import ProductionSystemAdapter
 
-
 class ProcessTypeEnum(str, Enum):
     """
     Enum that represents the different kind of processes.
 
     - ProductionProcesses: A process that can be performed on a product by a production resource.
     - TransportProcesses: A process that can be performed on a product by a transport resource.
     - CapabilityProcesses: A process that can be performed on a product by a resource, based on the capability of the resource.
@@ -46,22 +45,23 @@
         ID (str): ID of the process.
         description (str): Description of the process.
         time_model_id (str): ID of the time model of the process.
     """
 
     time_model_id: str
 
-    class Config:
-        schema_extra = {
-            "example": {
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
                 "ID": "P1",
                 "description": "Process 1",
                 "time_model_id": "function_time_model_1",
             }
-        }
+        ]
+    })
     
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash for the process data considering the time model data. Can be used to compare two process data objects for equal functionality.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter to access the time model data.
@@ -101,26 +101,24 @@
             type="ProductionProcesses",
         )
         ```
     """
 
     type: Literal[ProcessTypeEnum.ProductionProcesses]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Production process",
-                "value": {
-                    "ID": "P1",
-                    "description": "Process 1",
-                    "time_model_id": "function_time_model_1",
-                    "type": "ProductionProcesses",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "P1",
+                "description": "Process 1",
+                "time_model_id": "function_time_model_1",
+                "type": "ProductionProcesses",
             }
-        }
+        ]
+    })
 
 
 class CapabilityProcessData(ProcessData):
     """
     Class that represents capability process data. Capability processes are not compared by their IDs but their Capabilities.
 
     Args:
@@ -143,27 +141,25 @@
         )
         ```
     """
 
     type: Literal[ProcessTypeEnum.CapabilityProcesses]
     capability: str
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Capability process",
-                "value": {
-                    "ID": "P1",
-                    "description": "Process 1",
-                    "time_model_id": "function_time_model_1",
-                    "type": "CapabilityProcesses",
-                    "capability": "C1",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "P1",
+                "description": "Process 1",
+                "time_model_id": "function_time_model_1",
+                "type": "CapabilityProcesses",
+                "capability": "C1",
             }
-        }
+        ]
+    })
 
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash for the capability process data considering the capability, time model and type of the process. Can be used to compare two process data objects for equal functionality.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter to access the time model data.
@@ -195,52 +191,48 @@
             type="TransportProcesses",
         )
         ```
     """
 
     type: Literal[ProcessTypeEnum.TransportProcesses]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Transport process",
-                "value": {
-                    "ID": "TP1",
-                    "description": "Transport Process 1",
-                    "time_model_id": "manhattan_time_model_1",
-                    "type": "TransportProcesses",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "TP1",
+                "description": "Transport Process 1",
+                "time_model_id": "manhattan_time_model_1",
+                "type": "TransportProcesses",
             }
-        }
+        ]
+    })
 
 
 class CompoundProcessData(CoreAsset):
     """
     Class that represents a compound process. A compound process is a container for multiple processes that belong together, e.g. if a hardware module enables all processes of a CompoundProcess or if multiple similar processes can be performed.
     
     Args:
         ID (str): ID of the process module.
         description (str): Description of the process module.
         process_ids (List[str]): Process IDs of the process module.
     """
     process_ids: List[str]
     type: Literal[ProcessTypeEnum.CompoundProcesses]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Compound Process",
-                "value": {
-                    "ID": "CP1",
-                    "description": "Compound Process 1",
-                    "process_ids": ["P1", "P2"],
-                    "type": "CompoundProcesses",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "CP1",
+                "description": "Compound Process 1",
+                "process_ids": ["P1", "P2"],
+                "type": "CompoundProcesses",
             }
-        }
+        ]
+    })
 
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash for the compound process data considering the proces ids. Can be used to compare two process data objects for equal functionality.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter to access the process data.
@@ -285,26 +277,24 @@
         )
         ```
     """
 
     type: Literal[ProcessTypeEnum.RequiredCapabilityProcesses]
     capability: str
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Required Capability process",
-                "value": {
-                    "ID": "P1",
-                    "description": "Process 1",
-                    "type": "RequiredCapabilityProcesses",
-                    "capability": "C1",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "P1",
+                "description": "Process 1",
+                "type": "RequiredCapabilityProcesses",
+                "capability": "C1",
             }
-        }
+        ]
+    })
 
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash for the required capability process data considering the capability and type of the process. Can be used to compare two process data objects for equal functionality.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter to access the time model data.
@@ -355,26 +345,24 @@
 
         Returns:
             str: hash of the required capability process data.
         """
         raise NotImplementedError("Hash function not implemented for LinkTransportProcessData")
         # TODO: Implement hash function for LinkTransportProcessData and Nodes
         # return md5("".join([*sorted(process_hashes)]).encode("utf-8")).hexdigest()
-        
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Transport process",
-                "value": {
-                    "ID": "TP1",
-                    "description": "Transport Process 1",
-                    "time_model_id": "manhattan_time_model_1",
-                    "type": "LinkTransportProcesses",
-                    "links": [["Resource1", "Node2"], ["Node2", "Resource1"]],
-                },
+
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "TP1",
+                "description": "Transport Process 1",
+                "time_model_id": "manhattan_time_model_1",
+                "type": "LinkTransportProcesses",
+                "links": [["Resource1", "Node2"], ["Node2", "Resource1"]]
             }
-        }
+        ]
+    })
 
 PROCESS_DATA_UNION = Union[
     CompoundProcessData, RequiredCapabilityProcessData,
     ProductionProcessData, TransportProcessData, CapabilityProcessData, LinkTransportProcessData
 ]
```

### Comparing `prodsys-0.6.5/prodsys/models/product_data.py` & `prodsys-0.7.0/prodsys/models/product_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 from hashlib import md5
 from typing import Union, List, Dict, TYPE_CHECKING
-from pydantic import root_validator
+from pydantic import ConfigDict, model_validator
 from prodsys.models.core_asset import CoreAsset
 
 if TYPE_CHECKING:
     from prodsys.adapters.adapter import ProductionSystemAdapter
 
-
 class ProductData(CoreAsset):
     """
     Class that represents product data, specifically the required processes and the allows tranport process.
 
     The processes describe thereby the process model that needs to be completed for the product to be finished. There are three different ways to describe the process model:
 
     - Sequential process model: The processes are given as a list of process IDs. The processes are executed sequentially.
@@ -111,50 +110,49 @@
                 transport_process_hash = transport_process.hash(adapter)
                 break
         else:
             raise ValueError(f"Transport process with ID {self.transport_process} not found for product {self.ID}.")
         
         return md5("".join([*processes_hashes, transport_process_hash]).encode("utf-8")).hexdigest()
                    
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def check_processes(cls, values):
         if "product_type" in values and values["product_type"]:
             values["ID"] = values["product_type"]
         else:
             values["product_type"] = values["ID"]
         return values
-
-    class Config:
-        schema_extra = {
-            "examples": [
-                {
-                    "ID": "Product_1",
-                    "description": "Product with sequential process",
-                    "product_type": "Product_1",
-                    "processes": ["P1", "P2", "P3"],
-                    "transport_process": "TP1",
-                },
-                {
-                    "ID": "Product_1",
-                    "description": "Process with adjacency matrix process",
-                    "product_type": "Product_1",
-                    "processes": {
-                        "P1": ["P2", "P3"],
-                        "P2": ["P3"],
-                        "P3": [],
-                    },
-                    "transport_process": "TP1",
-                },
-                {
-                    "ID": "Product_1",
-                    "description": "Process with graph edges process",
-                    "product_type": "Product_1",
-                    "processes": [
-                        ["P1", "P2"],
-                        ["P1", "P3"],
-                        ["P2", "P4"],
-                        ["P3", "P4"],
-                    ],
-                    "transport_process": "TP1",
+    
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "Product_1",
+                "description": "Product with sequential process",
+                "product_type": "Product_1",
+                "processes": ["P1", "P2", "P3"],
+                "transport_process": "TP1",
+            },
+            {
+                "ID": "Product_1",
+                "description": "Process with adjacency matrix process",
+                "product_type": "Product_1",
+                "processes": {
+                    "P1": ["P2", "P3"],
+                    "P2": ["P3"],
+                    "P3": [],
                 },
-            ]
-        }
+                "transport_process": "TP1",
+            },
+            {
+                "ID": "Product_1",
+                "description": "Process with graph edges process",
+                "product_type": "Product_1",
+                "processes": [
+                    ["P1", "P2"],
+                    ["P1", "P3"],
+                    ["P2", "P4"],
+                    ["P3", "P4"],
+                ],
+                "transport_process": "TP1",
+            },
+        ]
+    })
```

### Comparing `prodsys-0.6.5/prodsys/models/queue_data.py` & `prodsys-0.7.0/prodsys/models/queue_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from __future__ import annotations
-
 from typing import Union
 from hashlib import md5
 
+from pydantic import ConfigDict
+
 from prodsys.models.core_asset import CoreAsset
 
 
 class QueueData(CoreAsset):
     """
     Class that represents a queue. If capacity is 0, the queue is considered infinite. Otherwise, the queue can hold a finite number of products cooresponding to the capacity.
 
@@ -44,23 +44,22 @@
 
 
         Returns:
             str: Hash of the queue.
         """
         return md5((str(self.capacity)).encode("utf-8")).hexdigest()
 
-
-    class Config:
-        schema_extra = {
-            "examples": [
-                {
-                    "ID": "Q1",
-                    "description": "Finte Queue",
-                    "capacity": 10,
-                },
-                {
-                    "ID": "Q1",
-                    "description": "Infinite Queue",
-                    "capacity": 0.0,
-                },
-            ]
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "Q1",
+                "description": "Finte Queue",
+                "capacity": 10,
+            },
+            {
+                "ID": "Q1",
+                "description": "Infinite Queue",
+                "capacity": 0.0,
+            },
+        ]
+    
+    })
```

### Comparing `prodsys-0.6.5/prodsys/models/resource_data.py` & `prodsys-0.7.0/prodsys/models/resource_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 """
 
 from __future__ import annotations
 from hashlib import md5
 from typing import Literal, Union, List, Optional, TYPE_CHECKING
 from enum import Enum
 
-from pydantic import validator, conlist
+from pydantic import ConfigDict, model_validator, conlist
 from prodsys.models.core_asset import CoreAsset
 
 if TYPE_CHECKING:
     from prodsys.adapters.adapter import ProductionSystemAdapter
 
-
 class ControllerEnum(str, Enum):
     """
     Enum that represents the controller of a resource.
 
     - PipelineController: Pipeline controller.
     - TransportController: Transport controller.
     """
@@ -73,34 +72,36 @@
         control_policy (Union[ResourceControlPolicy, TransportControlPolicy]): Control policy of the resource.
         process_ids (List[str]): Process IDs of the resource.
         process_capacities (Optional[List[int]], optional): Process capacities of the resource (in sequence of the capacity of the resource). Defaults to None.
         state_ids (Optional[List[str]], optional): State IDs of the resource. Defaults to [].
     """
 
     capacity: int
-    location: conlist(float, min_items=2, max_items=2) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) # type: ignore
 
     controller: ControllerEnum
     control_policy: Union[ResourceControlPolicy, TransportControlPolicy]
 
     process_ids: List[str]
     process_capacities: Optional[List[int]]
     state_ids: Optional[List[str]] = []
 
-    @validator("process_capacities", always=True)
-    def check_process_capacity(cls, v, values):
-        if not v:
-            return [values["capacity"] for _ in values["process_ids"]]
-        if len(v) != len(values["process_ids"]):
+    @model_validator(mode="before")
+    def check_process_capacity(cls, values):
+        if not isinstance(values, dict):
+            return values
+        if not "process_capacities" in values or values["process_capacities"] is None:
+            values["process_capacities"] = [values["capacity"] for _ in values["process_ids"]]
+        if len(values["process_capacities"]) != len(values["process_ids"]):
             raise ValueError(
-                f"process_capacities {v} must have the same length as processes {values['process_ids']}"
+                f"process_capacities {values['process_capacities']} must have the same length as processes {values['process_ids']}"
             )
-        if max(v) > values["capacity"]:
+        if max(values["process_capacities"]) > values["capacity"]:
             raise ValueError("process_capacities must be smaller than capacity")
-        return v 
+        return values
     
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash of the resource considering the capacity, location, controller, processes, process capacities and states. Can be used to compare resources for equal functionality.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter that contains the process and state data.
@@ -173,16 +174,16 @@
         )
         ```
     """
 
     controller: Literal[ControllerEnum.PipelineController]
     control_policy: ResourceControlPolicy
 
-    input_queues: Optional[List[str]]
-    output_queues: Optional[List[str]]
+    input_queues: List[str] = []
+    output_queues: List[str] = []
 
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash of the resource considering the capacity, location, controller, processes, process capacities, states, input queues and output queues. Can be used to compare resources for equal functionality.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter that contains the process and queue data.
@@ -201,40 +202,34 @@
                     queue_hashes.append(queue.hash())
                     break
             else:
                 raise ValueError(f"Queue with ID {queue_id} not found for resource {self.ID}.")
 
         return md5(("".join([base_class_hash, *sorted(queue_hashes)])).encode("utf-8")).hexdigest()
 
-
-
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Production Resource Data",
-                "value": {
-                    "ID": "R1",
-                    "description": "Resource 1",
-                    "capacity": 2,
-                    "location": [10.0, 10.0],
-                    "controller": "PipelineController",
-                    "control_policy": "FIFO",
-                    "process_ids": ["P1", "P2"],
-                    "process_capacities": [2, 1],
-                    "states": [
-                        "Breakdownstate_1",
-                        "Setup_State_1",
-                        "Setup_State_2",
-                        "ProcessBreakdownState_1",
-                    ],
-                    "input_queues": ["IQ1"],
-                    "output_queues": ["OQ1"],
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "R1",
+                "description": "Resource 1",
+                "capacity": 2,
+                "location": [10.0, 10.0],
+                "controller": "PipelineController",
+                "control_policy": "FIFO",
+                "process_ids": ["P1", "P2"],
+                "process_capacities": [2, 1],
+                "states": [
+                    "Breakdownstate_1",
+                    "Setup_State_1",
+                ],
+                "input_queues": ["IQ1"],
+                "output_queues": ["OQ1"],
             }
-        }
+        ]
+    })
 
 
 class TransportResourceData(ResourceData):
     """
     Class that represents transport resource data.
 
     Args:
@@ -263,27 +258,24 @@
         )
         ```
     """
 
     controller: Literal[ControllerEnum.TransportController]
     control_policy: TransportControlPolicy
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Transport Resource Data",
-                "value": {
-                    "ID": "TR1",
-                    "description": "Transport Resource 1",
-                    "capacity": 1,
-                    "location": [15.0, 15.0],
-                    "controller": "TransportController",
-                    "control_policy": "FIFO",
-                    "process_ids": ["TP1"],
-                    "process_capacities": None,
-                    "states": ["Breakdownstate_1"],
-                },
-            }
-        }
-
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "TR1",
+                "description": "Transport Resource 1",
+                "capacity": 1,
+                "location": [15.0, 15.0],
+                "controller": "TransportController",
+                "control_policy": "FIFO",
+                "process_ids": ["TP1"],
+                "process_capacities": None,
+                "states": ["Breakdownstate_1"],
+            },
+        ]
+    })
 
 RESOURCE_DATA_UNION = Union[ProductionResourceData, TransportResourceData]
```

### Comparing `prodsys-0.6.5/prodsys/models/scenario_data.py` & `prodsys-0.7.0/prodsys/models/scenario_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 This module contains the data structures for the scenario data that is used in optimization to determine the best configuration of a production system. A Scenario constists thereby of:
 - `ScenarioConstrainsData`: The constraints of the scenario.
 - `ScenarioOptionsData`: The options of the scenario.
 - `ScenarioInfoData`: The information of the scenario.
 - 'Objectives': The objectives of the scenario.
 - `ScenarioData`: The scenario data that contains the constraints, options, information and objectives of the scenario. 
 """
-
-from __future__ import annotations
-
 from typing import Literal, List, Optional, Dict
 from enum import Enum
 
-from pydantic import BaseModel, validator, conlist
+from pydantic import BaseModel, ConfigDict, field_validator, conlist
 
 from prodsys.models.performance_indicators import KPIEnum
 
 
 class ReconfigurationEnum(str, Enum):
     """
     Enum that represents the different levels of reconfigurations that are possible.
@@ -53,72 +50,74 @@
 
     max_reconfiguration_cost: float
     max_num_machines: int
     max_num_processes_per_machine: int
     max_num_transport_resources: int
     target_product_count: Optional[Dict[str, int]]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Scenario constraints",
-                "value": {
-                    "max_reconfiguration_cost": 120000,
-                    "max_num_machines": 10,
-                    "max_num_processes_per_machine": 2,
-                    "max_num_transport_resources": 2,
-                    "target_product_count": {"Product_1": 120, "Product_2": 200},
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "max_reconfiguration_cost": 120000,
+                "max_num_machines": 10,
+                "max_num_processes_per_machine": 2,
+                "max_num_transport_resources": 2,
+                "target_product_count": {"Product_1": 120, "Product_2": 200},
             }
-        }
-
+        ]
+    })
 
 class ScenarioOptionsData(BaseModel):
     """
     Class that represents the options of a scenario. The options are used to define the deegrees of freedom in the
     optimization scenario, i.e. the different possibilities to adjust the configuration to find a solution with higher
     performance. Options consider possible transformations of the configuration, possible logics of controllers and routers
     and possible positions of machines in the layout.
 
     Args:
         transformations (List[ReconfigurationEnum]): List of possible transformations of the configuration.
         machine_controllers (List[Literal["FIFO", "LIFO", "SPT"]]): List of possible controllers for machines.
         transport_controllers (List[Literal["FIFO", "SPT_transport", "Nearest_origin_and_longest_target_queues_transport", "Nearest_origin_and_shortest_target_input_queues_transport"]]): List of possible controllers for transport resources.
         routing_heuristics (List[Literal["shortest_queue", "random", "FIFO"]]): List of possible routing heuristics for sources.
-        positions (List[conlist(float, min_items=2, max_items=2)]): List of possible positions for machines in the layout.
+        positions (List[conlist(float, min_length=2, max_length=2)]): List of possible positions for machines in the layout.
 
     Raises:
         ValueError: If the positions are not a list of tuples of length 2.
     """
 
     transformations: List[ReconfigurationEnum]
     machine_controllers: List[Literal["FIFO", "LIFO", "SPT"]]
     transport_controllers: List[Literal["FIFO", "SPT_transport"]]
     routing_heuristics: List[Literal["shortest_queue", "random", "FIFO"]]
-    positions: List[conlist(float, min_items=2, max_items=2)] # type: ignore
+    positions: List[conlist(float, min_length=2, max_length=2)] # type: ignore
 
-    @validator("positions")
+    @field_validator("positions")
     def check_positions(cls, v):
         for e in v:
             if len(e) != 2:
                 raise ValueError("positions must be a list of tuples of length 2")
         return v
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Scenario options",
-                "value": {
-                    "machine_controllers": ["FIFO", "LIFO", "SPT"],
-                    "transport_controllers": ["FIFO", "SPT_transport"],
-                    "routing_heuristics": ["shortest_queue", "random", "FIFO"],
-                    "positions": [[10.0, 10.0], [20.0, 20.0]],
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "transformations": [
+                    "production_capacity",
+                    "transport_capacity",
+                    "layout",
+                    "sequencing_logic",
+                    "routing_logic",
+                ],
+                "machine_controllers": ["FIFO", "LIFO", "SPT"],
+                "transport_controllers": ["FIFO", "SPT_transport"],
+                "routing_heuristics": ["shortest_queue", "random", "FIFO"],
+                "positions": [[10.0, 10.0], [20.0, 20.0]],
             }
-        }
+        ]
+    })
 
 
 class ScenarioInfoData(BaseModel):
     """
     Class that represents the information of a scenario. The information is used to define some parameters that allow
     evaluation of the scenario.
 
@@ -134,51 +133,48 @@
     machine_cost: float
     transport_resource_cost: float
     process_module_cost: float
     breakdown_cost: Optional[float]
     time_range: Optional[int]
     maximum_breakdown_time: Optional[int]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Scenario information",
-                "value": {
-                    "machine_cost": 30000,
-                    "transport_resource_cost": 20000,
-                    "process_module_cost": 2300,
-                    "breakdown_cost": 1000,
-                    "time_range": 2600,
-                    "maximum_breakdown_time": 10,
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "machine_cost": 30000,
+                "transport_resource_cost": 20000,
+                "process_module_cost": 2300,
+                "breakdown_cost": 1000,
+                "time_range": 2600,
+                "maximum_breakdown_time": 10,
             }
-        }
+        ]
+    })
 
 
 class Objective(BaseModel):
     name: KPIEnum
     weight: float = 1.0
 
-    class Config:
-        schema_extra = {
-            "examples": [
-                {
-                    "name": KPIEnum.COST,
-                    "weight": 0.6,
-                },
-                {
-                    "name": KPIEnum.THROUGHPUT,
-                    "weight": 0.1,
-                },
-                {
-                    "name": KPIEnum.WIP,
-                    "weight": 0.5,
-                },
-            ]
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "name": KPIEnum.COST,
+                "weight": 0.6,
+            },
+            {
+                "name": KPIEnum.THROUGHPUT,
+                "weight": 0.1,
+            },
+            {
+                "name": KPIEnum.WIP,
+                "weight": 0.5,
+            },
+        ]
+    })
 
 
 class ScenarioData(BaseModel):
     """
     Class that represents a scenario and contraints data about constaints, options, information and objectives of the scenario.
 
     Args:
@@ -192,18 +188,17 @@
     """
 
     constraints: ScenarioConstrainsData
     options: ScenarioOptionsData
     info: ScenarioInfoData
     objectives: List[Objective]
 
-    class Config:
-        use_enum_values = True
-        schema_extra = {
-            "example": {
+    model_config=ConfigDict(use_enum_values=True, json_schema_extra={
+        "examples": [
+            {
                 "summary": "Scenario",
                 "value": {
                     "constraints": {
                         "max_reconfiguration_cost": 120000,
                         "max_num_machines": 10,
                         "max_num_processes_per_machine": 2,
                         "max_num_transport_resources": 2,
@@ -242,8 +237,9 @@
                         {
                             "name": KPIEnum.WIP,
                             "weight": 0.5,
                         },
                     ],
                 },
             }
-        }
+        ]
+    })
```

### Comparing `prodsys-0.6.5/prodsys/models/sink_data.py` & `prodsys-0.7.0/prodsys/models/sink_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from hashlib import md5
 from typing import List, Optional, TYPE_CHECKING
-from pydantic import conlist
+from pydantic import ConfigDict, conlist
 
 from prodsys.models.core_asset import CoreAsset
 
 if TYPE_CHECKING:
     from prodsys.adapters.adapter import ProductionSystemAdapter
 
 
@@ -31,31 +31,29 @@
             location=[50.0, 50.0],
             product_type="Product_1",
             input_queues=["SinkQueue"],
         )
         ```
     """
 
-    location: conlist(float, min_items=2, max_items=2) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) # type: ignore
     product_type: str
-    input_queues: Optional[List[str]]
-    
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Sink",
-                "value": {
-                    "ID": "SK1",
-                    "description": "Sink 1",
-                    "location": [50.0, 50.0],
-                    "product_type": "Product_1",
-                    "input_queues": ["SinkQueue"],
-                },
+    input_queues: List[str] = []
+
+    model_config=ConfigDict(json_schema_extra= {
+        "examples": [
+            {
+                "ID": "SK1",
+                "description": "Sink 1",
+                "location": [50.0, 50.0],
+                "product_type": "Product_1",
+                "input_queues": ["SinkQueue"],
             }
-        }
+        ]
+    })
     
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash for the sink considering its location, product type and input queues.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter of the production system.
```

### Comparing `prodsys-0.6.5/prodsys/models/source_data.py` & `prodsys-0.7.0/prodsys/models/source_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from hashlib import md5
 from typing import List, Optional, TYPE_CHECKING
-from pydantic import conlist
+from pydantic import ConfigDict, conlist
 from enum import Enum
 
 from prodsys.models.core_asset import CoreAsset
 
 if TYPE_CHECKING:
     from prodsys.adapters.adapter import ProductionSystemAdapter
 
@@ -44,19 +44,19 @@
             product_type="Product_1",
             time_model_id="function_time_model_4",
             router="SimpleRouter",
             routing_heuristic="shortest_queue",
             output_queues=["SourceQueue"],
         )
     """
-    location: conlist(float, min_items=2, max_items=2) # type: ignore
+    location: conlist(float, min_length=2, max_length=2) # type: ignore
     product_type: str
     time_model_id: str
     routing_heuristic: RoutingHeuristic
-    output_queues: Optional[List[str]]
+    output_queues: List[str] = []
     
     def hash(self, adapter: ProductionSystemAdapter) -> str:
         """
         Returns a unique hash for the source considering its location, product type, time model, routing heuristic and output queues.
 
         Args:
             adapter (ProductionSystemAdapter): Adapter of the production system.
@@ -88,23 +88,21 @@
                     output_queue_hashes.append(queue.hash())
                     break
             else:
                 raise ValueError(f"Queue with ID {output_queue} not found for source {self.ID}.")
 
         return md5(("".join([*map(str, self.location), product_hash, time_model_hash, self.routing_heuristic, *sorted(output_queue_hashes)])).encode("utf-8")).hexdigest()
     
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Source",
-                "value": {
-                    "ID": "S1",
-                    "description": "Source 1",
-                    "location": [0.0, 0.0],
-                    "product_type": "Product_1",
-                    "time_model_id": "function_time_model_4",
-                    "router": "SimpleRouter",
-                    "routing_heuristic": "shortest_queue",
-                    "output_queues": ["SourceQueue"],
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "S1",
+                "description": "Source 1",
+                "location": [0.0, 0.0],
+                "product_type": "Product_1",
+                "time_model_id": "function_time_model_4",
+                "router": "SimpleRouter",
+                "routing_heuristic": "shortest_queue",
+                "output_queues": ["SourceQueue"],
             }
-        }
+        ]
+    })
```

### Comparing `prodsys-0.6.5/prodsys/models/state_data.py` & `prodsys-0.7.0/prodsys/models/state_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 
 - `BreakDownStateData`: A state that makes a resource unavailable for a certain time.
 - `ProcessBreakDownStateData`: A state that makes a process unavailable for a certain time but other processes can still be performed.
 - `SetupStateData`: A state that represents the time needed to change the process of a resource.
 - `ProductionStateData`: A state that represents the time needed to process a product.
 - `TransportStateData`: A state that represents the time needed to transport a product.	    
 """
-
 from __future__ import annotations
+
 from hashlib import md5
 from enum import Enum
 from typing import Literal, Union, TYPE_CHECKING
 
+from pydantic import ConfigDict
+
 from prodsys.models.core_asset import CoreAsset
 
 if TYPE_CHECKING:
     from prodsys.adapters.adapter import ProductionSystemAdapter
 
 
-
 class StateTypeEnum(str, Enum):
     """
     Enum that represents the different kind of states.
 
     - BreakDownState: A state that makes a resource unavailable for a certain time.
     - ProductionState: A state that represents the time needed to process a product.
     - TransportState: A state that represents the time needed to transport a product.
@@ -77,27 +78,25 @@
         for time_model in adapter.time_model_data:
             if time_model.ID == self.time_model_id:
                 time_model_hash = time_model.hash()
                 break
         else:
             raise ValueError(f"Time model with ID {self.time_model_id} not found for state {self.ID}.")
         return md5(("".join([self.type, time_model_hash])).encode("utf-8")).hexdigest()
-
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "State",
-                "value": {
-                    "ID": "state_1",
-                    "description": "State data for state_1",
-                    "time_model_id": "time_model_1",
-                    "type": "ProductionState",
-                },
+    
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "state_1",
+                "description": "State data for state_1",
+                "time_model_id": "time_model_1",
+                "type": "ProductionState",
             }
-        }
+        ]
+    })
 
 
 class BreakDownStateData(StateData):
     """
     Class that represents a breakdown state.
 
     Args:
@@ -144,27 +143,25 @@
                 repair_time_model_hash = repair_time_model.hash()
                 break
         else:
             raise ValueError(f"Repair time model with ID {self.repair_time_model_id} not found for state {self.ID}.")
 
         return md5(("".join([base_class_hash, repair_time_model_hash])).encode("utf-8")).hexdigest()  
     
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Breakdown state",
-                "value": {
-                    "ID": "Breakdownstate_1",
-                    "description": "Breakdown state machine 1",
-                    "time_model_id": "function_time_model_5",
-                    "type": "BreakDownState",
-                    "repair_time_model_id": "function_time_model_8",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "Breakdownstate_1",
+                "description": "Breakdown state machine 1",
+                "time_model_id": "function_time_model_5",
+                "type": "BreakDownState",
+                "repair_time_model_id": "function_time_model_8",
             }
-        }
+        ]
+    })
 
 
 class ProcessBreakDownStateData(StateData):
     """
     Class that represents a process breakdown state. It is a breakdown state that is connected to a process. Other processes can still be executed while the process breakdown state is activen.
 
     Args:
@@ -222,29 +219,27 @@
                 repair_time_model_hash = repair_time_model.hash()
                 break
         else:
             raise ValueError(f"Repair time model with ID {self.repair_time_model_id} not found for process breakdown state {self.ID}.")
         
 
         return md5(("".join([base_class_hash, process_hash, repair_time_model_hash])).encode("utf-8")).hexdigest()
-
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Process breakdown state",
-                "value": {
-                    "ID": "ProcessBreakDownState_1",
-                    "description": "Process Breakdown state machine 1",
-                    "time_model_id": "function_time_model_7",
-                    "type": "ProcessBreakDownState",
-                    "process_id": "P1",
-                    "repair_time_model_id": "function_time_model_8",
-                },
+    
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "ProcessBreakDownState_1",
+                "description": "Process Breakdown state machine 1",
+                "time_model_id": "function_time_model_7",
+                "type": "ProcessBreakDownState",
+                "process_id": "P1",
+                "repair_time_model_id": "function_time_model_8",
             }
-        }
+        ]
+    })
 
 
 class ProductionStateData(StateData):
     """
     Class that represents a production state. By undergoing a production state, the product is processed and continues its process model. Production states don't have to be initialized because they are automatically created when a process is added to a resource.
 
     Args:
@@ -253,53 +248,48 @@
         time_model_id (str): Time model ID of the state.
         type (StateTypeEnum): Type of the state.
 
     """
 
     type: Literal[StateTypeEnum.ProductionState]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Production state",
-                "value": {
-                    "ID": "ProductionState_1",
-                    "description": "Production state machine 1",
-                    "time_model_id": "function_time_model_1",
-                    "type": "ProductionState",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "ProductionState_1",
+                "description": "Production state machine 1",
+                "time_model_id": "function_time_model_1",
+                "type": "ProductionState",
             }
-        }
-
+        ]
+    })
 
 class TransportStateData(StateData):
     """
     Class that represents a transport state. By undergoing a transport state, the product is transported and its position is changed. Transport states don't have to be initialized because they are automatically created when a transport process is added to a resource.
 
     Args:
         ID (str): ID of the state.
         description (str): Description of the state.
         time_model_id (str): Time model ID of the state.
         type (StateTypeEnum): Type of the state.
     """
 
     type: Literal[StateTypeEnum.TransportState]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Transport state",
-                "value": {
-                    "ID": "TransportState_1",
-                    "description": "Transport state machine 1",
-                    "time_model_id": "function_time_model_3",
-                    "type": "TransportState",
-                },
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "TransportState_1",
+                "description": "Transport state machine 1",
+                "time_model_id": "function_time_model_3",
+                "type": "TransportState",
             }
-        }
+        ]
+    })
 
 
 class SetupStateData(StateData):
     """
     Class that represents a setup state. By undergoing a setup state, the process is setup.
 
     Args:
@@ -349,29 +339,27 @@
                 if process.ID == process_id:
                     setup_process_hashes.append(process.hash(adapter))
                 break
             else:
                 raise ValueError(f"Process with ID {process_id} not found for setup state {self.ID}.")
 
         return md5(("".join([base_class_hash] + setup_process_hashes)).encode("utf-8")).hexdigest()
-
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Setup state",
-                "value": {
-                    "ID": "Setup_State_2",
-                    "description": "Setup state machine 2",
-                    "time_model_id": "function_time_model_2",
-                    "type": "SetupState",
-                    "origin_setup": "P2",
-                    "target_setup": "P1",
-                },
+    
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "Setup_State_2",
+                "description": "Setup state machine 2",
+                "time_model_id": "function_time_model_2",
+                "type": "SetupState",
+                "origin_setup": "P2",
+                "target_setup": "P1",
             }
-        }
+        ]
+    })
 
 
 STATE_DATA_UNION = Union[
     BreakDownStateData,
     ProductionStateData,
     TransportStateData,
     SetupStateData,
```

### Comparing `prodsys-0.6.5/prodsys/models/time_model_data.py` & `prodsys-0.7.0/prodsys/models/time_model_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 of products, performance of processes and transports and the duration of states.
 
 The following time models are possible:
 - `SequentialTimeModelData`: A time model that is based on a sequence of values.
 - `FunctionTimeModelData`: A time model that is based on a distribution function which gets sampled.
 - `ManhattanDistanceTimeModelData`: A time model that is based on the manhattan distance between two nodes and a constant velocity.
 """
+# from __future__ import annotations
 
-from __future__ import annotations
 from hashlib import md5
 from typing import List, Literal, Union
 from typing_extensions import deprecated
 from enum import Enum
 
-from pydantic import Field
+from pydantic import ConfigDict, Field
 
 from prodsys.models.core_asset import CoreAsset
 from prodsys.util.statistical_functions import FunctionTimeModelEnum
 
 
 class TimeModelEnum(str, Enum):
     """
@@ -76,25 +76,24 @@
         Returns a unique hash for the time model considering its sequence. Can be used to compare time models for equal functionality.
 
         Returns:
             str: Hash of the time model.
         """
         return md5(("".join([*map(str, self.sequence)])).encode("utf-8")).hexdigest()
     
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Sequential time model",
-                "value": {
-                    "ID": "sequence_time_model_1",
-                    "description": "Examplary sequence time model",
-                    "sequence": [25.0, 13.0, 15.0, 16.0, 17.0, 20.0, 21.0],
-                },
-            }
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "sequence_time_model_1",
+                "description": "Examplary sequence time model",
+                "sequence": [25.0, 13.0, 15.0, 16.0, 17.0, 20.0, 21.0],
+            },
+        ]
+    
+    })
 
 
 class SampleTimeModelData(CoreAsset):
     """
     Class that represents a time model that samples values from a provided data set by random choice of a sample element.
 
     Args:
@@ -121,25 +120,24 @@
         Returns a unique hash for the time model considering its samples. Can be used to compare time models for equal functionality.
 
         Returns:
             str: Hash of the time model.
         """
         return md5(("".join([*map(str, self.samples)])).encode("utf-8")).hexdigest()
     
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Sample time model",
-                "value": {
-                    "ID": "sample_time_model_1",
-                    "description": "Examplary sample time model",
-                    "samples": [25.0, 13.0, 15.0, 16.0, 17.0, 20.0, 21.0],
-                },
-            }
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "sample_time_model_1",
+                "description": "Examplary sample time model",
+                "samples": [25.0, 13.0, 15.0, 16.0, 17.0, 20.0, 21.0],
+            },
+        ]
+    
+    })
 
 
 class ScheduledTimeModelData(CoreAsset):
     """
     Class that represents a time model that is based on a schedule of timely values. Should only be used for arrival time models of sources.
 
     Args:
@@ -172,27 +170,26 @@
         Returns a unique hash for the time model considering its schedule and boolean values. Can be used to compare time models for equal functionality.
 
         Returns:
             str: Hash of the time model.
         """
         return md5(("".join([*map(str, self.schedule)] + [*map(str, [self.absolute, self.cyclic])])).encode("utf-8")).hexdigest()
     
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Scheduled time model",
-                "value": {
-                    "ID": "scheduled_time_model_1",
-                    "description": "Examplary scheduled time model",
-                    "schedule": [3.0, 5.0, 7.0, 9.0, 11.0, 13.0, 15.0],
-                    "absolute": True,
-                    "cyclic": False
-                },
-            }
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "scheduled_time_model_1",
+                "description": "Examplary scheduled time model",
+                "schedule": [3.0, 5.0, 7.0, 9.0, 11.0, 13.0, 15.0],
+                "absolute": True,
+                "cyclic": False
+            },
+        ]
+    
+    })
 
 
 class FunctionTimeModelData(CoreAsset):
     """
     Class that represents a time model that is based on a function and represents the timely values by their distribution function.
 
     Args:
@@ -217,27 +214,26 @@
     """
 
     distribution_function: FunctionTimeModelEnum
     location: float
     scale: float
     batch_size: int = Field(default=100, init=False)
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Function time model",
-                "value": {
-                    "ID": "function_time_model_1",
-                    "description": "normal distribution time model with 20 minutes",
-                    "distribution_function": "normal",
-                    "location": 20.0,
-                    "scale": 5.0,
-                },
-            }
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "function_time_model_1",
+                "description": "normal distribution time model with 20 minutes",
+                "distribution_function": "normal",
+                "location": 20.0,
+                "scale": 5.0,
+            },
+        ]
+    
+    })
     
     def hash(self) -> str:
         """
         Returns a unique hash for the time model considering its distribution function, location and scale. Can be used to compare time models for equal functionality.
 
         Returns:
             str: Hash of the time model.
@@ -278,27 +274,24 @@
         Returns a unique hash for the time model considering its speed and reaction time. Can be used to compare time models for equal functionality.
 
         Returns:
             str: Hash of the time model.
         """
         return md5(("".join([*map(str, [self.speed, self.reaction_time])])).encode("utf-8")).hexdigest()
     
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Manhattan time model",
-                "value": {
-                    "ID": "manhattan_time_model_1",
-                    "description": "manhattan time model with speed 180 m/min = 3 m/s",
-                    "speed": 30.0,
-                    "reaction_time": 0.15,
-                },
-            }
-        }
-
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "manhattan_time_model_1",
+                "description": "manhattan time model with speed 180 m/min = 3 m/s",
+                "speed": 180.0,
+                "reaction_time": 0.15,
+            },
+        ]
+    })
 
 class DistanceTimeModelData(CoreAsset):
     """
     Class that represents a time model that is based on the distance between two nodes and a constant velocity.
     The distance is calculated based on the metric provided.
 
     Args:
@@ -330,25 +323,23 @@
         Returns a unique hash for the time model considering its speed and reaction time. Can be used to compare time models for equal functionality.
 
         Returns:
             str: Hash of the time model.
         """
         return md5(("".join([*map(str, [self.speed, self.reaction_time, self.metric])])).encode("utf-8")).hexdigest()
     
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Distance time model",
-                "value": {
-                    "ID": "distance_time_model_1",
-                    "description": "distance time model with speed 180 m/min = 3 m/s",
-                    "speed": 30.0,
-                    "reaction_time": 0.15,
-                    "metric": "manhattan",
-                },
-            }
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "ID": "distance_time_model_1",
+                "description": "distance time model with speed 180 m/min = 3 m/s",
+                "speed": 30.0,
+                "reaction_time": 0.15,
+                "metric": "manhattan",
+            },
+        ]
+    })
 
 
 TIME_MODEL_DATA = Union[
     FunctionTimeModelData, SampleTimeModelData, ScheduledTimeModelData, DistanceTimeModelData, SequentialTimeModelData, ManhattanDistanceTimeModelData, 
 ]
```

### Comparing `prodsys-0.6.5/prodsys/optimization/__init__.py` & `prodsys-0.7.0/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.7.0/prodsys/optimization/evolutionary_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 from os import listdir
 from os.path import isfile, join
 
 from deap import algorithms, base, creator, tools
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from prodsys.simulation import sim
 from prodsys import adapters
 from prodsys.optimization.optimization_util import (
     crossover,
     evaluate,
     mutation,
@@ -62,29 +62,27 @@
     number_of_generations: int = 10
     population_size: int = 10
     mutation_rate: float = 0.1
     crossover_rate: float = 0.1
     number_of_seeds: int = 1
     number_of_processes: int = 1
 
-    class Config:
-        schema_extra = {
-            "examples": [
-                {
-                    "seed": 0,
-                    "number_of_generations": 10,
-                    "population_size": 10,
-                    "mutation_rate": 0.1,
-                    "crossover_rate": 0.1,
-                    "number_of_seeds": 1,
-                    "number_of_processes": 1,
-                },
-            ]
-        }
-
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "seed": 0,
+                "number_of_generations": 10,
+                "population_size": 10,
+                "mutation_rate": 0.1,
+                "crossover_rate": 0.1,
+                "number_of_seeds": 1,
+                "number_of_processes": 1,
+            },
+        ]
+    })
 
 
 def register_functions_in_toolbox(
     base_configuration: adapters.JsonProductionSystemAdapter,
     solution_dict: dict,
     performances: dict,
     weights: tuple,
@@ -256,15 +254,15 @@
         base_configuration (adapters.ProductionSystemAdapter): production system to optimize.
         hyper_parameters (EvolutionaryAlgorithmHyperparameters): Hyperparameters for configuration optimization using an evolutionary algorithm.
         save_folder (str): Folder to save the results in. Defaults to "results".
         initial_solutions_folder (str, optional): If specified, the initial solutions are read from this folder and considered in optimization. Defaults to "".
     """
     adapters.ProductionSystemAdapter.Config.validate = False
     adapters.ProductionSystemAdapter.Config.validate_assignment = False
-    base_configuration = base_configuration.copy(deep=True)
+    base_configuration = base_configuration.model_copy(deep=True)
     if not adapters.check_for_clean_compound_processes(base_configuration):
         logger.warning("Both compound processes and normal processes are used. This may lead to unexpected results.")
     if not check_breakdown_states_available(base_configuration):
         create_default_breakdown_states(base_configuration)
 
     util.prepare_save_folder(save_folder + "/")
     set_seed(hyper_parameters.seed)
```

### Comparing `prodsys-0.6.5/prodsys/optimization/math_opt.py` & `prodsys-0.7.0/prodsys/optimization/math_opt.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from copy import deepcopy
 import json
 import random
 import logging
 logger = logging.getLogger(__name__)
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 from prodsys import adapters
 from prodsys.models import (
     resource_data,
     processes_data,
     state_data,
     time_model_data,
 )
@@ -35,15 +35,15 @@
     Args:
         adapter_object (adapters.Adapter): Adapter object.
         number_of_transport_resources (int): Number of transport resources.
     """
     existing_transport_resource = adapter_object.resource_data[0]
     existing_transport_resource.ID = "TR0"
     for i in range(number_of_transport_resources - 1):
-        new_transport_resource = existing_transport_resource.copy(deep=True)
+        new_transport_resource = existing_transport_resource.model_copy(deep=True)
         new_transport_resource.ID = f"TR{i + 1}"
         adapter_object.resource_data.append(new_transport_resource)
 
 
 def get_modul_counts(adapter: adapters.ProductionSystemAdapter) -> Dict[str, int]:
     modul_count_dict = {}
     # Fall Prozessmodul noch nicht vorhanden fehlt
@@ -76,16 +76,15 @@
     s: Any = None
     a: Any = None
     v: Any = None
     t: Any = None
 
     processing_times_per_product_and_step: dict = None
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config=ConfigDict(arbitrary_types_allowed=True)
 
     def cost_module(self, x: int, Modul: str) -> int:
         module_cost = self.adapter.scenario_data.info.process_module_cost
         return module_cost * (x - get_modul_counts(self.adapter)[Modul])
 
     def set_variables(
         self,
@@ -462,15 +461,15 @@
         """
         nSolutions = self.model.SolCount
         solution_dict = {"current_generation": "00", "00": []}
         performances = {}
         performances["00"] = {}
 
         for result_counter in range(nSolutions):
-            new_adapter = self.adapter.copy(deep=True)
+            new_adapter = self.adapter.model_copy(deep=True)
             new_adapter.resource_data = [
                 resource
                 for resource in self.adapter.resource_data
                 if not isinstance(resource, resource_data.ProductionResourceData)
             ]
             adjust_number_of_transport_resources(
                 new_adapter, adjusted_number_of_transport_resources
@@ -542,25 +541,24 @@
     """
 
     optimization_time_portion: float = 0.5
     number_of_solutions: int = 1
     adjusted_number_of_transport_resources: int = 1
     number_of_seeds: int = 1
 
-    class Config:
-        schema_extra = {
-            "examples": [
-                {
-                    "optimization_time_portion": 0.5,
-                    "number_of_solutions": 1,
-                    "adjusted_number_of_transport_resources": 1,
-                    "number_of_seeds": 1,
-                },
-            ]
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "optimization_time_portion": 0.5,
+                "number_of_solutions": 1,
+                "adjusted_number_of_transport_resources": 1,
+                "number_of_seeds": 1,
+            },
+        ]
+    })
 
 
 def run_mathematical_optimization(
     save_folder: str,
     base_configuration_file_path: str,
     scenario_file_path: str,
     full_save: bool,
```

### Comparing `prodsys-0.6.5/prodsys/optimization/optimization_analysis.py` & `prodsys-0.7.0/prodsys/optimization/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/optimization/optimization_util.py` & `prodsys-0.7.0/prodsys/optimization/optimization_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,30 +148,30 @@
     transport_resources = adapters.get_transport_resources(adapter_object)
     machine_breakdown_states = [state for state in breakdown_states if any(state.ID in machine.state_ids for machine in machines)]
     transport_resource_breakdown_states = [state for state in breakdown_states if any(state.ID in transport_resource.state_ids for transport_resource in transport_resources)]
     # process_breakdown_states = [state for state in process_breakdown_states if any(state.ID in machine.state_ids and state.process_id in machine.process_ids for machine in machines)]
     if machine_breakdown_states and not check_breakdown_state_available(adapter_object, BreakdownStateNamingConvention.MACHINE_BREAKDOWN_STATE):
         if not check_states_for_heterogenous_time_models(machine_breakdown_states, adapter_object):
             raise ValueError(f"The machine breakdown states are not heterogenous and it is not ambiguous which state should be the Breakdownstate. Please check the time models or define a distinct machine breakdown state called {BreakdownStateNamingConvention.MACHINE_BREAKDOWN_STATE}.")
-        machine_breakdown_state = machine_breakdown_states[0].copy(deep=True)
+        machine_breakdown_state = machine_breakdown_states[0].model_copy(deep=True)
         machine_breakdown_state.ID = BreakdownStateNamingConvention.MACHINE_BREAKDOWN_STATE
         adapter_object.state_data.append(machine_breakdown_state)
         logger.info(f"Added default breakdown state for production resources to the production system.")
     if transport_resource_breakdown_states and not check_breakdown_state_available(adapter_object, BreakdownStateNamingConvention.TRANSPORT_RESOURCE_BREAKDOWN_STATE):
         if not check_states_for_heterogenous_time_models(transport_resource_breakdown_states, adapter_object):
             raise ValueError(f"The transport resource breakdown states are not heterogenous and it is not ambiguous which state should be the Breakdownstate. Please check the time models or define a distinct transport resource breakdown state called {BreakdownStateNamingConvention.TRANSPORT_RESOURCE_BREAKDOWN_STATE}.")
-        transport_resource_breakdown_state = transport_resource_breakdown_states[0].copy(deep=True)
+        transport_resource_breakdown_state = transport_resource_breakdown_states[0].model_copy(deep=True)
         transport_resource_breakdown_state.ID = BreakdownStateNamingConvention.TRANSPORT_RESOURCE_BREAKDOWN_STATE
         adapter_object.state_data.append(transport_resource_breakdown_state)
         logger.info(f"Added default breakdown state for transport resources to the production system.")
     # TODO: add later logic for adding breakdown states for process modules automatically again if problems with process id reworked
     # if process_breakdown_states and not check_breakdown_state_available(adapter_object, BreakdownStateNamingConvention.PROCESS_MODULE_BREAKDOWN_STATE):
     #     if not check_states_for_heterogenous_time_models(process_breakdown_states, adapter_object):
     #         raise ValueError(f"The process breakdown states are not heterogenous and it is not ambiguous which state should be the Breakdownstate. Please check the time models or define a distinct process breakdown state called {BreakdownStateNamingConvention.PROCESS_MODULE_BREAKDOWN_STATE}.")
-    #     process_breakdown_state = process_breakdown_states[0].copy()
+    #     process_breakdown_state = process_breakdown_states[0].model_copy()
     #     process_breakdown_state.ID = BreakdownStateNamingConvention.PROCESS_MODULE_BREAKDOWN_STATE
     #     adapter_object.state_data.append(process_breakdown_state)
     #     logger.info(f"Added default breakdown state for process modules to the production system.")
 
 def clean_out_breakdown_states_of_resources(
     adapter_object: adapters.ProductionSystemAdapter,
 ):
@@ -847,15 +847,15 @@
 
     Returns:
         adapters.ProductionSystemAdapter: Random configuration based on a baseline configuration.
     """
     transformations = baseline.scenario_data.options.transformations
     invalid_configuration_counter = 0
     while True:
-        adapter_object = baseline.copy(deep=True)
+        adapter_object = baseline.model_copy(deep=True)
         adapter_object.ID = str(uuid1())
 
         if scenario_data.ReconfigurationEnum.PRODUCTION_CAPACITY in transformations:
             get_random_production_capacity(adapter_object)
         if scenario_data.ReconfigurationEnum.TRANSPORT_CAPACITY in transformations:
             get_random_transport_capacity(adapter_object)
         if (
@@ -1014,15 +1014,15 @@
 
     if adapter_object.hash() not in solution_dict["hashes"]:
         solution_dict["hashes"][adapter_object.hash()] = {
             "generation": current_generation,
             "ID": adapter_object.ID,
         }
 
-    adapters.JsonProductionSystemAdapter(**adapter_object.dict()).write_data(
+    adapters.JsonProductionSystemAdapter(**adapter_object.model_dump()).write_data(
         f"{save_folder}/generation_{current_generation}_{adapter_object.ID}.json"
     )
 
 
 def evaluate(
     base_scenario: adapters.ProductionSystemAdapter,
     solution_dict: Dict[str, Union[list, str]],
```

### Comparing `prodsys-0.6.5/prodsys/optimization/simulated_annealing.py` & `prodsys-0.7.0/prodsys/optimization/simulated_annealing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
 import time
 from copy import deepcopy
 from numpy import full
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 import logging
+
 logger = logging.getLogger(__name__)
 
 from simanneal import Annealer
 
 from prodsys.simulation import sim
 from prodsys import adapters
 from prodsys.optimization.optimization_util import (
     check_valid_configuration,
     evaluate,
     mutation,
     document_individual,
     get_weights,
     check_breakdown_states_available,
-    create_default_breakdown_states
+    create_default_breakdown_states,
 )
 from prodsys.util.util import set_seed
 
 sim.VERBOSE = 0
 
 
 class ProductionSystemOptimization(Annealer):
@@ -32,15 +33,15 @@
         save_folder: str,
         performances: dict,
         solutions_dict: dict,
         start: float,
         weights: tuple,
         number_of_seeds: int = 1,
         initial_solution: adapters.ProductionSystemAdapter = None,
-        full_save: bool = False
+        full_save: bool = False,
     ):
         super().__init__(initial_solution, None)
         self.save_folder = save_folder
         self.base_configuration = base_configuration
         self.performances = performances
         self.solution_dict = solutions_dict
         self.start = start
@@ -80,45 +81,48 @@
             "time_stamp": time.perf_counter() - self.start,
             "hash": self.state.hash(),
         }
         with open(f"{self.save_folder}/optimization_results.json", "w") as json_file:
             json.dump(self.performances, json_file)
 
         return performance
-    
+
+
 class SimulatedAnnealingHyperparameters(BaseModel):
     """
     Hyperparameters to perform a configuration optimization with simulated annealing.
     Args:
         seed (int): Seed for random number generator
         Tmax (int): Maximum temperature
         Tmin (int): Minimum temperature
         steps (int): Number of steps
         updates (int): Number of updates
     """
+
     seed: int = 0
     Tmax: int = 10000
     Tmin: int = 1
     steps: int = 4000
     updates: int = 300
     number_of_seeds: int = 1
 
-    class Config:
-        schema_extra = {
-            "examples": [ 
-            {
+    model_config = ConfigDict(
+        json_schema_extra={
+            "examples": [
+                {
                     "seed": 0,
                     "Tmax": 10000,
                     "Tmin": 1,
                     "steps": 4000,
                     "updates": 300,
                     "number_of_seeds": 1,
                 },
             ]
         }
+    )
 
 
 def run_simulated_annealing(
     save_folder: str,
     base_configuration_file_path: str,
     scenario_file_path: str,
     full_save: bool,
@@ -153,78 +157,79 @@
 
     if initial_solution_file_path:
         initial_solution = adapters.JsonProductionSystemAdapter()
         initial_solution.read_data(initial_solution_file_path, scenario_file_path)
         if not initial_solution.ID:
             initial_solution.ID = "initial_solution"
     else:
-        initial_solution = base_configuration.copy(deep=True)
+        initial_solution = base_configuration.model_copy(deep=True)
 
     hyper_parameters = SimulatedAnnealingHyperparameters(
-        seed=seed, Tmax=Tmax, Tmin=Tmin, steps=steps, updates=updates, number_of_seeds=number_of_seeds)
+        seed=seed,
+        Tmax=Tmax,
+        Tmin=Tmin,
+        steps=steps,
+        updates=updates,
+        number_of_seeds=number_of_seeds,
+    )
 
     simulated_annealing_optimization(
         base_configuration=base_configuration,
         hyper_parameters=hyper_parameters,
         save_folder=save_folder,
         initial_solution=initial_solution,
-        full_save = full_save        
+        full_save=full_save,
     )
 
 
-
-
-
 def simulated_annealing_optimization(
     base_configuration: adapters.ProductionSystemAdapter,
     hyper_parameters: SimulatedAnnealingHyperparameters,
-    save_folder: str="results",
+    save_folder: str = "results",
     initial_solution: adapters.ProductionSystemAdapter = None,
-    full_save: bool = False
+    full_save: bool = False,
 ):
     """
     Optimize a production system configuration using simulated anealing.
 
     Args:
         base_configuration (adapters.ProductionSystemAdapter): production system to optimize.
         hyper_parameters (SimulatedAnnealingHyperparameters): Hyperparameters for simulated annealing.
         save_folder (str): Folder to save the results in. Defaults to "results".
         initial_solution (adapters.ProductionSystemAdapter, optional): Initial solution for optimization. Defaults to None.
     """
-    adapters.ProductionSystemAdapter.Config.validate = False
-    adapters.ProductionSystemAdapter.Config.validate_assignment = False
+    adapters.ProductionSystemAdapter.model_config["validate_assignment"] = False
     if not adapters.check_for_clean_compound_processes(base_configuration):
-        logger.warning("Both compound processes and normal processes are used. This may lead to unexpected results.")
+        logger.warning(
+            "Both compound processes and normal processes are used. This may lead to unexpected results."
+        )
     if not check_breakdown_states_available(base_configuration):
         create_default_breakdown_states(base_configuration)
     if not initial_solution:
-        initial_solution = base_configuration.copy(deep=True)
+        initial_solution = base_configuration.model_copy(deep=True)
 
     set_seed(hyper_parameters.seed)
 
     weights = get_weights(base_configuration, "min")
 
-    solution_dict = {
-        "current_generation": "0", 
-        "hashes": {} 
-    }
+    solution_dict = {"current_generation": "0", "hashes": {}}
     performances = {}
     performances["0"] = {}
     start = time.perf_counter()
 
     pso = ProductionSystemOptimization(
         base_configuration=base_configuration,
         save_folder=save_folder,
         performances=performances,
         solutions_dict=solution_dict,
         start=start,
         weights=weights,
         number_of_seeds=hyper_parameters.number_of_seeds,
         initial_solution=initial_solution,
-        full_save = full_save
+        full_save=full_save,
     )
 
     pso.Tmax = hyper_parameters.Tmax
     pso.Tmin = hyper_parameters.Tmin
     pso.steps = hyper_parameters.steps
     pso.updates = hyper_parameters.updates
 
@@ -232,15 +237,15 @@
 
 
 def optimize_configuration(
     base_configuration_file_path: str,
     scenario_file_path: str,
     save_folder: str,
     hyper_parameters: SimulatedAnnealingHyperparameters,
-    full_save: bool = False
+    full_save: bool = False,
 ):
     """
     Optimize a configuration with simulated annealing.
 
     Args:
         base_configuration_file_path (str): File path of the serialized base configuration (`prodsys.adapters.JsonProductionSystemAdapter`)
         scenario_file_path (str): File path of the serialized scenario (`prodsys.models.scenario_data.ScenarioData`)
@@ -254,9 +259,9 @@
         scenario_file_path=scenario_file_path,
         seed=hyper_parameters.seed,
         Tmax=hyper_parameters.Tmax,
         Tmin=hyper_parameters.Tmin,
         steps=hyper_parameters.steps,
         updates=hyper_parameters.updates,
         number_of_seeds=hyper_parameters.number_of_seeds,
-        full_save=full_save
+        full_save=full_save,
     )
```

### Comparing `prodsys-0.6.5/prodsys/optimization/tabu_search.py` & `prodsys-0.7.0/prodsys/optimization/tabu_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import logging
 logger = logging.getLogger(__name__)
 
 import json
 import time
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from prodsys.simulation import sim
 from prodsys import adapters
 from prodsys.optimization.optimization_util import (
     check_valid_configuration,
     crossover,
     evaluate,
@@ -147,26 +147,25 @@
 
     seed: int = 0
     tabu_size: int = 10
     max_steps: int = 300
     max_score: float = 500
     number_of_seeds: int = 1
 
-    class Config:
-        schema_extra = {
-            "examples": [
-                 {
-                    "seed": 0,
-                    "tabu_size": 10,
-                    "max_steps": 300,
-                    "max_score": 500,
-                    "number_of_seeds": 1,
-                },
-            ]
-        }
+    model_config=ConfigDict(json_schema_extra={
+        "examples": [
+            {
+                "seed": 0,
+                "tabu_size": 10,
+                "max_steps": 300,
+                "max_score": 500,
+                "number_of_seeds": 1,
+            },
+        ]
+    })
 
 
 def run_tabu_search(
     save_folder: str,
     base_configuration_file_path: str,
     scenario_file_path: str,
     seed: int,
@@ -198,15 +197,15 @@
 
     if initial_solution_file_path:
         initial_solution = adapters.JsonProductionSystemAdapter()
         initial_solution.read_data(initial_solution_file_path, scenario_file_path)
         if not initial_solution.ID:
             initial_solution.ID = "initial_solution"
     else:
-        initial_solution = base_configuration.copy(deep=True)
+        initial_solution = base_configuration.model_copy(deep=True)
 
     hyper_parameters = TabuSearchHyperparameters(
         seed=seed, tabu_size=tabu_size, max_steps=max_steps, max_score=max_score, number_of_seeds=number_of_seeds
     )
     tabu_search_optimization(
         base_configuration=base_configuration,
         hyper_parameters=hyper_parameters,
```

### Comparing `prodsys-0.6.5/prodsys/simulation/__init__.py` & `prodsys-0.7.0/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/simulation/control.py` & `prodsys-0.7.0/prodsys/simulation/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Callable
-from pydantic import BaseModel, Field, validator, Extra
-from typing import Any, List, Generator, TYPE_CHECKING, Union, Optional
+from pydantic import BaseModel, ConfigDict, Field, field_validator, ValidationInfo
+from typing import List, Generator, TYPE_CHECKING, Optional
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 # from process import Process
 from simpy import events
 
-from prodsys.simulation import node, request, route_finder, sim, state, process
-
-from prodsys.simulation.process import LinkTransportProcess, RequiredCapabilityProcess
 
 if TYPE_CHECKING:
-    from prodsys.simulation import product, process, state, resources, request, sink, source
+    from prodsys.simulation import product, process, state, resources, sink, source
+    from prodsys.simulation import request as request_module
     from prodsys.control import sequencing_control_env
     from prodsys.simulation.product import Locatable
 
 
-
 class Controller(ABC, BaseModel):
     """
     A controller is responsible for controlling the processes of a resource. The controller is requested by products requiring processes. The controller decides has a control policy that determines with which sequence requests are processed.
 
     Args:
-        control_policy (Callable[[List[request.Request]], None]): The control policy that determines the sequence of requests to be processed.
+        control_policy (Callable[[List[Request]], None]): The control policy that determines the sequence of requests to be processed.
         env (sim.Environment): The environment in which the controller is running.
 
     Attributes:
         resource (resources.Resource): The resource that is controlled by the controller.
         requested (events.Event): An event that is triggered when a request is made to the controller.
-        requests (List[request.Request]): A list of requests that are made to the controller.
+        requests (List[Request]): A list of requests that are made to the controller.
         running_processes (List[events.Event]): A list of (simpy) processes that are currently running on the resource.
     """
 
     control_policy: Callable[
         [
-            List[request.Request],
+            List[request_module.Request],
         ],
         None,
     ]
     env: sim.Environment
 
     resource: resources.Resource = Field(init=False, default=None)
-    requested: events.Event = Field(init=False, default=None)
-    requests: List[request.Request] = Field(init=False, default_factory=list)
+    requested: events.Event = Field(init=False, validate_default=True, default=None)
+    requests: List[request_module.Request] = Field(init=False, default_factory=list)
     running_processes: List[events.Process] = []
     reserved_requests_count: int = 0
 
-    @validator("requested", pre=True, always=True)
-    def init_requested(cls, v, values):
-        return events.Event(values["env"])
-
-    class Config:
-        arbitrary_types_allowed = True
-        extra = Extra.allow
+    @field_validator("requested", mode="before")
+    def init_requested(cls, v, info: ValidationInfo):
+        event = events.Event(info.data["env"])
+        return event
+
+    model_config=ConfigDict(arbitrary_types_allowed=True, extra="allow")
 
     def set_resource(self, resource: resources.Resource) -> None:
         self.resource = resource
         self.env = resource.env
 
-    def request(self, process_request: request.Request) -> None:
+    def request(self, process_request: request_module.Request) -> None:
         """
         Request the controller consider the request in the future for processing.
 
         Args:
-            process_request (request.Request): The request to be processed.
+            process_request (Request): The request to be processed.
         """
         self.requests.append(process_request)
         logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": f"Got requested by {process_request.product.product_data.ID}"})
         if not self.requested.triggered:
             logger.debug({"ID": "controller", "sim_time": self.env.now, "resource": self.resource.data.ID, "event": "Triggered requested event"})
             self.requested.succeed()
 
@@ -290,22 +286,22 @@
 
 
 class TransportController(Controller):
     """
     Controller for transport resources.
     """
     resource: resources.TransportResource = Field(init=False, default=None)
-    requests: List[request.TransportResquest] = Field(default_factory=list)
+    requests: List[request_module.TransportResquest] = Field(default_factory=list)
     control_policy: Callable[
         [
-            List[request.TransportResquest],
+            List[request_module.TransportResquest],
         ],
         None,
     ]
-    _current_locatable: Optional[product.Locatable] = Field(init=False, default=None)
+    _current_locatable: Optional[product.Locatable] = None
 
     def get_next_product_for_process(
         self, resource: product.Locatable, product: product.Product
     ) -> List[events.Event]:
         """
         Get the next product for a process from the input queue of a resource.
 
@@ -539,15 +535,15 @@
         )
        
         input_state.process = self.env.process(
             input_state.process_state(target=target_location, initial_transport_step=initial_transport_step, last_transport_step=last_transport_step)  # type: ignore False
         )
         yield input_state.process
 
-    def find_route_to_origin(self, process_request: request.TransportResquest) -> List[product.Locatable]:
+    def find_route_to_origin(self, process_request: request_module.TransportResquest) -> List[product.Locatable]:
         """
         Find the route to the origin of the transport request.
 
         Args:
             process_request (request.TransportResquest): The transport request.
 
         Returns:
@@ -558,72 +554,72 @@
             if not route_to_origin:
                 raise ValueError(f"Route to origin for transport of {process_request.product.product_data.ID} could not be found. Router selected a transport resource that can perform the transport but does not reach the origin.")
             return route_to_origin
         else:
             return [self._current_locatable, process_request.get_origin()]
 
 
-def FIFO_control_policy(requests: List[request.Request]) -> None:
+def FIFO_control_policy(requests: List[request_module.Request]) -> None:
     """
     Sort the requests according to the FIFO principle.
 
     Args:
-        requests (List[request.Request]): The list of requests.
+        requests (List[Request]): The list of requests.
     """
     pass
 
 
-def LIFO_control_policy(requests: List[request.Request]) -> None:
+def LIFO_control_policy(requests: List[request_module.Request]) -> None:
     """
     Sort the requests according to the LIFO principle (reverse the list).
 
     Args:
-        requests (List[request.Request]): The list of requests.
+        requests (List[Request]): The list of requests.
     """
     requests.reverse()
 
 
-def SPT_control_policy(requests: List[request.Request]) -> None:
+def SPT_control_policy(requests: List[request_module.Request]) -> None:
     """
     Sort the requests according to the SPT principle (shortest process time first).
 
     Args:
-        requests (List[request.Request]): The list of requests.
+        requests (List[Request]): The list of requests.
     """
     requests.sort(key=lambda x: x.process.get_expected_process_time())
 
 
-def SPT_transport_control_policy(requests: List[request.TransportResquest]) -> None:
+def SPT_transport_control_policy(requests: List[request_module.TransportResquest]) -> None:
     """
     Sort the requests according to the SPT principle (shortest process time first).
 
     Args:
         requests (List[request.TransportResquest]): The list of requests.
     """
     requests.sort(
         key=lambda x: x.process.get_expected_process_time(
             x.origin.get_location(), x.target.get_location()
         )
     )
-def nearest_origin_and_longest_target_queues_transport_control_policy(requests: List[request.TransportResquest]) -> None:
+def nearest_origin_and_longest_target_queues_transport_control_policy(requests: List[request_module.TransportResquest]) -> None:
     """
     Sort the requests according to nearest origin without considering the target location. 
     Second order sorting by descending length of the target output queues, to prefer targets where a product can be picked up.
     Args:
         requests (List[request.TransportResquest]): The list of requests.
     """
     requests.sort(
         key=lambda x: (
             x.process.get_expected_process_time(
                 x.resource.data.location, x.origin.get_location()),
                 - x.target.get_output_queue_length()
                 )
     )
 
-def nearest_origin_and_shortest_target_input_queues_transport_control_policy(requests: List[request.TransportResquest]) -> None:
+def nearest_origin_and_shortest_target_input_queues_transport_control_policy(requests: List[request_module.TransportResquest]) -> None:
     """
     Sort the requests according to nearest origin without considering the target location.
     Second order sorting by ascending length of the target input queue so that resources with empty input queues get material to process.
 
     Args:
         requests (List[request.TransportResquest]): The list of requests.
     """
@@ -632,31 +628,29 @@
             x.process.get_expected_process_time(
                 x.resource.data.location, x.origin.get_location()),
             x.target.get_input_queue_length()
             )
     )
 
 def agent_control_policy(
-    gym_env: sequencing_control_env.AbstractSequencingControlEnv, requests: List[request.Request]
+    gym_env: sequencing_control_env.AbstractSequencingControlEnv, requests: List[request_module.Request]
 ) -> None:
     """
     Sort the requests according to the agent's policy.
 
     Args:
         gym_env (gym_env.ProductionControlEnv): A gym environment, where the agent can interact with the simulation.
-        requests (List[request.Request]): The list of requests.
+        requests (List[Request]): The list of requests.
     """
     gym_env.interrupt_simulation_event.succeed()
 
 
 class BatchController(Controller):
     """
     A controller that processes the requests in batches.
     """
     pass
 
 
-from prodsys.simulation import resources, source, sink
-
-Controller.update_forward_refs()
-ProductionController.update_forward_refs()
-TransportController.update_forward_refs()
+from prodsys.simulation import resources, state, sink, source, route_finder, sim
+from prodsys.simulation import request as request_module
+from prodsys.simulation.process import LinkTransportProcess
```

### Comparing `prodsys-0.6.5/prodsys/simulation/logger.py` & `prodsys-0.7.0/prodsys/simulation/logger.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/simulation/observer.py` & `prodsys-0.7.0/prodsys/simulation/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,8 +93,7 @@
         return observe_output_queue(self.resource, self.product_factory)
     
     def observe_resource_available(self) -> ResourceAvailableObservation:
         return observe_resource_available(self.resource)
     
 from prodsys.factories import resource_factory, product_factory
 from prodsys.simulation import resources, state
-ResourceObserver.update_forward_refs()
```

### Comparing `prodsys-0.6.5/prodsys/simulation/proces_models.py` & `prodsys-0.7.0/prodsys/simulation/proces_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,106 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List, Optional, Dict
+from typing import TYPE_CHECKING, List, Optional, Dict
 import random
 from pydantic import BaseModel, Field
 
-from prodsys.simulation import process
 from prodsys.util.util import flatten
 
+if TYPE_CHECKING:
+    from prodsys.simulation.process import PROCESS_UNION
+
 
 class ProcessModel(ABC, BaseModel):
     """
     Abstract process model base class that defines the interface for all process models.
     """
 
     @abstractmethod
-    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
+    def get_next_possible_processes(self) -> Optional[List[PROCESS_UNION]]:
         """
         Returns the next possible processes.
 
         Returns:
-            Optional[List[process.PROCESS_UNION]]: List of possible processes.
+            Optional[List[PROCESS_UNION]]: List of possible processes.
         """
         pass
 
     @abstractmethod
     def update_marking_from_transition(
-        self, chosen_process: process.PROCESS_UNION
+        self, chosen_process: PROCESS_UNION
     ) -> None:
         """
         Updates the marking of the process model based on the chosen process.
 
         Args:
-            chosen_process (process.PROCESS_UNION): The chosen process that is executed.
+            chosen_process (PROCESS_UNION): The chosen process that is executed.
         """
         pass
 
 
 class ListProcessModel(ProcessModel):
     """
     Process model that is based on a list of processes. The processes are executed sequentially in the order of the list.
 
     Args:
-        process_list (List[process.PROCESS_UNION]): List of processes that are executed sequentially.
+        process_list (List[PROCESS_UNION]): List of processes that are executed sequentially.
     """
 
-    process_list: List[process.PROCESS_UNION]
+    process_list: List[PROCESS_UNION]
     current_marking: int = Field(default=0, init=False)
 
-    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
+    def get_next_possible_processes(self) -> Optional[List[PROCESS_UNION]]:
         if self.current_marking == len(self.process_list):
             return None
         return [self.process_list[self.current_marking]]
 
     def update_marking_from_transition(
-        self, chosen_process: process.PROCESS_UNION
+        self, chosen_process: PROCESS_UNION
     ) -> None:
         self.current_marking += 1
 
 class PrecendeGraphNode(BaseModel):
     """
     Class that represents a node in a precedence graph.
 
     Args:
-        process (process.PROCESS_UNION): The process that is represented by the node.
+        process (PROCESS_UNION): The process that is represented by the node.
         successors (Optional[List[PrecendeGraphNode]]): List of successor nodes.
         predecessors (Optional[List[PrecendeGraphNode]]): List of predecessor nodes.
 
     Attributes:
         marking (bool): Indicates if the node is marked.
     """
 
-    process: process.PROCESS_UNION
+    process: PROCESS_UNION
     successors: Optional[List[PrecendeGraphNode]] = []
     predecessors: Optional[List[PrecendeGraphNode]] = []
     marking: bool = Field(default=False, init=False)
 
     def update_marking(self):
         """
         Updates the marking of the node, to save that the process has been executed.
         """
         self.marking = True
 
 
 def get_predecessor_processes(
     target_process_id: str, adjacency_matrix: Dict[str, List[str]]
-) -> List[process.PROCESS_UNION]:
+) -> List[PROCESS_UNION]:
     """
     Returns the predecessing processes' IDs of a ID of a process.
 
     Args:
         target_process_id (str): process ID of the process for which the predecessing processes' IDs are returned.
         adjacency_matrix (Dict[str, List[str]]): Adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the successor processes.
 
     Returns:
-        List[process.PROCESS_UNION]: List of predecessing processes' IDs.
+        List[PROCESS_UNION]: List of predecessing processes' IDs.
     """
     predecessors = []
     for process_id, successors in adjacency_matrix.items():
         if target_process_id in successors:
             predecessors.append(process_id)
     return predecessors
 
@@ -147,15 +149,15 @@
 
     Attributes:
         nodes (List[PrecendeGraphNode]): List of nodes in the precedence graph.
         current_marking (Optional[PrecendeGraphNode]): The current marking, i.e. the node that represents the previously executed process, of the process model.
     """
 
     nodes: List[PrecendeGraphNode] = Field(default_factory=list, init=False)
-    current_marking: Optional[PrecendeGraphNode] = Field(init=False)
+    current_marking: Optional[PrecendeGraphNode] = Field(init=False, default=None)
 
     def __str__(self) -> str:
         """
         Returns a string representation of the adjacency matrix of the process model.
 
         Returns:
             str: String representation of the adjacency matrix of the process model.
@@ -178,27 +180,27 @@
         for node in self.nodes:
             if not node.predecessors:
                 possible_starts.append(node)
         if not possible_starts:
             raise ValueError("No initial marking found")
         self.current_marking = random.choice(possible_starts)
 
-    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
+    def get_next_possible_processes(self) -> Optional[List[PROCESS_UNION]]:
         if not self.current_marking:
             self.set_initial_marking()
         possible_processes = [
             node.process
             for node in self.nodes
             if not node.marking
             and (not node.predecessors or all(n.marking for n in node.predecessors))
         ]
         return possible_processes
 
     def update_marking_from_transition(
-        self, chosen_process: process.PROCESS_UNION
+        self, chosen_process: PROCESS_UNION
     ) -> None:
         chosen_node = [
             node for node in self.nodes if node.process == chosen_process
         ].pop()
         chosen_node.update_marking()
         self.current_marking = chosen_node
 
@@ -209,25 +211,25 @@
         Returns:
             List[str]: List of process IDs of all nodes in the process model.
         """
         return [node.process.process_data.ID for node in self.nodes]
 
     def add_node(
         self,
-        process: process.PROCESS_UNION,
-        successors: List[process.PROCESS_UNION],
-        predecessors: List[process.PROCESS_UNION],
+        process: PROCESS_UNION,
+        successors: List[PROCESS_UNION],
+        predecessors: List[PROCESS_UNION],
     ) -> None:
         """
         Adds a node to the process model. If the processes of the successors and predecessors are not in the process model, they are added as well, with for now empty lists of successors and predecessors.
 
         Args:
-            process (process.PROCESS_UNION): Process that is represented by the node.
-            successors (List[process.PROCESS_UNION]): List of successor processes.
-            predecessors (List[process.PROCESS_UNION]): List of predecessor processes.
+            process (PROCESS_UNION): Process that is represented by the node.
+            successors (List[PROCESS_UNION]): List of successor processes.
+            predecessors (List[PROCESS_UNION]): List of predecessor processes.
         """
         if not process.process_data.ID in self.get_node_process_ids():
             node = PrecendeGraphNode(process=process, successors=[], predecessors=[])
             self.nodes.append(node)
         else:
             node = [node for node in self.nodes if node.process == process].pop()
 
@@ -246,7 +248,9 @@
             if predecessor.process_data.ID not in self.get_node_process_ids():
                 self.add_node(predecessor, [], [])
             predecessor_nodes.append(
                 [node for node in self.nodes if node.process == predecessor].pop()
             )
 
         node.predecessors = predecessor_nodes
+
+from prodsys.simulation.process import PROCESS_UNION
```

### Comparing `prodsys-0.6.5/prodsys/simulation/process.py` & `prodsys-0.7.0/prodsys/simulation/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Union, List, Optional
 
-from numpy import isin
 from pydantic import BaseModel
 
 
-if TYPE_CHECKING:
-    from prodsys.simulation import resources, source, sink, node
 
-from prodsys.simulation import route_finder, time_model, request
+if TYPE_CHECKING:
+    from prodsys.simulation.resources import ProductionResource, TransportResource
+    from prodsys.simulation.source import Source
+    from prodsys.simulation.sink import Sink
+    from prodsys.simulation.node import Node
+    from prodsys.simulation import request
+from prodsys.simulation import route_finder, time_model
 
 from prodsys.models import processes_data
 
 
 class Process(ABC, BaseModel):
     """
     Abstract process base class that defines the interface for all processes.
@@ -140,27 +143,27 @@
 
     def get_process_time(self, origin: List[float], target: List[float]) -> float:
         return self.time_model.get_next_time(origin=origin, target=target)
 
     def get_expected_process_time(self, *args) -> float:
         return self.time_model.get_expected_time(*args)
     
-def is_process_with_capability(process: PROCESS_UNION) -> bool:
+def is_process_with_capability(process: "PROCESS_UNION") -> bool:
     """
     Returns True if the given process is a process with capability.
 
     Args:
         process (PROCESS_UNION): The process.
 
     Returns:
         bool: True if the given process is a process with capability.
     """
     return isinstance(process, CapabilityProcess) or isinstance(process, RequiredCapabilityProcess) or (isinstance(process, LinkTransportProcess) and process.process_data.capability)
 
-def is_available_process_with_capability(process: PROCESS_UNION) -> bool:
+def is_available_process_with_capability(process: "PROCESS_UNION") -> bool:
     """
     Returns True if the given process is an available process with capability.
 
     Args:
         process (PROCESS_UNION): The process.
 
     Returns:
@@ -246,15 +249,15 @@
         )
 
 class LinkTransportProcess(TransportProcess):
     """
     Class that represents a transport link process.
     """
     process_data: processes_data.LinkTransportProcessData
-    links: Optional[List[List[Union[node.Node, source.Source, sink.Sink, resources.ProductionResource]]]]
+    links: Optional[List[List[Union[Node, Source, Sink, ProductionResource]]]]
 
     def matches_request(self, request: request.TransportResquest) -> bool:
         requested_process = request.process
 
         if not isinstance(requested_process, LinkTransportProcess) and not isinstance(requested_process, RequiredCapabilityProcess) and not isinstance(
             requested_process, CompoundProcess
         ):
@@ -305,9 +308,13 @@
     TransportProcess,
     CapabilityProcess,
     LinkTransportProcess,
 ]
 """
 Union type for all processes.
 """
-from prodsys.simulation import resources, source, sink, node
-LinkTransportProcess.update_forward_refs()
+from prodsys.simulation.resources import ProductionResource, TransportResource
+from prodsys.simulation.source import Source
+from prodsys.simulation.sink import Sink
+from prodsys.simulation.node import Node
+from prodsys.simulation import request
+# LinkTransportProcess.model_rebuild()
```

### Comparing `prodsys-0.6.5/prodsys/simulation/product.py` & `prodsys-0.7.0/prodsys/simulation/product.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-from __future__ import annotations
+from typing import Union, Optional, Generator
 
-from abc import ABC
-from enum import Enum
-from collections.abc import Iterable
-from typing import List, Union, Optional, TYPE_CHECKING, Generator
-
-from pydantic import BaseModel, Field, Extra
+from pydantic import BaseModel, ConfigDict, Field
 
 import logging
 logger = logging.getLogger(__name__)
 
 import numpy as np
 from simpy import events
 
+from prodsys.models import product_data
+
 from prodsys.simulation import (
-    process,
     request,
+    process,
     router,
     resources,
     sim,
     sink,
     source,
     proces_models,
-    state,
     node
 )
+from prodsys.simulation.state import StateTypeEnum, StateEnum
 
-from prodsys.models import product_data
-
-
-class ProductInfo(BaseModel, extra=Extra.allow):
+class ProductInfo(BaseModel):
     """
     Class that represents information of the current state of a product.
 
     Args:
         resource_ID (str): ID of the resource that the product is currently at.
         state_ID (str): ID of the state that the product is currently at.
         event_time (float): Time of the event.
@@ -41,104 +35,106 @@
         product_ID (str): ID of the product.
         state_type (state.StateTypeEnum): Type of the state.
     """
 
     resource_ID: str = Field(init=False, default=None)
     state_ID: str = Field(init=False, default=None)
     event_time: float = Field(init=False, default=None)
-    activity: state.StateEnum = Field(init=False, default=None)
+    activity: StateEnum = Field(init=False, default=None)
     product_ID: str = Field(init=False, default=None)
-    state_type: state.StateTypeEnum = Field(init=False, default=None)
+    state_type: StateTypeEnum = Field(init=False, default=None)
+
+    model_config=ConfigDict(extra="allow")
 
     def log_finish_product(
         self,
         resource: Union[resources.Resource, sink.Sink, source.Source],
-        _product: Product,
+        _product: "Product",
         event_time: float,
     ):
         """
         Logs the finish of a product.
 
         Args:
             resource (Union[resources.Resource, sink.Sink, source.Source]): New resource of the product.
             _product (Product): Product that is finished.
             event_time (float): Time of the event.
         """
         self.resource_ID = resource.data.ID
         self.state_ID = resource.data.ID
         self.event_time = event_time
         self.product_ID = _product.product_data.ID
-        self.activity = state.StateEnum.finished_product
-        self.state_type = state.StateTypeEnum.sink
+        self.activity = StateEnum.finished_product
+        self.state_type = StateTypeEnum.sink
 
     def log_create_product(
         self,
         resource: Union[resources.Resource, sink.Sink, source.Source],
-        _product: Product,
+        _product: "Product",
         event_time: float,
     ) -> None:
         """
         Logs the creation of a product.
 
         Args:
             resource (Union[resources.Resource, sink.Sink, source.Source]): New resource of the product.
             _product (Product): Product that is created.
             event_time (float): Time of the event.
         """
         self.resource_ID = resource.data.ID
         self.state_ID = resource.data.ID
         self.event_time = event_time
         self.product_ID = _product.product_data.ID
-        self.activity = state.StateEnum.created_product
-        self.state_type = state.StateTypeEnum.source
+        self.activity = StateEnum.created_product
+        self.state_type = StateTypeEnum.source
 
     def log_start_process(
         self,
         resource: resources.Resource,
-        _product: Product,
+        _product: "Product",
         event_time: float,
-        state_type: state.StateTypeEnum,
+        state_type: StateTypeEnum,
     ) -> None:
         """
         Logs the start of a process.
 
         Args:
             resource (resources.Resource): Resource that the product is processed at.
             _product (Product): Product that is processed.
             event_time (float): Time of the event.
             state_type (state.StateTypeEnum): Type of the state.
         """
         self.resource_ID = resource.data.ID
         self.state_ID = resource.data.ID
         self.event_time = event_time
         self.product_ID = _product.product_data.ID
-        self.activity = state.StateEnum.start_state
+        self.activity = StateEnum.start_state
         self.state_type = state_type
 
     def log_end_process(
         self,
         resource: resources.Resource,
-        _product: Product,
+        _product: "Product",
         event_time: float,
-        state_type: state.StateTypeEnum,
+        state_type: StateTypeEnum,
     ) -> None:
         """
         Logs the end of a process.
 
         Args:
             resource (resources.Resource): Resource that the product is processed at.
             _product (Product): Product that is processed.
             event_time (float): Time of the event.
             state_type (state.StateTypeEnum): Type of the state.
         """
         self.resource_ID = resource.data.ID
         self.state_ID = resource.data.ID
         self.event_time = event_time
         self.product_ID = _product.product_data.ID
-        self.activity = state.StateEnum.end_state
+        self.activity = StateEnum.end_state
         self.state_type = state_type
 
 Locatable= Union[resources.Resource, node.Node, source.Source, sink.Sink]
 
 class Product(BaseModel):
     """
     Class that represents a product in the discrete event simulation. For easier instantion of the class, use the ProductFactory at prodsys.factories.product_factory.
@@ -150,25 +146,24 @@
         transport_process (process.Process): Transport process that represents the required transport processes.
         product_router (router.Router): Router that is used to route the product object.
     """
 
     env: sim.Environment
     product_data: product_data.ProductData
     process_model: proces_models.ProcessModel
-    transport_process: Union[process.LinkTransportProcess, process.TransportProcess, process.RequiredCapabilityProcess]
+    transport_process: Union[process.TransportProcess, process.RequiredCapabilityProcess, process.LinkTransportProcess]
     product_router: router.Router
 
     next_prodution_process: Optional[process.PROCESS_UNION] = Field(default=None, init=False)
     process: events.Process = Field(default=None, init=False)
     current_locatable: Locatable = Field(default=None, init=False)
     finished_process: events.Event = Field(default=None, init=False)
-    product_info: ProductInfo = ProductInfo()
+    product_info: ProductInfo = Field(default_factory=ProductInfo, init=False)
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config=ConfigDict(arbitrary_types_allowed=True)
 
     def update_location(self, resource: Locatable):
         """
         Updates the location of the product object.
 
         Args:
             resource (Locatable): Locatable objects where product object currently is.
@@ -200,17 +195,17 @@
         logger.debug({"ID": self.product_data.ID, "sim_time": self.env.now, "event": f"Finished processing of product"})
 
     def request_process(self, processing_request: request.Request) -> Generator:
         """
         Requests the next production process of the product object from the next production resource by creating a request event and registering it at the environment.
         """
         if isinstance(processing_request, request.TransportResquest):
-            type_ = state.StateTypeEnum.transport
+            type_ = StateTypeEnum.transport
         else:
-            type_ = state.StateTypeEnum.production
+            type_ = StateTypeEnum.production
         logger.debug({"ID": self.product_data.ID, "sim_time": self.env.now, "resource": processing_request.resource.data.ID, "event": f"Request process {processing_request.process.process_data.ID} for {type_}"})
         self.env.request_process_of_resource(
             request=processing_request
         )
         yield self.finished_process
         logger.debug({"ID": self.product_data.ID, "sim_time": self.env.now, "resource": processing_request.resource.data.ID, "event": f"Finished process {processing_request.process.process_data.ID} for {type_}"})
         self.product_info.log_end_process(
```

### Comparing `prodsys-0.6.5/prodsys/simulation/request.py` & `prodsys-0.7.0/prodsys/simulation/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional, List, Tuple, Union
 
 if TYPE_CHECKING:
-    from prodsys.simulation import product, process, resources, sink
-    from prodsys.simulation.product import Locatable
+    from prodsys.simulation.product import Product, Locatable
+    from prodsys.simulation.process import PROCESS_UNION, TransportProcess, LinkTransportProcess
+    from prodsys.simulation.resources import Resource, TransportResource
+    from prodsys.simulation.sink import Sink
 
 
 
 class Request:
     """
     Class to represents requests of a product for a process to be executed by a resource.
 
     Args:
         process (process.PROCESS_UNION): The process.
         product (product.Product): The product.
         resource (resources.Resource): The resource.
     """
     def __init__(
         self,
-        process: process.PROCESS_UNION,
-        product: product.Product,
-        resource: resources.Resource
+        process: PROCESS_UNION,
+        product: Product,
+        resource: Resource
     ):
         self.process = process
         self.product = product
         self.resource = resource
 
 
-    def set_process(self, process: process.PROCESS_UNION):
+    def set_process(self, process: PROCESS_UNION):
         """
         Sets the process of the request.
 
         Args:
             process (process.PROCESS_UNION): The process.
         """
         self.process = process
         # TODO: maybe do some special handling of compound processes here
 
 
-    def get_process(self) -> process.PROCESS_UNION:
+    def get_process(self) -> PROCESS_UNION:
         """
         Returns the process or the capability process of the request 
 
         Returns:
             process.PROCESS_UNION: The process.
         """
         return self.process
 
-    def get_product(self) -> product.Product:
+    def get_product(self) -> Product:
         """
         Returns the product of the request.
 
         Returns:
             product.Product: The product.
         """
         return self.product
 
-    def get_resource(self) -> resources.Resource:
+    def get_resource(self) -> Resource:
         """
         Returns the resource of the request.
 
         Returns:
             resources.Resource: The resource.
         """
         return self.resource
@@ -72,16 +74,16 @@
     Class to represents requests of a product for a storage in a sink to be executed by a resource.
 
     Args:
         Request (_type_): _description_
     """
     def __init__(
         self,
-        product: product.Product,
-        sink: sink.Sink
+        product: Product,
+        sink: Sink
     ):
         self.resource = sink
         self.product = product
         self.process = None
     
 
 
@@ -94,40 +96,40 @@
         product (product.Product): The product.
         resource (resources.TransportResource): The transport resource.
         origin (product.Location): The origin location, either a resource, source or sink.
         target (product.Location): The target location, either a resource, source or sink.
     """
     def __init__(
         self,
-        process: Union[process.TransportProcess, process.LinkTransportProcess],
-        product: product.Product,
-        resource: resources.TransportResource,
-        origin: product.Locatable,
-        target: product.Locatable,
+        process: Union[TransportProcess, LinkTransportProcess],
+        product: Product,
+        resource: TransportResource,
+        origin: Locatable,
+        target: Locatable,
     ):
-        self.process: Union[process.TransportProcess, process.LinkTransportProcess] = process
-        self.product: product.Product = product
-        self.resource: resources.TransportResource = resource
-        self.origin: product.Locatable = origin
-        self.target: product.Locatable = target
+        self.process: Union[TransportProcess, LinkTransportProcess] = process
+        self.product: Product = product
+        self.resource: TransportResource = resource
+        self.origin: Locatable = origin
+        self.target: Locatable = target
 
         self.route: Optional[List[Locatable]] = None
 
 
-    def set_process(self, process: process.PROCESS_UNION):
+    def set_process(self, process: PROCESS_UNION):
         """
         Sets the process of the request.
 
         Args:
             process (process.PROCESS_UNION): The process.
         """
         self.process = process
         # TODO: maybe do some special handling of compound processes here
 
-    def copy_cached_routes(self, request: TransportResquest):
+    def copy_cached_routes(self, request: "TransportResquest"):
         """
         Copies the cached routes from another transport request.
 
         Args:
             request (TransportResquest): The transport request.
         """
         self.route = request.route
@@ -138,42 +140,42 @@
 
         Args:
             process (process.TransportProcess): The process.
             route (List[product.Locatable]): The route.
         """
         self.route = route
 
-    def get_process(self) -> Union[process.TransportProcess, process.LinkTransportProcess]:
+    def get_process(self) -> Union[TransportProcess, LinkTransportProcess]:
         """
         Returns the transport process of the transport request.
 
         Returns:
             process.TransportProcess: The transport process.
         """
         return self.process
 
-    def get_resource(self) -> resources.TransportResource:
+    def get_resource(self) -> TransportResource:
         """
         Returns the transport resource of the transport request.
 
         Returns:
             resources.TransportResource: The transport resource.
         """
         return self.resource
 
-    def get_origin(self) -> product.Locatable:
+    def get_origin(self) -> Locatable:
         """
         Returns the origin location of the transport request.
 
         Returns:
             product.Locatable: The origin location.
         """
         return self.origin
 
-    def get_target(self) -> product.Locatable:
+    def get_target(self) -> Locatable:
         """
         Returns the target location of the transport request.
 
         Returns:
             product.Locatable: The target location.
         """
         return self.target
```

### Comparing `prodsys-0.6.5/prodsys/simulation/resources.py` & `prodsys-0.7.0/prodsys/simulation/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 from abc import ABC
 from typing import TYPE_CHECKING, List, Generator, Optional, Union
 
-from pydantic import BaseModel, Field, Extra
+from pydantic import BaseModel, ConfigDict, Field
 import random
 
 import logging
 logger = logging.getLogger(__name__)
 
 from simpy.resources import resource
 from simpy import events
 from prodsys.simulation import sim, store
 if TYPE_CHECKING:
-    from prodsys.simulation import process, control, state
+    from prodsys.simulation import control, state
+    from prodsys.simulation.process import PROCESS_UNION
 
 from prodsys.models.resource_data import (
     RESOURCE_DATA_UNION,
     ProductionResourceData,
     TransportResourceData,
 )
 from prodsys.util import util
@@ -25,41 +26,39 @@
 class Resource(BaseModel, ABC, resource.Resource):
     """
     Base class for all resources.
 
     Args:
         env (sim.Environment): The simpy environment.
         data (RESOURCE_DATA_UNION): The resource data.
-        processes (List[process.PROCESS_UNION]): The processes.
+        processes (List[PROCESS_UNION]): The processes.
         controller (control.Controller): The controller.
         states (List[state.State]): The states of the resource for breakdowns.
         production_states (List[state.State]): The states of the resource for production.
         setup_states (List[state.SetupState]): The states of the resource for setups.
         got_free (events.Event): The event that is triggered when the resource gets free of processes.
         active (events.Event): The event that is triggered when the resource is active.
-        current_setup (process.PROCESS_UNION): The current setup.
-        reserved_setup (process.PROCESS_UNION): The reserved setup.
+        current_setup (PROCESS_UNION): The current setup.
+        reserved_setup (PROCESS_UNION): The reserved setup.
     """
     env: sim.Environment
     data: RESOURCE_DATA_UNION
-    processes: List[process.PROCESS_UNION]
+    processes: List[PROCESS_UNION]
     controller: control.Controller
 
     states: List[state.State] = Field(default_factory=list, init=False)
     production_states: List[state.State] = Field(default_factory=list, init=False)
     setup_states: List[state.SetupState] = Field(default_factory=list, init=False)
 
     got_free: events.Event = Field(default=None, init=False)
     active: events.Event = Field(default=None, init=False)
-    current_setup: process.PROCESS_UNION = Field(default=None, init=False)
-    reserved_setup: process.PROCESS_UNION = Field(default=None, init=False)
+    current_setup: PROCESS_UNION = Field(default=None, init=False)
+    reserved_setup: PROCESS_UNION = Field(default=None, init=False)
 
-    class Config:
-        arbitrary_types_allowed = True
-        extra = Extra.allow
+    model_config=ConfigDict(arbitrary_types_allowed=True, extra="allow")
 
     @property
     def capacity_current_setup(self) -> int:
         """
         Returns the capacity of the resource for the current setup with considering that the resource could be in a setup process.
 
         Returns:
@@ -80,20 +79,20 @@
                 state
                 for state in self.production_states
                 if state.state_data.ID == current_setup_ID
             ]
         )
         return length
 
-    def reserve_setup(self, process: process.PROCESS_UNION) -> None:
+    def reserve_setup(self, process: PROCESS_UNION) -> None:
         """
         Reserves the setup of the resource for a process. This is used to prevent that capacity is wrong estimated during setup.
 
         Args:
-            process (process.PROCESS_UNION): The process that wants to reserve the setup.
+            process (PROCESS_UNION): The process that wants to reserve the setup.
         """
         self.reserved_setup = process
 
     def unreserve_setup(self) -> None:
         """
         Unreserves the setup of the resource. This is used to prevent that the resource is used for another process while it is in a setup process.
         """
@@ -164,20 +163,20 @@
         self.active = events.Event(self.env).succeed()
         self.got_free = events.Event(self.env)
         for actual_state in self.states + self.production_states + self.setup_states:
             actual_state.activate_state()
         for actual_state in self.states:
             actual_state.process = self.env.process(actual_state.process_state())
 
-    def get_process(self, process: process.PROCESS_UNION) -> state.State:
+    def get_process(self, process: PROCESS_UNION) -> state.State:
         """
         Returns the ProducitonState or CapabilityState of the resource for a process.
 
         Args:
-            process (process.PROCESS_UNION): The process to get the state for.
+            process (PROCESS_UNION): The process to get the state for.
 
         Raises:
             ValueError: If the process is not found in the resource.
 
         Returns:
             state.State: The state of the resource for the process.
         """
@@ -188,20 +187,20 @@
         ]
         if not possible_states:
             raise ValueError(
                 f"Process {process.process_data.ID} not found in resource {self.data.ID}"
             )
         return random.choice(possible_states)
 
-    def get_processes(self, process: process.PROCESS_UNION) -> List[state.State]:
+    def get_processes(self, process: PROCESS_UNION) -> List[state.State]:
         """
         Returns the ProducitonState or CapabilityState of the resource for a process.
 
         Args:
-            process (process.PROCESS_UNION): The process to get the state for.
+            process (PROCESS_UNION): The process to get the state for.
 
         Raises:
             ValueError: If the process is not found in the resource.
 
         Returns:
             List[state.State]: The state of the resource for the process.
         """
@@ -212,20 +211,20 @@
         ]
         if not possible_states:
             raise ValueError(
                 f"Process {process.process_data.ID} not found in resource {self.data.ID}"
             )
         return possible_states
 
-    def get_free_process(self, process: process.PROCESS_UNION) -> Optional[state.State]:
+    def get_free_process(self, process: PROCESS_UNION) -> Optional[state.State]:
         """
         Returns a free ProductionState or CapabilityState of the resource for a process.
 
         Args:
-            process (process.PROCESS_UNION): The process to get the state for.
+            process (PROCESS_UNION): The process to get the state for.
 
         Returns:
             Optional[state.State]: The state of the resource for the process.
         """
         for actual_state in self.production_states:
             if actual_state.state_data.ID == process.process_data.ID and (
                 actual_state.process is None or not actual_state.process.is_alive
@@ -329,20 +328,20 @@
             for state in self.production_states
             if (state.process and state.process.is_alive)
         ]
         logger.debug({"ID": self.data.ID, "sim_time": self.env.now, "resource": self.data.ID, "event": f"Start waiting for free of processes in preparation"})
         yield events.AllOf(self.env, running_processes)
         logger.debug({"ID": self.data.ID, "sim_time": self.env.now, "resource": self.data.ID, "event": f"Finished waiting for free of processes in preparation"})
 
-    def setup(self, _process: process.PROCESS_UNION) -> Generator:
+    def setup(self, _process: PROCESS_UNION) -> Generator:
         """
         Sets up the resource for a process.
 
         Args:
-            _process (process.PROCESS_UNION): The process to set up the resource for.
+            _process (PROCESS_UNION): The process to set up the resource for.
 
         Yields:
             Generator: The type of the yield depends on the process.
         """
         if self.current_setup is None:
             yield self.env.process(util.trivial_process(self.env))
             self.current_setup = _process
@@ -382,23 +381,23 @@
 class ProductionResource(Resource):
     """
     A production resource to perform production processes. Has additionally to a Resource input and output queues and a fixed location.
 
     Args:
         env (sim.Environment): The simpy environment.
         data (ProductionResourceData): The resource data.
-        processes (List[process.PROCESS_UNION]): The processes.
+        processes (List[PROCESS_UNION]): The processes.
         controller (control.ProductionController): The controller.
         states (List[state.State]): The states of the resource for breakdowns.
         production_states (List[state.State]): The states of the resource for production.
         setup_states (List[state.SetupState]): The states of the resource for setups.
         got_free (events.Event): The event that is triggered when the resource gets free of processes.
         active (events.Event): The event that is triggered when the resource is active.
-        current_setup (process.PROCESS_UNION): The current setup.
-        reserved_setup (process.PROCESS_UNION): The reserved setup.
+        current_setup (PROCESS_UNION): The current setup.
+        reserved_setup (PROCESS_UNION): The reserved setup.
         input_queues (List[store.Queue]): The input queues.
         output_queues (List[store.Queue]): The output queues.
 
 
     """
     data: ProductionResourceData
     controller: control.ProductionController
@@ -423,28 +422,26 @@
 class TransportResource(Resource):
     """
     A transport resource to perform transport processes. Can change its and the product's location during transport processes.
 
     Args:
         env (sim.Environment): The simpy environment.
         data (TransportResourceData): The resource data.
-        processes (List[process.PROCESS_UNION]): The processes.
+        processes (List[PROCESS_UNION]): The processes.
         controller (control.TransportController): The controller.
         states (List[state.State]): The states of the resource for breakdowns.
         production_states (List[state.State]): The states of the resource for production.
         setup_states (List[state.SetupState]): The states of the resource for setups.
         got_free (events.Event): The event that is triggered when the resource gets free of processes.
         active (events.Event): The event that is triggered when the resource is active.
-        current_setup (process.PROCESS_UNION): The current setup.
-        reserved_setup (process.PROCESS_UNION): The reserved setup.
+        current_setup (PROCESS_UNION): The current setup.
+        reserved_setup (PROCESS_UNION): The reserved setup.
     """
     data: TransportResourceData
     controller: control.TransportController
 
 
 RESOURCE_UNION = Union[ProductionResource, TransportResource]
 """ Union Type for Resources. """
 
-from prodsys.simulation import process, control, state
-Resource.update_forward_refs()
-ProductionResource.update_forward_refs()
-TransportResource.update_forward_refs()
+from prodsys.simulation import control, state
+from prodsys.simulation.process import PROCESS_UNION
```

### Comparing `prodsys-0.6.5/prodsys/simulation/route_finder.py` & `prodsys-0.7.0/prodsys/simulation/route_finder.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/simulation/router.py` & `prodsys-0.7.0/prodsys/simulation/router.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import simpy
 logger = logging.getLogger(__name__)
 
 import numpy as np
 
 from simpy import events
 
-from prodsys.simulation import resources
 from prodsys.simulation import request
+from prodsys.simulation import resources
 
 
 if TYPE_CHECKING:
     from prodsys.simulation import resources, product, sink
     from prodsys.factories import resource_factory, sink_factory
     from prodsys.control import routing_control_env
```

### Comparing `prodsys-0.6.5/prodsys/simulation/sim.py` & `prodsys-0.7.0/prodsys/simulation/sim.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/simulation/sink.py` & `prodsys-0.7.0/prodsys/simulation/sink.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import List, TYPE_CHECKING
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from prodsys.simulation import sim, store
 from prodsys.models import sink_data
 
 if TYPE_CHECKING:
     from prodsys.simulation import product
 
@@ -22,16 +22,15 @@
         input_queues (List[store.Queue], optional): The input queues. Defaults to [].
     """
     env: sim.Environment
     data: sink_data.SinkData
     product_factory: product_factory.ProductFactory
     input_queues: List[store.Queue] = Field(default_factory=list, init=False)
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config=ConfigDict(arbitrary_types_allowed=True)
 
     def add_input_queues(self, input_queues: List[store.Queue]):
         """
         Adds input queues to the sink.
 
         Args:
             input_queues (List[store.Queue]): The input queues.
@@ -69,11 +68,9 @@
         Registers a finished product when it reaches the sink.
 
         Args:
             product (product.Product): The finished product.
         """
         self.product_factory.register_finished_product(product)
 
-from prodsys.factories import product_factory
-Sink.update_forward_refs()
-    
+from prodsys.factories import product_factory
```

### Comparing `prodsys-0.6.5/prodsys/simulation/source.py` & `prodsys-0.7.0/prodsys/simulation/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from __future__ import annotations
 
 from typing import List, TYPE_CHECKING, Tuple, Generator
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 from simpy import events
 
 import logging
 logger = logging.getLogger(__name__)
 
 from prodsys.simulation import router, sim, store, time_model
 from prodsys.models import source_data, product_data
 
-if TYPE_CHECKING:
-    from prodsys.factories import product_factory
-
 
 class Source(BaseModel):
     """
     Class that represents a source.
 
     Args:
         env (sim.Environment): The simulation environment.
@@ -32,16 +29,15 @@
     data: source_data.SourceData
     product_data: product_data.ProductData
     product_factory: product_factory.ProductFactory
     time_model: time_model.TimeModel
     router: router.Router
     output_queues: List[store.Queue] = Field(default_factory=list, init=False)
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config=ConfigDict(arbitrary_types_allowed=True)
 
     def add_output_queues(self, output_queues: List[store.Queue]):
         """
         Adds output queues to the source.
 
         Args:
             output_queues (List[store.Queue]): The output queues.
@@ -106,8 +102,8 @@
 
         Returns:
             List[float]: The location. Has to be a list of length 2.
         """
         return self.data.location
     
 from prodsys.factories import product_factory
-Source.update_forward_refs()
+# Source.model_rebuild()
```

### Comparing `prodsys-0.6.5/prodsys/simulation/state.py` & `prodsys-0.7.0/prodsys/simulation/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,26 @@
 from typing import Optional, Union, TYPE_CHECKING, Generator, List
 
 import logging
 logger = logging.getLogger(__name__)
 
 from simpy import events
 from simpy import exceptions
-from pydantic import BaseModel, Extra, root_validator, Field
+from pydantic import BaseModel, ConfigDict, model_validator, Field
 
 from prodsys.simulation import sim, time_model
 from prodsys.models.state_data import (
     StateData,
     BreakDownStateData,
     ProductionStateData,
     TransportStateData,
     SetupStateData,
     ProcessBreakDownStateData,
 )
 
-if TYPE_CHECKING:
-    from prodsys.simulation import product, resources
-
-
 class StateEnum(str, Enum):
     """
     Enum for the different types a state can be in.
     """
     start_state = "start state"
     start_interrupt = "start interrupt"
     end_interrupt = "end interrupt"
@@ -46,15 +42,15 @@
     breakdown = "Breakdown"
     process_breakdown = "ProcessBreakdown"
     setup = "Setup"
     source = "Source"
     sink = "Sink"
 
 
-class StateInfo(BaseModel, extra=Extra.allow):
+class StateInfo(BaseModel):
     """
     Class that represents the current event information of a state while simulating.
 
     Args:
         ID (str): The ID of the state.
         resource_ID (str): The ID of the resource the state belongs to.
         _event_time (Optional[float], optional): The time of the event. Defaults to 0.0.
@@ -71,14 +67,16 @@
     _activity: Optional[StateEnum] = None
     _state_type: Optional[StateTypeEnum] = None
     _product_ID: str = ""
     _target_ID: str = ""
     _origin_ID: str = ""
     _empty_transport: Optional[bool] = None
 
+    model_config=ConfigDict(extra="allow")
+
     def log_transport(self, origin: Optional[product.Locatable], target: product.Locatable, state_type: StateTypeEnum, empty_transport: bool):
         """
         Logs the target location of a transport state.
 
         Args:
             origin (Optional[product.Locatable]): The origin location, either a resource, source, node or a sink.
             target (product.Locatable): The target location, either a resource, source, node or a sink.
@@ -191,16 +189,16 @@
     env: sim.Environment
     active: events.Event = Field(default=None, init=False)
     finished_process: events.Event = Field(default=None, init=False)
     resource: resources.Resource = Field(init=False, default=None)
     process: Optional[events.Process] = Field(default=None)
     state_info: StateInfo = Field(None)
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config=ConfigDict(arbitrary_types_allowed=True)
+
 
     def set_resource(self, resource_model: resources.Resource) -> None:
         """
         Sets the resource of the state.
 
         Args:
             resource_model (resources.Resource): The resource the state belongs to.
@@ -445,15 +443,15 @@
         state_info (StateInfo, optional): The state information of the state. Defaults to None.
         repair_time_model (time_model.TimeModel, optional): The time model of the repair time. Defaults to None.
     """
     state_data: BreakDownStateData
     repair_time_model: time_model.TimeModel
     active_breakdown: bool = False
 
-    @root_validator
+    @model_validator(mode="before")
     def post_init(cls, values):
         values["active"] = events.Event(values["env"])
         return values
 
     def process_state(self) -> Generator:
         while True:
             yield self.env.process(self.wait_for_breakdown())
@@ -494,15 +492,15 @@
         production_states (List[State], optional): The production states of the process. Defaults to None.
         repair_time_model (time_model.TimeModel, optional): The time model of the repair time. Defaults to None.
     """
     state_data: ProcessBreakDownStateData
     production_states: List[State] = None
     repair_time_model: time_model.TimeModel
 
-    @root_validator
+    @model_validator(mode="before")
     def post_init(cls, values):
         values["active"] = events.Event(values["env"])
         return values
 
     def set_production_states(self, production_states: List[ProductionState]):
         if any(
             [
@@ -638,7 +636,12 @@
 
 STATE_UNION = Union[
     BreakDownState, ProductionState, TransportState, SetupState, ProcessBreakDownState
 ]
 """
 Union Type of all states.
 """
+
+from prodsys.simulation import resources
+
+if TYPE_CHECKING:
+    from prodsys.simulation import product
```

### Comparing `prodsys-0.6.5/prodsys/simulation/store.py` & `prodsys-0.7.0/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/simulation/time_model.py` & `prodsys-0.7.0/prodsys/simulation/time_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from __future__ import annotations
-
 from abc import ABC, abstractmethod
 import itertools
 from typing import Callable, Iterator, List, Optional, Tuple, Union
 from typing_extensions import deprecated
 
 import numpy as np
-from pydantic import BaseModel, Field, PrivateAttr, validator
+from pydantic import BaseModel, ConfigDict, Field, PrivateAttr, field_validator
 
 from prodsys.models.time_model_data import (
     FunctionTimeModelData,
     SampleTimeModelData,
     ScheduledTimeModelData,
     DistanceTimeModelData,
     SequentialTimeModelData,
@@ -71,15 +69,15 @@
     """
     time_model_data: FunctionTimeModelData
     statistics_buffer: List[float] = []
     distribution_function_object: Callable[
         [FunctionTimeModelData], List[float]
     ] = FUNCTION_DICT[FunctionTimeModelEnum.Constant]
 
-    @validator("distribution_function_object", always=True)
+    @field_validator("distribution_function_object")
     def initialize_distribution_function(cls, v, values):
         return FUNCTION_DICT[values["time_model_data"].distribution_function]
 
     def get_next_time(
         self,
         origin: Optional[List[float]] = None,
         target: Optional[List[float]] = None,
@@ -159,16 +157,16 @@
 
     _time_value_iterator: Iterator[float] = PrivateAttr()
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._time_value_iterator = self._get_time_value_iterator()
 
-    class Config:
-        arbitrary_types_allowed = True
+    model_config=ConfigDict(arbitrary_types_allowed=True)
+
 
     def _get_time_value_iterator(self) -> Iterator[float]:
         """
         Returns an iterator for the time values of the schedule.
 
         Returns:
             Iterator[float]: The iterator for the time values of the schedule.
```

### Comparing `prodsys-0.6.5/prodsys/util/kpi_visualization.py` & `prodsys-0.7.0/prodsys/util/kpi_visualization.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/util/post_processing.py` & `prodsys-0.7.0/prodsys/util/post_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass, field
 from functools import cached_property
 
 from prodsys.simulation import state
 from prodsys.models import performance_indicators
 
 from typing import List
```

### Comparing `prodsys-0.6.5/prodsys/util/runner.py` & `prodsys-0.7.0/prodsys/util/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 import contextlib
 import random
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 from typing import List, Optional
 
 import numpy as np
 import time
 from functools import cached_property
 
 from prodsys.adapters import adapter
-from prodsys.simulation import sim
+from prodsys.simulation import sim, logger
 from prodsys.factories import (
     link_transport_process_updater,
     state_factory,
     time_model_factory,
     process_factory,
     queue_factory,
     resource_factory,
     product_factory,
     sink_factory,
     source_factory,
     node_factory,
 )
-from prodsys.simulation import logger
-from prodsys.util import post_processing, kpi_visualization, util
+
+from prodsys.util.post_processing import PostProcessor
+
+from prodsys.util import kpi_visualization, util
 from prodsys.models import performance_data
 
 VERBOSE = 1
 
 def run_simulation(adapter_object: adapter.ProductionSystemAdapter, run_length: int) -> Runner:
     """
     Runs the simulation for the given adapter and run length.
@@ -61,15 +63,15 @@
     try:
         yield
     finally:
         np.random.set_state(np_state)
         random.setstate(p_state)
 
 
-class Runner(BaseModel):
+class Runner:
     """
     Class to represent the simulation runner. It allows to run the simulation based on a provided adapter.
 
     Args:
         adapter (adapter.ProductionSystemAdapter): The adapter containing the production system to simulate.
 
     Attributes:
@@ -83,35 +85,31 @@
         sink_factory (sink_factory.SinkFactory): The sink factory to create the sinks.
         source_factory (source_factory.SourceFactory): The source factory to create the sources.
         product_factory (product_factory.ProductFactory): The product factory to create the products.
         event_logger (logger.Logger): The event logger to log the events.
         time_stamp (str): The time stamp of the simulation run.
         post_processor (post_processing.PostProcessor): The post processor to process the simulation results.
     """
-    adapter: adapter.ProductionSystemAdapter
-    env: sim.Environment = Field(
-        None, description="The environment to run the simulation in", init=False
-    )
-    time_model_factory: time_model_factory.TimeModelFactory = Field(
-        init=False, default=None
-    )
-    state_factory: state_factory.StateFactory = Field(init=False, default=None)
-    process_factory: process_factory.ProcessFactory = Field(init=False, default=None)
-    queue_factory: queue_factory.QueueFactory = Field(init=False, default=None)
-    resource_factory: resource_factory.ResourceFactory = Field(init=False, default=None)
-    node_factory: node_factory.NodeFactory = Field(init=False, default=None)
-    sink_factory: sink_factory.SinkFactory = Field(init=False, default=None)
-    source_factory: source_factory.SourceFactory = Field(init=False, default=None)
-    product_factory: product_factory.ProductFactory = Field(init=False, default=None)
-    event_logger: logger.Logger = Field(init=False, default=None)
-    time_stamp: str = Field(init=False, default="")
-    post_processor: post_processing.PostProcessor = Field(init=False, default=None)
 
-    class Config:
-        arbitrary_types_allowed = True
+    def __init__(self, adapter: adapter.ProductionSystemAdapter):
+        self.adapter = adapter
+        self.env = sim.Environment(seed=self.adapter.seed)
+        self.time_model_factory: time_model_factory.TimeModelFactory = None
+        self.state_factory: state_factory.StateFactory = None
+        self.process_factory: process_factory.ProcessFactory = None
+        self.queue_factory: queue_factory.QueueFactory = None
+        self.resource_factory: resource_factory.ResourceFactory = None
+        self.node_factory: node_factory.NodeFactory = None
+        self.sink_factory: sink_factory.SinkFactory = None
+        self.source_factory: source_factory.SourceFactory = None
+        self.product_factory: product_factory.ProductFactory = None
+        self.event_logger: logger.Logger = None
+        self.time_stamp: str = ""
+        self.post_processor: PostProcessor = None
+
 
     def initialize_simulation(self):
         """
         Initializes the simulation by creating the factories and all simulation objects. Needs to be done before running the simulation.
         """
         self.adapter.validate_configuration()
         with temp_seed(self.adapter.seed):
@@ -196,23 +194,23 @@
         t_0 = time.perf_counter()
 
         self.env.run(time_range)
 
         t_1 = time.perf_counter()
         self.time_stamp = time.strftime("%Y%m%d-%H%M%S")
 
-    def get_post_processor(self) -> post_processing.PostProcessor:
+    def get_post_processor(self) -> PostProcessor:
         """
         Returns the post processor to process the simulation results.
 
         Returns:
             post_processing.PostProcessor: The post processor to process the simulation results.
         """
         if not self.post_processor:
-            self.post_processor = post_processing.PostProcessor(df_raw=self.event_logger.get_data_as_dataframe())
+            self.post_processor = PostProcessor(df_raw=self.event_logger.get_data_as_dataframe())
         return self.post_processor
 
 
     def print_results(self):
         """
         Prints the aggregated simulation results, comprising the average throughput, WIP, throughput time and the time per state of the resources.
         """
@@ -278,15 +276,15 @@
     def get_aggregated_data_simulation_results(self) -> dict:
         """
         Returns the aggregated simulation results.
 
         Returns:
             dict: The aggregated simulation results.
         """
-        p = post_processing.PostProcessor(df_raw=self.event_logger.get_data_as_dataframe())
+        p = PostProcessor(df_raw=self.event_logger.get_data_as_dataframe())
         return p.get_aggregated_data()
 
     def save_results_as_csv(self, save_folder="data"):
         """
         Saves the simulation results as .csv-file marked with the time_stamp of simulation and the adapter ID if available.
 
         Args:
```

### Comparing `prodsys-0.6.5/prodsys/util/statistical_functions.py` & `prodsys-0.7.0/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/prodsys/util/util.py` & `prodsys-0.7.0/prodsys/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     file_paths = [f for f in listdir(folder_path) if isfile(join(folder_path, f))]
     adapter_objects = []
     for counter, file_path in enumerate(file_paths):
         if ".json" not in file_path or file_path == "optimization_results.json":
             continue
         adapter = adapters.JsonProductionSystemAdapter()
         adapter.read_data(join(folder_path, file_path))
-        adapter.scenario_data = base_configuration.scenario_data.copy()
+        adapter.scenario_data = base_configuration.scenario_data.model_copy()
         if not adapter.ID:
             adapter.ID = f"initial_solution_{counter}"
         adapter_objects.append(adapter)
     return adapter_objects
 
 def get_initial_solution_file_pth(
         folder_path: str
```

### Comparing `prodsys-0.6.5/pyproject.toml` & `prodsys-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.6.5"
+version = "0.7.0"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.13"
-pydantic = "^1.10.7"
+python = "^3.10"
+pydantic = "^2.7.1"
 simpy = "^4.0.1"
-fastapi = "0.99.1"
-uvicorn = {extras = ["standard"], version = "^0.21.1"}
+fastapi = "^0.111.0"
+uvicorn = {extras = ["standard"], version = "^0.29.0"}
 deap = "^1.3.3"
 simanneal = "^0.5.0"
 gurobipy = "^10.0.1"
 hydra-core = "^1.3.2"
 pandas = "^2.0.0"
 openpyxl = "^3.1.2"
 plotly = "^5.14.1"
```

### Comparing `prodsys-0.6.5/README.md` & `prodsys-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `prodsys-0.6.5/PKG-INFO` & `prodsys-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.6.5
+Version: 0.7.0
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ai
 Requires-Dist: deap (>=1.3.3,<2.0.0)
 Requires-Dist: email-validator (>=2.1.1,<3.0.0)
-Requires-Dist: fastapi (==0.99.1)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: gurobipy (>=10.0.1,<11.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pathfinding (>=1.0.9,<2.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: simanneal (>=0.5.0,<0.6.0)
 Requires-Dist: simpy (>=4.0.1,<5.0.0)
 Requires-Dist: tqdm (>=4.65,<5.0)
-Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0)
+Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
 
 ![prodsys logo](https://raw.githubusercontent.com/sdm4fzi/prodsys/main/resources/logo.svg)
 
 *prodsys - modeling, simulating and optimizing production systems*
 
 ![Build-sucess](https://img.shields.io/badge/build-success-green)
```

