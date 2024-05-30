# Comparing `tmp/neurosym-0.0.8.tar.gz` & `tmp/neurosym-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurosym-0.0.8.tar", last modified: Mon Nov  6 16:23:39 2023, max compression
+gzip compressed data, was "neurosym-0.0.9.tar", last modified: Mon Nov  6 16:32:28 2023, max compression
```

## Comparing `neurosym-0.0.8.tar` & `neurosym-0.0.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.513058 neurosym-0.0.8/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      619 2023-11-06 16:23:39.513058 neurosym-0.0.8/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      212 2023-10-30 21:25:26.000000 neurosym-0.0.8/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      816 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/__init__.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/compression/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       81 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/compression/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     6386 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/compression/process_abstraction.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/datasets/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       57 2023-11-06 16:11:13.000000 neurosym-0.0.8/neurosym/datasets/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     4125 2023-11-06 16:10:33.000000 neurosym-0.0.8/neurosym/datasets/load_data.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      265 2023-10-31 04:20:09.000000 neurosym-0.0.8/neurosym/datasets/near_data_example.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/dsl/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:26:35.000000 neurosym-0.0.8/neurosym/dsl/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2796 2023-11-06 16:20:55.000000 neurosym-0.0.8/neurosym/dsl/abstraction.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     6899 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/dsl/dsl.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     9296 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/dsl/dsl_factory.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2373 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/dsl/lambdas.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3769 2023-10-30 22:10:17.000000 neurosym-0.0.8/neurosym/dsl/pcfg.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     6090 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/dsl/production.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/examples/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      141 2023-10-31 04:24:49.000000 neurosym-0.0.8/neurosym/examples/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      355 2023-10-31 00:36:15.000000 neurosym-0.0.8/neurosym/examples/basic_arith.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/examples/dreamcoder/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       35 2023-10-31 04:24:49.000000 neurosym-0.0.8/neurosym/examples/dreamcoder/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3457 2023-10-30 22:18:00.000000 neurosym-0.0.8/neurosym/examples/dreamcoder/list_example.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1011 2023-10-31 04:24:49.000000 neurosym-0.0.8/neurosym/examples/mutable_arith_combinators.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/examples/near/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      563 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/examples/near/__init__.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/examples/near/dsls/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:20:43.000000 neurosym-0.0.8/neurosym/examples/near/dsls/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1442 2023-11-06 16:20:55.000000 neurosym-0.0.8/neurosym/examples/near/dsls/sequential_differentiable_dsl.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1187 2023-10-31 03:56:51.000000 neurosym-0.0.8/neurosym/examples/near/dsls/simple_differentiable_dsl.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/examples/near/methods/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:22:02.000000 neurosym-0.0.8/neurosym/examples/near/methods/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     6260 2023-10-31 03:56:51.000000 neurosym-0.0.8/neurosym/examples/near/methods/base_trainer.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     6359 2023-11-06 16:17:35.000000 neurosym-0.0.8/neurosym/examples/near/methods/near_example_trainer.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     4629 2023-10-31 03:56:51.000000 neurosym-0.0.8/neurosym/examples/near/neural_dsl.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/examples/near/operations/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       70 2023-10-31 03:56:51.000000 neurosym-0.0.8/neurosym/examples/near/operations/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      408 2023-11-06 16:04:40.000000 neurosym-0.0.8/neurosym/examples/near/operations/basic.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      662 2023-10-31 03:56:51.000000 neurosym-0.0.8/neurosym/examples/near/operations/lists.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      942 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/examples/near/search_graph.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym/programs/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:20:58.000000 neurosym-0.0.8/neurosym/programs/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1825 2023-10-30 22:26:55.000000 neurosym-0.0.8/neurosym/programs/hole.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      694 2023-08-30 22:20:39.000000 neurosym-0.0.8/neurosym/programs/s_expression.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3348 2023-10-31 04:24:49.000000 neurosym-0.0.8/neurosym/programs/s_expression_render.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/neurosym/search/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      101 2023-10-31 04:24:49.000000 neurosym-0.0.8/neurosym/search/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1351 2023-10-31 04:24:49.000000 neurosym-0.0.8/neurosym/search/astar_search.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      670 2023-10-31 04:24:49.000000 neurosym-0.0.8/neurosym/search/bfs_search.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1550 2023-10-30 22:02:32.000000 neurosym-0.0.8/neurosym/search/bounded_astar.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/neurosym/search_graph/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:19:13.000000 neurosym-0.0.8/neurosym/search_graph/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2631 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/search_graph/dsl_search_graph.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      334 2023-10-31 00:50:47.000000 neurosym-0.0.8/neurosym/search_graph/dsl_search_node.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      860 2023-10-31 00:52:43.000000 neurosym-0.0.8/neurosym/search_graph/hole_set_chooser.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      735 2023-10-30 22:25:17.000000 neurosym-0.0.8/neurosym/search_graph/metadata_computer.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      324 2023-06-07 01:19:53.000000 neurosym-0.0.8/neurosym/search_graph/search_graph.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      919 2023-10-30 22:02:32.000000 neurosym-0.0.8/neurosym/search_graph/search_graph_transformer.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/neurosym/types/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:17:46.000000 neurosym-0.0.8/neurosym/types/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     8841 2023-10-30 22:20:59.000000 neurosym-0.0.8/neurosym/types/type.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)    11732 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/types/type_signature.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3853 2023-11-06 16:22:30.000000 neurosym-0.0.8/neurosym/types/type_string_repr.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2851 2023-10-30 22:24:03.000000 neurosym-0.0.8/neurosym/types/type_with_environment.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/neurosym/utils/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-19 01:53:03.000000 neurosym-0.0.8/neurosym/utils/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2022 2023-10-30 22:31:57.000000 neurosym-0.0.8/neurosym/utils/tree_trie.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.505058 neurosym-0.0.8/neurosym.egg-info/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      619 2023-11-06 16:23:39.000000 neurosym-0.0.8/neurosym.egg-info/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2724 2023-11-06 16:23:39.000000 neurosym-0.0.8/neurosym.egg-info/SOURCES.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-11-06 16:23:39.000000 neurosym-0.0.8/neurosym.egg-info/dependency_links.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      127 2023-11-06 16:23:39.000000 neurosym-0.0.8/neurosym.egg-info/requires.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       15 2023-11-06 16:23:39.000000 neurosym-0.0.8/neurosym.egg-info/top_level.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-11-06 16:23:39.513058 neurosym-0.0.8/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      911 2023-11-06 16:22:20.000000 neurosym-0.0.8/setup.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/tests/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-30 23:29:31.000000 neurosym-0.0.8/tests/__init__.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/tests/basic_search/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.8/tests/basic_search/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2618 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/basic_search/search_test.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/tests/dreamcoder/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.8/tests/dreamcoder/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3286 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/dreamcoder/compression_test.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1317 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/dreamcoder/list_dsl_test.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/tests/dsl/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.8/tests/dsl/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      504 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/dsl/rules_test.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/tests/lambdas/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-09-28 01:53:12.000000 neurosym-0.0.8/tests/lambdas/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3544 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/lambdas/enumeration_regression_test.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     8908 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/lambdas/lambdas_test.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.509058 neurosym-0.0.8/tests/near/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.8/tests/near/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1205 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/near/test_modules.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     4612 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/near/test_sequential_dsl.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3361 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/near/test_simple_dsl.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      714 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/near/utils.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1070 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/only_direct_import_test.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.513058 neurosym-0.0.8/tests/templates/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.8/tests/templates/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)    15777 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/templates/expansion_test.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1977 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/templates/semantics_test.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:23:39.513058 neurosym-0.0.8/tests/type/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-09-28 01:53:12.000000 neurosym-0.0.8/tests/type/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     7005 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/type/render_test.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3680 2023-10-31 04:24:49.000000 neurosym-0.0.8/tests/type/unify_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.273190 neurosym-0.0.9/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      619 2023-11-06 16:32:28.273190 neurosym-0.0.9/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      212 2023-10-30 21:25:26.000000 neurosym-0.0.9/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      816 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/__init__.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym/compression/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       81 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/compression/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     6386 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/compression/process_abstraction.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym/datasets/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       57 2023-11-06 16:11:13.000000 neurosym-0.0.9/neurosym/datasets/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     4125 2023-11-06 16:10:33.000000 neurosym-0.0.9/neurosym/datasets/load_data.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      265 2023-10-31 04:20:09.000000 neurosym-0.0.9/neurosym/datasets/near_data_example.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym/dsl/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:26:35.000000 neurosym-0.0.9/neurosym/dsl/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2796 2023-11-06 16:20:55.000000 neurosym-0.0.9/neurosym/dsl/abstraction.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     6899 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/dsl/dsl.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     9296 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/dsl/dsl_factory.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2373 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/dsl/lambdas.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3769 2023-10-30 22:10:17.000000 neurosym-0.0.9/neurosym/dsl/pcfg.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     6090 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/dsl/production.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym/examples/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      141 2023-10-31 04:24:49.000000 neurosym-0.0.9/neurosym/examples/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      355 2023-10-31 00:36:15.000000 neurosym-0.0.9/neurosym/examples/basic_arith.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym/examples/dreamcoder/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       35 2023-10-31 04:24:49.000000 neurosym-0.0.9/neurosym/examples/dreamcoder/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3457 2023-10-30 22:18:00.000000 neurosym-0.0.9/neurosym/examples/dreamcoder/list_example.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1011 2023-10-31 04:24:49.000000 neurosym-0.0.9/neurosym/examples/mutable_arith_combinators.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym/examples/near/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      490 2023-11-06 16:32:11.000000 neurosym-0.0.9/neurosym/examples/near/__init__.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/examples/near/dsls/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:20:43.000000 neurosym-0.0.9/neurosym/examples/near/dsls/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1442 2023-11-06 16:20:55.000000 neurosym-0.0.9/neurosym/examples/near/dsls/sequential_differentiable_dsl.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1187 2023-10-31 03:56:51.000000 neurosym-0.0.9/neurosym/examples/near/dsls/simple_differentiable_dsl.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/examples/near/methods/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:27:51.000000 neurosym-0.0.9/neurosym/examples/near/methods/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     6260 2023-10-31 03:56:51.000000 neurosym-0.0.9/neurosym/examples/near/methods/base_trainer.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     6359 2023-11-06 16:31:48.000000 neurosym-0.0.9/neurosym/examples/near/methods/near_example_trainer.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     4629 2023-10-31 03:56:51.000000 neurosym-0.0.9/neurosym/examples/near/neural_dsl.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/examples/near/operations/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       70 2023-10-31 03:56:51.000000 neurosym-0.0.9/neurosym/examples/near/operations/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      408 2023-11-06 16:04:40.000000 neurosym-0.0.9/neurosym/examples/near/operations/basic.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      662 2023-10-31 03:56:51.000000 neurosym-0.0.9/neurosym/examples/near/operations/lists.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      942 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/examples/near/search_graph.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/programs/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:20:58.000000 neurosym-0.0.9/neurosym/programs/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1825 2023-10-30 22:26:55.000000 neurosym-0.0.9/neurosym/programs/hole.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      694 2023-08-30 22:20:39.000000 neurosym-0.0.9/neurosym/programs/s_expression.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3348 2023-10-31 04:24:49.000000 neurosym-0.0.9/neurosym/programs/s_expression_render.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/search/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      101 2023-10-31 04:24:49.000000 neurosym-0.0.9/neurosym/search/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1351 2023-10-31 04:24:49.000000 neurosym-0.0.9/neurosym/search/astar_search.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      670 2023-10-31 04:24:49.000000 neurosym-0.0.9/neurosym/search/bfs_search.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1550 2023-10-30 22:02:32.000000 neurosym-0.0.9/neurosym/search/bounded_astar.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/search_graph/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:19:13.000000 neurosym-0.0.9/neurosym/search_graph/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2631 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/search_graph/dsl_search_graph.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      334 2023-10-31 00:50:47.000000 neurosym-0.0.9/neurosym/search_graph/dsl_search_node.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      860 2023-10-31 00:52:43.000000 neurosym-0.0.9/neurosym/search_graph/hole_set_chooser.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      735 2023-10-30 22:25:17.000000 neurosym-0.0.9/neurosym/search_graph/metadata_computer.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      324 2023-06-07 01:19:53.000000 neurosym-0.0.9/neurosym/search_graph/search_graph.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      919 2023-10-30 22:02:32.000000 neurosym-0.0.9/neurosym/search_graph/search_graph_transformer.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/types/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-06-07 01:17:46.000000 neurosym-0.0.9/neurosym/types/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     8841 2023-10-30 22:20:59.000000 neurosym-0.0.9/neurosym/types/type.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)    11732 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/types/type_signature.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3853 2023-11-06 16:22:30.000000 neurosym-0.0.9/neurosym/types/type_string_repr.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2851 2023-10-30 22:24:03.000000 neurosym-0.0.9/neurosym/types/type_with_environment.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/neurosym/utils/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-19 01:53:03.000000 neurosym-0.0.9/neurosym/utils/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2022 2023-10-30 22:31:57.000000 neurosym-0.0.9/neurosym/utils/tree_trie.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.265190 neurosym-0.0.9/neurosym.egg-info/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      619 2023-11-06 16:32:28.000000 neurosym-0.0.9/neurosym.egg-info/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2724 2023-11-06 16:32:28.000000 neurosym-0.0.9/neurosym.egg-info/SOURCES.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-11-06 16:32:28.000000 neurosym-0.0.9/neurosym.egg-info/dependency_links.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      127 2023-11-06 16:32:28.000000 neurosym-0.0.9/neurosym.egg-info/requires.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       15 2023-11-06 16:32:28.000000 neurosym-0.0.9/neurosym.egg-info/top_level.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-11-06 16:32:28.273190 neurosym-0.0.9/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      911 2023-11-06 16:32:26.000000 neurosym-0.0.9/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/tests/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-30 23:29:31.000000 neurosym-0.0.9/tests/__init__.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/tests/basic_search/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.9/tests/basic_search/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2618 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/basic_search/search_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.269190 neurosym-0.0.9/tests/dreamcoder/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.9/tests/dreamcoder/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3286 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/dreamcoder/compression_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1317 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/dreamcoder/list_dsl_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.273190 neurosym-0.0.9/tests/dsl/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.9/tests/dsl/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      504 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/dsl/rules_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.273190 neurosym-0.0.9/tests/lambdas/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-09-28 01:53:12.000000 neurosym-0.0.9/tests/lambdas/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3544 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/lambdas/enumeration_regression_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     8908 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/lambdas/lambdas_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.273190 neurosym-0.0.9/tests/near/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.9/tests/near/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1205 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/near/test_modules.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     4612 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/near/test_sequential_dsl.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3361 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/near/test_simple_dsl.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      714 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/near/utils.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1070 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/only_direct_import_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.273190 neurosym-0.0.9/tests/templates/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-10-31 03:56:51.000000 neurosym-0.0.9/tests/templates/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)    15777 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/templates/expansion_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1977 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/templates/semantics_test.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-11-06 16:32:28.273190 neurosym-0.0.9/tests/type/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-09-28 01:53:12.000000 neurosym-0.0.9/tests/type/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     7005 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/type/render_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3680 2023-10-31 04:24:49.000000 neurosym-0.0.9/tests/type/unify_test.py
```

### Comparing `neurosym-0.0.8/PKG-INFO` & `neurosym-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosym
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neurosymbolic library.
 Home-page: https://github.com/kavigupta/neurosym-lib
 Author: Kavi Gupta
 Author-email: kavig+neurosym@mit.edu
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `neurosym-0.0.8/neurosym/__init__.py` & `neurosym-0.0.9/neurosym/__init__.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/compression/process_abstraction.py` & `neurosym-0.0.9/neurosym/compression/process_abstraction.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/datasets/load_data.py` & `neurosym-0.0.9/neurosym/datasets/load_data.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/dsl/abstraction.py` & `neurosym-0.0.9/neurosym/dsl/abstraction.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/dsl/dsl.py` & `neurosym-0.0.9/neurosym/dsl/dsl.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/dsl/dsl_factory.py` & `neurosym-0.0.9/neurosym/dsl/dsl_factory.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/dsl/lambdas.py` & `neurosym-0.0.9/neurosym/dsl/lambdas.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/dsl/pcfg.py` & `neurosym-0.0.9/neurosym/dsl/pcfg.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/dsl/production.py` & `neurosym-0.0.9/neurosym/dsl/production.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/dreamcoder/list_example.py` & `neurosym-0.0.9/neurosym/examples/dreamcoder/list_example.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/mutable_arith_combinators.py` & `neurosym-0.0.9/neurosym/examples/mutable_arith_combinators.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/near/dsls/sequential_differentiable_dsl.py` & `neurosym-0.0.9/neurosym/examples/near/dsls/sequential_differentiable_dsl.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/near/dsls/simple_differentiable_dsl.py` & `neurosym-0.0.9/neurosym/examples/near/dsls/simple_differentiable_dsl.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/near/methods/base_trainer.py` & `neurosym-0.0.9/neurosym/examples/near/methods/base_trainer.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/near/methods/near_example_trainer.py` & `neurosym-0.0.9/neurosym/examples/near/methods/near_example_trainer.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/near/neural_dsl.py` & `neurosym-0.0.9/neurosym/examples/near/neural_dsl.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/near/operations/lists.py` & `neurosym-0.0.9/neurosym/examples/near/operations/lists.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/examples/near/search_graph.py` & `neurosym-0.0.9/neurosym/examples/near/search_graph.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/programs/hole.py` & `neurosym-0.0.9/neurosym/programs/hole.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/programs/s_expression.py` & `neurosym-0.0.9/neurosym/programs/s_expression.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/programs/s_expression_render.py` & `neurosym-0.0.9/neurosym/programs/s_expression_render.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/search/astar_search.py` & `neurosym-0.0.9/neurosym/search/astar_search.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/search/bfs_search.py` & `neurosym-0.0.9/neurosym/search/bfs_search.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/search/bounded_astar.py` & `neurosym-0.0.9/neurosym/search/bounded_astar.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/search_graph/dsl_search_graph.py` & `neurosym-0.0.9/neurosym/search_graph/dsl_search_graph.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/search_graph/hole_set_chooser.py` & `neurosym-0.0.9/neurosym/search_graph/hole_set_chooser.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/search_graph/metadata_computer.py` & `neurosym-0.0.9/neurosym/search_graph/metadata_computer.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/search_graph/search_graph_transformer.py` & `neurosym-0.0.9/neurosym/search_graph/search_graph_transformer.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/types/type.py` & `neurosym-0.0.9/neurosym/types/type.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/types/type_signature.py` & `neurosym-0.0.9/neurosym/types/type_signature.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/types/type_string_repr.py` & `neurosym-0.0.9/neurosym/types/type_string_repr.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/types/type_with_environment.py` & `neurosym-0.0.9/neurosym/types/type_with_environment.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym/utils/tree_trie.py` & `neurosym-0.0.9/neurosym/utils/tree_trie.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/neurosym.egg-info/PKG-INFO` & `neurosym-0.0.9/neurosym.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosym
-Version: 0.0.8
+Version: 0.0.9
 Summary: Neurosymbolic library.
 Home-page: https://github.com/kavigupta/neurosym-lib
 Author: Kavi Gupta
 Author-email: kavig+neurosym@mit.edu
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

### Comparing `neurosym-0.0.8/neurosym.egg-info/SOURCES.txt` & `neurosym-0.0.9/neurosym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/setup.py` & `neurosym-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="neurosym",
-    version="0.0.8",
+    version="0.0.9",
     author="Kavi Gupta",
     author_email="kavig+neurosym@mit.edu",
     description="Neurosymbolic library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/neurosym-lib",
     packages=setuptools.find_packages(),
```

### Comparing `neurosym-0.0.8/tests/basic_search/search_test.py` & `neurosym-0.0.9/tests/basic_search/search_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/dreamcoder/compression_test.py` & `neurosym-0.0.9/tests/dreamcoder/compression_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/dreamcoder/list_dsl_test.py` & `neurosym-0.0.9/tests/dreamcoder/list_dsl_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/lambdas/enumeration_regression_test.py` & `neurosym-0.0.9/tests/lambdas/enumeration_regression_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/lambdas/lambdas_test.py` & `neurosym-0.0.9/tests/lambdas/lambdas_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/near/test_modules.py` & `neurosym-0.0.9/tests/near/test_modules.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/near/test_sequential_dsl.py` & `neurosym-0.0.9/tests/near/test_sequential_dsl.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/near/test_simple_dsl.py` & `neurosym-0.0.9/tests/near/test_simple_dsl.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/near/utils.py` & `neurosym-0.0.9/tests/near/utils.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/only_direct_import_test.py` & `neurosym-0.0.9/tests/only_direct_import_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/templates/expansion_test.py` & `neurosym-0.0.9/tests/templates/expansion_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/templates/semantics_test.py` & `neurosym-0.0.9/tests/templates/semantics_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/type/render_test.py` & `neurosym-0.0.9/tests/type/render_test.py`

 * *Files identical despite different names*

### Comparing `neurosym-0.0.8/tests/type/unify_test.py` & `neurosym-0.0.9/tests/type/unify_test.py`

 * *Files identical despite different names*

