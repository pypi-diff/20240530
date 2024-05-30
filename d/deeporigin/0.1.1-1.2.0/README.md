# Comparing `tmp/deeporigin-0.1.1.tar.gz` & `tmp/deeporigin-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeporigin-0.1.1.tar", last modified: Fri May 17 14:42:06 2024, max compression
+gzip compressed data, was "deeporigin-1.2.0.tar", last modified: Thu May 30 02:00:10 2024, max compression
```

## Comparing `deeporigin-0.1.1.tar` & `deeporigin-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.937538 deeporigin-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 14:42:03.000000 deeporigin-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 14:42:03.000000 deeporigin-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-17 14:42:06.937538 deeporigin-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 14:42:03.000000 deeporigin-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.933538 deeporigin-0.1.1/deeporigin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 14:42:03.000000 deeporigin-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:42:06.937538 deeporigin-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 14:42:04.000000 deeporigin-0.1.1/src/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/config/default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/feature_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/managed_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/base_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20138 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.933538 deeporigin-0.1.1/src/variables/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/anthropic_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/git_http_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/gurobi_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/mosek_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/open_ai_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/private_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/private_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_env_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_file_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/xpress_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.933538 deeporigin-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_cli_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_managed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    89806 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.995851 deeporigin-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 02:00:03.000000 deeporigin-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 02:00:03.000000 deeporigin-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-30 02:00:09.995851 deeporigin-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-30 02:00:03.000000 deeporigin-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.995851 deeporigin-1.2.0/deeporigin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-30 02:00:09.000000 deeporigin-1.2.0/deeporigin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-30 02:00:09.000000 deeporigin-1.2.0/deeporigin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:00:09.000000 deeporigin-1.2.0/deeporigin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 02:00:09.000000 deeporigin-1.2.0/deeporigin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-30 02:00:09.000000 deeporigin-1.2.0/deeporigin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 02:00:09.000000 deeporigin-1.2.0/deeporigin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-30 02:00:03.000000 deeporigin-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 02:00:09.995851 deeporigin-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.987851 deeporigin-1.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 02:00:07.000000 deeporigin-1.2.0/src/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.987851 deeporigin-1.2.0/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.987851 deeporigin-1.2.0/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/config/default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/feature_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.991850 deeporigin-1.2.0/src/managed_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/managed_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/managed_data/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17308 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/managed_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/managed_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/managed_data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.991850 deeporigin-1.2.0/src/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/base_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20138 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.991850 deeporigin-1.2.0/src/variables/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/anthropic_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/git_http_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/gurobi_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/mosek_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/open_ai_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/private_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/private_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/secret_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/secret_env_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/secret_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/secret_file_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/variables/types/xpress_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 02:00:03.000000 deeporigin-1.2.0/src/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:00:09.995851 deeporigin-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-30 02:00:03.000000 deeporigin-1.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-30 02:00:03.000000 deeporigin-1.2.0/tests/test_cli_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-30 02:00:03.000000 deeporigin-1.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-30 02:00:03.000000 deeporigin-1.2.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-30 02:00:03.000000 deeporigin-1.2.0/tests/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-30 02:00:03.000000 deeporigin-1.2.0/tests/test_managed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89806 2024-05-30 02:00:03.000000 deeporigin-1.2.0/tests/test_variables.py
```

### Comparing `deeporigin-0.1.1/LICENSE.txt` & `deeporigin-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/README.md` & `deeporigin-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 python client, which allows you to interact with 
 Deep Origin from the command line. 
 
 > [!WARNING]  
 > The `deeporigin` client is under active development. Features
 > may change, or be removed. 
 
-## Installation 
+## Installing 
 
 > [!CAUTION]
 > As a best practice, we recommend  installing this in a virtual environment. 
 
-### For end users
 
 ```bash
 pip install deeporigin
 ```
 
-### For developers
+## Developing 
 
 First, download from Github:
 
 ```bash
 git clone git@github.com:formiclabs/deeporigin-client.git
 cd deeporigin-client
 ```
```

### Comparing `deeporigin-0.1.1/deeporigin.egg-info/SOURCES.txt` & `deeporigin-1.2.0/deeporigin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/pyproject.toml` & `deeporigin-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name = "deeporigin"
 description = "Command line tool and Python client for working with Deep Origin"
 authors = [
     {name = "Deep Origin", email = "support@deeporigin.com"},
 ]
+readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
 ]
@@ -20,28 +21,35 @@
     "pyyaml",
     "requests",
     "termcolor",
     "validators",
     "pandas",
     "beartype",
     "tabulate",
+    "filetype",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "parameterized",
     "coverage",
     "interrogate",
 ]
-jupyter = ["ipykernel"]
-
-docs=["mkdocs", "mkdocs-material-extensions", "mkdocs-material", "mkdocstrings" ,"mkdocstrings-python","mkdocs-git-revision-date-localized-plugin","black"]
+jupyter = ["ipykernel","jupyter-black"]
 
+docs = ["mkdocs", 
+    "mkdocs-material-extensions", 
+    "mkdocs-material", 
+    "mkdocstrings",
+    "mkdocstrings-python",
+    "mkdocs-git-revision-date-localized-plugin",
+    "black"
+]
 
 [tool.setuptools]
 package-dir = {"deeporigin" = "src"}
 include-package-data = true
 
 [tool.setuptools.dynamic]
 version = {file = ["src/VERSION"]}
```

### Comparing `deeporigin-0.1.1/src/__init__.py` & `deeporigin-1.2.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/auth.py` & `deeporigin-1.2.0/src/auth.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/cli/__init__.py` & `deeporigin-1.2.0/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/cli/context.py` & `deeporigin-1.2.0/src/cli/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/cli/data.py` & `deeporigin-1.2.0/src/cli/data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/cli/variables.py` & `deeporigin-1.2.0/src/cli/variables.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/config/__init__.py` & `deeporigin-1.2.0/src/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/config/default.yml` & `deeporigin-1.2.0/src/config/default.yml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/context.py` & `deeporigin-1.2.0/src/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/feature_flags.py` & `deeporigin-1.2.0/src/feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/managed_data/_api.py` & `deeporigin-1.2.0/src/managed_data/_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """The `deeporigin.managed_data._api` module contains low-level functions for interacting
 with Deep Origin's managed data API. The functions in this module
 simply provide Pythonic interfaces to individual API endpoints."""
 
+import mimetypes
 import os
 from typing import Optional, Union
+from urllib.parse import parse_qs, urlparse, urlunparse
 
-import requests
 from beartype import beartype
 from deeporigin.exceptions import DeepOriginException
 from deeporigin.managed_data.client import Client, DeepOriginClient
 from deeporigin.managed_data.schema import (
     Cardinality,
     DataType,
     RowType,
 )
 
 
+@beartype
 def _get_default_client(client: Optional[Client] = None):
     """Internal function to instantiate client
 
     Creates and returns an authenticated client if
     not provided with one.
 
     Warning: Internal function
@@ -33,14 +35,197 @@
     if client is None:
         client = DeepOriginClient()  # pragma: no cover
         client.authenticate()  # pragma: no cover
     return client
 
 
 @beartype
+def assign_files_to_cell(
+    *,
+    file_ids: list[str],
+    database_id: str,
+    column_id: str,
+    row_id: Optional[str] = None,
+    client: Optional[Client] = None,
+) -> dict:
+    """Assign existing file(s) to a cell
+
+    Assign files to a cell in a database table, where the cell is identified by the database ID, row ID, and column ID. If row_id is None, a new row will be created.
+
+    Args:
+    file_id: ID of the file
+    column_id: ID of the column
+    row_id: ID of the row
+
+
+    """
+    client = _get_default_client(client)
+
+    if row_id is None:
+        data = make_database_rows(
+            database_id=database_id,
+            n_rows=1,
+            client=client,
+        )
+        row_id = data["rows"][0]["id"]
+
+    data = {
+        "databaseId": database_id,
+        "rows": [
+            {
+                "rowId": row_id,
+                "row": {},
+                "cells": [
+                    {
+                        "columnId": column_id,
+                        "value": {"fileIds": file_ids},
+                    },
+                ],
+            },
+        ],
+    }
+
+    return client.invoke("EnsureRows", data)
+
+
+@beartype
+def make_database_rows(
+    database_id: str,
+    n_rows: int = 1,
+    client: Optional[Client] = None,
+) -> dict:
+    """Makes one or several new row(s) in a Database table
+
+    This wraps the `EnsureRows` endpoint and sends a payload
+    designed to create new row(s) in a database table.
+
+
+    Args:
+        database_id: ID or Human ID of the database
+
+    Returns:
+        A dictionary that conforms to a [EnsureRowsResponse][src.managed_data.schema.EnsureRowsResponse]
+    """
+
+    client = _get_default_client(client)
+
+    if n_rows < 1:
+        raise DeepOriginException(
+            f"n_rows must be at least 1. However, n_rows was {n_rows}"
+        )
+
+    data = dict(
+        databaseId=database_id,
+        rows=[{"row": {}} for _ in range(n_rows)],
+    )
+
+    return client.invoke("EnsureRows", data)
+
+
+def upload_file(
+    file_path: str,
+    client: Optional[Client] = None,
+) -> None:
+    """Upload a file to Deep Origin."""
+
+    client = _get_default_client(client)
+
+    # attempt to guess the content type
+    mime_type, _ = mimetypes.guess_type(file_path)
+    content_type = mime_type if mime_type else "application/octet-stream"
+
+    content_length = os.path.getsize(file_path)
+
+    response = create_file_upload_url(
+        name=os.path.basename(file_path),
+        content_type=content_type,
+        content_length=content_length,
+    )
+
+    # extract pre-signed URL to upload to
+    url = urlparse(response["uploadUrl"])
+    url = urlunparse((url.scheme, url.netloc, url.path, "", "", ""))
+
+    # extract params
+    params = _parse_params_from_url(response["uploadUrl"])
+
+    headers = {
+        "Accept": "application/json, text/plain, */*",
+        "Connection": "keep-alive",
+        "Content-Length": str(content_length),
+        "Content-Type": content_type,
+    }
+
+    with open(file_path, "rb") as file:
+        put_response = client.put(
+            url,
+            headers=headers,
+            params=params,
+            data=file,
+        )
+
+        if put_response.status_code != 200:
+            raise DeepOriginException("Error uploading file")
+
+    return response["file"]
+
+
+@beartype
+def _parse_params_from_url(url: str) -> dict:
+    """utility function to extract params from a URL query
+
+    Warning: Internal function
+        Do not use this function
+
+    Args:
+        url: URL
+
+    Returns:
+        A dictionary of params
+    """
+
+    query = urlparse(url).query
+    params = parse_qs(query)
+    params = {key: value[0] for key, value in params.items()}
+    return params
+
+
+@beartype
+def create_file_upload_url(
+    *,
+    name: str,
+    content_type: str,
+    content_length: int,
+    client: Optional[Client] = None,
+) -> dict:
+    """low level function that wraps the `CreateFileUpload` endpoint.
+
+    Creates a new file upload URL.
+
+    Args:
+        name: Name of the file
+        content_type: Content type of the file
+        content_length: Content length of the file
+
+    Returns:
+        A dictionary that conforms to a [CreateFileUploadResponse][src.managed_data.schema.CreateFileUploadResponse]
+    """
+
+    client = _get_default_client(client)
+
+    data = {
+        "name": name,
+        "contentType": content_type,
+        "contentLength": str(content_length),
+    }
+
+    return client.invoke("CreateFileUpload", data)
+
+
+@beartype
 def create_workspace(
     *,
     name: str,
     hid: Optional[str] = None,
     parent_id: Optional[str] = None,
     client: Optional[Client] = None,
 ) -> dict:
@@ -525,20 +710,15 @@
 
     file_name = describe_file(file_id, client=client)["name"]
 
     url = create_file_download_url(file_id, client=client)["downloadUrl"]
 
     save_path = os.path.join(destination, file_name)
 
-    response = requests.get(url)
-    if response.status_code == 200:
-        with open(save_path, "wb") as file:
-            file.write(response.content)
-    else:
-        raise DeepOriginException(f"Failed to download file {file_id}")
+    client.download(url, save_path)
 
 
 @beartype
 def convert_id_format(
     *,
     hids: Optional[Union[list[str], set[str]]] = None,
     ids: Optional[Union[list[str], set[str]]] = None,
```

### Comparing `deeporigin-0.1.1/src/managed_data/api.py` & `deeporigin-1.2.0/src/managed_data/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,50 @@
 from deeporigin.managed_data import _api
 from deeporigin.managed_data.client import Client
 from deeporigin.managed_data.schema import DatabaseReturnType, IDFormat
 from deeporigin.utils import PREFIXES
 
 
 @beartype
+def upload_file_to_new_database_row(
+    *,
+    database_id: str,
+    file_path: str,
+    column_id: str,
+    client: Optional[Client] = None,
+):
+    """Upload a file to a new row in a database.
+
+    Upload a file to a new row in a database. This utility function
+    wraps two level functions:
+
+        - [upload_file][src.managed_data.api.upload_file]
+        - [assign_files_to_cell][src.managed_data.api.assign_files_to_cell]
+
+    Args:
+        database_id: ID (or human ID) of a database.
+        file_path: Path to the file to upload.
+        column_id: ID (or human ID) of a column in the database.
+
+    """
+    # upload file
+    response = _api.upload_file(file_path, client=client)
+    file_id = response["id"]
+
+    # assign file to column
+    # we're not specifying row_id, which will create a new row
+    return _api.assign_files_to_cell(
+        file_ids=[file_id],
+        database_id=database_id,
+        column_id=column_id,
+        client=client,
+    )
+
+
+@beartype
 def get_tree(
     *,
     include_rows: bool = True,
     client: Optional[Client] = None,
 ) -> list[dict]:
     """Construct a tree of all workspaces, databases and rows.
 
@@ -258,14 +294,17 @@
     file_ids = []
     reference_ids = []
 
     for column in columns:
         data[column["id"]] = []
 
     for row in rows:
+        if "fields" not in row.keys():
+            continue
+
         data[row_id].append(row["hid"])
         data["Validation Status"].append(row["validationStatus"])
 
         fields = row["fields"]
 
         for column in columns:
             value = _parse_column_value(
```

### Comparing `deeporigin-0.1.1/src/managed_data/schema.py` & `deeporigin-1.2.0/src/managed_data/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     name: str
     parentId: str = "placeholder"  # sometimes not returned
     dateCreated: str
     dateUpdated: str
     createdByUserDrn: str
     hid: str
     hidPrefix: str
-    cols: list
+    cols: list = []
     rowJsonSchema: dict = dict()
 
     model_config = ConfigDict(extra="forbid")
 
 
 class CreateWorkspaceResponse(BaseModel):
     """Schema for responses from the
```

### Comparing `deeporigin-0.1.1/src/utils.py` & `deeporigin-1.2.0/src/utils.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/base_type.py` & `deeporigin-1.2.0/src/variables/base_type.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/core.py` & `deeporigin-1.2.0/src/variables/core.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/__init__.py` & `deeporigin-1.2.0/src/variables/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/aws_profile.py` & `deeporigin-1.2.0/src/variables/types/aws_profile.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/env_var.py` & `deeporigin-1.2.0/src/variables/types/env_var.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/file.py` & `deeporigin-1.2.0/src/variables/types/file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/git_http_credentials.py` & `deeporigin-1.2.0/src/variables/types/git_http_credentials.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/private_gpg_key.py` & `deeporigin-1.2.0/src/variables/types/private_gpg_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/private_ssh_key.py` & `deeporigin-1.2.0/src/variables/types/private_ssh_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/secret_env_var_value.py` & `deeporigin-1.2.0/src/variables/types/secret_env_var_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/secret_file_value.py` & `deeporigin-1.2.0/src/variables/types/secret_file_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/src/variables/types/xpress_license_file.py` & `deeporigin-1.2.0/src/variables/types/xpress_license_file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/tests/test_cli.py` & `deeporigin-1.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/tests/test_cli_data.py` & `deeporigin-1.2.0/tests/test_cli_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import pytest
 from beartype import beartype
 from deeporigin import cli
 from deeporigin.managed_data import _api
 from deeporigin.managed_data.client import (
     Client,
     DeepOriginClient,
-    MockClient,
 )
 from deeporigin.managed_data.schema import DescribeFileResponse, ListRowsResponse
+from mock_client import MockClient
 
 # this allows us to try every CLI command with both
 # multiple options using pytest.mark.parametrize
 JSON_OPTIONS = (
     ["--json"],
     [],
 )
```

### Comparing `deeporigin-0.1.1/tests/test_config.py` & `deeporigin-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/tests/test_context.py` & `deeporigin-1.2.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/tests/test_feature_flags.py` & `deeporigin-1.2.0/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.1/tests/test_managed_data.py` & `deeporigin-1.2.0/tests/test_managed_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 import pandas as pd
 import pytest
 from deeporigin.exceptions import DeepOriginException
 from deeporigin.managed_data import _api, api
 from deeporigin.managed_data.client import (
     DeepOriginClient,
-    MockClient,
 )
 from deeporigin.managed_data.schema import (
     DATAFRAME_ATTRIBUTE_KEYS,
     CreateDatabaseResponse,
     CreateWorkspaceResponse,
     DescribeFileResponse,
     DescribeRowResponseDatabase,
     DescribeRowResponseRow,
     ListRowsResponse,
 )
 from deeporigin.utils import PREFIXES
+from mock_client import MockClient
 
 
 @pytest.fixture(scope="session", autouse=True)
 def config(pytestconfig):
     """this fixture performs some setup tasks
     before all tests are run, and runs only once"""
 
@@ -337,15 +337,14 @@
     if "file" not in config.keys():
         return
 
     file_id = config["file"]["id"]
 
     if config["mock"]:
         _api.download_file(file_id, client=config["client"])
-        os.remove("placeholder")
 
         with pytest.raises(DeepOriginException, match="should be a path to a folder"):
             _api.download_file(
                 file_id,
                 client=config["client"],
                 destination="non-existent-path",
             )
```

### Comparing `deeporigin-0.1.1/tests/test_variables.py` & `deeporigin-1.2.0/tests/test_variables.py`

 * *Files identical despite different names*

