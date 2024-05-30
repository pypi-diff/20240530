# Comparing `tmp/tinybird-cli-4.0.2.dev0.tar.gz` & `tmp/tinybird-cli-4.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-4.0.2.dev0.tar", last modified: Wed May 29 11:11:20 2024, max compression
+gzip compressed data, was "tinybird-cli-4.0.3.dev0.tar", last modified: Thu May 30 14:12:19 2024, max compression
```

## Comparing `tinybird-cli-4.0.2.dev0.tar` & `tinybird-cli-4.0.3.dev0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/
--rw-r--r--   0 root         (0) root         (0)    70608 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 11:11:20.228909 tinybird-cli-4.0.2.dev0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.225909 tinybird-cli-4.0.2.dev0/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-29 11:11:18.000000 tinybird-cli-4.0.2.dev0/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.225909 tinybird-cli-4.0.2.dev0/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46918 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   210873 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    60657 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41589 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    81800 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11523 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.226909 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    38296 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    13910 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64576 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78632 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    32368 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31968 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26132 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    11064 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-05-29 11:11:13.000000 tinybird-cli-4.0.2.dev0/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 11:11:20.227909 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    70608 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-29 11:11:20.000000 tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:12:19.418952 tinybird-cli-4.0.3.dev0/
+-rw-r--r--   0 root         (0) root         (0)    70711 2024-05-30 14:12:19.418952 tinybird-cli-4.0.3.dev0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 14:12:19.418952 tinybird-cli-4.0.3.dev0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:12:19.414952 tinybird-cli-4.0.3.dev0/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-30 14:12:18.000000 tinybird-cli-4.0.3.dev0/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:12:19.414952 tinybird-cli-4.0.3.dev0/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46918 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   210873 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    60657 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41589 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    81800 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11523 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:12:19.416952 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    38296 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    13910 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64576 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78632 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    32368 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31968 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26132 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:12:19.417952 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    11064 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-05-30 14:12:13.000000 tinybird-cli-4.0.3.dev0/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 14:12:19.417952 tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    70711 2024-05-30 14:12:19.000000 tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-30 14:12:19.000000 tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 14:12:19.000000 tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-30 14:12:19.000000 tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-30 14:12:19.000000 tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-30 14:12:19.000000 tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-4.0.2.dev0/PKG-INFO` & `tinybird-cli-4.0.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 4.0.2.dev0
+Version: 4.0.3.dev0
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,14 +14,20 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ----------
 
+4.0.3.dev0
+************
+
+- `Fixed` Pin `tinybird-cli>=4,<5` in `requirements.txt` on `tb init --git`
+
+
 4.0.0
 ************
 
 This is a major release, please read the commands affected below and consider updating your scripts and workflow before upgrading to these version.
 
 - `Deprecated` `--semver` flag and `tb release` commands are now deprecated. You can keep using `tb deploy` to integrate and deploy from git. Changes are deployed to the main Workspace instead of to a Release.
 - `Removed` `--cicd` flag and CI/CD templates generation from `tb init`. You can still use the git integration, just create your own pipelines. You can use the ones in this repo as an exmple https://github.com/tinybirdco/ci
```

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/ch_utils/constants.py` & `tinybird-cli-4.0.3.dev0/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/ch_utils/engine.py` & `tinybird-cli-4.0.3.dev0/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/check_pypi.py` & `tinybird-cli-4.0.3.dev0/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/client.py` & `tinybird-cli-4.0.3.dev0/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/config.py` & `tinybird-cli-4.0.3.dev0/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/connectors.py` & `tinybird-cli-4.0.3.dev0/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/context.py` & `tinybird-cli-4.0.3.dev0/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/datafile.py` & `tinybird-cli-4.0.3.dev0/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/datatypes.py` & `tinybird-cli-4.0.3.dev0/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/feedback_manager.py` & `tinybird-cli-4.0.3.dev0/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/git_settings.py` & `tinybird-cli-4.0.3.dev0/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/sql.py` & `tinybird-cli-4.0.3.dev0/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/sql_template.py` & `tinybird-cli-4.0.3.dev0/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/sql_template_fmt.py` & `tinybird-cli-4.0.3.dev0/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/sql_toolset.py` & `tinybird-cli-4.0.3.dev0/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/syncasync.py` & `tinybird-cli-4.0.3.dev0/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/cicd.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class Provider(Enum):
     GitHub = 0
     GitLab = 1
 
 
 WORKFLOW_VERSION = "v3.1.0"
 
-DEFAULT_REQUIREMENTS_FILE = "tinybird-cli>=3,<4"
+DEFAULT_REQUIREMENTS_FILE = "tinybird-cli>=4,<5"
 
 GITHUB_CI_YML = """
     ##################################################
     ###   Visit https://github.com/tinybirdco/ci   ###
     ###   for more details or custom CI/CD         ###
     ##################################################
```

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/common.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/config.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/job.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/test.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/token.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-4.0.3.dev0/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird/tornado_template.py` & `tinybird-cli-4.0.3.dev0/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 4.0.2.dev0
+Version: 4.0.3.dev0
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,14 +14,20 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ----------
 
+4.0.3.dev0
+************
+
+- `Fixed` Pin `tinybird-cli>=4,<5` in `requirements.txt` on `tb init --git`
+
+
 4.0.0
 ************
 
 This is a major release, please read the commands affected below and consider updating your scripts and workflow before upgrading to these version.
 
 - `Deprecated` `--semver` flag and `tb release` commands are now deprecated. You can keep using `tb deploy` to integrate and deploy from git. Changes are deployed to the main Workspace instead of to a Release.
 - `Removed` `--cicd` flag and CI/CD templates generation from `tb init`. You can still use the git integration, just create your own pipelines. You can use the ones in this repo as an exmple https://github.com/tinybirdco/ci
```

### Comparing `tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-4.0.2.dev0/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-4.0.3.dev0/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

