# Comparing `tmp/binsync-4.1.8.tar.gz` & `tmp/binsync-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binsync-4.1.8.tar", last modified: Tue May 14 16:11:33 2024, max compression
+gzip compressed data, was "binsync-4.1.9.tar", last modified: Wed May 15 18:52:37 2024, max compression
```

## Comparing `binsync-4.1.8.tar` & `binsync-4.1.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.932966 binsync-4.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-14 16:11:29.000000 binsync-4.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 16:11:29.000000 binsync-4.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-05-14 16:11:33.932966 binsync-4.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-14 16:11:29.000000 binsync-4.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.920966 binsync-4.1.8/binsync/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/binsync_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    34776 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.924966 binsync-4.1.8/binsync/core/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/core/cache.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27287 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/core/scheduler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20405 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.924966 binsync-4.1.8/binsync/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.924966 binsync-4.1.8/binsync/interface_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/interface_overrides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/interface_overrides/angr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/interface_overrides/binja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/interface_overrides/ghidra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/interface_overrides/ida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/loggercfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.924966 binsync-4.1.8/binsync/stub_files/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/stub_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.924966 binsync-4.1.8/binsync/stub_files/angr_files/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/stub_files/angr_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/stub_files/angr_files/plugin.toml
--rw-r--r--   0 runner    (1001) docker     (127)    22965 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/stub_files/binsync_binja_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/stub_files/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.928966 binsync-4.1.8/binsync/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19696 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/config_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/control_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.928966 binsync-4.1.8/binsync/ui/force_push/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/force_push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/force_push/force_push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.928966 binsync-4.1.8/binsync/ui/force_push/panels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/force_push/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/force_push/panels/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/force_push/panels/globals_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/force_push/panels/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/magic_sync_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.928966 binsync-4.1.8/binsync/ui/panel_tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/panel_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/panel_tabs/activity_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/panel_tabs/ctx_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/panel_tabs/functions_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/panel_tabs/globals_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/panel_tabs/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/panel_tabs/util_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-14 16:11:29.000000 binsync-4.1.8/binsync/ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.928966 binsync-4.1.8/binsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-05-14 16:11:33.000000 binsync-4.1.8/binsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-14 16:11:33.000000 binsync-4.1.8/binsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:11:33.000000 binsync-4.1.8/binsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-14 16:11:33.000000 binsync-4.1.8/binsync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-14 16:11:33.000000 binsync-4.1.8/binsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 16:11:33.000000 binsync-4.1.8/binsync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-14 16:11:29.000000 binsync-4.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:11:33.932966 binsync-4.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:11:33.928966 binsync-4.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-05-14 16:11:29.000000 binsync-4.1.8/tests/test_angr_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-14 16:11:29.000000 binsync-4.1.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-14 16:11:29.000000 binsync-4.1.8/tests/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.942892 binsync-4.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 18:52:31.000000 binsync-4.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 18:52:31.000000 binsync-4.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-05-15 18:52:37.938892 binsync-4.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10189 2024-05-15 18:52:31.000000 binsync-4.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.930892 binsync-4.1.9/binsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/binsync_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34734 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.934892 binsync-4.1.9/binsync/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/core/cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27287 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/core/scheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20405 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.934892 binsync-4.1.9/binsync/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.934892 binsync-4.1.9/binsync/interface_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/interface_overrides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/interface_overrides/angr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/interface_overrides/binja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/interface_overrides/ghidra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/interface_overrides/ida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/loggercfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.934892 binsync-4.1.9/binsync/stub_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/stub_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.934892 binsync-4.1.9/binsync/stub_files/angr_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/stub_files/angr_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/stub_files/angr_files/plugin.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    22965 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/stub_files/binsync_binja_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/stub_files/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.934892 binsync-4.1.9/binsync/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19696 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/config_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/control_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.938892 binsync-4.1.9/binsync/ui/force_push/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/force_push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/force_push/force_push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.938892 binsync-4.1.9/binsync/ui/force_push/panels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/force_push/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/force_push/panels/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/force_push/panels/globals_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/force_push/panels/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/magic_sync_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.938892 binsync-4.1.9/binsync/ui/panel_tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/panel_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/panel_tabs/activity_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/panel_tabs/ctx_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/panel_tabs/functions_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/panel_tabs/globals_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/panel_tabs/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/panel_tabs/util_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-15 18:52:31.000000 binsync-4.1.9/binsync/ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.938892 binsync-4.1.9/binsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-05-15 18:52:37.000000 binsync-4.1.9/binsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-15 18:52:37.000000 binsync-4.1.9/binsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:52:37.000000 binsync-4.1.9/binsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 18:52:37.000000 binsync-4.1.9/binsync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-15 18:52:37.000000 binsync-4.1.9/binsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 18:52:37.000000 binsync-4.1.9/binsync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-15 18:52:31.000000 binsync-4.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:52:37.942892 binsync-4.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:52:37.938892 binsync-4.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-05-15 18:52:31.000000 binsync-4.1.9/tests/test_angr_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-15 18:52:31.000000 binsync-4.1.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-15 18:52:31.000000 binsync-4.1.9/tests/test_state.py
```

### Comparing `binsync-4.1.8/LICENSE` & `binsync-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/PKG-INFO` & `binsync-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsync
-Version: 4.1.8
+Version: 4.1.9
 Summary: A Collaboration framework for binary analysis tasks.
 License: BSD 2 Clause
 Project-URL: Homepage, https://github.com/angr/binsync
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: sortedcontainers
 Requires-Dist: toml
 Requires-Dist: GitPython
 Requires-Dist: filelock
 Requires-Dist: pycparser
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
-Requires-Dist: libbs>=1.3.2
+Requires-Dist: libbs>=1.3.3
 Provides-Extra: test
 Requires-Dist: angr-management; extra == "test"
 Requires-Dist: pytest-qt; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: ghidra
 Requires-Dist: ghidra_bridge; extra == "ghidra"
@@ -74,15 +74,16 @@
 
 ## Supported Platforms
 - IDA Pro: **>= 7.3**
 - Binary Ninja: **>= 2.4**
 - angr-management: **>= 9.0**
 - Ghidra: **>= 10.1**
 
-All versions require **Python >= 3.7** and **Git** installed on your system. Ghidra support is still very much in early stage, so only expect the minimal features like artifact name syncing and comments.
+All versions require **Python >= 3.8** and **Git** installed on your system. 
+Ghidra support is still very much in early stage, so only expect the minimal features like artifact name syncing and comments.
 
 
 ## Decompiler Support Progress
 Although we support the decompilers in the earlier section, not every decompiler is supported at the same level of syncing. 
 To understand the difference between artifact support, pull, push, and auto push, read our [decompiler use introduction](https://binsync.net/docs/dec-introduction/).
 
 ### IDA Pro
```

### Comparing `binsync-4.1.8/README.md` & `binsync-4.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 
 ## Supported Platforms
 - IDA Pro: **>= 7.3**
 - Binary Ninja: **>= 2.4**
 - angr-management: **>= 9.0**
 - Ghidra: **>= 10.1**
 
-All versions require **Python >= 3.7** and **Git** installed on your system. Ghidra support is still very much in early stage, so only expect the minimal features like artifact name syncing and comments.
+All versions require **Python >= 3.8** and **Git** installed on your system. 
+Ghidra support is still very much in early stage, so only expect the minimal features like artifact name syncing and comments.
 
 
 ## Decompiler Support Progress
 Although we support the decompilers in the earlier section, not every decompiler is supported at the same level of syncing. 
 To understand the difference between artifact support, pull, push, and auto push, read our [decompiler use introduction](https://binsync.net/docs/dec-introduction/).
 
 ### IDA Pro
```

### Comparing `binsync-4.1.8/binsync/__init__.py` & `binsync-4.1.9/binsync/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "4.1.8"
+__version__ = "4.1.9"
 
 
 #
 # logging
 #
 
 import logging
```

### Comparing `binsync-4.1.8/binsync/__main__.py` & `binsync-4.1.9/binsync/__main__.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/binsync_plugin.py` & `binsync-4.1.9/binsync/binsync_plugin.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/configuration.py` & `binsync-4.1.9/binsync/configuration.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/controller.py` & `binsync-4.1.9/binsync/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,14 +424,15 @@
         if self.sync_semaphore._value == self.DEFAULT_SEMAPHORE_SIZE:
             self.commit_artifact(*args, **kwargs)
 
     @init_checker
     def commit_artifact(self, artifact: Artifact, commit_msg=None, set_last_change=True, make_func=True, from_user=None, **kwargs) -> bool:
         """
         This function is NOT thread safe. You must call it in the order you want commits to appear.
+        Additionally, the Artifact must be LIFTED before committing it!
         """
         _l.debug(f"Attempting to push %s...", artifact)
         if not artifact:
             _l.warning(f"Attempting to push a None artifact, skipping...")
             return False
 
         try:
@@ -440,23 +441,22 @@
         except KeyError:
             _l.info(f"Attempting to push an unsupported Artifact of type {artifact}")
             return False
 
         state: State = self.client.master_state
         # assure functions existence for artifacts requiring a function
         if isinstance(artifact, (FunctionHeader, StackVariable, Comment)) and make_func:
-            func_addr = self.deci.art_lifter.lift_addr(artifact.func_addr if hasattr(artifact, "func_addr") else artifact.addr)
+            func_addr = artifact.func_addr if hasattr(artifact, "func_addr") else artifact.addr
             if func_addr is not None and not state.get_function(func_addr):
                 state.set_function(
-                    self.deci.art_lifter.lift(Function(func_addr, self.deci.get_func_size(func_addr))),
+                    Function(func_addr, self.deci.get_func_size(func_addr)),
                     set_last_change=set_last_change
                 )
 
         # take the current changes and layer them on top of the change in the state now
-        artifact = self.deci.art_lifter.lift(artifact)
         if not set_last_change:
             artifact.reset_last_change()
 
         identifiers = DecompilerInterface.get_identifiers(artifact)
         current_art = get_art_func(state, *identifiers)
         merged_artifact = self.merge_artifacts(current_art, artifact, merge_level=MergeLevel.OVERWRITE)
```

### Comparing `binsync-4.1.8/binsync/core/cache.py` & `binsync-4.1.9/binsync/core/cache.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/core/client.py` & `binsync-4.1.9/binsync/core/client.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/core/scheduler.py` & `binsync-4.1.9/binsync/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/core/state.py` & `binsync-4.1.9/binsync/core/state.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/core/user.py` & `binsync-4.1.9/binsync/core/user.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/installer.py` & `binsync-4.1.9/binsync/installer.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/interface_overrides/angr.py` & `binsync-4.1.9/binsync/interface_overrides/angr.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/interface_overrides/binja.py` & `binsync-4.1.9/binsync/interface_overrides/binja.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/interface_overrides/ghidra.py` & `binsync-4.1.9/binsync/interface_overrides/ghidra.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/interface_overrides/ida.py` & `binsync-4.1.9/binsync/interface_overrides/ida.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/loggercfg.py` & `binsync-4.1.9/binsync/loggercfg.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/stub_files/binsync_binja_logo.png` & `binsync-4.1.9/binsync/stub_files/binsync_binja_logo.png`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/stub_files/plugin.json` & `binsync-4.1.9/binsync/stub_files/plugin.json`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/config_dialog.py` & `binsync-4.1.9/binsync/ui/config_dialog.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/control_panel.py` & `binsync-4.1.9/binsync/ui/control_panel.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/force_push/force_push.py` & `binsync-4.1.9/binsync/ui/force_push/force_push.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/force_push/panels/functions_table.py` & `binsync-4.1.9/binsync/ui/force_push/panels/functions_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/force_push/panels/globals_table.py` & `binsync-4.1.9/binsync/ui/force_push/panels/globals_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/force_push/panels/table_model.py` & `binsync-4.1.9/binsync/ui/force_push/panels/table_model.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/magic_sync_dialog.py` & `binsync-4.1.9/binsync/ui/magic_sync_dialog.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/panel_tabs/activity_table.py` & `binsync-4.1.9/binsync/ui/panel_tabs/activity_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/panel_tabs/ctx_table.py` & `binsync-4.1.9/binsync/ui/panel_tabs/ctx_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/panel_tabs/functions_table.py` & `binsync-4.1.9/binsync/ui/panel_tabs/functions_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/panel_tabs/globals_table.py` & `binsync-4.1.9/binsync/ui/panel_tabs/globals_table.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/panel_tabs/table_model.py` & `binsync-4.1.9/binsync/ui/panel_tabs/table_model.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/panel_tabs/util_panel.py` & `binsync-4.1.9/binsync/ui/panel_tabs/util_panel.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync/ui/utils.py` & `binsync-4.1.9/binsync/ui/utils.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/binsync.egg-info/PKG-INFO` & `binsync-4.1.9/binsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsync
-Version: 4.1.8
+Version: 4.1.9
 Summary: A Collaboration framework for binary analysis tasks.
 License: BSD 2 Clause
 Project-URL: Homepage, https://github.com/angr/binsync
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 Requires-Dist: sortedcontainers
 Requires-Dist: toml
 Requires-Dist: GitPython
 Requires-Dist: filelock
 Requires-Dist: pycparser
 Requires-Dist: prompt_toolkit
 Requires-Dist: tqdm
-Requires-Dist: libbs>=1.3.2
+Requires-Dist: libbs>=1.3.3
 Provides-Extra: test
 Requires-Dist: angr-management; extra == "test"
 Requires-Dist: pytest-qt; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: ghidra
 Requires-Dist: ghidra_bridge; extra == "ghidra"
@@ -74,15 +74,16 @@
 
 ## Supported Platforms
 - IDA Pro: **>= 7.3**
 - Binary Ninja: **>= 2.4**
 - angr-management: **>= 9.0**
 - Ghidra: **>= 10.1**
 
-All versions require **Python >= 3.7** and **Git** installed on your system. Ghidra support is still very much in early stage, so only expect the minimal features like artifact name syncing and comments.
+All versions require **Python >= 3.8** and **Git** installed on your system. 
+Ghidra support is still very much in early stage, so only expect the minimal features like artifact name syncing and comments.
 
 
 ## Decompiler Support Progress
 Although we support the decompilers in the earlier section, not every decompiler is supported at the same level of syncing. 
 To understand the difference between artifact support, pull, push, and auto push, read our [decompiler use introduction](https://binsync.net/docs/dec-introduction/).
 
 ### IDA Pro
```

### Comparing `binsync-4.1.8/binsync.egg-info/SOURCES.txt` & `binsync-4.1.9/binsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/pyproject.toml` & `binsync-4.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "sortedcontainers",
     "toml",
     "GitPython",
     "filelock",
     "pycparser",
     "prompt_toolkit",
     "tqdm",
-    "libbs>=1.3.2"
+    "libbs>=1.3.3"
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

### Comparing `binsync-4.1.8/tests/test_angr_gui.py` & `binsync-4.1.9/tests/test_angr_gui.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/tests/test_client.py` & `binsync-4.1.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `binsync-4.1.8/tests/test_state.py` & `binsync-4.1.9/tests/test_state.py`

 * *Files identical despite different names*

