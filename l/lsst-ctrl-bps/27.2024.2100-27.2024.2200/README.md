# Comparing `tmp/lsst_ctrl_bps-27.2024.2100.tar.gz` & `tmp/lsst_ctrl_bps-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_ctrl_bps-27.2024.2100.tar", last modified: Thu May 23 10:08:51 2024, max compression
+gzip compressed data, was "lsst_ctrl_bps-27.2024.2200.tar", last modified: Thu May 30 09:56:25 2024, max compression
```

## Comparing `lsst_ctrl_bps-27.2024.2100.tar` & `lsst_ctrl_bps-27.2024.2200.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.951941 lsst_ctrl_bps-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 10:08:51.951941 lsst_ctrl_bps-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.935941 lsst_ctrl_bps-27.2024.2100/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.939941 lsst_ctrl_bps-27.2024.2100/doc/lsst.ctrl.bps/
--rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/doc/lsst.ctrl.bps/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/doc/lsst.ctrl.bps/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    49121 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/doc/lsst.ctrl.bps/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.939941 lsst_ctrl_bps-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.939941 lsst_ctrl_bps-27.2024.2100/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.939941 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.943941 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.943941 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/bps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.943941 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.947941 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/option_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/clustered_quantum_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22623 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.947941 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/etc/bps_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/etc/bps_eb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30486 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/generic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/pre_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/quantum_clustering_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)    42853 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/wms_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.951941 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:08:51.000000 lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-23 10:08:51.951941 lsst_ctrl_bps-27.2024.2100/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:51.947941 lsst_ctrl_bps-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_bps_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_bpsconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_clustered_quantum_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_generic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_pre_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_quantum_clustering_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-23 10:08:45.000000 lsst_ctrl_bps-27.2024.2100/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.293789 lsst_ctrl_bps-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 09:56:25.293789 lsst_ctrl_bps-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.277789 lsst_ctrl_bps-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.281789 lsst_ctrl_bps-27.2024.2200/doc/lsst.ctrl.bps/
+-rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/doc/lsst.ctrl.bps/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/doc/lsst.ctrl.bps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    49121 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/doc/lsst.ctrl.bps/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.281789 lsst_ctrl_bps-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.281789 lsst_ctrl_bps-27.2024.2200/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.281789 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.285789 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.285789 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/bps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.289789 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.289789 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/clustered_quantum_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22623 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.289789 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/etc/bps_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/etc/bps_eb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30486 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/generic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/pre_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/quantum_clustering_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42853 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:56:25.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/wms_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.293789 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 09:56:25.000000 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-30 09:56:25.000000 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:25.000000 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 09:56:25.000000 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 09:56:25.000000 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:56:25.000000 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:24.000000 lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 09:56:25.293789 lsst_ctrl_bps-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:25.293789 lsst_ctrl_bps-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_bps_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_bpsconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_clustered_quantum_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_generic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_pre_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_quantum_clustering_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-30 09:56:19.000000 lsst_ctrl_bps-27.2024.2200/tests/test_transform.py
```

### Comparing `lsst_ctrl_bps-27.2024.2100/PKG-INFO` & `lsst_ctrl_bps-27.2024.2200/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: Pluggable execution of workflow graphs from Rubin pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps-27.2024.2100/README.md` & `lsst_ctrl_bps-27.2024.2200/README.md`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/bsd_license.txt` & `lsst_ctrl_bps-27.2024.2200/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/doc/lsst.ctrl.bps/CHANGES.rst` & `lsst_ctrl_bps-27.2024.2200/doc/lsst.ctrl.bps/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/doc/lsst.ctrl.bps/index.rst` & `lsst_ctrl_bps-27.2024.2200/doc/lsst.ctrl.bps/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/doc/lsst.ctrl.bps/quickstart.rst` & `lsst_ctrl_bps-27.2024.2200/doc/lsst.ctrl.bps/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/gpl-v3.0.txt` & `lsst_ctrl_bps-27.2024.2200/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/pyproject.toml` & `lsst_ctrl_bps-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/__init__.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/__init__.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/__init__.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_config.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_config.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_draw.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_draw.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_reports.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_reports.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/bps_utils.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/bps_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cancel.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cancel.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/bps.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/bps.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/cmd/__init__.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/cmd/commands.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/__init__.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/arguments.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/option_groups.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/option_groups.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/cli/opt/options.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/clustered_quantum_graph.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/clustered_quantum_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/constants.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/constants.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/drivers.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/drivers.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/etc/bps_defaults.yaml` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/etc/bps_defaults.yaml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/etc/bps_eb.yaml` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/etc/bps_eb.yaml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/generic_workflow.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/generic_workflow.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/ping.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/ping.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/pre_transform.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/pre_transform.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/prepare.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/prepare.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/quantum_clustering_funcs.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/quantum_clustering_funcs.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/report.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/report.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/restart.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/restart.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/submit.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/submit.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/transform.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/transform.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst/ctrl/bps/wms_service.py` & `lsst_ctrl_bps-27.2024.2200/python/lsst/ctrl/bps/wms_service.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/PKG-INFO` & `lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: Pluggable execution of workflow graphs from Rubin pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps-27.2024.2100/python/lsst_ctrl_bps.egg-info/SOURCES.txt` & `lsst_ctrl_bps-27.2024.2200/python/lsst_ctrl_bps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_bps_utils.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_bps_utils.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_bpsconfig.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_bpsconfig.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_cli_commands.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_clustered_quantum_graph.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_clustered_quantum_graph.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_drivers.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_generic_workflow.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_generic_workflow.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_ping.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_pre_transform.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_pre_transform.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_quantum_clustering_funcs.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_quantum_clustering_funcs.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_report.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps-27.2024.2100/tests/test_transform.py` & `lsst_ctrl_bps-27.2024.2200/tests/test_transform.py`

 * *Files identical despite different names*

