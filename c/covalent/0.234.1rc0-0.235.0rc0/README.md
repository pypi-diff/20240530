# Comparing `tmp/covalent-0.234.1rc0.tar.gz` & `tmp/covalent-0.235.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-0.234.1rc0.tar", last modified: Fri May 10 12:52:29 2024, max compression
+gzip compressed data, was "covalent-0.235.0rc0.tar", last modified: Thu May 30 10:56:45 2024, max compression
```

## Comparing `covalent-0.234.1rc0.tar` & `covalent-0.235.0rc0.tar`

### file list

```diff
@@ -1,412 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/_api/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_api/apiclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/_dispatcher_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_dispatcher_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_dispatcher_plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_dispatcher_plugins/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/_file_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_file_transfer/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/blob_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/gcloud_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/http_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/rsync_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/s3_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/shutil_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_programmatic/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_programmatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_programmatic/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_results_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/qresult.py
--rw-r--r--   0 runner    (1001) docker     (127)    18128 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/results_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/transport_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/_shared_files/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/pickling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/qelectron_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/qinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/qresult_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/_shared_files/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/transport_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/util_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depsbash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depscall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depsmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depspip.py
--rw-r--r--   0 runner    (1001) docker     (127)    32980 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18557 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/lepton.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/qdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/qelectron.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/qnode.py
--rw-r--r--   0 runner    (1001) docker     (127)    19920 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/transportable_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/cloud_resource_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/cloud_resource_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/cloud_resource_manager/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29163 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/executor_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/executor_plugins/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/executor_plugins/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/executor_plugins/remote_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/qbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.722677 covalent-0.234.1rc0/covalent/executor/quantum_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/leptons/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/leptons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/quantum/qclient/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/quantum/qcluster/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/default_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/quantum/qserver/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/quantum/qserver/servers/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/servers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/database_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/dir_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/sqlite_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/time_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/trigger_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent_dispatcher/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/db_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    31291 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/asset_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/electron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/tg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/tg.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/tg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/tg_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/uri_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_db/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/dispatchdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/write_result_to_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_object_store/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_object_store/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_object_store/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_service/
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/app_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/runnersvc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/26d71848a404_v12.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/97202f5f47cb_v13.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/9b9d58f02985_v11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/b60c5ecdf927_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14035 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/electron_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/graph_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/lattice_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/logs_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16365 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/summary_dal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/database/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/database/config/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/config/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/lattices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/models/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/dispatch_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/electrons_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/graph_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/lattices_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/logs_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/settings_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/routes/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/graph_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/logs_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/api/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/file_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/models_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/result_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.726677 covalent-0.234.1rc0/covalent_ui/webapp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/webapp/build/
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/favicon64x64.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/logo192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    29252 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/logo512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/logo64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.726677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.790677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)  2856333 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127) 10104263 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   307919 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   675742 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   374848 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   958942 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js
--rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/back.c0aa0e78.svg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/close.2a867415.svg
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/download.d767a1c5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/exit.a2c5304b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/logs.551f3d28.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/sublattice.f6ee1fb5.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/zoom-in.f2603f36.svg
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/zoom-out.24dd0db1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/requirements-client.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/requirements-qelectron.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.265981 covalent-0.235.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-30 10:56:45.261981 covalent-0.235.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.185982 covalent-0.235.0rc0/covalent/
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.185982 covalent-0.235.0rc0/covalent/_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_api/apiclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.185982 covalent-0.235.0rc0/covalent/_dispatcher_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_dispatcher_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_dispatcher_plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_dispatcher_plugins/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.185982 covalent-0.235.0rc0/covalent/_file_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.189982 covalent-0.235.0rc0/covalent/_file_transfer/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/blob_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/gcloud_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/http_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/rsync_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/s3_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/shutil_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.189982 covalent-0.235.0rc0/covalent/_programmatic/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_programmatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_programmatic/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.189982 covalent-0.235.0rc0/covalent/_results_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_results_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_results_manager/qresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16965 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_results_manager/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_results_manager/results_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_results_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_results_manager/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.189982 covalent-0.235.0rc0/covalent/_serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_serialize/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_serialize/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_serialize/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_serialize/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_serialize/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.193982 covalent-0.235.0rc0/covalent/_shared_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/qelectron_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/qinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/qresult_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.193982 covalent-0.235.0rc0/covalent/_shared_files/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/schemas/transport_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/util_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_shared_files/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.197981 covalent-0.235.0rc0/covalent/_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/depsbash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/depscall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/depsmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/depspip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32972 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18557 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/lepton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/qdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/qelectron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/qnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19920 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/_workflow/transportable_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.197981 covalent-0.235.0rc0/covalent/cloud_resource_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/cloud_resource_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/cloud_resource_manager/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.197981 covalent-0.235.0rc0/covalent/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29163 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.197981 covalent-0.235.0rc0/covalent/executor/executor_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/executor_plugins/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/executor_plugins/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/executor_plugins/remote_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/qbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.177981 covalent-0.235.0rc0/covalent/executor/quantum_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.197981 covalent-0.235.0rc0/covalent/executor/quantum_plugins/aws_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.201981 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.201981 covalent-0.235.0rc0/covalent/executor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/utils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/executor/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.201981 covalent-0.235.0rc0/covalent/leptons/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/leptons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.201981 covalent-0.235.0rc0/covalent/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.201981 covalent-0.235.0rc0/covalent/quantum/qclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qclient/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qclient/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qclient/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.201981 covalent-0.235.0rc0/covalent/quantum/qcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qcluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qcluster/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qcluster/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qcluster/default_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qcluster/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.201981 covalent-0.235.0rc0/covalent/quantum/qserver/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qserver/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qserver/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qserver/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.205981 covalent-0.235.0rc0/covalent/quantum/qserver/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qserver/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qserver/servers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/quantum/qserver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.205981 covalent-0.235.0rc0/covalent/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/triggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/triggers/database_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/triggers/dir_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/triggers/sqlite_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/triggers/time_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent/triggers/trigger_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.185982 covalent-0.235.0rc0/covalent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-30 10:56:45.000000 covalent-0.235.0rc0/covalent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-05-30 10:56:45.000000 covalent-0.235.0rc0/covalent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:56:45.000000 covalent-0.235.0rc0/covalent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 10:56:45.000000 covalent-0.235.0rc0/covalent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:56:45.000000 covalent-0.235.0rc0/covalent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-30 10:56:45.000000 covalent-0.235.0rc0/covalent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 10:56:45.000000 covalent-0.235.0rc0/covalent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.205981 covalent-0.235.0rc0/covalent_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.205981 covalent-0.235.0rc0/covalent_dispatcher/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.205981 covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/db_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/deploy_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30955 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.205981 covalent-0.235.0rc0/covalent_dispatcher/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.209981 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/asset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.209981 covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher_modules/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.209981 covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_core/runner_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.213981 covalent-0.235.0rc0/covalent_dispatcher/_dal/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.213981 covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.213981 covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/tg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.213981 covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/tg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/tg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/tg_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.213981 covalent-0.235.0rc0/covalent_dispatcher/_dal/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/utils/file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_dal/utils/uri_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.217981 covalent-0.235.0rc0/covalent_dispatcher/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/dispatchdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15479 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_db/write_result_to_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.217981 covalent-0.235.0rc0/covalent_dispatcher/_object_store/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_object_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_object_store/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.217981 covalent-0.235.0rc0/covalent_dispatcher/_service/
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_service/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_service/app_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_service/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_service/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_service/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_service/runnersvc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.217981 covalent-0.235.0rc0/covalent_dispatcher/_triggers_app/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_triggers_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/_triggers_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_dispatcher/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.217981 covalent-0.235.0rc0/covalent_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/26d71848a404_v12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/97202f5f47cb_v13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/9b9d58f02985_v11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/b60c5ecdf927_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_ui/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_ui/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14035 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/electron_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/graph_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/lattice_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/logs_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16365 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/summary_dal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_ui/api/v1/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_ui/api/v1/database/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/database/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/database/config/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.221981 covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/electron_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/lattices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.225981 covalent-0.235.0rc0/covalent_ui/api/v1/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/models/dispatch_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/models/electrons_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/models/graph_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/models/lattices_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/models/logs_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/models/settings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.225981 covalent-0.235.0rc0/covalent_ui/api/v1/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.225981 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/graph_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/logs_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/routes/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.225981 covalent-0.235.0rc0/covalent_ui/api/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/utils/file_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/utils/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/utils/models_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/api/v1/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-30 10:53:40.000000 covalent-0.235.0rc0/covalent_ui/result_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.181982 covalent-0.235.0rc0/covalent_ui/webapp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.225981 covalent-0.235.0rc0/covalent_ui/webapp/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-30 10:54:35.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-30 10:54:35.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/favicon64x64.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-30 10:54:35.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/logo192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29252 2024-05-30 10:54:35.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/logo512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-30 10:54:35.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/logo64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-30 10:54:35.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 10:54:35.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.181982 covalent-0.235.0rc0/covalent_ui/webapp/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.229981 covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.253981 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  2856333 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 10104263 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   307919 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   675742 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   374848 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   958942 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:56:45.261981 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/back.c0aa0e78.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/close.2a867415.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/download.d767a1c5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/exit.a2c5304b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/logs.551f3d28.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/sublattice.f6ee1fb5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/zoom-in.f2603f36.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 10:56:43.000000 covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/zoom-out.24dd0db1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-30 10:53:41.000000 covalent-0.235.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-30 10:53:41.000000 covalent-0.235.0rc0/requirements-client.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 10:53:41.000000 covalent-0.235.0rc0/requirements-qelectron.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-30 10:53:41.000000 covalent-0.235.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:56:45.265981 covalent-0.235.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-05-30 10:53:41.000000 covalent-0.235.0rc0/setup.py
```

### Comparing `covalent-0.234.1rc0/LICENSE` & `covalent-0.235.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/PKG-INFO` & `covalent-0.235.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent
-Version: 0.234.1rc0
+Version: 0.235.0rc0
 Summary: Covalent Workflow Tool
 Home-page: https://github.com/AgnostiqHQ/covalent
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: Apache License 2.0
-Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.234.1-rc.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.235.0-rc.0.tar.gz
 Description: <div align="center">
           <img src="./doc/source/_static/banner_executor.gif" alt="hero" />
         </div>
         </br>
         <div align="center">
         
         [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https://github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: covalent Version: 0.234.1rc0 Summary: Covalent
+Metadata-Version: 2.1 Name: covalent Version: 0.235.0rc0 Summary: Covalent
 Workflow Tool Home-page: https://github.com/AgnostiqHQ/covalent Author:
 Agnostiq Author-email: support@agnostiq.ai Maintainer: Agnostiq License: Apache
 License 2.0 Download-URL: https://github.com/AgnostiqHQ/covalent/archive/
-v0.234.1-rc.0.tar.gz Description:
+v0.235.0-rc.0.tar.gz Description:
                                     [hero]
           [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/
 covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https:
  //github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md) [![Static Badge]
   (https://img.shields.io/badge/python-3.8_%7C_3.9_%7C_3.10-%235552FF)](#) [!
           [Static Badge](https://img.shields.io/badge/tests-passing-
     %235552FF?logo=github)](https://github.com/AgnostiqHQ/covalent/actions/
```

### Comparing `covalent-0.234.1rc0/README.md` & `covalent-0.235.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/__init__.py` & `covalent-0.235.0rc0/covalent/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_api/__init__.py` & `covalent-0.235.0rc0/covalent/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_api/apiclient.py` & `covalent-0.235.0rc0/covalent/_api/apiclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     """Thin wrapper around Requests to centralize error handling."""
 
     def __init__(self, dispatcher_addr: str, adapter: HTTPAdapter = None, auto_raise: bool = True):
         self.dispatcher_addr = dispatcher_addr
         self.adapter = adapter
         self.auto_raise = auto_raise
 
-    def prepare_headers(self, **kwargs):
+    def prepare_headers(self, kwargs):
         extra_headers = CovalentAPIClient.get_extra_headers()
         headers = kwargs.get("headers", {})
         if headers:
             kwargs.pop("headers")
         headers.update(extra_headers)
         return headers
 
     def get(self, endpoint: str, **kwargs):
-        headers = self.prepare_headers(**kwargs)
+        headers = self.prepare_headers(kwargs)
         url = self.dispatcher_addr + endpoint
         try:
             with requests.Session() as session:
                 if self.adapter:
                     session.mount("http://", self.adapter)
 
                 r = session.get(url, headers=headers, **kwargs)
@@ -58,15 +58,15 @@
             message = f"The Covalent server cannot be reached at {url}. Local servers can be started using `covalent start` in the terminal. If you are using a remote Covalent server, contact your systems administrator to report an outage."
             print(message)
             raise
 
         return r
 
     def put(self, endpoint: str, **kwargs):
-        headers = self.prepare_headers()
+        headers = self.prepare_headers(kwargs)
         url = self.dispatcher_addr + endpoint
         try:
             with requests.Session() as session:
                 if self.adapter:
                     session.mount("http://", self.adapter)
 
                 r = session.put(url, headers=headers, **kwargs)
@@ -77,15 +77,15 @@
             message = f"The Covalent server cannot be reached at {url}. Local servers can be started using `covalent start` in the terminal. If you are using a remote Covalent server, contact your systems administrator to report an outage."
             print(message)
             raise
 
         return r
 
     def post(self, endpoint: str, **kwargs):
-        headers = self.prepare_headers()
+        headers = self.prepare_headers(kwargs)
         url = self.dispatcher_addr + endpoint
         try:
             with requests.Session() as session:
                 if self.adapter:
                     session.mount("http://", self.adapter)
 
                 r = session.post(url, headers=headers, **kwargs)
@@ -96,15 +96,15 @@
             message = f"The Covalent server cannot be reached at {url}. Local servers can be started using `covalent start` in the terminal. If you are using a remote Covalent server, contact your systems administrator to report an outage."
             print(message)
             raise
 
         return r
 
     def delete(self, endpoint: str, **kwargs):
-        headers = self.prepare_headers()
+        headers = self.prepare_headers(kwargs)
         url = self.dispatcher_addr + endpoint
         try:
             with requests.Session() as session:
                 if self.adapter:
                     session.mount("http://", self.adapter)
 
                 r = session.delete(url, headers=headers, **kwargs)
```

### Comparing `covalent-0.234.1rc0/covalent/_dispatcher_plugins/__init__.py` & `covalent-0.235.0rc0/covalent/_dispatcher_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_dispatcher_plugins/base.py` & `covalent-0.235.0rc0/covalent/_dispatcher_plugins/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_dispatcher_plugins/local.py` & `covalent-0.235.0rc0/covalent/_dispatcher_plugins/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Use of this file is prohibited except in compliance with the License.
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
 import tempfile
 from copy import deepcopy
 from functools import wraps
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 from furl import furl
@@ -43,14 +44,17 @@
 app_log = logger.app_log
 log_stack_info = logger.log_stack_info
 
 dispatch_cache_dir = Path(get_config("sdk.dispatch_cache_dir"))
 dispatch_cache_dir.mkdir(parents=True, exist_ok=True)
 
 
+BASE_ENDPOINT = os.getenv("COVALENT_DISPATCH_BASE_ENDPOINT", "/api/v2/dispatches")
+
+
 def get_redispatch_request_body_v2(
     dispatch_id: str,
     staging_dir: str,
     new_args: List,
     new_kwargs: Dict,
     replace_electrons: Optional[Dict[str, Callable]],
     dispatcher_addr: str = None,
@@ -536,18 +540,18 @@
             automatically pull the task assets from the submitted asset URIs.
         """
 
         if dispatcher_addr is None:
             dispatcher_addr = format_server_url()
 
         stripped = strip_local_uris(manifest) if push_assets else manifest
-        endpoint = "/api/v2/dispatches"
+        endpoint = BASE_ENDPOINT
 
         if parent_dispatch_id:
-            endpoint = f"{endpoint}/{parent_dispatch_id}/subdispatches"
+            endpoint = f"{BASE_ENDPOINT}/{parent_dispatch_id}/sublattices"
 
         r = APIClient(dispatcher_addr).post(endpoint, data=stripped.model_dump_json())
         r.raise_for_status()
 
         parsed_resp = ResultSchema.model_validate(r.json())
 
         return merge_response_manifest(manifest, parsed_resp)
@@ -592,38 +596,44 @@
     @staticmethod
     def _upload(assets: List[AssetSchema]):
         local_scheme_prefix = "file://"
         total = len(assets)
         number_uploaded = 0
         for i, asset in enumerate(assets):
             if not asset.remote_uri or not asset.uri:
-                app_log.debug(f"Skipping asset {i+1} out of {total}")
+                app_log.debug(f"Skipping asset {i + 1} out of {total}")
                 continue
             if asset.remote_uri.startswith(local_scheme_prefix):
                 copy_file_locally(asset.uri, asset.remote_uri)
                 number_uploaded += 1
             else:
                 _upload_asset(asset.uri, asset.remote_uri)
                 number_uploaded += 1
-            app_log.debug(f"Uploaded asset {i+1} out of {total}.")
+            app_log.debug(f"Uploaded asset {i + 1} out of {total}.")
         app_log.debug(f"uploaded {number_uploaded} assets.")
 
 
 def _upload_asset(local_uri, remote_uri):
     scheme_prefix = "file://"
     if local_uri.startswith(scheme_prefix):
         local_path = local_uri[len(scheme_prefix) :]
     else:
         local_path = local_uri
 
+    filesize = os.path.getsize(local_path)
     with open(local_path, "rb") as reader:
         app_log.debug(f"uploading to {remote_uri}")
         f = furl(remote_uri)
         scheme = f.scheme
         host = f.host
         port = f.port
         dispatcher_addr = f"{scheme}://{host}:{port}"
         endpoint = str(f.path)
         api_client = APIClient(dispatcher_addr)
+        if f.query:
+            endpoint = f"{endpoint}?{f.query}"
+
+        # Workaround for Requests bug when streaming from empty files
+        data = reader.read() if filesize < 50 else reader
 
-        r = api_client.put(endpoint, data=reader)
+        r = api_client.put(endpoint, headers={"Content-Length": str(filesize)}, data=data)
         r.raise_for_status()
```

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/__init__.py` & `covalent-0.235.0rc0/covalent/_file_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/enums.py` & `covalent-0.235.0rc0/covalent/_file_transfer/enums.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/file.py` & `covalent-0.235.0rc0/covalent/_file_transfer/file.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/file_transfer.py` & `covalent-0.235.0rc0/covalent/_file_transfer/file_transfer.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/folder.py` & `covalent-0.235.0rc0/covalent/_file_transfer/folder.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/__init__.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/blob_strategy.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/blob_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/gcloud_strategy.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/gcloud_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/http_strategy.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/http_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/rsync_strategy.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/rsync_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/s3_strategy.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/s3_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/shutil_strategy.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/shutil_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py` & `covalent-0.235.0rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_programmatic/__init__.py` & `covalent-0.235.0rc0/covalent/_programmatic/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_programmatic/commands.py` & `covalent-0.235.0rc0/covalent/_programmatic/commands.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_results_manager/__init__.py` & `covalent-0.235.0rc0/covalent/_results_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_results_manager/qresult.py` & `covalent-0.235.0rc0/covalent/_results_manager/qresult.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_results_manager/result.py` & `covalent-0.235.0rc0/covalent/_results_manager/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Result object."""
 import os
 import re
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Set, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 from .._shared_files import logger
 from .._shared_files.config import get_config
 from .._shared_files.context_managers import active_lattice_manager
 from .._shared_files.defaults import postprocess_prefix, prefix_separator, sublattice_prefix
 from .._shared_files.util_classes import RESULT_STATUS, Status
 from .._workflow.lattice import Lattice
@@ -512,38 +512,7 @@
             None
 
         Returns:
             result: The final output of the dispatch.
         """
 
         return self._result
-
-
-def _filter_cova_decorators(function_string: str, cova_imports: Set[str]) -> str:
-    """
-    Given a string representing a function, comment out any Covalent-related decorators.
-
-    Args
-        function_string: A string representation of a workflow function.
-
-    Returns:
-        The function string with Covalent-related decorators commented out.
-    """
-
-    has_cova_decorator = False
-    in_decorator = 0
-    function_lines = function_string.split("\n")
-    for i in range(len(function_lines)):
-        line = function_lines[i].strip()
-        if in_decorator > 0:
-            function_lines[i] = f"# {function_lines[i]}"
-            in_decorator += line.count("(")
-            in_decorator -= line.count(")")
-        elif line.startswith("@"):
-            decorator_name = line.split("@")[1].split(".")[0].split("(")[0]
-            if decorator_name in cova_imports:
-                function_lines[i] = f"# {function_lines[i]}"
-                has_cova_decorator = True
-                in_decorator += line.count("(")
-                in_decorator -= line.count(")")
-
-    return "\n".join(function_lines) if has_cova_decorator else function_string
```

### Comparing `covalent-0.234.1rc0/covalent/_results_manager/results_manager.py` & `covalent-0.235.0rc0/covalent/_results_manager/results_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_results_manager/utils.py` & `covalent-0.235.0rc0/covalent/_results_manager/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_results_manager/wait.py` & `covalent-0.235.0rc0/covalent/_results_manager/wait.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_serialize/__init__.py` & `covalent-0.235.0rc0/covalent/_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_serialize/common.py` & `covalent-0.235.0rc0/covalent/_serialize/common.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_serialize/electron.py` & `covalent-0.235.0rc0/covalent/_serialize/electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,16 @@
     if "custom_asset_keys" in node_attrs["metadata"]:
         return {key: AssetSchema(size=0) for key in node_attrs["metadata"]["custom_asset_keys"]}
 
 
 def serialize_node(node_id: int, node_attrs: dict, node_storage_path) -> ElectronSchema:
     meta = _serialize_node_metadata(node_attrs, node_storage_path)
     assets = _serialize_node_assets(node_attrs, node_storage_path)
-    custom_assets = _get_node_custom_assets(node_attrs)
-    return ElectronSchema(id=node_id, metadata=meta, assets=assets, custom_assets=custom_assets)
+    assets._custom = _get_node_custom_assets(node_attrs)
+    return ElectronSchema(id=node_id, metadata=meta, assets=assets)
 
 
 def deserialize_node(e: ElectronSchema, metadata_only: bool = False) -> dict:
     node_attrs = _deserialize_node_metadata(e.metadata)
     node_assets = _deserialize_node_assets(e.assets)
 
     asset_metadata = node_assets.pop("metadata")
```

### Comparing `covalent-0.234.1rc0/covalent/_serialize/lattice.py` & `covalent-0.235.0rc0/covalent/_serialize/lattice.py`

 * *Files 26% similar despite different names*

```diff
@@ -36,18 +36,14 @@
 
 
 ASSET_TYPES = {
     "workflow_function": AssetType.TRANSPORTABLE,
     "workflow_function_string": AssetType.TEXT,
     "doc": AssetType.TEXT,
     "inputs": AssetType.TRANSPORTABLE,
-    "named_args": AssetType.TRANSPORTABLE,
-    "named_kwargs": AssetType.TRANSPORTABLE,
-    "cova_imports": AssetType.JSONABLE,
-    "lattice_imports": AssetType.TEXT,
     "hooks": AssetType.JSONABLE,
 }
 
 
 def _serialize_lattice_metadata(lat) -> LatticeMetadata:
     name = lat.__name__
     executor = lat.metadata["executor"]
@@ -108,102 +104,61 @@
         ASSET_FILENAME_MAP["doc"],
     )
 
     inputs_asset = save_asset(
         lat.inputs, ASSET_TYPES["inputs"], storage_path, ASSET_FILENAME_MAP["inputs"]
     )
 
-    # Deprecate
-    named_args_asset = save_asset(
-        lat.named_args,
-        ASSET_TYPES["named_args"],
-        storage_path,
-        ASSET_FILENAME_MAP["named_args"],
-    )
-    named_kwargs_asset = save_asset(
-        lat.named_kwargs,
-        ASSET_TYPES["named_kwargs"],
-        storage_path,
-        ASSET_FILENAME_MAP["named_kwargs"],
-    )
-    cova_imports_asset = save_asset(
-        lat.cova_imports,
-        ASSET_TYPES["cova_imports"],
-        storage_path,
-        ASSET_FILENAME_MAP["cova_imports"],
-    )
-    lattice_imports_asset = save_asset(
-        lat.lattice_imports,
-        ASSET_TYPES["lattice_imports"],
-        storage_path,
-        ASSET_FILENAME_MAP["lattice_imports"],
-    )
-
-    # NOTE: these are actually JSONable
     hooks_asset = save_asset(
         lat.metadata["hooks"],
         ASSET_TYPES["hooks"],
         storage_path,
         ASSET_FILENAME_MAP["hooks"],
     )
 
     return LatticeAssets(
         workflow_function=workflow_func_asset,
         workflow_function_string=workflow_func_str_asset,
         doc=docstring_asset,
         inputs=inputs_asset,
-        named_args=named_args_asset,
-        named_kwargs=named_kwargs_asset,
-        cova_imports=cova_imports_asset,
-        lattice_imports=lattice_imports_asset,
         hooks=hooks_asset,
     )
 
 
 def _deserialize_lattice_assets(assets: LatticeAssets) -> dict:
     workflow_function = load_asset(assets.workflow_function, ASSET_TYPES["workflow_function"])
     workflow_function_string = load_asset(
         assets.workflow_function_string, ASSET_TYPES["workflow_function_string"]
     )
     doc = load_asset(assets.doc, ASSET_TYPES["doc"])
     inputs = load_asset(assets.inputs, ASSET_TYPES["inputs"])
-    named_args = load_asset(assets.named_args, ASSET_TYPES["named_args"])
-    named_kwargs = load_asset(assets.named_kwargs, ASSET_TYPES["named_kwargs"])
-    cova_imports = load_asset(assets.cova_imports, ASSET_TYPES["cova_imports"])
-    lattice_imports = load_asset(assets.lattice_imports, ASSET_TYPES["lattice_imports"])
     hooks = load_asset(assets.hooks, ASSET_TYPES["hooks"])
     return {
         "workflow_function": workflow_function,
         "workflow_function_string": workflow_function_string,
         "__doc__": doc,
         "inputs": inputs,
-        "named_args": named_args,
-        "named_kwargs": named_kwargs,
-        "cova_imports": cova_imports,
-        "lattice_imports": lattice_imports,
         "metadata": {
             "hooks": hooks,
         },
     }
 
 
 def _get_lattice_custom_assets(lat: Lattice) -> Dict[str, AssetSchema]:
     if "custom_asset_keys" in lat.metadata:
         return {key: AssetSchema(size=0) for key in lat.metadata["custom_asset_keys"]}
 
 
 def serialize_lattice(lat, storage_path: str) -> LatticeSchema:
     meta = _serialize_lattice_metadata(lat)
     assets = _serialize_lattice_assets(lat, storage_path)
-    custom_assets = _get_lattice_custom_assets(lat)
+    assets._custom = _get_lattice_custom_assets(lat)
     tg = serialize_transport_graph(lat.transport_graph, storage_path)
 
-    return LatticeSchema(
-        metadata=meta, assets=assets, custom_assets=custom_assets, transport_graph=tg
-    )
+    return LatticeSchema(metadata=meta, assets=assets, transport_graph=tg)
 
 
 def deserialize_lattice(model: LatticeSchema) -> Lattice:
     def dummy_function(x):
         return x
 
     lat = Lattice(dummy_function)
```

### Comparing `covalent-0.234.1rc0/covalent/_serialize/result.py` & `covalent-0.235.0rc0/covalent/_serialize/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_serialize/transport_graph.py` & `covalent-0.235.0rc0/covalent/_serialize/transport_graph.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/__init__.py` & `covalent-0.235.0rc0/covalent/_shared_files/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/config.py` & `covalent-0.235.0rc0/covalent/_shared_files/config.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/context_managers.py` & `covalent-0.235.0rc0/covalent/_shared_files/context_managers.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/defaults.py` & `covalent-0.235.0rc0/covalent/_shared_files/defaults.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/exceptions.py` & `covalent-0.235.0rc0/covalent/_shared_files/exceptions.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/logger.py` & `covalent-0.235.0rc0/covalent/_shared_files/logger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/metrics.py` & `covalent-0.235.0rc0/covalent/_shared_files/metrics.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/pickling.py` & `covalent-0.235.0rc0/covalent/_shared_files/pickling.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/qelectron_utils.py` & `covalent-0.235.0rc0/covalent/_shared_files/qelectron_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/qinfo.py` & `covalent-0.235.0rc0/covalent/_shared_files/qinfo.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/qresult_utils.py` & `covalent-0.235.0rc0/covalent/_shared_files/qresult_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/__init__.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/asset.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/asset.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/common.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/common.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/edge.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/edge.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/electron.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/electron.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 
 """FastAPI models for /api/v1/resultv2 endpoints"""
 
 from datetime import datetime
 from typing import Dict, Optional
 
-from pydantic import BaseModel, field_validator
+from pydantic import BaseModel
 
 from .asset import AssetSchema
 from .common import StatusEnum
 
 ELECTRON_METADATA_KEYS = {
     "task_group_id",
     "name",
@@ -87,39 +87,34 @@
     stdout: Optional[AssetSchema] = None
     stderr: Optional[AssetSchema] = None
     qelectron_db: Optional[AssetSchema] = None
 
     # user dependent assets
     hooks: AssetSchema
 
+    _custom: Optional[Dict[str, AssetSchema]] = None
+
 
 class ElectronMetadata(BaseModel):
     task_group_id: int
     name: str
     executor: str
     executor_data: dict
     qelectron_data_exists: Optional[bool] = None
     sub_dispatch_id: Optional[str] = None
     status: StatusEnum
     start_time: Optional[datetime] = None
     end_time: Optional[datetime] = None
 
+    _custom: Optional[Dict] = None
+
     # For use by redispatch
     def reset(self):
         self.status = StatusEnum.NEW_OBJECT
         self.start_time = None
         self.end_time = None
 
 
 class ElectronSchema(BaseModel):
     id: int
     metadata: ElectronMetadata
     assets: ElectronAssets
-    custom_assets: Optional[Dict[str, AssetSchema]] = None
-
-    @field_validator("custom_assets")
-    def check_custom_asset_keys(cls, v):
-        if v is not None:
-            for key in v:
-                if key in ASSET_FILENAME_MAP:
-                    raise ValueError(f"Asset {key} conflicts with built-in key")
-        return v
```

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/lattice.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/lattice.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """FastAPI models for /api/v1/resultv2 endpoints"""
 
 from typing import Dict, Optional
 
-from pydantic import BaseModel, field_validator
+from pydantic import BaseModel
 
 from .asset import AssetSchema
 from .transport_graph import TransportGraphSchema
 
 LATTICE_METADATA_KEYS = {
     "__name__",
     "python_version",
@@ -35,18 +35,14 @@
 }
 
 LATTICE_ASSET_KEYS = {
     "workflow_function",
     "workflow_function_string",
     "__doc__",
     "inputs",
-    "named_args",
-    "named_kwargs",
-    "cova_imports",
-    "lattice_imports",
     # user dependent assets
     "hooks",
 }
 
 LATTICE_FUNCTION_FILENAME = "function.tobj"
 LATTICE_FUNCTION_STRING_FILENAME = "function_string.txt"
 LATTICE_DOCSTRING_FILENAME = "function_docstring.txt"
@@ -79,40 +75,37 @@
 
 
 class LatticeAssets(BaseModel):
     workflow_function: AssetSchema
     workflow_function_string: AssetSchema
     doc: AssetSchema  # __doc__
     inputs: AssetSchema
-    named_args: AssetSchema
-    named_kwargs: AssetSchema
-    cova_imports: AssetSchema
-    lattice_imports: AssetSchema
+
+    # Deprecated
+    named_args: AssetSchema = AssetSchema(size=0)
+    named_kwargs: AssetSchema = AssetSchema(size=0)
+    cova_imports: AssetSchema = AssetSchema(size=0)
+    lattice_imports: AssetSchema = AssetSchema(size=0)
 
     # lattice.metadata
     hooks: AssetSchema
 
+    _custom: Optional[Dict[str, AssetSchema]] = None
+
 
 class LatticeMetadata(BaseModel):
     name: str  # __name__
     executor: str
     executor_data: dict
     workflow_executor: str
     workflow_executor_data: dict
     python_version: Optional[str] = None
     covalent_version: Optional[str] = None
 
+    _custom: Optional[Dict] = None
+
 
 class LatticeSchema(BaseModel):
     metadata: LatticeMetadata
     assets: LatticeAssets
-    custom_assets: Optional[Dict[str, AssetSchema]] = None
 
     transport_graph: TransportGraphSchema
-
-    @field_validator("custom_assets")
-    def check_custom_asset_keys(cls, v):
-        if v is not None:
-            for key in v:
-                if key in ASSET_FILENAME_MAP:
-                    raise ValueError(f"Asset {key} conflicts with built-in key")
-        return v
```

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/result.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """FastAPI models for /api/v1/resultv2 endpoints"""
 
 from datetime import datetime
-from typing import Optional
+from typing import Dict, Optional
 
 from pydantic import BaseModel
 
 from .asset import AssetSchema
 from .common import StatusEnum
 from .lattice import LATTICE_ERROR_FILENAME, LATTICE_RESULTS_FILENAME, LatticeSchema
 
@@ -50,27 +50,31 @@
 class ResultMetadata(BaseModel):
     dispatch_id: str
     root_dispatch_id: str
     status: StatusEnum
     start_time: Optional[datetime] = None
     end_time: Optional[datetime] = None
 
+    _custom: Optional[Dict] = None
+
     # For use by redispatch
     def reset(self):
         self.dispatch_id = ""
         self.root_dispatch_id = ""
         self.status = StatusEnum.NEW_OBJECT
         self.start_time = None
         self.end_time = None
 
 
 class ResultAssets(BaseModel):
     result: AssetSchema
     error: AssetSchema
 
+    _custom: Optional[Dict[str, AssetSchema]] = None
+
 
 class ResultSchema(BaseModel):
     metadata: ResultMetadata
     assets: ResultAssets
     lattice: LatticeSchema
 
     # For use by redispatch
```

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/schemas/transport_graph.py` & `covalent-0.235.0rc0/covalent/_shared_files/schemas/transport_graph.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/util_classes.py` & `covalent-0.235.0rc0/covalent/_shared_files/util_classes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_shared_files/utils.py` & `covalent-0.235.0rc0/covalent/_shared_files/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/__init__.py` & `covalent-0.235.0rc0/covalent/_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/deps.py` & `covalent-0.235.0rc0/covalent/_workflow/deps.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/depsbash.py` & `covalent-0.235.0rc0/covalent/_workflow/depsbash.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/depscall.py` & `covalent-0.235.0rc0/covalent/_workflow/depscall.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/depsmodule.py` & `covalent-0.235.0rc0/covalent/_workflow/depsmodule.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/depspip.py` & `covalent-0.235.0rc0/covalent/_workflow/depspip.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/electron.py` & `covalent-0.235.0rc0/covalent/_workflow/electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,29 +425,33 @@
                 "status",
                 RESULT_STATUS.PENDING_REPLACEMENT,
             )
 
             active_lattice.replace_electrons[name] = replacement_electron
             return bound_electron
 
+        # Avoid direct attribute access since that might trigger
+        # Electron.__getattr__ when executors build sublattices
+        # constructed with older versions of Covalent
+        function_string = self.__dict__.get("_function_string")
+
         # Handle sublattices by injecting _build_sublattice_graph node
         if isinstance(self.function, Lattice):
             parent_metadata = active_lattice.metadata.copy()
             app_log.debug(f"Parent lattice metadata: {parent_metadata}")
             e_meta = parent_metadata.copy()
             e_meta["executor"] = e_meta.pop("workflow_executor")
             e_meta["executor_data"] = e_meta.pop("workflow_executor_data")
 
             sub_electron = Electron(
                 function=_build_sublattice_graph,
                 metadata=e_meta,
             )
 
             name = sublattice_prefix + self.function.__name__
-            function_string = self._function_string
             bound_electron = sub_electron(
                 self.function, json.dumps(parent_metadata), *args, **kwargs
             )
 
             active_lattice.transport_graph.set_node_value(bound_electron.node_id, "name", name)
             active_lattice.transport_graph.set_node_value(
                 bound_electron.node_id,
@@ -460,15 +464,15 @@
         # Add a node to the transport graph of the active lattice. Electrons bound to nodes will never be packed with the
         # 'master' Electron. # Add non-sublattice node to the transport graph of the active lattice.
 
         self.node_id = active_lattice.transport_graph.add_node(
             name=self.function.__name__,
             function=self.function,
             metadata=self.metadata.copy(),
-            function_string=self._function_string,
+            function_string=function_string,
             task_group_id=self.task_group_id if self.packing_tasks else None,
         )
         self.task_group_id = self.task_group_id if self.packing_tasks else self.node_id
 
         if self.function:
             named_args, named_kwargs = get_named_params(self.function, args, kwargs)
 
@@ -843,35 +847,27 @@
 
     if active_lattice and not active_lattice.post_processing:
         return child.wait_for(parents)
     else:
         return child
 
 
-@electron
-def to_decoded_electron_collection(**x):
-    """Interchanges order of serialize -> collection"""
-    collection = list(x.values())[0]
-    if isinstance(collection, list):
-        return TransportableObject.deserialize_list(collection)
-    elif isinstance(collection, dict):
-        return TransportableObject.deserialize_dict(collection)
-
-
 # Copied from runner.py
 def _build_sublattice_graph(sub: Lattice, json_parent_metadata: str, *args, **kwargs):
     import os
 
     parent_metadata = json.loads(json_parent_metadata)
     for k in sub.metadata.keys():
         if not sub.metadata[k] and k != "triggers":
             sub.metadata[k] = parent_metadata[k]
 
     sub.build_graph(*args, **kwargs)
 
+    DISABLE_LEGACY_SUBLATTICES = os.environ.get("COVALENT_DISABLE_LEGACY_SUBLATTICES") == "1"
+
     try:
         # Attempt multistage sublattice dispatch. For now we require
         # the executor to reach the Covalent server
         parent_dispatch_id = os.environ["COVALENT_DISPATCH_ID"]
         dispatcher_url = os.environ["COVALENT_DISPATCHER_URL"]
 
         with tempfile.TemporaryDirectory(prefix="covalent-") as staging_path:
@@ -887,9 +883,11 @@
             )
             LocalDispatcher.upload_assets(recv_manifest)
 
         return recv_manifest.model_dump_json()
 
     except Exception as ex:
         # Fall back to legacy sublattice handling
+        if DISABLE_LEGACY_SUBLATTICES:
+            raise
         print("Falling back to legacy sublattice handling")
         return sub.serialize_to_json()
```

### Comparing `covalent-0.234.1rc0/covalent/_workflow/lattice.py` & `covalent-0.235.0rc0/covalent/_workflow/lattice.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 )
 
 if TYPE_CHECKING:
     from .._results_manager.result import Result
     from ..executor import BaseExecutor
     from ..triggers import BaseTrigger
 
-from .._shared_files.utils import get_imports, get_serialized_function_str
+from .._shared_files.utils import get_serialized_function_str
 
 consumable_constraints = []
 
 DEFAULT_METADATA_VALUES = asdict(DefaultMetadataValues())
 
 app_log = logger.app_log
 log_stack_info = logger.log_stack_info
@@ -77,18 +77,15 @@
         self.workflow_function_string = get_serialized_function_str(self.workflow_function)
         self.transport_graph = transport_graph or _TransportGraph()
         self.metadata = {}
         self.__name__ = self.workflow_function.__name__
         self.__doc__ = self.workflow_function.__doc__
         self.post_processing = False
         self.inputs = None
-        self.named_args = None
-        self.named_kwargs = None
         self.electron_outputs = {}
-        self.lattice_imports, self.cova_imports = get_imports(self.workflow_function)
 
         self.workflow_function = TransportableObject.make_transportable(self.workflow_function)
 
         # Bound electrons are defined as electrons with a valid node_id, since it means they are bound to a TransportGraph.
         self._bound_electrons = {}  # Clear before serializing
 
         self.python_version = self.workflow_function.python_version
@@ -101,32 +98,28 @@
 
         attributes["metadata"] = encode_metadata(self.metadata)
         attributes["transport_graph"] = None
         if self.transport_graph:
             attributes["transport_graph"] = self.transport_graph.serialize_to_json()
 
         attributes["inputs"] = self.inputs.to_dict()
-        attributes["named_args"] = self.named_args.to_dict()
-        attributes["named_kwargs"] = self.named_kwargs.to_dict()
 
         attributes["electron_outputs"] = {}
         for node_name, output in self.electron_outputs.items():
             attributes["electron_outputs"][node_name] = output.to_dict()
 
         return json.dumps(attributes)
 
     @staticmethod
     def deserialize_from_json(json_data: str) -> None:
         attributes = json.loads(json_data)
 
         for node_name, object_dict in attributes["electron_outputs"].items():
             attributes["electron_outputs"][node_name] = TransportableObject.from_dict(object_dict)
 
-        attributes["named_kwargs"] = TransportableObject.from_dict(attributes["named_kwargs"])
-        attributes["named_args"] = TransportableObject.from_dict(attributes["named_args"])
         attributes["inputs"] = TransportableObject.from_dict(attributes["inputs"])
 
         if attributes["transport_graph"]:
             tg = _TransportGraph()
             tg.deserialize_from_json(attributes["transport_graph"])
             attributes["transport_graph"] = tg
 
@@ -205,17 +198,14 @@
         workflow_function = self.workflow_function.get_deserialized()
 
         named_args, named_kwargs = get_named_params(workflow_function, args, kwargs)
         new_args = [v for _, v in named_args.items()]
         new_kwargs = dict(named_kwargs.items())
 
         self.inputs = TransportableObject({"args": args, "kwargs": kwargs})
-        self.named_args = TransportableObject(named_args)
-        self.named_kwargs = TransportableObject(named_kwargs)
-        self.lattice_imports, self.cova_imports = get_imports(workflow_function)
 
         # Set any lattice metadata not explicitly set by the user
         constraint_names = {"executor", "workflow_executor", "hooks"}
         new_metadata = {
             name: DEFAULT_METADATA_VALUES[name]
             for name in constraint_names
             if self.metadata[name] is None
```

### Comparing `covalent-0.234.1rc0/covalent/_workflow/lepton.py` & `covalent-0.235.0rc0/covalent/_workflow/lepton.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/postprocessing.py` & `covalent-0.235.0rc0/covalent/_workflow/postprocessing.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/qdevice.py` & `covalent-0.235.0rc0/covalent/_workflow/qdevice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/qelectron.py` & `covalent-0.235.0rc0/covalent/_workflow/qelectron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/qnode.py` & `covalent-0.235.0rc0/covalent/_workflow/qnode.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/transport.py` & `covalent-0.235.0rc0/covalent/_workflow/transport.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/_workflow/transportable_object.py` & `covalent-0.235.0rc0/covalent/_workflow/transportable_object.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/cloud_resource_manager/__init__.py` & `covalent-0.235.0rc0/covalent/cloud_resource_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/cloud_resource_manager/core.py` & `covalent-0.235.0rc0/covalent/cloud_resource_manager/core.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/__init__.py` & `covalent-0.235.0rc0/covalent/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/base.py` & `covalent-0.235.0rc0/covalent/executor/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/executor_plugins/dask.py` & `covalent-0.235.0rc0/covalent/executor/executor_plugins/dask.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/executor_plugins/local.py` & `covalent-0.235.0rc0/covalent/executor/executor_plugins/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/executor_plugins/remote_executor.py` & `covalent-0.235.0rc0/covalent/executor/executor_plugins/remote_executor.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/qbase.py` & `covalent-0.235.0rc0/covalent/executor/qbase.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py` & `covalent-0.235.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/schemas.py` & `covalent-0.235.0rc0/covalent/executor/schemas.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/utils/__init__.py` & `covalent-0.235.0rc0/covalent/executor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/utils/context.py` & `covalent-0.235.0rc0/covalent/executor/utils/context.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/utils/enums.py` & `covalent-0.235.0rc0/covalent/executor/utils/enums.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/utils/serialize.py` & `covalent-0.235.0rc0/covalent/executor/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/executor/utils/wrappers.py` & `covalent-0.235.0rc0/covalent/executor/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/leptons/__init__.py` & `covalent-0.235.0rc0/covalent/leptons/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/__init__.py` & `covalent-0.235.0rc0/covalent/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qclient/__init__.py` & `covalent-0.235.0rc0/covalent/quantum/qclient/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qclient/base_client.py` & `covalent-0.235.0rc0/covalent/quantum/qclient/base_client.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qclient/core.py` & `covalent-0.235.0rc0/covalent/quantum/qclient/core.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qclient/local_client.py` & `covalent-0.235.0rc0/covalent/quantum/qclient/local_client.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qcluster/__init__.py` & `covalent-0.235.0rc0/covalent/quantum/qcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qcluster/base.py` & `covalent-0.235.0rc0/covalent/quantum/qcluster/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qcluster/clusters.py` & `covalent-0.235.0rc0/covalent/quantum/qcluster/clusters.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qcluster/default_selectors.py` & `covalent-0.235.0rc0/covalent/quantum/qcluster/default_selectors.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qcluster/simulator.py` & `covalent-0.235.0rc0/covalent/quantum/qcluster/simulator.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qserver/__init__.py` & `covalent-0.235.0rc0/covalent/quantum/qserver/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qserver/core.py` & `covalent-0.235.0rc0/covalent/quantum/qserver/core.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qserver/database.py` & `covalent-0.235.0rc0/covalent/quantum/qserver/database.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qserver/serialize.py` & `covalent-0.235.0rc0/covalent/quantum/qserver/serialize.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qserver/servers/__init__.py` & `covalent-0.235.0rc0/covalent/quantum/qserver/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qserver/servers/local.py` & `covalent-0.235.0rc0/covalent/quantum/qserver/servers/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/quantum/qserver/utils.py` & `covalent-0.235.0rc0/covalent/quantum/qserver/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/triggers/__init__.py` & `covalent-0.235.0rc0/covalent/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/triggers/base.py` & `covalent-0.235.0rc0/covalent/triggers/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/triggers/database_trigger.py` & `covalent-0.235.0rc0/covalent/triggers/database_trigger.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 # limitations under the License.
 
 import time
 from functools import partial
 from threading import Event
 from typing import List
 
-from sqlalchemy import create_engine
-from sqlalchemy.orm import Session
-
 from covalent._shared_files import logger
 
 from .base import BaseTrigger
 
 app_log = logger.app_log
 log_stack_info = logger.log_stack_info
 
@@ -84,14 +81,20 @@
 
     def observe(self) -> None:
         """
         Keep performing the trigger action as long as
         where conditions are met or until stop has being called
         """
 
+        # Since these modules are only used server-side, delay their
+        # imports to avoid introducing a sqlalchemy requirement to
+        # SDK-only installs
+        from sqlalchemy import create_engine
+        from sqlalchemy.orm import Session
+
         app_log.debug("Inside DatabaseTrigger's observe")
         event_count = 0
 
         try:
             self.engine = create_engine(self.db_path)
 
             with Session(self.engine) as db:
```

### Comparing `covalent-0.234.1rc0/covalent/triggers/dir_trigger.py` & `covalent-0.235.0rc0/covalent/triggers/dir_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/triggers/sqlite_trigger.py` & `covalent-0.235.0rc0/covalent/triggers/sqlite_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/triggers/time_trigger.py` & `covalent-0.235.0rc0/covalent/triggers/time_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent/triggers/trigger_loader.py` & `covalent-0.235.0rc0/covalent/triggers/trigger_loader.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent.egg-info/PKG-INFO` & `covalent-0.235.0rc0/covalent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent
-Version: 0.234.1rc0
+Version: 0.235.0rc0
 Summary: Covalent Workflow Tool
 Home-page: https://github.com/AgnostiqHQ/covalent
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: Apache License 2.0
-Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.234.1-rc.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.235.0-rc.0.tar.gz
 Description: <div align="center">
           <img src="./doc/source/_static/banner_executor.gif" alt="hero" />
         </div>
         </br>
         <div align="center">
         
         [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https://github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: covalent Version: 0.234.1rc0 Summary: Covalent
+Metadata-Version: 2.1 Name: covalent Version: 0.235.0rc0 Summary: Covalent
 Workflow Tool Home-page: https://github.com/AgnostiqHQ/covalent Author:
 Agnostiq Author-email: support@agnostiq.ai Maintainer: Agnostiq License: Apache
 License 2.0 Download-URL: https://github.com/AgnostiqHQ/covalent/archive/
-v0.234.1-rc.0.tar.gz Description:
+v0.235.0-rc.0.tar.gz Description:
                                     [hero]
           [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/
 covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https:
  //github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md) [![Static Badge]
   (https://img.shields.io/badge/python-3.8_%7C_3.9_%7C_3.10-%235552FF)](#) [!
           [Static Badge](https://img.shields.io/badge/tests-passing-
     %235552FF?logo=github)](https://github.com/AgnostiqHQ/covalent/actions/
```

### Comparing `covalent-0.234.1rc0/covalent.egg-info/SOURCES.txt` & `covalent-0.235.0rc0/covalent.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 covalent/triggers/sqlite_trigger.py
 covalent/triggers/time_trigger.py
 covalent/triggers/trigger_loader.py
 covalent_dispatcher/__init__.py
 covalent_dispatcher/entry_point.py
 covalent_dispatcher/_cli/__init__.py
 covalent_dispatcher/_cli/cli.py
-covalent_dispatcher/_cli/migrate.py
 covalent_dispatcher/_cli/service.py
 covalent_dispatcher/_cli/groups/__init__.py
 covalent_dispatcher/_cli/groups/db_group.py
 covalent_dispatcher/_cli/groups/deploy_group.py
 covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py
 covalent_dispatcher/_core/__init__.py
 covalent_dispatcher/_core/data_manager.py
```

### Comparing `covalent-0.234.1rc0/covalent.egg-info/requires.txt` & `covalent-0.235.0rc0/covalent.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 networkx>=2.8.6
 psutil>=5.9.0
 pydantic>=2.1.1
 python-multipart>=0.0.6
 python-socketio>=5.7.1
 requests>=2.24.0
 rich<=13.3.5,>=12.0.0
-simplejson>=3.17.6
 sqlalchemy<2.0.0,>=1.4.37
 sqlalchemy_utils>=0.38.3
 toml>=0.10.2
 typing-extensions>=4.8.0
-uvicorn[standard]==0.18.3
+uvicorn[standard]
 watchdog>=2.2.1
-werkzeug>=2.0.3
 
 [aws]
 boto3>=1.20.48
 
 [azure]
 azure-identity>=1.13.0
 azure-storage-blob>=12.16.0
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_cli/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_cli/cli.py` & `covalent-0.235.0rc0/covalent_dispatcher/_cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,15 @@
 from importlib import metadata
 from platform import machine, python_version, system
 
 import click
 from rich.console import Console
 
 from .groups import db, deploy
-from .service import (
-    cluster,
-    config,
-    logs,
-    migrate_legacy_result_object,
-    print_header,
-    purge,
-    restart,
-    start,
-    status,
-    stop,
-)
+from .service import cluster, config, logs, print_header, purge, restart, start, status, stop
 
 
 # Main entrypoint
 @click.group(invoke_without_command=True)
 @click.option("-v", "--version", is_flag=True, help="Display version information.")
 @click.pass_context
 def cli(ctx: click.Context, version: bool) -> None:
@@ -69,12 +58,11 @@
 cli.add_command(restart)
 cli.add_command(status)
 cli.add_command(purge)
 cli.add_command(logs)
 cli.add_command(cluster)
 cli.add_command(db)
 cli.add_command(config)
-cli.add_command(migrate_legacy_result_object)
 cli.add_command(deploy)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/db_group.py` & `covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/db_group.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group.py` & `covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/deploy_group.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py` & `covalent-0.235.0rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_cli/service.py` & `covalent-0.235.0rc0/covalent_dispatcher/_cli/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 from rich.table import Table
 from rich.text import Text
 from sqlalchemy import exc as sa_exc
 
 from covalent._shared_files.config import ConfigManager, get_config, reload_config, set_config
 
 from .._db.datastore import DataStore
-from .migrate import migrate_pickled_result_object
 
 UI_PIDFILE = get_config("dispatcher.cache_dir") + "/ui.pid"
 UI_LOGFILE = get_config("user_interface.log_dir") + "/covalent_ui.log"
 UI_SRVDIR = f"{os.path.dirname(os.path.abspath(__file__))}/../../covalent_ui"
 
 MIGRATION_WARNING_MSG = "Covalent not started. The database needs to be upgraded."
 MIGRATION_COMMAND_MSG = (
@@ -783,25 +782,14 @@
     else:
         console.print(
             f"{UI_LOGFILE} not found. Restart the server to create a new log file.",
             style="bold red",
         )
 
 
-@click.command()
-@click.argument("result_pickle_path")
-def migrate_legacy_result_object(result_pickle_path) -> None:
-    """Migrate a legacy result object
-
-    Example: `covalent migrate-legacy-result-object result.pkl`
-    """
-
-    migrate_pickled_result_object(result_pickle_path)
-
-
 # Cluster CLI handlers (client side wrappers for the async handlers exposed
 # in the dask cluster process)
 async def _get_cluster_status(uri: str):
     """
     Returns status of all workers and scheduler in the cluster
     """
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_manager.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/asset_manager.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/asset_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/dispatch.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/dispatch.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/electron.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/graph.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/graph.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/importer.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/importer.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/job_manager.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/job_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/lattice.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/utils.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/data_modules/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/store.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/dispatcher_modules/store.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/execution.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/execution.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/runner.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/runner.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/cancel.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/cancel.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/jobs.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/jobs.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/utils.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/runner_modules/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_ng.py` & `covalent-0.235.0rc0/covalent_dispatcher/_core/runner_ng.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/asset.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/asset.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/base.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/controller.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/controller.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,14 @@
     "workflow_function",
     "workflow_function_string",
     "transport_graph",
     "metadata",
     "name",
     "doc",
     "inputs",
-    "named_args",
-    "named_kwargs",
-    "cova_imports",
-    "lattice_imports",
 }
 
 METADATA_KEYS = lattice.LATTICE_METADATA_KEYS.copy()
 METADATA_KEYS.remove("__name__")
 METADATA_KEYS.add("name")
 
 ASSET_KEYS = lattice.LATTICE_ASSET_KEYS.copy()
@@ -64,18 +60,14 @@
 
 # Obsoleted by LatticeAsset table
 _asset_record_map = {
     "workflow_function": "function_filename",
     "workflow_function_string": "function_string_filename",
     "doc": "docstring_filename",
     "inputs": "inputs_filename",
-    "named_args": "named_args_filename",
-    "named_kwargs": "named_kwargs_filename",
-    "cova_imports": "cova_imports_filename",
-    "lattice_imports": "lattice_imports_filename",
     "executor_data": "executor_data_filename",
     "workflow_executor_data": "workflow_executor_data_filename",
     "hooks": "hooks_filename",
 }
 
 
 def get_executor_data_filter(raw: str):
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/edge.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/edge.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/electron.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/electron.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/lattice.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/result.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/tg.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/exporters/tg.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/electron.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 
     """
 
     # Maps asset keys to asset records
     asset_recs = {}
 
     for asset_key, asset in e.assets:
+        # Register these later
+        if asset_key == "_custom":
+            continue
+
         node_storage_path, object_key = object_store.get_uri_components(
             dispatch_id,
             e.id,
             asset_key,
         )
 
         object_key = ASSET_FILENAME_MAP[asset_key]
@@ -153,16 +157,16 @@
         asset_recs[asset_key] = Asset.create(session, insert_kwargs=asset_kwargs, flush=False)
 
         # Send this back to the client
         asset.digest = None
         asset.remote_uri = f"file://{local_uri}"
 
     # Register custom assets
-    if e.custom_assets:
-        for asset_key, asset in e.custom_assets.items():
+    if e.assets._custom:
+        for asset_key, asset in e.assets._custom.items():
             object_key = f"{asset_key}.data"
             local_uri = os.path.join(node_storage_path, object_key)
 
             asset_kwargs = {
                 "storage_type": object_store.scheme,
                 "storage_path": node_storage_path,
                 "object_key": object_key,
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/lattice.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/lattice.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,20 @@
 import json
 import os
 
 from sqlalchemy.orm import Session
 
 from covalent._shared_files.config import get_config
 from covalent._shared_files.schemas.lattice import (
-    LATTICE_COVA_IMPORTS_FILENAME,
     LATTICE_DOCSTRING_FILENAME,
     LATTICE_ERROR_FILENAME,
     LATTICE_FUNCTION_FILENAME,
     LATTICE_FUNCTION_STRING_FILENAME,
     LATTICE_HOOKS_FILENAME,
     LATTICE_INPUTS_FILENAME,
-    LATTICE_LATTICE_IMPORTS_FILENAME,
-    LATTICE_NAMED_ARGS_FILENAME,
-    LATTICE_NAMED_KWARGS_FILENAME,
     LATTICE_RESULTS_FILENAME,
     LATTICE_STORAGE_TYPE,
     LatticeAssets,
     LatticeSchema,
 )
 from covalent_dispatcher._dal.asset import Asset
 from covalent_dispatcher._dal.lattice import Lattice
@@ -67,20 +63,16 @@
 
     legacy_kwargs = {
         "docstring_filename": LATTICE_DOCSTRING_FILENAME,
         "function_filename": LATTICE_FUNCTION_FILENAME,
         "function_string_filename": LATTICE_FUNCTION_STRING_FILENAME,
         "error_filename": LATTICE_ERROR_FILENAME,
         "inputs_filename": LATTICE_INPUTS_FILENAME,
-        "named_args_filename": LATTICE_NAMED_ARGS_FILENAME,
-        "named_kwargs_filename": LATTICE_NAMED_KWARGS_FILENAME,
         "results_filename": LATTICE_RESULTS_FILENAME,
         "hooks_filename": LATTICE_HOOKS_FILENAME,
-        "cova_imports_filename": LATTICE_COVA_IMPORTS_FILENAME,
-        "lattice_imports_filename": LATTICE_LATTICE_IMPORTS_FILENAME,
     }
     kwargs.update(legacy_kwargs)
     return kwargs
 
 
 def import_lattice_assets(
     session: Session,
@@ -90,14 +82,18 @@
     object_store: BaseProvider,
 ) -> LatticeAssets:
     """Insert asset records and populate the asset link table"""
     asset_ids = {}
 
     # Register built-in assets
     for asset_key, asset in lat.assets:
+        # Deal with these later
+        if asset_key == "_custom":
+            continue
+
         storage_path, object_key = object_store.get_uri_components(
             dispatch_id=dispatch_id,
             node_id=None,
             asset_key=asset_key,
         )
 
         local_uri = os.path.join(storage_path, object_key)
@@ -114,16 +110,16 @@
         asset_ids[asset_key] = Asset.create(session, insert_kwargs=asset_kwargs, flush=False)
 
         # Send this back to the client
         asset.digest = None
         asset.remote_uri = f"file://{local_uri}"
 
     # Register custom assets
-    if lat.custom_assets:
-        for asset_key, asset in lat.custom_assets.items():
+    if lat.assets._custom:
+        for asset_key, asset in lat.assets._custom.items():
             object_key = f"{asset_key}.data"
             local_uri = os.path.join(storage_path, object_key)
 
             asset_kwargs = {
                 "storage_type": object_store.scheme,
                 "storage_path": storage_path,
                 "object_key": object_key,
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/result.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/tg.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/importers/tg.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/job.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/job.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/lattice.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/result.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/tg.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/tg.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/tg_ops.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/tg_ops.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/file_transfer.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/utils/file_transfer.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/uri_filters.py` & `covalent-0.235.0rc0/covalent_dispatcher/_dal/utils/uri_filters.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/datastore.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/datastore.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/dispatchdb.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/dispatchdb.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 """Dispatch DataBase script."""
 
 import copy
 from datetime import datetime
 
 import networkx as nx
-import simplejson
 
 import covalent.executor as covalent_executor
 from covalent._shared_files import logger
 from covalent._shared_files.config import get_config
 from covalent._shared_files.util_classes import Status
 
 app_log = logger.app_log
@@ -121,46 +120,14 @@
     if isinstance(obj, Status):
         return obj.STATUS
     if isinstance(obj, datetime):
         return obj.isoformat()
     return str(obj)
 
 
-def encode_result(result_obj):
-    lattice = result_obj.lattice
-
-    result_string = result_obj.encoded_result.json
-    if not result_string:
-        result_string = result_obj.encoded_result.object_string
-
-    named_args = {k: v.object_string for k, v in lattice.named_args.items()}
-    named_kwargs = {k: v.object_string for k, v in lattice.named_kwargs.items()}
-    result_dict = {
-        "dispatch_id": result_obj.dispatch_id,
-        "status": result_obj.status,
-        "result": result_string,
-        "start_time": result_obj.start_time,
-        "end_time": result_obj.end_time,
-        "results_dir": result_obj.results_dir,
-        "error": result_obj.error,
-        "lattice": {
-            "function_string": lattice.workflow_function_string,
-            "doc": lattice.__doc__,
-            "name": lattice.__name__,
-            "inputs": encode_dict({**named_args, **named_kwargs}),
-            "metadata": extract_metadata(lattice.metadata),
-        },
-        "graph": extract_graph(result_obj.lattice.transport_graph._graph),
-    }
-
-    jsonified_result = simplejson.dumps(result_dict, default=result_encoder, ignore_nan=True)
-
-    return jsonified_result
-
-
 class DispatchDB:
     """
     Wrapper for the database of workflows.
     """
 
     def __init__(self, dbpath: str = None) -> None:
         if dbpath:
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/jobdb.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/jobdb.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/models.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,30 +88,30 @@
 
     # Name of the file containing an error message for the workflow
     error_filename = Column(Text)
 
     # Name of the file containing the serialized input data
     inputs_filename = Column(Text)
 
-    # Name of the file containing the serialized named args
+    # DEPRECATED: Name of the file containing the serialized named args
     named_args_filename = Column(Text)
 
-    # Name of the file containing the serialized named kwargs
+    # DEPRECATED: Name of the file containing the serialized named kwargs
     named_kwargs_filename = Column(Text)
 
     # name of the file containing the serialized output
     results_filename = Column(Text)
 
     # Name of the file containing the default electron hooks
     hooks_filename = Column(Text)
 
-    # Name of the file containing the set of cova imports
+    # DEPRECATED: Name of the file containing the set of cova imports
     cova_imports_filename = Column(Text)
 
-    # Name of the file containing the set of lattice imports
+    # DEPRECATED: Name of the file containing the set of lattice imports
     lattice_imports_filename = Column(Text)
 
     # Results directory (will be deprecated soon)
     results_dir = Column(Text)
 
     # Dispatch id of the root lattice in a hierarchy of sublattices
     root_dispatch_id = Column(String(64), nullable=True)
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/update.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/update.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/upsert.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/upsert.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,20 +53,16 @@
 ELECTRON_HOOKS_FILENAME = ELECTRON_FILENAMES["hooks"]
 ELECTRON_STORAGE_TYPE = "file"
 LATTICE_FUNCTION_FILENAME = LATTICE_FILENAMES["workflow_function"]
 LATTICE_FUNCTION_STRING_FILENAME = LATTICE_FILENAMES["workflow_function_string"]
 LATTICE_DOCSTRING_FILENAME = LATTICE_FILENAMES["doc"]
 LATTICE_ERROR_FILENAME = LATTICE_FILENAMES["error"]
 LATTICE_INPUTS_FILENAME = LATTICE_FILENAMES["inputs"]
-LATTICE_NAMED_ARGS_FILENAME = LATTICE_FILENAMES["named_args"]
-LATTICE_NAMED_KWARGS_FILENAME = LATTICE_FILENAMES["named_kwargs"]
 LATTICE_RESULTS_FILENAME = LATTICE_FILENAMES["result"]
 LATTICE_HOOKS_FILENAME = LATTICE_FILENAMES["hooks"]
-LATTICE_COVA_IMPORTS_FILENAME = LATTICE_FILENAMES["cova_imports"]
-LATTICE_LATTICE_IMPORTS_FILENAME = LATTICE_FILENAMES["lattice_imports"]
 LATTICE_STORAGE_TYPE = "file"
 
 CUSTOM_ASSETS_FIELD = "custom_asset_keys"
 
 
 def _lattice_data(session: Session, result: Result, electron_id: int = None) -> int:
     """
@@ -104,20 +100,16 @@
 
     for key, filename, data in [
         ("workflow_function", LATTICE_FUNCTION_FILENAME, result.lattice.workflow_function),
         ("workflow_function_string", LATTICE_FUNCTION_STRING_FILENAME, workflow_func_string),
         ("doc", LATTICE_DOCSTRING_FILENAME, result.lattice.__doc__),
         ("error", LATTICE_ERROR_FILENAME, result.error),
         ("inputs", LATTICE_INPUTS_FILENAME, result.lattice.inputs),
-        ("named_args", LATTICE_NAMED_ARGS_FILENAME, result.lattice.named_args),
-        ("named_kwargs", LATTICE_NAMED_KWARGS_FILENAME, result.lattice.named_kwargs),
         ("result", LATTICE_RESULTS_FILENAME, result._result),
         ("hooks", LATTICE_HOOKS_FILENAME, result.lattice.metadata["hooks"]),
-        ("cova_imports", LATTICE_COVA_IMPORTS_FILENAME, result.lattice.cova_imports),
-        ("lattice_imports", LATTICE_LATTICE_IMPORTS_FILENAME, result.lattice.lattice_imports),
     ]:
         digest, size = local_store.store_file(data_storage_path, filename, data)
         asset_record_kwargs = {
             "storage_type": LATTICE_STORAGE_TYPE,
             "storage_path": str(data_storage_path),
             "object_key": filename,
             "digest_alg": digest.algorithm,
@@ -157,20 +149,16 @@
         "function_string_filename": LATTICE_FUNCTION_STRING_FILENAME,
         "executor": result.lattice.metadata["executor"],
         "executor_data": json.dumps(result.lattice.metadata["executor_data"]),
         "workflow_executor": result.lattice.metadata["workflow_executor"],
         "workflow_executor_data": json.dumps(result.lattice.metadata["workflow_executor_data"]),
         "error_filename": LATTICE_ERROR_FILENAME,
         "inputs_filename": LATTICE_INPUTS_FILENAME,
-        "named_args_filename": LATTICE_NAMED_ARGS_FILENAME,
-        "named_kwargs_filename": LATTICE_NAMED_KWARGS_FILENAME,
         "results_filename": LATTICE_RESULTS_FILENAME,
         "hooks_filename": LATTICE_HOOKS_FILENAME,
-        "cova_imports_filename": LATTICE_COVA_IMPORTS_FILENAME,
-        "lattice_imports_filename": LATTICE_LATTICE_IMPORTS_FILENAME,
         "results_dir": results_dir,
         "root_dispatch_id": result.root_dispatch_id,
         "python_version": result.lattice.python_version,
         "covalent_version": result.lattice.covalent_version,
         "created_at": datetime.now(timezone.utc),
         "updated_at": datetime.now(timezone.utc),
         "started_at": result.start_time,
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_db/write_result_to_db.py` & `covalent-0.235.0rc0/covalent_dispatcher/_db/write_result_to_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,20 +91,16 @@
     function_string_filename: str,
     executor: str,
     executor_data: str,
     workflow_executor: str,
     workflow_executor_data: str,
     error_filename: str,
     inputs_filename: str,
-    named_args_filename: str,
-    named_kwargs_filename: str,
     results_filename: str,
     hooks_filename: str,
-    cova_imports_filename: str,
-    lattice_imports_filename: str,
     results_dir: str,
     root_dispatch_id: str,
     created_at: dt,
     updated_at: dt,
     started_at: dt,
     completed_at: dt,
 ) -> int:
@@ -129,20 +125,16 @@
         function_string_filename=function_string_filename,
         executor=executor,
         executor_data=executor_data,
         workflow_executor=workflow_executor,
         workflow_executor_data=workflow_executor_data,
         error_filename=error_filename,
         inputs_filename=inputs_filename,
-        named_args_filename=named_args_filename,
-        named_kwargs_filename=named_kwargs_filename,
         results_filename=results_filename,
         hooks_filename=hooks_filename,
-        cova_imports_filename=cova_imports_filename,
-        lattice_imports_filename=lattice_imports_filename,
         results_dir=results_dir,
         root_dispatch_id=root_dispatch_id,
         is_active=True,
         created_at=created_at,
         updated_at=updated_at,
         started_at=started_at,
         completed_at=completed_at,
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_object_store/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_object_store/base.py` & `covalent-0.235.0rc0/covalent_dispatcher/_object_store/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_object_store/local.py` & `covalent-0.235.0rc0/covalent_dispatcher/_object_store/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_service/app.py` & `covalent-0.235.0rc0/covalent_dispatcher/_service/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         app_log.debug(f"Exception in register: {e}")
         raise HTTPException(
             status_code=400,
             detail=f"Failed to submit workflow: {e}",
         ) from e
 
 
-@router.post("/dispatches/{dispatch_id}/subdispatches", status_code=201)
+@router.post("/dispatches/{dispatch_id}/sublattices", status_code=201)
 async def register_subdispatch(
     manifest: ResultSchema,
     dispatch_id: str,
 ) -> ResultSchema:
     """Register a subdispatch in the database.
 
     Args:
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_service/app_dask.py` & `covalent-0.235.0rc0/covalent_dispatcher/_service/app_dask.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_service/assets.py` & `covalent-0.235.0rc0/covalent_dispatcher/_service/assets.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_service/heartbeat.py` & `covalent-0.235.0rc0/covalent_dispatcher/_service/heartbeat.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_service/models.py` & `covalent-0.235.0rc0/covalent_dispatcher/_service/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,15 @@
 
 
 class LatticeAssetKey(str, Enum):
     workflow_function = "workflow_function"
     workflow_function_string = "workflow_function_string"
     doc = "doc"
     inputs = "inputs"
-    named_args = "named_args"
-    named_kwargs = "named_kwargs"
     hooks = "hooks"
-    cova_imports = "cova_imports"
-    lattice_imports = "lattice_imports"
 
 
 class ElectronAssetKey(str, Enum):
     function = "function"
     function_string = "function_string"
     output = "output"
     value = "value"
```

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_service/runnersvc.py` & `covalent-0.235.0rc0/covalent_dispatcher/_service/runnersvc.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/__init__.py` & `covalent-0.235.0rc0/covalent_dispatcher/_triggers_app/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/app.py` & `covalent-0.235.0rc0/covalent_dispatcher/_triggers_app/app.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_dispatcher/entry_point.py` & `covalent-0.235.0rc0/covalent_dispatcher/entry_point.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/README.md` & `covalent-0.235.0rc0/covalent_migrations/README.md`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/alembic.ini` & `covalent-0.235.0rc0/covalent_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/env.py` & `covalent-0.235.0rc0/covalent_migrations/env.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/script.py.mako` & `covalent-0.235.0rc0/covalent_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py` & `covalent-0.235.0rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/26d71848a404_v12.py` & `covalent-0.235.0rc0/covalent_migrations/versions/26d71848a404_v12.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py` & `covalent-0.235.0rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/97202f5f47cb_v13.py` & `covalent-0.235.0rc0/covalent_migrations/versions/97202f5f47cb_v13.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/9b9d58f02985_v11.py` & `covalent-0.235.0rc0/covalent_migrations/versions/9b9d58f02985_v11.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/b60c5ecdf927_init.py` & `covalent-0.235.0rc0/covalent_migrations/versions/b60c5ecdf927_init.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py` & `covalent-0.235.0rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py` & `covalent-0.235.0rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/main.py` & `covalent-0.235.0rc0/covalent_ui/api/main.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/electron_dal.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/electron_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/graph_dal.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/graph_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/lattice_dal.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/lattice_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/logs_dal.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/logs_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/summary_dal.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/data_layer/summary_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/database/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/database/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/database/config/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/database/config/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/database/config/db.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/database/config/db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron_dependency.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/electron_dependency.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/lattices.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/database/schema/lattices.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/models/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/models/dispatch_model.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/models/dispatch_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/models/electrons_model.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/models/electrons_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/models/graph_model.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/models/graph_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/models/lattices_model.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/models/lattices_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/models/logs_model.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/models/logs_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/models/settings_model.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/models/settings_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/graph_route.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/graph_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/logs_route.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/logs_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/routes/routes.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/routes/routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/utils/__init__.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/utils/file_handle.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/utils/file_handle.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/utils/log_handler.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/utils/log_handler.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/utils/models_helper.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/utils/models_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/api/v1/utils/status.py` & `covalent-0.235.0rc0/covalent_ui/api/v1/utils/status.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/app.py` & `covalent-0.235.0rc0/covalent_ui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,11 +129,10 @@
         tr_app.disable_triggers = True
 
     # Start covalent main app
     uvicorn.run(
         app_name,
         host=host,
         port=port,
-        debug=DEBUG,
         reload=RELOAD,
         log_config=log_config(),
     )
```

### Comparing `covalent-0.234.1rc0/covalent_ui/result_webhook.py` & `covalent-0.235.0rc0/covalent_ui/result_webhook.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import aiohttp
 import requests
 
 import covalent_ui.app as ui_server
 from covalent._results_manager import Result
 from covalent._shared_files import logger
-from covalent._shared_files.utils import get_ui_url
+from covalent._shared_files.utils import get_named_params, get_ui_url
 from covalent_dispatcher._db.dispatchdb import encode_dict, extract_graph, extract_metadata
 
 app_log = logger.app_log
 
 # UI server webhook for result updates
 
 
@@ -74,16 +74,19 @@
     Args: lattice: The lattice to draw with a pre-built graph.
 
     Returns: None
     """
 
     graph = lattice.transport_graph.get_internal_graph_copy()
 
-    named_args = lattice.named_args.get_deserialized()
-    named_kwargs = lattice.named_kwargs.get_deserialized()
+    inputs = lattice.inputs.get_deserialized()
+    fn = lattice.workflow_function.get_deserialized()
+    args = inputs["args"]
+    kwargs = inputs["kwargs"]
+    named_args, named_kwargs = get_named_params(fn, args, kwargs)
 
     draw_request = json.dumps(
         {
             "event": "draw-request",
             "payload": {
                 "lattice": {
                     "function_string": lattice.workflow_function_string,
```

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/asset-manifest.json` & `covalent-0.235.0rc0/covalent_ui/webapp/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/favicon.ico` & `covalent-0.235.0rc0/covalent_ui/webapp/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/favicon64x64.ico` & `covalent-0.235.0rc0/covalent_ui/webapp/build/favicon64x64.ico`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/index.html` & `covalent-0.235.0rc0/covalent_ui/webapp/build/index.html`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/logo192x192.png` & `covalent-0.235.0rc0/covalent_ui/webapp/build/logo192x192.png`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/logo512x512.png` & `covalent-0.235.0rc0/covalent_ui/webapp/build/logo512x512.png`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/logo64x64.png` & `covalent-0.235.0rc0/covalent_ui/webapp/build/logo64x64.png`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg` & `covalent-0.235.0rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/pyproject.toml` & `covalent-0.235.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-0.234.1rc0/setup.py` & `covalent-0.235.0rc0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 from setuptools.command.egg_info import egg_info, manifest_maker
 
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
 
 with open("VERSION") as f:
     version = f.read().strip()
 
+# Allow installing a particular commit for testing
+commit_sha = os.getenv("COVALENT_COMMIT_SHA")
+artifact_id = commit_sha if commit_sha else f"v{version}"
 
 requirements_file = "requirements.txt"
 exclude_modules = [
     "tests",
     "tests.*",
 ]
 sdk_only = os.environ.get("COVALENT_SDK_ONLY") == "1"
@@ -198,15 +201,15 @@
 
 setup_info = {
     "name": "covalent",
     "packages": find_packages(exclude=exclude_modules),
     "version": version,
     "maintainer": "Agnostiq",
     "url": "https://github.com/AgnostiqHQ/covalent",
-    "download_url": f"https://github.com/AgnostiqHQ/covalent/archive/v{version}.tar.gz",
+    "download_url": f"https://github.com/AgnostiqHQ/covalent/archive/{artifact_id}.tar.gz",
     "license": "Apache License 2.0",
     "author": "Agnostiq",
     "author_email": "support@agnostiq.ai",
     "description": "Covalent Workflow Tool",
     "long_description": open("README.md", encoding="utf-8").read(),
     "long_description_content_type": "text/markdown",
     "include_package_data": True,
```

