# Comparing `tmp/adapta-2.9.1.tar.gz` & `tmp/adapta-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapta-2.9.1.tar", max compression
+gzip compressed data, was "adapta-2.9.2.tar", max compression
```

## Comparing `adapta-2.9.1.tar` & `adapta-2.9.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0    10693 2024-03-26 11:16:26.107453 adapta-2.9.1/LICENSE
--rw-r--r--   0        0        0      811 2024-03-26 11:16:26.107453 adapta-2.9.1/README.md
--rw-r--r--   0        0        0      668 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/__init__.py
--rw-r--r--   0        0        0       22 2024-03-26 11:16:38.939486 adapta-2.9.1/adapta/_version.py
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/connectors/__init__.py
--rw-r--r--   0        0        0      699 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/connectors/service_bus/__init__.py
--rw-r--r--   0        0        0     1919 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/connectors/service_bus/_connector.py
--rw-r--r--   0        0        0     4111 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/README.md
--rw-r--r--   0        0        0      788 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/__init__.py
--rw-r--r--   0        0        0     7907 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/_async_logger.py
--rw-r--r--   0        0        0     7520 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/_base.py
--rw-r--r--   0        0        0     3021 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/_internal.py
--rw-r--r--   0        0        0    11496 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/_internal_logger.py
--rw-r--r--   0        0        0     3481 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/_logger_interface.py
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.107453 adapta-2.9.1/adapta/logs/handlers/__init__.py
--rw-r--r--   0        0        0     9086 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/logs/handlers/datadog_api_handler.py
--rw-r--r--   0        0        0     2216 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/logs/handlers/safe_stream_handler.py
--rw-r--r--   0        0        0      746 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/logs/models/__init__.py
--rw-r--r--   0        0        0      799 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/logs/models/_log_level.py
--rw-r--r--   0        0        0      968 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/logs/models/_logs_metadata.py
--rw-r--r--   0        0        0      677 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/metrics/__init__.py
--rw-r--r--   0        0        0     3220 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/metrics/_base.py
--rw-r--r--   0        0        0     1930 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/metrics/providers/README.md
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/metrics/providers/__init__.py
--rw-r--r--   0        0        0     4471 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/metrics/providers/datadog_provider.py
--rw-r--r--   0        0        0      658 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/ml/__init__.py
--rw-r--r--   0        0        0     1228 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/ml/_model.py
--rw-r--r--   0        0        0      704 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/ml/mlflow/__init__.py
--rw-r--r--   0        0        0     5324 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/ml/mlflow/_client.py
--rw-r--r--   0        0        0     4017 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/ml/mlflow/_functions.py
--rw-r--r--   0        0        0      679 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/process_communication/__init__.py
--rw-r--r--   0        0        0     3339 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/process_communication/_models.py
--rw-r--r--   0        0        0      732 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/schema_management/README.md
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/schema_management/__init__.py
--rw-r--r--   0        0        0     1436 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/schema_management/schema_entity.py
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/__init__.py
--rw-r--r--   0        0        0     2833 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/README.md
--rw-r--r--   0        0        0     1544 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/__init__.py
--rw-r--r--   0        0        0     8363 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/_azure_client.py
--rw-r--r--   0        0        0     2401 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/_base.py
--rw-r--r--   0        0        0     1792 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/_local_client.py
--rw-r--r--   0        0        0      738 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/aws/__init__.py
--rw-r--r--   0        0        0     3048 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/aws/_aws_client.py
--rw-r--r--   0        0        0     2614 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/aws/_aws_credentials.py
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/hashicorp_vault/__init__.py
--rw-r--r--   0        0        0     2700 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
--rw-r--r--   0        0        0     2606 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py
--rw-r--r--   0        0        0     3459 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/hashicorp_vault/oidc_client.py
--rw-r--r--   0        0        0     1957 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/security/clients/hashicorp_vault/token_client.py
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/__init__.py
--rw-r--r--   0        0        0     2671 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/blob/README.md
--rw-r--r--   0        0        0      627 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/blob/__init__.py
--rw-r--r--   0        0        0    11585 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/blob/azure_storage_client.py
--rw-r--r--   0        0        0     5385 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/blob/base.py
--rw-r--r--   0        0        0     5661 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/blob/s3_storage_client.py
--rw-r--r--   0        0        0      670 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/cache/__init__.py
--rw-r--r--   0        0        0     3456 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/cache/_base.py
--rw-r--r--   0        0        0     3370 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/cache/redis_cache.py
--rw-r--r--   0        0        0     2946 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/README.md
--rw-r--r--   0        0        0      603 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/__init__.py
--rw-r--r--   0        0        0     4696 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/azure_sql.py
--rw-r--r--   0        0        0      680 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/models/__init__.py
--rw-r--r--   0        0        0     1452 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/models/_models.py
--rw-r--r--   0        0        0     7732 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/odbc.py
--rw-r--r--   0        0        0     3528 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/snowflake_sql.py
--rw-r--r--   0        0        0     4545 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/database/trino_sql.py
--rw-r--r--   0        0        0     3560 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/delta_lake/README.md
--rw-r--r--   0        0        0      726 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/delta_lake/__init__.py
--rw-r--r--   0        0        0    11704 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/delta_lake/_functions.py
--rw-r--r--   0        0        0     2252 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/delta_lake/_models.py
--rw-r--r--   0        0        0      627 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/distributed_object_store/__init__.py
--rw-r--r--   0        0        0     5752 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/README.md
--rw-r--r--   0        0        0      704 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/__init__.py
--rw-r--r--   0        0        0     1553 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/_models.py
--rw-r--r--   0        0        0    28285 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/astra_client.py
--rw-r--r--   0        0        0      737 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/exceptions.py
--rw-r--r--   0        0        0      674 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/__init__.py
--rw-r--r--   0        0        0     1663 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/_functions.py
--rw-r--r--   0        0        0     2211 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/astra.py
--rw-r--r--   0        0        0     2283 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/aws.py
--rw-r--r--   0        0        0     5307 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/azure.py
--rw-r--r--   0        0        0     2102 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/base.py
--rw-r--r--   0        0        0    13072 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/filter_expression.py
--rw-r--r--   0        0        0     5682 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/format.py
--rw-r--r--   0        0        0     6635 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/hive.py
--rw-r--r--   0        0        0     1524 2024-03-26 11:16:26.111453 adapta-2.9.1/adapta/storage/models/local.py
--rw-r--r--   0        0        0     2414 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/query_enabled_store/README.md
--rw-r--r--   0        0        0      804 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/query_enabled_store/__init__.py
--rw-r--r--   0        0        0     5672 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/query_enabled_store/_models.py
--rw-r--r--   0        0        0     4544 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/query_enabled_store/_qes_astra.py
--rw-r--r--   0        0        0     2259 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/query_enabled_store/_qes_delta.py
--rw-r--r--   0        0        0     1953 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/secrets/README.md
--rw-r--r--   0        0        0      671 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/secrets/__init__.py
--rw-r--r--   0        0        0     2221 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/secrets/_base.py
--rw-r--r--   0        0        0     2363 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/secrets/azure_secret_client.py
--rw-r--r--   0        0        0     2892 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
--rw-r--r--   0        0        0     7253 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/README.md
--rw-r--r--   0        0        0      816 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/__init__.py
--rw-r--r--   0        0        0     8168 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/_common.py
--rw-r--r--   0        0        0     3951 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/concurrent_task_runner.py
--rw-r--r--   0        0        0       87 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/data_structures/__init__.py
--rw-r--r--   0        0        0     5392 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/data_structures/_functions.py
--rw-r--r--   0        0        0      180 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/decorators/__init__.py
--rw-r--r--   0        0        0     4365 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/decorators/_logging.py
--rw-r--r--   0        0        0     1507 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/decorators/_rate_limit.py
--rw-r--r--   0        0        0       86 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/python_typing/__init__.py
--rw-r--r--   0        0        0      391 2024-03-26 11:16:26.115453 adapta-2.9.1/adapta/utils/python_typing/_functions.py
--rw-r--r--   0        0        0     2617 2024-03-26 11:16:38.939486 adapta-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 adapta-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0    10693 2024-04-03 09:19:20.454319 adapta-2.9.2/LICENSE
+-rw-r--r--   0        0        0      811 2024-04-03 09:19:20.454319 adapta-2.9.2/README.md
+-rw-r--r--   0        0        0      668 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-03 09:19:34.618173 adapta-2.9.2/adapta/_version.py
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/connectors/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/connectors/service_bus/__init__.py
+-rw-r--r--   0        0        0     1919 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/connectors/service_bus/_connector.py
+-rw-r--r--   0        0        0     4111 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/README.md
+-rw-r--r--   0        0        0      788 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/__init__.py
+-rw-r--r--   0        0        0     7907 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/_async_logger.py
+-rw-r--r--   0        0        0     7520 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/_base.py
+-rw-r--r--   0        0        0     3021 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/_internal.py
+-rw-r--r--   0        0        0    11496 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/_internal_logger.py
+-rw-r--r--   0        0        0     3481 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/_logger_interface.py
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/handlers/__init__.py
+-rw-r--r--   0        0        0     9086 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/handlers/datadog_api_handler.py
+-rw-r--r--   0        0        0     2216 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/handlers/safe_stream_handler.py
+-rw-r--r--   0        0        0      746 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/models/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/models/_log_level.py
+-rw-r--r--   0        0        0      968 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/logs/models/_logs_metadata.py
+-rw-r--r--   0        0        0      677 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/metrics/__init__.py
+-rw-r--r--   0        0        0     3220 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/metrics/_base.py
+-rw-r--r--   0        0        0     1930 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/metrics/providers/README.md
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     4471 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/metrics/providers/datadog_provider.py
+-rw-r--r--   0        0        0      658 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/ml/__init__.py
+-rw-r--r--   0        0        0     1228 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/ml/_model.py
+-rw-r--r--   0        0        0      704 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/ml/mlflow/__init__.py
+-rw-r--r--   0        0        0     5324 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/ml/mlflow/_client.py
+-rw-r--r--   0        0        0     4017 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/ml/mlflow/_functions.py
+-rw-r--r--   0        0        0      679 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/process_communication/__init__.py
+-rw-r--r--   0        0        0     3339 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/process_communication/_models.py
+-rw-r--r--   0        0        0      732 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/schema_management/README.md
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/schema_management/__init__.py
+-rw-r--r--   0        0        0     1436 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/schema_management/schema_entity.py
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/__init__.py
+-rw-r--r--   0        0        0     2833 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/README.md
+-rw-r--r--   0        0        0     1544 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/__init__.py
+-rw-r--r--   0        0        0     8363 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/_azure_client.py
+-rw-r--r--   0        0        0     2401 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/_base.py
+-rw-r--r--   0        0        0     1792 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/_local_client.py
+-rw-r--r--   0        0        0      738 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/aws/__init__.py
+-rw-r--r--   0        0        0     3048 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/aws/_aws_client.py
+-rw-r--r--   0        0        0     2614 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/aws/_aws_credentials.py
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/hashicorp_vault/__init__.py
+-rw-r--r--   0        0        0     2700 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
+-rw-r--r--   0        0        0     2606 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/hashicorp_vault/kubernetes_client.py
+-rw-r--r--   0        0        0     3459 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/hashicorp_vault/oidc_client.py
+-rw-r--r--   0        0        0     1957 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/security/clients/hashicorp_vault/token_client.py
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/__init__.py
+-rw-r--r--   0        0        0     2671 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/blob/README.md
+-rw-r--r--   0        0        0      627 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/blob/__init__.py
+-rw-r--r--   0        0        0    11585 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/blob/azure_storage_client.py
+-rw-r--r--   0        0        0     5385 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/blob/base.py
+-rw-r--r--   0        0        0     5661 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/blob/s3_storage_client.py
+-rw-r--r--   0        0        0      670 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/cache/__init__.py
+-rw-r--r--   0        0        0     3456 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/cache/_base.py
+-rw-r--r--   0        0        0     3370 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/cache/redis_cache.py
+-rw-r--r--   0        0        0     2946 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/database/README.md
+-rw-r--r--   0        0        0      603 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/database/__init__.py
+-rw-r--r--   0        0        0     4696 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/database/azure_sql.py
+-rw-r--r--   0        0        0      680 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/database/models/__init__.py
+-rw-r--r--   0        0        0     1452 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/database/models/_models.py
+-rw-r--r--   0        0        0     7732 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/database/odbc.py
+-rw-r--r--   0        0        0     3528 2024-04-03 09:19:20.454319 adapta-2.9.2/adapta/storage/database/snowflake_sql.py
+-rw-r--r--   0        0        0     4545 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/database/trino_sql.py
+-rw-r--r--   0        0        0     3560 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/delta_lake/README.md
+-rw-r--r--   0        0        0      726 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/delta_lake/__init__.py
+-rw-r--r--   0        0        0    11704 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/delta_lake/_functions.py
+-rw-r--r--   0        0        0     2252 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/delta_lake/_models.py
+-rw-r--r--   0        0        0      627 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/distributed_object_store/__init__.py
+-rw-r--r--   0        0        0     5752 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/README.md
+-rw-r--r--   0        0        0      704 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/__init__.py
+-rw-r--r--   0        0        0     1553 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/_models.py
+-rw-r--r--   0        0        0    28285 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/astra_client.py
+-rw-r--r--   0        0        0      737 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/exceptions.py
+-rw-r--r--   0        0        0      674 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/__init__.py
+-rw-r--r--   0        0        0     1663 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/_functions.py
+-rw-r--r--   0        0        0     2211 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/astra.py
+-rw-r--r--   0        0        0     2283 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/aws.py
+-rw-r--r--   0        0        0     5307 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/azure.py
+-rw-r--r--   0        0        0     2102 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/base.py
+-rw-r--r--   0        0        0    13072 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/filter_expression.py
+-rw-r--r--   0        0        0     5682 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/format.py
+-rw-r--r--   0        0        0     6635 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/hive.py
+-rw-r--r--   0        0        0     1524 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/models/local.py
+-rw-r--r--   0        0        0     2414 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/query_enabled_store/README.md
+-rw-r--r--   0        0        0      804 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/query_enabled_store/__init__.py
+-rw-r--r--   0        0        0     5672 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/query_enabled_store/_models.py
+-rw-r--r--   0        0        0     4544 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/query_enabled_store/_qes_astra.py
+-rw-r--r--   0        0        0     2259 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/query_enabled_store/_qes_delta.py
+-rw-r--r--   0        0        0     1953 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/secrets/README.md
+-rw-r--r--   0        0        0      671 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/secrets/__init__.py
+-rw-r--r--   0        0        0     2221 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/secrets/_base.py
+-rw-r--r--   0        0        0     2363 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/secrets/azure_secret_client.py
+-rw-r--r--   0        0        0     2892 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
+-rw-r--r--   0        0        0     7253 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/README.md
+-rw-r--r--   0        0        0      816 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/__init__.py
+-rw-r--r--   0        0        0     8168 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/_common.py
+-rw-r--r--   0        0        0     3951 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/concurrent_task_runner.py
+-rw-r--r--   0        0        0       87 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/data_structures/__init__.py
+-rw-r--r--   0        0        0     5392 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/data_structures/_functions.py
+-rw-r--r--   0        0        0      180 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/decorators/__init__.py
+-rw-r--r--   0        0        0     4365 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/decorators/_logging.py
+-rw-r--r--   0        0        0     1507 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/decorators/_rate_limit.py
+-rw-r--r--   0        0        0       86 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/python_typing/__init__.py
+-rw-r--r--   0        0        0      705 2024-04-03 09:19:20.458319 adapta-2.9.2/adapta/utils/python_typing/_functions.py
+-rw-r--r--   0        0        0     2617 2024-04-03 09:19:34.618173 adapta-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 adapta-2.9.2/PKG-INFO
```

### Comparing `adapta-2.9.1/LICENSE` & `adapta-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/README.md` & `adapta-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/__init__.py` & `adapta-2.9.2/adapta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/connectors/__init__.py` & `adapta-2.9.2/adapta/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/connectors/service_bus/__init__.py` & `adapta-2.9.2/adapta/connectors/service_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/connectors/service_bus/_connector.py` & `adapta-2.9.2/adapta/connectors/service_bus/_connector.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/README.md` & `adapta-2.9.2/adapta/logs/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/__init__.py` & `adapta-2.9.2/adapta/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/_async_logger.py` & `adapta-2.9.2/adapta/logs/_async_logger.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/_base.py` & `adapta-2.9.2/adapta/logs/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/_internal.py` & `adapta-2.9.2/adapta/logs/_internal.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/_internal_logger.py` & `adapta-2.9.2/adapta/logs/_internal_logger.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/_logger_interface.py` & `adapta-2.9.2/adapta/logs/_logger_interface.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/handlers/__init__.py` & `adapta-2.9.2/adapta/logs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/handlers/datadog_api_handler.py` & `adapta-2.9.2/adapta/logs/handlers/datadog_api_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/handlers/safe_stream_handler.py` & `adapta-2.9.2/adapta/logs/handlers/safe_stream_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/models/__init__.py` & `adapta-2.9.2/adapta/logs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/models/_log_level.py` & `adapta-2.9.2/adapta/logs/models/_log_level.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/logs/models/_logs_metadata.py` & `adapta-2.9.2/adapta/logs/models/_logs_metadata.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/metrics/__init__.py` & `adapta-2.9.2/adapta/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/metrics/_base.py` & `adapta-2.9.2/adapta/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/metrics/providers/README.md` & `adapta-2.9.2/adapta/metrics/providers/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/metrics/providers/__init__.py` & `adapta-2.9.2/adapta/metrics/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/metrics/providers/datadog_provider.py` & `adapta-2.9.2/adapta/metrics/providers/datadog_provider.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/ml/__init__.py` & `adapta-2.9.2/adapta/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/ml/_model.py` & `adapta-2.9.2/adapta/ml/_model.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/ml/mlflow/__init__.py` & `adapta-2.9.2/adapta/ml/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/ml/mlflow/_client.py` & `adapta-2.9.2/adapta/ml/mlflow/_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/ml/mlflow/_functions.py` & `adapta-2.9.2/adapta/ml/mlflow/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/process_communication/__init__.py` & `adapta-2.9.2/adapta/process_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/process_communication/_models.py` & `adapta-2.9.2/adapta/process_communication/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/schema_management/README.md` & `adapta-2.9.2/adapta/schema_management/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/schema_management/__init__.py` & `adapta-2.9.2/adapta/schema_management/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/schema_management/schema_entity.py` & `adapta-2.9.2/adapta/schema_management/schema_entity.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/__init__.py` & `adapta-2.9.2/adapta/security/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/README.md` & `adapta-2.9.2/adapta/security/clients/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/__init__.py` & `adapta-2.9.2/adapta/security/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/_azure_client.py` & `adapta-2.9.2/adapta/security/clients/_azure_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/_base.py` & `adapta-2.9.2/adapta/security/clients/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/_local_client.py` & `adapta-2.9.2/adapta/security/clients/_local_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/aws/__init__.py` & `adapta-2.9.2/adapta/security/clients/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/aws/_aws_client.py` & `adapta-2.9.2/adapta/security/clients/aws/_aws_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/aws/_aws_credentials.py` & `adapta-2.9.2/adapta/security/clients/aws/_aws_credentials.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/hashicorp_vault/__init__.py` & `adapta-2.9.2/adapta/security/clients/hashicorp_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py` & `adapta-2.9.2/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py` & `adapta-2.9.2/adapta/security/clients/hashicorp_vault/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/hashicorp_vault/oidc_client.py` & `adapta-2.9.2/adapta/security/clients/hashicorp_vault/oidc_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/security/clients/hashicorp_vault/token_client.py` & `adapta-2.9.2/adapta/security/clients/hashicorp_vault/token_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/__init__.py` & `adapta-2.9.2/adapta/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/blob/README.md` & `adapta-2.9.2/adapta/storage/blob/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/blob/__init__.py` & `adapta-2.9.2/adapta/storage/blob/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/blob/azure_storage_client.py` & `adapta-2.9.2/adapta/storage/blob/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/blob/base.py` & `adapta-2.9.2/adapta/storage/blob/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/blob/s3_storage_client.py` & `adapta-2.9.2/adapta/storage/blob/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/cache/__init__.py` & `adapta-2.9.2/adapta/storage/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/cache/_base.py` & `adapta-2.9.2/adapta/storage/cache/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/cache/redis_cache.py` & `adapta-2.9.2/adapta/storage/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/README.md` & `adapta-2.9.2/adapta/storage/database/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/__init__.py` & `adapta-2.9.2/adapta/storage/database/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/azure_sql.py` & `adapta-2.9.2/adapta/storage/database/azure_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/models/__init__.py` & `adapta-2.9.2/adapta/storage/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/models/_models.py` & `adapta-2.9.2/adapta/storage/database/models/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/odbc.py` & `adapta-2.9.2/adapta/storage/database/odbc.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/snowflake_sql.py` & `adapta-2.9.2/adapta/storage/database/snowflake_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/database/trino_sql.py` & `adapta-2.9.2/adapta/storage/database/trino_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/delta_lake/README.md` & `adapta-2.9.2/adapta/storage/delta_lake/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/delta_lake/__init__.py` & `adapta-2.9.2/adapta/storage/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/delta_lake/_functions.py` & `adapta-2.9.2/adapta/storage/delta_lake/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/delta_lake/_models.py` & `adapta-2.9.2/adapta/storage/delta_lake/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/distributed_object_store/__init__.py` & `adapta-2.9.2/adapta/storage/distributed_object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/README.md` & `adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/__init__.py` & `adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/_models.py` & `adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/distributed_object_store/datastax_astra/astra_client.py` & `adapta-2.9.2/adapta/storage/distributed_object_store/datastax_astra/astra_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/exceptions.py` & `adapta-2.9.2/adapta/storage/exceptions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/__init__.py` & `adapta-2.9.2/adapta/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/_functions.py` & `adapta-2.9.2/adapta/storage/models/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/astra.py` & `adapta-2.9.2/adapta/storage/models/astra.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/aws.py` & `adapta-2.9.2/adapta/storage/models/aws.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/azure.py` & `adapta-2.9.2/adapta/storage/models/azure.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/base.py` & `adapta-2.9.2/adapta/storage/models/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/filter_expression.py` & `adapta-2.9.2/adapta/storage/models/filter_expression.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/format.py` & `adapta-2.9.2/adapta/storage/models/format.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/hive.py` & `adapta-2.9.2/adapta/storage/models/hive.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/models/local.py` & `adapta-2.9.2/adapta/storage/models/local.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/query_enabled_store/README.md` & `adapta-2.9.2/adapta/storage/query_enabled_store/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/query_enabled_store/__init__.py` & `adapta-2.9.2/adapta/storage/query_enabled_store/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/query_enabled_store/_models.py` & `adapta-2.9.2/adapta/storage/query_enabled_store/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/query_enabled_store/_qes_astra.py` & `adapta-2.9.2/adapta/storage/query_enabled_store/_qes_astra.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/query_enabled_store/_qes_delta.py` & `adapta-2.9.2/adapta/storage/query_enabled_store/_qes_delta.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/secrets/README.md` & `adapta-2.9.2/adapta/storage/secrets/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/secrets/__init__.py` & `adapta-2.9.2/adapta/storage/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/secrets/_base.py` & `adapta-2.9.2/adapta/storage/secrets/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/secrets/azure_secret_client.py` & `adapta-2.9.2/adapta/storage/secrets/azure_secret_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py` & `adapta-2.9.2/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/utils/README.md` & `adapta-2.9.2/adapta/utils/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/utils/__init__.py` & `adapta-2.9.2/adapta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/utils/_common.py` & `adapta-2.9.2/adapta/utils/_common.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/utils/concurrent_task_runner.py` & `adapta-2.9.2/adapta/utils/concurrent_task_runner.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/utils/data_structures/_functions.py` & `adapta-2.9.2/adapta/utils/data_structures/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/utils/decorators/_logging.py` & `adapta-2.9.2/adapta/utils/decorators/_logging.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/adapta/utils/decorators/_rate_limit.py` & `adapta-2.9.2/adapta/utils/decorators/_rate_limit.py`

 * *Files identical despite different names*

### Comparing `adapta-2.9.1/pyproject.toml` & `adapta-2.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adapta"
-version = "2.9.1"
+version = "2.9.2"
 description = "Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'Apache 2.0'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/adapta'
```

### Comparing `adapta-2.9.1/PKG-INFO` & `adapta-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adapta
-Version: 2.9.1
+Version: 2.9.2
 Summary: Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier.
 Home-page: https://github.com/SneaksAndData/adapta
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

