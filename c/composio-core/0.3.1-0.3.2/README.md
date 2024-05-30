# Comparing `tmp/composio_core-0.3.1.tar.gz` & `tmp/composio_core-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.3.1.tar", last modified: Thu May 30 09:15:36 2024, max compression
+gzip compressed data, was "composio_core-0.3.2.tar", last modified: Thu May 30 15:24:18 2024, max compression
```

## Comparing `composio_core-0.3.1.tar` & `composio_core-0.3.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.720712 composio_core-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 09:15:18.000000 composio_core-0.3.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-30 09:15:36.720712 composio_core-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-30 09:15:18.000000 composio_core-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.708712 composio_core-0.3.1/composio/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.712712 composio_core-0.3.1/composio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/add.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7910 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/triggers.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/cli/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.712712 composio_core-0.3.1/composio/client/
--rw-r--r--   0 runner    (1001) docker     (127)    31185 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/client/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)   213764 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/client/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/client/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/client/local_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.712712 composio_core-0.3.1/composio/local_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.712712 composio_core-0.3.1/composio/local_tools/file/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/file/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.712712 composio_core-0.3.1/composio/local_tools/local_workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.712712 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.716712 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.716712 composio_core-0.3.1/composio/local_tools/local_workspace/commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/commons/command_runner_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/commons/get_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/commons/history_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/commons/local_docker_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/commons/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.716712 composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.716712 composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.716712 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.716712 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/local_workspace/workspace/workspace_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.720712 composio_core-0.3.1/composio/local_tools/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/mathematical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/mathematical/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/mathematical/mathematical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/local_tools/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.720712 composio_core-0.3.1/composio/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/storage/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.720712 composio_core-0.3.1/composio/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.720712 composio_core-0.3.1/composio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/utils/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 09:15:18.000000 composio_core-0.3.1/composio/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:15:36.720712 composio_core-0.3.1/composio_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-30 09:15:36.000000 composio_core-0.3.1/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-30 09:15:36.000000 composio_core-0.3.1/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:15:36.000000 composio_core-0.3.1/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 09:15:36.000000 composio_core-0.3.1/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 09:15:36.000000 composio_core-0.3.1/composio_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 09:15:36.000000 composio_core-0.3.1/composio_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:15:36.720712 composio_core-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 09:15:18.000000 composio_core-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.485798 composio_core-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 15:23:58.000000 composio_core-0.3.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-30 15:24:18.485798 composio_core-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-30 15:23:58.000000 composio_core-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.473798 composio_core-0.3.2/composio/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.473798 composio_core-0.3.2/composio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/add.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7910 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/cli/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    31185 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)   235201 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/client/local_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/file/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/local_workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.477798 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19278 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/command_runner_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/get_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/history_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/local_docker_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/local_workspace/workspace/workspace_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/local_tools/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/mathematical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/mathematical/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/mathematical/mathematical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/local_tools/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/storage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.481798 composio_core-0.3.2/composio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 15:23:58.000000 composio_core-0.3.2/composio/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:24:18.485798 composio_core-0.3.2/composio_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 15:24:18.000000 composio_core-0.3.2/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:24:18.485798 composio_core-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 15:23:58.000000 composio_core-0.3.2/setup.py
```

### Comparing `composio_core-0.3.1/PKG-INFO` & `composio_core-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.1
+Version: 0.3.2
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.1/README.md` & `composio_core-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/__init__.py` & `composio_core-0.3.2/composio/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/actions.py` & `composio_core-0.3.2/composio/cli/actions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/add.py` & `composio_core-0.3.2/composio/cli/add.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/apps.py` & `composio_core-0.3.2/composio/cli/apps.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/connections.py` & `composio_core-0.3.2/composio/cli/connections.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/context.py` & `composio_core-0.3.2/composio/cli/context.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/integrations.py` & `composio_core-0.3.2/composio/cli/integrations.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/login.py` & `composio_core-0.3.2/composio/cli/login.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/cli/triggers.py` & `composio_core-0.3.2/composio/cli/triggers.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/client/__init__.py` & `composio_core-0.3.2/composio/client/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/client/endpoints.py` & `composio_core-0.3.2/composio/client/endpoints.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/client/enums.py` & `composio_core-0.3.2/composio/client/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,218 +12,278 @@
 
     @property
     def name(self) -> str:
         """Returns trigger name."""
         return self.value[0]
 
     IMPORTANT = ("default", "important")
-    ASANA_BATCH_API = ("asana", "Batch API")
-    ASANA_GOAL_RELATIONSHIPS = ("asana", "Goal relationships")
-    ASANA_USER_TASK_LISTS = ("asana", "User task lists")
-    ASANA_STORIES = ("asana", "Stories")
-    ASANA_CUSTOM_FIELDS = ("asana", "Custom fields")
-    ASANA_MEMBERSHIPS = ("asana", "Memberships")
-    ASANA_JOBS = ("asana", "Jobs")
-    ASANA_TIME_TRACKING_ENTRIES = ("asana", "Time tracking entries")
     ASANA_ALLOCATIONS = ("asana", "Allocations")
-    ASANA_RULES = ("asana", "Rules")
-    ASANA_ATTACHMENTS = ("asana", "Attachments")
-    ASANA_GOALS = ("asana", "Goals")
-    ASANA_CUSTOM_FIELD_SETTINGS = ("asana", "Custom field settings")
-    ASANA_TEAM_MEMBERSHIPS = ("asana", "Team memberships")
-    ASANA_ORGANIZATION_EXPORTS = ("asana", "Organization exports")
-    ASANA_PROJECTS = ("asana", "Projects")
-    ASANA_PORTFOLIOS = ("asana", "Portfolios")
     ASANA_AUDIT_LOG_API = ("asana", "Audit log API")
-    ASANA_TIME_PERIODS = ("asana", "Time periods")
-    ASANA_EVENTS = ("asana", "Events")
-    ASANA_TASK_TEMPLATES = ("asana", "Task templates")
-    ASANA_TYPEAHEAD = ("asana", "Typeahead")
+    ASANA_USERS = ("asana", "Users")
     ASANA_WORKSPACE_MEMBERSHIPS = ("asana", "Workspace memberships")
-    ASANA_WORKSPACES = ("asana", "Workspaces")
+    ASANA_TASKS = ("asana", "Tasks")
+    ASANA_TYPEAHEAD = ("asana", "Typeahead")
+    ASANA_TIME_TRACKING_ENTRIES = ("asana", "Time tracking entries")
     ASANA_WEBHOOKS = ("asana", "Webhooks")
-    ASANA_PROJECT_STATUSES = ("asana", "Project statuses")
-    ASANA_PROJECT_BRIEFS = ("asana", "Project briefs")
+    ASANA_ATTACHMENTS = ("asana", "Attachments")
+    ASANA_PROJECTS = ("asana", "Projects")
+    ASANA_CUSTOM_FIELD_SETTINGS = ("asana", "Custom field settings")
+    ASANA_PROJECT_MEMBERSHIPS = ("asana", "Project memberships")
     ASANA_TEAMS = ("asana", "Teams")
-    ASANA_USERS = ("asana", "Users")
+    ASANA_GOALS = ("asana", "Goals")
     ASANA_TAGS = ("asana", "Tags")
-    ASANA_PROJECT_MEMBERSHIPS = ("asana", "Project memberships")
+    ASANA_ORGANIZATION_EXPORTS = ("asana", "Organization exports")
+    ASANA_TIME_PERIODS = ("asana", "Time periods")
+    ASANA_BATCH_API = ("asana", "Batch API")
+    ASANA_PORTFOLIOS = ("asana", "Portfolios")
     ASANA_STATUS_UPDATES = ("asana", "Status updates")
-    ASANA_TASKS = ("asana", "Tasks")
+    ASANA_STORIES = ("asana", "Stories")
+    ASANA_TASK_TEMPLATES = ("asana", "Task templates")
     ASANA_PORTFOLIO_MEMBERSHIPS = ("asana", "Portfolio memberships")
+    ASANA_PROJECT_BRIEFS = ("asana", "Project briefs")
+    ASANA_USER_TASK_LISTS = ("asana", "User task lists")
+    ASANA_EVENTS = ("asana", "Events")
+    ASANA_JOBS = ("asana", "Jobs")
+    ASANA_MEMBERSHIPS = ("asana", "Memberships")
+    ASANA_CUSTOM_FIELDS = ("asana", "Custom fields")
+    ASANA_RULES = ("asana", "Rules")
     ASANA_PROJECT_TEMPLATES = ("asana", "Project templates")
+    ASANA_WORKSPACES = ("asana", "Workspaces")
+    ASANA_PROJECT_STATUSES = ("asana", "Project statuses")
+    ASANA_GOAL_RELATIONSHIPS = ("asana", "Goal relationships")
     ASANA_SECTIONS = ("asana", "Sections")
-    ATTIO_META = ("attio", "Meta")
+    ASANA_TEAM_MEMBERSHIPS = ("asana", "Team memberships")
+    ATTIO_WORKSPACE_MEMBERS = ("attio", "Workspace members")
     ATTIO_OBJECTS = ("attio", "Objects")
+    ATTIO_TASKS = ("attio", "Tasks")
+    ATTIO_RECORDS = ("attio", "Records")
     ATTIO_ENTRIES = ("attio", "Entries")
-    ATTIO_COMMENTS = ("attio", "Comments")
     ATTIO_WEBHOOKS = ("attio", "Webhooks")
-    ATTIO_NOTES = ("attio", "Notes")
+    ATTIO_COMMENTS = ("attio", "Comments")
+    ATTIO_META = ("attio", "Meta")
+    ATTIO_THREADS = ("attio", "Threads")
     ATTIO_LISTS = ("attio", "Lists")
-    ATTIO_WORKSPACE_MEMBERS = ("attio", "Workspace members")
-    ATTIO_TASKS = ("attio", "Tasks")
+    ATTIO_NOTES = ("attio", "Notes")
     ATTIO_ATTRIBUTES = ("attio", "Attributes")
-    ATTIO_THREADS = ("attio", "Threads")
-    ATTIO_RECORDS = ("attio", "Records")
-    BREVO_FILES = ("brevo", "Files")
-    BREVO_CONTACTS = ("brevo", "Contacts")
-    BREVO_SENDERS = ("brevo", "Senders")
-    BREVO_PROCESS = ("brevo", "Process")
-    BREVO_TRANSACTIONAL_WHATSAPP = ("brevo", "Transactional WhatsApp")
+    BREVO_INBOUND_PARSING = ("brevo", "Inbound Parsing")
+    BREVO_TASKS = ("brevo", "Tasks")
+    BREVO_WEBHOOKS = ("brevo", "Webhooks")
+    BREVO_TRANSACTIONAL_EMAILS = ("brevo", "Transactional emails")
+    BREVO_USER = ("brevo", "User")
     BREVO_EMAIL_CAMPAIGNS = ("brevo", "Email Campaigns")
+    BREVO_MASTER_ACCOUNT = ("brevo", "Master account")
     BREVO_DEALS = ("brevo", "Deals")
-    BREVO_ACCOUNT = ("brevo", "Account")
-    BREVO_CONVERSATIONS = ("brevo", "Conversations")
-    BREVO_COUPONS = ("brevo", "Coupons")
+    BREVO_ECOMMERCE = ("brevo", "Ecommerce")
+    BREVO_COMPANIES = ("brevo", "Companies")
+    BREVO_FILES = ("brevo", "Files")
+    BREVO_SMS_CAMPAIGNS = ("brevo", "SMS Campaigns")
     BREVO_TRANSACTIONAL_SMS = ("brevo", "Transactional SMS")
-    BREVO_MASTER_ACCOUNT = ("brevo", "Master account")
     BREVO_DOMAINS = ("brevo", "Domains")
-    BREVO_COMPANIES = ("brevo", "Companies")
-    BREVO_RESELLER = ("brevo", "Reseller")
-    BREVO_NOTES = ("brevo", "Notes")
-    BREVO_WEBHOOKS = ("brevo", "Webhooks")
-    BREVO_INBOUND_PARSING = ("brevo", "Inbound Parsing")
-    BREVO_USER = ("brevo", "User")
+    BREVO_COUPONS = ("brevo", "Coupons")
+    BREVO_SENDERS = ("brevo", "Senders")
+    BREVO_PROCESS = ("brevo", "Process")
+    BREVO_CONVERSATIONS = ("brevo", "Conversations")
     BREVO_EVENT = ("brevo", "Event")
-    BREVO_TRANSACTIONAL_EMAILS = ("brevo", "Transactional emails")
-    BREVO_EXTERNAL_FEEDS = ("brevo", "External Feeds")
-    BREVO_TASKS = ("brevo", "Tasks")
-    BREVO_ECOMMERCE = ("brevo", "Ecommerce")
     BREVO_WHATSAPP_CAMPAIGNS = ("brevo", "WhatsApp Campaigns")
-    BREVO_SMS_CAMPAIGNS = ("brevo", "SMS Campaigns")
+    BREVO_NOTES = ("brevo", "Notes")
+    BREVO_TRANSACTIONAL_WHATSAPP = ("brevo", "Transactional WhatsApp")
+    BREVO_EXTERNAL_FEEDS = ("brevo", "External Feeds")
+    BREVO_CONTACTS = ("brevo", "Contacts")
+    BREVO_ACCOUNT = ("brevo", "Account")
+    BREVO_RESELLER = ("brevo", "Reseller")
     CLICKUP_TIME_TRACKING = ("clickup", "Time Tracking")
+    CLICKUP_MEMBERS = ("clickup", "Members")
+    CLICKUP_USERS = ("clickup", "Users")
+    CLICKUP_TASKS = ("clickup", "Tasks")
     CLICKUP_GUESTS = ("clickup", "Guests")
+    CLICKUP_WEBHOOKS = ("clickup", "Webhooks")
+    CLICKUP_ATTACHMENTS = ("clickup", "Attachments")
     CLICKUP_COMMENTS = ("clickup", "Comments")
     CLICKUP_ROLES = ("clickup", "Roles")
-    CLICKUP_SHARED_HIERARCHY = ("clickup", "Shared Hierarchy")
-    CLICKUP_TASK_TEMPLATES = ("clickup", "Task Templates")
-    CLICKUP_ATTACHMENTS = ("clickup", "Attachments")
+    CLICKUP_VIEWS = ("clickup", "Views")
     CLICKUP_GOALS = ("clickup", "Goals")
-    CLICKUP_TASK_CHECKLISTS = ("clickup", "Task Checklists")
-    CLICKUP_CUSTOM_TASK_TYPES = ("clickup", "Custom Task Types")
-    CLICKUP_LISTS = ("clickup", "Lists")
-    CLICKUP_TIME_TRACKING__LEGACY_ = ("clickup", "Time Tracking (Legacy)")
-    CLICKUP_WEBHOOKS = ("clickup", "Webhooks")
-    CLICKUP_TASK_RELATIONSHIPS = ("clickup", "Task Relationships")
     CLICKUP_TEAMS___USER_GROUPS = ("clickup", "Teams - User Groups")
-    CLICKUP_CUSTOM_FIELDS = ("clickup", "Custom Fields")
-    CLICKUP_FOLDERS = ("clickup", "Folders")
     CLICKUP_TAGS = ("clickup", "Tags")
-    CLICKUP_USERS = ("clickup", "Users")
-    CLICKUP_SPACES = ("clickup", "Spaces")
-    CLICKUP_TASKS = ("clickup", "Tasks")
+    CLICKUP_LISTS = ("clickup", "Lists")
     CLICKUP_TEAMS___WORKSPACES = ("clickup", "Teams - Workspaces")
-    CLICKUP_MEMBERS = ("clickup", "Members")
-    CLICKUP_VIEWS = ("clickup", "Views")
+    CLICKUP_FOLDERS = ("clickup", "Folders")
+    CLICKUP_SHARED_HIERARCHY = ("clickup", "Shared Hierarchy")
+    CLICKUP_TASK_TEMPLATES = ("clickup", "Task Templates")
     CLICKUP_AUTHORIZATION = ("clickup", "Authorization")
-    ELEVENLABS_MODELS = ("elevenlabs", "models")
+    CLICKUP_CUSTOM_FIELDS = ("clickup", "Custom Fields")
+    CLICKUP_TASK_RELATIONSHIPS = ("clickup", "Task Relationships")
+    CLICKUP_SPACES = ("clickup", "Spaces")
+    CLICKUP_TIME_TRACKING__LEGACY_ = ("clickup", "Time Tracking (Legacy)")
+    CLICKUP_TASK_CHECKLISTS = ("clickup", "Task Checklists")
+    CLICKUP_CUSTOM_TASK_TYPES = ("clickup", "Custom Task Types")
+    ELEVENLABS_AUDIO_NATIVE = ("elevenlabs", "audio-native")
+    ELEVENLABS_VOICE_GENERATION = ("elevenlabs", "voice-generation")
     ELEVENLABS_SPEECH_HISTORY = ("elevenlabs", "speech-history")
+    ELEVENLABS_MODELS = ("elevenlabs", "models")
     ELEVENLABS_WORKSPACE = ("elevenlabs", "workspace")
     ELEVENLABS_SPEECH_TO_SPEECH = ("elevenlabs", "speech-to-speech")
-    ELEVENLABS_TEXT_TO_SPEECH = ("elevenlabs", "text-to-speech")
-    ELEVENLABS_PROJECTS = ("elevenlabs", "projects")
     ELEVENLABS_SAMPLES = ("elevenlabs", "samples")
-    ELEVENLABS_PRONUNCIATION_DICTIONARY = ("elevenlabs", "Pronunciation Dictionary")
+    ELEVENLABS_USER = ("elevenlabs", "user")
     ELEVENLABS_DUBBING = ("elevenlabs", "dubbing")
+    ELEVENLABS_PRONUNCIATION_DICTIONARY = ("elevenlabs", "Pronunciation Dictionary")
     ELEVENLABS_VOICES = ("elevenlabs", "voices")
-    ELEVENLABS_VOICE_GENERATION = ("elevenlabs", "voice-generation")
-    ELEVENLABS_USER = ("elevenlabs", "user")
-    ELEVENLABS_AUDIO_NATIVE = ("elevenlabs", "audio-native")
-    FIGMA_COMMENT_REACTIONS = ("figma", "Comment Reactions")
-    FIGMA_COMPONENTS = ("figma", "Components")
-    FIGMA_ACTIVITY_LOGS = ("figma", "Activity Logs")
-    FIGMA_COMMENTS = ("figma", "Comments")
-    FIGMA_DEV_RESOURCES = ("figma", "Dev Resources")
+    ELEVENLABS_TEXT_TO_SPEECH = ("elevenlabs", "text-to-speech")
+    ELEVENLABS_PROJECTS = ("elevenlabs", "projects")
     FIGMA_PAYMENTS = ("figma", "Payments")
+    FIGMA_COMPONENTS = ("figma", "Components")
+    FIGMA_STYLES = ("figma", "Styles")
     FIGMA_USERS = ("figma", "Users")
+    FIGMA_COMMENT_REACTIONS = ("figma", "Comment Reactions")
     FIGMA_VARIABLES = ("figma", "Variables")
-    FIGMA_STYLES = ("figma", "Styles")
-    FIGMA_FILES = ("figma", "Files")
+    FIGMA_DEV_RESOURCES = ("figma", "Dev Resources")
     FIGMA_WEBHOOKS = ("figma", "Webhooks")
-    FIGMA_PROJECTS = ("figma", "Projects")
     FIGMA_COMPONENT_SETS = ("figma", "Component Sets")
-    LISTENNOTES_PODCASTER_API = ("listennotes", "Podcaster API")
+    FIGMA_COMMENTS = ("figma", "Comments")
+    FIGMA_FILES = ("figma", "Files")
+    FIGMA_PROJECTS = ("figma", "Projects")
+    FIGMA_ACTIVITY_LOGS = ("figma", "Activity Logs")
     LISTENNOTES_SEARCH_API = ("listennotes", "Search API")
-    LISTENNOTES_DIRECTORY_API = ("listennotes", "Directory API")
     LISTENNOTES_PLAYLIST_API = ("listennotes", "Playlist API")
+    LISTENNOTES_DIRECTORY_API = ("listennotes", "Directory API")
+    LISTENNOTES_PODCASTER_API = ("listennotes", "Podcaster API")
     LISTENNOTES_INSIGHTS_API = ("listennotes", "Insights API")
-    NASA_PROJECT = ("nasa", "Project")
     NASA_ORGANIZATION = ("nasa", "Organization")
     NASA_RESOURCE = ("nasa", "Resource")
-    OKTA_SUBSCRIPTION = ("okta", "Subscription")
-    OKTA_USERFACTOR = ("okta", "UserFactor")
-    OKTA_AUTHORIZATIONSERVER = ("okta", "AuthorizationServer")
+    NASA_PROJECT = ("nasa", "Project")
+    OKTA_FEATURE = ("okta", "Feature")
+    OKTA_USERTYPE = ("okta", "UserType")
     OKTA_NETWORKZONE = ("okta", "NetworkZone")
-    OKTA_BRAND = ("okta", "Brand")
-    OKTA_LINKEDOBJECT = ("okta", "LinkedObject")
-    OKTA_AUTHENTICATOR = ("okta", "Authenticator")
-    OKTA_POLICY = ("okta", "Policy")
-    OKTA_INLINEHOOK = ("okta", "InlineHook")
     OKTA_USERSCHEMA = ("okta", "UserSchema")
-    OKTA_ORG = ("okta", "Org")
-    OKTA_TEMPLATE = ("okta", "Template")
-    OKTA_GROUP = ("okta", "Group")
-    OKTA_THREATINSIGHT = ("okta", "ThreatInsight")
-    OKTA_PROFILEMAPPING = ("okta", "ProfileMapping")
-    OKTA_SESSION = ("okta", "Session")
+    OKTA_SUBSCRIPTION = ("okta", "Subscription")
+    OKTA_USER = ("okta", "User")
     OKTA_GROUPSCHEMA = ("okta", "GroupSchema")
+    OKTA_EVENTHOOK = ("okta", "EventHook")
+    OKTA_SESSION = ("okta", "Session")
+    OKTA_POLICY = ("okta", "Policy")
+    OKTA_THREATINSIGHT = ("okta", "ThreatInsight")
+    OKTA_TRUSTEDORIGIN = ("okta", "TrustedOrigin")
     OKTA_LOG = ("okta", "Log")
+    OKTA_PROFILEMAPPING = ("okta", "ProfileMapping")
+    OKTA_AUTHENTICATOR = ("okta", "Authenticator")
+    OKTA_TEMPLATE = ("okta", "Template")
+    OKTA_APPLICATION = ("okta", "Application")
+    OKTA_ORG = ("okta", "Org")
+    OKTA_LINKEDOBJECT = ("okta", "LinkedObject")
+    OKTA_INLINEHOOK = ("okta", "InlineHook")
     OKTA_DOMAIN = ("okta", "Domain")
-    OKTA_USERTYPE = ("okta", "UserType")
-    OKTA_USER = ("okta", "User")
-    OKTA_TRUSTEDORIGIN = ("okta", "TrustedOrigin")
-    OKTA_FEATURE = ("okta", "Feature")
     OKTA_IDENTITYPROVIDER = ("okta", "IdentityProvider")
-    OKTA_APPLICATION = ("okta", "Application")
-    OKTA_EVENTHOOK = ("okta", "EventHook")
-    SPOTIFY_SEARCH = ("spotify", "Search")
-    SPOTIFY_GENRES = ("spotify", "Genres")
+    OKTA_USERFACTOR = ("okta", "UserFactor")
+    OKTA_GROUP = ("okta", "Group")
+    OKTA_BRAND = ("okta", "Brand")
+    OKTA_AUTHORIZATIONSERVER = ("okta", "AuthorizationServer")
+    SLACK_APPS = ("slack", "apps")
+    SLACK_TEAM_PROFILE = ("slack", "team.profile")
+    SLACK_ADMIN_APPS_APPROVED = ("slack", "admin.apps.approved")
+    SLACK_ADMIN_TEAMS_SETTINGS = ("slack", "admin.teams.settings")
+    SLACK_ADMIN_CONVERSATIONS_EKM = ("slack", "admin.conversations.ekm")
+    SLACK_ADMIN_INVITEREQUESTS_DENIED = ("slack", "admin.inviteRequests.denied")
+    SLACK_APPS_EVENT_AUTHORIZATIONS = ("slack", "apps.event.authorizations")
+    SLACK_STARS = ("slack", "stars")
+    SLACK_OAUTH = ("slack", "oauth")
+    SLACK_REMINDERS = ("slack", "reminders")
+    SLACK_ADMIN_APPS_REQUESTS = ("slack", "admin.apps.requests")
+    SLACK_ADMIN_USERS = ("slack", "admin.users")
+    SLACK_DIALOG = ("slack", "dialog")
+    SLACK_REACTIONS = ("slack", "reactions")
+    SLACK_SEARCH = ("slack", "search")
+    SLACK_API = ("slack", "api")
+    SLACK_IMPORTANT = ("slack", "important")
+    SLACK_OAUTH_V2 = ("slack", "oauth.v2")
+    SLACK_PINS = ("slack", "pins")
+    SLACK_ADMIN_APPS_RESTRICTED = ("slack", "admin.apps.restricted")
+    SLACK_ADMIN_APPS = ("slack", "admin.apps")
+    SLACK_ADMIN_CONVERSATIONS_RESTRICTACCESS = (
+        "slack",
+        "admin.conversations.restrictAccess",
+    )
+    SLACK_EMOJI = ("slack", "emoji")
+    SLACK_APPS_PERMISSIONS_USERS = ("slack", "apps.permissions.users")
+    SLACK_BOTS = ("slack", "bots")
+    SLACK_FILES = ("slack", "files")
+    SLACK_ADMIN_USERGROUPS = ("slack", "admin.usergroups")
+    SLACK_ADMIN = ("slack", "admin")
+    SLACK_TEAM = ("slack", "team")
+    SLACK_ADMIN_USERS_SESSION = ("slack", "admin.users.session")
+    SLACK_CHAT_SCHEDULEDMESSAGES = ("slack", "chat.scheduledMessages")
+    SLACK_FILES_REMOTE = ("slack", "files.remote")
+    SLACK_WORKFLOWS = ("slack", "workflows")
+    SLACK_CONVERSATIONS = ("slack", "conversations")
+    SLACK_APPS_PERMISSIONS_SCOPES = ("slack", "apps.permissions.scopes")
+    SLACK_ADMIN_EMOJI = ("slack", "admin.emoji")
+    SLACK_DND = ("slack", "dnd")
+    SLACK_RTM = ("slack", "rtm")
+    SLACK_ADMIN_TEAMS_ADMINS = ("slack", "admin.teams.admins")
+    SLACK_FILES_COMMENTS = ("slack", "files.comments")
+    SLACK_USERS = ("slack", "users")
+    SLACK_USERGROUPS_USERS = ("slack", "usergroups.users")
+    SLACK_ADMIN_CONVERSATIONS = ("slack", "admin.conversations")
+    SLACK_APPS_PERMISSIONS = ("slack", "apps.permissions")
+    SLACK_CHAT = ("slack", "chat")
+    SLACK_ADMIN_INVITEREQUESTS = ("slack", "admin.inviteRequests")
+    SLACK_USERGROUPS = ("slack", "usergroups")
+    SLACK_ADMIN_INVITEREQUESTS_APPROVED = ("slack", "admin.inviteRequests.approved")
+    SLACK_ADMIN_TEAMS = ("slack", "admin.teams")
+    SLACK_ADMIN_TEAMS_OWNERS = ("slack", "admin.teams.owners")
+    SLACK_AUTH = ("slack", "auth")
+    SLACK_CALLS_PARTICIPANTS = ("slack", "calls.participants")
+    SLACK_MIGRATION = ("slack", "migration")
+    SLACK_APPS_PERMISSIONS_RESOURCES = ("slack", "apps.permissions.resources")
+    SLACK_USERS_PROFILE = ("slack", "users.profile")
+    SLACK_VIEWS = ("slack", "views")
+    SLACK_CALLS = ("slack", "calls")
     SPOTIFY_EPISODES = ("spotify", "Episodes")
-    SPOTIFY_ALBUMS = ("spotify", "Albums")
-    SPOTIFY_LIBRARY = ("spotify", "Library")
     SPOTIFY_USERS = ("spotify", "Users")
-    SPOTIFY_PLAYER = ("spotify", "Player")
-    SPOTIFY_CHAPTERS = ("spotify", "Chapters")
     SPOTIFY_MARKETS = ("spotify", "Markets")
-    SPOTIFY_AUDIOBOOKS = ("spotify", "Audiobooks")
-    SPOTIFY_ARTISTS = ("spotify", "Artists")
-    SPOTIFY_SHOWS = ("spotify", "Shows")
-    SPOTIFY_PLAYLISTS = ("spotify", "Playlists")
+    SPOTIFY_PLAYER = ("spotify", "Player")
     SPOTIFY_TRACKS = ("spotify", "Tracks")
+    SPOTIFY_PLAYLISTS = ("spotify", "Playlists")
+    SPOTIFY_GENRES = ("spotify", "Genres")
+    SPOTIFY_SHOWS = ("spotify", "Shows")
+    SPOTIFY_CHAPTERS = ("spotify", "Chapters")
     SPOTIFY_CATEGORIES = ("spotify", "Categories")
-    TASKADE_PROJECT = ("taskade", "Project")
-    TASKADE_WORKSPACE = ("taskade", "Workspace")
-    TASKADE_TASK = ("taskade", "Task")
+    SPOTIFY_ARTISTS = ("spotify", "Artists")
+    SPOTIFY_ALBUMS = ("spotify", "Albums")
+    SPOTIFY_AUDIOBOOKS = ("spotify", "Audiobooks")
+    SPOTIFY_SEARCH = ("spotify", "Search")
+    SPOTIFY_LIBRARY = ("spotify", "Library")
     TASKADE_ME = ("taskade", "Me")
+    TASKADE_TASK = ("taskade", "Task")
     TASKADE_FOLDER = ("taskade", "Folder")
+    TASKADE_WORKSPACE = ("taskade", "Workspace")
     TASKADE_AGENT = ("taskade", "Agent")
-    WHATSAPP_GROUPS = ("whatsapp", "Groups")
+    TASKADE_PROJECT = ("taskade", "Project")
+    WHATSAPP_REGISTRATION = ("whatsapp", "Registration")
+    WHATSAPP_USERS = ("whatsapp", "Users")
+    WHATSAPP_APPLICATION = ("whatsapp", "Application")
+    WHATSAPP_MESSAGES = ("whatsapp", "Messages")
+    WHATSAPP_HEALTH = ("whatsapp", "Health")
+    WHATSAPP_PROFILE = ("whatsapp", "Profile")
     WHATSAPP_CONTACTS = ("whatsapp", "Contacts")
+    WHATSAPP_CERTIFICATES = ("whatsapp", "Certificates")
     WHATSAPP_MEDIA = ("whatsapp", "Media")
-    WHATSAPP_PROFILE = ("whatsapp", "Profile")
-    WHATSAPP_USERS = ("whatsapp", "Users")
-    WHATSAPP_REGISTRATION = ("whatsapp", "Registration")
     WHATSAPP_BACKUP_RESTORE = ("whatsapp", "Backup/Restore")
-    WHATSAPP_HEALTH = ("whatsapp", "Health")
-    WHATSAPP_MESSAGES = ("whatsapp", "Messages")
     WHATSAPP_BUSINESS_PROFILE = ("whatsapp", "Business Profile")
-    WHATSAPP_APPLICATION = ("whatsapp", "Application")
+    WHATSAPP_GROUPS = ("whatsapp", "Groups")
     WHATSAPP_TWO_STEP_VERIFICATION = ("whatsapp", "Two-Step Verification")
-    WHATSAPP_CERTIFICATES = ("whatsapp", "Certificates")
-    ZOOM_SIP_PHONE = ("zoom", "SIP Phone")
+    ZOOM_TRACKING_FIELD = ("zoom", "Tracking Field")
     ZOOM_ARCHIVING = ("zoom", "Archiving")
-    ZOOM_H323_DEVICES = ("zoom", "H323 Devices")
-    ZOOM_MEETINGS = ("zoom", "Meetings")
-    ZOOM_PAC = ("zoom", "PAC")
     ZOOM_TSP = ("zoom", "TSP")
-    ZOOM_REPORTS = ("zoom", "Reports")
     ZOOM_WEBINARS = ("zoom", "Webinars")
+    ZOOM_MEETINGS = ("zoom", "Meetings")
     ZOOM_DEVICES = ("zoom", "Devices")
-    ZOOM_TRACKING_FIELD = ("zoom", "Tracking Field")
+    ZOOM_PAC = ("zoom", "PAC")
+    ZOOM_SIP_PHONE = ("zoom", "SIP Phone")
     ZOOM_CLOUD_RECORDING = ("zoom", "Cloud Recording")
+    ZOOM_H323_DEVICES = ("zoom", "H323 Devices")
+    ZOOM_REPORTS = ("zoom", "Reports")
 
 
 class App(str, Enum):
     """Composio App."""
 
     @property
     def is_local(self) -> bool:
@@ -314,14 +374,15 @@
     FRONT = "front"
     GITHUB = "github"
     GITLAB = "gitlab"
     GMAIL = "gmail"
     GOOGLECALENDAR = "googlecalendar"
     GOOGLEDOCS = "googledocs"
     GOOGLEDRIVE = "googledrive"
+    GOOGLEMEET = "googlemeet"
     GOOGLESHEETS = "googlesheets"
     GOOGLETASKS = "googletasks"
     GORGIAS = "gorgias"
     GUMROAD = "gumroad"
     GURU = "guru"
     HACKERRANK_WORK = "hackerrank-work"
     HARVEST = "harvest"
@@ -3508,68 +3569,81 @@
         False,
     )
     GOOGLECALENDAR_GET_CURRENT_DATE_TIME = (
         "googlecalendar",
         "googlecalendar_get_current_date_time",
         False,
     )
+    GOOGLEDOCS_UPDATE_EXISTING_DOCUMENT = (
+        "googledocs",
+        "googledocs_update_existing_document",
+        False,
+    )
+    GOOGLEDOCS_GET_DOCUMENT_BY_ID = (
+        "googledocs",
+        "googledocs_get_document_by_id",
+        False,
+    )
+    GOOGLEDOCS_CREATE_DOCUMENT = ("googledocs", "googledocs_create_document", False)
     GOOGLEDRIVE_COPY_FILE = ("googledrive", "googledrive_copy_file", False)
     GOOGLEDRIVE_CREATE_FOLDER = ("googledrive", "googledrive_create_folder", False)
     GOOGLEDRIVE_CREATE_FILE_FROM_TEXT = (
         "googledrive",
         "googledrive_create_file_from_text",
         False,
     )
     GOOGLEDRIVE_FIND_FILE = ("googledrive", "googledrive_find_file", False)
     GOOGLEDRIVE_FIND_FOLDER = ("googledrive", "googledrive_find_folder", False)
     GOOGLEDRIVE_ADD_FILE_SHARING_PREFERENCE = (
         "googledrive",
         "googledrive_add_file_sharing_preference",
         False,
     )
-    GOOGLESHEETS_CREATE_GOOGLE_SHEET1 = (
-        "googlesheets",
-        "googlesheets_create_google_sheet1",
-        False,
-    )
-    GOOGLESHEETS_CREATE_SPREADSHEET_COLUMN = (
-        "googlesheets",
-        "googlesheets_create_spreadsheet_column",
+    GOOGLEDRIVE_EXPORT_FILE = ("googledrive", "googledrive_export_file", False)
+    GOOGLEDRIVE_EDIT_FILE = ("googledrive", "googledrive_edit_file", False)
+    GOOGLEDRIVE_DELETE_FOLDER_OR_FILE = (
+        "googledrive",
+        "googledrive_delete_folder_or_file",
         False,
     )
-    GOOGLESHEETS_CREATE_SPREADSHEET_ROW = (
-        "googlesheets",
-        "googlesheets_create_spreadsheet_row",
+    GOOGLEMEET_GET_MEET = ("googlemeet", "googlemeet_get_meet", False)
+    GOOGLEMEET_CREATE_MEET = ("googlemeet", "googlemeet_create_meet", False)
+    GOOGLEMEET_GET_CONFERENCE_RECORD_FOR_MEET = (
+        "googlemeet",
+        "googlemeet_get_conference_record_for_meet",
         False,
     )
-    GOOGLESHEETS_LOOKUP_SPREADSHEET_ROW = (
-        "googlesheets",
-        "googlesheets_lookup_spreadsheet_row",
+    GOOGLEMEET_GET_RECORDINGS_BY_CONFERENCE_RECORD_ID = (
+        "googlemeet",
+        "googlemeet_get_recordings_by_conference_record_id",
         False,
     )
-    GOOGLESHEETS_FIND_WORKSHEET_BY_TITLE = (
-        "googlesheets",
-        "googlesheets_find_worksheet_by_title",
+    GOOGLEMEET_GET_TRANSCRIPTS_BY_CONFERENCE_RECORD_ID = (
+        "googlemeet",
+        "googlemeet_get_transcripts_by_conference_record_id",
         False,
     )
-    GOOGLESHEETS_FORMAT_SPREADSHEET_ROW = (
+    GOOGLESHEETS_CREATE_GOOGLE_SHEET1 = (
         "googlesheets",
-        "googlesheets_format_spreadsheet_row",
+        "googlesheets_create_google_sheet1",
         False,
     )
-    GOOGLESHEETS_UPDATE_SPREADSHEET_ROW = (
+    GOOGLESHEETS_GET_SPREADSHEET_INFO = (
         "googlesheets",
-        "googlesheets_update_spreadsheet_row",
+        "googlesheets_get_spreadsheet_info",
         False,
     )
-    GOOGLESHEETS_FIND_OR_CREATE_WORKSHEET = (
+    GOOGLESHEETS_LOOKUP_SPREADSHEET_ROW = (
         "googlesheets",
-        "googlesheets_find_or_create_worksheet",
+        "googlesheets_lookup_spreadsheet_row",
         False,
     )
+    GOOGLESHEETS_BATCH_UPDATE = ("googlesheets", "googlesheets_batch_update", False)
+    GOOGLESHEETS_CLEAR_VALUES = ("googlesheets", "googlesheets_clear_values", False)
+    GOOGLESHEETS_BATCH_GET = ("googlesheets", "googlesheets_batch_get", False)
     GOOGLETASKS_CREATE_TASK_LIST = (
         "googletasks",
         "googletasks_create_task_list",
         False,
     )
     GOOGLETASKS_DELETE_TASK_LIST = (
         "googletasks",
@@ -4894,18 +4968,476 @@
     OKTA_NETWORK_ZONE_DEACTIVATE_ZONE_LIFECYCLE = (
         "okta",
         "okta_network_zone_deactivate_zone_lifecycle",
         False,
     )
     SCHEDULER_SCHEDULE_JOB_ACTION = ("scheduler", "scheduler_schedule_job_action", True)
     SERPAPI_SEARCH = ("serpapi", "serpapi_search", True)
-    SLACK_SEND_SLACK_MESSAGE = ("slack", "slack_send_slack_message", False)
-    SLACK_LIST_SLACK_CHANNELS = ("slack", "slack_list_slack_channels", False)
-    SLACK_LIST_SLACK_MEMBERS = ("slack", "slack_list_slack_members", False)
-    SLACK_LIST_SLACK_MESSAGES = ("slack", "slack_list_slack_messages", False)
+    SLACK_ADMIN_APPS_APPROVE_APP_INSTALLATION = (
+        "slack",
+        "slack_admin_apps_approve_app_installation",
+        False,
+    )
+    SLACK_ADMIN_APPS_APPROVED_LIST = ("slack", "slack_admin_apps_approved_list", False)
+    SLACK_ADMIN_APPS_REQUESTS_LIST = ("slack", "slack_admin_apps_requests_list", False)
+    SLACK_ADMIN_APPS_RESTRICT_APP = ("slack", "slack_admin_apps_restrict_app", False)
+    SLACK_ADMIN_APPS_RESTRICTED_GET_LIST = (
+        "slack",
+        "slack_admin_apps_restricted_get_list",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_ARCHIVE_CHANNEL = (
+        "slack",
+        "slack_admin_conversations_archive_channel",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_CONVERT_TO_PRIVATE_CHANNEL = (
+        "slack",
+        "slack_admin_conversations_convert_to_private_channel",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_CREATE_CHANNEL_BASED_CONVERSATION = (
+        "slack",
+        "slack_admin_conversations_create_channel_based_conversation",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_DELETE_CHANNEL = (
+        "slack",
+        "slack_admin_conversations_delete_channel",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_DISCONNECT_SHARED_CHANNEL = (
+        "slack",
+        "slack_admin_conversations_disconnect_shared_channel",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_E_KM_LIST_ORIGINAL_CONNECTED_CHANNEL_INFO = (
+        "slack",
+        "slack_admin_conversations_e_km_list_original_connected_channel_info",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_GET_CONVERSATION_PREF_S = (
+        "slack",
+        "slack_admin_conversations_get_conversation_pref_s",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_GET_TEAMS_LIST = (
+        "slack",
+        "slack_admin_conversations_get_teams_list",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_INVITE_USER_TO_CHANNEL = (
+        "slack",
+        "slack_admin_conversations_invite_user_to_channel",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_RENAME_CHANNEL = (
+        "slack",
+        "slack_admin_conversations_rename_channel",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_RESTRICT_ACCESS_ADD_GROUP_IDP_GROUPS = (
+        "slack",
+        "slack_admin_conversations_restrict_access_add_group_idp_groups",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_RESTRICT_ACCESS_LIST_GROUPS = (
+        "slack",
+        "slack_admin_conversations_restrict_access_list_groups",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_RESTRICT_ACCESS_REMOVE_IDP_GROUP = (
+        "slack",
+        "slack_admin_conversations_restrict_access_remove_idp_group",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_SEARCH_CHANNELS = (
+        "slack",
+        "slack_admin_conversations_search_channels",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_SET_CONVERSATION_PREF_S = (
+        "slack",
+        "slack_admin_conversations_set_conversation_pref_s",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATIONS_SET_TEAMS_WORK_SPACE_CONNECTION = (
+        "slack",
+        "slack_admin_conversations_set_teams_work_space_connection",
+        False,
+    )
+    SLACK_ADMIN_CONVERSATION_SUN_ARCHIVE_CHANNEL = (
+        "slack",
+        "slack_admin_conversation_sun_archive_channel",
+        False,
+    )
+    SLACK_ADMIN_E_MOJI_ADDE_MOJI = ("slack", "slack_admin_e_moji_adde_moji", False)
+    SLACK_ADMIN_E_MOJI_ALIAS_ADD = ("slack", "slack_admin_e_moji_alias_add", False)
+    SLACK_ADMIN_E_MOJI_LIST_ENTERPRISE_E_MOJI = (
+        "slack",
+        "slack_admin_e_moji_list_enterprise_e_moji",
+        False,
+    )
+    SLACK_ADMIN_E_MOJI_REMOVE_ENTERPRISE_E_MOJI = (
+        "slack",
+        "slack_admin_e_moji_remove_enterprise_e_moji",
+        False,
+    )
+    SLACK_ADMIN_E_MOJI_RENAME_E_MOJI = (
+        "slack",
+        "slack_admin_e_moji_rename_e_moji",
+        False,
+    )
+    SLACK_ADMIN_INVITE_REQUESTS_APPROVE_REQUEST = (
+        "slack",
+        "slack_admin_invite_requests_approve_request",
+        False,
+    )
+    SLACK_ADMIN_INVITE_REQUESTS_APPROVED_LIST = (
+        "slack",
+        "slack_admin_invite_requests_approved_list",
+        False,
+    )
+    SLACK_ADMIN_INVITE_REQUESTS_DENIED_LIST = (
+        "slack",
+        "slack_admin_invite_requests_denied_list",
+        False,
+    )
+    SLACK_ADMIN_INVITE_REQUESTS_DENY_REQUEST = (
+        "slack",
+        "slack_admin_invite_requests_deny_request",
+        False,
+    )
+    SLACK_ADMIN_INVITE_REQUESTS_LIST_PENDING_WORK_SPACE_INVITE_REQUESTS = (
+        "slack",
+        "slack_admin_invite_requests_list_pending_work_space_invite_requests",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_ADMINS_GET_ALL = (
+        "slack",
+        "slack_admin_teams_admins_get_all",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_CREATE_ENTERPRISE_TEAM = (
+        "slack",
+        "slack_admin_teams_create_enterprise_team",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_LIST_ALL = ("slack", "slack_admin_teams_list_all", False)
+    SLACK_ADMIN_TEAMS_OWNERS_LIST_OWNERS = (
+        "slack",
+        "slack_admin_teams_owners_list_owners",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_SETTINGS_GET_INFO = (
+        "slack",
+        "slack_admin_teams_settings_get_info",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_SETTINGS_SET_DEFAULT_CHANNELS = (
+        "slack",
+        "slack_admin_teams_settings_set_default_channels",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_SETTINGS_SET_DESCRIPTION = (
+        "slack",
+        "slack_admin_teams_settings_set_description",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_SETTINGS_SET_DISCOVER_ABILITY_OF_WORK_SPACE = (
+        "slack",
+        "slack_admin_teams_settings_set_discover_ability_of_work_space",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_SETTINGS_SET_ICON = (
+        "slack",
+        "slack_admin_teams_settings_set_icon",
+        False,
+    )
+    SLACK_ADMIN_TEAMS_SETTINGS_SET_NAME = (
+        "slack",
+        "slack_admin_teams_settings_set_name",
+        False,
+    )
+    SLACK_ADMIN_USER_GROUPS_ADD_DEFAULT_CHANNELS = (
+        "slack",
+        "slack_admin_user_groups_add_default_channels",
+        False,
+    )
+    SLACK_ADMIN_USER_GROUPS_ASSOCIATE_DEFAULT_WORK_SPACES = (
+        "slack",
+        "slack_admin_user_groups_associate_default_work_spaces",
+        False,
+    )
+    SLACK_ADMIN_USER_GROUPS_LIST_CHANNELS_GET = (
+        "slack",
+        "slack_admin_user_groups_list_channels_get",
+        False,
+    )
+    SLACK_ADMIN_USER_GROUPS_REMOVE_CHANNELS = (
+        "slack",
+        "slack_admin_user_groups_remove_channels",
+        False,
+    )
+    SLACK_ADMIN_USERS_ADD_WORK_SPACE_USER = (
+        "slack",
+        "slack_admin_users_add_work_space_user",
+        False,
+    )
+    SLACK_ADMIN_USERS_INVITE_USER_TO_WORK_SPACE = (
+        "slack",
+        "slack_admin_users_invite_user_to_work_space",
+        False,
+    )
+    SLACK_ADMIN_USERS_LIST_WORK_SPACE_USERS = (
+        "slack",
+        "slack_admin_users_list_work_space_users",
+        False,
+    )
+    SLACK_ADMIN_USERS_REMOVE_USER_FROM_WORK_SPACE = (
+        "slack",
+        "slack_admin_users_remove_user_from_work_space",
+        False,
+    )
+    SLACK_ADMIN_USERS_SESSION_INVALIDATE_SESSION = (
+        "slack",
+        "slack_admin_users_session_invalidate_session",
+        False,
+    )
+    SLACK_ADMIN_USERS_SESSION_RESET_SESSIONS = (
+        "slack",
+        "slack_admin_users_session_reset_sessions",
+        False,
+    )
+    SLACK_ADMIN_USERS_SET_ADMIN_USER = (
+        "slack",
+        "slack_admin_users_set_admin_user",
+        False,
+    )
+    SLACK_ADMIN_USERS_SET_EXPIRATION_GUEST = (
+        "slack",
+        "slack_admin_users_set_expiration_guest",
+        False,
+    )
+    SLACK_ADMIN_USERS_SET_WORK_SPACE_OWNER = (
+        "slack",
+        "slack_admin_users_set_work_space_owner",
+        False,
+    )
+    SLACK_ADMIN_USERS_SET_REGULAR_USER = (
+        "slack",
+        "slack_admin_users_set_regular_user",
+        False,
+    )
+    SLACK_API_TEST = ("slack", "slack_api_test", False)
+    SLACK_APPS_EVENT_AUTHORIZATIONS_GET_LIST = (
+        "slack",
+        "slack_apps_event_authorizations_get_list",
+        False,
+    )
+    SLACK_APPS_PERMISSIONS_LIST_PERMISSIONS = (
+        "slack",
+        "slack_apps_permissions_list_permissions",
+        False,
+    )
+    SLACK_APPS_PERMISSIONS_ADDITIONAL_SCOPES_REQUEST = (
+        "slack",
+        "slack_apps_permissions_additional_scopes_request",
+        False,
+    )
+    SLACK_APPS_PERMISSIONS_RESOURCES_GET_RESOURCES_LIST = (
+        "slack",
+        "slack_apps_permissions_resources_get_resources_list",
+        False,
+    )
+    SLACK_APPS_PERMISSIONS_SCOPES_GET_LIST = (
+        "slack",
+        "slack_apps_permissions_scopes_get_list",
+        False,
+    )
+    SLACK_APPS_PERMISSIONS_USERS_LIST_USER_GRANTS = (
+        "slack",
+        "slack_apps_permissions_users_list_user_grants",
+        False,
+    )
+    SLACK_APPS_PERMISSIONS_USERS_REQUEST_MODAL = (
+        "slack",
+        "slack_apps_permissions_users_request_modal",
+        False,
+    )
+    SLACK_APPS_UNINSTALL = ("slack", "slack_apps_uninstall", False)
+    SLACK_AU_TH_REVOKE = ("slack", "slack_au_th_revoke", False)
+    SLACK_AU_TH_TEST = ("slack", "slack_au_th_test", False)
+    SLACK_BOTS_INFO = ("slack", "slack_bots_info", False)
+    SLACK_CALLS_ADD = ("slack", "slack_calls_add", False)
+    SLACK_CALLS_END = ("slack", "slack_calls_end", False)
+    SLACK_CALLS_INFO = ("slack", "slack_calls_info", False)
+    SLACK_CALLS_PARTICIPANTS_ADD_NEW_PARTICIPANT = (
+        "slack",
+        "slack_calls_participants_add_new_participant",
+        False,
+    )
+    SLACK_CALLS_PARTICIPANTS_REGISTER_REMOVED = (
+        "slack",
+        "slack_calls_participants_register_removed",
+        False,
+    )
+    SLACK_CALLS_UPDATE = ("slack", "slack_calls_update", False)
+    SLACK_CHAT_DELETE = ("slack", "slack_chat_delete", False)
+    SLACK_CHAT_DELETE_SCHEDULED_MESSAGE = (
+        "slack",
+        "slack_chat_delete_scheduled_message",
+        False,
+    )
+    SLACK_CHAT_GET_PERMALINK = ("slack", "slack_chat_get_permalink", False)
+    SLACK_CHAT_ME_MESSAGE = ("slack", "slack_chat_me_message", False)
+    SLACK_CHAT_POST_EPHEMERAL = ("slack", "slack_chat_post_ephemeral", False)
+    SLACK_CHAT_POST_MESSAGE = ("slack", "slack_chat_post_message", False)
+    SLACK_CHAT_SCHEDULE_MESSAGE = ("slack", "slack_chat_schedule_message", False)
+    SLACK_CHAT_SCHEDULED_MESSAGES_LIST = (
+        "slack",
+        "slack_chat_scheduled_messages_list",
+        False,
+    )
+    SLACK_CHAT_UNFURL = ("slack", "slack_chat_unfurl", False)
+    SLACK_CHAT_UPDATE = ("slack", "slack_chat_update", False)
+    SLACK_CONVERSATIONS_ARCHIVE = ("slack", "slack_conversations_archive", False)
+    SLACK_CONVERSATIONS_CLOSE = ("slack", "slack_conversations_close", False)
+    SLACK_CONVERSATIONS_CREATE = ("slack", "slack_conversations_create", False)
+    SLACK_CONVERSATIONS_HISTORY = ("slack", "slack_conversations_history", False)
+    SLACK_CONVERSATIONS_INFO = ("slack", "slack_conversations_info", False)
+    SLACK_CONVERSATIONS_INVITE = ("slack", "slack_conversations_invite", False)
+    SLACK_CONVERSATIONS_JOIN = ("slack", "slack_conversations_join", False)
+    SLACK_CONVERSATIONS_KICK = ("slack", "slack_conversations_kick", False)
+    SLACK_CONVERSATIONS_LEAVE = ("slack", "slack_conversations_leave", False)
+    SLACK_CONVERSATIONS_LIST = ("slack", "slack_conversations_list", False)
+    SLACK_CONVERSATIONS_MARK = ("slack", "slack_conversations_mark", False)
+    SLACK_CONVERSATIONS_MEMBERS = ("slack", "slack_conversations_members", False)
+    SLACK_CONVERSATIONS_OPEN = ("slack", "slack_conversations_open", False)
+    SLACK_CONVERSATIONS_RENAME = ("slack", "slack_conversations_rename", False)
+    SLACK_CONVERSATIONS_REPLIES = ("slack", "slack_conversations_replies", False)
+    SLACK_CONVERSATIONS_SET_PURPOSE = (
+        "slack",
+        "slack_conversations_set_purpose",
+        False,
+    )
+    SLACK_CONVERSATIONS_SET_TOPIC = ("slack", "slack_conversations_set_topic", False)
+    SLACK_CONVERSATION_SUN_ARCHIVE = ("slack", "slack_conversation_sun_archive", False)
+    SLACK_DIALOG_OPEN = ("slack", "slack_dialog_open", False)
+    SLACK_DND_END_DND = ("slack", "slack_dnd_end_dnd", False)
+    SLACK_DND_END_SNOOZE = ("slack", "slack_dnd_end_snooze", False)
+    SLACK_DND_INFO = ("slack", "slack_dnd_info", False)
+    SLACK_DND_SET_SNOOZE = ("slack", "slack_dnd_set_snooze", False)
+    SLACK_DND_TEAM_INFO = ("slack", "slack_dnd_team_info", False)
+    SLACK_E_MOJI_LIST = ("slack", "slack_e_moji_list", False)
+    SLACK_FILES_COMMENTS_DELETE_COMMENT = (
+        "slack",
+        "slack_files_comments_delete_comment",
+        False,
+    )
+    SLACK_FILES_DELETE = ("slack", "slack_files_delete", False)
+    SLACK_FILES_INFO = ("slack", "slack_files_info", False)
+    SLACK_FILES_LIST = ("slack", "slack_files_list", False)
+    SLACK_FILES_REMOTE_ADD_FROM_REMOTE = (
+        "slack",
+        "slack_files_remote_add_from_remote",
+        False,
+    )
+    SLACK_FILES_REMOTE_GET_INFO = ("slack", "slack_files_remote_get_info", False)
+    SLACK_FILES_REMOTE_LIST_REMOTE_FILES = (
+        "slack",
+        "slack_files_remote_list_remote_files",
+        False,
+    )
+    SLACK_FILES_REMOTE_DELETE_FILE = ("slack", "slack_files_remote_delete_file", False)
+    SLACK_FILES_REMOTE_SHARE_REMOTE_FILE = (
+        "slack",
+        "slack_files_remote_share_remote_file",
+        False,
+    )
+    SLACK_FILES_REMOTE_UPDATE_REMOTE_FILE = (
+        "slack",
+        "slack_files_remote_update_remote_file",
+        False,
+    )
+    SLACK_FILES_REVOKE_PUBLIC_URL = ("slack", "slack_files_revoke_public_url", False)
+    SLACK_FILES_SHARED_PUBLIC_URL = ("slack", "slack_files_shared_public_url", False)
+    SLACK_FILES_UPLOAD = ("slack", "slack_files_upload", False)
+    SLACK_MIGRATION_EXCHANGE = ("slack", "slack_migration_exchange", False)
+    SLACK_OAUTH_ACCESS = ("slack", "slack_oauth_access", False)
+    SLACK_OAUTH_TOKEN = ("slack", "slack_oauth_token", False)
+    SLACK_OAUTH_V_2_EXCHANGE_TOKEN = ("slack", "slack_oauth_v_2_exchange_token", False)
+    SLACK_PINS_ADD = ("slack", "slack_pins_add", False)
+    SLACK_PINS_LIST = ("slack", "slack_pins_list", False)
+    SLACK_PINS_REMOVE = ("slack", "slack_pins_remove", False)
+    SLACK_REACTIONS_ADD = ("slack", "slack_reactions_add", False)
+    SLACK_REACTIONS_GET = ("slack", "slack_reactions_get", False)
+    SLACK_REACTIONS_LIST = ("slack", "slack_reactions_list", False)
+    SLACK_REACTIONS_REMOVE = ("slack", "slack_reactions_remove", False)
+    SLACK_REMINDERS_ADD = ("slack", "slack_reminders_add", False)
+    SLACK_REMINDERS_COMPLETE = ("slack", "slack_reminders_complete", False)
+    SLACK_REMINDERS_DELETE = ("slack", "slack_reminders_delete", False)
+    SLACK_REMINDERS_INFO = ("slack", "slack_reminders_info", False)
+    SLACK_REMINDERS_LIST = ("slack", "slack_reminders_list", False)
+    SLACK_RT_M_CONNECT = ("slack", "slack_rt_m_connect", False)
+    SLACK_SEARCH_MESSAGES = ("slack", "slack_search_messages", False)
+    SLACK_STARS_ADD = ("slack", "slack_stars_add", False)
+    SLACK_STARS_LIST = ("slack", "slack_stars_list", False)
+    SLACK_STARS_REMOVE = ("slack", "slack_stars_remove", False)
+    SLACK_TEAM_ACCESS_LOGS = ("slack", "slack_team_access_logs", False)
+    SLACK_TEAMBILL_ABLE_INFO = ("slack", "slack_teambill_able_info", False)
+    SLACK_TEAM_INFO = ("slack", "slack_team_info", False)
+    SLACK_TEAM_INTEGRATION_LOGS = ("slack", "slack_team_integration_logs", False)
+    SLACK_TEAM_PROFILE_GET_PROFILE = ("slack", "slack_team_profile_get_profile", False)
+    SLACK_USER_GROUPS_CREATE = ("slack", "slack_user_groups_create", False)
+    SLACK_USER_GROUPS_DISABLE = ("slack", "slack_user_groups_disable", False)
+    SLACK_USER_GROUPS_ENABLE = ("slack", "slack_user_groups_enable", False)
+    SLACK_USER_GROUPS_LIST = ("slack", "slack_user_groups_list", False)
+    SLACK_USER_GROUPS_UPDATE = ("slack", "slack_user_groups_update", False)
+    SLACK_USER_GROUPS_USERS_LIST_ALL_USERS = (
+        "slack",
+        "slack_user_groups_users_list_all_users",
+        False,
+    )
+    SLACK_USER_GROUPS_USERS_UPDATE_LIST = (
+        "slack",
+        "slack_user_groups_users_update_list",
+        False,
+    )
+    SLACK_USERS_CONVERSATIONS = ("slack", "slack_users_conversations", False)
+    SLACK_USERS_DELETE_PHOTO = ("slack", "slack_users_delete_photo", False)
+    SLACK_USERS_GET_PRESENCE = ("slack", "slack_users_get_presence", False)
+    SLACK_USERS_IDENTITY = ("slack", "slack_users_identity", False)
+    SLACK_USERS_INFO = ("slack", "slack_users_info", False)
+    SLACK_USERS_LIST = ("slack", "slack_users_list", False)
+    SLACK_USERS_LOOKUP_BY_EMAIL = ("slack", "slack_users_lookup_by_email", False)
+    SLACK_USERS_PROFILE_GET_PROFILE_INFO = (
+        "slack",
+        "slack_users_profile_get_profile_info",
+        False,
+    )
+    SLACK_USERS_PROFILE_SET_PROFILE_INFO = (
+        "slack",
+        "slack_users_profile_set_profile_info",
+        False,
+    )
+    SLACK_USERS_SET_ACTIVE = ("slack", "slack_users_set_active", False)
+    SLACK_USERS_SET_PHOTO = ("slack", "slack_users_set_photo", False)
+    SLACK_USERS_SET_PRESENCE = ("slack", "slack_users_set_presence", False)
+    SLACK_VIEWS_OPEN = ("slack", "slack_views_open", False)
+    SLACK_VIEWS_PUBLISH = ("slack", "slack_views_publish", False)
+    SLACK_VIEWS_PUSH = ("slack", "slack_views_push", False)
+    SLACK_VIEWS_UPDATE = ("slack", "slack_views_update", False)
+    SLACK_WORK_FLOWS_STEP_COMPLETED = (
+        "slack",
+        "slack_work_flows_step_completed",
+        False,
+    )
+    SLACK_WORK_FLOWS_STEP_FAILED = ("slack", "slack_work_flows_step_failed", False)
+    SLACK_WORK_FLOWS_UPDATE_STEP = ("slack", "slack_work_flows_update_step", False)
     SLACKBOT_SEND_SLACK_MESSAGE = ("slackbot", "slackbot_send_slack_message", False)
     SLACKBOT_LIST_SLACK_CHANNELS = ("slackbot", "slackbot_list_slack_channels", False)
     SLACKBOT_LIST_SLACK_MEMBERS = ("slackbot", "slackbot_list_slack_members", False)
     SLACKBOT_LIST_SLACK_MESSAGES = ("slackbot", "slackbot_list_slack_messages", False)
     SNOWFLAKE_RUN_QUERY = ("snowflake", "snowflake_run_query", False)
     SNOWFLAKE_SHOW_TABLES = ("snowflake", "snowflake_show_tables", False)
     SNOWFLAKE_DESCRIBE_TABLE = ("snowflake", "snowflake_describe_table", False)
@@ -6156,8 +6688,12 @@
     def event(self) -> str:
         """Event name."""
         return self.value[1]
 
     GITHUB_PULL_REQUEST_EVENT = ("github", "github_pull_request_event")
     GITHUB_COMMIT_EVENT = ("github", "github_commit_event")
     SLACK_NEW_MESSAGE = ("slack", "slack_receive_message")
+    SLACK_THREAD_REPLY = ("slack", "slack_receive_thread_reply")
+    SLACK_REACTION_REMOVED = ("slack", "slack_reaction_removed")
+    SLACK_REACTION_ADDED = ("slack", "slack_reaction_added")
+    SLACK_NEW_CHANNEL_CREATED = ("slack", "slack_channel_created")
     SLACKBOT_NEW_MESSAGE = ("slackbot", "slackbot_receive_message")
```

### Comparing `composio_core-0.3.1/composio/client/exceptions.py` & `composio_core-0.3.2/composio/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/client/http.py` & `composio_core-0.3.2/composio/client/http.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/client/local_handler.py` & `composio_core-0.3.2/composio/client/local_handler.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/constants.py` & `composio_core-0.3.2/composio/constants.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/exceptions.py` & `composio_core-0.3.2/composio/exceptions.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/action.py` & `composio_core-0.3.2/composio/local_tools/action.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/file/tool.py` & `composio_core-0.3.2/composio/local_tools/file/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     workspace_factory: WorkspaceManagerFactory = None
     history_processor: HistoryProcessor = None
 
     def __init__(self):
         super().__init__()
         self.name = "agent"
         self.logger = logger
-        self.config_file_path = Path(CONFIG_FILE_PATH)
+        self.config_file_path = ""
         self.args = None
         self.workspace_id = ""
         # set self.command --> it is used by history-processor to record the command as part of history
         self.command = ""
         self.image_name = ""
         self.container_name = ""
         self.container_process = None
@@ -94,14 +94,15 @@
     ):
         self.workspace_factory = workspace_factory
         self.history_processor = history_processor
 
     def _setup(self, args: RunCommandOnWorkspaceRequest):
         self.args = args
         self.workspace_id = args.workspace_id
+        self.config_file_path = Path(CONFIG_FILE_PATH)
         # set self.command --> it is used by history-processor to record the command as part of history
         self.command = args.input_cmd
         workspace_meta = get_workspace_meta_from_manager(
             self.workspace_factory, self.workspace_id
         )
         self.image_name = workspace_meta[KEY_IMAGE_NAME]
         self.container_name = workspace_meta[KEY_CONTAINER_NAME]
```

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     script_file = SCRIPT_CURSOR_DEFAULT
     command = "set_cursors"
     workspace_factory: WorkspaceManagerFactory = None
     history_processor: HistoryProcessor = None
 
     def __init__(self):
         super().__init__()
-        super().__init__()
         self.args = None
         self.workspace_id = ""
         self.image_name = ""
         self.container_name = ""
         self.container_process = None
         self.parent_pids = []
         self.container_obj = None
```

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/commons/command_runner_model.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/commons/command_runner_model.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/commons/history_processor.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/commons/history_processor.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/commons/local_docker_workspace.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/commons/local_docker_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/commons/parsing.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/commons/parsing.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/commons/utils.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/commons/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/create_workspace.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/create_workspace.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         self.repo_name = REPO_NAME
         self.image_name = ""
         self.container_name = ""
         self.container_process = None
         self.parent_pids = []
         self.container_obj = None
         self.logger = logger
-        self._github_token = self.load_github_token_from_host_env()
         self.repo_type = "not_local"
 
     def _setup(self, args: SetupGithubRepoRequest):
         self.args = args
         self.workspace_id = args.workspace_id
         workspace_meta = get_workspace_meta_from_manager(
             self.workspace_factory, self.workspace_id
@@ -80,14 +79,15 @@
         )
         self.parent_pids = workspace_meta[KEY_PARENT_PIDS]
         self.container_obj = self.get_container_by_container_name()
         if not self.container_obj:
             raise ValueError(
                 f"container-name {self.container_name} is not a valid docker-container"
             )
+        self._github_token = self.load_github_token_from_host_env()
 
     def set_workspace_and_history(
         self,
         workspace_factory: WorkspaceManagerFactory,
         history_processor: HistoryProcessor,
     ):
         self.workspace_factory = workspace_factory
```

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,19 +137,17 @@
         if not self.config and self.config_file_path is not None:
             # If unassigned, we load the config from the file to store its contents with the overall arguments
             config = AgentConfig.load_yaml(self.config_file_path)
             object.__setattr__(self, "config", config)
         assert self.config is not None  # mypy
 
     def set_env_variables(self):
-        commands_to_execute = (
-            [self.config.state_command.code]
-            + ["pip install flake8"]
-            + [f"{k}={v}" for k, v in self.config.env_variables.items()]
-        )
+        commands_to_execute = [self.config.state_command.code] + [
+            f"{k}={v}" for k, v in self.config.env_variables.items()
+        ]
         commands = "\n".join(commands_to_execute)
         return_code = 0
         output = None
         try:
             output, return_code = communicate(
                 self.container_process, self.container_obj, commands, self.parent_pids
             )
```

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/workspace/actions/workspace_status.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/actions/workspace_status.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/local_workspace/workspace/workspace_tool.py` & `composio_core-0.3.2/composio/local_tools/local_workspace/workspace/workspace_tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/mathematical/calculator.py` & `composio_core-0.3.2/composio/local_tools/mathematical/calculator.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/local_tools/tool.py` & `composio_core-0.3.2/composio/local_tools/tool.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/storage/base.py` & `composio_core-0.3.2/composio/storage/base.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/tools/__init__.py` & `composio_core-0.3.2/composio/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/tools/schema.py` & `composio_core-0.3.2/composio/tools/schema.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/utils/decorators.py` & `composio_core-0.3.2/composio/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/utils/git.py` & `composio_core-0.3.2/composio/utils/git.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/utils/shared.py` & `composio_core-0.3.2/composio/utils/shared.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio/utils/url.py` & `composio_core-0.3.2/composio/utils/url.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/composio_core.egg-info/PKG-INFO` & `composio_core-0.3.2/composio_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.3.1
+Version: 0.3.2
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.3.1/composio_core.egg-info/SOURCES.txt` & `composio_core-0.3.2/composio_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composio_core-0.3.1/setup.py` & `composio_core-0.3.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from pathlib import Path
 from setuptools import setup
 from setuptools import setup, find_packages
 
 setup(
     name="composio_core",
-    version="0.3.1",
+    version="0.3.2",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

