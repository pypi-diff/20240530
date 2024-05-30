# Comparing `tmp/pydflow-1.8.8.tar.gz` & `tmp/pydflow-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydflow-1.8.8.tar", last modified: Sat Oct  7 02:36:01 2023, max compression
+gzip compressed data, was "pydflow-1.8.9.tar", last modified: Sat Oct  7 03:29:25 2023, max compression
```

## Comparing `pydflow-1.8.8.tar` & `pydflow-1.8.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.138496 pydflow-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2023-10-07 02:35:46.000000 pydflow-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-07 02:35:46.000000 pydflow-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    32716 2023-10-07 02:36:01.138496 pydflow-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31968 2023-10-07 02:35:46.000000 pydflow-1.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-07 02:35:46.000000 pydflow-1.8.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-07 02:36:01.138496 pydflow-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-10-07 02:35:46.000000 pydflow-1.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.114496 pydflow-1.8.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.122496 pydflow-1.8.8/src/dflow/
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/argo_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.126496 pydflow-1.8.8/src/dflow/client/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/client/v1alpha1_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/client/v1alpha1_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/client/v1alpha1_retry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5861 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/client/v1alpha1_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/client/v1alpha1_value_from.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/code_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/context_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14881 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    58155 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    28566 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/op_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.130497 pydflow-1.8.8/src/dflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17727 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/bohrium.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    25505 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/launching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/lebesgue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/oss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/plugins/ray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.130497 pydflow-1.8.8/src/dflow/python/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16708 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/python/op.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/python/opio.py
--rw-r--r--   0 runner    (1001) docker     (127)    36789 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/python/python_op_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11585 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/python/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16413 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)   108608 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/step.py
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/util_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    28485 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55184 2023-10-07 02:35:46.000000 pydflow-1.8.8/src/dflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.134497 pydflow-1.8.8/src/pydflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32716 2023-10-07 02:36:01.000000 pydflow-1.8.8/src/pydflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-10-07 02:36:01.000000 pydflow-1.8.8/src/pydflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 02:36:01.000000 pydflow-1.8.8/src/pydflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-07 02:36:01.000000 pydflow-1.8.8/src/pydflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-07 02:36:01.000000 pydflow-1.8.8/src/pydflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-07 02:36:01.000000 pydflow-1.8.8/src/pydflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 02:36:01.138496 pydflow-1.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_big_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_conditional_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_makevasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_recurse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_reuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-07 02:35:46.000000 pydflow-1.8.8/tests/test_subpath_slices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.336229 pydflow-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2023-10-07 03:29:12.000000 pydflow-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-07 03:29:12.000000 pydflow-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32716 2023-10-07 03:29:25.336229 pydflow-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31968 2023-10-07 03:29:12.000000 pydflow-1.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-07 03:29:12.000000 pydflow-1.8.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-07 03:29:25.336229 pydflow-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-10-07 03:29:12.000000 pydflow-1.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.324229 pydflow-1.8.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.328229 pydflow-1.8.9/src/dflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/argo_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.332229 pydflow-1.8.9/src/dflow/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/client/v1alpha1_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/client/v1alpha1_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/client/v1alpha1_retry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5861 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/client/v1alpha1_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/client/v1alpha1_value_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/code_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/context_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14881 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58155 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28566 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/op_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.332229 pydflow-1.8.9/src/dflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17727 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/bohrium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25505 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/launching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/lebesgue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/oss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/plugins/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.332229 pydflow-1.8.9/src/dflow/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16708 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/python/op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/python/opio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36789 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/python/python_op_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11585 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/python/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16413 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108608 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/util_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28485 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55184 2023-10-07 03:29:12.000000 pydflow-1.8.9/src/dflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.336229 pydflow-1.8.9/src/pydflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32716 2023-10-07 03:29:25.000000 pydflow-1.8.9/src/pydflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2023-10-07 03:29:25.000000 pydflow-1.8.9/src/pydflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-07 03:29:25.000000 pydflow-1.8.9/src/pydflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-07 03:29:25.000000 pydflow-1.8.9/src/pydflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-07 03:29:25.000000 pydflow-1.8.9/src/pydflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-07 03:29:25.000000 pydflow-1.8.9/src/pydflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-07 03:29:25.336229 pydflow-1.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_big_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_conditional_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8450 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_makevasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_recurse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-07 03:29:12.000000 pydflow-1.8.9/tests/test_subpath_slices.py
```

### Comparing `pydflow-1.8.8/LICENSE` & `pydflow-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/PKG-INFO` & `pydflow-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.8.8
+Version: 1.8.9
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.8.8/README.md` & `pydflow-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/setup.py` & `pydflow-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/__init__.py` & `pydflow-1.8.9/src/dflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/argo_objects.py` & `pydflow-1.8.9/src/dflow/argo_objects.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/client/v1alpha1_artifact.py` & `pydflow-1.8.9/src/dflow/client/v1alpha1_artifact.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/client/v1alpha1_parameter.py` & `pydflow-1.8.9/src/dflow/client/v1alpha1_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/client/v1alpha1_retry_strategy.py` & `pydflow-1.8.9/src/dflow/client/v1alpha1_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/client/v1alpha1_sequence.py` & `pydflow-1.8.9/src/dflow/client/v1alpha1_sequence.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/client/v1alpha1_value_from.py` & `pydflow-1.8.9/src/dflow/client/v1alpha1_value_from.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/code_gen.py` & `pydflow-1.8.9/src/dflow/code_gen.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/common.py` & `pydflow-1.8.9/src/dflow/common.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/config.py` & `pydflow-1.8.9/src/dflow/config.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/context_syntax.py` & `pydflow-1.8.9/src/dflow/context_syntax.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/dag.py` & `pydflow-1.8.9/src/dflow/dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/executor.py` & `pydflow-1.8.9/src/dflow/executor.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/io.py` & `pydflow-1.8.9/src/dflow/io.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/main.py` & `pydflow-1.8.9/src/dflow/main.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/op_template.py` & `pydflow-1.8.9/src/dflow/op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/bohrium.py` & `pydflow-1.8.9/src/dflow/plugins/bohrium.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/datasets.py` & `pydflow-1.8.9/src/dflow/plugins/datasets.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/dispatcher.py` & `pydflow-1.8.9/src/dflow/plugins/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/launching.py` & `pydflow-1.8.9/src/dflow/plugins/launching.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/lebesgue.py` & `pydflow-1.8.9/src/dflow/plugins/lebesgue.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/metadata.py` & `pydflow-1.8.9/src/dflow/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/oss.py` & `pydflow-1.8.9/src/dflow/plugins/oss.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/plugins/ray.py` & `pydflow-1.8.9/src/dflow/plugins/ray.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/python/op.py` & `pydflow-1.8.9/src/dflow/python/op.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/python/opio.py` & `pydflow-1.8.9/src/dflow/python/opio.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/python/python_op_template.py` & `pydflow-1.8.9/src/dflow/python/python_op_template.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/python/utils.py` & `pydflow-1.8.9/src/dflow/python/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/resource.py` & `pydflow-1.8.9/src/dflow/resource.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/slurm.py` & `pydflow-1.8.9/src/dflow/slurm.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/step.py` & `pydflow-1.8.9/src/dflow/step.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/steps.py` & `pydflow-1.8.9/src/dflow/steps.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/task.py` & `pydflow-1.8.9/src/dflow/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         if dependencies is None:
             dependencies = []
         self.dependencies = dependencies
         super().__init__(name=name, template=template, **kwargs)
         if self.prepare_step is not None:
             self.dependencies.append(self.prepare_step)
         if self.check_step is not None:
-            self.check_step.dependencies.append(self)
+            self.check_step.dependencies = [
+                "%s.Succeeded || %s.Failed || %s.Errored" % (self, self, self)]
 
     @classmethod
     def from_dict(cls, d, templates):
         task = super().from_dict(d, templates)
         task.dependencies = d.get("dependencies", [])
         if d.get("depends"):
             for dep in d["depends"].split("&&"):
```

### Comparing `pydflow-1.8.8/src/dflow/util_ops.py` & `pydflow-1.8.9/src/dflow/util_ops.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/utils.py` & `pydflow-1.8.9/src/dflow/utils.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/dflow/workflow.py` & `pydflow-1.8.9/src/dflow/workflow.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/src/pydflow.egg-info/PKG-INFO` & `pydflow-1.8.9/src/pydflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydflow
-Version: 1.8.8
+Version: 1.8.9
 Summary: Dflow is a Python framework for constructing scientific computing workflows employing Argo Workflows as the workflow engine.
 Home-page: https://github.com/deepmodeling/dflow
 Author: Xinzijian Liu
 Author-email: liuxzj@dp.tech
 License: LGPLv3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pydflow-1.8.8/src/pydflow.egg-info/SOURCES.txt` & `pydflow-1.8.9/src/pydflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_big_parameter.py` & `pydflow-1.8.9/tests/test_big_parameter.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_conditional_outputs.py` & `pydflow-1.8.9/tests/test_conditional_outputs.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_dag.py` & `pydflow-1.8.9/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_group_size.py` & `pydflow-1.8.9/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_makevasp.py` & `pydflow-1.8.9/tests/test_makevasp.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_python.py` & `pydflow-1.8.9/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_recurse.py` & `pydflow-1.8.9/tests/test_recurse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_reuse.py` & `pydflow-1.8.9/tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_slices.py` & `pydflow-1.8.9/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `pydflow-1.8.8/tests/test_subpath_slices.py` & `pydflow-1.8.9/tests/test_subpath_slices.py`

 * *Files identical despite different names*

