# Comparing `tmp/pulumi_dbtcloud-0.2.0a1716988489.tar.gz` & `tmp/pulumi_dbtcloud-0.2.0a1717083774.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dbtcloud-0.2.0a1716988489.tar", last modified: Wed May 29 13:17:16 2024, max compression
+gzip compressed data, was "pulumi_dbtcloud-0.2.0a1717083774.tar", last modified: Thu May 30 16:12:11 2024, max compression
```

## Comparing `pulumi_dbtcloud-0.2.0a1716988489.tar` & `pulumi_dbtcloud-0.2.0a1717083774.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    59512 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    46115 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21215 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    30802 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable_job_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25219 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    28372 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    15306 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/group_partial_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    69766 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/license_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    16495 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29966 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/partial_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    22632 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    47259 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    29051 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:17:16.172694 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 13:17:16.000000 pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-29 13:17:09.000000 pulumi_dbtcloud-0.2.0a1716988489/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:17:16.176694 pulumi_dbtcloud-0.2.0a1716988489/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:12:11.570035 pulumi_dbtcloud-0.2.0a1717083774/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-30 16:12:11.570035 pulumi_dbtcloud-0.2.0a1717083774/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:12:11.570035 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59512 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/big_query_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:12:11.570035 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46115 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21215 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30802 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14751 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/environment_variable_job_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25219 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/fabric_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28372 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/fabric_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_azure_dev_ops_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_azure_dev_ops_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_big_query_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15306 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/group_partial_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69766 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/license_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30185 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16495 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29966 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/partial_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22632 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project_artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    47259 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15033 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29051 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:12:11.570035 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-30 16:12:11.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-30 16:12:11.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:12:11.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 16:12:11.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 16:12:11.000000 pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-30 16:12:05.000000 pulumi_dbtcloud-0.2.0a1717083774/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:12:11.570035 pulumi_dbtcloud-0.2.0a1717083774/setup.cfg
```

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1717083774/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.2.0a1716988489
+Version: 0.2.0a1717083774
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
-Project-URL: Homepage, https://www.pulumi.com
+Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0
 Requires-Dist: semver>=2.8.1
```

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/README.md` & `pulumi_dbtcloud-0.2.0a1717083774/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/__init__.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_inputs.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/_utilities.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/big_query_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/big_query_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/__init__.pyi` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/config/vars.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/connection.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/databricks_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/environment_variable_job_override.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/environment_variable_job_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/extended_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_connection.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/fabric_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/fabric_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/fabric_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_project.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_azure_dev_ops_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_azure_dev_ops_repository.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_azure_dev_ops_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_big_query_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_big_query_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_connection.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_databricks_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environment_variable.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_environments.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_environments.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_extended_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_group_users.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_group_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_job.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_notification.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_postgres_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_privatelink_endpoint.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_project.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_repository.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_service_token.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_user_groups.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/get_webhook.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/get_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/group.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/group_partial_permissions.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/group_partial_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/job.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/license_map.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/license_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/notification.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/outputs.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/partial_notification.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/partial_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/postgres_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_artefacts.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project_artefacts.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_connection.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/project_repository.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/project_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/provider.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/repository.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/service_token.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/user_groups.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud/webhook.py` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.2.0a1716988489
+Version: 0.2.0a1717083774
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
-Project-URL: Homepage, https://www.pulumi.com
+Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0
 Requires-Dist: semver>=2.8.1
```

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pulumi_dbtcloud.egg-info/SOURCES.txt` & `pulumi_dbtcloud-0.2.0a1717083774/pulumi_dbtcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716988489/pyproject.toml` & `pulumi_dbtcloud-0.2.0a1717083774/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
   name = "pulumi_dbtcloud"
   description = "A Pulumi package for creating and managing dbt Cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "dbtcloud", "dbt", "cloud", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.2.0a1716988489"
+  version = "0.2.0a1717083774"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
-    Homepage = "https://www.pulumi.com"
+    Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-dbtcloud"
 
 [build-system]
   requires = ["setuptools>=61.0"]
   build-backend = "setuptools.build_meta"
 
 [tool]
```

