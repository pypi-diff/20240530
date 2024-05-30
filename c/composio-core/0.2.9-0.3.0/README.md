# Comparing `tmp/composio_core-0.2.9.tar.gz` & `tmp/composio_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.2.9.tar", last modified: Thu Apr 18 18:49:37 2024, max compression
+gzip compressed data, was "composio_core-0.3.0.tar", last modified: Thu May 30 03:50:37 2024, max compression
```

## Comparing `composio_core-0.2.9.tar` & `composio_core-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,99 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.098840 composio_core-0.2.9/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-15 07:39:40.000000 composio_core-0.2.9/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:49:37.098646 composio_core-0.2.9/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-15 07:39:40.000000 composio_core-0.2.9/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.094983 composio_core-0.2.9/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      159 2024-04-15 07:39:40.000000 composio_core-0.2.9/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    22112 2024-04-18 18:43:06.000000 composio_core-0.2.9/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.097376 composio_core-0.2.9/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-15 07:39:40.000000 composio_core-0.2.9/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7018 2024-04-16 18:37:25.000000 composio_core-0.2.9/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    10226 2024-04-16 18:39:17.000000 composio_core-0.2.9/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    22118 2024-04-18 18:43:44.000000 composio_core-0.2.9/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)        0 2024-04-15 07:39:40.000000 composio_core-0.2.9/composio/sdk/shared.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1358 2024-04-16 16:08:42.000000 composio_core-0.2.9/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3455 2024-04-16 17:03:02.000000 composio_core-0.2.9/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:37.098444 composio_core-0.2.9/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      796 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      489 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      103 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-18 18:49:37.000000 composio_core-0.2.9/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      528 2024-04-15 07:39:40.000000 composio_core-0.2.9/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)      130 2024-04-15 07:39:40.000000 composio_core-0.2.9/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:49:37.098876 composio_core-0.2.9/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1127 2024-04-18 18:44:03.000000 composio_core-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.567452 composio_core-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-30 03:50:21.000000 composio_core-0.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-30 03:50:37.567452 composio_core-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-30 03:50:21.000000 composio_core-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.555452 composio_core-0.3.0/composio/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.555452 composio_core-0.3.0/composio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/add.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7910 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/cli/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.559452 composio_core-0.3.0/composio/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    31184 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/client/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)   213764 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/client/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/client/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/client/local_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.559452 composio_core-0.3.0/composio/local_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.559452 composio_core-0.3.0/composio/local_tools/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/file/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.559452 composio_core-0.3.0/composio/local_tools/local_workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.559452 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.559452 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/edit_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/scroll_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/search_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/actions/set_cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/cmd_manager/cmd_manager_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.563452 composio_core-0.3.0/composio/local_tools/local_workspace/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/commons/command_runner_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/commons/get_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/commons/history_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/commons/local_docker_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/commons/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.563452 composio_core-0.3.0/composio/local_tools/local_workspace/history_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/history_keeper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.563452 composio_core-0.3.0/composio/local_tools/local_workspace/history_keeper/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/history_keeper/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/history_keeper/actions/get_workspace_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/history_keeper/history_keeper_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.563452 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.563452 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/actions/create_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/actions/setup_github_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/actions/workspace_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/actions/workspace_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/local_workspace/workspace/workspace_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.563452 composio_core-0.3.0/composio/local_tools/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/mathematical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/mathematical/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/mathematical/mathematical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/local_tools/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.567452 composio_core-0.3.0/composio/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/storage/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.567452 composio_core-0.3.0/composio/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.567452 composio_core-0.3.0/composio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/utils/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-30 03:50:21.000000 composio_core-0.3.0/composio/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 03:50:37.567452 composio_core-0.3.0/composio_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-30 03:50:37.000000 composio_core-0.3.0/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-30 03:50:37.000000 composio_core-0.3.0/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 03:50:37.000000 composio_core-0.3.0/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 03:50:37.000000 composio_core-0.3.0/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 03:50:37.000000 composio_core-0.3.0/composio_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 03:50:37.000000 composio_core-0.3.0/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 03:50:37.567452 composio_core-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-30 03:50:21.000000 composio_core-0.3.0/setup.py
```

