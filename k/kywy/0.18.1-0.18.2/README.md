# Comparing `tmp/kywy-0.18.1.tar.gz` & `tmp/kywy-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kywy-0.18.1.tar", last modified: Fri May 24 20:21:20 2024, max compression
+gzip compressed data, was "kywy-0.18.2.tar", last modified: Wed May 29 20:14:41 2024, max compression
```

## Comparing `kywy-0.18.1.tar` & `kywy-0.18.2.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.326760 kywy-0.18.1/
--rw-r--r--   0 emmanuel   (501) staff       (20)     1605 2024-05-24 20:21:20.326533 kywy-0.18.1/PKG-INFO
--rw-r--r--   0 emmanuel   (501) staff       (20)      932 2024-05-10 18:10:19.000000 kywy-0.18.1/README.md
--rw-r--r--   0 emmanuel   (501) staff       (20)      876 2024-05-22 13:45:23.000000 kywy-0.18.1/pyproject.toml
--rw-r--r--   0 emmanuel   (501) staff       (20)       38 2024-05-24 20:21:20.326802 kywy-0.18.1/setup.cfg
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.308581 kywy-0.18.1/src/
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.309613 kywy-0.18.1/src/kywy/
--rw-r--r--   0 emmanuel   (501) staff       (20)       23 2024-05-24 20:21:03.000000 kywy-0.18.1/src/kywy/__init__.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.316732 kywy-0.18.1/src/kywy/client/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     7823 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/benchmark.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     1024 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/chat.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    29733 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/commands.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     7390 2024-05-23 19:57:26.000000 kywy-0.18.1/src/kywy/client/computation_nodes.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      947 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/configuration.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    18930 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/data.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     5624 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/data_generator.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    16164 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/client/data_loader.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      909 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/data_providers.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    18360 2024-05-17 20:49:05.000000 kywy-0.18.1/src/kywy/client/dsl.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     3792 2024-05-14 17:52:23.000000 kywy-0.18.1/src/kywy/client/entities.py
--rw-r--r--   0 emmanuel   (501) staff       (20)       41 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/errors.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    24567 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/generator.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    12868 2024-05-23 22:48:59.000000 kywy-0.18.1/src/kywy/client/kawa_client.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     1217 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/kawa_decorators.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      255 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/kawa_types.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    17494 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/client/layout_builder.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.317542 kywy-0.18.1/src/kywy/test/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-23 22:48:35.000000 kywy-0.18.1/src/kywy/test/__init__.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.319022 kywy-0.18.1/src/kywy/test/computation/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/__init__.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.320313 kywy-0.18.1/src/kywy/test/computation/filtering/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/filtering/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     3777 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/filtering/test_computation_with_number_filters.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     6783 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/filtering/test_computation_with_temporal_filters.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     4929 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/filtering/test_computation_with_text_filters.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     2328 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/filtering/test_multiple_filter_clauses.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.320573 kywy-0.18.1/src/kywy/test/computation/sorting/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/sorting/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     7352 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/sorting/test_computation_sorting.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     5062 2024-05-22 13:45:23.000000 kywy-0.18.1/src/kywy/test/computation/test_computation_alias.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    17502 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/computation/test_computation_dsl.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    11148 2024-05-23 18:02:10.000000 kywy-0.18.1/src/kywy/test/computation/test_multiple_levels_of_grouping.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     8837 2024-05-22 13:45:23.000000 kywy-0.18.1/src/kywy/test/computation/test_sampling.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.321215 kywy-0.18.1/src/kywy/test/gen_ai/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/gen_ai/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     2929 2024-05-23 18:00:42.000000 kywy-0.18.1/src/kywy/test/gen_ai/test_gen_ai_chart.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     1028 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/kawa_base_e2e_test.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.323053 kywy-0.18.1/src/kywy/test/loading_and_ddl/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/loading_and_ddl/__init__.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     1886 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/loading_and_ddl/test_data_generator.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    36520 2024-05-22 13:45:23.000000 kywy-0.18.1/src/kywy/test/loading_and_ddl/test_data_loader.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    13616 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/loading_and_ddl/test_delete_data.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     7921 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/loading_and_ddl/test_partition_management.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.323413 kywy-0.18.1/src/kywy/test/python_columns/
--rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.1/src/kywy/test/python_columns/__init__.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.325936 kywy-0.18.1/src/kywy/test/python_columns/resources/
--rw-r--r--   0 emmanuel   (501) staff       (20)      357 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_script_measure1.py
--rw-r--r--   0 emmanuel   (501) staff       (20)     1458 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_script_with_all_types.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      353 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_with_error_when_executing.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      339 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_with_no_pk_in_params.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      441 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_with_no_pk_in_params_with_logging.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      250 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_with_pk_in_params.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      298 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_with_secret.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      488 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_script_with_missing_arguments_will_throw_error.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      637 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_script_with_two_functions_will_throw_error.py
--rw-r--r--   0 emmanuel   (501) staff       (20)      334 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/resources/test_script_without_any_function_with_inputs.py
--rw-r--r--   0 emmanuel   (501) staff       (20)    22539 2024-05-24 20:20:07.000000 kywy-0.18.1/src/kywy/test/python_columns/test_python_column.py
-drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-24 20:21:20.326231 kywy-0.18.1/src/kywy.egg-info/
--rw-r--r--   0 emmanuel   (501) staff       (20)     1605 2024-05-24 20:21:20.000000 kywy-0.18.1/src/kywy.egg-info/PKG-INFO
--rw-r--r--   0 emmanuel   (501) staff       (20)     2776 2024-05-24 20:21:20.000000 kywy-0.18.1/src/kywy.egg-info/SOURCES.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        1 2024-05-24 20:21:20.000000 kywy-0.18.1/src/kywy.egg-info/dependency_links.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)      198 2024-05-24 20:21:20.000000 kywy-0.18.1/src/kywy.egg-info/requires.txt
--rw-r--r--   0 emmanuel   (501) staff       (20)        5 2024-05-24 20:21:20.000000 kywy-0.18.1/src/kywy.egg-info/top_level.txt
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.165151 kywy-0.18.2/
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1605 2024-05-29 20:14:41.164913 kywy-0.18.2/PKG-INFO
+-rw-r--r--   0 emmanuel   (501) staff       (20)      932 2024-05-10 18:10:19.000000 kywy-0.18.2/README.md
+-rw-r--r--   0 emmanuel   (501) staff       (20)      876 2024-05-22 13:45:23.000000 kywy-0.18.2/pyproject.toml
+-rw-r--r--   0 emmanuel   (501) staff       (20)       38 2024-05-29 20:14:41.165203 kywy-0.18.2/setup.cfg
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.139951 kywy-0.18.2/src/
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.141194 kywy-0.18.2/src/kywy/
+-rw-r--r--   0 emmanuel   (501) staff       (20)       23 2024-05-29 20:12:26.000000 kywy-0.18.2/src/kywy/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.156133 kywy-0.18.2/src/kywy/client/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     7823 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/benchmark.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1024 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/chat.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    29733 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/commands.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     7390 2024-05-23 19:57:26.000000 kywy-0.18.2/src/kywy/client/computation_nodes.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      947 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/configuration.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    18930 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/data.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     5624 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/data_generator.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    16613 2024-05-29 19:19:54.000000 kywy-0.18.2/src/kywy/client/data_loader.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      909 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/data_providers.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    19498 2024-05-29 19:29:42.000000 kywy-0.18.2/src/kywy/client/dsl.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     3792 2024-05-14 17:52:23.000000 kywy-0.18.2/src/kywy/client/entities.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)       41 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/errors.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    24567 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/generator.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    12868 2024-05-23 22:48:59.000000 kywy-0.18.2/src/kywy/client/kawa_client.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1217 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/kawa_decorators.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      255 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/kawa_types.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    17494 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/client/layout_builder.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.156564 kywy-0.18.2/src/kywy/test/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-23 22:48:35.000000 kywy-0.18.2/src/kywy/test/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.158172 kywy-0.18.2/src/kywy/test/computation/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.159476 kywy-0.18.2/src/kywy/test/computation/filtering/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/filtering/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     3777 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/filtering/test_computation_with_number_filters.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     6783 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/filtering/test_computation_with_temporal_filters.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     4929 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/filtering/test_computation_with_text_filters.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     2328 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/filtering/test_multiple_filter_clauses.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.159712 kywy-0.18.2/src/kywy/test/computation/sorting/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/sorting/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     7352 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/sorting/test_computation_sorting.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     5062 2024-05-29 18:54:28.000000 kywy-0.18.2/src/kywy/test/computation/test_computation_alias.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    17502 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/computation/test_computation_dsl.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     3043 2024-05-29 19:33:38.000000 kywy-0.18.2/src/kywy/test/computation/test_computation_sheet_profiling.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    11148 2024-05-23 18:02:10.000000 kywy-0.18.2/src/kywy/test/computation/test_multiple_levels_of_grouping.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     8837 2024-05-22 13:45:23.000000 kywy-0.18.2/src/kywy/test/computation/test_sampling.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.160268 kywy-0.18.2/src/kywy/test/gen_ai/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/gen_ai/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     2929 2024-05-23 18:00:42.000000 kywy-0.18.2/src/kywy/test/gen_ai/test_gen_ai_chart.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1028 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/kawa_base_e2e_test.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.161713 kywy-0.18.2/src/kywy/test/loading_and_ddl/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/loading_and_ddl/__init__.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1886 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/loading_and_ddl/test_data_generator.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    36520 2024-05-22 13:45:23.000000 kywy-0.18.2/src/kywy/test/loading_and_ddl/test_data_loader.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    13616 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/loading_and_ddl/test_delete_data.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     7921 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/loading_and_ddl/test_partition_management.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.162120 kywy-0.18.2/src/kywy/test/python_columns/
+-rw-r--r--   0 emmanuel   (501) staff       (20)        0 2024-05-10 18:10:19.000000 kywy-0.18.2/src/kywy/test/python_columns/__init__.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.164433 kywy-0.18.2/src/kywy/test/python_columns/resources/
+-rw-r--r--   0 emmanuel   (501) staff       (20)      357 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_script_measure1.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1458 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_script_with_all_types.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      353 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_with_error_when_executing.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      339 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_with_no_pk_in_params.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      441 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_with_no_pk_in_params_with_logging.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      250 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_with_pk_in_params.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      298 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_with_secret.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      488 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_script_with_missing_arguments_will_throw_error.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      637 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_script_with_two_functions_will_throw_error.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)      334 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/resources/test_script_without_any_function_with_inputs.py
+-rw-r--r--   0 emmanuel   (501) staff       (20)    22539 2024-05-24 20:20:07.000000 kywy-0.18.2/src/kywy/test/python_columns/test_python_column.py
+drwxr-xr-x   0 emmanuel   (501) staff       (20)        0 2024-05-29 20:14:41.164636 kywy-0.18.2/src/kywy.egg-info/
+-rw-r--r--   0 emmanuel   (501) staff       (20)     1605 2024-05-29 20:14:41.000000 kywy-0.18.2/src/kywy.egg-info/PKG-INFO
+-rw-r--r--   0 emmanuel   (501) staff       (20)     2838 2024-05-29 20:14:41.000000 kywy-0.18.2/src/kywy.egg-info/SOURCES.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)        1 2024-05-29 20:14:41.000000 kywy-0.18.2/src/kywy.egg-info/dependency_links.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)      198 2024-05-29 20:14:41.000000 kywy-0.18.2/src/kywy.egg-info/requires.txt
+-rw-r--r--   0 emmanuel   (501) staff       (20)        5 2024-05-29 20:14:41.000000 kywy-0.18.2/src/kywy.egg-info/top_level.txt
```

### Comparing `kywy-0.18.1/PKG-INFO` & `kywy-0.18.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kywy
-Version: 0.18.1
+Version: 0.18.2
 Summary: Python client for Kawa - https://docs.kawa.ai
 Author-email: Kawa Analytics <emmmanuel@kawa.ai>, Kawa Analytics <max@kawa.ai>
 Maintainer-email: Kawa Analytics <max@kawa.ai>, Kawa Analytics <emmmanuel@kawa.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.21.3
 Requires-Dist: pandas>=1.3.4
```

### Comparing `kywy-0.18.1/README.md` & `kywy-0.18.2/README.md`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/pyproject.toml` & `kywy-0.18.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/benchmark.py` & `kywy-0.18.2/src/kywy/client/benchmark.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/chat.py` & `kywy-0.18.2/src/kywy/client/chat.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/commands.py` & `kywy-0.18.2/src/kywy/client/commands.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/computation_nodes.py` & `kywy-0.18.2/src/kywy/client/computation_nodes.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/configuration.py` & `kywy-0.18.2/src/kywy/client/configuration.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/data.py` & `kywy-0.18.2/src/kywy/client/data.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/data_generator.py` & `kywy-0.18.2/src/kywy/client/data_generator.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/data_loader.py` & `kywy-0.18.2/src/kywy/client/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,14 +285,24 @@
                         df[column_name] = df[column_name].map(lambda x: int(x.timestamp() * 1000) if x else None)
                     except ValueError as e:
                         # todo:
                         #  fix 'ValueError: The truth value of a DatetimeIndex is ambiguous.
                         #  Use a.empty, a.bool(), a.item(), a.any() or a.all()'
                         traceback.print_exc()
 
+        # Replace None/NaN with empty strings in text columns
+        text_column_names = []
+        text_indicators = [i for i in indicators if i.get('type') == 'text']
+        for text_indicator in text_indicators:
+            column_name = text_indicator.get('indicatorId')
+            if column_name in df.columns:
+                text_column_names.append(column_name)
+
+        df.fillna(value={v: '' for v in text_column_names}, inplace=True)
+
         # Call prepare data that will check if we can start loading and give us the offset for automatic index
         prepare_data = self._k.post(url=prepare_url, data={})
 
         if not prepare_data.get('canRunLoading'):
             raise Exception(
                 'We cannot start ingestion due to: ' + prepare_data.get('raisonItCannotStart', 'No reason given'))
```

### Comparing `kywy-0.18.1/src/kywy/client/data_providers.py` & `kywy-0.18.2/src/kywy/client/data_providers.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/dsl.py` & `kywy-0.18.2/src/kywy/client/dsl.py`

 * *Files 6% similar despite different names*

```diff
@@ -522,23 +522,50 @@
             for group_id, group_name in enumerate(self._group_by):
                 prev_name = f'grouping({group_id})'
                 new_name = f'group({group_id}) {group_name}'
                 df.rename(columns={prev_name: new_name}, inplace=True)
 
         return df
 
-    def schema(self):
-        sheet = self._k.entities.sheets().get_entity(self._sheet_name)
-        if not sheet:
-            raise Exception('Sheet with name {} was not found in the current workspace'.format(self._sheet_name))
+    def profile(self, column_name: typing.Optional[str] = None):
+        sheet = self._load_sheet()
+        all_columns = sheet.get('indicatorColumns', []) + sheet.get('computedColumns', [])
+        data = {
+            'sheetId': sheet.get('id'),
+        }
+
+        if column_name:
+            for c in all_columns:
+                if c['displayInformation']['displayName'] == column_name:
+                    data['columnId'] = c['columnId']
+
+        sheet_profile = self._k.post(
+            url=f'{self._k.kawa_api_url}/computation/compute-sheet-stats',
+            data=data,
+        )
+
+        profile_with_column_names = {}
+        for column_id, column_profile in sheet_profile.items():
+            matching_column_names = [
+                c['displayInformation']['displayName']
+                for c in all_columns
+                if c['columnId'] == column_id]
+
+            if matching_column_names:
+                profile_with_column_names[matching_column_names[0]] = column_profile
 
+        return profile_with_column_names
+
+    def schema(self):
+        sheet = self._load_sheet()
         indicator_columns = sheet.get('indicatorColumns', [])
         computed_columns = sheet.get('computedColumns', [])
 
-        return [{c['displayInformation']['displayName']: c['type']} for c in [*indicator_columns, *computed_columns]]
+        return [{c['displayInformation']['displayName']: c['type']} for c in
+                [*indicator_columns, *computed_columns]]
 
     def _transform_to_dict(self, skip_cache=False, ):
 
         body = {
             'sheetName': self._sheet_name,
             'timeZone': self._tz,
             'limit': self._limit,
@@ -567,7 +594,13 @@
         if self._view_id:
             body['viewId'] = self._view_id
 
         if self._as_user_id:
             body['asUserId'] = self._as_user_id
 
         return body
+
+    def _load_sheet(self):
+        sheet = self._k.entities.sheets().get_entity(self._sheet_name)
+        if not sheet:
+            raise Exception('Sheet with name {} was not found in the current workspace'.format(self._sheet_name))
+        return sheet
```

### Comparing `kywy-0.18.1/src/kywy/client/entities.py` & `kywy-0.18.2/src/kywy/client/entities.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/generator.py` & `kywy-0.18.2/src/kywy/client/generator.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/kawa_client.py` & `kywy-0.18.2/src/kywy/client/kawa_client.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/kawa_decorators.py` & `kywy-0.18.2/src/kywy/client/kawa_decorators.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/client/layout_builder.py` & `kywy-0.18.2/src/kywy/client/layout_builder.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/filtering/test_computation_with_number_filters.py` & `kywy-0.18.2/src/kywy/test/computation/filtering/test_computation_with_number_filters.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/filtering/test_computation_with_temporal_filters.py` & `kywy-0.18.2/src/kywy/test/computation/filtering/test_computation_with_temporal_filters.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/filtering/test_computation_with_text_filters.py` & `kywy-0.18.2/src/kywy/test/computation/filtering/test_computation_with_text_filters.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/filtering/test_multiple_filter_clauses.py` & `kywy-0.18.2/src/kywy/test/computation/filtering/test_multiple_filter_clauses.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/sorting/test_computation_sorting.py` & `kywy-0.18.2/src/kywy/test/computation/sorting/test_computation_sorting.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/test_computation_alias.py` & `kywy-0.18.2/src/kywy/test/computation/test_computation_alias.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/test_computation_dsl.py` & `kywy-0.18.2/src/kywy/test/computation/test_computation_dsl.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/test_multiple_levels_of_grouping.py` & `kywy-0.18.2/src/kywy/test/computation/test_multiple_levels_of_grouping.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/computation/test_sampling.py` & `kywy-0.18.2/src/kywy/test/computation/test_sampling.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/gen_ai/test_gen_ai_chart.py` & `kywy-0.18.2/src/kywy/test/gen_ai/test_gen_ai_chart.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/kawa_base_e2e_test.py` & `kywy-0.18.2/src/kywy/test/kawa_base_e2e_test.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/loading_and_ddl/test_data_generator.py` & `kywy-0.18.2/src/kywy/test/loading_and_ddl/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/loading_and_ddl/test_data_loader.py` & `kywy-0.18.2/src/kywy/test/loading_and_ddl/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/loading_and_ddl/test_delete_data.py` & `kywy-0.18.2/src/kywy/test/loading_and_ddl/test_delete_data.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/loading_and_ddl/test_partition_management.py` & `kywy-0.18.2/src/kywy/test/loading_and_ddl/test_partition_management.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/python_columns/resources/test_python_columns_script_with_all_types.py` & `kywy-0.18.2/src/kywy/test/python_columns/resources/test_python_columns_script_with_all_types.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/python_columns/resources/test_script_with_two_functions_will_throw_error.py` & `kywy-0.18.2/src/kywy/test/python_columns/resources/test_script_with_two_functions_will_throw_error.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy/test/python_columns/test_python_column.py` & `kywy-0.18.2/src/kywy/test/python_columns/test_python_column.py`

 * *Files identical despite different names*

### Comparing `kywy-0.18.1/src/kywy.egg-info/PKG-INFO` & `kywy-0.18.2/src/kywy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kywy
-Version: 0.18.1
+Version: 0.18.2
 Summary: Python client for Kawa - https://docs.kawa.ai
 Author-email: Kawa Analytics <emmmanuel@kawa.ai>, Kawa Analytics <max@kawa.ai>
 Maintainer-email: Kawa Analytics <max@kawa.ai>, Kawa Analytics <emmmanuel@kawa.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.21.3
 Requires-Dist: pandas>=1.3.4
```

### Comparing `kywy-0.18.1/src/kywy.egg-info/SOURCES.txt` & `kywy-0.18.2/src/kywy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/kywy/client/kawa_types.py
 src/kywy/client/layout_builder.py
 src/kywy/test/__init__.py
 src/kywy/test/kawa_base_e2e_test.py
 src/kywy/test/computation/__init__.py
 src/kywy/test/computation/test_computation_alias.py
 src/kywy/test/computation/test_computation_dsl.py
+src/kywy/test/computation/test_computation_sheet_profiling.py
 src/kywy/test/computation/test_multiple_levels_of_grouping.py
 src/kywy/test/computation/test_sampling.py
 src/kywy/test/computation/filtering/__init__.py
 src/kywy/test/computation/filtering/test_computation_with_number_filters.py
 src/kywy/test/computation/filtering/test_computation_with_temporal_filters.py
 src/kywy/test/computation/filtering/test_computation_with_text_filters.py
 src/kywy/test/computation/filtering/test_multiple_filter_clauses.py
```

