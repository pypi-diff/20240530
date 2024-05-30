# Comparing `tmp/spine_engine-0.24.0.tar.gz` & `tmp/spine_engine-0.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_engine-0.24.0.tar", last modified: Tue Apr 30 07:29:17 2024, max compression
+gzip compressed data, was "spine_engine-0.24.1.tar", last modified: Thu May 30 13:45:39 2024, max compression
```

## Comparing `spine_engine-0.24.0.tar` & `spine_engine-0.24.1.tar`

### file list

```diff
@@ -1,217 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.github/workflows/run_unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-30 07:29:06.000000 spine_engine-0.24.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 07:29:06.000000 spine_engine-0.24.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-30 07:29:06.000000 spine_engine-0.24.0/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-30 07:29:17.105780 spine_engine-0.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-30 07:29:06.000000 spine_engine-0.24.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-30 07:29:06.000000 spine_engine-0.24.0/bin/build_doc.bat
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 07:29:06.000000 spine_engine-0.24.0/bin/build_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 07:29:06.000000 spine_engine-0.24.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/config/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_runner/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/conda_kernel_spec_runner/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/execution_manager_base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/kernel_execution_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/persistent_execution_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/process_execution_manager/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/spine_repl/
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/execution_managers/spine_repl/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/load_project_items/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/load_project_items/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/executor/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/executor/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/multithread/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/multithread/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/multithread_executor/thread_executor/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/connection/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/executable_item_base/
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/executable_item_base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.081780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_info/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_info/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_resource/
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_resource/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item/project_item_specification_factory/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item_loader/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/project_item_loader/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine/
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine_server/
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/spine_engine_server/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/command_line_arguments/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/command_line_arguments/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/helpers/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/queue_logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/queue_logger/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/returning_process/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/returning_process/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/utils/serialization/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/docs/source/autoapi/spine_engine/version/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/autoapi/spine_engine/version/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-30 07:29:06.000000 spine_engine-0.24.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.085780 spine_engine-0.24.0/fig/
--rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-04-30 07:29:06.000000 spine_engine-0.24.0/fig/eu-emblem-low-res.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-30 07:29:06.000000 spine_engine-0.24.0/fig/spineengine_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-30 07:29:06.000000 spine_engine-0.24.0/fig/spineengine_on_wht.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-04-30 07:29:06.000000 spine_engine-0.24.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-30 07:29:06.000000 spine_engine-0.24.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:29:17.105780 spine_engine-0.24.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.089780 spine_engine-0.24.0/spine_engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.089780 spine_engine-0.24.0/spine_engine/execution_managers/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/execution_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/kernel_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    30262 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/persistent_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/process_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.jl
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16252 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/jumpster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/load_project_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.093780 spine_engine-0.24.0/spine_engine/project_item/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28819 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/executable_item_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_specification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item/project_item_specification_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/project_item_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.093780 spine_engine-0.24.0/spine_engine/server/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/certificate_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19731 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/engine_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/persistent_execution_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/ping_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/project_extractor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/project_remover_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/project_retriever_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/remote_execution_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/service_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/start_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.093780 spine_engine-0.24.0/spine_engine/server/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/event_data_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/server_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/server/util/zip_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    36567 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/spine_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/spine_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/command_line_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/execution_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/queue_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/returning_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-30 07:29:06.000000 spine_engine-0.24.0/spine_engine/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 07:29:16.000000 spine_engine-0.24.0/spine_engine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/spine_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:29:16.000000 spine_engine-0.24.0/spine_engine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 07:29:17.000000 spine_engine-0.24.0/spine_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/execution_managers/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/test_kernel_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/test_persistent_execution_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/execution_managers/test_process_execution_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.073780 spine_engine-0.24.0/tests/mock_project_items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/mock_project_items/items_module/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.097780 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/executable_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/mock_project_items/items_module/test_item/specification_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/project_item/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/test_ExecutableItem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/project_item/test_project_item_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/allowEndpoints.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/certificates/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/private_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/private_keys/client.key_secret
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/private_keys/server.key_secret
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/secfolder_for_tests/public_keys/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/public_keys/client.key
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/secfolder_for_tests/public_keys/server.key
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_EngineServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_PingService.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_ProjectExtractorService.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_ProjectRemoverService.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/test_start_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.101780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/local/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/local/project_local_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/local/specification_local_data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.077780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld2.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/projectforpackagingtests/input2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/test_EventDataConverter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/test_ServerMessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/util/test_ZipHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/server/zippedproject.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/test_load_project_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    52129 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/test_spine_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:29:17.105780 spine_engine-0.24.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/test_command_line_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-30 07:29:06.000000 spine_engine-0.24.0/tests/utils/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.282861 spine_engine-0.24.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 13:45:32.000000 spine_engine-0.24.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.262861 spine_engine-0.24.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 13:45:32.000000 spine_engine-0.24.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.262861 spine_engine-0.24.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-30 13:45:32.000000 spine_engine-0.24.1/.github/workflows/run_unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-30 13:45:32.000000 spine_engine-0.24.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 13:45:32.000000 spine_engine-0.24.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-30 13:45:32.000000 spine_engine-0.24.1/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-30 13:45:39.282861 spine_engine-0.24.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-30 13:45:32.000000 spine_engine-0.24.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.262861 spine_engine-0.24.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 13:45:32.000000 spine_engine-0.24.1/bin/build_doc.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 13:45:32.000000 spine_engine-0.24.1/bin/build_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 13:45:32.000000 spine_engine-0.24.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.266861 spine_engine-0.24.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-30 13:45:32.000000 spine_engine-0.24.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-30 13:45:32.000000 spine_engine-0.24.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.266861 spine_engine-0.24.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-30 13:45:32.000000 spine_engine-0.24.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 13:45:32.000000 spine_engine-0.24.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.266861 spine_engine-0.24.1/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)    55634 2024-05-30 13:45:32.000000 spine_engine-0.24.1/fig/eu-emblem-low-res.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-30 13:45:32.000000 spine_engine-0.24.1/fig/spineengine_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-30 13:45:32.000000 spine_engine-0.24.1/fig/spineengine_on_wht.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-30 13:45:32.000000 spine_engine-0.24.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-30 13:45:32.000000 spine_engine-0.24.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-30 13:45:32.000000 spine_engine-0.24.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:45:39.282861 spine_engine-0.24.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.266861 spine_engine-0.24.1/spine_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.270861 spine_engine-0.24.1/spine_engine/execution_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/conda_kernel_spec_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/conda_kernel_spec_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/execution_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/kernel_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30262 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/persistent_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/process_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/spine_repl.jl
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/execution_managers/spine_repl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16250 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/jumpster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/load_project_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.270861 spine_engine-0.24.1/spine_engine/project_item/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28819 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9065 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item/executable_item_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item/project_item_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item/project_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item/project_item_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item/project_item_specification_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/project_item_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.274861 spine_engine-0.24.1/spine_engine/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/certificate_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19714 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/engine_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/persistent_execution_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/ping_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/project_extractor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/project_remover_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/project_retriever_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/remote_execution_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/service_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/start_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.274861 spine_engine-0.24.1/spine_engine/server/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/util/event_data_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/util/server_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/server/util/zip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36615 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/spine_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.274861 spine_engine-0.24.1/spine_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/utils/command_line_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/utils/execution_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17102 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/utils/queue_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/utils/returning_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-30 13:45:32.000000 spine_engine-0.24.1/spine_engine/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 13:45:39.000000 spine_engine-0.24.1/spine_engine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.282861 spine_engine-0.24.1/spine_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-30 13:45:39.000000 spine_engine-0.24.1/spine_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-30 13:45:39.000000 spine_engine-0.24.1/spine_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:45:39.000000 spine_engine-0.24.1/spine_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:45:38.000000 spine_engine-0.24.1/spine_engine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-30 13:45:39.000000 spine_engine-0.24.1/spine_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 13:45:39.000000 spine_engine-0.24.1/spine_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.274861 spine_engine-0.24.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.274861 spine_engine-0.24.1/tests/execution_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/execution_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/execution_managers/test_kernel_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/execution_managers/test_persistent_execution_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/execution_managers/test_process_execution_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.262861 spine_engine-0.24.1/tests/mock_project_items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.274861 spine_engine-0.24.1/tests/mock_project_items/items_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/mock_project_items/items_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.274861 spine_engine-0.24.1/tests/mock_project_items/items_module/test_item/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/mock_project_items/items_module/test_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/mock_project_items/items_module/test_item/executable_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/mock_project_items/items_module/test_item/specification_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/project_item/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/project_item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/project_item/test_ExecutableItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/project_item/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/project_item/test_project_item_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/secfolder_for_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/secfolder_for_tests/allowEndpoints.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/secfolder_for_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/secfolder_for_tests/certificates/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/secfolder_for_tests/private_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/secfolder_for_tests/private_keys/client.key_secret
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/secfolder_for_tests/private_keys/server.key_secret
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/secfolder_for_tests/public_keys/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/secfolder_for_tests/public_keys/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/secfolder_for_tests/public_keys/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/test_EngineServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/test_PingService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/test_ProjectExtractorService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/test_ProjectRemoverService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/test_start_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.278861 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.282861 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/local/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/local/project_local_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/local/specification_local_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.262861 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.282861 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/specifications/Tool/helloworld2.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/projectforpackagingtests/input2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/test_EventDataConverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/test_ServerMessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/util/test_ZipHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/server/zippedproject.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/test_load_project_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52129 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/test_spine_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:45:39.282861 spine_engine-0.24.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/utils/test_command_line_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/utils/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-05-30 13:45:32.000000 spine_engine-0.24.1/tests/utils/test_serialization.py
```

### Comparing `spine_engine-0.24.0/.github/workflows/run_unit_tests.yml` & `spine_engine-0.24.1/.github/workflows/run_unit_tests.yml`

 * *Files 15% similar despite different names*

```diff
@@ -9,39 +9,44 @@
 jobs:
   unit-tests:
     name: Unit tests
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [windows-latest, ubuntu-22.04]
-        python-version: [3.8, 3.9, "3.10", 3.11]
+        python-version: [3.8, 3.9, "3.10", 3.11, 3.12]
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Version from Git tags
       run: git describe --tags
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+        cache: pip
+        cache-dependency-path: |
+          pyproject.toml
+          requirements.txt
+          dev-requirements.txt
     - name: Display Python version
       run:
          python -c "import sys; print(sys.version)"
     - name: Install additional packages for Linux
       if: runner.os == 'Linux'
       run: |
         sudo apt-get install -y unixodbc-dev
     - name: Install dependencies
       env:
         PYTHONUTF8: 1
       run: |
         python -m pip install --upgrade pip
-        pip install git+https://github.com/spine-tools/Spine-Database-API.git#egg=spinedb_api
-        pip install .[dev]
+        pip install -r requirements.txt
+        pip install -r dev-requirements.txt
     - name: List packages
       run:
         pip list
     - name: Install python3 kernelspecs
       run: |
         pip install ipykernel
         python -m ipykernel install --user
```

### Comparing `spine_engine-0.24.0/COPYING` & `spine_engine-0.24.1/COPYING`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/COPYING.LESSER` & `spine_engine-0.24.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/PKG-INFO` & `spine_engine-0.24.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 Metadata-Version: 2.1
 Name: spine_engine
-Version: 0.24.0
+Version: 0.24.1
 Summary: A package to run Spine workflows.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/spine-engine
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.8.1
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: pendulum<3.0.0
-Requires-Dist: protobuf<3.21.0
 Requires-Dist: networkx>2.5.1
 Requires-Dist: datapackage<1.16,>=1.15.2
 Requires-Dist: jupyter_client>=6.0
-Requires-Dist: spinedb_api>=0.31.0
+Requires-Dist: spinedb_api>=0.31.2
 Requires-Dist: pyzmq>=21.0
-Requires-Dist: markupsafe<2.1
-Provides-Extra: dev
-Requires-Dist: coverage[toml]; extra == "dev"
 
 # Spine Engine
 
-[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
+[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Unit tests](https://github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests")
 [![codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/spine-engine)
 [![PyPI version](https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-engine)
 
 A Python package to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox) workflows.
 
 <p align="center" width="100%">
@@ -49,19 +44,14 @@
 
 ### Installation
 
 To install Spine Engine into an existing Python environment, run
 
     $ pip install spine_engine
 
-### Dependencies
-
-Spine Engine installation will install [dagster](https://dagster.readthedocs.io/en/master/index.html).
-
-&nbsp;
 <hr>
 <center>
 <table width=500px frame="none">
 <tr>
 <td valign="middle" width=100px>
 <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
 <td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
```

#### html2text {}

```diff
@@ -1,38 +1,34 @@
-Metadata-Version: 2.1 Name: spine_engine Version: 0.24.0 Summary: A package to
+Metadata-Version: 2.1 Name: spine_engine Version: 0.24.1 Summary: A package to
 run Spine workflows. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/spine-engine Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
-Python: <3.12,>=3.8.1 Description-Content-Type: text/markdown License-File:
-COPYING License-File: COPYING.LESSER Requires-Dist: pendulum<3.0.0 Requires-
-Dist: protobuf<3.21.0 Requires-Dist: networkx>2.5.1 Requires-Dist:
+Python: >=3.8.1 Description-Content-Type: text/markdown License-File: COPYING
+License-File: COPYING.LESSER Requires-Dist: networkx>2.5.1 Requires-Dist:
 datapackage<1.16,>=1.15.2 Requires-Dist: jupyter_client>=6.0 Requires-Dist:
-spinedb_api>=0.31.0 Requires-Dist: pyzmq>=21.0 Requires-Dist: markupsafe<2.1
-Provides-Extra: dev Requires-Dist: coverage[toml]; extra == "dev" # Spine
-Engine [![Python](https://img.shields.io/badge/python-
-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/
-downloads/release/python-379/) [![Unit tests](https://github.com/spine-tools/
-spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/
-spine-engine/actions?query=workflow%3A"Unit+tests") [![codecov](https://
-codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://
-codecov.io/gh/spine-tools/spine-engine) [![PyPI version](https://badge.fury.io/
-py/spine-engine.svg)](https://badge.fury.io/py/spine-engine) A Python package
-to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
+spinedb_api>=0.31.2 Requires-Dist: pyzmq>=21.0 # Spine Engine [![Python](https:
+//img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-
+blue.svg)](https://www.python.org/downloads/release/python-379/) [![Unit tests]
+(https://github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)]
+(https://github.com/spine-tools/spine-engine/
+actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
+tools/spine-engine/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-
+tools/spine-engine) [![PyPI version](https://badge.fury.io/py/spine-
+engine.svg)](https://badge.fury.io/py/spine-engine) A Python package to
+coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
 Spine-Toolbox) workflows.
                                 [Spine Engine]
 ## License Spine Engine is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
 the [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/
 by-sa/4.0/). ## Getting started ### Installation To install Spine Engine into
-an existing Python environment, run $ pip install spine_engine ### Dependencies
-Spine Engine installation will install [dagster](https://
-dagster.readthedocs.io/en/master/index.html).  
+an existing Python environment, run $ pip install spine_engine
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spine_engine-0.24.0/README.md` & `spine_engine-0.24.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Spine Engine
 
-[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
+[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Unit tests](https://github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests")
 [![codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/spine-engine)
 [![PyPI version](https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-engine)
 
 A Python package to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox) workflows.
 
 <p align="center" width="100%">
@@ -23,19 +23,14 @@
 
 ### Installation
 
 To install Spine Engine into an existing Python environment, run
 
     $ pip install spine_engine
 
-### Dependencies
-
-Spine Engine installation will install [dagster](https://dagster.readthedocs.io/en/master/index.html).
-
-&nbsp;
 <hr>
 <center>
 <table width=500px frame="none">
 <tr>
 <td valign="middle" width=100px>
 <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
 <td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
```

#### html2text {}

```diff
@@ -1,25 +1,23 @@
 # Spine Engine [![Python](https://img.shields.io/badge/python-
-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/
+3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](https://www.python.org/
 downloads/release/python-379/) [![Unit tests](https://github.com/spine-tools/
 spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/
 spine-engine/actions?query=workflow%3A"Unit+tests") [![codecov](https://
 codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://
 codecov.io/gh/spine-tools/spine-engine) [![PyPI version](https://badge.fury.io/
 py/spine-engine.svg)](https://badge.fury.io/py/spine-engine) A Python package
 to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
 Spine-Toolbox) workflows.
                                 [Spine Engine]
 ## License Spine Engine is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
 the [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/
 by-sa/4.0/). ## Getting started ### Installation To install Spine Engine into
-an existing Python environment, run $ pip install spine_engine ### Dependencies
-Spine Engine installation will install [dagster](https://
-dagster.readthedocs.io/en/master/index.html).  
+an existing Python environment, run $ pip install spine_engine
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spine_engine-0.24.0/docs/Makefile` & `spine_engine-0.24.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/docs/make.bat` & `spine_engine-0.24.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/docs/source/conf.py` & `spine_engine-0.24.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `spine_engine-0.24.0/fig/eu-emblem-low-res.jpg` & `spine_engine-0.24.1/fig/eu-emblem-low-res.jpg`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/fig/spineengine_logo.svg` & `spine_engine-0.24.1/fig/spineengine_logo.svg`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/fig/spineengine_on_wht.svg` & `spine_engine-0.24.1/fig/spineengine_on_wht.svg`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/pylintrc` & `spine_engine-0.24.1/pylintrc`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/pyproject.toml` & `spine_engine-0.24.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,40 +3,30 @@
 dynamic = ["version"]
 authors = [{name = "Spine Project consortium", email = "spine_info@vtt.fi"}]
 license = {text = "LGPL-3.0-or-later"}
 description = "A package to run Spine workflows."
 keywords = ["energy system modelling", "workflow", "optimisation", "database"]
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
-	    "Programming Language :: Python :: 3",
-	    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
-	    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+    "Operating System :: OS Independent",
 ]
-requires-python = ">=3.8.1, <3.12"
+requires-python = ">=3.8.1"
 dependencies = [
-    # dagster versions lower that 1.5.7 do not support pendulum >= 3.0.0
-    "pendulum < 3.0.0",
-    # https://developers.google.com/protocol-buffers/docs/news/2022-05-06#python-updates
-    "protobuf<3.21.0",
     "networkx>2.5.1",
     "datapackage>=1.15.2, <1.16",
     "jupyter_client>=6.0",
-    "spinedb_api>=0.31.0",
+    "spinedb_api>=0.31.2",
     "pyzmq >=21.0",
-    # dagster 0.12.8 requires Jinja2<3.0, which tries to import
-    # soft_unicode, which has been removed in markupsafe 2.1
-    "markupsafe < 2.1",
 ]
 
 [project.urls]
 Repository = "https://github.com/spine-tools/spine-engine"
 
-[project.optional-dependencies]
-dev = ["coverage[toml]"]
-
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=6.2", "wheel", "build"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "spine_engine/version.py"
 version_scheme = "release-branch-semver"
@@ -45,25 +35,25 @@
 zip-safe = false
 
 [tool.setuptools.package-data]
 spine_engine = ["execution_managers/spine_repl.jl"]
 
 [tool.setuptools.packages.find]
 exclude = [
-	"bin*",
-	"docs*",
-	"fig*",
-	"tests*",
+    "bin*",
+    "docs*",
+    "fig*",
+    "tests*",
 ]
 
 [tool.coverage.run]
 source = ["spine_engine"]
 branch = true
 concurrency = ["multiprocessing", "thread"]
 disable_warnings = ["no-data-collected"]
 
 [tool.coverage.report]
 ignore_errors = true
 
 [tool.black]
 line-length = 120
-exclude = '\.git'
+exclude = '\.git|version.py'
```

### Comparing `spine_engine-0.24.0/spine_engine/__init__.py` & `spine_engine-0.24.1/spine_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/config.py` & `spine_engine-0.24.1/spine_engine/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 # GAMS
 GAMS_EXECUTABLE = _executable("gams")
 
 # Julia
 JULIA_EXECUTABLE = _executable("julia")
 
+
 # Python
 def is_frozen():
     """Checks if we are currently running as frozen bundle.
 
     Returns:
         bool: True if we are frozen, False otherwise
     """
```

### Comparing `spine_engine-0.24.0/spine_engine/exception.py` & `spine_engine-0.24.1/spine_engine/exception.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/__init__.py` & `spine_engine-0.24.1/spine_engine/execution_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_manager.py` & `spine_engine-0.24.1/spine_engine/execution_managers/conda_kernel_spec_manager.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/conda_kernel_spec_runner.py` & `spine_engine-0.24.1/spine_engine/execution_managers/conda_kernel_spec_runner.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/execution_manager_base.py` & `spine_engine-0.24.1/spine_engine/execution_managers/execution_manager_base.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/kernel_execution_manager.py` & `spine_engine-0.24.1/spine_engine/execution_managers/kernel_execution_manager.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/persistent_execution_manager.py` & `spine_engine-0.24.1/spine_engine/execution_managers/persistent_execution_manager.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/process_execution_manager.py` & `spine_engine-0.24.1/spine_engine/execution_managers/process_execution_manager.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.jl` & `spine_engine-0.24.1/spine_engine/execution_managers/spine_repl.jl`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/execution_managers/spine_repl.py` & `spine_engine-0.24.1/spine_engine/execution_managers/spine_repl.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/jumpster.py` & `spine_engine-0.24.1/spine_engine/jumpster.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     pass
 
 
 class JumpsterEvent(DefinitionBase):
     def __init__(self, event_type, item_name, direction, **kwargs):
         super().__init__(item_name, direction)
         self.event_type = event_type
-        for (key, value) in kwargs.items():
+        for key, value in kwargs.items():
             setattr(self, key, value)
 
 
 class Failure(BaseException):
     """A failure"""
```

### Comparing `spine_engine-0.24.0/spine_engine/load_project_items.py` & `spine_engine-0.24.1/spine_engine/load_project_items.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item/__init__.py` & `spine_engine-0.24.1/spine_engine/project_item/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item/connection.py` & `spine_engine-0.24.1/spine_engine/project_item/connection.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item/executable_item_base.py` & `spine_engine-0.24.1/spine_engine/project_item/executable_item_base.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item/project_item_info.py` & `spine_engine-0.24.1/spine_engine/project_item/project_item_info.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item/project_item_resource.py` & `spine_engine-0.24.1/spine_engine/project_item/project_item_resource.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item/project_item_specification.py` & `spine_engine-0.24.1/spine_engine/project_item/project_item_specification.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item/project_item_specification_factory.py` & `spine_engine-0.24.1/spine_engine/project_item/project_item_specification_factory.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/project_item_loader.py` & `spine_engine-0.24.1/spine_engine/project_item_loader.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/__init__.py` & `spine_engine-0.24.1/spine_engine/server/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/certificate_creator.py` & `spine_engine-0.24.1/spine_engine/server/certificate_creator.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/engine_server.py` & `spine_engine-0.24.1/spine_engine/server/engine_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
         self.persistent_exec_mngrs = dict()
         self.start()  # Start serving
 
     def close(self):
         """Closes the server by sending a KILL message to this thread using a PAIR socket."""
         if self.auth is not None:
             self.auth.stop()
-            time.sleep(0.2)  # wait a bit until authenticator has been closed
+            while self.auth.is_alive():
+                pass
         self.ctrl_msg_sender.send(b"KILL")
         self.join()  # Wait for the thread to finish and sockets to close
         self.ctrl_msg_sender.close()  # Close this in the same thread that it was created in
         self._context.term()
 
     def serve(self):
         """Creates the required sockets, which are polled asynchronously. The ROUTER socket handles communicating
```

### Comparing `spine_engine-0.24.0/spine_engine/server/persistent_execution_service.py` & `spine_engine-0.24.1/spine_engine/server/persistent_execution_service.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/ping_service.py` & `spine_engine-0.24.1/spine_engine/server/ping_service.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/project_extractor_service.py` & `spine_engine-0.24.1/spine_engine/server/project_extractor_service.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/project_remover_service.py` & `spine_engine-0.24.1/spine_engine/server/project_remover_service.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/project_retriever_service.py` & `spine_engine-0.24.1/spine_engine/server/project_retriever_service.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/remote_execution_service.py` & `spine_engine-0.24.1/spine_engine/server/remote_execution_service.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/request.py` & `spine_engine-0.24.1/spine_engine/server/request.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/service_base.py` & `spine_engine-0.24.1/spine_engine/server/service_base.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/start_server.py` & `spine_engine-0.24.1/spine_engine/server/start_server.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/util/__init__.py` & `spine_engine-0.24.1/spine_engine/server/util/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/util/event_data_converter.py` & `spine_engine-0.24.1/spine_engine/server/util/event_data_converter.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/util/server_message.py` & `spine_engine-0.24.1/spine_engine/server/util/server_message.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/server/util/zip_handler.py` & `spine_engine-0.24.1/spine_engine/server/util/zip_handler.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/spine_engine.py` & `spine_engine-0.24.1/spine_engine/spine_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,17 +402,19 @@
                 raise Failure()
             item = self.make_item(item_name, ED.BACKWARD)
             resources = item.output_resources(ED.BACKWARD)
             for r in resources:
                 r.metadata["db_server_manager_queue"] = self._db_server_manager_queue
             yield Output(value=resources)
             yield Finalization(
-                item_finish_state=ItemExecutionFinishState.SUCCESS
-                if self._execution_permits[item_name]
-                else ItemExecutionFinishState.EXCLUDED
+                item_finish_state=(
+                    ItemExecutionFinishState.SUCCESS
+                    if self._execution_permits[item_name]
+                    else ItemExecutionFinishState.EXCLUDED
+                )
             )
 
         return SolidDefinition(item_name=item_name, direction=ED.BACKWARD, input_defs=[], compute_fn=compute_fn)
 
     def _make_forward_solid_def(self, item_name):
         """Returns a SolidDefinition for executing the given item.
```

### Comparing `spine_engine-0.24.0/spine_engine/utils/__init__.py` & `spine_engine-0.24.1/spine_engine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/utils/command_line_arguments.py` & `spine_engine-0.24.1/spine_engine/utils/command_line_arguments.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/utils/execution_resources.py` & `spine_engine-0.24.1/spine_engine/utils/execution_resources.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/utils/helpers.py` & `spine_engine-0.24.1/spine_engine/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/utils/queue_logger.py` & `spine_engine-0.24.1/spine_engine/utils/queue_logger.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/utils/returning_process.py` & `spine_engine-0.24.1/spine_engine/utils/returning_process.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/spine_engine/utils/serialization.py` & `spine_engine-0.24.1/spine_engine/utils/serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,17 @@
     if sys.platform == "win32":
         path = path[1:]  # Remove extra '/' from the beginning
     if os.path.isfile(path):
         is_relative = path_in_dir(path, project_dir)
         serialized = {
             "type": "file_url",
             "relative": is_relative,
-            "path": os.path.relpath(path, project_dir).replace(os.sep, "/")
-            if is_relative
-            else path.replace(os.sep, "/"),
+            "path": (
+                os.path.relpath(path, project_dir).replace(os.sep, "/") if is_relative else path.replace(os.sep, "/")
+            ),
             "scheme": parsed.scheme,
         }
         if parsed.query:
             serialized["query"] = parsed.query
     else:
         serialized = {"type": "url", "relative": False, "path": url}
     return serialized
```

### Comparing `spine_engine-0.24.0/spine_engine.egg-info/PKG-INFO` & `spine_engine-0.24.1/spine_engine.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 Metadata-Version: 2.1
 Name: spine_engine
-Version: 0.24.0
+Version: 0.24.1
 Summary: A package to run Spine workflows.
 Author-email: Spine Project consortium <spine_info@vtt.fi>
 License: LGPL-3.0-or-later
 Project-URL: Repository, https://github.com/spine-tools/spine-engine
 Keywords: energy system modelling,workflow,optimisation,database
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.12,>=3.8.1
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
-Requires-Dist: pendulum<3.0.0
-Requires-Dist: protobuf<3.21.0
 Requires-Dist: networkx>2.5.1
 Requires-Dist: datapackage<1.16,>=1.15.2
 Requires-Dist: jupyter_client>=6.0
-Requires-Dist: spinedb_api>=0.31.0
+Requires-Dist: spinedb_api>=0.31.2
 Requires-Dist: pyzmq>=21.0
-Requires-Dist: markupsafe<2.1
-Provides-Extra: dev
-Requires-Dist: coverage[toml]; extra == "dev"
 
 # Spine Engine
 
-[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
+[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-blue.svg)](https://www.python.org/downloads/release/python-379/)
 [![Unit tests](https://github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests")
 [![codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/spine-engine)
 [![PyPI version](https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-engine)
 
 A Python package to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox) workflows.
 
 <p align="center" width="100%">
@@ -49,19 +44,14 @@
 
 ### Installation
 
 To install Spine Engine into an existing Python environment, run
 
     $ pip install spine_engine
 
-### Dependencies
-
-Spine Engine installation will install [dagster](https://dagster.readthedocs.io/en/master/index.html).
-
-&nbsp;
 <hr>
 <center>
 <table width=500px frame="none">
 <tr>
 <td valign="middle" width=100px>
 <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
 <td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
```

#### html2text {}

```diff
@@ -1,38 +1,34 @@
-Metadata-Version: 2.1 Name: spine_engine Version: 0.24.0 Summary: A package to
+Metadata-Version: 2.1 Name: spine_engine Version: 0.24.1 Summary: A package to
 run Spine workflows. Author-email: Spine Project consortium
 vtt.fi> License: LGPL-3.0-or-later Project-URL: Repository, https://github.com/
 spine-tools/spine-engine Keywords: energy system
 modelling,workflow,optimisation,database Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU Lesser General Public
 License v3 (LGPLv3) Classifier: Operating System :: OS Independent Requires-
-Python: <3.12,>=3.8.1 Description-Content-Type: text/markdown License-File:
-COPYING License-File: COPYING.LESSER Requires-Dist: pendulum<3.0.0 Requires-
-Dist: protobuf<3.21.0 Requires-Dist: networkx>2.5.1 Requires-Dist:
+Python: >=3.8.1 Description-Content-Type: text/markdown License-File: COPYING
+License-File: COPYING.LESSER Requires-Dist: networkx>2.5.1 Requires-Dist:
 datapackage<1.16,>=1.15.2 Requires-Dist: jupyter_client>=6.0 Requires-Dist:
-spinedb_api>=0.31.0 Requires-Dist: pyzmq>=21.0 Requires-Dist: markupsafe<2.1
-Provides-Extra: dev Requires-Dist: coverage[toml]; extra == "dev" # Spine
-Engine [![Python](https://img.shields.io/badge/python-
-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/
-downloads/release/python-379/) [![Unit tests](https://github.com/spine-tools/
-spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/
-spine-engine/actions?query=workflow%3A"Unit+tests") [![codecov](https://
-codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://
-codecov.io/gh/spine-tools/spine-engine) [![PyPI version](https://badge.fury.io/
-py/spine-engine.svg)](https://badge.fury.io/py/spine-engine) A Python package
-to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
+spinedb_api>=0.31.2 Requires-Dist: pyzmq>=21.0 # Spine Engine [![Python](https:
+//img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11|%203.12-
+blue.svg)](https://www.python.org/downloads/release/python-379/) [![Unit tests]
+(https://github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)]
+(https://github.com/spine-tools/spine-engine/
+actions?query=workflow%3A"Unit+tests") [![codecov](https://codecov.io/gh/spine-
+tools/spine-engine/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-
+tools/spine-engine) [![PyPI version](https://badge.fury.io/py/spine-
+engine.svg)](https://badge.fury.io/py/spine-engine) A Python package to
+coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
 Spine-Toolbox) workflows.
                                 [Spine Engine]
 ## License Spine Engine is released under the GNU Lesser General Public License
 (LGPL) license. All accompanying documentation and manual are released under
 the [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/
 by-sa/4.0/). ## Getting started ### Installation To install Spine Engine into
-an existing Python environment, run $ pip install spine_engine ### Dependencies
-Spine Engine installation will install [dagster](https://
-dagster.readthedocs.io/en/master/index.html).  
+an existing Python environment, run $ pip install spine_engine
 ===============================================================================
             This project has received funding from European Climate,
 [EU emblem] Infrastructure and Environment Executive Agency under the European
             Unionâs HORIZON Research and Innovation Actions under grant
             agreement NÂ°101095998.
             This project has received funding from the European Unionâs
 [EU emblem] Horizon 2020 research and innovation programme under grant
```

### Comparing `spine_engine-0.24.0/tests/__init__.py` & `spine_engine-0.24.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/execution_managers/__init__.py` & `spine_engine-0.24.1/tests/execution_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/execution_managers/test_kernel_execution_manager.py` & `spine_engine-0.24.1/tests/execution_managers/test_kernel_execution_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         exec_mngr = KernelExecutionManager(logger, NATIVE_KERNEL_NAME, cmds, group_id="SomeGroup")
         self.assertTrue(exec_mngr._kernel_manager.is_alive())
         exec_mngr = self.replace_client(exec_mngr)
         retval = exec_mngr.run_until_complete()  # Run commands
         self.assertEqual(0, retval)
         self.assertTrue(exec_mngr._kernel_manager.is_alive())
         connection_file = exec_mngr._kernel_manager.connection_file
-        exec_mngr = self.release_exec_mngr_resources(exec_mngr)
-        exec_mngr = None
+        self.release_exec_mngr_resources(exec_mngr)
+        del exec_mngr
         self.assertEqual(1, _kernel_manager_factory.n_kernel_managers())
         _kernel_manager_factory.shutdown_kernel_manager(connection_file)
         self.assertEqual(0, _kernel_manager_factory.n_kernel_managers())
         message_emits = logger.msg_kernel_execution.emit.call_args_list
         expected_msg = {"type": "execution_started", "kernel_name": NATIVE_KERNEL_NAME}
         last_expected_msg = {"type": "stdout", "data": "hello\n"}
         # NOTE: In GitHub unittest runner on Ubuntu Python 3.9+ there is an extra warning message in message_emits
```

### Comparing `spine_engine-0.24.0/tests/execution_managers/test_persistent_execution_manager.py` & `spine_engine-0.24.1/tests/execution_managers/test_persistent_execution_manager.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/execution_managers/test_process_execution_manager.py` & `spine_engine-0.24.1/tests/execution_managers/test_process_execution_manager.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/project_item/__init__.py` & `spine_engine-0.24.1/tests/project_item/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/project_item/test_ExecutableItem.py` & `spine_engine-0.24.1/tests/project_item/test_ExecutableItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Unit tests for ExecutableItem.
-
-"""
+""" Unit tests for ExecutableItem. """
 from tempfile import TemporaryDirectory
 import unittest
 from unittest import mock
 from spine_engine import ExecutionDirection
 from spine_engine.project_item.executable_item_base import ExecutableItemBase
```

### Comparing `spine_engine-0.24.0/tests/project_item/test_connection.py` & `spine_engine-0.24.1/tests/project_item/test_connection.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/project_item/test_project_item_resource.py` & `spine_engine-0.24.1/tests/project_item/test_project_item_resource.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/__init__.py` & `spine_engine-0.24.1/tests/server/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/test_EngineServer.py` & `spine_engine-0.24.1/tests/server/test_EngineServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 # Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option)
 # any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
-"""
-Unit tests for EngineServer class.
-"""
+""" Unit tests for EngineServer class. """
 
 import threading
 import unittest
 import zmq
 import os
 import pathlib
 from spine_engine.server.engine_server import EngineServer, ServerSecurityModel
@@ -171,12 +169,12 @@
         self.assertFalse(server.ctrl_msg_sender.closed)
         self.assertFalse(server._context.closed)
         self.assertTrue(server.is_alive())
         server.close()
         self.assertTrue(server.ctrl_msg_sender.closed)  # PAIR socket should be closed
         self.assertTrue(server._context.closed)  # Context should be closed
         self.assertFalse(server.is_alive())  # server thread should not be alive
-        self.assertEqual(threading.active_count(), 1)  # Only one thread running after close
+        self.assertTrue(all(thread.name != "EngineServerThread" for thread in threading.enumerate()))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `spine_engine-0.24.0/tests/server/test_PingService.py` & `spine_engine-0.24.1/tests/server/test_PingService.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/test_ProjectExtractorService.py` & `spine_engine-0.24.1/tests/server/test_ProjectExtractorService.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/test_ProjectRemoverService.py` & `spine_engine-0.24.1/tests/server/test_ProjectRemoverService.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/test_start_server.py` & `spine_engine-0.24.1/tests/server/test_start_server.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/util/__init__.py` & `spine_engine-0.24.1/tests/server/util/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json` & `spine_engine-0.24.1/tests/server/util/projectforpackagingtests/.spinetoolbox/project.json`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/util/test_EventDataConverter.py` & `spine_engine-0.24.1/tests/server/util/test_EventDataConverter.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/util/test_ServerMessage.py` & `spine_engine-0.24.1/tests/server/util/test_ServerMessage.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/util/test_ZipHandler.py` & `spine_engine-0.24.1/tests/server/util/test_ZipHandler.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/server/zippedproject.zip` & `spine_engine-0.24.1/tests/server/zippedproject.zip`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/test_load_project_items.py` & `spine_engine-0.24.1/tests/test_load_project_items.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/test_spine_engine.py` & `spine_engine-0.24.1/tests/test_spine_engine.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/utils/__init__.py` & `spine_engine-0.24.1/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/utils/test_command_line_args.py` & `spine_engine-0.24.1/tests/utils/test_command_line_args.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/utils/test_helpers.py` & `spine_engine-0.24.1/tests/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.24.0/tests/utils/test_serialization.py` & `spine_engine-0.24.1/tests/utils/test_serialization.py`

 * *Files identical despite different names*

