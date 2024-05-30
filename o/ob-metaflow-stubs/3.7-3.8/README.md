# Comparing `tmp/ob-metaflow-stubs-3.7.tar.gz` & `tmp/ob-metaflow-stubs-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-3.7.tar", last modified: Wed May 22 22:08:55 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-3.8.tar", last modified: Thu May 30 17:29:02 2024, max compression
```

## Comparing `ob-metaflow-stubs-3.7.tar` & `ob-metaflow-stubs-3.8.tar`

### file list

```diff
@@ -1,170 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107671 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.387925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.391925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.395925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.399925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.399925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.403926 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.403926 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/logs_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/perimeters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/procpoll.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/metaflow-stubs/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/profilers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/tagging_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 22:08:54.000000 ob-metaflow-stubs-3.7/metaflow-stubs/tuple_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 22:08:55.000000 ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:08:55.407925 ob-metaflow-stubs-3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 22:08:37.000000 ob-metaflow-stubs-3.7/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.021279 ob-metaflow-stubs-3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 17:28:41.000000 ob-metaflow-stubs-3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 17:29:02.021279 ob-metaflow-stubs-3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-30 17:28:41.000000 ob-metaflow-stubs-3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.001279 ob-metaflow-stubs-3.8/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.001279 ob-metaflow-stubs-3.8/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.001279 ob-metaflow-stubs-3.8/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.001279 ob-metaflow-stubs-3.8/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.005279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.005279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.005279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.005279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.005279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.005279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.009279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.009279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.009279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.013279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.013279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.013279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.013279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.017279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29098 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.017279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.017279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.017279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/logs_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/perimeters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.017279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.021279 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/procpoll.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.021279 ob-metaflow-stubs-3.8/metaflow-stubs/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/profilers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/pylint_wrapper.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.021279 ob-metaflow-stubs-3.8/metaflow-stubs/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/runner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23267 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/runner/metaflow_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/runner/nbrun.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/runner/subprocess_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/tagging_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-30 17:28:59.000000 ob-metaflow-stubs-3.8/metaflow-stubs/tuple_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:29:02.021279 ob-metaflow-stubs-3.8/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-30 17:29:01.000000 ob-metaflow-stubs-3.8/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-30 17:29:01.000000 ob-metaflow-stubs-3.8/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:29:01.000000 ob-metaflow-stubs-3.8/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 17:29:01.000000 ob-metaflow-stubs-3.8/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:29:02.021279 ob-metaflow-stubs-3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-30 17:28:41.000000 ob-metaflow-stubs-3.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 17:28:41.000000 ob-metaflow-stubs-3.8/version.py
```

### Comparing `ob-metaflow-stubs-3.7/PKG-INFO` & `ob-metaflow-stubs-3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.7
+Version: 3.8
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.490721                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.704529                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.client.core
-    import metaflow.metaflow_current
+    import metaflow._vendor.click.types
+    import metaflow.parameters
     import io
+    import metaflow.datastore.inputs
+    import metaflow.runner.metaflow_runner
     import metaflow.events
+    import metaflow.client.core
     import datetime
-    import metaflow.parameters
-    import metaflow.datastore.inputs
     import typing
     import metaflow.plugins.datatools.s3.s3
-    import metaflow._vendor.click.types
+    import metaflow.metaflow_current
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,195 +723,267 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
-    
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    gpu : int, default 0
+        Number of GPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on AWS Batch. If not specified, and
+        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    queue : str, default METAFLOW_BATCH_JOB_QUEUE
+        AWS Batch Job Queue to submit the job to.
+    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
+        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
+    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
+        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
+        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
+    max_swap : int, optional, default None
+        The total amount of swap memory (in MiB) a container can use for this
+        step. This parameter is translated to the `--memory-swap` option in
+        Docker where the value is the sum of the container memory plus the
+        `max_swap` value.
+    swappiness : int, optional, default None
+        This allows you to tune memory swappiness behavior for this step.
+        A swappiness value of 0 causes swapping not to happen unless absolutely
+        necessary. A swappiness value of 100 causes pages to be swapped very
+        aggressively. Accepted values are whole numbers between 0 and 100.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step. Note that tmpfs is
+        not available on Fargate compute environments
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default None
+        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
+    inferentia : int, default 0
+        Number of Inferentia chips required for this step.
+    trainium : int, default None
+        Alias for inferentia. Use only one of the two.
+    efa : int, default 0
+        Number of elastic fabric adapter network devices to attach to container
+    ephemeral_storage : int, default None
+        The total amount, in GiB, of ephemeral storage to set for the task, 21-200GiB.
+        This is only relevant for Fargate compute environments
+    log_driver: str, optional, default None
+        The log driver to use for the Amazon ECS container.
+    log_options: List[str], optional, default None
+        List of strings containing options for the chosen log driver. The configurable values
+        depend on the `log driver` chosen. Validation of these options is not supported yet.
+        Example: [`awslogs-group:aws/batch/job`]
     """
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def batch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def batch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+def batch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None):
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
-    
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
-    
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    gpu : int, default 0
+        Number of GPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on AWS Batch. If not specified, and
+        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    queue : str, default METAFLOW_BATCH_JOB_QUEUE
+        AWS Batch Job Queue to submit the job to.
+    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
+        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
+    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
+        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
+        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
+    max_swap : int, optional, default None
+        The total amount of swap memory (in MiB) a container can use for this
+        step. This parameter is translated to the `--memory-swap` option in
+        Docker where the value is the sum of the container memory plus the
+        `max_swap` value.
+    swappiness : int, optional, default None
+        This allows you to tune memory swappiness behavior for this step.
+        A swappiness value of 0 causes swapping not to happen unless absolutely
+        necessary. A swappiness value of 100 causes pages to be swapped very
+        aggressively. Accepted values are whole numbers between 0 and 100.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step. Note that tmpfs is
+        not available on Fargate compute environments
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default None
+        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
+    inferentia : int, default 0
+        Number of Inferentia chips required for this step.
+    trainium : int, default None
+        Alias for inferentia. Use only one of the two.
+    efa : int, default 0
+        Number of elastic fabric adapter network devices to attach to container
+    ephemeral_storage : int, default None
+        The total amount, in GiB, of ephemeral storage to set for the task, 21-200GiB.
+        This is only relevant for Fargate compute environments
+    log_driver: str, optional, default None
+        The log driver to use for the Amazon ECS container.
+    log_options: List[str], optional, default None
+        List of strings containing options for the chosen log driver. The configurable values
+        depend on the `log driver` chosen. Validation of these options is not supported yet.
+        Example: [`awslogs-group:aws/batch/job`]
     """
     ...
 
 @typing.overload
-def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the resources needed when executing this step.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
     
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
     """
-    Specifies the resources needed when executing this step.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
     
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
+    Specifies a timeout for your step.
     
-    Note that you may add multiple `@card` decorators in a step with different parameters.
+    This decorator is useful if this step may hang indefinitely.
     
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
     
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
+    Specifies a timeout for your step.
     
-    Note that you may add multiple `@card` decorators in a step with different parameters.
+    This decorator is useful if this step may hang indefinitely.
     
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
     
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
 def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the Conda environment for the step.
@@ -964,157 +1037,87 @@
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
     cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
+        Number of CPUs required for this step.
     gpu : int, default 0
-        Number of GPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
     memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on AWS Batch. If not specified, and
-        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    queue : str, default METAFLOW_BATCH_JOB_QUEUE
-        AWS Batch Job Queue to submit the job to.
-    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
-        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
-    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
-        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
-        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
+        Memory size (in MB) required for this step.
     shared_memory : int, optional, default None
         The value for the size (in MiB) of the /dev/shm volume for this step.
         This parameter maps to the `--shm-size` option in Docker.
-    max_swap : int, optional, default None
-        The total amount of swap memory (in MiB) a container can use for this
-        step. This parameter is translated to the `--memory-swap` option in
-        Docker where the value is the sum of the container memory plus the
-        `max_swap` value.
-    swappiness : int, optional, default None
-        This allows you to tune memory swappiness behavior for this step.
-        A swappiness value of 0 causes swapping not to happen unless absolutely
-        necessary. A swappiness value of 100 causes pages to be swapped very
-        aggressively. Accepted values are whole numbers between 0 and 100.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step. Note that tmpfs is
-        not available on Fargate compute environments
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default None
-        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
-    inferentia : int, default 0
-        Number of Inferentia chips required for this step.
-    trainium : int, default None
-        Alias for inferentia. Use only one of the two.
-    efa : int, default 0
-        Number of elastic fabric adapter network devices to attach to container
-    ephemeral_storage: int, default None
-        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
-        This is only relevant for Fargate compute environments
-    log_driver: str, optional, default None
-        The log driver to use for the Amazon ECS container.
-    log_options: List[str], optional, default None
-        List of strings containing options for the chosen log driver. The configurable values
-        depend on the `log driver` chosen. Validation of these options is not supported yet.
-        Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
-def batch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def batch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def batch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None):
+def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
     """
-    Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
     cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
+        Number of CPUs required for this step.
     gpu : int, default 0
-        Number of GPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
     memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on AWS Batch. If not specified, and
-        METAFLOW_BATCH_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    queue : str, default METAFLOW_BATCH_JOB_QUEUE
-        AWS Batch Job Queue to submit the job to.
-    iam_role : str, default METAFLOW_ECS_S3_ACCESS_IAM_ROLE
-        AWS IAM role that AWS Batch container uses to access AWS cloud resources.
-    execution_role : str, default METAFLOW_ECS_FARGATE_EXECUTION_ROLE
-        AWS IAM role that AWS Batch can use [to trigger AWS Fargate tasks]
-        (https://docs.aws.amazon.com/batch/latest/userguide/execution-IAM-role.html).
+        Memory size (in MB) required for this step.
     shared_memory : int, optional, default None
         The value for the size (in MiB) of the /dev/shm volume for this step.
         This parameter maps to the `--shm-size` option in Docker.
-    max_swap : int, optional, default None
-        The total amount of swap memory (in MiB) a container can use for this
-        step. This parameter is translated to the `--memory-swap` option in
-        Docker where the value is the sum of the container memory plus the
-        `max_swap` value.
-    swappiness : int, optional, default None
-        This allows you to tune memory swappiness behavior for this step.
-        A swappiness value of 0 causes swapping not to happen unless absolutely
-        necessary. A swappiness value of 100 causes pages to be swapped very
-        aggressively. Accepted values are whole numbers between 0 and 100.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step. Note that tmpfs is
-        not available on Fargate compute environments
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default None
-        Path to tmpfs mount for this step. Defaults to /metaflow_temp.
-    inferentia : int, default 0
-        Number of Inferentia chips required for this step.
-    trainium : int, default None
-        Alias for inferentia. Use only one of the two.
-    efa : int, default 0
-        Number of elastic fabric adapter network devices to attach to container
-    ephemeral_storage: int, default None
-        The total amount, in GiB, of ephemeral storage to set for the task (21-200)
-        This is only relevant for Fargate compute environments
-    log_driver: str, optional, default None
-        The log driver to use for the Amazon ECS container.
-    log_options: List[str], optional, default None
-        List of strings containing options for the chosen log driver. The configurable values
-        depend on the `log driver` chosen. Validation of these options is not supported yet.
-        Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
 def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies secrets to be retrieved and injected as environment variables prior to
@@ -1144,41 +1147,59 @@
     ----------
     sources : List[Union[str, Dict[str, Any]]], default: []
         List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
-def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies that the step will success under all circumstances.
+    
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies that the step will success under all circumstances.
+    
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None, port: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on Kubernetes.
     
@@ -1234,14 +1255,65 @@
         Shared memory size (in MiB) required for this step
     port: int, optional
         Port number to specify in the Kubernetes job object
     """
     ...
 
 @typing.overload
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
 def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the PyPI packages for the step.
     
     Information in this decorator will augment any
     attributes set in the `@pyi_base` flow-level decorator. Hence,
     you can use `@pypi_base` to set packages required by all
@@ -1283,112 +1355,59 @@
     python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
+    Specifies environment variables to be set prior to the execution of a step.
     
     Parameters
     ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
     """
     ...
 
 @typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
+def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
     """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
+    Specifies environment variables to be set prior to the execution of a step.
     
     Parameters
     ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
     """
     ...
 
-@typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    Specifies what flows belong to the same project.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    A project-specific namespace is created for all flows that
+    use the same `@project(name)`.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
-    """
-    ...
-
-@typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
-    """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    name : str
+        Project name. Make sure that the name is unique amongst all
+        projects that use the same production scheduler. The name may
+        contain only lowercase alphanumeric characters and underscores.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
     
-    Parameters
-    ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
     """
     ...
 
 @typing.overload
 def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the times when the flow should be run when running on a
@@ -1433,99 +1452,53 @@
         specified by this expression.
     timezone : str, optional, default None
         Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
         which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
-@typing.overload
-def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the Conda environment for all steps of the flow.
-    
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
-    """
-    ...
-
-@typing.overload
-def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
-    """
-    Specifies the Conda environment for all steps of the flow.
-    
-    Use `@conda_base` to set common libraries required by all
-    steps and use `@conda` to specify step-specific additions.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables Conda.
-    """
-    ...
-
-@typing.overload
-def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the PyPI packages for all steps of the flow.
-    
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
-    ...
-
-@typing.overload
-def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies the PyPI packages for all steps of the flow.
+    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
+    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
+    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
+    added as a flow decorators. Adding more than one decorator will ensure that `start` step
+    starts only after all sensors finish.
     
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    bucket_key : Union[str, List[str]]
+        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
+        When it's specified as a full s3:// url, please leave `bucket_name` as None
+    bucket_name : str
+        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
+        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
+    wildcard_match : bool
+        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
+    aws_conn_id : str
+        a reference to the s3 connection on Airflow. (Default: None)
+    verify : bool
+        Whether or not to verify SSL certificates for S3 connection. (Default: None)
     """
     ...
 
 @typing.overload
 def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the event(s) that this flow depends on.
@@ -1616,113 +1589,50 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
-def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+@typing.overload
+def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
-    before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
-    and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
-    added as a flow decorators. Adding more than one decorator will ensure that `start` step
-    starts only after all sensors finish.
+    Specifies the PyPI packages for all steps of the flow.
     
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    bucket_key : Union[str, List[str]]
-        The key(s) being waited on. Supports full s3:// style url or relative path from root level.
-        When it's specified as a full s3:// url, please leave `bucket_name` as None
-    bucket_name : str
-        Name of the S3 bucket. Only needed when bucket_key is not provided as a full s3:// url.
-        When specified, all the keys passed to bucket_key refers to this bucket. (Default:None)
-    wildcard_match : bool
-        whether the bucket_key should be interpreted as a Unix wildcard pattern. (Default: False)
-    aws_conn_id : str
-        a reference to the s3 connection on Airflow. (Default: None)
-    verify : bool
-        Whether or not to verify SSL certificates for S3 connection. (Default: None)
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
-    """
+@typing.overload
+def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
     ...
 
-def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies what flows belong to the same project.
-    
-    A project-specific namespace is created for all flows that
-    use the same `@project(name)`.
+    Specifies the PyPI packages for all steps of the flow.
     
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    name : str
-        Project name. Make sure that the name is unique amongst all
-        projects that use the same production scheduler. The name may
-        contain only lowercase alphanumeric characters and underscores.
-    
-    
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
 def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the flow(s) that this flow depends on.
@@ -1821,14 +1731,105 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
+@typing.overload
+def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the Conda environment for all steps of the flow.
+    
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
+    """
+    ...
+
+@typing.overload
+def conda_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def conda_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
+    """
+    Specifies the Conda environment for all steps of the flow.
+    
+    Use `@conda_base` to set common libraries required by all
+    steps and use `@conda` to specify step-specific additions.
+    
+    Parameters
+    ----------
+    packages : Dict[str, str], default {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables Conda.
+    """
+    ...
+
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
+    """
+    ...
+
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
     pass None to this call.
@@ -2771,10 +2772,208 @@
         ...
     def __getstate__(self):
         ...
     def __setstate__(self, state):
         ...
     ...
 
+class Runner(object, metaclass=type):
+    def __init__(self, flow_file: str, show_output: bool = True, profile: typing.Optional[str] = None, env: typing.Optional[typing.Dict] = None, cwd: typing.Optional[str] = None, **kwargs):
+        ...
+    def __enter__(self) -> metaflow.runner.metaflow_runner.Runner:
+        ...
+    def __aenter__(self) -> metaflow.runner.metaflow_runner.Runner:
+        ...
+    def _Runner__get_executing_run(self, tfp_runner_attribute, command_obj):
+        ...
+    def run(self, **kwargs) -> metaflow.runner.metaflow_runner.ExecutingRun:
+        """
+        Blocking execution of the run. This method will wait until
+        the run has completed execution.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun containing the results of the run.
+        """
+        ...
+    def resume(self, **kwargs):
+        """
+        Blocking resume execution of the run.
+        This method will wait until the resumed run has completed execution.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python ./myflow.py` after
+            the `resume` command.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun containing the results of the resumed run.
+        """
+        ...
+    def async_run(self, **kwargs) -> metaflow.runner.metaflow_runner.ExecutingRun:
+        """
+        Non-blocking execution of the run. This method will return as soon as the
+        run has launched.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the run that was started.
+        """
+        ...
+    def async_resume(self, **kwargs):
+        """
+        Non-blocking resume execution of the run.
+        This method will return as soon as the resume has launched.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `resume` command.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the resumed run that was started.
+        """
+        ...
+    def __exit__(self, exc_type, exc_value, traceback):
+        ...
+    def __aexit__(self, exc_type, exc_value, traceback):
+        ...
+    def cleanup(self):
+        """
+        Delete any temporary files created during execution.
+        """
+        ...
+    ...
+
+class NBRunner(object, metaclass=type):
+    def __init__(self, flow, show_output: bool = True, profile: typing.Optional[str] = None, env: typing.Optional[typing.Dict] = None, base_dir: str = "/tmp", **kwargs):
+        ...
+    def nbrun(self, **kwargs):
+        """
+        Blocking execution of the run. This method will wait until
+        the run has completed execution.
+        
+        Note that in contrast to `run`, this method returns a
+        `metaflow.Run` object directly and calls `cleanup()` internally
+        to support a common notebook pattern of executing a flow and
+        retrieving its results immediately.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        Run
+            A `metaflow.Run` object representing the finished run.
+        """
+        ...
+    def nbresume(self, **kwargs):
+        """
+        Blocking resuming of a run. This method will wait until
+        the resumed run has completed execution.
+        
+        Note that in contrast to `resume`, this method returns a
+        `metaflow.Run` object directly and calls `cleanup()` internally
+        to support a common notebook pattern of executing a flow and
+        retrieving its results immediately.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `resume` command.
+        
+        Returns
+        -------
+        Run
+            A `metaflow.Run` object representing the resumed run.
+        """
+        ...
+    def run(self, **kwargs):
+        """
+        Runs the flow.
+        """
+        ...
+    def resume(self, **kwargs):
+        """
+        Resumes the flow.
+        """
+        ...
+    def async_run(self, **kwargs):
+        """
+        Non-blocking execution of the run. This method will return as soon as the
+        run has launched. This method is equivalent to `Runner.async_run`.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the run that was started.
+        """
+        ...
+    def async_resume(self, **kwargs):
+        """
+        Non-blocking execution of the run. This method will return as soon as the
+        run has launched. This method is equivalent to `Runner.async_resume`.
+        
+        Note that this method is asynchronous and needs to be `await`ed.
+        
+        Parameters
+        ----------
+        **kwargs : Any
+            Additional arguments that you would pass to `python myflow.py` after
+            the `run` command, in particular, any parameters accepted by the flow.
+        
+        Returns
+        -------
+        ExecutingRun
+            ExecutingRun representing the run that was started.
+        """
+        ...
+    def cleanup(self):
+        """
+        Delete any temporary files created during execution.
+        
+        Call this method after using `async_run` or `async_resume`. You don't
+        have to call this after `nbrun` or `nbresume`.
+        """
+        ...
+    ...
+
 def get_aws_client(module, with_error = False, role_arn = None, session_vars = None, client_params = None):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/cards.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.511701                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.725759                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_client
-    import metaflow
-    import metaflow.plugins.cards.card_modules.card
-    import metaflow.plugins.cards.card_modules.components
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow.plugins.cards.card_modules.card
     import typing
+    import metaflow
+    import metaflow.plugins.cards.card_modules.components
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
     retrieve them from the datastore. Actual card contents are retrieved lazily either when
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/cli.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.516442                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.733893                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
@@ -27,69 +27,91 @@
     Returns
     -------
     str, optional
         Namespace set (result of get_namespace()).
     """
     ...
 
-current: metaflow.metaflow_current.Current
-
-def validate_tags(tags, existing_tags = None):
+def get_metadata() -> str:
     """
-    Raises MetaflowTaggingError if invalid based on these rules:
+    Returns the current Metadata provider.
     
-    Tag set size is too large. But it's OK if tag set is not larger
-    than an existing tag set (if provided).
+    If this is not set explicitly using `metadata`, the default value is
+    determined through the Metaflow configuration. You can use this call to
+    check that your configuration is set up properly.
     
-    Then, we validate each tag.  See validate_tag()
+    If multiple configuration profiles are present, this call returns the one
+    selected through the `METAFLOW_PROFILE` environment variable.
+    
+    Returns
+    -------
+    str
+        Information about the Metadata provider currently selected. This information typically
+        returns provider specific information (like URL for remote providers or local paths for
+        local providers).
     """
     ...
 
 class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-DATASTORES: list
-
-ENVIRONMENTS: list
-
-LOGGING_SIDECARS: dict
-
-METADATA_PROVIDERS: list
-
-MONITOR_SIDECARS: dict
+DECOSPECS: str
 
 DEFAULT_DATASTORE: str
 
 DEFAULT_ENVIRONMENT: str
 
 DEFAULT_EVENT_LOGGER: str
 
 DEFAULT_METADATA: str
 
 DEFAULT_MONITOR: str
 
 DEFAULT_PACKAGE_SUFFIXES: str
 
+current: metaflow.metaflow_current.Current
+
+LOG_SOURCES: list
+
+DATASTORES: list
+
+ENVIRONMENTS: list
+
+LOGGING_SIDECARS: dict
+
+METADATA_PROVIDERS: list
+
+MONITOR_SIDECARS: dict
+
 class PyLint(object, metaclass=type):
     def __init__(self, fname):
         ...
     def has_pylint(self):
         ...
     def run(self, logger = None, warnings = False, pylint_config = []):
         ...
     ...
 
-LOG_SOURCES: list
+def validate_tags(tags, existing_tags = None):
+    """
+    Raises MetaflowTaggingError if invalid based on these rules:
+    
+    Tag set size is too large. But it's OK if tag set is not larger
+    than an existing tag set (if provided).
+    
+    Then, we validate each tag.  See validate_tag()
+    """
+    ...
 
 UBF_CONTROL: str
 
 UBF_TASK: str
 
 ERASE_TO_EOL: str
 
@@ -108,18 +130,21 @@
 
 def echo_always(line, **kwargs):
     ...
 
 def logger(body = "", system_msg = False, head = "", bad = False, timestamp = True, nl = True):
     ...
 
+def config_merge_cb(ctx, param, value):
+    ...
+
 def common_run_options(func):
     ...
 
-def write_run_id(run_id_file, run_id):
+def write_file(file_path, content):
     ...
 
 def before_run(obj, tags, decospecs):
     ...
 
 def print_metaflow_exception(ex):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.514155                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.728189                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.client.core
     import datetime
     import typing
-    import metaflow.client.core
     import metaflow.events
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.499969                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.714534                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.client.core
-    import metaflow
-    import metaflow.metaflow_current
     import metaflow.events
-    import datetime
+    import metaflow.client.core
     import tarfile
+    import datetime
+    import metaflow.exception
     import typing
+    import metaflow
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/client/filecache.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.517338                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.734733                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.datastore.content_addressed_store
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/clone_util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.514710                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.732792                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/events.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.502015                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.716709                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
     import metaflow
+    import metaflow.events
 
 TYPE_CHECKING: bool
 
 class MetaflowEvent(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, name, id, timestamp, type):
         """
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/exception.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.492522                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.706332                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/flowspec.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.501291                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.715966                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.unbounded_foreach
-    import metaflow.exception
     import metaflow.parameters
     import metaflow.datastore.inputs
+    import metaflow.exception
     import typing
+    import metaflow.unbounded_foreach
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/includefile.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.509863                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.724049                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
+    import metaflow._vendor.click.types
     import metaflow.parameters
+    import io
     import typing
     import metaflow.plugins.datatools.s3.s3
-    import metaflow._vendor.click.types
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/metadata/metadata.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.535673                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.753025                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.metadata.metadata
+    import metaflow.exception
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class MetaflowTaggingError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/metadata/util.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.579200                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.794240                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/metaflow_config.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.493577                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.707319                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
@@ -134,14 +134,16 @@
 
 DEFAULT_RUNTIME_LIMIT: int
 
 UI_URL: None
 
 CONTACT_INFO: dict
 
+DECOSPECS: str
+
 ECS_S3_ACCESS_IAM_ROLE: None
 
 ECS_FARGATE_EXECUTION_ROLE: None
 
 BATCH_JOB_QUEUE: None
 
 BATCH_CONTAINER_IMAGE: None
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/metaflow_current.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.581431                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.797993                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow
     import metaflow.plugins.cards.component_serializer
-    import metaflow.metaflow_current
     import metaflow.events
+    import metaflow
     import typing
+    import metaflow.metaflow_current
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
@@ -238,27 +238,14 @@
         Returns
         -------
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
-    def trigger(self) -> "metaflow.events.Trigger":
-        """
-        (only in the presence of the @trigger, or @trigger_on_finish decorators)
-        
-        Returns `Trigger` if the current run is triggered by an event
-        
-        Returns
-        -------
-        Trigger
-            `Trigger` if triggered by an event
-        """
-        ...
-    @property
     def project_name(self) -> str:
         """
         (only in the presence of the @project decorator)
         
         The name of the project assigned to this flow, i.e. `X` in `@project(name=X)`.
         
         Returns
@@ -317,11 +304,24 @@
         
         Returns
         -------
         bool
             True if the flow is deployed with `--production`.
         """
         ...
+    @property
+    def trigger(self) -> "metaflow.events.Trigger":
+        """
+        (only in the presence of the @trigger, or @trigger_on_finish decorators)
+        
+        Returns `Trigger` if the current run is triggered by an event
+        
+        Returns
+        -------
+        Trigger
+            `Trigger` if triggered by an event
+        """
+        ...
     ...
 
 current: Current
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/multicore_utils.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.493996                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.707823                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/parameters.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.495083                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.708971                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import metaflow.exception
     import metaflow._vendor.click.types
     import metaflow.parameters
+    import metaflow.exception
+    import typing
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.503607                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.718176                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.unbounded_foreach
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.546291                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.773718                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow._vendor.click.types
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow._vendor.click.types
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.547269                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.774649                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.544199                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.771814                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.543824                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.771343                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.544423                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.782079                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,15 +13,10 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
-    def __init__(self, msg):
-        ...
-    ...
-
-class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
+class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.544654                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.772285                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.569177                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.794725                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
 
 class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, msg):
         ...
     ...
 
 class AirflowTask(object, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.569567                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.795102                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
-    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.569911                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.795443                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
     import metaflow.exception
-    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.559162                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.758229                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.557822                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.756846                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.563290                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.762147                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.parameters
+    import metaflow._vendor.click.types
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow._vendor.click.types
-    import metaflow.parameters
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.564849                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.763697                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
+    import metaflow.parameters
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.parameters
+    import metaflow.decorators
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.558589                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.757586                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.events
     import metaflow.decorators
+    import metaflow.metaflow_current
     import metaflow
+    import metaflow.events
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.514455                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.731869                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.550132                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.754185                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.576936                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.787186                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.578239                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.788514                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.575902                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.786211                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.577653                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.787940                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.578630                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.793528                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.secrets
-    import metaflow.exception
     import abc
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.570368                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.788728                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.571199                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.789763                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/production_token.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/production_token.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.570151                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.789497                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def new_token(token_prefix, prev_token = None):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.570924                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.737817                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.573435                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.791935                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.574655                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.793128                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
+    import metaflow.parameters
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.parameters
+    import metaflow.decorators
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.571508                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.793947                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
-AWS_SANDBOX_ENABLED: bool
-
-AWS_SANDBOX_REGION: None
+def aws_retry(f):
+    ...
 
-SFN_EXECUTION_LOG_GROUP_ARN: None
+def get_s3_client(s3_role_arn = None, s3_session_vars = None, s3_client_params = None):
+    ...
 
-class StepFunctionsClient(object, metaclass=type):
-    def __init__(self):
-        ...
-    def search(self, name):
-        ...
-    def push(self, name, definition, role_arn, log_execution_history):
+class S3Tail(object, metaclass=type):
+    def __init__(self, s3url):
         ...
-    def get(self, name):
+    def reset_client(self, hard_reset = False):
         ...
-    def trigger(self, state_machine_arn, input):
+    def clone(self, s3url):
         ...
-    def list_executions(self, state_machine_arn, states):
+    @property
+    def bytes_read(self):
         ...
-    def terminate_execution(self, execution_arn):
+    @property
+    def tail(self):
         ...
-    def get_state_machine_arn(self, name):
+    def __iter__(self):
         ...
-    def delete(self, name):
+    def _make_range_request(self, *args, **kwargs):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.570755                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.789103                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.566235                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.782984                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.566452                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.772044                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,16 +13,15 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowAzureAuthenticationError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class MetaflowAzureResourceError(metaflow.exception.MetaflowException, metaclass=type):
+class AirflowException(metaflow.exception.MetaflowException, metaclass=type):
+    def __init__(self, msg):
+        ...
     ...
 
-class MetaflowAzurePackageError(metaflow.exception.MetaflowException, metaclass=type):
+class NotSupportedException(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/azure_secret_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.567586                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.784392                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.secrets
-    import metaflow.exception
     import abc
+    import metaflow.exception
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.566845                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.783641                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.567167                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.783965                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.530676                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.747087                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.542828                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.781605                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.parameters
     import metaflow.client.core
     import datetime
-    import metaflow.parameters
+    import metaflow.exception
     import typing
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.532212                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.748661                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.plugins.cards.card_client
+    import metaflow.exception
     import metaflow
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.538742                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.777222                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.540184                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.779011                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.539446                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.778275                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class CardComponentCollector(object, metaclass=type):
     def __init__(self, logger = None, card_creator = None):
         ...
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.536466                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.775100                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.526197                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.742912                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.532616                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.749055                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.568606                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.795823                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.580304                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.796972                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.579932                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.796595                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.579562                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.796227                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.534470                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.750877                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
     import metaflow.plugins.cards.card_modules.card
     import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
+    import typing
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.568039                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.784746                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.568229                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.784931                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.527350                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.744052                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.540682                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.779523                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.538488                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.776965                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
-    import metaflow.exception
     import metaflow.plugins.cards.card_modules.basic
+    import metaflow.exception
     import metaflow.plugins.cards.card_modules.components
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.537080                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.775692                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.522244                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.738712                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.520658                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.737422                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import io
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.530201                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.746630                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.552287                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.756421                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import io
-    import metaflow.plugins.datatools.s3.s3
     import metaflow.exception
+    import metaflow.plugins.datatools.s3.s3
+    import io
 
 class RangeInfo(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, total_size: int, request_offset: int = 0, request_length: int = -1):
         """
         Create new instance of RangeInfo(total_size, request_offset, request_length)
         """
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.506921                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.721246                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.metaflow_current
     import io
     import metaflow.datastore.inputs
+    import metaflow.exception
     import typing
     import metaflow.plugins.datatools.s3.s3
+    import metaflow.metaflow_current
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.578963                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.738017                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
-def aws_retry(f):
-    ...
-
-def get_s3_client(s3_role_arn = None, s3_session_vars = None, s3_client_params = None):
-    ...
-
-class S3Tail(object, metaclass=type):
-    def __init__(self, s3url):
-        ...
-    def reset_client(self, hard_reset = False):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
-    def clone(self, s3url):
-        ...
-    @property
-    def bytes_read(self):
-        ...
-    @property
-    def tail(self):
-        ...
-    def __iter__(self):
-        ...
-    def _make_range_request(self, *args, **kwargs):
+    def __str__(self):
         ...
     ...
 
+MAGIC_FILE: str
+
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.529572                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.746107                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/debug_logger.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.523971                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.740930                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.event_logger
+    import metaflow.monitor
 
-class DebugEventLogger(metaflow.event_logger.NullEventLogger, metaclass=type):
+class DebugMonitor(metaflow.monitor.NullMonitor, metaclass=type):
     @classmethod
     def get_worker(cls):
         ...
     ...
 
-class DebugEventLoggerSidecar(object, metaclass=type):
+class DebugMonitorSidecar(object, metaclass=type):
     def __init__(self):
         ...
     def process_message(self, msg):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/debug_monitor.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.524190                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.705118                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.monitor
+    import metaflow.exception
 
-class DebugMonitor(metaflow.monitor.NullMonitor, metaclass=type):
-    @classmethod
-    def get_worker(cls):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
+    def __str__(self):
+        ...
+    ...
+
+CLIENT_REFRESH_INTERVAL_SECONDS: int
+
+class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class DebugMonitorSidecar(object, metaclass=type):
+class KubernetesClient(object, metaclass=type):
     def __init__(self):
         ...
-    def process_message(self, msg):
+    def get(self):
+        ...
+    def job(self, **kwargs):
+        ...
+    def jobset(self, **kwargs):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.521098                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.789278                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class EnvironmentDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
+class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.522814                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.739867                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.557441                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.753734                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.decorators
+    import metaflow.metaflow_current
     import metaflow.plugins.parallel_decorator
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.566041                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.782782                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.secrets
-    import metaflow.exception
     import abc
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.565328                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.732153                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,10 +13,19 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
+        ...
+    def run(self, logger = None, warnings = False, pylint_config = []):
+        ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.565616                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.782370                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.531135                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.747577                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.554298                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.767699                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.557055                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.770410                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow._vendor.click.types
+    import metaflow.exception
     import metaflow.decorators
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.491304                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.739546                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
+    import metaflow.decorators
+    import metaflow.metaflow_current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-CLIENT_REFRESH_INTERVAL_SECONDS: int
+current: metaflow.metaflow_current.Current
 
-class KubernetesClientException(metaflow.exception.MetaflowException, metaclass=type):
-    ...
+VALID_NAME_RE: str
 
-class KubernetesClient(object, metaclass=type):
-    def __init__(self):
-        ...
-    def get(self):
-        ...
-    def job(self, **kwargs):
+VALID_NAME_LEN: int
+
+class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
-    def jobset(self, **kwargs):
+    def get_top_level_options(self):
         ...
     ...
 
+def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+    ...
+
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.556144                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.769473                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.decorators
     import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/kubernetes/kubernetes_jobsets.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.555178                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.768549                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/logs_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/logs_cli.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.527944                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.745586                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.logs_cli
-    import metaflow.exception
     import metaflow._vendor.click.core
+    import metaflow.exception
+    import metaflow.plugins.logs_cli
 
 LOGGER_TIMESTAMP: str
 
 class CommandException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 LOG_SOURCES: list
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.521532                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.735710                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/perimeters.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/perimeters.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.491600                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.705422                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/project_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.523138                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.765918                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.decorators
+    import metaflow.metaflow_environment
+    import metaflow.plugins.pypi.conda_environment
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
+class CondaEnvironment(metaflow.metaflow_environment.MetaflowEnvironment, metaclass=type):
+    def __init__(self, flow):
         ...
-    def __str__(self):
+    def set_local_root(self, local_root):
         ...
-    ...
-
-current: metaflow.metaflow_current.Current
-
-VALID_NAME_RE: str
-
-VALID_NAME_LEN: int
-
-class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+    def decospecs(self):
+        ...
+    def validate_environment(self, echo, datastore_type):
+        ...
+    def init_environment(self, echo):
+        ...
+    def executable(self, step_name, default = None):
+        ...
+    def interpreter(self, step_name):
+        ...
+    def is_disabled(self, step):
+        ...
+    def pylint_config(self):
+        ...
+    @classmethod
+    def get_client_info(cls, flow_name, metadata):
+        ...
+    def add_to_package(self):
+        ...
+    def bootstrap_commands(self, step_name, datastore_type):
+        ...
+    def get_environment_manifest_path(self):
+        ...
+    def read_from_environment_manifest(self, keys):
         ...
-    def get_top_level_options(self):
+    def write_to_environment_manifest(self, keys, value):
         ...
     ...
 
-def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+class PyPIEnvironment(metaflow.plugins.pypi.conda_environment.CondaEnvironment, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.518763                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.735924                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.decorators
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
-        ...
-    def __str__(self):
-        ...
+class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
-MAGIC_FILE: str
-
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.547813                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.764243                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.549152                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.765530                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_environment
     import io
     import metaflow.exception
     import abc
-    import metaflow.metaflow_environment
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.549557                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.735216                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.pypi.conda_environment
-    import metaflow.metaflow_environment
+    import metaflow.unbounded_foreach
+    import metaflow.decorators
 
-class CondaEnvironment(metaflow.metaflow_environment.MetaflowEnvironment, metaclass=type):
-    def __init__(self, flow):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
-    def set_local_root(self, local_root):
+    def __str__(self):
         ...
-    def decospecs(self):
-        ...
-    def validate_environment(self, echo, datastore_type):
+    ...
+
+UBF_CONTROL: str
+
+UBF_TASK: str
+
+class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
+    def __init__(self, iterable):
         ...
-    def init_environment(self, echo):
+    def __iter__(self):
         ...
-    def executable(self, step_name, default = None):
+    def __next__(self):
         ...
-    def interpreter(self, step_name):
+    def __getitem__(self, key):
         ...
-    def is_disabled(self, step):
+    def __len__(self):
         ...
-    def pylint_config(self):
+    def __str__(self):
         ...
-    @classmethod
-    def get_client_info(cls, flow_name, metadata):
+    def __repr__(self):
         ...
-    def add_to_package(self):
+    ...
+
+class InternalTestUnboundedForeachDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, attributes = None, statically_defined = False):
         ...
-    def bootstrap_commands(self, step_name, datastore_type):
+    def step_init(self, flow, graph, step_name, decorators, environment, flow_datastore, logger):
         ...
-    def get_environment_manifest_path(self):
+    def control_task_step_func(self, flow, graph, retry_count):
         ...
-    def read_from_environment_manifest(self, keys):
+    def task_decorate(self, step_func, flow, graph, retry_count, max_user_code_retries, ubf_context):
         ...
-    def write_to_environment_manifest(self, keys, value):
+    def step_task_retry_count(self):
         ...
     ...
 
-class PyPIEnvironment(metaflow.plugins.pypi.conda_environment.CondaEnvironment, metaclass=type):
-    ...
-
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/pypi/utils.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.548349                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.764780                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/retry_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.522494                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.740334                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAX_ATTEMPTS: int
-
-class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+class StorageExecutor(object, metaclass=type):
+    def __init__(self, use_processes = False):
+        ...
+    def warm_up(self):
         ...
-    def step_task_retry_count(self):
+    def submit(self, *args, **kwargs):
         ...
     ...
 
+def handle_executor_exceptions(func):
+    """
+    Decorator for handling errors that come from an Executor. This decorator should
+    only be used on functions where executor errors are possible. I.e. the function
+    uses StorageExecutor.
+    """
+    ...
+
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.520931                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.738230                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.553229                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.766726                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.secrets
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.552974                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.766485                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.529167                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.745165                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.client.core
-    import metaflow.metaflow_current
     import metaflow.events
+    import metaflow.client.core
     import datetime
+    import metaflow.exception
+    import metaflow.metaflow_current
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/plugins/timeout_decorator.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/procpoll.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.518213                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.732548                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
-    import metaflow.decorators
+    import metaflow.procpoll
 
-class MetaflowException(Exception, metaclass=type):
-    def __init__(self, msg = "", lineno = None):
-        ...
-    def __str__(self):
+class ProcPollEvent(object, metaclass=type):
+    def __init__(self, fd, can_read = False, is_terminated = False):
         ...
     ...
 
-UBF_CONTROL: str
-
-DEFAULT_RUNTIME_LIMIT: int
+class ProcPoll(object, metaclass=type):
+    def poll(self):
+        ...
+    def add(self, fd):
+        ...
+    def remove(self, fd):
+        ...
+    ...
 
-class TimeoutException(metaflow.exception.MetaflowException, metaclass=type):
+class LinuxProcPoll(ProcPoll, metaclass=type):
+    def __init__(self):
+        ...
+    def add(self, fd):
+        ...
+    def remove(self, fd):
+        ...
+    def poll(self, timeout):
+        ...
     ...
 
-class TimeoutDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def __init__(self, *args, **kwargs):
+class DarwinProcPoll(ProcPoll, metaclass=type):
+    def __init__(self):
         ...
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+    def add(self, fd):
         ...
-    def task_pre_step(self, step_name, task_datastore, metadata, run_id, task_id, flow, graph, retry_count, max_user_code_retries, ubf_context, inputs):
+    def remove(self, fd):
         ...
-    def task_post_step(self, step_name, flow, graph, retry_count, max_user_code_retries):
+    def poll(self, timeout):
         ...
     ...
 
-def get_run_time_limit_for_task(step_decos):
+def make_poll():
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/procpoll.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,41 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.515112                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.736290                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.procpoll
+    import metaflow.decorators
+    import metaflow.exception
 
-class ProcPollEvent(object, metaclass=type):
-    def __init__(self, fd, can_read = False, is_terminated = False):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
         ...
-    ...
-
-class ProcPoll(object, metaclass=type):
-    def poll(self):
-        ...
-    def add(self, fd):
-        ...
-    def remove(self, fd):
+    def __str__(self):
         ...
     ...
 
-class LinuxProcPoll(ProcPoll, metaclass=type):
-    def __init__(self):
-        ...
-    def add(self, fd):
-        ...
-    def remove(self, fd):
-        ...
-    def poll(self, timeout):
-        ...
+UBF_CONTROL: str
+
+DEFAULT_RUNTIME_LIMIT: int
+
+class TimeoutException(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
-class DarwinProcPoll(ProcPoll, metaclass=type):
-    def __init__(self):
+class TimeoutDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, *args, **kwargs):
         ...
-    def add(self, fd):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
-    def remove(self, fd):
+    def task_pre_step(self, step_name, task_datastore, metadata, run_id, task_id, flow, graph, retry_count, max_user_code_retries, ubf_context, inputs):
         ...
-    def poll(self, timeout):
+    def task_post_step(self, step_name, flow, graph, retry_count, max_user_code_retries):
         ...
     ...
 
-def make_poll():
+def get_run_time_limit_for_task(step_decos):
     ...
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/profilers/__init__.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/profilers/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.491830                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.705655                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class gpu_profile(object, metaclass=type):
     def __init__(self, include_artifacts = True, artifact_prefix = "gpu_profile_", interval = 1):
```

### Comparing `ob-metaflow-stubs-3.7/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-3.8/metaflow-stubs/tagging_util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.16.2+ob(v1)                                                   #
-# Generated on 2024-05-22T22:08:54.495385                                        #
+# MF version: 2.12.0.1+ob(v1)                                                    #
+# Generated on 2024-05-30T17:28:59.709378                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-3.8/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 3.7
+Version: 3.8
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `ob-metaflow-stubs-3.7/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-3.8/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -132,11 +132,15 @@
 metaflow-stubs/plugins/pypi/pypi_decorator.pyi
 metaflow-stubs/plugins/pypi/pypi_environment.pyi
 metaflow-stubs/plugins/pypi/utils.pyi
 metaflow-stubs/plugins/secrets/__init__.pyi
 metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
 metaflow-stubs/plugins/secrets/secrets_decorator.pyi
 metaflow-stubs/profilers/__init__.pyi
+metaflow-stubs/runner/__init__.pyi
+metaflow-stubs/runner/metaflow_runner.pyi
+metaflow-stubs/runner/nbrun.pyi
+metaflow-stubs/runner/subprocess_manager.pyi
 ob_metaflow_stubs.egg-info/PKG-INFO
 ob_metaflow_stubs.egg-info/SOURCES.txt
 ob_metaflow_stubs.egg-info/dependency_links.txt
 ob_metaflow_stubs.egg-info/top_level.txt
```

### Comparing `ob-metaflow-stubs-3.7/setup.py` & `ob-metaflow-stubs-3.8/setup.py`

 * *Files identical despite different names*

