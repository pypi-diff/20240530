# Comparing `tmp/globus-compute-endpoint-2.8.0a0.tar.gz` & `tmp/globus-compute-endpoint-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.8.0a0.tar", last modified: Mon Nov 20 20:48:55 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.9.0.tar", last modified: Wed Dec 13 21:50:47 2023, max compression
```

## Comparing `globus-compute-endpoint-2.8.0a0.tar` & `globus-compute-endpoint-2.9.0.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.016746 globus-compute-endpoint-2.8.0a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      385 2023-11-09 20:18:47.000000 globus-compute-endpoint-2.8.0a0/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     2733 2023-11-20 20:48:55.016663 globus-compute-endpoint-2.8.0a0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.8.0a0/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:54.997779 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    20461 2023-10-20 21:22:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.000406 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.002961 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/
--rw-r--r--   0 lei        (501) staff       (20)       41 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     8713 2023-11-08 18:25:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/config.py
--rw-r--r--   0 lei        (501) staff       (20)      760 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)      146 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/default_config.yaml
--rw-r--r--   0 lei        (501) staff       (20)      560 2023-11-08 18:25:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/example_identity_mapping_config.json
--rw-r--r--   0 lei        (501) staff       (20)     4254 2023-11-08 18:25:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/model.py
--rw-r--r--   0 lei        (501) staff       (20)      265 2023-09-06 19:32:42.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/user_config_schema.json
--rw-r--r--   0 lei        (501) staff       (20)     1833 2023-10-11 17:14:42.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/user_config_template.yaml
--rw-r--r--   0 lei        (501) staff       (20)      707 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/user_environment.yaml
--rw-r--r--   0 lei        (501) staff       (20)    10769 2023-11-09 20:18:47.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/utils.py
--rw-r--r--   0 lei        (501) staff       (20)    32668 2023-11-20 20:37:16.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    30223 2023-11-20 20:37:16.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)     7651 2023-11-08 18:25:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/identity_mapper.py
--rw-r--r--   0 lei        (501) staff       (20)    24384 2023-11-08 18:25:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     3161 2023-09-11 16:28:45.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.004283 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      291 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11922 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)    14408 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14231 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.004655 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     3247 2023-11-08 18:25:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.006400 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/
--rw-r--r--   0 lei        (501) staff       (20)      310 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6351 2023-11-09 20:18:47.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/base.py
--rw-r--r--   0 lei        (501) staff       (20)     9206 2023-11-15 20:50:15.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/globus_compute.py
--rw-r--r--   0 lei        (501) staff       (20)     4746 2023-09-11 16:28:45.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/helper.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.009347 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1943 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    35522 2023-11-08 21:31:55.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/engine.py
--rw-r--r--   0 lei        (501) staff       (20)    49295 2023-09-06 19:49:50.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    36125 2023-09-06 19:49:50.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9295 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     7312 2023-09-11 16:28:45.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    19094 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5427 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     3725 2023-11-15 20:50:15.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/process_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     3525 2023-11-15 20:50:15.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/thread_pool.py
--rw-r--r--   0 lei        (501) staff       (20)     3584 2023-10-24 18:09:22.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.009569 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.009930 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      422 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)     8499 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.010099 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.010993 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/providers/kubernetes/template.py
--rw-r--r--   0 lei        (501) staff       (20)     5231 2023-11-08 18:25:42.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/self_diagnostic.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.012704 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7424 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5470 2023-08-17 22:31:18.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6225 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-11-20 20:47:44.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.015823 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     2733 2023-11-20 20:48:54.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     4135 2023-11-20 20:48:54.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-11-20 20:48:54.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      353 2023-11-20 20:48:54.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      456 2023-11-20 20:48:54.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-11-20 20:48:54.000000 globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-11-20 20:48:55.017042 globus-compute-endpoint-2.8.0a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3826 2023-11-20 20:47:40.000000 globus-compute-endpoint-2.8.0a0/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.013412 globus-compute-endpoint-2.8.0a0/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.8.0a0/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     4078 2023-11-15 20:50:22.000000 globus-compute-endpoint-2.8.0a0/tests/conftest.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.013835 globus-compute-endpoint-2.8.0a0/tests/integration/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    11663 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/conftest.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.014319 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2063 2023-11-15 20:50:22.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/conftest.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.014696 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:55.015611 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2218 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
--rw-r--r--   0 lei        (501) staff       (20)     2168 2023-11-08 18:25:44.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/test_manager.py
--rw-r--r--   0 lei        (501) staff       (20)     1273 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     1182 2023-08-17 23:30:28.000000 globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/mock_executors.py
--rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.8.0a0/tests/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.254910 globus-compute-endpoint-2.9.0/
+-rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)      385 2023-11-10 18:11:31.000000 globus-compute-endpoint-2.9.0/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     2730 2023-12-13 21:50:47.254810 globus-compute-endpoint-2.9.0/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      871 2023-04-17 20:09:04.000000 globus-compute-endpoint-2.9.0/PyPI.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.214950 globus-compute-endpoint-2.9.0/globus_compute_endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)      131 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    20825 2023-12-04 21:57:18.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.225081 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.230116 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/
+-rw-r--r--   0 chris      (501) staff       (20)       41 2023-10-19 17:11:34.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     8713 2023-11-06 17:12:09.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/config.py
+-rw-r--r--   0 chris      (501) staff       (20)      760 2023-07-10 15:27:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/default_config.py
+-rw-r--r--   0 chris      (501) staff       (20)      146 2023-07-21 16:37:09.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/default_config.yaml
+-rw-r--r--   0 chris      (501) staff       (20)      560 2023-11-06 17:12:09.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/example_identity_mapping_config.json
+-rw-r--r--   0 chris      (501) staff       (20)     4226 2023-12-04 21:57:18.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/model.py
+-rw-r--r--   0 chris      (501) staff       (20)      265 2023-08-28 19:55:50.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/user_config_schema.json
+-rw-r--r--   0 chris      (501) staff       (20)     1833 2023-10-11 17:42:30.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/user_config_template.yaml
+-rw-r--r--   0 chris      (501) staff       (20)      707 2023-08-14 18:39:21.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/user_environment.yaml
+-rw-r--r--   0 chris      (501) staff       (20)    10769 2023-11-10 18:11:31.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/utils.py
+-rw-r--r--   0 chris      (501) staff       (20)    32668 2023-11-29 16:02:16.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 chris      (501) staff       (20)    34264 2023-12-04 21:57:18.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)     7651 2023-11-06 17:12:09.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/identity_mapper.py
+-rw-r--r--   0 chris      (501) staff       (20)    24384 2023-11-06 17:12:09.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 chris      (501) staff       (20)     3161 2023-09-11 21:52:05.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.232509 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 chris      (501) staff       (20)      291 2023-08-07 16:30:24.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      689 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 chris      (501) staff       (20)    11922 2023-10-31 22:34:05.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 chris      (501) staff       (20)    14408 2023-10-31 22:34:05.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/result_publisher.py
+-rw-r--r--   0 chris      (501) staff       (20)    14231 2023-10-31 22:34:05.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 chris      (501) staff       (20)     5184 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 chris      (501) staff       (20)     7275 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.233502 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 chris      (501) staff       (20)     3908 2023-12-04 21:57:18.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      110 2023-06-08 19:30:56.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.236374 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/
+-rw-r--r--   0 chris      (501) staff       (20)      310 2023-07-18 16:13:32.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7669 2023-12-13 16:13:12.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/base.py
+-rw-r--r--   0 chris      (501) staff       (20)    10086 2023-12-04 21:57:18.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/globus_compute.py
+-rw-r--r--   0 chris      (501) staff       (20)     4746 2023-09-11 21:52:05.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/helper.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.241554 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1943 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/container_sched.py
+-rw-r--r--   0 chris      (501) staff       (20)    35522 2023-11-10 18:11:31.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/engine.py
+-rw-r--r--   0 chris      (501) staff       (20)    49295 2023-07-25 15:47:26.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/interchange.py
+-rw-r--r--   0 chris      (501) staff       (20)     9712 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 chris      (501) staff       (20)      267 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 chris      (501) staff       (20)    36125 2023-08-01 17:50:19.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/manager.py
+-rw-r--r--   0 chris      (501) staff       (20)     9295 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/messages.py
+-rw-r--r--   0 chris      (501) staff       (20)     7312 2023-09-11 21:52:05.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/worker.py
+-rw-r--r--   0 chris      (501) staff       (20)    19094 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/worker_map.py
+-rw-r--r--   0 chris      (501) staff       (20)     5427 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py
+-rw-r--r--   0 chris      (501) staff       (20)     3725 2023-11-10 18:11:31.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/process_pool.py
+-rw-r--r--   0 chris      (501) staff       (20)     3525 2023-11-10 18:11:31.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/thread_pool.py
+-rw-r--r--   0 chris      (501) staff       (20)     3584 2023-11-14 22:15:53.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 chris      (501) staff       (20)      220 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.241916 globus-compute-endpoint-2.9.0/globus_compute_endpoint/executors/
+-rw-r--r--   0 chris      (501) staff       (20)      141 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.243112 globus-compute-endpoint-2.9.0/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      422 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 chris      (501) staff       (20)     8499 2023-06-21 21:36:42.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.243487 globus-compute-endpoint-2.9.0/globus_compute_endpoint/providers/
+-rw-r--r--   0 chris      (501) staff       (20)      115 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.245119 globus-compute-endpoint-2.9.0/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    12926 2023-04-26 19:06:47.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 chris      (501) staff       (20)       50 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/providers/kubernetes/template.py
+-rw-r--r--   0 chris      (501) staff       (20)     5231 2023-10-11 17:42:30.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/self_diagnostic.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.248525 globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/
+-rw-r--r--   0 chris      (501) staff       (20)      280 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7424 2023-07-19 17:12:42.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     5470 2023-04-24 14:59:12.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 chris      (501) staff       (20)     6222 2023-12-13 16:13:12.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 chris      (501) staff       (20)     1610 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 chris      (501) staff       (20)      804 2023-12-13 16:28:29.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.253619 globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     2730 2023-12-13 21:50:47.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     4197 2023-12-13 21:50:47.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-12-13 21:50:47.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      353 2023-12-13 21:50:47.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)      455 2023-12-13 21:50:47.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       30 2023-12-13 21:50:47.000000 globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      282 2023-12-13 21:50:47.255450 globus-compute-endpoint-2.9.0/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     3825 2023-12-13 16:28:29.000000 globus-compute-endpoint-2.9.0/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.249716 globus-compute-endpoint-2.9.0/tests/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.9.0/tests/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     4078 2023-11-15 19:59:40.000000 globus-compute-endpoint-2.9.0/tests/conftest.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.250468 globus-compute-endpoint-2.9.0/tests/integration/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/tests/integration/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    11663 2023-10-16 19:19:06.000000 globus-compute-endpoint-2.9.0/tests/integration/conftest.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.251026 globus-compute-endpoint-2.9.0/tests/integration/endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2063 2023-11-15 19:59:40.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/conftest.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.252236 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:47.253293 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2218 2023-08-01 20:13:46.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
+-rw-r--r--   0 chris      (501) staff       (20)     2168 2023-11-06 17:12:09.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/test_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)     1273 2023-06-30 16:09:15.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py
+-rw-r--r--   0 chris      (501) staff       (20)     1182 2023-08-01 20:13:46.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/mock_executors.py
+-rw-r--r--   0 chris      (501) staff       (20)     4676 2023-12-04 21:57:18.000000 globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/test_gcengine_retries.py
+-rw-r--r--   0 chris      (501) staff       (20)     3553 2023-12-04 21:57:18.000000 globus-compute-endpoint-2.9.0/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.8.0a0/LICENSE` & `globus-compute-endpoint-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/PKG-INFO` & `globus-compute-endpoint-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.8.0a0
+Version: 2.9.0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
@@ -17,23 +17,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: globus-sdk
-Requires-Dist: globus-compute-sdk==2.8.0a0
+Requires-Dist: globus-compute-sdk==2.9.0
 Requires-Dist: globus-compute-common==0.3.0
 Requires-Dist: globus-identity-mapping==0.1.0
 Requires-Dist: texttable<2,>=1.6.4
 Requires-Dist: psutil<6
 Requires-Dist: python-daemon<3,>=2
 Requires-Dist: click<9,>=8
 Requires-Dist: pyzmq!=22.3.0,<=23.2.0,>=22.0.0
-Requires-Dist: parsl==2023.7.3
+Requires-Dist: parsl==2023.12.4
 Requires-Dist: pika>=1.2.0
 Requires-Dist: pyprctl<0.2.0
 Requires-Dist: setproctitle<1.4,>=1.3.2
 Requires-Dist: pyyaml<7.0,>=6.0
 Requires-Dist: jinja2<3.2,>=3.1.2
 Requires-Dist: jsonschema<4.20,>=4.19.0
 Requires-Dist: cachetools>=5.3.1
```

### Comparing `globus-compute-endpoint-2.8.0a0/PyPI.md` & `globus-compute-endpoint-2.9.0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -589,21 +589,34 @@
 @click.option(
     "--yes", default=False, is_flag=True, help="Do not ask for confirmation to delete."
 )
 @common_options
 @handle_auth_errors
 def delete_endpoint(*, ep_dir: pathlib.Path, force: bool, yes: bool):
     """Deletes an endpoint and its config."""
+
+    ep_conf = None
+    try:
+        ep_conf = get_config(ep_dir)
+    except Exception as e:
+        print(f"({type(e).__name__}) {e}\n")
+        if not yes:
+            yes = click.confirm(
+                f"Failed to read configuration from {ep_dir}/\n"
+                f"  Are you sure you want to delete endpoint <{ep_dir.name}>?",
+                abort=True,
+            )
+
     if not yes:
-        click.confirm(
-            f"Are you sure you want to delete the endpoint named <{ep_dir.name}>?",
+        yes = click.confirm(
+            f"Are you sure you want to delete endpoint <{ep_dir.name}>?",
             abort=True,
         )
 
-    Endpoint.delete_endpoint(ep_dir, get_config(ep_dir), force=force)
+    Endpoint.delete_endpoint(ep_dir, ep_conf, force=force)
 
 
 @app.command("self-diagnostic")
 @click.option(
     "-z",
     "--gzip",
     "compress",
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/config.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/default_config.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/example_identity_mapping_config.json` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/example_identity_mapping_config.json`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/model.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     type: str = "HighThroughputEngine"
     provider: t.Optional[ProviderModel]
     strategy: t.Optional[StrategyModel]
     address: t.Optional[t.Union[str, AddressModel]]
     worker_ports: t.Optional[t.Tuple[int, int]]
     worker_port_range: t.Optional[t.Tuple[int, int]]
     interchange_port_range: t.Optional[t.Tuple[int, int]]
+    max_retries_on_system_failure: t.Optional[int]
 
     _validate_type = _validate_import("type", engines)
     _validate_provider = _validate_params("provider")
     _validate_strategy = _validate_params("strategy")
     _validate_address = _validate_params("address")
 
     class Config:
@@ -115,24 +116,23 @@
     amqp_port: t.Optional[int]
 
     _validate_engine = _validate_params("engine")
 
     @pydantic.root_validator
     @classmethod
     def _validate(cls, values):
-        is_mt = values.get("multi_user") is True
+        is_mu = values.get("multi_user") is True
 
-        if is_mt:
+        if is_mu:
             msg_engine = "no engine if multi-user"
-            msg_identity = "multi-user requires identity_mapping_config_path"
         else:
             msg_engine = "missing engine"
             msg_identity = "identity_mapping_config_path should not be specified"
-        assert is_mt is not bool(values.get("engine")), msg_engine
-        assert is_mt is bool(values.get("identity_mapping_config_path")), msg_identity
+            assert not bool(values.get("identity_mapping_config_path")), msg_identity
+        assert is_mu is not bool(values.get("engine")), msg_engine
         return values
 
     def dict(self, *args, **kwargs):
         # Slight modification is needed here since we still
         # store the engine/executor in a list named executors
         ret = super().dict(*args, **kwargs)
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/user_config_template.yaml` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/user_config_template.yaml`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/user_environment.yaml` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/user_environment.yaml`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/config/utils.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/config/utils.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,17 +89,18 @@
     def __init__(
         self,
         conf_dir: pathlib.Path,
         endpoint_uuid: str | None,
         config: Config,
         reg_info: dict | None = None,
     ):
-        log.info("Endpoint Manager initialization")
+        log.debug("Endpoint Manager initialization")
 
         self.conf_dir = conf_dir
+        self._config = config
         self._reload_requested = False
         self._time_to_stop = False
         self._kill_event = threading.Event()
 
         self._children: dict[int, UserEndpointRecord] = {}
 
         self._wait_for_child = False
@@ -111,22 +112,31 @@
 
         self._cached_cmd_start_args: TTLCache[int, T_CMD_START_ARGS] = TTLCache(
             maxsize=32768, ttl=config.mu_child_ep_grace_period_s
         )
 
         endpoint_uuid = Endpoint.get_endpoint_id(conf_dir) or endpoint_uuid
 
-        if not config.identity_mapping_config_path:
+        self._mu_user = pwd.getpwuid(os.getuid())
+        privileged = is_privileged(self._mu_user)
+
+        self._allow_same_user = not privileged
+        if config.force_mu_allow_same_user:
+            self._allow_same_user = True
+            _warn_str = privileged and "privileged process" or "unprivileged process"
             msg = (
-                "No identity mapping file specified; please specify"
-                " identity_mapping_config_path"
+                "Configuration item `force_mu_allow_same_user` set to `true`; this is"
+                " considered a very dangerous override -- please use with care,"
+                " especially if allowing this endpoint to be utilized by multiple"
+                " users."
+                f"\n  Endpoint (UID, GID): ({os.getuid()}, {os.getgid()}) {_warn_str}"
             )
-            log.error(msg)
-            print(msg, file=sys.stderr)
-            exit(os.EX_OSFILE)
+            log.warning(msg)
+            if sys.stderr.isatty():
+                print(f"\033[31;1;40m{msg}\033[0m")  # Red bold on black
 
         if not reg_info:
             try:
                 client_options = {
                     "funcx_service_address": config.funcx_service_address,
                     "environment": config.environment,
                 }
@@ -168,15 +178,66 @@
         if endpoint_uuid and upstream_ep_uuid != endpoint_uuid:
             log.error(
                 "Unexpected response from server: mismatched endpoint id."
                 f"\n  Expected: {endpoint_uuid}, received: {upstream_ep_uuid}"
             )
             exit(os.EX_SOFTWARE)
 
-        self._endpoint_uuid_str = str(upstream_ep_uuid)
+        endpoint_uuid = str(upstream_ep_uuid)  # convenience
+        self._endpoint_uuid_str = endpoint_uuid
+
+        self.identity_mapper: PosixIdentityMapper | None = None
+        if not is_privileged(user_privs_only=True):
+            # Test for uid-change privileges only because we don't want to enable
+            # identity mapping unless the process UID has specifically these
+            # privileges; else an unrelated permission (e.g., NET_BIND) would
+            # allow identity mapping.
+            if config.identity_mapping_config_path:
+                msg = (
+                    "`identity_mapping_config_path` specified, but process is not"
+                    " privileged (e.g., not `root`) -- identity mapping configuration"
+                    " will be ignored; only requests from identities that match the"
+                    " identity that registered this endpoint will be honored."
+                    f"\n    (ignored) '{config.identity_mapping_config_path}'"
+                )
+                log.warning(msg)
+        else:
+            if not config.identity_mapping_config_path:
+                msg = (
+                    "No identity mapping file specified; please specify"
+                    " identity_mapping_config_path"
+                )
+                log.error(msg)
+                print(msg, file=sys.stderr)
+                exit(os.EX_OSFILE)
+
+            # Only map identities if possibility of *changing* uid; otherwise
+            # we enforce that the identity of UEPs must match the
+            # parent-process' authorization -- we do not want to allow an open
+            # endpoint by a non-power user.
+            try:
+                self.identity_mapper = PosixIdentityMapper(
+                    config.identity_mapping_config_path, self._endpoint_uuid_str
+                )
+
+            except PermissionError as e:
+                msg = f"({type(e).__name__}) {e}"
+                log.error(msg)
+                print(msg, file=sys.stderr)
+                exit(os.EX_NOPERM)
+
+            except Exception as e:
+                msg = (
+                    f"({type(e).__name__}) {e} -- Unable to read identity mapping"
+                    f" configuration from: {config.identity_mapping_config_path}"
+                )
+                log.debug(msg, exc_info=e)
+                log.error(msg)
+                print(msg, file=sys.stderr)
+                exit(os.EX_CONFIG)
 
         try:
             cq_info = reg_info["command_queue_info"]
             _ = cq_info["connection_url"], cq_info["queue"]
         except Exception as e:
             log.debug("%s", reg_info)
             log.error(
@@ -186,48 +247,14 @@
             exit(os.EX_DATAERR)
 
         if config.amqp_port:
             cq_info["connection_url"] = update_url_port(
                 cq_info["connection_url"], config.amqp_port
             )
 
-        self._mu_user = pwd.getpwuid(os.getuid())
-        if config.force_mu_allow_same_user:
-            self._allow_same_user = True
-            log.warning(
-                "Configuration item `force_mu_allow_same_user` set to true; this is"
-                " considered a very dangerous override -- please use with care,"
-                " especially if allowing this endpoint to be utilized by multiple"
-                " users."
-                f"\n  Endpoint (UID, GID): ({os.getuid()}, {os.getgid()})"
-            )
-        else:
-            self._allow_same_user = not is_privileged(self._mu_user)
-
-        try:
-            self.identity_mapper = PosixIdentityMapper(
-                config.identity_mapping_config_path, self._endpoint_uuid_str
-            )
-
-        except PermissionError as e:
-            msg = f"({type(e).__name__}) {e}"
-            log.error(msg)
-            print(msg, file=sys.stderr)
-            exit(os.EX_NOPERM)
-
-        except Exception as e:
-            msg = (
-                f"({type(e).__name__}) {e} -- Unable to read identity mapping"
-                f" configuration from: {config.identity_mapping_config_path}"
-            )
-            log.debug(msg, exc_info=e)
-            log.error(msg)
-            print(msg, file=sys.stderr)
-            exit(os.EX_CONFIG)
-
         # sanitize passwords in logs
         log_reg_info = re.subn(r"://.*?@", r"://***:***@", repr(reg_info))
         log.debug(f"Registration information: {log_reg_info}")
 
         json_file = conf_dir / "endpoint.json"
 
         # `endpoint_id` key kept for backward compatibility when
@@ -404,14 +431,44 @@
             "Shutdown complete."
             f"\n---------- Endpoint Manager ends: {self._endpoint_uuid_str}\n\n"
         )
 
     def _event_loop(self):
         self._command.start()
 
+        parent_identities = set()
+        if not is_privileged():
+            client_options = {
+                "funcx_service_address": self._config.funcx_service_address,
+                "environment": self._config.environment,
+            }
+            log.debug("Ascertaining user identity set (%s)", client_options)
+
+            gcc = GC.Client(**client_options)
+            try:
+                userinfo = gcc.login_manager.get_auth_client().userinfo()
+                ids = userinfo["identity_set"]
+                parent_identities.update(ident["sub"] for ident in ids)
+                log.debug(
+                    "User-endpoint start requests are valid from identites: %s",
+                    parent_identities,
+                )
+                del gcc, client_options, ids
+                if not parent_identities:
+                    # Not a privileged user -- we require at least one identity
+                    # against which to match start endpoint requests.
+                    raise LookupError("No authorized identities found")
+
+            except Exception as exc:
+                msg = "Failed to determine identity set; try `whoami` command?"
+                log.error(f"({type(exc).__name__}) {exc}\n    {msg}")
+                log.debug("Stopping; failed to determine identities", exc_info=exc)
+                self._time_to_stop = True
+                return
+
         valid_method_name_re = re.compile(r"^cmd_[A-Za-z][0-9A-Za-z_]{0,99}$")
         max_skew_s = 180  # 3 minutes; ignore commands with out-of-date timestamp
         while not self._time_to_stop:
             if self._wait_for_child:
                 self.wait_for_children()
 
             try:
@@ -441,15 +498,15 @@
 
                 msg = json.loads(body)
                 command = msg.get("command")
                 command_args = msg.get("args", [])
                 command_kwargs = msg.get("kwargs", {})
             except Exception as e:
                 log.error(
-                    f"Unable to deserialize Globus Compute services command."
+                    "Unable to deserialize Globus Compute services command."
                     f"  ({e.__class__.__name__}) {e}"
                 )
                 continue
 
             now = round(time.time())
             if abs(now - server_cmd_ts) > max_skew_s:
                 server_pp_ts = datetime.fromtimestamp(server_cmd_ts).strftime("%c")
@@ -461,48 +518,68 @@
                     f"\n  Endpoint timestamp: {now:,} ({endp_pp_ts})"
                 )
                 continue
 
             try:
                 effective_identity = msg["globus_effective_identity"]
                 identity_set = msg["globus_identity_set"]
+                globus_username = msg["globus_username"]
             except Exception as e:
                 log.error(f"Invalid server command.  ({e.__class__.__name__}) {e}")
                 continue
 
             identity_for_log = (
                 f"\n  Globus effective identity: {effective_identity}"
-                f"\n  Globus identity set: {identity_set}"
+                f"\n  Globus username: {globus_username}"
             )
-            try:
-                local_username = self.identity_mapper.map_identity(identity_set)
-                if not local_username:
-                    raise LookupError()
-            except LookupError as e:
-                log.error(
-                    "Identity failed to map to a local user name."
-                    f"  ({e.__class__.__name__}) {e}{identity_for_log}"
-                )
-                continue
-            except Exception as e:
-                msg = "Unhandled error attempting to map user."
-                log.debug(f"{msg}{identity_for_log}", exc_info=e)
-                log.error(f"{msg}  ({e.__class__.__name__}) {e}{identity_for_log}")
-                continue
 
-            try:
-                local_user_rec = pwd.getpwnam(local_username)
+            local_user_rec = None
+            local_username = None
+            if not self.identity_mapper or parent_identities:
+                # we are not a privileged user, so *only* allow the identity (or
+                # linked identities) of the parent process auth'd to run tasks
+
+                cmd_identities = {ident["sub"] for ident in identity_set}
+                if not parent_identities.intersection(cmd_identities):
+                    log.error(
+                        "Ignoring start request for untrusted identity."
+                        f"{identity_for_log}"
+                    )
+                    continue
+                local_user_rec = self._mu_user
+                local_username = self._mu_user.pw_name
 
-            except Exception as e:
-                log.error(
-                    f"({type(e).__name__}) {e}\n"
-                    "  Identity mapped to a local user name, but local user does not"
-                    f" exist.\n  Local user name: {local_username}{identity_for_log}"
-                )
-                continue
+            else:
+                try:
+                    local_username = self.identity_mapper.map_identity(identity_set)
+                    if not local_username:
+                        raise LookupError()
+                except LookupError as e:
+                    log.error(
+                        "Identity failed to map to a local user name."
+                        f"  ({e.__class__.__name__}) {e}{identity_for_log}"
+                    )
+                    continue
+                except Exception as e:
+                    msg = "Unhandled error attempting to map user."
+                    log.debug(f"{msg}{identity_for_log}", exc_info=e)
+                    log.error(f"{msg}  ({e.__class__.__name__}) {e}{identity_for_log}")
+                    continue
+
+                try:
+                    local_user_rec = pwd.getpwnam(local_username)
+
+                except Exception as e:
+                    log.error(
+                        f"({type(e).__name__}) {e}\n"
+                        "  Identity mapped to a local user name, but local user does"
+                        " not exist."
+                        f"\n  Local user name: {local_username}{identity_for_log}"
+                    )
+                    continue
 
             try:
                 if not (command and valid_method_name_re.match(command)):
                     raise InvalidCommandError(f"Unknown or invalid command: {command}")
 
                 command_func = getattr(self, command, None)
                 if not command_func:
@@ -782,10 +859,11 @@
             exit_code += 1
             os.execvpe(proc_args[0], args=proc_args, env=env)
 
             # not executed, except perhaps in testing
             exit_code += 1  # type: ignore
         except Exception as e:
             log.error(f"Unable to exec for {uname} - ({e.__class__.__name__}) {e}")
+            log.debug(f"Failed to exec for {uname}", exc_info=e)
         finally:
             # Only executed if execvpe fails (or isn't reached)
             exit(exit_code)
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/identity_mapper.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/identity_mapper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_publisher.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/result_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,14 +58,29 @@
         _pyprctl.Cap.SYS_RESOURCE,
         _pyprctl.Cap.SYS_TIME,
         _pyprctl.Cap.SYS_TTY_CONFIG,
         _pyprctl.Cap.SYSLOG,
         _pyprctl.Cap.WAKE_ALARM,
     }
 
+    # list of targeted "you can change user" CAPs.  Some of the CAPs in
+    # _MULTI_USER_CAPS might be given legitimately to a process (e.g.,
+    # BPF, NET_BIND_SERVICE); just in case, separate out the ones that are
+    # very, very likely of interest for changing the UID
+    _USER_CHANGE_CAPS = {
+        _pyprctl.Cap.CHOWN,
+        _pyprctl.Cap.DAC_OVERRIDE,
+        _pyprctl.Cap.DAC_READ_SEARCH,
+        _pyprctl.Cap.FOWNER,
+        _pyprctl.Cap.FSETID,
+        _pyprctl.Cap.SETGID,
+        _pyprctl.Cap.SETFCAP,
+        _pyprctl.Cap.SETUID,
+    }
+
 
 def _redact_url_creds(raw: _T, redact_user=True, repl="***", count=0) -> _T:
     """
     Redact URL credentials found in `raw`, by replacing the password and
     (optionally) username with `repl`.
 
     (A wrapper over `re.sub()`)
@@ -80,22 +95,23 @@
     else:
         repl = rf"://\1:{repl}@"
     if isinstance(raw, str):
         return _url_user_pass_re.sub(repl=repl, string=raw, count=count)
     return _urlb_user_pass_re.sub(repl=repl.encode(), string=raw, count=count)
 
 
-def is_privileged(posix_user=None):
+def is_privileged(posix_user=None, user_privs_only=False) -> bool:
     if not posix_user:
         posix_user = _pwd.getpwuid(_os.getuid())
 
+    caps_to_check = user_privs_only and _USER_CHANGE_CAPS or _MULTI_USER_CAPS
     proc_caps = _pyprctl.CapState.get_current()
     has_privileges = posix_user.pw_uid == 0
     has_privileges |= posix_user.pw_name == "root"
-    has_privileges |= any(c in proc_caps.effective for c in _MULTI_USER_CAPS)
+    has_privileges |= any(c in proc_caps.effective for c in caps_to_check)
     return has_privileges
 
 
 def update_url_port(url_string: str, new_port: int | str) -> str:
     c_url = urllib.parse.urlparse(url_string)
     if c_url.port:
         netloc = c_url.netloc.replace(f":{c_url.port}", f":{new_port}")
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/worker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,187 +1,219 @@
+from __future__ import annotations
+
+import argparse
 import logging
-import queue
-import threading
-import time
+import os
+import signal
+import sys
 import typing as t
-import uuid
-from abc import ABC, abstractmethod
-from concurrent.futures import Future
 
+import dill
+import zmq
 from globus_compute_common import messagepack
+from globus_compute_common.messagepack.message_types import Result as OutgoingResult
 from globus_compute_common.messagepack.message_types import (
-    EPStatusReport,
-    Result,
-    TaskTransition,
+    ResultErrorDetails as OutgoingResultErrorDetails,
 )
-from globus_compute_common.tasks import ActorName, TaskState
-from globus_compute_endpoint.engines.helper import execute_task
+from globus_compute_endpoint.engines.high_throughput.messages import Message
 from globus_compute_endpoint.exception_handling import (
     get_error_string,
     get_result_error_details,
 )
+from globus_compute_endpoint.logging_config import setup_logging
+from globus_compute_sdk.sdk.utils import get_env_details
+from globus_compute_sdk.serialize import ComputeSerializer
 
-logger = logging.getLogger(__name__)
+log = logging.getLogger(__name__)
 
+DEFAULT_RESULT_SIZE_LIMIT_MB = 10
+DEFAULT_RESULT_SIZE_LIMIT_B = DEFAULT_RESULT_SIZE_LIMIT_MB * 1024 * 1024
 
-class ReportingThread:
-    def __init__(
-        self, target: t.Callable, args: t.List, reporting_period: float = 30.0
-    ):
-        """This class wraps threading.Thread to run a callable in a loop
-        periodically until the user calls `stop`. A status attribute can
-        report exceptions to the parent thread upon failure.
-        Parameters
-        ----------
-        target: Target function to be invoked to get report and post to queue
-        args: args to be passed to target fn
-        kwargs: kwargs to be passed to target fn
-        reporting_period: float, defaults to 30.0s
-        """
-        self.status: Future = Future()
-        self._shutdown_event = threading.Event()
-        self.reporting_period = reporting_period
-        self._thread = threading.Thread(
-            target=self.run_in_loop, args=[target] + args, name="GCReportingThread"
-        )
 
-    def start(self):
-        logger.info("Start called")
-        self._thread.start()
+class Worker:
+    """The Globus Compute worker
+    Parameters
+    ----------
 
-    def run_in_loop(self, target: t.Callable, *args) -> None:
-        while True:
-            try:
-                target(*args)
-            except Exception as e:
-                # log and update future before exiting, if it is not already set
-                self.status.set_exception(exception=e)
-                self._shutdown_event.set()
-            if self._shutdown_event.wait(timeout=self.reporting_period):
-                break
-
-        logger.warning("ReportingThread exiting")
-
-    def stop(self) -> None:
-        self._shutdown_event.set()
-        self._thread.join(timeout=0.1)
-
-
-class GlobusComputeEngineBase(ABC):
-    """Shared functionality and interfaces required by all GlobusCompute Engines.
-    This is designed to plug-in executors following the concurrent.futures.Executor
-    interface as execution backends to GlobusCompute
+    worker_id : str
+     Worker id string
+
+    address : str
+     Address at which the manager might be reached. This is usually 127.0.0.1
+
+    port : int
+     Port at which the manager can be reached
+
+    result_size_limit : int
+     Maximum result size allowed in Bytes
+     Default = 10 MB
+
+    Globus Compute worker will use the REP sockets to:
+         task = recv ()
+         result = execute(task)
+         send(result)
     """
 
     def __init__(
         self,
-        *args: object,
-        endpoint_id: t.Optional[uuid.UUID] = None,
-        **kwargs: object,
+        worker_id,
+        address,
+        port,
+        worker_type="RAW",
+        result_size_limit=DEFAULT_RESULT_SIZE_LIMIT_B,
     ):
-        self._shutdown_event = threading.Event()
-        self.endpoint_id = endpoint_id
-
-        # remove these unused vars that we are adding to just keep
-        # endpoint interchange happy
-        self.container_type: t.Optional[str] = None
-        self.funcx_service_address: t.Optional[str] = None
-        self.run_dir: t.Optional[str] = None
-        # This attribute could be set by the subclasses in their
-        # start method if another component insists on owning the queue.
-        self.results_passthrough: queue.Queue[
-            dict[str, bytes | str | None]
-        ] = queue.Queue()
+        self.worker_id = worker_id
+        self.address = address
+        self.port = port
+        self.worker_type = worker_type
+        self.serializer = ComputeSerializer()
+        self.serialize = self.serializer.serialize
+        self.deserialize = self.serializer.deserialize
+        self.result_size_limit = result_size_limit
+
+        log.info(f"Initializing worker {worker_id}")
+        log.info(f"Worker is of type: {worker_type}")
+
+        self.context = zmq.Context()
+        self.poller = zmq.Poller()
+        self.identity = worker_id.encode()
+
+        self.task_socket = self.context.socket(zmq.DEALER)
+        self.task_socket.setsockopt(zmq.IDENTITY, self.identity)
+
+        log.info(f"Trying to connect to : tcp://{self.address}:{self.port}")
+        self.task_socket.connect(f"tcp://{self.address}:{self.port}")
+        self.poller.register(self.task_socket, zmq.POLLIN)
+        signal.signal(signal.SIGTERM, self.handler)
+
+    def handler(self, signum, frame):
+        log.error(f"Signal handler called with signal {signum}")
+        sys.exit(1)
+
+    def _send_registration_message(self):
+        log.debug("Sending registration")
+        payload = {"worker_id": self.worker_id, "worker_type": self.worker_type}
+        self.task_socket.send_multipart([b"REGISTER", dill.dumps(payload)])
 
-    @abstractmethod
-    def start(
-        self,
-        *args,
-        **kwargs,
-    ) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    def get_status_report(self) -> EPStatusReport:
-        raise NotImplementedError
-
-    def report_status(self) -> None:
-        status_report = self.get_status_report()
-        packed: bytes = messagepack.pack(status_report)
-        self.results_passthrough.put({"message": packed})
-
-    def _status_report(self, shutdown_event: threading.Event, heartbeat_period: float):
-        while not shutdown_event.wait(timeout=heartbeat_period):
-            status_report = self.get_status_report()
-            packed = messagepack.pack(status_report)
-            self.results_passthrough.put({"message": packed})
-
-    def _setup_future_done_callback(self, task_id: str, future: Future) -> None:
-        """
-        Set up the done() callback for the provided future.
-
-        The done callback handles
-        Callback to post result to the passthrough queue
-        Parameters
-        ----------
-        future: Future for which the callback is triggerd
-        """
-
-        exec_beg = TaskTransition(  # Reminder: used by *closure*, below
-            timestamp=time.time_ns(),
-            actor=ActorName.INTERCHANGE,
-            state=TaskState.WAITING_FOR_LAUNCH,
-        )
+    def start(self):
+        log.info("Starting worker")
+        self._send_registration_message()
 
-        def _done_cb(f: Future):
-            if f.exception():
-                exc = f.exception()
-                code, user_message = get_result_error_details(exc)
-                error_details = {"code": code, "user_message": user_message}
-                exec_end = TaskTransition(
-                    timestamp=time.time_ns(),
-                    actor=ActorName.INTERCHANGE,
-                    state=TaskState.EXEC_END,
-                )
-                result_message = dict(
-                    task_id=task_id,
-                    data=get_error_string(exc=exc),
-                    exception=get_error_string(exc=exc),
-                    error_details=error_details,
-                    task_statuses=[exec_beg, exec_end],  # only transition info we have
-                )
-                packed = messagepack.pack(Result(**result_message))
+        while True:
+            log.debug("Waiting for task")
+            p_task_id, p_container_id, msg = self.task_socket.recv_multipart()
+            task_id: str = dill.loads(p_task_id)
+            container_id: str = dill.loads(p_container_id)
+            log.debug(f"Received task with task_id='{task_id}' and msg='{msg}'")
+
+            if task_id == "KILL":
+                log.info("[KILL] -- Worker KILL message received! ")
+                # send a "worker die" message back to the manager
+                self.task_socket.send_multipart([b"WRKR_DIE", b""])
+                log.info(f"*** WORKER {self.worker_id} ABOUT TO DIE ***")
+                # Kill the worker after accepting death in message to manager.
+                sys.exit()
             else:
-                packed = f.result()
+                result = self._worker_execute_task(task_id, msg)
+                result["container_id"] = container_id
+                log.debug("Sending result")
+                # send bytes over the socket back to the manager
+                self.task_socket.send_multipart([b"TASK_RET", dill.dumps(result)])
+
+        log.warning("Broke out of the loop... dying")
+
+    def compose_exception_message(self, task_id: str) -> bytes:
+        code, user_message = get_result_error_details()
+        outgoing_result = OutgoingResult(
+            task_id=task_id,
+            data=get_error_string(),
+            error_details=OutgoingResultErrorDetails(
+                code=code,
+                user_message=user_message,
+            ),
+            details=get_env_details(),
+        )
+        return messagepack.pack(outgoing_result)
 
-            self.results_passthrough.put({"task_id": task_id, "message": packed})
+    def _worker_execute_task(
+        self, task_id: str, msg: bytes
+    ) -> dict[str, t.Union[str, bytes]]:
+        result_message: dict[str, t.Union[str, bytes]] = {"task_id": task_id}
+        try:
+            # Unwrap HTEX's Task packing
+            task_message = Message.unpack(msg)
+            serialized_fn_package = task_message.task_buffer.decode()
+
+            # Deserialize HTEX Engines' wrapping of
+            # execute_task, messagepack_payload)
+            function, args, kwargs = self.deserialize(serialized_fn_package)
+
+            # Execute
+            serialized_result: bytes = function(*args, **kwargs)
+            result_message["data"] = serialized_result
+
+        except Exception:
+            log.exception("Failed to execute task")
+            serialized_error = self.compose_exception_message(task_id)
+            result_message["data"] = serialized_error
+
+        return result_message
+
+
+def cli_run():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-w", "--worker_id", required=True, help="ID of worker from process_worker_pool"
+    )
+    parser.add_argument(
+        "-t", "--type", required=False, help="Container type of worker", default="RAW"
+    )
+    parser.add_argument(
+        "-a", "--address", required=True, help="Address for the manager, eg X,Y,"
+    )
+    parser.add_argument(
+        "-p",
+        "--port",
+        required=True,
+        help="Internal port at which the worker connects to the manager",
+    )
+    parser.add_argument(
+        "--logdir", required=True, help="Directory path where worker log files written"
+    )
+    parser.add_argument(
+        "-d",
+        "--debug",
+        action="store_true",
+        help="Directory path where worker log files written",
+    )
+    args = parser.parse_args()
+
+    setup_logging(
+        logfile=os.path.join(args.logdir, f"funcx_worker_{args.worker_id}.log"),
+        debug=args.debug,
+    )
+
+    # Redirect the stdout and stderr
+    stdout_path = os.path.join(args.logdir, f"funcx_worker_{args.worker_id}.stdout")
+    stderr_path = os.path.join(args.logdir, f"funcx_worker_{args.worker_id}.stderr")
+    with open(stdout_path, "w") as fo, open(stderr_path, "w") as fe:
+        # Redirect the stdout
+        old_stdout, old_stderr = sys.stdout, sys.stderr
+        sys.stdout = fo
+        sys.stderr = fe
+
+        try:
+            worker = Worker(
+                args.worker_id,
+                args.address,
+                int(args.port),
+                worker_type=args.type,
+            )
+            worker.start()
+        finally:
+            # Switch them back
+            sys.stdout = old_stdout
+            sys.stderr = old_stderr
 
-        future.add_done_callback(_done_cb)
 
-    @abstractmethod
-    def _submit(
-        self,
-        func: t.Callable,
-        *args: t.Any,
-        **kwargs: t.Any,
-    ) -> Future:
-        """Subclass should use the internal execution system to implement this"""
-        raise NotImplementedError()
-
-    def submit(self, task_id: str, packed_task: bytes) -> Future:
-        """GC Endpoints should submit tasks via this method so that tasks are
-        tracked properly.
-        Parameters
-        ----------
-        packed_task: messagepack bytes buffer
-        Returns
-        -------
-        future
-        """
-
-        future = self._submit(execute_task, task_id, packed_task)
-        self._setup_future_done_callback(task_id, future)
-        return future
-
-    @abstractmethod
-    def shutdown(self, /, **kwargs) -> None:
-        raise NotImplementedError()
+if __name__ == "__main__":
+    cli_run()
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/globus_compute.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/globus_compute.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,27 +20,32 @@
 
 
 class GlobusComputeEngine(GlobusComputeEngineBase):
     def __init__(
         self,
         *args,
         label: str = "GlobusComputeEngine",
+        max_retries_on_system_failure: int = 0,
         strategy: t.Optional[SimpleStrategy] = SimpleStrategy(),
         executor: t.Optional[HighThroughputExecutor] = None,
         **kwargs,
     ):
         self.run_dir = os.getcwd()
         self.label = label
         self._status_report_thread = ReportingThread(target=self.report_status, args=[])
-        super().__init__(*args, **kwargs)
+        super().__init__(
+            *args, max_retries_on_system_failure=max_retries_on_system_failure, **kwargs
+        )
         self.strategy = strategy
         self.max_workers_per_node = 1
         if executor is None:
             executor = HighThroughputExecutor(  # type: ignore
-                *args, label=label, **kwargs
+                *args,
+                label=label,
+                **kwargs,
             )
         self.executor = executor
 
     def start(
         self,
         *args,
         endpoint_id: t.Optional[uuid.UUID] = None,
@@ -209,14 +214,34 @@
         logger.info(f"Scaling out {blocks} blocks")
         return self.executor.scale_out(blocks=blocks)
 
     def scale_in(self, blocks: int):
         logger.info(f"Scaling in {blocks} blocks")
         return self.executor.scale_in(blocks=blocks)
 
+    def _handle_task_exception(
+        self,
+        task_id: str,
+        execution_begin: TaskTransition,
+        exception: BaseException,
+    ) -> bytes:
+        result_bytes = b""
+        retry_info = self._retry_table[task_id]
+        if retry_info["retry_count"] < self.max_retries_on_system_failure:
+            retry_info["retry_count"] += 1
+            retry_info["exception_history"].append(exception)
+            self.submit(task_id, retry_info["packed_task"])
+        else:
+            # This is a terminal state
+            result_bytes = super()._handle_task_exception(
+                task_id=task_id, execution_begin=execution_begin, exception=exception
+            )
+
+        return result_bytes
+
     @property
     def scaling_enabled(self) -> bool:
         """Indicates whether scaling is possible"""
         max_blocks = self.executor.provider.max_blocks
         return max_blocks > 0
 
     def get_status_report(self) -> EPStatusReport:
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/helper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/container_sched.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/engine.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/engine.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/interchange.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/manager.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/messages.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/worker_map.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/process_pool.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/process_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/engines/thread_pool.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/engines/thread_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/self_diagnostic.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/self_diagnostic.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import math
 import time
 
 from globus_compute_endpoint.strategies.base import BaseStrategy
-from parsl.providers.base import JobState
+from parsl.jobs.states import JobState
 
 log = logging.getLogger(__name__)
 
 
 class SimpleStrategy(BaseStrategy):
     """Implements the simple strategy"""
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.8.0a0"
+__version__ = "2.9.0"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.8.0a0
+Version: 2.9.0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
@@ -17,23 +17,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: globus-sdk
-Requires-Dist: globus-compute-sdk==2.8.0a0
+Requires-Dist: globus-compute-sdk==2.9.0
 Requires-Dist: globus-compute-common==0.3.0
 Requires-Dist: globus-identity-mapping==0.1.0
 Requires-Dist: texttable<2,>=1.6.4
 Requires-Dist: psutil<6
 Requires-Dist: python-daemon<3,>=2
 Requires-Dist: click<9,>=8
 Requires-Dist: pyzmq!=22.3.0,<=23.2.0,>=22.0.0
-Requires-Dist: parsl==2023.7.3
+Requires-Dist: parsl==2023.12.4
 Requires-Dist: pika>=1.2.0
 Requires-Dist: pyprctl<0.2.0
 Requires-Dist: setproctitle<1.4,>=1.3.2
 Requires-Dist: pyyaml<7.0,>=6.0
 Requires-Dist: jinja2<3.2,>=3.1.2
 Requires-Dist: jsonschema<4.20,>=4.19.0
 Requires-Dist: cachetools>=5.3.1
```

### Comparing `globus-compute-endpoint-2.8.0a0/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.9.0/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -75,11 +75,12 @@
 tests/utils.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/endpoint/__init__.py
 tests/integration/endpoint/conftest.py
 tests/integration/endpoint/executors/__init__.py
 tests/integration/endpoint/executors/mock_executors.py
+tests/integration/endpoint/executors/test_gcengine_retries.py
 tests/integration/endpoint/executors/high_throughput/__init__.py
 tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
 tests/integration/endpoint/executors/high_throughput/test_manager.py
 tests/integration/endpoint/executors/high_throughput/test_worker_map.py
```

### Comparing `globus-compute-endpoint-2.8.0a0/setup.py` & `globus-compute-endpoint-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.31.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.8.0a0",
+    "globus-compute-sdk==2.9.0",
     "globus-compute-common==0.3.0",
     "globus-identity-mapping==0.1.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
@@ -30,15 +30,15 @@
     # building from source, which may mean there's an issue in the packaged library
     # further investigation may be needed if the issue persists in the next pyzmq
     # release
     "pyzmq>=22.0.0,!=22.3.0,<=23.2.0",
     # 'parsl' is a core requirement of the globus-compute-endpoint, essential to a range
     # of different features and functions
     # pin exact versions because it does not use semver
-    "parsl==2023.7.3",
+    "parsl==2023.12.4",
     "pika>=1.2.0",
     "pyprctl<0.2.0",
     "setproctitle>=1.3.2,<1.4",
     "pyyaml>=6.0,<7.0",
     "jinja2>=3.1.2,<3.2",
     "jsonschema>=4.19.0,<4.20",
     "cachetools>=5.3.1",
```

### Comparing `globus-compute-endpoint-2.8.0a0/tests/conftest.py` & `globus-compute-endpoint-2.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/tests/integration/conftest.py` & `globus-compute-endpoint-2.9.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/conftest.py` & `globus-compute-endpoint-2.9.0/tests/integration/endpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py` & `globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/test_manager.py` & `globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/test_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py` & `globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.8.0a0/tests/integration/endpoint/executors/mock_executors.py` & `globus-compute-endpoint-2.9.0/tests/integration/endpoint/executors/mock_executors.py`

 * *Files identical despite different names*

