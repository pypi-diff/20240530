# Comparing `tmp/mosaicml-cli-0.6.8.tar.gz` & `tmp/mosaicml-cli-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.6.8.tar", last modified: Thu Feb 15 21:58:36 2024, max compression
+gzip compressed data, was "mosaicml-cli-0.6.9.tar", last modified: Thu Feb 22 20:43:08 2024, max compression
```

## Comparing `mosaicml-cli-0.6.8.tar` & `mosaicml-cli-0.6.9.tar`

### file list

```diff
@@ -1,249 +1,250 @@
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.166924 mosaicml-cli-0.6.8/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4686 2024-02-15 21:58:36.166583 mosaicml-cli-0.6.8/PKG-INFO
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     7086 2023-12-08 23:08:16.000000 mosaicml-cli-0.6.8/README.md
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.105957 mosaicml-cli-0.6.8/mcli/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3256 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/__init__.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.106710 mosaicml-cli-0.6.8/mcli/admin/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      349 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/admin/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2234 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/admin/helpers.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.107843 mosaicml-cli-0.6.8/mcli/api/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/__init__.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.108377 mosaicml-cli-0.6.8/mcli/api/cluster/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      283 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/cluster/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8508 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.108881 mosaicml-cli-0.6.8/mcli/api/code_eval/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      373 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/code_eval/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3355 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/code_eval/api_get_code_eval_output.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.109660 mosaicml-cli-0.6.8/mcli/api/engine/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/engine/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    30942 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/engine/engine.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1362 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/engine/retry.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    13426 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/exceptions.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.111289 mosaicml-cli-0.6.8/mcli/api/finetuning_runs/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      948 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/finetuning_runs/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    13806 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_create_finetuning_run.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6045 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_delete_finetuning_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8800 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_get_finetuning_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3201 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_list_finetuning_events.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6658 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_stop_finetuning_runs.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.114637 mosaicml-cli-0.6.8/mcli/api/inference_deployments/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1957 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3909 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_create_default_deployment.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3300 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5204 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4423 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8757 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2045 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3656 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5166 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_stop_inference_deployments.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6628 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.115527 mosaicml-cli-0.6.8/mcli/api/mint/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/mint/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8451 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/mint/shell.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3266 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/mint/tty.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.117860 mosaicml-cli-0.6.8/mcli/api/model/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1203 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/model/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     9838 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/model/cluster_details.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4569 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/model/finetune.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6089 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/model/inference_deployment.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      900 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/model/lambda_response.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    18945 2023-11-13 23:14:40.000000 mosaicml-cli-0.6.8/mcli/api/model/run.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8826 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/model/run_debug_info.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1454 2023-12-08 23:08:16.000000 mosaicml-cli-0.6.8/mcli/api/model/run_event.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1139 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/model/user.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.122604 mosaicml-cli-0.6.8/mcli/api/runs/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1463 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/runs/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3758 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_create_interactive_run.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3033 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_create_run.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2878 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_create_run_event.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4485 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2323 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_get_run_debug_info.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    15388 2024-02-15 21:57:58.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    11211 2024-02-15 21:42:33.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5442 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_start_run.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6244 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5886 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_update_run.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6150 2023-12-08 23:08:16.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    10049 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.123027 mosaicml-cli-0.6.8/mcli/api/schema/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/schema/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      636 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.124390 mosaicml-cli-0.6.8/mcli/api/secrets/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      309 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/secrets/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2386 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3057 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3779 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2354 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/typing_future.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.124857 mosaicml-cli-0.6.8/mcli/api/users/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      139 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/users/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2802 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/api/users/api_get_users.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      920 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/api/utils.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.125537 mosaicml-cli-0.6.8/mcli/cli/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/__init__.py
--rwxr-xr-x   0 jimmy.xu   (502) staff       (20)     6865 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/cli.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.126734 mosaicml-cli-0.6.8/mcli/cli/common/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/common/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2532 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5275 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/common/finetuning_run_filters.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     7466 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.127235 mosaicml-cli-0.6.8/mcli/cli/m_connect/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6940 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.128141 mosaicml-cli-0.6.8/mcli/cli/m_create/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_create/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2385 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_create/m_create.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    19400 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.128860 mosaicml-cli-0.6.8/mcli/cli/m_debug/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_debug/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1220 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_debug/debug_run.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1482 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_debug/m_debug.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.129704 mosaicml-cli-0.6.8/mcli/cli/m_delete/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     7903 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_delete/delete.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     7538 2023-11-13 23:14:40.000000 mosaicml-cli-0.6.8/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.130237 mosaicml-cli-0.6.8/mcli/cli/m_deploy/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4253 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.132398 mosaicml-cli-0.6.8/mcli/cli/m_describe/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5859 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_clusters.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4325 2023-11-23 00:12:15.000000 mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_finetuning_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4282 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    13087 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2293 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_users.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4527 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.132898 mosaicml-cli-0.6.8/mcli/cli/m_finetune/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_finetune/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5545 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_finetune/m_finetune.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.135517 mosaicml-cli-0.6.8/mcli/cli/m_get/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      467 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6996 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/clusters.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     7837 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/display.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6509 2023-11-13 23:14:40.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/finetuning_runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     7412 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4997 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/m_get.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    13719 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/runs.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2069 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/secrets.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1601 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_get/users.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.136126 mosaicml-cli-0.6.8/mcli/cli/m_init/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_init/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3909 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.136568 mosaicml-cli-0.6.8/mcli/cli/m_interactive/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8377 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.138079 mosaicml-cli-0.6.8/mcli/cli/m_kube/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5523 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1398 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2050 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6946 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.138644 mosaicml-cli-0.6.8/mcli/cli/m_log/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_log/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    17700 2024-02-15 21:57:58.000000 mosaicml-cli-0.6.8/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.139162 mosaicml-cli-0.6.8/mcli/cli/m_ping/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1407 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.139680 mosaicml-cli-0.6.8/mcli/cli/m_predict/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2216 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.140126 mosaicml-cli-0.6.8/mcli/cli/m_root/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_root/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      536 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.140724 mosaicml-cli-0.6.8/mcli/cli/m_run/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_run/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    12796 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.142942 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2964 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1793 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2267 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1656 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      840 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/organization.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1931 2023-12-08 23:08:16.000000 mosaicml-cli-0.6.8/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.143590 mosaicml-cli-0.6.8/mcli/cli/m_stop/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     9552 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.144088 mosaicml-cli-0.6.8/mcli/cli/m_update/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_update/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8832 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_update/m_update.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.144933 mosaicml-cli-0.6.8/mcli/cli/m_util/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_util/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1189 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_util/m_util.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    10957 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/cli/m_util/util.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.145545 mosaicml-cli-0.6.8/mcli/cli/m_watchdog/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_watchdog/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3615 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/cli/m_watchdog/m_watchdog.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    13360 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/config.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.148250 mosaicml-cli-0.6.8/mcli/models/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1412 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/models/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5664 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/models/common.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5813 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/models/finetune_config.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      623 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/models/finetune_task_type.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2103 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/models/gpu_type.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    15087 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/models/inference_deployment_config.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      239 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/models/lambda_input.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     8771 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/models/mcli_secret.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    15002 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/models/run_config.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.148610 mosaicml-cli-0.6.8/mcli/objects/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/__init__.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.150933 mosaicml-cli-0.6.8/mcli/objects/secrets/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1271 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.153766 mosaicml-cli-0.6.8/mcli/objects/secrets/create/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1646 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/base.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1277 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/databricks.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2244 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2408 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6377 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1412 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/hugging_face.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3858 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4276 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5342 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      691 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/databricks.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      783 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1278 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/env_var.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      556 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/gcp.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1267 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/mounted.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      967 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/oci.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1028 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/s3.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1718 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.154710 mosaicml-cli-0.6.8/mcli/proto/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/proto/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1477 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/proto/mint_pb2.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1098 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/proto/mint_pb2.pyi
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.155039 mosaicml-cli-0.6.8/mcli/sdk/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)      319 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/sdk/__init__.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.159870 mosaicml-cli-0.6.8/mcli/utils/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        0 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/__init__.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6318 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_cli.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5039 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/utils/utils_completers.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    11372 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/utils/utils_config.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1684 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_date.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2225 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_epilog.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     7118 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_finetune.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    10774 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_interactive.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4503 2023-12-08 23:08:16.000000 mosaicml-cli-0.6.8/mcli/utils/utils_logging.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1631 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1042 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_model.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6288 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/utils/utils_pypi.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3470 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_rich.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     5358 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_run_status.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1103 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_spinner.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    11809 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_string_functions.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     2044 2024-02-14 23:33:47.000000 mosaicml-cli-0.6.8/mcli/utils/utils_types.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1001 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/mcli/utils/utils_yaml.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3890 2024-02-15 21:58:17.000000 mosaicml-cli-0.6.8/mcli/version.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.162662 mosaicml-cli-0.6.8/mosaicml_cli.egg-info/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     4686 2024-02-15 21:58:36.000000 mosaicml-cli-0.6.8/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6432 2024-02-15 21:58:36.000000 mosaicml-cli-0.6.8/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        1 2024-02-15 21:58:36.000000 mosaicml-cli-0.6.8/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jimmy.xu   (502) staff       (20)       75 2024-02-15 21:58:36.000000 mosaicml-cli-0.6.8/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     1680 2024-02-15 21:58:36.000000 mosaicml-cli-0.6.8/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 jimmy.xu   (502) staff       (20)        5 2024-02-15 21:58:36.000000 mosaicml-cli-0.6.8/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 jimmy.xu   (502) staff       (20)    31087 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/pyproject.toml
--rw-r--r--   0 jimmy.xu   (502) staff       (20)       38 2024-02-15 21:58:36.166981 mosaicml-cli-0.6.8/setup.cfg
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     3096 2023-12-08 23:08:16.000000 mosaicml-cli-0.6.8/setup.py
-drwxr-xr-x   0 jimmy.xu   (502) staff       (20)        0 2024-02-15 21:58:36.162278 mosaicml-cli-0.6.8/tests/
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6449 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/tests/test_config.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)       62 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/tests/test_simple.py
--rw-r--r--   0 jimmy.xu   (502) staff       (20)     6116 2023-11-08 00:21:50.000000 mosaicml-cli-0.6.8/tests/test_upgrade.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.605723 mosaicml-cli-0.6.9/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4686 2024-02-22 20:43:08.605273 mosaicml-cli-0.6.9/PKG-INFO
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     7086 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/README.md
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.535137 mosaicml-cli-0.6.9/mcli/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3256 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/__init__.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.535939 mosaicml-cli-0.6.9/mcli/admin/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      349 2023-11-16 19:59:08.000000 mosaicml-cli-0.6.9/mcli/admin/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2234 2023-11-16 19:59:08.000000 mosaicml-cli-0.6.9/mcli/admin/helpers.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.537297 mosaicml-cli-0.6.9/mcli/api/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/api/__init__.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.538200 mosaicml-cli-0.6.9/mcli/api/cluster/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      283 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/cluster/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8508 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.539248 mosaicml-cli-0.6.9/mcli/api/code_eval/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      373 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/code_eval/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3355 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/code_eval/api_get_code_eval_output.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.540569 mosaicml-cli-0.6.9/mcli/api/engine/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/api/engine/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    30942 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/api/engine/engine.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1362 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/engine/retry.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    13426 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/exceptions.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.543074 mosaicml-cli-0.6.9/mcli/api/finetuning_runs/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      948 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/finetuning_runs/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    13806 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_create_finetuning_run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6045 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_delete_finetuning_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8800 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_get_finetuning_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3201 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_list_finetuning_events.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6658 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_stop_finetuning_runs.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.547274 mosaicml-cli-0.6.9/mcli/api/inference_deployments/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1957 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3909 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_create_default_deployment.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3300 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5204 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4423 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8757 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2045 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3656 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5166 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_stop_inference_deployments.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6628 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.548282 mosaicml-cli-0.6.9/mcli/api/mint/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-02-27 19:44:05.000000 mosaicml-cli-0.6.9/mcli/api/mint/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8451 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/mint/shell.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3266 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/mint/tty.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.551307 mosaicml-cli-0.6.9/mcli/api/model/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1203 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/model/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     9838 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/model/cluster_details.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4569 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/model/finetune.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6089 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      900 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/model/lambda_response.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    19673 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/model/run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8826 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/model/run_debug_info.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1454 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/model/run_event.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1139 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/model/user.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.555947 mosaicml-cli-0.6.9/mcli/api/runs/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1463 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/api/runs/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3784 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_create_interactive_run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3059 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2878 2023-11-16 19:59:08.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_create_run_event.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4511 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2323 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_get_run_debug_info.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    15388 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    12529 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5468 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6270 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5912 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_update_run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6176 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    10049 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.556702 mosaicml-cli-0.6.9/mcli/api/schema/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/api/schema/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      636 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.558081 mosaicml-cli-0.6.9/mcli/api/secrets/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      309 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/api/secrets/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2386 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3057 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3779 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2354 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/api/typing_future.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.558765 mosaicml-cli-0.6.9/mcli/api/users/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      139 2023-01-27 22:04:36.000000 mosaicml-cli-0.6.9/mcli/api/users/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3083 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/api/users/api_get_users.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      920 2023-07-16 04:54:11.000000 mosaicml-cli-0.6.9/mcli/api/utils.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.559219 mosaicml-cli-0.6.9/mcli/cli/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/__init__.py
+-rwxr-xr-x   0 nancy.hung   (502) staff       (20)     6865 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/cli.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.561118 mosaicml-cli-0.6.9/mcli/cli/common/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-27 21:57:37.000000 mosaicml-cli-0.6.9/mcli/cli/common/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2532 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5275 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/common/finetuning_run_filters.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     7466 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.561698 mosaicml-cli-0.6.9/mcli/cli/m_connect/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-02-27 19:44:05.000000 mosaicml-cli-0.6.9/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6940 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.562716 mosaicml-cli-0.6.9/mcli/cli/m_create/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2385 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    19400 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.563793 mosaicml-cli-0.6.9/mcli/cli/m_debug/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_debug/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1220 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_debug/debug_run.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1482 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_debug/m_debug.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.564737 mosaicml-cli-0.6.9/mcli/cli/m_delete/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     7903 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     7538 2023-11-16 19:59:08.000000 mosaicml-cli-0.6.9/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.565502 mosaicml-cli-0.6.9/mcli/cli/m_deploy/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-03-11 00:15:00.000000 mosaicml-cli-0.6.9/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4253 2023-08-22 20:49:45.000000 mosaicml-cli-0.6.9/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.567980 mosaicml-cli-0.6.9/mcli/cli/m_describe/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-23 18:20:34.000000 mosaicml-cli-0.6.9/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5859 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_clusters.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4325 2023-11-19 22:26:22.000000 mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_finetuning_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4282 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    13087 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2293 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_users.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4527 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.568677 mosaicml-cli-0.6.9/mcli/cli/m_finetune/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_finetune/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5545 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_finetune/m_finetune.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.573023 mosaicml-cli-0.6.9/mcli/cli/m_get/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      547 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6996 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     7837 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/display.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6509 2023-11-16 19:59:08.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/finetuning_runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     7412 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5626 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1236 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/organizations.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    13719 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/runs.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2069 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1633 2024-02-22 20:42:00.000000 mosaicml-cli-0.6.9/mcli/cli/m_get/users.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.573662 mosaicml-cli-0.6.9/mcli/cli/m_init/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3909 2023-11-16 19:59:08.000000 mosaicml-cli-0.6.9/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.574505 mosaicml-cli-0.6.9/mcli/cli/m_interactive/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8377 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.576463 mosaicml-cli-0.6.9/mcli/cli/m_kube/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5523 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1398 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2050 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6946 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.577002 mosaicml-cli-0.6.9/mcli/cli/m_log/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    17700 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.577857 mosaicml-cli-0.6.9/mcli/cli/m_ping/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-03-27 18:32:10.000000 mosaicml-cli-0.6.9/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1407 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.578392 mosaicml-cli-0.6.9/mcli/cli/m_predict/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-03-27 18:32:10.000000 mosaicml-cli-0.6.9/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2216 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.578892 mosaicml-cli-0.6.9/mcli/cli/m_root/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      536 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.579392 mosaicml-cli-0.6.9/mcli/cli/m_run/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    12796 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.581570 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2964 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1793 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2267 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1656 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      840 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/organization.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1931 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.582144 mosaicml-cli-0.6.9/mcli/cli/m_stop/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     9552 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.582818 mosaicml-cli-0.6.9/mcli/cli/m_update/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/mcli/cli/m_update/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8832 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_update/m_update.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.583796 mosaicml-cli-0.6.9/mcli/cli/m_util/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1189 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    10957 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/cli/m_util/util.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.584345 mosaicml-cli-0.6.9/mcli/cli/m_watchdog/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/mcli/cli/m_watchdog/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3615 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/cli/m_watchdog/m_watchdog.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    13360 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/config.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.587683 mosaicml-cli-0.6.9/mcli/models/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1412 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/models/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5664 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/models/common.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5813 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/models/finetune_config.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      623 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/models/finetune_task_type.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2103 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/models/gpu_type.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    15087 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      239 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/models/lambda_input.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     8771 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/models/mcli_secret.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    15002 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/models/run_config.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.588154 mosaicml-cli-0.6.9/mcli/objects/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/objects/__init__.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.590394 mosaicml-cli-0.6.9/mcli/objects/secrets/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1271 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.593338 mosaicml-cli-0.6.9/mcli/objects/secrets/create/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1646 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1277 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/databricks.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2244 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2408 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6377 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1412 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/hugging_face.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3858 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4276 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5342 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      691 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/databricks.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      783 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1278 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      556 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1267 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      967 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/oci.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1028 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/s3.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1718 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.594240 mosaicml-cli-0.6.9/mcli/proto/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-04-26 15:39:03.000000 mosaicml-cli-0.6.9/mcli/proto/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1477 2023-04-26 15:39:03.000000 mosaicml-cli-0.6.9/mcli/proto/mint_pb2.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1098 2023-04-26 15:39:03.000000 mosaicml-cli-0.6.9/mcli/proto/mint_pb2.pyi
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.594552 mosaicml-cli-0.6.9/mcli/sdk/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)      319 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/sdk/__init__.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.599839 mosaicml-cli-0.6.9/mcli/utils/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        0 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/utils/__init__.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6318 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/utils/utils_cli.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5039 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/utils/utils_completers.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    11372 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/utils/utils_config.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1684 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/utils/utils_date.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2225 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/utils/utils_epilog.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     7118 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/utils/utils_finetune.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    10774 2023-06-22 00:52:50.000000 mosaicml-cli-0.6.9/mcli/utils/utils_interactive.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4503 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/mcli/utils/utils_logging.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1631 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1042 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/utils/utils_model.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6288 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/utils/utils_pypi.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3470 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/utils/utils_rich.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     5358 2023-08-22 20:49:45.000000 mosaicml-cli-0.6.9/mcli/utils/utils_run_status.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1103 2023-03-13 21:15:25.000000 mosaicml-cli-0.6.9/mcli/utils/utils_spinner.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    11809 2023-10-25 04:49:20.000000 mosaicml-cli-0.6.9/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     2044 2024-02-21 20:58:53.000000 mosaicml-cli-0.6.9/mcli/utils/utils_types.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1001 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/mcli/utils/utils_yaml.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3890 2024-02-22 20:42:06.000000 mosaicml-cli-0.6.9/mcli/version.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.602437 mosaicml-cli-0.6.9/mosaicml_cli.egg-info/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     4686 2024-02-22 20:43:08.000000 mosaicml-cli-0.6.9/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6464 2024-02-22 20:43:08.000000 mosaicml-cli-0.6.9/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        1 2024-02-22 20:43:08.000000 mosaicml-cli-0.6.9/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)       75 2024-02-22 20:43:08.000000 mosaicml-cli-0.6.9/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     1680 2024-02-22 20:43:08.000000 mosaicml-cli-0.6.9/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)        5 2024-02-22 20:43:08.000000 mosaicml-cli-0.6.9/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 nancy.hung   (502) staff       (20)    31087 2023-05-12 17:52:25.000000 mosaicml-cli-0.6.9/pyproject.toml
+-rw-r--r--   0 nancy.hung   (502) staff       (20)       38 2024-02-22 20:43:08.605783 mosaicml-cli-0.6.9/setup.cfg
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     3096 2024-01-16 22:39:32.000000 mosaicml-cli-0.6.9/setup.py
+drwxr-xr-x   0 nancy.hung   (502) staff       (20)        0 2024-02-22 20:43:08.602104 mosaicml-cli-0.6.9/tests/
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6449 2023-07-06 18:50:39.000000 mosaicml-cli-0.6.9/tests/test_config.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)       62 2023-01-05 21:09:09.000000 mosaicml-cli-0.6.9/tests/test_simple.py
+-rw-r--r--   0 nancy.hung   (502) staff       (20)     6116 2023-03-15 00:46:33.000000 mosaicml-cli-0.6.9/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.6.8/PKG-INFO` & `mosaicml-cli-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.6.8
+Version: 0.6.9
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,47 +57,47 @@
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "sphinx"
 Requires-Dist: sphinxemoji==0.2.0; extra == "sphinx"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "sphinx"
 Requires-Dist: myst-parser>=0.16.1; extra == "sphinx"
 Requires-Dist: docutils>=0.17.0; extra == "sphinx"
 Requires-Dist: sphinx-design; extra == "sphinx"
 Provides-Extra: all
+Requires-Dist: sphinx-design; extra == "all"
 Requires-Dist: furo==2022.9.29; extra == "all"
-Requires-Dist: radon>=5.1.0; extra == "all"
-Requires-Dist: sphinxcontrib-jsmath>=1.0.1; extra == "all"
+Requires-Dist: yapf>=0.33.0; extra == "all"
+Requires-Dist: sphinxcontrib-applehelp>=1.0.2; extra == "all"
+Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "all"
 Requires-Dist: sphinxcontrib-images>=0.9.4; extra == "all"
+Requires-Dist: sphinxcontrib-katex==0.9.4; extra == "all"
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "all"
-Requires-Dist: yapf>=0.33.0; extra == "all"
-Requires-Dist: sphinx-argparse==0.4.0; extra == "all"
-Requires-Dist: isort>=5.9.3; extra == "all"
+Requires-Dist: sphinxcontrib-qthelp>=1.0.3; extra == "all"
+Requires-Dist: pylint>=2.12.2; extra == "all"
+Requires-Dist: pytest-cov>=4.0.0; extra == "all"
 Requires-Dist: pytest>=6.2.5; extra == "all"
 Requires-Dist: toml>=0.10.2; extra == "all"
-Requires-Dist: pyright==1.1.256; extra == "all"
+Requires-Dist: sphinxemoji==0.2.0; extra == "all"
+Requires-Dist: sphinx-copybutton==0.5.2; extra == "all"
+Requires-Dist: pytest-mock>=3.7.0; extra == "all"
+Requires-Dist: build>=0.10.0; extra == "all"
 Requires-Dist: sphinxcontrib-htmlhelp>=2.0.0; extra == "all"
-Requires-Dist: sphinx_external_toc==0.3.0; extra == "all"
-Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "all"
+Requires-Dist: pyright==1.1.256; extra == "all"
 Requires-Dist: twine>=4.0.2; extra == "all"
-Requires-Dist: sphinxcontrib-devhelp>=1.0.2; extra == "all"
-Requires-Dist: sphinx-copybutton==0.5.2; extra == "all"
-Requires-Dist: sphinxcontrib-katex==0.9.4; extra == "all"
+Requires-Dist: isort>=5.9.3; extra == "all"
+Requires-Dist: sphinx-argparse==0.4.0; extra == "all"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "all"
-Requires-Dist: pytest-mock>=3.7.0; extra == "all"
-Requires-Dist: pylint>=2.12.2; extra == "all"
-Requires-Dist: sphinxcontrib-applehelp>=1.0.2; extra == "all"
+Requires-Dist: radon>=5.1.0; extra == "all"
 Requires-Dist: sphinx-panels==0.6.0; extra == "all"
+Requires-Dist: sphinxcontrib-jsmath>=1.0.1; extra == "all"
+Requires-Dist: sphinx==4.4.0; extra == "all"
 Requires-Dist: docutils>=0.17.0; extra == "all"
 Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: sphinx==4.4.0; extra == "all"
-Requires-Dist: build>=0.10.0; extra == "all"
-Requires-Dist: sphinx-markdown-tables==0.0.17; extra == "all"
-Requires-Dist: sphinxemoji==0.2.0; extra == "all"
+Requires-Dist: sphinx_external_toc==0.3.0; extra == "all"
+Requires-Dist: sphinxcontrib-devhelp>=1.0.2; extra == "all"
 Requires-Dist: myst-parser>=0.16.1; extra == "all"
-Requires-Dist: sphinxcontrib-qthelp>=1.0.3; extra == "all"
-Requires-Dist: sphinx-design; extra == "all"
-Requires-Dist: pytest-cov>=4.0.0; extra == "all"
+Requires-Dist: sphinx-markdown-tables==0.0.17; extra == "all"
 
 
 #  MosaicML CLI (MCLI)
 
 ### MCLI is the interface for interacting with the MosaicML platform
 
 To get started with MCLI, read the [documentation](https://mcli.docs.mosaicml.com/)
```

### Comparing `mosaicml-cli-0.6.8/README.md` & `mosaicml-cli-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/__init__.py` & `mosaicml-cli-0.6.9/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/admin/helpers.py` & `mosaicml-cli-0.6.9/mcli/admin/helpers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.6.9/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/code_eval/api_get_code_eval_output.py` & `mosaicml-cli-0.6.9/mcli/api/code_eval/api_get_code_eval_output.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/engine/engine.py` & `mosaicml-cli-0.6.9/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/engine/retry.py` & `mosaicml-cli-0.6.9/mcli/api/engine/retry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/exceptions.py` & `mosaicml-cli-0.6.9/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/finetuning_runs/__init__.py` & `mosaicml-cli-0.6.9/mcli/api/finetuning_runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_create_finetuning_run.py` & `mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_create_finetuning_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_delete_finetuning_runs.py` & `mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_delete_finetuning_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_get_finetuning_runs.py` & `mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_get_finetuning_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_list_finetuning_events.py` & `mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_list_finetuning_events.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/finetuning_runs/api_stop_finetuning_runs.py` & `mosaicml-cli-0.6.9/mcli/api/finetuning_runs/api_stop_finetuning_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_create_default_deployment.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_create_default_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_stop_inference_deployments.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_stop_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.6.9/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/mint/shell.py` & `mosaicml-cli-0.6.9/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/mint/tty.py` & `mosaicml-cli-0.6.9/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/__init__.py` & `mosaicml-cli-0.6.9/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.6.9/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/finetune.py` & `mosaicml-cli-0.6.9/mcli/api/model/finetune.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.6.9/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/lambda_response.py` & `mosaicml-cli-0.6.9/mcli/api/model/lambda_response.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/run.py` & `mosaicml-cli-0.6.9/mcli/api/model/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ GraphQL representation of MCLIJob"""
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from datetime import datetime
+from datetime import datetime, timezone
 from enum import Enum
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Tuple
 
 from mcli.api.exceptions import MAPIException
 from mcli.api.schema.generic_model import DeserializableModel, convert_datetime
 from mcli.models.run_config import RunConfig
@@ -175,39 +175,32 @@
     retry_on_system_failure: bool
     cluster: str
     gpus: int
     gpu_type: str
     cpus: int
     node_count: int
     latest_resumption: Resumption
+    is_deleted: bool
+    run_type: RunType
 
     max_retries: Optional[int] = None
     reason: Optional[str] = None
     nodes: List[Node] = field(default_factory=list)
     submitted_config: Optional[RunConfig] = None
     metadata: Optional[Dict[str, Any]] = None
     last_resumption_id: Optional[str] = None
     resumptions: List[Resumption] = field(default_factory=list)
     lifecycle: List[RunLifecycle] = field(default_factory=list)
     image: Optional[str] = None
 
     max_duration: Optional[float] = None
 
     _required_properties: Tuple[str] = tuple([
-        'id',
-        'name',
-        'status',
-        'createdAt',
-        'updatedAt',
-        'reason',
-        'createdByEmail',
-        'priority',
-        'preemptible',
-        'retryOnSystemFailure',
-        'resumptions',
+        'id', 'name', 'status', 'createdAt', 'updatedAt', 'reason', 'createdByEmail', 'priority', 'preemptible',
+        'retryOnSystemFailure', 'resumptions', 'isDeleted', 'runType'
     ])
 
     @property
     def started_at(self) -> Optional[datetime]:
         """The time the run was first started
 
         If there are multiple resumptions, this will be the earliest start time
@@ -229,15 +222,15 @@
         If there are multiple resumptions, this will be the last end time
         Completed At will be None if the last resumption has not been completed
 
         Returns:
             The time the run was last completed
         """
 
-        for resumption in self.resumptions[:-1]:
+        for resumption in self.resumptions[::-1]:
             if resumption.ended_at:
                 return resumption.ended_at
 
             # Stopped resumptions are special: you can technically stop a resumption
             # before it starts, resulting in a resumption with no start or end time.
             # For these cases, use the previous resumption's end time (if it exists)
 
@@ -306,14 +299,30 @@
         return len(self.resumptions)
 
     @property
     def max_duration_seconds(self) -> Optional[int]:
         if self.max_duration:
             return int(self.max_duration * 3600)
 
+    def get_gpu_hours(self) -> float:
+        total = 0
+        for resumption in self.resumptions:
+            if not resumption.started_at:
+                continue
+
+            ended_at = resumption.ended_at
+            if not ended_at:
+                if self.latest_resumption.index == resumption.index:
+                    ended_at = datetime.now(timezone.utc)
+                else:
+                    continue
+            total += resumption.gpus * (ended_at - resumption.started_at).total_seconds() / (60 * 60)
+
+        return total
+
     def clone(
         self,
         name: Optional[str] = None,
         image: Optional[str] = None,
         cluster: Optional[str] = None,
         instance: Optional[str] = None,
         nodes: Optional[int] = None,
@@ -494,14 +503,18 @@
             'retry_on_system_failure': response['retryOnSystemFailure'],
             'max_duration': max_duration,
             'cluster': latest_resumption.cluster,
             'gpus': latest_resumption.gpus,
             'gpu_type': latest_resumption.gpu_type,
             'cpus': latest_resumption.cpus,
             'node_count': latest_resumption.node_count,
+
+            # If it's not included in the response, assume it's not deleted
+            'is_deleted': response['isDeleted'],
+            'run_type': RunType(response['runType']),
         }
 
         details = response.get('details', {})
         if details:
             submitted_run_input = details.get('originalRunInput')
             args['submitted_config'] = RunConfig.from_mapi_response(
                 submitted_run_input) if submitted_run_input is not None else None
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/run_debug_info.py` & `mosaicml-cli-0.6.9/mcli/api/model/run_debug_info.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/run_event.py` & `mosaicml-cli-0.6.9/mcli/api/model/run_event.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/model/user.py` & `mosaicml-cli-0.6.9/mcli/api/model/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/__init__.py` & `mosaicml-cli-0.6.9/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_create_interactive_run.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_create_interactive_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     createdAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
+    runType
+    isDeleted
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_create_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     createdAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
+    isDeleted
+    runType
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_create_run_event.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_create_run_event.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_delete_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     createdAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
+    isDeleted
+    runType
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_get_run_debug_info.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_get_run_debug_info.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_get_runs.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     reason
     createdByEmail
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     maxDurationSeconds
+    isDeleted
+    runType
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
@@ -70,14 +72,16 @@
     reason
     createdByEmail
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
     maxDurationSeconds
+    runType
+    isDeleted
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
@@ -184,14 +188,17 @@
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
     user_emails: Optional[List[str]] = None,
     run_types: Optional[Union[List[str], List[RunType]]] = None,
     include_details: bool = False,
+    include_deleted: bool = False,
+    ended_before: Optional[Union[str, datetime]] = None,
+    ended_after: Optional[Union[str, datetime]] = None,
     limit: Optional[int] = None,
 ) -> ObjectList[Run]:
     ...
 
 
 @overload
 def get_runs(
@@ -204,14 +211,17 @@
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     user_emails: Optional[List[str]] = None,
     run_types: Optional[Union[List[str], List[RunType]]] = None,
     include_details: bool = False,
+    include_deleted: bool = False,
+    ended_before: Optional[Union[str, datetime]] = None,
+    ended_after: Optional[Union[str, datetime]] = None,
     limit: Optional[int] = None,
 ) -> Future[ObjectList[Run]]:
     ...
 
 
 def get_runs(
     runs: Optional[Union[List[str], List[Run], ObjectList[Run]]] = None,
@@ -223,14 +233,17 @@
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
     user_emails: Optional[List[str]] = None,
     run_types: Optional[Union[List[str], List[RunType]]] = None,
     include_details: bool = False,
+    include_deleted: bool = False,
+    ended_before: Optional[Union[str, datetime]] = None,
+    ended_after: Optional[Union[str, datetime]] = None,
     limit: Optional[int] = None,
 ):
     """List runs that have been launched in the MosaicML platform
 
     The returned list will contain all of the details stored about the requested runs.
 
     Arguments:
@@ -262,14 +275,17 @@
             value will be ignored.
         future: Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to `get_runs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of runs, use ``return_value.result()``
             with an optional ``timeout`` argument.
         include_details: If true, will fetch detailed information like run input for each run.
+        include_deleted: If true, will include deleted runs in the response.
+        ended_before: Only runs ended strictly before this time will be returned.
+        ended_after: Only runs ended at or after this time will be returned.
         limit: Maximum number of runs to return. If None, all runs will be returned.
 
     Raises:
         MAPIException: If connecting to MAPI, raised when a MAPI communication error occurs
     """
 
     filters = {}
@@ -278,14 +294,24 @@
     if before or after:
         date_filters = {}
         if before:
             date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
         if after:
             date_filters['gte'] = after.astimezone().isoformat() if isinstance(after, datetime) else after
         filters['createdAt'] = date_filters
+    if ended_before or ended_after:
+        date_filters = {}
+        if ended_before:
+            date_filters['lt'] = ended_before.astimezone().isoformat() if isinstance(ended_before,
+                                                                                     datetime) else ended_before
+        if ended_after:
+            date_filters['gte'] = ended_after.astimezone().isoformat() if isinstance(ended_after,
+                                                                                     datetime) else ended_after
+        filters['endedAt'] = date_filters
+
     if statuses:
         filters['status'] = {'in': [s.value.upper() if isinstance(s, RunStatus) else s.upper() for s in statuses]}
 
     if cluster_names:
         filters['clusterName'] = {'in': [c if isinstance(c, str) else c.name for c in cluster_names]}
     if gpu_types:
         filters['gpuType'] = {'in': [gt.value if isinstance(gt, GPUType) else gt for gt in gpu_types]}
@@ -294,15 +320,15 @@
 
     if run_types:
         filters['runType'] = {'in': [r.value.upper() if isinstance(r, RunType) else r.upper() for r in run_types]}
 
     variables = {
         VARIABLE_DATA_NAME_PAGINATED: {
             'filters': filters,
-            'includeDeleted': False,
+            'includeDeleted': include_deleted,
             'limit': limit,
         },
     }
 
     cfg = MCLIConfig.load_config()
     cfg.update_entity(variables[VARIABLE_DATA_NAME_PAGINATED])
     if user_emails:
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_start_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     createdAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
+    runType
+    isDeleted
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_stop_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     createdAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
+    isDeleted
+    runType
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_update_run.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_update_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     createdAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
+    runType
+    isDeleted
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_update_run_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     createdAt
     updatedAt
     reason
     priority
     maxRetries
     preemptible
     retryOnSystemFailure
+    runType
+    isDeleted
     resumptions {{
         clusterName
         cpus
         gpuType
         gpus
         nodes
         executionIndex
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.6.9/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.6.9/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.6.9/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.6.9/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.6.9/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/typing_future.py` & `mosaicml-cli-0.6.9/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.6.9/mcli/api/users/api_get_users.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,43 +29,47 @@
 
 
 @overload
 def get_users(
     users: Optional[Union[List[str], List[User]]] = None,
     *,
     user_emails: Optional[List[str]] = None,
+    organization: Optional[str] = None,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
 ) -> ObjectList[User]:
     ...
 
 
 @overload
 def get_users(
     users: Optional[Union[List[str], List[User]]] = None,
     *,
     user_emails: Optional[List[str]] = None,
+    organization: Optional[str] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
 ) -> Future[ObjectList[User]]:
     ...
 
 
 def get_users(
     users: Optional[Union[List[str], List[User]]] = None,
     *,
     user_emails: Optional[List[str]] = None,
+    organization: Optional[str] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
 ):
     """List users in the MosaicML platform
 
     Arguments:
         user_ids: List of user ids to get. This can be a list of ID strings or :type User: objects.
         user_emails: List of user emails to get.
+        organization: Organization ID to get users from.
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised. If ``future`` is ``True``, this
             value will be ignored.
         future: Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to `get_users` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of runs, use ``return_value.result()``
@@ -77,15 +81,17 @@
 
     filters = {}
     if users:
         filters['id'] = {'in': [u.id if isinstance(u, User) else u for u in users]}
     if user_emails is not None:
         filters['email'] = {'in': user_emails}
 
-    variables = {VARIABLE_DATA_NAME: {'filters': filters,}}
+    variables = {VARIABLE_DATA_NAME: {'filters': filters}}
+    if organization:
+        variables[VARIABLE_DATA_NAME]["entity"] = {"organizationIds": organization}
 
     response = run_plural_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=User,
         variables=variables,
     )
```

### Comparing `mosaicml-cli-0.6.8/mcli/api/utils.py` & `mosaicml-cli-0.6.9/mcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/cli.py` & `mosaicml-cli-0.6.9/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.6.9/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/common/finetuning_run_filters.py` & `mosaicml-cli-0.6.9/mcli/cli/common/finetuning_run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.6.9/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.6.9/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.6.9/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.6.9/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_debug/debug_run.py` & `mosaicml-cli-0.6.9/mcli/cli/m_debug/debug_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_debug/m_debug.py` & `mosaicml-cli-0.6.9/mcli/cli/m_debug/m_debug.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.6.9/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.6.9/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.6.9/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_clusters.py` & `mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_finetuning_runs.py` & `mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_finetuning_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_describe/describe_users.py` & `mosaicml-cli-0.6.9/mcli/cli/m_describe/describe_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.6.9/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_finetune/m_finetune.py` & `mosaicml-cli-0.6.9/mcli/cli/m_finetune/m_finetune.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/display.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/finetuning_runs.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/finetuning_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/m_get.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ CLI Get options"""
 import argparse
 from typing import List, Optional
 
 from mcli import config
-from mcli.cli.m_get import cli_get_secrets, get_clusters, get_users
+from mcli.cli.m_get import cli_get_secrets, get_clusters, get_organizations, get_users
 from mcli.cli.m_get.display import OutputDisplay
 from mcli.cli.m_get.finetuning_runs import get_finetuning_runs_argparser
 from mcli.cli.m_get.inference_deployments import get_deployments_argparser
 from mcli.cli.m_get.runs import get_runs_argparser
 from mcli.cli.m_log.m_log import add_log_parser
 from mcli.models.mcli_secret import SecretType
 from mcli.utils.utils_model import SubmissionType
@@ -45,17 +45,28 @@
                                 default=config.ADMIN_MODE,
                                 help='Include the cluster ids in the output')
     add_common_arguments(cluster_parser)
     cluster_parser.set_defaults(func=get_clusters)
 
     if is_admin:
         user_parser = subparsers.add_parser('user', aliases=['users'], help='List users')
+        mcli_config = config.MCLIConfig.load_config()
+        kwargs = {'type': str, 'dest': 'org_id', 'help': 'Filter users by organization id'}
+        if mcli_config.organization_id:
+            kwargs['default'] = mcli_config.organization_id
+        user_parser.add_argument('--org', **kwargs)
         add_common_arguments(user_parser)
         user_parser.set_defaults(func=get_users)
 
+        org_parser = subparsers.add_parser('org',
+                                           aliases=['orgs', 'organizations', 'organization'],
+                                           help='List organizations')
+        add_common_arguments(org_parser)
+        org_parser.set_defaults(func=get_organizations)
+
     # pylint: disable-next=invalid-name
     SECRET_EXAMPLES = """
 
 Examples:
 
 > mcli get secrets
 NAME         TYPE
```

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_get/users.py` & `mosaicml-cli-0.6.9/mcli/cli/m_get/users.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     @property
     def index_label(self) -> str:
         return 'organization_id'
 
 
 @cli_error_handler('mcli get users')
-def get_users(output: OutputDisplay = OutputDisplay.TABLE, **kwargs) -> int:
+def get_users(org_id: str, output: OutputDisplay = OutputDisplay.TABLE, **kwargs) -> int:
     del kwargs
 
-    users = api_get_users()
+    users = api_get_users(organization=org_id)
     display = UserDisplay(users)
     display.print(output)
 
     return 0
```

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.6.9/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.6.9/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.6.9/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.6.9/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.6.9/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.6.9/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.6.9/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.6.9/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.6.9/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.6.9/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.6.9/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.6.9/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.6.9/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.6.9/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.6.9/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_set_unset/organization.py` & `mosaicml-cli-0.6.9/mcli/cli/m_set_unset/organization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.6.9/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.6.9/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_update/m_update.py` & `mosaicml-cli-0.6.9/mcli/cli/m_update/m_update.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.6.9/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_util/util.py` & `mosaicml-cli-0.6.9/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/cli/m_watchdog/m_watchdog.py` & `mosaicml-cli-0.6.9/mcli/cli/m_watchdog/m_watchdog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/config.py` & `mosaicml-cli-0.6.9/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/__init__.py` & `mosaicml-cli-0.6.9/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/common.py` & `mosaicml-cli-0.6.9/mcli/models/common.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/finetune_config.py` & `mosaicml-cli-0.6.9/mcli/models/finetune_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/finetune_task_type.py` & `mosaicml-cli-0.6.9/mcli/models/finetune_task_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/gpu_type.py` & `mosaicml-cli-0.6.9/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.6.9/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/mcli_secret.py` & `mosaicml-cli-0.6.9/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/models/run_config.py` & `mosaicml-cli-0.6.9/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/databricks.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/databricks.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/hugging_face.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/hugging_face.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/databricks.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/databricks.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.6.9/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.6.9/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/proto/mint_pb2.pyi` & `mosaicml-cli-0.6.9/mcli/proto/mint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_cli.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_completers.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_completers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_config.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_date.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_finetune.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_finetune.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_logging.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_model.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_rich.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_types.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.6.9/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/mcli/version.py` & `mosaicml-cli-0.6.9/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.6.8'
+__version__ = '0.6.9'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.6.8/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.6.9/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.6.8
+Version: 0.6.9
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,47 +57,47 @@
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "sphinx"
 Requires-Dist: sphinxemoji==0.2.0; extra == "sphinx"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "sphinx"
 Requires-Dist: myst-parser>=0.16.1; extra == "sphinx"
 Requires-Dist: docutils>=0.17.0; extra == "sphinx"
 Requires-Dist: sphinx-design; extra == "sphinx"
 Provides-Extra: all
+Requires-Dist: sphinx-design; extra == "all"
 Requires-Dist: furo==2022.9.29; extra == "all"
-Requires-Dist: radon>=5.1.0; extra == "all"
-Requires-Dist: sphinxcontrib-jsmath>=1.0.1; extra == "all"
+Requires-Dist: yapf>=0.33.0; extra == "all"
+Requires-Dist: sphinxcontrib-applehelp>=1.0.2; extra == "all"
+Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "all"
 Requires-Dist: sphinxcontrib-images>=0.9.4; extra == "all"
+Requires-Dist: sphinxcontrib-katex==0.9.4; extra == "all"
 Requires-Dist: sphinxcontrib-serializinghtml==1.1.5; extra == "all"
-Requires-Dist: yapf>=0.33.0; extra == "all"
-Requires-Dist: sphinx-argparse==0.4.0; extra == "all"
-Requires-Dist: isort>=5.9.3; extra == "all"
+Requires-Dist: sphinxcontrib-qthelp>=1.0.3; extra == "all"
+Requires-Dist: pylint>=2.12.2; extra == "all"
+Requires-Dist: pytest-cov>=4.0.0; extra == "all"
 Requires-Dist: pytest>=6.2.5; extra == "all"
 Requires-Dist: toml>=0.10.2; extra == "all"
-Requires-Dist: pyright==1.1.256; extra == "all"
+Requires-Dist: sphinxemoji==0.2.0; extra == "all"
+Requires-Dist: sphinx-copybutton==0.5.2; extra == "all"
+Requires-Dist: pytest-mock>=3.7.0; extra == "all"
+Requires-Dist: build>=0.10.0; extra == "all"
 Requires-Dist: sphinxcontrib-htmlhelp>=2.0.0; extra == "all"
-Requires-Dist: sphinx_external_toc==0.3.0; extra == "all"
-Requires-Dist: sphinx-rtd-theme==1.0.0; extra == "all"
+Requires-Dist: pyright==1.1.256; extra == "all"
 Requires-Dist: twine>=4.0.2; extra == "all"
-Requires-Dist: sphinxcontrib-devhelp>=1.0.2; extra == "all"
-Requires-Dist: sphinx-copybutton==0.5.2; extra == "all"
-Requires-Dist: sphinxcontrib-katex==0.9.4; extra == "all"
+Requires-Dist: isort>=5.9.3; extra == "all"
+Requires-Dist: sphinx-argparse==0.4.0; extra == "all"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "all"
-Requires-Dist: pytest-mock>=3.7.0; extra == "all"
-Requires-Dist: pylint>=2.12.2; extra == "all"
-Requires-Dist: sphinxcontrib-applehelp>=1.0.2; extra == "all"
+Requires-Dist: radon>=5.1.0; extra == "all"
 Requires-Dist: sphinx-panels==0.6.0; extra == "all"
+Requires-Dist: sphinxcontrib-jsmath>=1.0.1; extra == "all"
+Requires-Dist: sphinx==4.4.0; extra == "all"
 Requires-Dist: docutils>=0.17.0; extra == "all"
 Requires-Dist: pre-commit>=2.17.0; extra == "all"
-Requires-Dist: sphinx==4.4.0; extra == "all"
-Requires-Dist: build>=0.10.0; extra == "all"
-Requires-Dist: sphinx-markdown-tables==0.0.17; extra == "all"
-Requires-Dist: sphinxemoji==0.2.0; extra == "all"
+Requires-Dist: sphinx_external_toc==0.3.0; extra == "all"
+Requires-Dist: sphinxcontrib-devhelp>=1.0.2; extra == "all"
 Requires-Dist: myst-parser>=0.16.1; extra == "all"
-Requires-Dist: sphinxcontrib-qthelp>=1.0.3; extra == "all"
-Requires-Dist: sphinx-design; extra == "all"
-Requires-Dist: pytest-cov>=4.0.0; extra == "all"
+Requires-Dist: sphinx-markdown-tables==0.0.17; extra == "all"
 
 
 #  MosaicML CLI (MCLI)
 
 ### MCLI is the interface for interacting with the MosaicML platform
 
 To get started with MCLI, read the [documentation](https://mcli.docs.mosaicml.com/)
```

### Comparing `mosaicml-cli-0.6.8/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.6.9/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 mcli/cli/m_finetune/m_finetune.py
 mcli/cli/m_get/__init__.py
 mcli/cli/m_get/clusters.py
 mcli/cli/m_get/display.py
 mcli/cli/m_get/finetuning_runs.py
 mcli/cli/m_get/inference_deployments.py
 mcli/cli/m_get/m_get.py
+mcli/cli/m_get/organizations.py
 mcli/cli/m_get/runs.py
 mcli/cli/m_get/secrets.py
 mcli/cli/m_get/users.py
 mcli/cli/m_init/__init__.py
 mcli/cli/m_init/m_init.py
 mcli/cli/m_interactive/__init__.py
 mcli/cli/m_interactive/m_interactive.py
```

### Comparing `mosaicml-cli-0.6.8/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.6.9/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -11,47 +11,47 @@
 typing_extensions>=4.0.1
 validators>=0.20.0
 requests<3,>=2.26.0
 urllib3>=1.23
 numpy
 
 [all]
+sphinx-design
 furo==2022.9.29
-radon>=5.1.0
-sphinxcontrib-jsmath>=1.0.1
+yapf>=0.33.0
+sphinxcontrib-applehelp>=1.0.2
+sphinx-rtd-theme==1.0.0
 sphinxcontrib-images>=0.9.4
+sphinxcontrib-katex==0.9.4
 sphinxcontrib-serializinghtml==1.1.5
-yapf>=0.33.0
-sphinx-argparse==0.4.0
-isort>=5.9.3
+sphinxcontrib-qthelp>=1.0.3
+pylint>=2.12.2
+pytest-cov>=4.0.0
 pytest>=6.2.5
 toml>=0.10.2
-pyright==1.1.256
+sphinxemoji==0.2.0
+sphinx-copybutton==0.5.2
+pytest-mock>=3.7.0
+build>=0.10.0
 sphinxcontrib-htmlhelp>=2.0.0
-sphinx_external_toc==0.3.0
-sphinx-rtd-theme==1.0.0
+pyright==1.1.256
 twine>=4.0.2
-sphinxcontrib-devhelp>=1.0.2
-sphinx-copybutton==0.5.2
-sphinxcontrib-katex==0.9.4
+isort>=5.9.3
+sphinx-argparse==0.4.0
 sphinxext-opengraph==0.8.2
-pytest-mock>=3.7.0
-pylint>=2.12.2
-sphinxcontrib-applehelp>=1.0.2
+radon>=5.1.0
 sphinx-panels==0.6.0
+sphinxcontrib-jsmath>=1.0.1
+sphinx==4.4.0
 docutils>=0.17.0
 pre-commit>=2.17.0
-sphinx==4.4.0
-build>=0.10.0
-sphinx-markdown-tables==0.0.17
-sphinxemoji==0.2.0
+sphinx_external_toc==0.3.0
+sphinxcontrib-devhelp>=1.0.2
 myst-parser>=0.16.1
-sphinxcontrib-qthelp>=1.0.3
-sphinx-design
-pytest-cov>=4.0.0
+sphinx-markdown-tables==0.0.17
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.6.8/pyproject.toml` & `mosaicml-cli-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/setup.py` & `mosaicml-cli-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/tests/test_config.py` & `mosaicml-cli-0.6.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.6.8/tests/test_upgrade.py` & `mosaicml-cli-0.6.9/tests/test_upgrade.py`

 * *Files identical despite different names*

