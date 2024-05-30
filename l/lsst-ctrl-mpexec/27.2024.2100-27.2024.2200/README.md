# Comparing `tmp/lsst_ctrl_mpexec-27.2024.2100.tar.gz` & `tmp/lsst_ctrl_mpexec-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_ctrl_mpexec-27.2024.2100.tar", last modified: Thu May 23 10:11:15 2024, max compression
+gzip compressed data, was "lsst_ctrl_mpexec-27.2024.2200.tar", last modified: Thu May 30 09:58:41 2024, max compression
```

## Comparing `lsst_ctrl_mpexec-27.2024.2100.tar` & `lsst_ctrl_mpexec-27.2024.2200.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.094293 lsst_ctrl_mpexec-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-23 10:11:15.090293 lsst_ctrl_mpexec-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.078292 lsst_ctrl_mpexec-27.2024.2100/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.078292 lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/pipetask.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.078292 lsst_ctrl_mpexec-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.078292 lsst_ctrl_mpexec-27.2024.2100/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.082293 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.082293 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.086293 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.086293 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.086293 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    19210 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/pipetask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.086293 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/confirmable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/run_qbb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    41717 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cmdLineFwk.py
--rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/dotTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/execFixupDataId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/executionGraphFixup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    27923 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/mpGraphExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19881 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/preExecInit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/quantumGraphExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/separablePipelineExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16065 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/showInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/simple_pipeline_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    25906 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/singleQuantumExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/taskFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:11:14.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.090293 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-23 10:11:15.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-23 10:11:15.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:11:15.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 10:11:15.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 10:11:15.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:11:15.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:11:14.000000 lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-23 10:11:15.094293 lsst_ctrl_mpexec-27.2024.2100/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:11:15.090293 lsst_ctrl_mpexec-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdCleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdPurge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdQgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdUpdateGraphRun.py
--rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cliScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cliUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46363 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_cmdLineFwk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_dotTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    31497 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_preExecInit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_separablePipelineExecutor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_simple_pipeline_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-23 10:11:05.000000 lsst_ctrl_mpexec-27.2024.2100/tests/test_taskFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.384482 lsst_ctrl_mpexec-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-30 09:58:41.384482 lsst_ctrl_mpexec-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.368482 lsst_ctrl_mpexec-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.372482 lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/pipetask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.368482 lsst_ctrl_mpexec-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.372482 lsst_ctrl_mpexec-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.372482 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.376482 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.376482 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.376482 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.376482 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19210 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/pipetask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.380482 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/confirmable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/run_qbb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41717 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cmdLineFwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/dotTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/execFixupDataId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/executionGraphFixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27923 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/mpGraphExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19881 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/preExecInit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/quantumGraphExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/separablePipelineExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16065 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/showInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17269 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/simple_pipeline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25906 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/singleQuantumExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/taskFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:58:41.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.384482 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-30 09:58:41.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-30 09:58:41.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:58:41.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 09:58:41.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 09:58:41.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:58:41.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:58:40.000000 lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 09:58:41.384482 lsst_ctrl_mpexec-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:58:41.384482 lsst_ctrl_mpexec-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdCleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdPurge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdQgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdUpdateGraphRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7178 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cliScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46363 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_cmdLineFwk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_dotTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31497 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_preExecInit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_separablePipelineExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_simple_pipeline_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-30 09:58:35.000000 lsst_ctrl_mpexec-27.2024.2200/tests/test_taskFactory.py
```

### Comparing `lsst_ctrl_mpexec-27.2024.2100/PKG-INFO` & `lsst_ctrl_mpexec-27.2024.2200/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-mpexec
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: Pipeline execution infrastructure for the Rubin Observatory LSST Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_mpexec
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_mpexec-27.2024.2100/README.rst` & `lsst_ctrl_mpexec-27.2024.2200/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/bsd_license.txt` & `lsst_ctrl_mpexec-27.2024.2200/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/CHANGES.rst` & `lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst` & `lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/configuring-pipetask-tasks.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/doc/lsst.ctrl.mpexec/index.rst` & `lsst_ctrl_mpexec-27.2024.2200/doc/lsst.ctrl.mpexec/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/gpl-v3.0.txt` & `lsst_ctrl_mpexec-27.2024.2200/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/pyproject.toml` & `lsst_ctrl_mpexec-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/__init__.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/__init__.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/__init__.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/__init__.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/cmd/__init__.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/cmd/commands.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/__init__.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/arguments.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/optionGroups.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/opt/options.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/pipetask.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/pipetask.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/__init__.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/build.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/build.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/cleanup.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/cleanup.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/confirmable.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/confirmable.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/pre_exec_init_qbb.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/purge.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/purge.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/qgraph.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/qgraph.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/report.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/report.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/run.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/run.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/run_qbb.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/run_qbb.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/script/update_graph_run.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cli/utils.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/cmdLineFwk.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/cmdLineFwk.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/dotTools.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/dotTools.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/execFixupDataId.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/execFixupDataId.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/executionGraphFixup.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/executionGraphFixup.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/log_capture.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/log_capture.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/mpGraphExecutor.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/mpGraphExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/preExecInit.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/preExecInit.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/quantumGraphExecutor.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/quantumGraphExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/reports.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/reports.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/separablePipelineExecutor.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/separablePipelineExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/showInfo.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/showInfo.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/simple_pipeline_executor.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/simple_pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/singleQuantumExecutor.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/singleQuantumExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/taskFactory.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/taskFactory.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst/ctrl/mpexec/util.py` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst/ctrl/mpexec/util.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/PKG-INFO` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-mpexec
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: Pipeline execution infrastructure for the Rubin Observatory LSST Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_mpexec
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_mpexec-27.2024.2100/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt` & `lsst_ctrl_mpexec-27.2024.2200/python/lsst_ctrl_mpexec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdCleanup.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdCleanup.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdPurge.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdPurge.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdQgraph.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdQgraph.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdReport.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdReport.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cliCmdUpdateGraphRun.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cliCmdUpdateGraphRun.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cliScript.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cliScript.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cliUtils.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cliUtils.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_cmdLineFwk.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_cmdLineFwk.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_dotTools.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_dotTools.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_executors.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_executors.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_preExecInit.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_preExecInit.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_reports.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_separablePipelineExecutor.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_separablePipelineExecutor.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_simple_pipeline_executor.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_simple_pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_mpexec-27.2024.2100/tests/test_taskFactory.py` & `lsst_ctrl_mpexec-27.2024.2200/tests/test_taskFactory.py`

 * *Files identical despite different names*

