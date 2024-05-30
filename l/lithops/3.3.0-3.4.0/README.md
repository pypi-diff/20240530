# Comparing `tmp/lithops-3.3.0.tar.gz` & `tmp/lithops-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lithops-3.3.0.tar", last modified: Thu Apr 25 15:46:09 2024, max compression
+gzip compressed data, was "lithops-3.4.0.tar", last modified: Thu May 30 14:21:21 2024, max compression
```

## Comparing `lithops-3.3.0.tar` & `lithops-3.4.0.tar`

### file list

```diff
@@ -1,254 +1,255 @@
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/
--rw-r--r--   0 josep     (1000) josep     (1000)    11357 2024-04-25 15:46:09.000000 lithops-3.3.0/LICENSE
--rw-r--r--   0 josep     (1000) josep     (1000)     1363 2024-04-25 15:46:09.742859 lithops-3.3.0/PKG-INFO
--rw-r--r--   0 josep     (1000) josep     (1000)     9399 2024-04-25 15:46:09.000000 lithops-3.3.0/README.md
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.712859 lithops-3.3.0/lithops/
--rw-r--r--   0 josep     (1000) josep     (1000)      576 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9545 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4153 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/constants.py
--rw-r--r--   0 josep     (1000) josep     (1000)    33987 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/executors.py
--rw-r--r--   0 josep     (1000) josep     (1000)    13862 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/future.py
--rw-r--r--   0 josep     (1000) josep     (1000)    19644 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/invokers.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/job/
--rw-r--r--   0 josep     (1000) josep     (1000)      128 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    13053 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/job.py
--rw-r--r--   0 josep     (1000) josep     (1000)    14699 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/partitioner.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9658 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/job/serialize.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/globber/
--rw-r--r--   0 josep     (1000) josep     (1000)       72 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/globber/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4385 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/globber/globber.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/imp/
--rw-r--r--   0 josep     (1000) josep     (1000)      428 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/imp/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2497 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/imp/imp.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/inspect/
--rw-r--r--   0 josep     (1000) josep     (1000)      120 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/inspect/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5658 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/inspect/inspect.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/multyvac/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/multyvac/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    14397 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/multyvac/module_dependency.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/libs/openwhisk/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/openwhisk/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10745 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/libs/openwhisk/client.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/localhost/
--rw-r--r--   0 josep     (1000) josep     (1000)      152 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/localhost/v1/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v1/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12369 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v1/localhost.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2720 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v1/runner.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/localhost/v2/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v2/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10612 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v2/localhost.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7330 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/localhost/v2/service.py
--rw-r--r--   0 josep     (1000) josep     (1000)    18089 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/monitor.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/multiprocessing/
--rw-r--r--   0 josep     (1000) josep     (1000)     1346 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1717 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    21677 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/connection.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5146 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/context.py
--rw-r--r--   0 josep     (1000) josep     (1000)    22273 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/managers.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9391 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/pool.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7960 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/process.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5579 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/queues.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8911 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/sharedctypes.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9185 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/synchronize.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7884 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/multiprocessing/util.py
--rw-r--r--   0 josep     (1000) josep     (1000)     6323 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/plots.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7865 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/retries.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/scripts/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/scripts/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5904 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/scripts/cleaner.py
--rw-r--r--   0 josep     (1000) josep     (1000)    35956 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/scripts/cli.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/
--rw-r--r--   0 josep     (1000) josep     (1000)       75 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/
--rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12637 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2733 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1606 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aliyun_fc/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/aws_batch/
--rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    27091 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/aws_batch.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5175 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2851 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_batch/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/aws_lambda/
--rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    29346 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/aws_lambda.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1473 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/build_layer.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5499 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1545 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/aws_lambda/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/azure_containers/
--rw-r--r--   0 josep     (1000) josep     (1000)      109 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    14266 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/azure_containers.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5678 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2401 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_containers/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/azure_functions/
--rw-r--r--   0 josep     (1000) josep     (1000)      107 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    15633 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/azure_functions.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4944 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2579 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/azure_functions/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops/serverless/backends/code_engine/
--rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    31342 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/code_engine.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5837 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4436 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/code_engine/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/
--rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    16936 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5926 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2612 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/gcp_functions/
--rw-r--r--   0 josep     (1000) josep     (1000)      101 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3439 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2511 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    20582 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/gcp_functions/gcp_functions.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/ibm_cf/
--rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3378 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1595 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    15478 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/ibm_cf/ibm_cf.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/k8s/
--rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3792 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7321 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    31307 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/k8s/k8s.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/knative/
--rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5986 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2614 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    30354 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/knative/knative.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/openwhisk/
--rw-r--r--   0 josep     (1000) josep     (1000)       94 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2221 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1604 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9655 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/openwhisk/openwhisk.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/serverless/backends/oracle_f/
--rw-r--r--   0 josep     (1000) josep     (1000)      104 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3022 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1646 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/entry_point.py
--rw-r--r--   0 josep     (1000) josep     (1000)    15292 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/backends/oracle_f/oracle_f.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4435 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/serverless/serverless.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/
--rw-r--r--   0 josep     (1000) josep     (1000)      141 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/aws_ec2/
--rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/aws_ec2/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    52738 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/aws_ec2/aws_ec2.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2781 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/aws_ec2/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/azure_vms/
--rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/azure_vms/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    37978 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/azure_vms/azure_vms.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2691 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/azure_vms/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/
--rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4082 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    48122 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/standalone/backends/vm/
--rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/vm/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1059 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/vm/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5020 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/backends/vm/vm.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4815 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/keeper.py
--rw-r--r--   0 josep     (1000) josep     (1000)    23693 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/master.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1961 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/runner.py
--rw-r--r--   0 josep     (1000) josep     (1000)    16922 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/standalone.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8567 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/utils.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10362 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/standalone/worker.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/
--rw-r--r--   0 josep     (1000) josep     (1000)      118 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/__init__.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/aliyun_oss/
--rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aliyun_oss/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9631 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1742 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aliyun_oss/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/aws_s3/
--rw-r--r--   0 josep     (1000) josep     (1000)       78 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aws_s3/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10713 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aws_s3/aws_s3.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1189 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/aws_s3/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/azure_storage/
--rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/azure_storage/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9192 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/azure_storage/azure_storage.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1025 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/azure_storage/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/ceph/
--rw-r--r--   0 josep     (1000) josep     (1000)       85 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ceph/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11552 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ceph/ceph.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1125 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ceph/config.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/gcp_storage/
--rw-r--r--   0 josep     (1000) josep     (1000)       91 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/gcp_storage/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1530 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/gcp_storage/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8656 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/gcp_storage/gcp_storage.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/ibm_cos/
--rw-r--r--   0 josep     (1000) josep     (1000)       98 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ibm_cos/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     3901 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ibm_cos/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    14099 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/ibm_cos/ibm_cos.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.732859 lithops-3.3.0/lithops/storage/backends/infinispan/
--rw-r--r--   0 josep     (1000) josep     (1000)       90 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1051 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10131 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan/infinispan.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/
--rw-r--r--   0 josep     (1000) josep     (1000)      103 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1072 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     8918 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/localhost/
--rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/localhost/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)      789 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/localhost/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9548 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/localhost/localhost.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/minio/
--rw-r--r--   0 josep     (1000) josep     (1000)       87 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/minio/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1131 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/minio/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11569 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/minio/minio.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/oracle_oss/
--rw-r--r--   0 josep     (1000) josep     (1000)       96 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/oracle_oss/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1303 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/oracle_oss/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11630 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/oracle_oss/oracle_oss.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/redis/
--rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/redis/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1007 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/redis/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9625 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/redis/redis.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/storage/backends/swift/
--rw-r--r--   0 josep     (1000) josep     (1000)       64 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/swift/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)      993 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/swift/config.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9922 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/backends/swift/swift.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7531 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/cloud_proxy.py
--rw-r--r--   0 josep     (1000) josep     (1000)    20932 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/storage.py
--rw-r--r--   0 josep     (1000) josep     (1000)     5052 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/storage/utils.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/tests/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1662 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/conftest.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4176 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/functions.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2025 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_call_async.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4508 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_map.py
--rw-r--r--   0 josep     (1000) josep     (1000)     9375 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_map_reduce.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4982 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_retries.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12045 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/tests/test_storage.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/util/
--rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4204 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/ibm_token_manager.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/util/joblib/
--rw-r--r--   0 josep     (1000) josep     (1000)      464 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/joblib/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)     7596 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/joblib/lithops_backend.py
--rw-r--r--   0 josep     (1000) josep     (1000)     1057 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/metrics.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4708 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/util/ssh_client.py
--rw-r--r--   0 josep     (1000) josep     (1000)    22687 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/utils.py
--rw-r--r--   0 josep     (1000) josep     (1000)       74 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/version.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12264 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/wait.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.742859 lithops-3.3.0/lithops/worker/
--rw-r--r--   0 josep     (1000) josep     (1000)      138 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/__init__.py
--rw-r--r--   0 josep     (1000) josep     (1000)    10174 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/handler.py
--rw-r--r--   0 josep     (1000) josep     (1000)     2888 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/invoker.py
--rw-r--r--   0 josep     (1000) josep     (1000)    12849 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/jobrunner.py
--rw-r--r--   0 josep     (1000) josep     (1000)     4510 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/status.py
--rw-r--r--   0 josep     (1000) josep     (1000)    11178 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops/worker/utils.py
-drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-04-25 15:46:09.722859 lithops-3.3.0/lithops.egg-info/
--rw-r--r--   0 josep     (1000) josep     (1000)     1363 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/PKG-INFO
--rw-r--r--   0 josep     (1000) josep     (1000)     7734 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/SOURCES.txt
--rw-r--r--   0 josep     (1000) josep     (1000)        1 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/dependency_links.txt
--rw-r--r--   0 josep     (1000) josep     (1000)       79 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/entry_points.txt
--rw-r--r--   0 josep     (1000) josep     (1000)      796 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/requires.txt
--rw-r--r--   0 josep     (1000) josep     (1000)        8 2024-04-25 15:46:09.000000 lithops-3.3.0/lithops.egg-info/top_level.txt
--rw-r--r--   0 josep     (1000) josep     (1000)       38 2024-04-25 15:46:09.742859 lithops-3.3.0/setup.cfg
--rw-r--r--   0 josep     (1000) josep     (1000)     2694 2024-04-25 15:46:09.000000 lithops-3.3.0/setup.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/
+-rw-r--r--   0 josep     (1000) josep     (1000)    11357 2024-05-30 14:21:21.000000 lithops-3.4.0/LICENSE
+-rw-r--r--   0 josep     (1000) josep     (1000)     1396 2024-05-30 14:21:21.847682 lithops-3.4.0/PKG-INFO
+-rw-r--r--   0 josep     (1000) josep     (1000)     9413 2024-05-30 14:21:21.000000 lithops-3.4.0/README.md
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/
+-rw-r--r--   0 josep     (1000) josep     (1000)      576 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9067 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3999 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/constants.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    34423 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/executors.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14040 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/future.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    19645 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/invokers.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/job/
+-rw-r--r--   0 josep     (1000) josep     (1000)      128 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/job/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    13053 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/job/job.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14699 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/job/partitioner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9737 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/job/serialize.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/libs/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/libs/globber/
+-rw-r--r--   0 josep     (1000) josep     (1000)       72 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/globber/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4385 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/globber/globber.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/libs/imp/
+-rw-r--r--   0 josep     (1000) josep     (1000)      428 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/imp/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2497 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/imp/imp.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/libs/inspect/
+-rw-r--r--   0 josep     (1000) josep     (1000)      120 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/inspect/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5666 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/inspect/inspect.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/libs/multyvac/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/multyvac/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14397 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/multyvac/module_dependency.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/libs/openwhisk/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/openwhisk/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10745 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/libs/openwhisk/client.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/localhost/
+-rw-r--r--   0 josep     (1000) josep     (1000)      231 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1785 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/localhost/v1/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/v1/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12699 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/v1/localhost.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2720 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/v1/runner.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops/localhost/v2/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/v2/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    15022 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/v2/localhost.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2619 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/localhost/v2/runner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    18195 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/monitor.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/multiprocessing/
+-rw-r--r--   0 josep     (1000) josep     (1000)     1346 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1717 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    21677 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/connection.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5146 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/context.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    22273 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/managers.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9391 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/pool.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7960 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/process.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5579 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/queues.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8911 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/sharedctypes.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9185 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/synchronize.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7884 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/multiprocessing/util.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     6323 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/plots.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7865 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/retries.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/scripts/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/scripts/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5904 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/scripts/cleaner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    36034 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/scripts/cli.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/
+-rw-r--r--   0 josep     (1000) josep     (1000)       75 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/aliyun_fc/
+-rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aliyun_fc/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12637 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2733 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aliyun_fc/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1606 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aliyun_fc/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/aws_batch/
+-rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_batch/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    26812 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_batch/aws_batch.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5407 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_batch/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2851 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_batch/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/aws_lambda/
+-rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_lambda/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    29346 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_lambda/aws_lambda.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1473 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_lambda/build_layer.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5499 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_lambda/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1545 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/aws_lambda/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/azure_containers/
+-rw-r--r--   0 josep     (1000) josep     (1000)      109 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_containers/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14266 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_containers/azure_containers.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5678 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_containers/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2401 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_containers/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/azure_functions/
+-rw-r--r--   0 josep     (1000) josep     (1000)      107 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_functions/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    15633 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_functions/azure_functions.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4944 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_functions/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2579 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/azure_functions/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/code_engine/
+-rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/code_engine/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    31342 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/code_engine/code_engine.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5837 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/code_engine/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4436 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/code_engine/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/
+-rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    16936 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5926 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2612 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/gcp_functions/
+-rw-r--r--   0 josep     (1000) josep     (1000)      101 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_functions/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3439 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_functions/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2511 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_functions/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    20582 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/gcp_functions/gcp_functions.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.827682 lithops-3.4.0/lithops/serverless/backends/ibm_cf/
+-rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/ibm_cf/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3378 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/ibm_cf/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1595 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/ibm_cf/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    15478 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/ibm_cf/ibm_cf.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/serverless/backends/k8s/
+-rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/k8s/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3792 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/k8s/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7321 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/k8s/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    31307 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/k8s/k8s.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/serverless/backends/knative/
+-rw-r--r--   0 josep     (1000) josep     (1000)       97 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/knative/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5986 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/knative/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2614 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/knative/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    30354 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/knative/knative.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/serverless/backends/openwhisk/
+-rw-r--r--   0 josep     (1000) josep     (1000)       94 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/openwhisk/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2221 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/openwhisk/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1604 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/openwhisk/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9655 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/openwhisk/openwhisk.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/serverless/backends/oracle_f/
+-rw-r--r--   0 josep     (1000) josep     (1000)      104 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/oracle_f/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3022 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/oracle_f/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1646 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/oracle_f/entry_point.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    15292 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/backends/oracle_f/oracle_f.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4435 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/serverless/serverless.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/standalone/
+-rw-r--r--   0 josep     (1000) josep     (1000)      141 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/standalone/backends/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/standalone/backends/aws_ec2/
+-rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/aws_ec2/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    52753 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/aws_ec2/aws_ec2.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2986 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/aws_ec2/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/standalone/backends/azure_vms/
+-rw-r--r--   0 josep     (1000) josep     (1000)       93 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/azure_vms/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    37978 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/azure_vms/azure_vms.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2691 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/azure_vms/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/standalone/backends/ibm_vpc/
+-rw-r--r--   0 josep     (1000) josep     (1000)       89 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/ibm_vpc/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4082 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/ibm_vpc/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    48122 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/standalone/backends/vm/
+-rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/vm/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1059 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/vm/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5020 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/backends/vm/vm.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4815 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/keeper.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    23693 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/master.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1961 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/runner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    16922 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/standalone.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8567 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/utils.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10362 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/standalone/worker.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/storage/
+-rw-r--r--   0 josep     (1000) josep     (1000)      118 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/storage/backends/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/__init__.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/storage/backends/aliyun_oss/
+-rw-r--r--   0 josep     (1000) josep     (1000)      106 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/aliyun_oss/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9631 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1742 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/aliyun_oss/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/storage/backends/aws_s3/
+-rw-r--r--   0 josep     (1000) josep     (1000)       78 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/aws_s3/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10713 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/aws_s3/aws_s3.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1189 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/aws_s3/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/storage/backends/azure_storage/
+-rw-r--r--   0 josep     (1000) josep     (1000)       99 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/azure_storage/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9192 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/azure_storage/azure_storage.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1025 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/azure_storage/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/storage/backends/ceph/
+-rw-r--r--   0 josep     (1000) josep     (1000)       85 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/ceph/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11650 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/ceph/ceph.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1125 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/ceph/config.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.837682 lithops-3.4.0/lithops/storage/backends/gcp_storage/
+-rw-r--r--   0 josep     (1000) josep     (1000)       91 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/gcp_storage/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1530 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/gcp_storage/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8656 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/gcp_storage/gcp_storage.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/ibm_cos/
+-rw-r--r--   0 josep     (1000) josep     (1000)       98 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/ibm_cos/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     3901 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/ibm_cos/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    14099 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/ibm_cos/ibm_cos.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/infinispan/
+-rw-r--r--   0 josep     (1000) josep     (1000)       90 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/infinispan/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1051 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/infinispan/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10131 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/infinispan/infinispan.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/infinispan_hotrod/
+-rw-r--r--   0 josep     (1000) josep     (1000)      103 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/infinispan_hotrod/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1072 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/infinispan_hotrod/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     8918 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/localhost/
+-rw-r--r--   0 josep     (1000) josep     (1000)       95 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/localhost/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)      910 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/localhost/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9548 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/localhost/localhost.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/minio/
+-rw-r--r--   0 josep     (1000) josep     (1000)       87 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/minio/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1131 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/minio/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11569 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/minio/minio.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/oracle_oss/
+-rw-r--r--   0 josep     (1000) josep     (1000)       96 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/oracle_oss/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1303 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/oracle_oss/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11630 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/oracle_oss/oracle_oss.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/redis/
+-rw-r--r--   0 josep     (1000) josep     (1000)       80 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/redis/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1007 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/redis/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     9625 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/redis/redis.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/storage/backends/swift/
+-rw-r--r--   0 josep     (1000) josep     (1000)       64 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/swift/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)      993 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/swift/config.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10476 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/backends/swift/swift.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7531 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/cloud_proxy.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    20928 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/storage.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     5052 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/storage/utils.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/tests/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1507 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/conftest.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4671 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/functions.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2025 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/test_call_async.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4508 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/test_map.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10067 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/test_map_reduce.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4982 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/test_retries.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12045 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/tests/test_storage.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/util/
+-rw-r--r--   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/util/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4204 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/util/ibm_token_manager.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/util/joblib/
+-rw-r--r--   0 josep     (1000) josep     (1000)      464 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/util/joblib/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     7596 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/util/joblib/lithops_backend.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     1057 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/util/metrics.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4708 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/util/ssh_client.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    23146 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/utils.py
+-rw-r--r--   0 josep     (1000) josep     (1000)       74 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/version.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12348 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/wait.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.847682 lithops-3.4.0/lithops/worker/
+-rw-r--r--   0 josep     (1000) josep     (1000)      138 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/worker/__init__.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    10174 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/worker/handler.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     2888 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/worker/invoker.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    12872 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/worker/jobrunner.py
+-rw-r--r--   0 josep     (1000) josep     (1000)     4533 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/worker/status.py
+-rw-r--r--   0 josep     (1000) josep     (1000)    11333 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops/worker/utils.py
+drwxr-xr-x   0 josep     (1000) josep     (1000)        0 2024-05-30 14:21:21.817682 lithops-3.4.0/lithops.egg-info/
+-rw-r--r--   0 josep     (1000) josep     (1000)     1396 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops.egg-info/PKG-INFO
+-rw-r--r--   0 josep     (1000) josep     (1000)     7761 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops.egg-info/SOURCES.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)        1 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops.egg-info/dependency_links.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)       79 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops.egg-info/entry_points.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)      984 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops.egg-info/requires.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)        8 2024-05-30 14:21:21.000000 lithops-3.4.0/lithops.egg-info/top_level.txt
+-rw-r--r--   0 josep     (1000) josep     (1000)       38 2024-05-30 14:21:21.847682 lithops-3.4.0/setup.cfg
+-rw-r--r--   0 josep     (1000) josep     (1000)     2835 2024-05-30 14:21:21.000000 lithops-3.4.0/setup.py
```

### Comparing `lithops-3.3.0/LICENSE` & `lithops-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/PKG-INFO` & `lithops-3.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: lithops
-Version: 3.3.0
+Version: 3.4.0
 Summary: Lithops lets you transparently run your Python applications in the Cloud
 Home-page: https://github.com/lithops-cloud/lithops
 Author: Gil Vernik, Josep Sampe
 Author-email: gilv@ibm.com, josep.sampe@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.6
 Provides-Extra: aliyun
 Provides-Extra: all
+Provides-Extra: aws
 Provides-Extra: azure
+Provides-Extra: ceph
 Provides-Extra: gcp
+Provides-Extra: ibm
 Provides-Extra: joblib
+Provides-Extra: knative
+Provides-Extra: kubernetes
+Provides-Extra: minio
 Provides-Extra: multiprocessing
 Provides-Extra: oracle
+Provides-Extra: plotting
+Provides-Extra: redis
 Provides-Extra: tests
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `lithops-3.3.0/README.md` & `lithops-3.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -191,8 +191,8 @@
 * [Towards Multicloud Access Transparency in Serverless Computing](https://www.computer.org/csdl/magazine/so/5555/01/09218932/1nMMkpZ8Ko8) - IEEE Software 2021
 * [Primula: a Practical Shuffle/Sort Operator for Serverless Computing](https://dl.acm.org/doi/10.1145/3429357.3430522) - ACM/IFIP International Middleware Conference 2020. [See presentation here](https://www.youtube.com/watch?v=v698iu5YfWM)
 * [Bringing scaling transparency to Proteomics applications with serverless computing](https://dl.acm.org/doi/abs/10.1145/3429880.3430101) - 6th International Workshop on Serverless Computing (WoSC6) 2020. [See presentation here](https://www.serverlesscomputing.org/wosc6/#p10)
 * [Serverless data analytics in the IBM Cloud](https://dl.acm.org/citation.cfm?id=3284029) - ACM/IFIP International Middleware Conference 2018
 
 
 # Acknowledgements
-This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No 825184.
+This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No 825184 (CloudButton).
```

### Comparing `lithops-3.3.0/lithops/__init__.py` & `lithops-3.4.0/lithops/__init__.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/config.py` & `lithops-3.4.0/lithops/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -168,55 +168,41 @@
         config_data[backend] = {}
 
     if 'backend' in config_overwrite and config_overwrite['backend']:
         config_data[backend].update(config_overwrite['backend'])
 
     if mode == c.LOCALHOST:
         logger.debug("Loading compute backend module: localhost")
-
-        config_data[backend]['max_workers'] = 1
-
-        if 'execution_timeout' not in config_data['lithops']:
-            config_data['lithops']['execution_timeout'] = c.EXECUTION_TIMEOUT_LOCALHOST_DEFAULT
-
-        if 'storage' not in config_data['lithops']:
-            config_data['lithops']['storage'] = c.LOCALHOST
-
-        if 'worker_processes' not in config_data[c.LOCALHOST]:
-            config_data[backend]['worker_processes'] = c.CPU_COUNT
-
-        if 'runtime' not in config_data[c.LOCALHOST]:
-            config_data[backend]['runtime'] = c.LOCALHOST_RUNTIME_DEFAULT
+        cb_config = importlib.import_module('lithops.localhost.config')
+        cb_config.load_config(config_data)
 
     elif mode == c.SERVERLESS:
         logger.debug(f"Loading Serverless backend module: {backend}")
         cb_config = importlib.import_module(f'lithops.serverless.backends.{backend}.config')
         cb_config.load_config(config_data)
 
     elif mode == c.STANDALONE:
         logger.debug(f"Loading Standalone backend module: {backend}")
         sb_config = importlib.import_module(f'lithops.standalone.backends.{backend}.config')
         sb_config.load_config(config_data)
         config_data['lithops']['chunksize'] = 0
 
-    if 'monitoring' not in config_data['lithops']:
-        config_data['lithops']['monitoring'] = c.MONITORING_DEFAULT
-
-    if 'execution_timeout' not in config_data['lithops']:
-        config_data['lithops']['execution_timeout'] = c.EXECUTION_TIMEOUT_DEFAULT
-
     if 'chunksize' not in config_data['lithops']:
         config_data['lithops']['chunksize'] = config_data[backend]['worker_processes']
 
     if load_storage_config:
         config_data = default_storage_config(config_data=config_data)
         if config_data['lithops']['storage'] == c.LOCALHOST \
            and backend != c.LOCALHOST:
             raise Exception(f'Localhost storage backend cannot be used with {backend}')
 
+    for key in c.LITHOPS_DEFAULT_CONFIG_KEYS:
+        if key not in config_data['lithops']:
+            config_data['lithops'][key] = c.LITHOPS_DEFAULT_CONFIG_KEYS[key]
+
     return config_data
 
 
 def default_storage_config(config_file=None, config_data=None, backend=None):
     """ Function to load default storage config """
 
     config_data = copy.deepcopy(config_data) or load_config(config_file)
@@ -236,14 +222,15 @@
     sb_config.load_config(config_data)
 
     return config_data
 
 
 def extract_storage_config(config):
     s_config = {}
+    s_config['monitoring_interval'] = config['lithops']['monitoring_interval']
     backend = config['lithops']['storage']
     s_config['backend'] = backend
     s_config[backend] = config[backend] if backend in config and config[backend] else {}
     s_config[backend]['user_agent'] = f'lithops/{__version__}'
 
     return s_config
```

### Comparing `lithops-3.3.0/lithops/constants.py` & `lithops-3.4.0/lithops/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
-import sys
 import tempfile
 
 LOGGER_LEVEL = 'info'
 LOGGER_STREAM = 'ext://sys.stderr'
 LOGGER_FORMAT = "%(asctime)s [%(levelname)s] %(filename)s:%(lineno)s -- %(message)s"
 LOGGER_FORMAT_SHORT = "[%(levelname)s] %(filename)s:%(lineno)s -- %(message)s"
 LOGGER_LEVEL_CHOICES = ["debug", "info", "warning", "error", "critical"]
@@ -31,33 +30,23 @@
 
 LOCALHOST = 'localhost'
 SERVERLESS = 'serverless'
 STANDALONE = 'standalone'
 
 MODE_DEFAULT = SERVERLESS
 
-MONITORING_DEFAULT = 'storage'
-MONITORING_INTERVAL = 2
-
 SERVERLESS_BACKEND_DEFAULT = 'aws_lambda'
 STANDALONE_BACKEND_DEFAULT = 'aws_ec2'
 STORAGE_BACKEND_DEFAULT = 'aws_s3'
 
 JOBS_PREFIX = "lithops.jobs"
 TEMP_PREFIX = "lithops.jobs/tmp"
 LOGS_PREFIX = "lithops.logs"
 RUNTIMES_PREFIX = "lithops.runtimes"
 
-EXECUTION_TIMEOUT_DEFAULT = 1800
-EXECUTION_TIMEOUT_LOCALHOST_DEFAULT = 3600
-
-LOCALHOST_RUNTIME_DEFAULT = os.path.basename(sys.executable)
-LOCALHOST_SERVICE_IDLE_TIMEOUT = 3
-LOCALHOST_SERVICE_CHECK_INTERVAL = 2
-
 MAX_AGG_DATA_SIZE = 4  # 4MiB
 
 WORKER_PROCESSES_DEFAULT = 1
 
 TEMP_DIR = os.path.realpath(tempfile.gettempdir())
 USER_TEMP_DIR = 'lithops-' + os.getenv("USER", "root")
 LITHOPS_TEMP_DIR = os.path.join(TEMP_DIR, USER_TEMP_DIR)
@@ -76,14 +65,20 @@
 
 HOME_DIR = os.path.expanduser('~')
 CONFIG_DIR = os.path.join(HOME_DIR, '.lithops')
 CACHE_DIR = os.path.join(CONFIG_DIR, 'cache')
 CONFIG_FILE = os.path.join(CONFIG_DIR, 'config')
 CONFIG_FILE_GLOBAL = os.path.join("/etc", "lithops", "config")
 
+LITHOPS_DEFAULT_CONFIG_KEYS = {
+    'monitoring': 'storage',
+    'monitoring_interval': 2,
+    'execution_timeout': 1800
+}
+
 SA_INSTALL_DIR = '/opt/lithops'
 SA_SETUP_LOG_FILE = f'{SA_INSTALL_DIR}/setup.log'
 SA_SETUP_DONE_FILE = f'{SA_INSTALL_DIR}/setup-done.flag'
 SA_MASTER_LOG_FILE = f'{LITHOPS_TEMP_DIR}/master-service.log'
 SA_WORKER_LOG_FILE = f'{LITHOPS_TEMP_DIR}/worker-service.log'
 SA_MASTER_SERVICE_PORT = 8080
 SA_WORKER_SERVICE_PORT = 8081
```

### Comparing `lithops-3.3.0/lithops/executors.py` & `lithops-3.4.0/lithops/executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,24 +26,24 @@
 from collections.abc import Callable
 from datetime import datetime
 
 from lithops import constants
 from lithops.future import ResponseFuture
 from lithops.invokers import create_invoker
 from lithops.storage import InternalStorage
-from lithops.wait import wait, ALL_COMPLETED, THREADPOOL_SIZE, WAIT_DUR_SEC, ALWAYS
+from lithops.wait import wait, ALL_COMPLETED, THREADPOOL_SIZE, ALWAYS
 from lithops.job import create_map_job, create_reduce_job
 from lithops.config import default_config, \
     extract_localhost_config, extract_standalone_config, \
     extract_serverless_config, get_log_info, extract_storage_config
 from lithops.constants import LOCALHOST, CLEANER_DIR, \
     SERVERLESS, STANDALONE
 from lithops.utils import setup_lithops_logger, \
     is_lithops_worker, create_executor_id, create_futures_list
-from lithops.localhost import LocalhostHandler, LocalhostHandlerV2
+from lithops.localhost import LocalhostHandlerV1, LocalhostHandlerV2
 from lithops.standalone import StandaloneHandler
 from lithops.serverless import ServerlessHandler
 from lithops.storage.utils import create_job_key, CloudObject
 from lithops.monitor import JobMonitor
 from lithops.utils import FuturesList
 
 
@@ -114,16 +114,16 @@
         self.storage = self.internal_storage.storage
 
         self.backend = self.config['lithops']['backend']
         self.mode = self.config['lithops']['mode']
 
         if self.mode == LOCALHOST:
             localhost_config = extract_localhost_config(self.config)
-            if localhost_config.get('version', 1) == 1:
-                self.compute_handler = LocalhostHandler(localhost_config)
+            if localhost_config.get('version', 2) == 1:
+                self.compute_handler = LocalhostHandlerV1(localhost_config)
             else:
                 self.compute_handler = LocalhostHandlerV2(localhost_config)
         elif self.mode == SERVERLESS:
             serverless_config = extract_serverless_config(self.config)
             self.compute_handler = ServerlessHandler(serverless_config, self.internal_storage)
         elif self.mode == STANDALONE:
             standalone_config = extract_standalone_config(self.config)
@@ -395,15 +395,15 @@
         self,
         fs: Optional[Union[ResponseFuture, FuturesList, List[ResponseFuture]]] = None,
         throw_except: Optional[bool] = True,
         return_when: Optional[Any] = ALL_COMPLETED,
         download_results: Optional[bool] = False,
         timeout: Optional[int] = None,
         threadpool_size: Optional[int] = THREADPOOL_SIZE,
-        wait_dur_sec: Optional[int] = WAIT_DUR_SEC,
+        wait_dur_sec: Optional[int] = None,
         show_progressbar: Optional[bool] = True
     ) -> Tuple[FuturesList, FuturesList]:
         """
         Wait for the Future instances (possibly created by different Executor instances)
         given by fs to complete. Returns a named 2-tuple of sets. The first set, named done,
         contains the futures that completed (finished or cancelled futures) before the wait
         completed. The second set, named not_done, contains the futures that did not complete
@@ -412,15 +412,15 @@
 
         :param fs: Futures list. Default None
         :param throw_except: Re-raise exception if call raised. Default True
         :param return_when: Percentage of done futures
         :param download_results: Download results. Default false (Only get statuses)
         :param timeout: Timeout of waiting for results
         :param threadpool_size: Number of threads to use. Default 64
-        :param wait_dur_sec: Time interval between each check
+        :param wait_dur_sec: Time interval between each check. Default 1 second
         :param show_progressbar: whether or not to show the progress bar.
 
         :return: `(fs_done, fs_notdone)` where `fs_done` is a list of futures that have
             completed and `fs_notdone` is a list of futures that have not completed.
         """
         futures = fs or self.futures
 
@@ -466,25 +466,25 @@
 
     def get_result(
         self,
         fs: Optional[Union[ResponseFuture, FuturesList, List[ResponseFuture]]] = None,
         throw_except: Optional[bool] = True,
         timeout: Optional[int] = None,
         threadpool_size: Optional[int] = THREADPOOL_SIZE,
-        wait_dur_sec: Optional[int] = WAIT_DUR_SEC,
+        wait_dur_sec: Optional[int] = None,
         show_progressbar: Optional[bool] = True
     ):
         """
         For getting the results from all function activations
 
         :param fs: Futures list. Default None
         :param throw_except: Reraise exception if call raised. Default True.
         :param timeout: Timeout for waiting for results.
         :param threadpool_size: Number of threads to use. Default 128
-        :param wait_dur_sec: Time interval between each check.
+        :param wait_dur_sec: Time interval between each check. Default 1 second
         :param show_progressbar: whether or not to show the progress bar.
 
         :return: The result of the future/s
         """
         pending_to_read = len(fs) if fs else len(
             [f for f in self.futures if not f._read and not f.futures])
 
@@ -539,16 +539,21 @@
 
         ftrs_to_plot = [f for f in ftrs if (f.success or f.done) and not f.error]
 
         if not ftrs_to_plot:
             logger.debug(f'ExecutorID {self.executor_id} - No futures ready to plot')
             return
 
-        logging.getLogger('matplotlib').setLevel(logging.WARNING)
-        from lithops.plots import create_timeline, create_histogram
+        try:
+            logging.getLogger('matplotlib').setLevel(logging.WARNING)
+            from lithops.plots import create_timeline, create_histogram
+        except ImportError:
+            raise ModuleNotFoundError(
+                "Please install 'pip3 install lithops[plotting]' for "
+                "making use of the plot() method")
 
         logger.info(f'ExecutorID {self.executor_id} - Creating execution plots')
 
         create_timeline(ftrs_to_plot, dst, figsize)
         create_histogram(ftrs_to_plot, dst, figsize)
 
     def clean(
@@ -624,16 +629,21 @@
     def job_summary(self, cloud_objects_n: Optional[int] = 0):
         """
         Logs information of a job executed by the calling function executor.
         currently supports: code_engine, ibm_vpc and ibm_cf.
 
         :param cloud_objects_n: number of cloud object used in COS, declared by user.
         """
-        import pandas as pd
-        import numpy as np
+        try:
+            import pandas as pd
+            import numpy as np
+        except ImportError:
+            raise ModuleNotFoundError(
+                "Please install 'pip3 install lithops[plotting]' for "
+                "making use of the job_summary() method")
 
         def init():
             headers = ['Job_ID', 'Function', 'Invocations', 'Memory(MB)', 'AvgRuntime', 'Cost', 'CloudObjects']
             pd.DataFrame([], columns=headers).to_csv(self.log_path, index=False)
 
         def append(content):
             """ appends job information to log file."""
```

### Comparing `lithops-3.3.0/lithops/future.py` & `lithops-3.4.0/lithops/future.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,17 +48,14 @@
         Running = "Running"
         Ready = "Ready"
         Success = "Success"
         Error = "Error"
         Done = "Done"
         Unknown = "Unknown"
 
-    GET_RESULT_SLEEP_SECS = 1
-    GET_RESULT_MAX_RETRIES = 10
-
     def __init__(self, call_id, job, job_metadata, storage_config):
         self.call_id = call_id
         self.job_id = job.job_id
         self.job_key = job.job_key
         self.executor_id = job.executor_id
         self.function_name = job.function_name
         self.execution_timeout = job.execution_timeout
@@ -165,23 +162,25 @@
     def _set_mapreduce(self):
         """ Set the future as mapreduce map"""
         self._read = True
         self._produce_output = False
         if self.success:
             self._state = ResponseFuture.State.Done
 
-    def status(self, throw_except=True, internal_storage=None, check_only=False):
+    def status(self, throw_except=True, internal_storage=None, check_only=False, wait_dur_sec=1):
         """
         Return the status returned by the call.
         If the call raised an exception, this method will raise the same exception
         If the future is cancelled before completing then CancelledError will be raised.
 
         :param check_only: Return None immediately if job is not complete. Default False.
         :param throw_except: Reraise exception if call raised. Default true.
         :param internal_storage: Storage handler to poll cloud storage. Default None.
+        :param wait_dur_sec: Time interval between each check
+
         :return: Result of the call.
         :raises CancelledError: If the job is cancelled before completed.
         :raises TimeoutError: If job is not complete after `timeout` seconds.
         """
         if self._state == ResponseFuture.State.New:
             raise ValueError("task not yet invoked")
 
@@ -195,15 +194,15 @@
             self._call_status = internal_storage.get_call_status(self.executor_id, self.job_id, self.call_id)
             self._status_query_count += 1
 
             if check_only:
                 return self._call_status
 
             while self._call_status is None:
-                time.sleep(self.GET_RESULT_SLEEP_SECS)
+                time.sleep(wait_dur_sec)
                 self._call_status = internal_storage.get_call_status(self.executor_id, self.job_id, self.call_id)
                 self._status_query_count += 1
             self._host_status_done_tstamp = time.time()
 
         self.stats['host_status_done_tstamp'] = self._host_status_done_tstamp or time.time()
         self.stats['host_status_query_count'] = self._status_query_count
         self.activation_id = self._call_status['activation_id']
@@ -292,47 +291,50 @@
         if self._call_output or not self._produce_output:
             self._set_state(ResponseFuture.State.Done)
         else:
             self._set_state(ResponseFuture.State.Success)
 
         return self._call_status
 
-    def result(self, throw_except=True, internal_storage=None):
+    def result(self, throw_except=True, internal_storage=None, retries=10, wait_dur_sec=1):
         """
         Return the value returned by the call.
         If the call raised an exception, this method will raise the same exception
         If the future is cancelled before completing then CancelledError will be raised.
 
         :param throw_except: Reraise exception if call raised. Default true.
         :param internal_storage: Storage handler to poll cloud storage. Default None.
+        :param retries: Number of times to check if the result file is in the storage
+        :param wait_dur_sec: Time interval between each retry check
+
         :return: Result of the call.
         :raises CancelledError: If the job is cancelled before completed.
         :raises TimeoutError: If job is not complete after `timeout` seconds.
         """
         if self._state == ResponseFuture.State.New:
             raise ValueError("Task not yet invoked")
 
         if not self.done and internal_storage is None:
             internal_storage = InternalStorage(storage_config=self._storage_config)
 
-        self.status(throw_except=throw_except, internal_storage=internal_storage)
+        self.status(throw_except=throw_except, internal_storage=internal_storage, wait_dur_sec=wait_dur_sec)
 
         if self.futures:
             self._call_output = self._new_futures
             self._set_state(ResponseFuture.State.Done)
 
         if self.done:
             return self._call_output
 
         if self._call_output is None:
             call_output = internal_storage.get_call_output(self.executor_id, self.job_id, self.call_id)
             self._output_query_count += 1
 
-            while call_output is None and self._output_query_count < self.GET_RESULT_MAX_RETRIES:
-                time.sleep(self.GET_RESULT_SLEEP_SECS)
+            while call_output is None and self._output_query_count < retries:
+                time.sleep(wait_dur_sec)
                 call_output = internal_storage.get_call_output(self.executor_id, self.job_id, self.call_id)
                 self._output_query_count += 1
 
             if call_output is None:
                 if throw_except:
                     raise Exception(
                         f'ExecutorID {self.executor_id} | JobID {self.job_id} - Unable to get '
```

### Comparing `lithops-3.3.0/lithops/invokers.py` & `lithops-3.4.0/lithops/invokers.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                              "is not compatible with the local Python version {}")
                             .format(self.runtime_name, py_remote_version, py_local_version))
 
         return runtime_meta
 
     def _create_payload(self, job):
         """
-        Creates the default pyload dictionary
+        Creates the default payload dictionary
         """
         payload = {
             'config': self.config,
             'chunksize': job.chunksize,
             'log_level': self.log_level,
             'func_name': job.function_name,
             'func_key': job.func_key,
```

### Comparing `lithops-3.3.0/lithops/job/job.py` & `lithops-3.4.0/lithops/job/job.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/job/partitioner.py` & `lithops-3.4.0/lithops/job/partitioner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/job/serialize.py` & `lithops-3.4.0/lithops/job/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         mod_paths = set()
 
         for obj in list_of_objs:
             strs.append(cloudpickle.dumps(obj))
 
         if include_modules is None:
             # If include_modules is explicitly set to None, no module is included
+            logger.debug('Module manager disabled. Modules to transmit: None')
             return (strs, mod_paths)
 
         if len(include_modules) == 0:
             # If include_modules is not provided (empty list by default),
             # inspect the objects looking for referenced modules
             self._modulemgr = ModuleDependencyAnalyzer()
             self._modulemgr.ignore(preinstalled_modules)
```

### Comparing `lithops-3.3.0/lithops/libs/globber/globber.py` & `lithops-3.4.0/lithops/libs/globber/globber.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/libs/imp/imp.py` & `lithops-3.4.0/lithops/libs/imp/imp.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/libs/inspect/inspect.py` & `lithops-3.4.0/lithops/libs/inspect/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 @functools.lru_cache()
 def _shadowed_dict_from_mro_tuple(mro):
     for entry in mro:
         dunder_dict = _get_dunder_dict_of_class(entry)
         if '__dict__' in dunder_dict:
             class_dict = dunder_dict['__dict__']
-            if not (type(class_dict) is types.GetSetDescriptorType
+            if not (isinstance(class_dict, types.GetSetDescriptorType)
                     and class_dict.__name__ == "__dict__"
                     and class_dict.__objclass__ is entry):
                 return class_dict
     return _sentinel
 
 
 def _shadowed_dict(klass):
@@ -124,15 +124,15 @@
     """
     instance_result = _sentinel
 
     objtype = type(obj)
     if type not in _static_getmro(objtype):
         klass = objtype
         dict_attr = _shadowed_dict(klass)
-        if (dict_attr is _sentinel or type(dict_attr) is types.MemberDescriptorType):
+        if (dict_attr is _sentinel or isinstance(dict_attr, types.MemberDescriptorType)):
             instance_result = _check_instance(obj, attr)
     else:
         klass = obj
 
     klass_result = _check_class(klass, attr)
 
     if instance_result is not _sentinel and klass_result is not _sentinel:
```

### Comparing `lithops-3.3.0/lithops/libs/multyvac/module_dependency.py` & `lithops-3.4.0/lithops/libs/multyvac/module_dependency.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/libs/openwhisk/client.py` & `lithops-3.4.0/lithops/libs/openwhisk/client.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/localhost/v1/localhost.py` & `lithops-3.4.0/lithops/localhost/v1/localhost.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,95 +25,107 @@
 import threading
 import subprocess as sp
 from shutil import copyfile
 from pathlib import Path
 
 from lithops.version import __version__
 from lithops.constants import (
-    LOCALHOST_RUNTIME_DEFAULT,
-    RN_LOG_FILE,
     TEMP_DIR,
     USER_TEMP_DIR,
     LITHOPS_TEMP_DIR,
     COMPUTE_CLI_MSG,
     JOBS_PREFIX
 )
 from lithops.utils import (
     BackendType,
     get_docker_path,
     is_lithops_worker,
+    is_podman,
     is_unix_system
 )
+from lithops.localhost.config import (
+    LocvalhostEnvironment,
+    get_environment
+)
 
 logger = logging.getLogger(__name__)
 
-RUNNER = os.path.join(LITHOPS_TEMP_DIR, 'localhost-runner.py')
+RUNNER_FILE = os.path.join(LITHOPS_TEMP_DIR, 'localhost-runner.py')
 LITHOPS_LOCATION = os.path.dirname(os.path.abspath(lithops.__file__))
 
 
-class LocalhostHandler:
+class LocalhostHandlerV1:
     """
     A localhostHandler object is used by invokers and other components to access
     underlying localhost backend without exposing the implementation details.
     """
 
     def __init__(self, config):
         logger.debug('Creating Localhost compute client')
         self.config = config
-        self.runtime_name = self.config.get('runtime', LOCALHOST_RUNTIME_DEFAULT)
-        self.env = None
+        self.runtime_name = self.config['runtime']
+        self.environment = get_environment(self.runtime_name)
 
+        self.env = None
         self.job_queue = queue.Queue()
         self.job_manager = None
-        self.should_run = True
+        self.invocation_in_progress = False
 
         msg = COMPUTE_CLI_MSG.format('Localhost compute v1')
         logger.info(f"{msg}")
 
     def get_backend_type(self):
         """
         Wrapper method that returns the type of the backend (Batch or FaaS)
         """
         return BackendType.BATCH.value
 
     def init(self):
         """
         Init tasks for localhost
         """
-        default_env = self.runtime_name.startswith(('python', '/'))
-        self.env = DefaultEnv(self.config) if default_env else DockerEnv(self.config)
+        if self.environment == LocvalhostEnvironment.DEFAULT:
+            self.env = DefaultEnvironment(self.config)
+        else:
+            self.env = ContainerEnvironment(self.config)
+
         self.env.setup()
 
     def start_manager(self):
         """
         Starts manager thread to keep order in tasks
         """
 
         def job_manager():
             logger.debug('Staring localhost job manager')
-            self.should_run = True
 
-            while self.should_run:
+            while True:
                 job_payload, job_filename = self.job_queue.get()
+
                 if job_payload is None and job_filename is None:
-                    if self.job_queue.empty():
-                        break
-                    else:
+                    if self.invocation_in_progress or not self.job_queue.empty():
                         continue
+                    else:
+                        break
+
                 executor_id = job_payload['executor_id']
                 job_id = job_payload['job_id']
                 total_calls = len(job_payload['call_ids'])
                 job_key = job_payload['job_key']
                 logger.debug(f'ExecutorID {executor_id} | JobID {job_id} - Running '
                              f'{total_calls} activations in the localhost worker')
-                process = self.env.run(job_key, job_filename)
+                process = self.env.run_job(job_key, job_filename)
                 process.communicate()  # blocks until the process finishes
                 logger.debug(f'ExecutorID {executor_id} | JobID {job_id} - Execution finished')
+
                 if self.job_queue.empty():
-                    break
+                    if self.invocation_in_progress:
+                        continue
+                    else:
+                        break
 
             self.job_manager = None
             logger.debug("Localhost job manager finished")
 
         if not self.job_manager:
             self.job_manager = threading.Thread(target=job_manager)
             self.job_manager.start()
@@ -125,25 +137,26 @@
         logger.info(f"Deploying runtime: {runtime_name}")
         return self.env.get_metadata()
 
     def invoke(self, job_payload):
         """
         Run the job description against the selected environment
         """
+        self.invocation_in_progress = True
         executor_id = job_payload['executor_id']
         job_id = job_payload['job_id']
 
         logger.debug(f'ExecutorID {executor_id} | JobID {job_id} - Putting job into localhost queue')
 
-        self.start_manager()
-
         job_filename = self.env.prepare_job_file(job_payload)
-
         self.job_queue.put((job_payload, job_filename))
 
+        self.start_manager()
+        self.invocation_in_progress = False
+
     def get_runtime_key(self, runtime_name, *args):
         """
         Generate the runtime key that identifies the runtime
         """
         runtime_key = os.path.join('localhost', __version__, runtime_name.strip("/"))
 
         return runtime_key
@@ -166,48 +179,45 @@
         """
         pass
 
     def clear(self, job_keys=None, exception=None):
         """
         Kills all running jobs processes
         """
-        self.should_run = False
-
         while not self.job_queue.empty():
             try:
                 self.job_queue.get(False)
             except Exception:
                 pass
 
         self.env.stop(job_keys)
 
         if self.job_manager:
             self.job_queue.put((None, None))
 
-        self.should_run = True
-
 
-class BaseEnv:
+class ExecutionEnvironment:
     """
     Base environment class for shared methods
     """
 
     def __init__(self, config):
         self.config = config
         self.runtime_name = self.config['runtime']
+        self.is_unix_system = is_unix_system()
         self.jobs = {}  # dict to store executed jobs (job_keys) and PIDs
 
     def _copy_lithops_to_tmp(self):
-        if is_lithops_worker() and os.path.isfile(RUNNER):
+        if is_lithops_worker() and os.path.isfile(RUNNER_FILE):
             return
         os.makedirs(LITHOPS_TEMP_DIR, exist_ok=True)
         shutil.rmtree(os.path.join(LITHOPS_TEMP_DIR, 'lithops'), ignore_errors=True)
         shutil.copytree(LITHOPS_LOCATION, os.path.join(LITHOPS_TEMP_DIR, 'lithops'))
         src_handler = os.path.join(LITHOPS_LOCATION, 'localhost', 'v1', 'runner.py')
-        copyfile(src_handler, RUNNER)
+        copyfile(src_handler, RUNNER_FILE)
 
     def prepare_job_file(self, job_payload):
         """
         Creates the job file that contains the job payload to be executed
         """
         job_key = job_payload['job_key']
         storage_backend = job_payload['config']['lithops']['storage']
@@ -219,15 +229,15 @@
 
         os.makedirs(local_job_dir, exist_ok=True)
         local_job_filename = os.path.join(local_job_dir, job_file)
 
         with open(local_job_filename, 'w') as jl:
             json.dump(job_payload, jl, default=str)
 
-        if isinstance(self, DockerEnv):
+        if isinstance(self, ContainerEnvironment):
             job_filename = f'{docker_job_dir}/{job_file}'
         else:
             job_filename = local_job_filename
 
         return job_filename
 
     def stop(self, job_keys=None):
@@ -235,15 +245,15 @@
         Stops running processes
         """
 
         def kill_job(job_key):
             if self.jobs[job_key].poll() is None:
                 logger.debug(f'Killing job {job_key} with PID {self.jobs[job_key].pid}')
                 PID = self.jobs[job_key].pid
-                if is_unix_system():
+                if self.is_unix_system:
                     PGID = os.getpgid(PID)
                     os.killpg(PGID, signal.SIGKILL)
                 else:
                     os.kill(PID, signal.SIGTERM)
             del self.jobs[job_key]
 
         to_delete = job_keys or list(self.jobs.keys())
@@ -251,123 +261,129 @@
             try:
                 if job_key in self.jobs:
                     kill_job(job_key)
             except Exception:
                 pass
 
 
-class DefaultEnv(BaseEnv):
+class DefaultEnvironment(ExecutionEnvironment):
     """
     Default environment uses current python3 installation
     """
 
     def __init__(self, config):
         super().__init__(config)
-        logger.debug(f'Starting python environment for {self.runtime_name}')
+        logger.debug(f'Starting default environment for {self.runtime_name}')
 
     def setup(self):
-        logger.debug('Setting up python environment')
+        logger.debug('Setting up default environment')
         self._copy_lithops_to_tmp()
 
     def get_metadata(self):
-        if not os.path.isfile(RUNNER):
+        if not os.path.isfile(RUNNER_FILE):
             self.setup()
 
-        logger.debug(f"Extracting runtime metadata from: {self.runtime_name}")
-        cmd = [self.runtime_name, RUNNER, 'get_metadata']
-        process = sp.run(cmd, check=True, stdout=sp.PIPE, universal_newlines=True,
-                         start_new_session=True)
+        logger.debug(f"Extracting metadata from: {self.runtime_name}")
+        cmd = [self.runtime_name, RUNNER_FILE, 'get_metadata']
+        process = sp.run(
+            cmd, check=True,
+            stdout=sp.PIPE,
+            universal_newlines=True,
+            start_new_session=True
+        )
         runtime_meta = json.loads(process.stdout.strip())
         return runtime_meta
 
-    def run(self, job_key, job_filename):
+    def run_job(self, job_key, job_filename):
         """
         Runs a job
         """
-        if not os.path.isfile(RUNNER):
+        if not os.path.isfile(RUNNER_FILE):
             self.setup()
 
-        cmd = [self.runtime_name, RUNNER, 'run_job', job_filename]
-        log = open(RN_LOG_FILE, 'a')
-        process = sp.Popen(cmd, stdout=log, stderr=log, start_new_session=True)
+        cmd = [self.runtime_name, RUNNER_FILE, 'run_job', job_filename]
+        process = sp.Popen(cmd, start_new_session=True)
         self.jobs[job_key] = process
 
         return process
 
 
-class DockerEnv(BaseEnv):
+class ContainerEnvironment(ExecutionEnvironment):
     """
     Docker environment uses a docker runtime image
     """
 
     def __init__(self, config):
         super().__init__(config)
+        logger.debug(f'Starting container environment for {self.runtime_name}')
         self.use_gpu = self.config.get('use_gpu', False)
-        logger.debug(f'Starting docker environment for {self.runtime_name}')
-        self.uid = os.getuid() if is_unix_system() else None
-        self.gid = os.getgid() if is_unix_system() else None
+        self.docker_path = get_docker_path()
+        self.is_podman = is_podman(self.docker_path)
+        self.uid = os.getuid() if self.is_unix_system else None
+        self.gid = os.getgid() if self.is_unix_system else None
 
     def setup(self):
-        logger.debug('Setting up Docker environment')
+        logger.debug('Setting up container environment')
         self._copy_lithops_to_tmp()
         if self.config.get('pull_runtime', False):
-            logger.debug('Pulling Docker runtime {}'.format(self.runtime_name))
-            sp.run(shlex.split(f'docker pull {self.runtime_name}'), check=True,
-                   stdout=sp.PIPE, universal_newlines=True)
+            logger.debug(f'Pulling runtime {self.runtime_name}')
+            sp.run(
+                shlex.split(f'docker pull {self.runtime_name}'), check=True,
+                stdout=sp.PIPE, universal_newlines=True
+            )
 
     def get_metadata(self):
-        if not os.path.isfile(RUNNER):
+        if not os.path.isfile(RUNNER_FILE):
             self.setup()
 
-        logger.debug(f"Extracting runtime metadata from: {self.runtime_name}")
+        logger.debug(f"Extracting metadata from: {self.runtime_name}")
 
         tmp_path = Path(TEMP_DIR).as_posix()
-        docker_path = get_docker_path()
 
-        cmd = f'{docker_path} run --name lithops_metadata '
-        cmd += f'--user {self.uid}:{self.gid} ' if is_unix_system() else ''
+        cmd = f'{self.docker_path} run --name lithops_metadata '
+        cmd += f'--user {self.uid}:{self.gid} ' if self.is_unix_system and not self.is_podman else ''
         cmd += f'--env USER={os.getenv("USER", "root")} '
         cmd += f'--rm -v {tmp_path}:/tmp --entrypoint "python3" '
         cmd += f'{self.runtime_name} /tmp/{USER_TEMP_DIR}/localhost-runner.py get_metadata'
 
-        process = sp.run(shlex.split(cmd), check=True, stdout=sp.PIPE,
-                         universal_newlines=True, start_new_session=True)
+        process = sp.run(
+            shlex.split(cmd), check=True, stdout=sp.PIPE,
+            universal_newlines=True, start_new_session=True
+        )
         runtime_meta = json.loads(process.stdout.strip())
 
         return runtime_meta
 
-    def run(self, job_key, job_filename):
+    def run_job(self, job_key, job_filename):
         """
         Runs a job
         """
-        if not os.path.isfile(RUNNER):
+        if not os.path.isfile(RUNNER_FILE):
             self.setup()
 
         tmp_path = Path(TEMP_DIR).as_posix()
-        docker_path = get_docker_path()
 
-        cmd = f'{docker_path} run --name lithops_{job_key} '
+        cmd = f'{self.docker_path} run --name lithops_{job_key} '
         cmd += '--gpus all ' if self.use_gpu else ''
-        cmd += f'--user {self.uid}:{self.gid} ' if is_unix_system() else ''
+        cmd += f'--user {self.uid}:{self.gid} ' if self.is_unix_system and not self.is_podman else ''
         cmd += f'--env USER={os.getenv("USER", "root")} '
         cmd += f'--rm -v {tmp_path}:/tmp --entrypoint "python3" '
         cmd += f'{self.runtime_name} /tmp/{USER_TEMP_DIR}/localhost-runner.py run_job {job_filename}'
 
-        log = open(RN_LOG_FILE, 'a')
-        process = sp.Popen(shlex.split(cmd), stdout=log, stderr=log, start_new_session=True)
+        process = sp.Popen(shlex.split(cmd), start_new_session=True)
         self.jobs[job_key] = process
 
         return process
 
     def stop(self, job_keys=None):
         """
         Stops running containers
         """
-        if job_keys:
-            for job_key in job_keys:
-                sp.Popen(shlex.split(f'docker rm -f lithops_{job_key}'),
-                         stdout=sp.DEVNULL, stderr=sp.DEVNULL)
-        else:
-            for job_key in self.jobs:
-                sp.Popen(shlex.split(f'docker rm -f lithops_{job_key}'),
-                         stdout=sp.DEVNULL, stderr=sp.DEVNULL)
+        jk_to_delete = job_keys or list(self.jobs.keys())
+
+        for job_key in jk_to_delete:
+            sp.Popen(
+                shlex.split(f'{self.docker_path} rm -f lithops_{job_key}'),
+                stdout=sp.DEVNULL, stderr=sp.DEVNULL
+            )
+
         super().stop(job_keys)
```

### Comparing `lithops-3.3.0/lithops/localhost/v1/runner.py` & `lithops-3.4.0/lithops/localhost/v1/runner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/localhost/v2/localhost.py` & `lithops-3.4.0/lithops/storage/backends/swift/swift.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# (C) Copyright IBM Corp. 2023
+# (C) Copyright IBM Corp. 2020
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,307 +12,278 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
 import json
-import uuid
-import shlex
-import time
-import signal
-import lithops
-import logging
 import shutil
-import xmlrpc.client
-import subprocess as sp
-from enum import Enum
-from shutil import copyfile
-from pathlib import Path
-
-from lithops.version import __version__
-from lithops.constants import (
-    LOCALHOST_SERVICE_CHECK_INTERVAL,
-    LOCALHOST_SERVICE_IDLE_TIMEOUT,
-    LOCALHOST_RUNTIME_DEFAULT,
-    TEMP_DIR,
-    USER_TEMP_DIR,
-    LITHOPS_TEMP_DIR,
-    COMPUTE_CLI_MSG,
-    SV_LOG_FILE,
-    CPU_COUNT,
-)
-from lithops.utils import (
-    BackendType,
-    find_free_port,
-    get_docker_path,
-    is_lithops_worker,
-    is_unix_system
-)
+import logging
+import requests
+from lithops.storage.utils import StorageNoSuchKeyError
+from lithops.utils import sizeof_fmt
+from lithops.constants import STORAGE_CLI_MSG
 
 logger = logging.getLogger(__name__)
 
-SERVICE_FILE = os.path.join(LITHOPS_TEMP_DIR, 'localhost-service.py')
-LITHOPS_LOCATION = os.path.dirname(os.path.abspath(lithops.__file__))
-
-
-class LocalhostMode(Enum):
-    CREATE = 'create'
-    REUSE = 'reuse'
 
-
-class LocalhostHandlerV2:
+class StorageBackend:
     """
-    A localhostHandler object is used by invokers and other components to
-    access underlying localhost backend without exposing the implementation
-    details.
+    A wrap-up around OpenStack Swift APIs.
     """
 
-    def __init__(self, localhost_config):
-        logger.debug('Creating Localhost compute client')
-        self.config = localhost_config
-        self.runtime_name = self.config.get('runtime', LOCALHOST_RUNTIME_DEFAULT)
-        self.env = None
-
-        msg = COMPUTE_CLI_MSG.format('Localhost compute v2')
-        logger.info(f"{msg}")
-
-    def get_backend_type(self):
-        """
-        Wrapper method that returns the type of the backend (Batch or FaaS)
-        """
-        return BackendType.BATCH.value
-
-    def init(self):
-        """
-        Init tasks for localhost
-        """
-        default_env = self.runtime_name.startswith(('python', '/'))
-        self.env = DefaultEnv(self.config) if default_env else DockerEnv(self.config)
-        self.env.setup()
-
-    def deploy_runtime(self, runtime_name, *args):
-        """
-        Extract the runtime metadata and preinstalled modules
-        """
-        logger.info(f"Deploying runtime: {runtime_name}")
-        return self.env.get_metadata()
-
-    def invoke(self, job_payload):
-        """
-        Run the job description against the selected environment
-        """
-        executor_id = job_payload['executor_id']
-        job_id = job_payload['job_id']
-        total_calls = len(job_payload['call_ids'])
-
-        logger.debug(f'ExecutorID {executor_id} | JobID {job_id} - Running '
-                     f'{total_calls} activations in the localhost worker')
-        self.env.run(job_payload)
-
-    def get_runtime_key(self, runtime_name, *args):
-        """
-        Generate the runtime key that identifies the runtime
-        """
-        runtime_key = os.path.join('localhost', __version__, runtime_name.strip("/"))
-
-        return runtime_key
-
-    def get_runtime_info(self):
-        """
-        Method that returns a dictionary with all the relevant runtime
-        information set in config
-        """
-        return {
-            'runtime_name': self.config['runtime'],
-            'runtime_memory': self.config.get('runtime_memory'),
-            'runtime_timeout': self.config.get('runtime_timeout'),
-            'max_workers': self.config['max_workers'],
+    def __init__(self, swift_config):
+        logger.debug("Creating OpenStack Swift client")
+        self.auth_url = swift_config['auth_url']
+        self.user_id = swift_config['user_id']
+        self.project_id = swift_config['project_id']
+        self.password = swift_config['password']
+        self.region = swift_config['region']
+        self.user_domain_name = swift_config.get("user_domain_name", "default")
+        self.project_domain_name = swift_config.get("project_domain_name", "default")
+        self.endpoint = None
+
+        if 'token' in swift_config:
+            self.token = swift_config['token']
+            self.endpoint = swift_config['endpoint']
+        else:
+            self.token = self.generate_swift_token()
+            swift_config['token'] = self.token
+            swift_config['endpoint'] = self.endpoint
+
+        self.session = requests.session()
+        self.session.headers.update({'X-Auth-Token': self.token})
+        adapter = requests.adapters.HTTPAdapter(pool_maxsize=64, max_retries=3)
+        self.session.mount('http://', adapter)
+        self.session.mount('https://', adapter)
+
+        msg = STORAGE_CLI_MSG.format('OpenStack Swift')
+        logger.info("{} - Region: {}".format(msg, self.region))
+
+    def generate_bucket_name(self):
+        """
+        Generates a unique bucket name
+        """
+        self.config['storage_bucket'] = f'lithops-{self.region}-{self.user_id[:6].lower()}'
+
+        return self.config['storage_bucket']
+
+    def generate_swift_token(self):
+        """
+        Generates new token for accessing to Swift.
+        :return: token
+        """
+        url = self.auth_url + "/v3/auth/tokens"
+        headers = {'Content-Type': 'application/json'}
+        data = {
+            "auth": {
+                "identity": {
+                    "methods": ["password"],
+                    "password": {
+                        "user": {
+                            "name": self.user_id,
+                            "password": self.password,
+                            "domain": {"name": self.user_domain_name}
+                        }
+                    }
+                },
+                "scope": {
+                    "project": {
+                        "id": self.project_id,
+                        "domain": {"name": self.project_domain_name}
+                    }
+                }
+            }
         }
+        json_data = json.dumps(data)
 
-    def clean(self, **kwargs):
-        """
-        Deletes all local runtimes
-        """
-        pass
+        r = requests.post(url, data=json_data, headers=headers)
 
-    def clear(self, job_keys=None, exception=None):
-        """
-        Kills the running service in case of exception
-        """
-        if exception is not None:
-            self.env.stop(job_keys)
+        if r.status_code == 201:
+            backend_info = json.loads(r.text)
 
+            for service in backend_info['token']['catalog']:
+                if service['name'] == 'swift':
+                    for endpoint in service['endpoints']:
+                        if endpoint['region'] == self.region:
+                            if endpoint['interface'] == 'public':
+                                self.endpoint = endpoint['url'].replace('https:', 'http:')
 
-class BaseEnv:
-    """
-    Base environment class for shared methods
-    """
-
-    def __init__(self, config):
-        self.config = config
-        self.runtime_name = self.config['runtime']
-        self.worker_processes = self.config.get('worker_processes', CPU_COUNT)
-        self.max_idle_timeout = self.config.get('max_idle_timeout', LOCALHOST_SERVICE_IDLE_TIMEOUT)
-        self.check_interval = self.config.get('check_interval', LOCALHOST_SERVICE_CHECK_INTERVAL)
-        self.job_keys = []
-        self.service_process = None
-        self.client = None
-        self.service_running = False
-
-    def _copy_lithops_to_tmp(self):
-        if is_lithops_worker() and os.path.isfile(SERVICE_FILE):
-            return
-        os.makedirs(LITHOPS_TEMP_DIR, exist_ok=True)
-        shutil.rmtree(os.path.join(LITHOPS_TEMP_DIR, 'lithops'), ignore_errors=True)
-        shutil.copytree(LITHOPS_LOCATION, os.path.join(LITHOPS_TEMP_DIR, 'lithops'))
-        src_handler = os.path.join(LITHOPS_LOCATION, 'localhost', 'v2', 'service.py')
-        copyfile(src_handler, SERVICE_FILE)
-
-    def get_metadata(self):
-        self.start_service()
-        logger.debug(f"Extracting runtime metadata from: {self.runtime_name}")
-
-        while True:
-            try:
-                response = self.client.extract_runtime_meta()
-                break
-            except (ConnectionRefusedError, ConnectionResetError):
-                time.sleep(0.1)
+            if not self.endpoint:
+                raise Exception('Invalid region name')
 
-        if response:
-            return json.loads(response)
+            return r.headers['X-Subject-Token']
         else:
-            raise Exception("An error ocurred trying to get the runtime metadata. "
-                            f"Check {SERVICE_FILE.replace('.py', '.log')}")
+            message = json.loads(r.text)['error']['message']
+            raise Exception("{} - {} - {}".format(r.status_code, r.reason, message))
 
-    def run(self, job_payload):
+    def put_object(self, bucket_name, key, data):
         """
-        Adds a job to the localhost service
-        """
-        self.start_service()
-        self.job_keys.append(job_payload['job_key'])
-        invoked = False
-        while not invoked:
+        Put an object in Swift. Override the object if the key already exists.
+        :param key: key of the object.
+        :param data: data of the object
+        :type data: str/bytes
+        :return: None
+        """
+        url = '/'.join([self.endpoint, bucket_name, key])
+        try:
+            res = self.session.put(url, data=data)
+            status = 'OK' if res.status_code == 201 else 'Error'
             try:
-                invoked = self.client.add_job(json.dumps(job_payload))
-            except (ConnectionRefusedError, ConnectionResetError):
-                time.sleep(0.1)
-
-    def stop(self, job_keys):
-        """
-        Stops localhost executor service
-        """
-        job_keys = job_keys or list(self.jobs_keys)
-
-        if self.service_running:
-            self.service_running = False
-            if self.service_process and self.service_process.poll() is None:
-                PID = self.service_process.pid
-                logger.debug(f'Stopping localhost executor service with PID {PID}')
-                if is_unix_system():
-                    PGID = os.getpgid(PID)
-                    os.killpg(PGID, signal.SIGKILL)
+                logger.debug('PUT Object {} - Size: {} - {}'.format(key, sizeof_fmt(len(data)), status))
+            except Exception:
+                logger.debug('PUT Object {} - {}'.format(key, status))
+        except Exception as e:
+            print(e)
+
+    def get_object(self, bucket_name, key, stream=False, extra_get_args={}):
+        """
+        Get object from Swift with a key. Throws StorageNoSuchKeyError if the given key does not exist.
+        :param key: key of the object
+        :return: Data of the object
+        :rtype: str/bytes
+        """
+        url = '/'.join([self.endpoint, bucket_name, key])
+        headers = {'X-Auth-Token': self.token}
+        headers.update(extra_get_args)
+        try:
+            res = self.session.get(url, headers=headers, stream=stream)
+            if res.status_code == 200 or res.status_code == 206:
+                if stream:
+                    data = res.raw
                 else:
-                    os.kill(PID, signal.SIGTERM)
-            self.service_process = None
-
-
-class DefaultEnv(BaseEnv):
-    """
-    Default environment uses current python3 installation
-    """
-
-    def __init__(self, config):
-        super().__init__(config)
-        logger.debug(f'Starting python environment for {self.runtime_name}')
-
-    def setup(self):
-        logger.debug('Setting up python environment')
-        self._copy_lithops_to_tmp()
-
-    def start_service(self):
-        if self.service_process and self.service_process.poll() is None:
-            return
-
-        if not os.path.isfile(SERVICE_FILE):
-            self.setup()
-
-        logger.debug('Starting localhost executor service - Python environment')
-
-        service_port = find_free_port()
-
-        cmd = [self.runtime_name, SERVICE_FILE, str(self.worker_processes),
-               str(service_port), str(self.max_idle_timeout), str(self.check_interval)]
-        log = open(SV_LOG_FILE, 'a')
-        process = sp.Popen(cmd, stdout=log, stderr=log, start_new_session=True)
-        self.service_process = process
-
-        self.client = xmlrpc.client.ServerProxy(f'http://localhost:{service_port}')
-        self.service_running = True
-
-    def join(self):
+                    data = res.content
+                return data
+            elif res.status_code == 404:
+                raise StorageNoSuchKeyError(bucket_name, key)
+            else:
+                raise Exception('{} - {}'.format(res.status_code, key))
+        except StorageNoSuchKeyError:
+            raise StorageNoSuchKeyError(bucket_name, key)
+        except Exception as e:
+            print(e)
+            raise StorageNoSuchKeyError(bucket_name, key)
+
+    def upload_file(self, file_name, bucket, key=None, extra_args={}, config=None):
+        """Upload a file
+
+        :param file_name: File to upload
+        :param bucket: Bucket to upload to
+        :param key: S3 object name. If not specified then file_name is used
+        :return: True if file was uploaded, else False
+        """
+        # If S3 key was not specified, use file_name
+        if key is None:
+            key = os.path.basename(file_name)
+
+        # Upload the file
+        try:
+            with open(file_name, 'rb') as in_file:
+                self.put_object(bucket, key, in_file)
+        except Exception as e:
+            logging.error(e)
+            return False
+        return True
+
+    def download_file(self, bucket, key, file_name=None, extra_args={}, config=None):
+        """Download a file
+
+        :param bucket: Bucket to download from
+        :param key: S3 object name. If not specified then file_name is used
+        :param file_name: File to upload
+        :return: True if file was downloaded, else False
+        """
+        # If file_name was not specified, use S3 key
+        if file_name is None:
+            file_name = key
+
+        # Download the file
+        try:
+            dirname = os.path.dirname(file_name)
+            if dirname and not os.path.exists(dirname):
+                os.makedirs(dirname)
+            with open(file_name, 'wb') as out:
+                data_stream = self.get_object(bucket, key, stream=True)
+                shutil.copyfileobj(data_stream, out)
+        except Exception as e:
+            logging.error(e)
+            return False
+        return True
+
+    def head_object(self, bucket_name, key):
+        """
+        Head object from Swift with a key. Throws StorageNoSuchKeyError if the given key does not exist.
+        :param key: key of the object
+        :return: Data of the object
+        :rtype: str/bytes
+        """
+        url = '/'.join([self.endpoint, bucket_name, key])
+        try:
+            res = self.session.head(url)
+            if res.status_code == 200:
+                return res.headers
+            elif res.status_code == 404:
+                raise StorageNoSuchKeyError(bucket_name, key)
+            else:
+                raise Exception('{} - {}'.format(res.status_code, key))
+        except Exception:
+            raise StorageNoSuchKeyError(bucket_name, key)
+
+    def delete_object(self, bucket_name, key):
+        """
+        Delete an object from Swift.
+        :param bucket: bucket name
+        :param key: data key
+        """
+        url = '/'.join([self.endpoint, bucket_name, key])
+        return self.session.delete(url)
+
+    def delete_objects(self, bucket_name, key_list):
+        """
+        Delete a list of objects from Swift.
+        :param bucket: bucket name
+        :param key: data key
+        """
+        headers = {'X-Auth-Token': self.token,
+                   'X-Bulk-Delete': 'True'}
+
+        keys_to_delete = []
+        for key in key_list:
+            keys_to_delete.append('/{}/{}'.format(bucket_name, key))
+
+        keys_to_delete = '\n'.join(keys_to_delete)
+        url = '/'.join([self.endpoint, '?bulk-delete'])
+        return self.session.delete(url, data=keys_to_delete, headers=headers)
+
+    def list_objects(self, bucket_name, prefix='', match_pattern=None):
+        """
+        Lists the objects in a bucket. Throws StorageNoSuchKeyError if the given bucket does not exist.
+        :param key: key of the object
+        :return: Data of the object
+        :rtype: str/bytes
         """
-        Waits until the underlying service finishes its execution
-        """
-        while self.service_process and self.service_process.poll() is None:
-            time.sleep(5)
-
-
-class DockerEnv(BaseEnv):
-    """
-    Docker environment uses a docker runtime image
-    """
-
-    def __init__(self, config):
-        super().__init__(config)
-        self.use_gpu = self.config.get('use_gpu', False)
-        logger.debug(f'Starting docker environment for {self.runtime_name}')
-        self.container_id = str(uuid.uuid4()).replace('-', '')[:12]
-        self.uid = os.getuid() if is_unix_system() else None
-        self.gid = os.getgid() if is_unix_system() else None
-
-    def setup(self):
-        logger.debug('Setting up Docker environment')
-        self._copy_lithops_to_tmp()
-        if self.config.get('pull_runtime', False):
-            logger.debug('Pulling Docker runtime {}'.format(self.runtime_name))
-            sp.run(shlex.split(f'docker pull {self.runtime_name}'), check=True,
-                   stdout=sp.PIPE, universal_newlines=True)
-
-    def start_service(self):
-        if self.service_process and self.service_process.poll() is None:
-            return
-
-        if not os.path.isfile(SERVICE_FILE):
-            self.setup()
-
-        logger.debug('Starting localhost executor service - Docker environemnt')
-
-        tmp_path = Path(TEMP_DIR).as_posix()
-        docker_path = get_docker_path()
-        service_port = find_free_port()
-
-        cmd = f'{docker_path} run --name lithops_{self.container_id} '
-        cmd += '--gpus all ' if self.use_gpu else ''
-        cmd += f'--user {self.uid}:{self.gid} ' if is_unix_system() else ''
-        cmd += f'--env USER={os.getenv("USER", "root")} '
-        cmd += f'-p {service_port}:{service_port} '
-        cmd += f'--rm -v {tmp_path}:/tmp --entrypoint "python3" '
-        cmd += f'{self.runtime_name} /tmp/{USER_TEMP_DIR}/localhost-service.py '
-        cmd += f'{self.worker_processes} {service_port} '
-        cmd += f'{self.max_idle_timeout} {self.check_interval}'
-
-        log = open(SV_LOG_FILE, 'a')
-        process = sp.Popen(shlex.split(cmd), stdout=log, stderr=log, start_new_session=True)
-        self.service_process = process
-
-        self.client = xmlrpc.client.ServerProxy(f'http://localhost:{service_port}')
-        self.service_running = True
-
-    def stop(self):
-        """
-        Stops localhost service container containers
-        """
-        sp.Popen(shlex.split(f'docker rm -f lithops_{self.container_id}'),
-                 stdout=sp.DEVNULL, stderr=sp.DEVNULL)
-        super().stop()
+        if prefix:
+            url = '/'.join([self.endpoint, bucket_name, '?format=json&prefix=' + prefix])
+        else:
+            url = '/'.join([self.endpoint, bucket_name, '?format=json'])
+        try:
+            res = self.session.get(url)
+            objects = res.json()
+
+            # TODO: Adapt to Key and Size
+            return objects
+        except Exception as e:
+            raise e
+
+    def list_keys(self, bucket_name, prefix):
+        """
+        Return a list of keys for the given prefix.
+        :param prefix: Prefix to filter object names.
+        :return: List of keys in bucket that match the given prefix.
+        :rtype: list of str
+        """
+        try:
+            objects = self.list_objects(bucket_name, prefix)
+            object_keys = [r['name'] for r in objects]
+            return object_keys
+        except Exception as e:
+            raise e
```

### Comparing `lithops-3.3.0/lithops/localhost/v2/service.py` & `lithops-3.4.0/lithops/multiprocessing/process.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,248 +1,280 @@
 #
-# (C) Copyright IBM Corp. 2023
+# Module providing the `Process` class which emulates `threading.Thread`
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# multiprocessing/process.py
+#
+# Copyright (c) 2006-2008, R Oudkerk
+# Licensed to PSF under a Contributor Agreement.
+#
+# Modifications Copyright (c) 2020 Cloudlab URV
+#
+
+#
+# Imports
 #
 
+import itertools
+import traceback
 import os
-import time
-import json
-import sys
 import logging
-import platform
-import threading
-import multiprocessing as mp
-from enum import Enum
-from queue import Empty
-from multiprocessing.managers import SyncManager
-from xmlrpc.server import SimpleXMLRPCServer
-
-from lithops import utils
-from lithops.worker.utils import get_runtime_metadata
-from lithops.worker.handler import (
-    ShutdownSentinel,
-    create_job,
-    prepare_and_run_task
-)
-from lithops.constants import (
-    CPU_COUNT,
-    LITHOPS_TEMP_DIR,
-    JOBS_DIR,
-    LOCALHOST_SERVICE_CHECK_INTERVAL,
-    LOCALHOST_SERVICE_IDLE_TIMEOUT,
-    LOGS_DIR,
-    SV_LOG_FILE,
-    LOGGER_FORMAT
-)
-
-log_file_stream = open(SV_LOG_FILE, 'a')
-
-os.makedirs(LITHOPS_TEMP_DIR, exist_ok=True)
-os.makedirs(JOBS_DIR, exist_ok=True)
-os.makedirs(LOGS_DIR, exist_ok=True)
-
-logging.basicConfig(stream=log_file_stream, level=logging.DEBUG, format=LOGGER_FORMAT)
-logger = logging.getLogger('lithops.localhost.service')
-
-# Change spawn method for MacOS
-if platform.system() == 'Darwin':
-    mp.set_start_method("fork")
-
-task_runners = []
-
-# Set Localhost backend to the env
-os.environ['__LITHOPS_BACKEND'] = 'Localhost'
-
-
-class ProcessStatus(Enum):
-    IDLE = 'idle'
-    BUSY = 'busy'
-
-
-class ServerThread(threading.Thread):
-
-    def __init__(self, service_port, work_queue):
-        super().__init__()
-
-        self.server = SimpleXMLRPCServer(('0.0.0.0', service_port), logRequests=False)
-
-        self.service_port = service_port
-        self.work_queue = work_queue
-
-        self.server.register_function(self.add_job, 'add_job')
-        self.server.register_function(self.extract_runtime_meta, 'extract_runtime_meta')
-
-    def add_job(self, job_payload):
-        logger.info("Received new job")
-        job = create_job(json.loads(job_payload))
-        logger.info(f'ExecutorID {job.executor_id} | JobID {job.job_id} - Adding '
-                    f'{job.total_calls} tasks in the localhost worker')
-        try:
-            job_status_dict[job.job_key] = 0
-            for call_id in job.call_ids:
-                data = job.data.pop(0)
-                self.work_queue.put((job, call_id, data))
-            return True
-        except Exception as e:
-            logger.debug(e)
-            return False
-
-    def extract_runtime_meta(self):
-        logger.info('Requesting runtime metadata')
-        try:
-            runtime_meta = get_runtime_metadata()
-            return json.dumps(runtime_meta)
-        except Exception as e:
-            logger.debug(e)
-            return False
+import multiprocessing as _mp
 
-    def start(self):
-        logger.info(f'Lithops localhost executor service started on port {self.service_port}')
-        self.server.serve_forever()
+from lithops import FunctionExecutor
+from lithops.utils import is_lithops_worker
+from . import config as mp_config
+from . import util
 
-    def stop(self):
-        logger.info('Shutting down the executor service')
-        for process_runner in range(len(task_runners)):
-            try:
-                self.work_queue.put(ShutdownSentinel())
-            except Exception:
-                pass
-        for runner in task_runners:
-            runner.join()
-        self.server.shutdown()
-        self.server.server_close()
-
-
-def check_inactivity(server_thread, max_idle_timeout, check_interval):
-    """
-    A thread that checks if the service is inactive every 'check_interval'
-    until 'max_idle_timeout,' where it automatically stops itself.
-    """
-    tasks_running = False
-    last_usage_time = time.time()
-
-    while True:
-        time.sleep(check_interval)
-
-        if all(value == ProcessStatus.IDLE.value for value in worker_status_dict.values()):
-            if tasks_running:
-                tasks_running = False
-                last_usage_time = time.time()
-        else:
-            tasks_running = True
-            last_usage_time = time.time()
+#
+#
+#
 
-        time_since_last_usage = time.time() - last_usage_time
+try:
+    ORIGINAL_DIR = os.path.abspath(os.getcwd())
+except OSError:
+    ORIGINAL_DIR = None
+
+_process_counter = itertools.count(1)
+_children = set()
+logger = logging.getLogger(__name__)
 
-        if int(max_idle_timeout - time_since_last_usage) <= 0:
-            server_thread.stop()
-            break
 
+#
+# Public functions
+#
 
-def process_event(
-        event, pid,
-        worker_status_dict
-):
+def current_process():
     """
-    Processes the events received from the work queue
+    Return process object representing the current process
     """
-    task, call_id, data = event
-    task.call_id = call_id
-    task.data = data
-
-    worker_status_dict[pid] = ProcessStatus.BUSY.value
-
-    prepare_and_run_task(task)
+    if is_lithops_worker():
+        p = CloudProcess(name=os.environ.get('LITHOPS_MP_WORKER_NAME'))
+        p._pid = os.environ.get('__LITHOPS_SESSION_ID', '-1')
+        return p
+    else:
+        return _mp.current_process()
 
-    worker_status_dict[pid] = ProcessStatus.IDLE.value
 
-    # task_id = f'{task.job_key}-{task.call_id}'
-    # Path(os.path.join(JOBS_DIR, f'{task_id}' + '.done')).touch()
+def active_children():
+    """
+    Return list of process objects corresponding to live child processes
+    """
+    raise NotImplementedError()
 
 
-def python_queue_consumer(
-        pid,
-        work_queue,
-        worker_status_dict
-):
+def parent_process():
     """
-    Listens to the job_queue and executes the individual job tasks
+    Return process object representing the parent process
     """
-    logger.info(f'Worker process {pid} started')
-    while True:
-        try:
-            event = work_queue.get(block=True)
-        except Empty:
-            break
-        except BrokenPipeError:
-            break
-
-        if isinstance(event, ShutdownSentinel):
-            break
-
-        process_event(event, pid, worker_status_dict)
-
-    logger.info(f'Worker process {pid} finished')
-
-
-if __name__ == "__main__":
-    logger.info('*' * 60)
-
-    worker_processes = int(sys.argv[1]) if len(sys.argv) > 1 else CPU_COUNT
-    service_port = int(sys.argv[2]) if len(sys.argv) > 2 else utils.find_free_port()
-    max_idle_timeout = int(sys.argv[3]) if len(sys.argv) > 3 else LOCALHOST_SERVICE_IDLE_TIMEOUT
-    check_interval = int(sys.argv[4]) if len(sys.argv) > 4 else LOCALHOST_SERVICE_CHECK_INTERVAL
-
-    logger.info(f'Starting Lithops localhost executor service - Worker processes: {worker_processes}')
-
-    manager = SyncManager()
-    manager.start()
-    work_queue = manager.Queue()
-    worker_status_dict = manager.dict()
-    job_status_dict = manager.dict()
-    job_status_lock = manager.Lock()
-
-    server_thread = ServerThread(service_port, work_queue)
-
-    # Start worker processes
-    for pid in range(int(worker_processes)):
-        worker_status_dict[pid] = ProcessStatus.IDLE.value
-        p = mp.Process(
-            target=python_queue_consumer,
-            args=(
-                pid,
-                work_queue,
-                worker_status_dict
-            )
-        )
-        task_runners.append(p)
-        p.start()
-
-    if max_idle_timeout >= 0:
-        logger.info('Starting inactivity checker thread: Idle timeout: '
-                    f'{max_idle_timeout} - Check interval {check_interval}')
-        threading.Thread(
-            target=check_inactivity,
-            args=(server_thread, max_idle_timeout, check_interval),
-            daemon=True
-        ).start()
+    raise NotImplementedError()
+
+
+#
+# Cloud worker
+#
+
+def cloud_process_wrapper(data, func, initializer=None, initargs=(), name=None, log_stream=None, op=None):
+    # Put worker name in envs to get it from within the function
+    os.environ['LITHOPS_MP_WORKER_NAME'] = 'test'
+
+    # Setup remote logger
+    if log_stream is not None:
+        remote_log_buff = util.RemoteLogIOBuffer(log_stream)
+        remote_log_buff.start()
     else:
-        logger.info('Inactivity checker thread is disabled because '
-                    f'of: Idle timeout: {max_idle_timeout}')
+        remote_log_buff = None
+
+    # Execute worker initializer function
+    if initializer is not None:
+        initializer(*initargs)
+
+    try:
+        if op == 'apply':
+            res = func(*data['args'], **data['kwargs'])
+        elif op == 'map':
+            res = func(data,)
+        elif op == 'starmap':
+            res = func(*data)
+        else:
+            exception = Exception(op)
+            raise exception
+        return res
+    except Exception as e:
+        # Print exception stack trace to remote logging buffer
+        exception = e
+        header = "---------- {} at {} ({}) ----------".format(e.__class__.__name__,
+                                                              os.environ.get('LITHOPS_MP_WORKER_NAME'),
+                                                              os.environ.get('__LITHOPS_SESSION_ID'))
+        exception_body = traceback.format_exc()
+        footer = '-' * len(header)
+        if remote_log_buff:
+            remote_log_buff.write('\n'.join([header, exception_body, footer, '']))
+    finally:
+        if remote_log_buff:
+            remote_log_buff.flush()
+            remote_log_buff.stop()
+
+    if exception:
+        raise exception
+
+    @property
+    def __name__(self):
+        return os.environ.get('LITHOPS_MP_WORKER_NAME')
 
-    server_thread.start()
 
-    manager.shutdown()
-    log_file_stream.flush()
-    logger.info('Lithops localhost executor service has been stopped')
-    log_file_stream.close()
+#
+# CloudProcess Class
+#
+
+class CloudProcess:
+    def __init__(self, group=None, target=None, name=None, args=None, kwargs=None, *, daemon=None):
+        assert group is None, 'process grouping is not implemented'
+
+        if args is None:
+            args = ()
+        if kwargs is None:
+            kwargs = {}
+
+        self._config = {}
+        self._parent_pid = os.getpid()
+        self._target = target
+        self._args = tuple(args)
+        self._kwargs = dict(kwargs)
+        self._name = name or (type(self).__name__ + '-' + str(next(_process_counter)))
+        self._pid = None
+        if daemon is not None:
+            self.daemon = daemon
+        lithops_config = mp_config.get_parameter(mp_config.LITHOPS_CONFIG)
+        self._executor = FunctionExecutor(**lithops_config)
+        self._future = None
+        self._sentinel = object()
+        self._remote_logger = None
+        self._redis = util.get_redis_client()
+
+    def run(self):
+        """
+        Method to be run in sub-process; can be overridden in sub-class
+        """
+        if self._target:
+            self._target(*self._args, **self._kwargs)
+
+    def start(self):
+        """
+        Start child process
+        """
+        assert not self._pid, 'cannot start a process twice'
+        assert self._parent_pid == os.getpid(), 'can only start a process object created by current process'
+
+        self._remote_logger, stream = util.setup_log_streaming(self._executor)
+
+        extra_env = mp_config.get_parameter(mp_config.ENV_VARS)
+
+        process_name = '-'.join(['CloudProcess', str(next(_process_counter)), self._target.__name__])
+        self._future = self._executor.call_async(cloud_process_wrapper,
+                                                 {'func': self._target,
+                                                  'data': {
+                                                      'args': self._args,
+                                                      'kwargs': self._kwargs
+                                                  },
+                                                  'initializer': None,
+                                                  'initargs': None,
+                                                  'name': process_name,
+                                                  'log_stream': stream,
+                                                  'op': 'apply'},
+                                                 extra_env=extra_env)
+        self._pid = '/'.join([self._future.executor_id, self._future.job_id, self._future.call_id])
+        del self._target, self._args, self._kwargs
+
+    def terminate(self):
+        """
+        Terminate process; sends SIGTERM signal or uses TerminateProcess()
+        """
+        raise NotImplementedError()
+
+    def join(self, timeout=None):
+        """
+        Wait until child process terminates
+        """
+        assert self._parent_pid == os.getpid(), 'can only join a child process'
+        assert self._pid, 'can only join a started process'
+
+        exception = None
+        try:
+            self._executor.wait(fs=[self._future])
+        except Exception as e:
+            exception = e
+        finally:
+            if self._remote_logger:
+                self._remote_logger.stop()
+
+            util.export_execution_details([self._future], self._executor)
+
+            if exception:
+                raise exception
+
+    def is_alive(self):
+        """
+        Return whether process is alive
+        """
+        raise NotImplementedError()
+
+    @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    def name(self, name):
+        assert isinstance(name, str), 'name must be a string'
+        self._name = name
+
+    @property
+    def daemon(self):
+        """
+        Return whether process is a daemon
+        """
+        return self._config.get('daemon', False)
+
+    @daemon.setter
+    def daemon(self, daemonic):
+        """
+        Set whether process is a daemon
+        """
+        assert not self._pid, 'process has already started'
+        self._config['daemon'] = daemonic
+
+    @property
+    def authkey(self):
+        return self._config['authkey']
+
+    @authkey.setter
+    def authkey(self, authkey):
+        """
+        Set authorization key of process
+        """
+        self._config['authkey'] = authkey
+
+    @property
+    def exitcode(self):
+        """
+        Return exit code of process or `None` if it has yet to stop
+        """
+        raise NotImplementedError()
+
+    @property
+    def ident(self):
+        """
+        Return identifier (PID) of process or `None` if it has yet to start
+        """
+        return self._pid
+
+    pid = ident
+
+    @property
+    def sentinel(self):
+        """
+        Return a file descriptor (Unix) or handle (Windows) suitable for
+        waiting for process termination.
+        """
+        try:
+            return self._sentinel
+        except AttributeError:
+            raise ValueError("process not started")
```

### Comparing `lithops-3.3.0/lithops/monitor.py` & `lithops-3.4.0/lithops/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import lithops
 import pickle
 import sys
 import queue
 import threading
 import concurrent.futures as cf
 from tblib import pickling_support
-from lithops.constants import MONITORING_INTERVAL
 
 pickling_support.install()
 
 logger = logging.getLogger(__name__)
 
 LOG_INTERVAL = 30  # Print monitor debug every LOG_INTERVAL seconds
 
@@ -76,19 +75,20 @@
     def remove_futures(self, fs):
         """
         Remove from the current thread a list of futures
         """
         self._print_status_log()
 
         for future in fs:
-            self.futures.remove(future)
+            if future in self.futures:
+                self.futures.remove(future)
 
-        present_jobs = {future.job_id for future in fs}
-        for job_id in present_jobs:
-            self.present_jobs.remove(job_id)
+        for job_id in {future.job_id for future in fs}:
+            if job_id in self.present_jobs:
+                self.present_jobs.remove(job_id)
 
     def _all_ready(self):
         """
         Checks if all futures are ready, success or done
         """
         return all([f.ready or f.success or f.done for f in self.futures])
 
@@ -424,33 +424,33 @@
 
     def run(self):
         """
         Run method
         """
         logger.debug(f'ExecutorID {self.executor_id} - Starting Storage job monitor')
 
-        WAIT_DUR_SEC = self.monitoring_interval
+        wait_dur_sec = self.monitoring_interval
         prevoius_log = None
         log_time = 0
 
         while not self._all_ready():
-            time.sleep(WAIT_DUR_SEC)
-            WAIT_DUR_SEC = self.monitoring_interval
-            log_time += WAIT_DUR_SEC
+            time.sleep(wait_dur_sec)
+            wait_dur_sec = self.monitoring_interval
+            log_time += wait_dur_sec
 
             if not self.should_run:
                 break
 
             callids_running, callids_done = \
                 self.internal_storage.get_job_status(self.executor_id)
 
             # verify if there are new callids_done and reduce the sleep
             new_callids_done = callids_done - self.callids_done_processed_status
             if len(new_callids_done) > 0:
-                WAIT_DUR_SEC = 0.5
+                wait_dur_sec = self.monitoring_interval / 5
 
             # generate tokens and mark futures as running/done
             self._generate_tokens(callids_running, callids_done)
             self._tag_future_as_running(callids_running)
             self._tag_future_as_ready(callids_done)
             prevoius_log, log_time = self._print_status_log(prevoius_log, log_time)
 
@@ -458,44 +458,46 @@
 
 
 class JobMonitor:
 
     def __init__(self, executor_id, internal_storage, config=None):
         self.executor_id = executor_id
         self.internal_storage = internal_storage
+        self.storage_config = internal_storage.get_storage_config()
+        self.storage_backend = internal_storage.backend
         self.config = config
-        self.backend = self.config['lithops']['monitoring'].lower() if config else 'storage'
+        self.type = self.config['lithops']['monitoring'].lower() if config else 'storage'
+
         self.token_bucket_q = queue.Queue()
         self.monitor = None
         self.job_chunksize = {}
 
         self.MonitorClass = getattr(
             lithops.monitor,
-            f'{self.backend.capitalize()}Monitor'
+            f'{self.type.capitalize()}Monitor'
         )
 
     def start(self, fs, job_id=None, chunksize=None, generate_tokens=False):
-        if self.backend == 'storage':
-            mi = self.config['lithops'].get('monitoring_interval', MONITORING_INTERVAL) \
-                if self.config else MONITORING_INTERVAL
-            bk_config = {'monitoring_interval': mi}
+        if self.type == 'storage':
+            monitoring_interval = self.storage_config['monitoring_interval']
+            monitor_config = {'monitoring_interval': monitoring_interval}
         else:
-            bk_config = self.config.get(self.backend)
+            monitor_config = self.config.get(self.type)
 
         if job_id:
             self.job_chunksize[job_id] = chunksize
 
         if not self.monitor or not self.monitor.is_alive():
             self.monitor = self.MonitorClass(
                 executor_id=self.executor_id,
                 internal_storage=self.internal_storage,
                 token_bucket_q=self.token_bucket_q,
                 job_chunksize=self.job_chunksize,
                 generate_tokens=generate_tokens,
-                config=bk_config
+                config=monitor_config
             )
 
         self.monitor.add_futures(fs)
 
         if not self.monitor.is_alive():
             self.monitor.start()
```

### Comparing `lithops-3.3.0/lithops/multiprocessing/__init__.py` & `lithops-3.4.0/lithops/multiprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/config.py` & `lithops-3.4.0/lithops/multiprocessing/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/connection.py` & `lithops-3.4.0/lithops/multiprocessing/connection.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/context.py` & `lithops-3.4.0/lithops/multiprocessing/context.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/managers.py` & `lithops-3.4.0/lithops/multiprocessing/managers.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/pool.py` & `lithops-3.4.0/lithops/multiprocessing/pool.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/queues.py` & `lithops-3.4.0/lithops/multiprocessing/queues.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/sharedctypes.py` & `lithops-3.4.0/lithops/multiprocessing/sharedctypes.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/synchronize.py` & `lithops-3.4.0/lithops/multiprocessing/synchronize.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/multiprocessing/util.py` & `lithops-3.4.0/lithops/multiprocessing/util.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/plots.py` & `lithops-3.4.0/lithops/plots.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/retries.py` & `lithops-3.4.0/lithops/retries.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/scripts/cleaner.py` & `lithops-3.4.0/lithops/scripts/cleaner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/scripts/cli.py` & `lithops-3.4.0/lithops/scripts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,33 +524,34 @@
     runtime_meta['runtime_timeout'] = runtime_timeout
     internal_storage.put_runtime_meta(runtime_key, runtime_meta)
 
     logger.info('Runtime deployed')
 
 
 @runtime.command('list')
+@click.argument('name', default='all', required=False)
 @click.option('--config', '-c', default=None, help='path to yaml config file', type=click.Path(exists=True))
 @click.option('--backend', '-b', default=None, help='compute backend')
 @click.option('--storage', '-s', default=None, help='storage backend')
 @click.option('--debug', '-d', is_flag=True, help='debug mode')
-def list_runtimes(config, backend, storage, debug):
+def list_runtimes(name, config, backend, storage, debug):
     """ list all deployed serverless runtime. """
     log_level = logging.INFO if not debug else logging.DEBUG
     setup_lithops_logger(log_level)
 
     config = load_yaml_config(config) if config else None
     config_ow = set_config_ow(backend=backend)
     config = default_config(config_data=config, config_overwrite=config_ow, load_storage_config=False)
 
     if config['lithops']['mode'] != SERVERLESS:
         raise Exception('"lithops runtime list" command is only available for serverless backends')
 
     compute_config = extract_serverless_config(config)
     compute_handler = ServerlessHandler(compute_config, None)
-    runtimes = compute_handler.list_runtimes()
+    runtimes = compute_handler.list_runtimes(runtime_name=name)
 
     headers = ['Runtime Name', 'Memory Size', 'Lithops Version', 'Worker Name']
 
     print()
     print(tabulate(runtimes, headers=headers))
     print(f'\nTotal runtimes: {len(runtimes)}')
```

### Comparing `lithops-3.3.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py` & `lithops-3.4.0/lithops/serverless/backends/aliyun_fc/aliyun_fc.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/aliyun_fc/config.py` & `lithops-3.4.0/lithops/serverless/backends/aliyun_fc/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/aliyun_fc/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/aliyun_fc/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/aws_batch/aws_batch.py` & `lithops-3.4.0/lithops/serverless/backends/aws_batch/aws_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,27 +140,20 @@
                 compute_resources_spec['allocationStrategy'] = 'SPOT_CAPACITY_OPTIMIZED'
 
             if self.env_type in {'EC2', 'SPOT'}:
                 compute_resources_spec['instanceRole'] = self.aws_batch_config['instance_role']
                 compute_resources_spec['minvCpus'] = 0
                 compute_resources_spec['instanceTypes'] = ['optimal']
 
-            if 'service_role' in self.aws_batch_config:
-                res = self.batch_client.create_compute_environment(
-                    computeEnvironmentName=self._compute_env_name,
-                    type='MANAGED',
-                    computeResources=compute_resources_spec,
-                    serviceRole=self.aws_batch_config['service_role']
-                )
-            else:
-                res = self.batch_client.create_compute_environment(
-                    computeEnvironmentName=self._compute_env_name,
-                    type='MANAGED',
-                    computeResources=compute_resources_spec,
-                )
+            res = self.batch_client.create_compute_environment(
+                computeEnvironmentName=self._compute_env_name,
+                type='MANAGED',
+                computeResources=compute_resources_spec,
+                serviceRole=self.aws_batch_config.get('service_role', "")
+            )
 
             if res['ResponseMetadata']['HTTPStatusCode'] != 200:
                 raise Exception(res)
 
             created = False
             while not created:
                 compute_env = self._get_compute_env(self._compute_env_name)
@@ -272,18 +265,19 @@
         if job_def is None:
             logger.debug(f'Creating new Job Definition {job_def_name}')
             image_name, _, _ = self._get_full_image_name(runtime_name)
 
             container_properties = {
                 'image': image_name,
                 'executionRoleArn': self.aws_batch_config['execution_role'],
+                'jobRoleArn': self.aws_batch_config['job_role'],
                 'resourceRequirements': [
                     {
                         'type': 'VCPU',
-                        'value': str(self.aws_batch_config['container_vcpus'])
+                        'value': str(self.aws_batch_config['runtime_cpu'])
                     },
                     {
                         'type': 'MEMORY',
                         'value': str(self.aws_batch_config['runtime_memory'])
                     }
                 ],
             }
```

### Comparing `lithops-3.3.0/lithops/serverless/backends/aws_batch/config.py` & `lithops-3.4.0/lithops/serverless/backends/aws_lambda/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright Cloudlab URV 2021
+# Copyright Cloudlab URV 2020
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,121 +15,124 @@
 #
 
 import copy
 import logging
 
 logger = logging.getLogger(__name__)
 
-ENV_TYPES = {'EC2', 'SPOT', 'FARGATE', 'FARGATE_SPOT'}
-RUNTIME_ZIP = 'lithops_aws_batch.zip'
+DEFAULT_REQUIREMENTS = [
+    'numpy',
+    'requests',
+    'redis',
+    'pika',
+    'cloudpickle',
+    'ps-mem',
+    'tblib',
+    'urllib3<2',
+    'psutil'
+]
+
+AVAILABLE_PY_RUNTIMES = {
+    '3.6': 'python3.6',
+    '3.7': 'python3.7',
+    '3.8': 'python3.8',
+    '3.9': 'python3.9',
+    '3.10': 'python3.10',
+    '3.11': 'python3.11',
+    '3.12': 'python3.12'
+}
 
-AVAILABLE_MEM_FARGATE = [512] + [1024 * i for i in range(1, 31)]
-AVAILABLE_CPU_FARGATE = [0.25, 0.5, 1, 2, 4]
+USER_RUNTIME_PREFIX = 'lithops.user_runtimes'
 
 DEFAULT_CONFIG_KEYS = {
     'runtime_timeout': 180,  # Default: 180 seconds => 3 minutes
-    'runtime_memory': 1024,  # Default memory: 1GB
+    'runtime_memory': 256,  # Default memory: 256 MB
+    'max_workers': 1000,
     'worker_processes': 1,
-    'container_vcpus': 0.5,
-    'env_max_cpus': 10,
-    'env_type': 'FARGATE_SPOT',
-    'assign_public_ip': True,
-    'subnets': []
+    'invoke_pool_threads': 64,
+    'architecture': 'x86_64',
+    'ephemeral_storage': 512,
+    'env_vars': {},
+    'vpc': {'subnets': [], 'security_groups': []},
+    'efs': []
 }
 
-RUNTIME_TIMEOUT_MAX = 7200  # Max. timeout: 7200s == 2h
-RUNTIME_MEMORY_MAX = 30720  # Max. memory: 30720 MB
-
-REQ_PARAMS = ('execution_role', 'instance_role', 'security_groups')
+REQ_PARAMS = ('execution_role',)
 
-DOCKERFILE_DEFAULT = """
-RUN apt-get update && apt-get install -y \
-        zip \
-        && rm -rf /var/lib/apt/lists/*
-
-RUN pip install --upgrade --ignore-installed setuptools six pip \
-    && pip install --upgrade --no-cache-dir --ignore-installed \
-        boto3 \
-        pika \
-        glob2 \
-        redis \
-        requests \
-        PyYAML \
-        kubernetes \
-        numpy \
-        cloudpickle \
-        ps-mem \
-        tblib
-
-# Copy Lithops proxy and lib to the container image.
-ENV APP_HOME /lithops
-WORKDIR $APP_HOME
+RUNTIME_TIMEOUT_MAX = 900  # Max. timeout: 900 s == 15 min
+RUNTIME_MEMORY_MIN = 128  # Max. memory: 128 MB
+RUNTIME_MEMORY_MAX = 10240  # Max. memory: 10240 MB
 
-COPY lithops_aws_batch.zip .
-RUN unzip lithops_aws_batch.zip && rm lithops_aws_batch.zip
-
-ENTRYPOINT python entry_point.py
-"""
+RUNTIME_TMP_SZ_MIN = 512
+RUNTIME_TMP_SZ_MAX = 10240
 
 
 def load_config(config_data):
 
-    if not config_data['aws_batch']:
-        raise Exception("'aws_batch' section is mandatory in the configuration")
+    if not config_data['aws_lambda']:
+        raise Exception("'aws_lambda' section is mandatory in the configuration")
 
     if 'aws' not in config_data:
         config_data['aws'] = {}
 
-    temp = copy.deepcopy(config_data['aws_batch'])
-    config_data['aws_batch'].update(config_data['aws'])
-    config_data['aws_batch'].update(temp)
+    temp = copy.deepcopy(config_data['aws_lambda'])
+    config_data['aws_lambda'].update(config_data['aws'])
+    config_data['aws_lambda'].update(temp)
 
     for param in REQ_PARAMS:
-        if param not in config_data['aws_batch']:
-            msg = f'"{param}" is mandatory in the "aws_batch" section of the configuration'
+        if param not in config_data['aws_lambda']:
+            msg = f'"{param}" is mandatory in the "aws_lambda" section of the configuration'
             raise Exception(msg)
 
     for key in DEFAULT_CONFIG_KEYS:
-        if key not in config_data['aws_batch']:
-            config_data['aws_batch'][key] = DEFAULT_CONFIG_KEYS[key]
+        if key not in config_data['aws_lambda']:
+            config_data['aws_lambda'][key] = DEFAULT_CONFIG_KEYS[key]
 
-    if config_data['aws_batch']['runtime_memory'] > RUNTIME_MEMORY_MAX:
+    if config_data['aws_lambda']['runtime_memory'] > RUNTIME_MEMORY_MAX:
         logger.warning("Memory set to {} - {} exceeds "
-                       "the maximum amount".format(RUNTIME_MEMORY_MAX, config_data['aws_batch']['runtime_memory']))
-        config_data['aws_batch']['runtime_memory'] = RUNTIME_MEMORY_MAX
+                       "the maximum amount".format(RUNTIME_MEMORY_MAX, config_data['aws_lambda']['runtime_memory']))
+        config_data['aws_lambda']['runtime_memory'] = RUNTIME_MEMORY_MAX
+
+    if config_data['aws_lambda']['runtime_memory'] < RUNTIME_MEMORY_MIN:
+        logger.warning("Memory set to {} - {} is lower than "
+                       "the minimum amount".format(RUNTIME_MEMORY_MIN, config_data['aws_lambda']['runtime_memory']))
+        config_data['aws_lambda']['runtime_memory'] = RUNTIME_MEMORY_MIN
 
-    if config_data['aws_batch']['runtime_timeout'] > RUNTIME_TIMEOUT_MAX:
+    if config_data['aws_lambda']['runtime_timeout'] > RUNTIME_TIMEOUT_MAX:
         logger.warning("Timeout set to {} - {} exceeds the "
-                       "maximum amount".format(RUNTIME_TIMEOUT_MAX, config_data['aws_batch']['runtime_timeout']))
-        config_data['aws_batch']['runtime_timeout'] = RUNTIME_TIMEOUT_MAX
+                       "maximum amount".format(RUNTIME_TIMEOUT_MAX, config_data['aws_lambda']['runtime_timeout']))
+        config_data['aws_lambda']['runtime_timeout'] = RUNTIME_TIMEOUT_MAX
+
+    if not {'subnets', 'security_groups'}.issubset(set(config_data['aws_lambda']['vpc'])):
+        raise Exception("'subnets' and 'security_groups' are mandatory sections under 'aws_lambda/vpc'")
+
+    if not isinstance(config_data['aws_lambda']['vpc']['subnets'], list):
+        raise Exception("Unknown type {} for 'aws_lambda/"
+                        "vpc/subnet' section".format(type(config_data['aws_lambda']['vpc']['subnets'])))
+
+    if not isinstance(config_data['aws_lambda']['vpc']['security_groups'], list):
+        raise Exception("Unknown type {} for 'aws_lambda/"
+                        "vpc/security_groups' section".format(type(config_data['aws_lambda']['vpc']['security_groups'])))
+
+    if not isinstance(config_data['aws_lambda']['efs'], list):
+        raise Exception("Unknown type {} for "
+                        "'aws_lambda/efs' section".format(type(config_data['aws_lambda']['vpc']['security_groups'])))
 
-    config_data['aws_batch']['max_workers'] = config_data['aws_batch']['env_max_cpus'] // config_data['aws_batch']['container_vcpus']
+    if not all(
+            ['access_point' in efs_conf and 'mount_path' in efs_conf for efs_conf in config_data['aws_lambda']['efs']]):
+        raise Exception("List of 'access_point' and 'mount_path' mandatory in 'aws_lambda/efs section'")
 
-    if config_data['aws_batch']['env_type'] not in ENV_TYPES:
-        raise Exception(
-            'AWS Batch env type must be one of {} (is {})'.format(ENV_TYPES, config_data['aws_batch']['env_type']))
-
-    if config_data['aws_batch']['env_type'] in {'FARGATE, FARGATE_SPOT'}:
-        if config_data['aws_batch']['container_vcpus'] not in AVAILABLE_CPU_FARGATE:
-            raise Exception('{} container vcpus is not available for {} environment (choose one of {})'.format(
-                config_data['aws_batch']['runtime_memory'], config_data['aws_batch']['env_type'],
-                AVAILABLE_CPU_FARGATE
-            ))
-        if config_data['aws_batch']['runtime_memory'] not in AVAILABLE_MEM_FARGATE:
-            raise Exception('{} runtime memory is not available for {} environment (choose one of {})'.format(
-                config_data['aws_batch']['runtime_memory'], config_data['aws_batch']['env_type'],
-                AVAILABLE_MEM_FARGATE
-            ))
-
-    if config_data['aws_batch']['env_type'] in {'EC2', 'SPOT'}:
-        if 'instance_role' not in config_data['aws_batch']:
-            raise Exception("'instance_role' mandatory for EC2 or SPOT environments")
+    if not all([efs_conf['mount_path'].startswith('/mnt') for efs_conf in config_data['aws_lambda']['efs']]):
+        raise Exception("All mount paths must start with '/mnt' on 'aws_lambda/efs/*/mount_path' section")
 
-    assert isinstance(config_data['aws_batch']['assign_public_ip'], bool)
+    # Lambda runtime config
+    if config_data['aws_lambda']['ephemeral_storage'] < RUNTIME_TMP_SZ_MIN \
+            or config_data['aws_lambda']['ephemeral_storage'] > RUNTIME_TMP_SZ_MAX:
+        raise Exception(f'Ephemeral storage value must be between {RUNTIME_TMP_SZ_MIN} and {RUNTIME_TMP_SZ_MAX}')
 
-    if 'region_name' in config_data['aws_batch']:
-        config_data['aws_batch']['region'] = config_data['aws_batch'].pop('region_name')
+    if 'region_name' in config_data['aws_lambda']:
+        config_data['aws_lambda']['region'] = config_data['aws_lambda'].pop('region_name')
 
-    if 'region' not in config_data['aws_batch']:
-        raise Exception('"region" is mandatory under the "aws_batch" or "aws" section of the configuration')
+    if 'region' not in config_data['aws_lambda']:
+        raise Exception('"region" is mandatory under the "aws_lambda" or "aws" section of the configuration')
     elif 'region' not in config_data['aws']:
-        config_data['aws']['region'] = config_data['aws_batch']['region']
+        config_data['aws']['region'] = config_data['aws_lambda']['region']
```

### Comparing `lithops-3.3.0/lithops/serverless/backends/aws_batch/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/aws_batch/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/aws_lambda/aws_lambda.py` & `lithops-3.4.0/lithops/serverless/backends/aws_lambda/aws_lambda.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,15 @@
         response = self.lambda_client.list_functions(FunctionVersion='ALL')
         get_runtimes(response)
         while 'NextMarker' in response:
             response = self.lambda_client.list_functions(Marker=response['NextMarker'])
             get_runtimes(response)
 
         if runtime_name != 'all':
-            runtimes = [tup for tup in runtimes if runtime_name in tup[0]]
+            runtimes = [tup for tup in runtimes if runtime_name == tup[0]]
 
         return runtimes
 
     def invoke(self, runtime_name, runtime_memory, payload):
         """
         Invoke lambda function asynchronously
         @param runtime_name: name of the runtime
```

### Comparing `lithops-3.3.0/lithops/serverless/backends/aws_lambda/build_layer.py` & `lithops-3.4.0/lithops/serverless/backends/aws_lambda/build_layer.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/aws_lambda/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/aws_lambda/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/azure_containers/azure_containers.py` & `lithops-3.4.0/lithops/serverless/backends/azure_containers/azure_containers.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/azure_containers/config.py` & `lithops-3.4.0/lithops/serverless/backends/azure_containers/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/azure_containers/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/azure_containers/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/azure_functions/azure_functions.py` & `lithops-3.4.0/lithops/serverless/backends/azure_functions/azure_functions.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/azure_functions/config.py` & `lithops-3.4.0/lithops/serverless/backends/azure_functions/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/azure_functions/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/azure_functions/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/code_engine/code_engine.py` & `lithops-3.4.0/lithops/serverless/backends/code_engine/code_engine.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/code_engine/config.py` & `lithops-3.4.0/lithops/serverless/backends/code_engine/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/code_engine/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/code_engine/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py` & `lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/cloudrun.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/config.py` & `lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/gcp_cloudrun/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/gcp_functions/config.py` & `lithops-3.4.0/lithops/serverless/backends/gcp_functions/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/gcp_functions/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/gcp_functions/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/gcp_functions/gcp_functions.py` & `lithops-3.4.0/lithops/serverless/backends/gcp_functions/gcp_functions.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/ibm_cf/config.py` & `lithops-3.4.0/lithops/serverless/backends/ibm_cf/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/ibm_cf/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/ibm_cf/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/ibm_cf/ibm_cf.py` & `lithops-3.4.0/lithops/serverless/backends/ibm_cf/ibm_cf.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/k8s/config.py` & `lithops-3.4.0/lithops/serverless/backends/k8s/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/k8s/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/k8s/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/k8s/k8s.py` & `lithops-3.4.0/lithops/serverless/backends/k8s/k8s.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/knative/config.py` & `lithops-3.4.0/lithops/serverless/backends/knative/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/knative/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/knative/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/knative/knative.py` & `lithops-3.4.0/lithops/serverless/backends/knative/knative.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/openwhisk/config.py` & `lithops-3.4.0/lithops/serverless/backends/openwhisk/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/openwhisk/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/openwhisk/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/openwhisk/openwhisk.py` & `lithops-3.4.0/lithops/serverless/backends/openwhisk/openwhisk.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/oracle_f/config.py` & `lithops-3.4.0/lithops/serverless/backends/oracle_f/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/oracle_f/entry_point.py` & `lithops-3.4.0/lithops/serverless/backends/oracle_f/entry_point.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/backends/oracle_f/oracle_f.py` & `lithops-3.4.0/lithops/serverless/backends/oracle_f/oracle_f.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/serverless/serverless.py` & `lithops-3.4.0/lithops/serverless/serverless.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/backends/aws_ec2/aws_ec2.py` & `lithops-3.4.0/lithops/standalone/backends/aws_ec2/aws_ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,15 +583,15 @@
                 'mode': self.mode,
                 'vpc_data_type': self.vpc_data_type,
                 'ssh_data_type': self.ssh_data_type,
                 'master_name': self.master.name,
                 'master_id': self.vpc_key,
                 'vpc_name': self.vpc_name,
                 'vpc_id': self.config['vpc_id'],
-                'iam_role': self.config['iam_role'],
+                'instance_role': self.config['instance_role'],
                 'target_ami': self.config['target_ami'],
                 'ssh_key_name': self.config['ssh_key_name'],
                 'ssh_key_filename': self.config['ssh_key_filename'],
                 'public_subnet_id': self.config['public_subnet_id'],
                 # 'private_subnet_id': self.config['private_subnet_id'],
                 'security_group_id': self.config['security_group_id'],
                 'internet_gateway_id': self.config['internet_gateway_id'],
@@ -1170,15 +1170,15 @@
         else:
             BlockDeviceMappings = None
 
         LaunchSpecification = {
             "ImageId": self.config['target_ami'],
             "InstanceType": self.instance_type,
             "EbsOptimized": False,
-            "IamInstanceProfile": {'Name': self.config['iam_role']},
+            "IamInstanceProfile": {'Name': self.config['instance_role']},
             "Monitoring": {'Enabled': False},
             'KeyName': self.config['ssh_key_name']
         }
 
         LaunchSpecification['NetworkInterfaces'] = [{
             'AssociatePublicIpAddress': True,
             'DeviceIndex': 0,
```

### Comparing `lithops-3.3.0/lithops/standalone/backends/aws_ec2/config.py` & `lithops-3.4.0/lithops/standalone/backends/aws_ec2/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'request_spot_instances': True,
     'delete_on_dismantle': True,
     'max_workers': 100,
     'worker_processes': 'AUTO'
 }
 
 REQ_PARAMS_1 = ('instance_id',)
-REQ_PARAMS_2 = ('iam_role',)
+REQ_PARAMS_2 = ('instance_role',)
 
 
 def load_config(config_data):
 
     if not config_data['aws_ec2']:
         raise Exception("'aws_ec2' section is mandatory in the configuration")
 
@@ -62,14 +62,18 @@
 
     if config_data['standalone']['exec_mode'] == 'consume':
         params_to_check = REQ_PARAMS_1
         config_data['aws_ec2']['max_workers'] = 1
     else:
         params_to_check = REQ_PARAMS_2
 
+    # iam_role is deprectaded. To be removed in a future release
+    if 'iam_role' in config_data['aws_ec2']:
+        config_data['aws_ec2']['instance_role'] = config_data['aws_ec2'].pop('iam_role')
+
     for param in params_to_check:
         if param not in config_data['aws_ec2']:
             msg = f"'{param}' is mandatory in the 'aws_ec2' section of the configuration"
             raise Exception(msg)
 
     if 'region_name' in config_data['aws_ec2']:
         config_data['aws_ec2']['region'] = config_data['aws_ec2'].pop('region_name')
```

### Comparing `lithops-3.3.0/lithops/standalone/backends/azure_vms/azure_vms.py` & `lithops-3.4.0/lithops/standalone/backends/azure_vms/azure_vms.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/backends/azure_vms/config.py` & `lithops-3.4.0/lithops/standalone/backends/azure_vms/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/backends/ibm_vpc/config.py` & `lithops-3.4.0/lithops/standalone/backends/ibm_vpc/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py` & `lithops-3.4.0/lithops/standalone/backends/ibm_vpc/ibm_vpc.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/backends/vm/config.py` & `lithops-3.4.0/lithops/standalone/backends/vm/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/backends/vm/vm.py` & `lithops-3.4.0/lithops/standalone/backends/vm/vm.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/keeper.py` & `lithops-3.4.0/lithops/standalone/keeper.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/master.py` & `lithops-3.4.0/lithops/standalone/master.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/runner.py` & `lithops-3.4.0/lithops/standalone/runner.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/standalone.py` & `lithops-3.4.0/lithops/standalone/standalone.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/utils.py` & `lithops-3.4.0/lithops/standalone/utils.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/standalone/worker.py` & `lithops-3.4.0/lithops/standalone/worker.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py` & `lithops-3.4.0/lithops/storage/backends/aliyun_oss/aliyun_oss.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/aliyun_oss/config.py` & `lithops-3.4.0/lithops/storage/backends/aliyun_oss/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/aws_s3/aws_s3.py` & `lithops-3.4.0/lithops/storage/backends/aws_s3/aws_s3.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/aws_s3/config.py` & `lithops-3.4.0/lithops/storage/backends/aws_s3/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/azure_storage/azure_storage.py` & `lithops-3.4.0/lithops/storage/backends/azure_storage/azure_storage.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/azure_storage/config.py` & `lithops-3.4.0/lithops/storage/backends/azure_storage/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/ceph/ceph.py` & `lithops-3.4.0/lithops/storage/backends/ceph/ceph.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         client_config = botocore.client.Config(
             max_pool_connections=128,
             user_agent_extra=user_agent,
             connect_timeout=CONN_READ_TIMEOUT,
             read_timeout=CONN_READ_TIMEOUT,
             retries={'max_attempts': OBJ_REQ_RETRIES}
         )
+        if 'region' in ceph_config:
+            client_config.region_name = ceph_config['region']
 
         self.s3_client = boto3.client(
             's3', aws_access_key_id=ceph_config['access_key_id'],
             aws_secret_access_key=ceph_config['secret_access_key'],
             aws_session_token=ceph_config.get('session_token'),
             config=client_config,
             endpoint_url=self.service_endpoint
```

### Comparing `lithops-3.3.0/lithops/storage/backends/ceph/config.py` & `lithops-3.4.0/lithops/storage/backends/ceph/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/gcp_storage/config.py` & `lithops-3.4.0/lithops/storage/backends/gcp_storage/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/gcp_storage/gcp_storage.py` & `lithops-3.4.0/lithops/storage/backends/gcp_storage/gcp_storage.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/ibm_cos/config.py` & `lithops-3.4.0/lithops/storage/backends/ibm_cos/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/ibm_cos/ibm_cos.py` & `lithops-3.4.0/lithops/storage/backends/ibm_cos/ibm_cos.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/infinispan/config.py` & `lithops-3.4.0/lithops/storage/backends/infinispan/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/infinispan/infinispan.py` & `lithops-3.4.0/lithops/storage/backends/infinispan/infinispan.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/config.py` & `lithops-3.4.0/lithops/storage/backends/infinispan_hotrod/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py` & `lithops-3.4.0/lithops/storage/backends/infinispan_hotrod/infinispan_hotrod.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/localhost/config.py` & `lithops-3.4.0/lithops/storage/backends/localhost/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 #
 
 
 def load_config(config_data):
     if 'localhost' not in config_data or config_data['localhost'] is None:
         config_data['localhost'] = {}
 
+    if 'monitoring_interval' not in config_data['lithops']:
+        config_data['lithops']['monitoring_interval'] = 0.1
+
     config_data['localhost']['storage_bucket'] = 'storage'
```

### Comparing `lithops-3.3.0/lithops/storage/backends/localhost/localhost.py` & `lithops-3.4.0/lithops/storage/backends/localhost/localhost.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/minio/config.py` & `lithops-3.4.0/lithops/storage/backends/minio/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/minio/minio.py` & `lithops-3.4.0/lithops/storage/backends/minio/minio.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/oracle_oss/config.py` & `lithops-3.4.0/lithops/storage/backends/oracle_oss/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/oracle_oss/oracle_oss.py` & `lithops-3.4.0/lithops/storage/backends/oracle_oss/oracle_oss.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/redis/config.py` & `lithops-3.4.0/lithops/storage/backends/redis/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/redis/redis.py` & `lithops-3.4.0/lithops/storage/backends/redis/redis.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/backends/swift/config.py` & `lithops-3.4.0/lithops/storage/backends/swift/config.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/cloud_proxy.py` & `lithops-3.4.0/lithops/storage/cloud_proxy.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/storage/storage.py` & `lithops-3.4.0/lithops/storage/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 RUNTIME_META_CACHE = {}
 COBJECTS_INDEX = itertools.count()
 
 
 class Storage:
     """
     An Storage object is used by partitioner and other components to access
-    underlying storage backend without exposing the the implementation details.
+    underlying storage backend without exposing the implementation details.
     """
 
     def __init__(self, config=None, backend=None, storage_config=None):
         """ Creates an Storage instance
 
         :param config: lithops configuration dict
         :param backend: storage backend name
```

### Comparing `lithops-3.3.0/lithops/storage/utils.py` & `lithops-3.4.0/lithops/storage/utils.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/tests/conftest.py` & `lithops-3.4.0/lithops/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,31 +21,27 @@
 @pytest.fixture(scope="session", autouse=True)
 def setup_global(request):
     config = request.config
     config_file = config.getoption("--config")
     backend = config.getoption("--backend")
     storage = config.getoption("--storage")
     region = config.getoption("--region")
-    debug = config.getoption("--debug")
 
     config_data = None
 
     if config_file:
         if os.path.exists(config_file):
             config_data = load_yaml_config(config_file)
         else:
             raise FileNotFoundError(f"The provided config file '{config_file}' does not exist")
 
     config_ow = {'lithops': {}, 'backend': {}}
+    config_ow['lithops']['log_level'] = 'DEBUG'
     if storage:
         config_ow['lithops']['storage'] = storage
-        if storage == 'localhost':
-            config_ow['lithops']['monitoring_interval'] = 0.1
     if backend:
         config_ow['lithops']['backend'] = backend
-    if debug:
-        config_ow['lithops']['log_level'] = 'DEBUG'
     if region:
         config_ow['backend']['region'] = region
 
     lithops_config = default_config(config_data=config_data, config_overwrite=config_ow)
     pytest.lithops_config = lithops_config
```

### Comparing `lithops-3.3.0/lithops/tests/functions.py` & `lithops-3.4.0/lithops/tests/functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import lithops
+import time
 import pickle
 
 
 def simple_map_function(x, y):
     return x + y
 
 
@@ -24,32 +25,49 @@
 
 
 def lithops_return_futures_map(x):
     def _func(x):
         return x + 1
 
     fexec = lithops.FunctionExecutor()
-    return fexec.map(_func, range(x))
+    futures = fexec.map(_func, range(x))
+
+    # this while loop is required to pass localhost tests on Windows
+    while not all(f.running or f.ready for f in futures):
+        time.sleep(0.1)
+
+    return futures
 
 
 def lithops_return_futures_call_async(x):
     def _func(x):
         return x + 1
 
     fexec = lithops.FunctionExecutor()
-    return fexec.call_async(_func, x + 5)
+    fut = fexec.call_async(_func, x + 5)
+
+    # this while loop is required to pass localhost tests on Windows
+    while not (fut.running or fut.ready):
+        time.sleep(0.1)
+
+    return fut
 
 
 def lithops_return_futures_map_multiple(x):
     def _func(x):
         return x + 1
 
     fexec = lithops.FunctionExecutor()
     fut1 = fexec.map(_func, range(x))
     fut2 = fexec.map(_func, range(x))
+
+    # this while loop is required to pass localhost tests on Windows
+    while not all(f.running or f.ready for f in fut1 + fut2):
+        time.sleep(0.1)
+
     return fut1 + fut2
 
 
 def my_map_function_obj(obj, id):
     """returns a dictionary of {word:number of appearances} key:value items."""
     print('Function id: {}'.format(id))
     print('Bucket: {}'.format(obj.bucket))
```

### Comparing `lithops-3.3.0/lithops/tests/test_call_async.py` & `lithops-3.4.0/lithops/tests/test_call_async.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/tests/test_map.py` & `lithops-3.4.0/lithops/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/tests/test_map_reduce.py` & `lithops-3.4.0/lithops/tests/test_map_reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,61 +110,65 @@
         logger.info('Testing map_reduce() over URLs')
         fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         fexec.map_reduce(my_map_function_url, TEST_FILES_URLS,
                          my_reduce_function, obj_chunk_number=2)
         result = fexec.get_result()
         assert result == self.words_in_files
 
-    def test_chunks_bucket(self):
+    def test_bucket_chunk_size(self):
         """tests the ability to create a separate function invocation
         based on the following parameters: chunk_size creates [file_size//chunk_size]
-        invocations to process each chunk_size bytes, of a given object. chunk_number
-        creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each.
+        invocations to process each chunk_size bytes, of a given object.
         """
-
-        logger.info('Testing chunks on a bucket')
         OBJ_CHUNK_SIZE = 1 * 800 ** 2  # create a new invocation
-        OBJ_CHUNK_NUMBER = 2
         activations = 0
 
         data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
 
         fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
-        futures = fexec.map_reduce(my_map_function_obj, data_prefix,
-                                   my_reduce_function,
-                                   obj_chunk_size=OBJ_CHUNK_SIZE)
+        futures = fexec.map_reduce(
+            my_map_function_obj, data_prefix,
+            my_reduce_function, obj_chunk_size=OBJ_CHUNK_SIZE
+        )
         result = fexec.get_result(futures)
         assert result == self.words_in_files
 
         for size in get_dataset_key_size(self.storage, self.bucket):
             activations += math.ceil(size / OBJ_CHUNK_SIZE)
 
         assert len(futures) == activations + 1  # +1 due to the reduce function
 
+    def test_bucket_chunk_number(self):
+        """tests the ability to create a separate function invocation
+        based on the following parameters: chunk_number
+        creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each.
+        """
+        OBJ_CHUNK_NUMBER = 2
+
+        data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
+
         fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
-        futures = fexec.map_reduce(my_map_function_obj, data_prefix,
-                                   my_reduce_function, obj_chunk_number=OBJ_CHUNK_NUMBER)
+        futures = fexec.map_reduce(
+            my_map_function_obj, data_prefix,
+            my_reduce_function, obj_chunk_number=OBJ_CHUNK_NUMBER
+        )
         result = fexec.get_result(futures)
         assert result == self.words_in_files
 
         assert len(futures) == len(TEST_FILES_URLS) * OBJ_CHUNK_NUMBER + 1
 
-    def test_chunks_bucket_one_reducer_per_object(self):
+    def test_bucket_chunk_size_one_reducer_per_object(self):
         """tests the ability to create a separate function invocation based
         on the following parameters, as well as create a separate invocation
         of a reduce function for each object: chunk_size creates [file_size//chunk_size]
         invocations to process each chunk_size bytes, of a given object. hunk_number
         creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each.
         """
-
-        logger.info('Testing chunks on a bucket with one reducer per object')
         OBJ_CHUNK_SIZE = 1 * 1024 ** 2
-        OBJ_CHUNK_NUMBER = 2
         activations = 0
-
         data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
 
         fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         futures = fexec.map_reduce(
             my_map_function_obj, data_prefix,
             my_reduce_function,
             obj_chunk_size=OBJ_CHUNK_SIZE,
@@ -175,14 +179,24 @@
 
         for size in get_dataset_key_size(self.storage, self.bucket):
             activations += math.ceil(size / OBJ_CHUNK_SIZE)
 
         # + len(TEST_FILES_URLS) due to map_reduce activation per object
         assert len(futures) == activations + len(TEST_FILES_URLS)
 
+    def test_bucket_chunk_number_one_reducer_per_object(self):
+        """tests the ability to create a separate function invocation based
+        on the following parameters, as well as create a separate invocation
+        of a reduce function for each object: chunk_size creates [file_size//chunk_size]
+        invocations to process each chunk_size bytes, of a given object. hunk_number
+        creates 'chunk_number' invocations that process [file_size//chunk_number] bytes each.
+        """
+        OBJ_CHUNK_NUMBER = 2
+        data_prefix = self.storage_backend + '://' + self.bucket + '/' + DATASET_PREFIX + '/'
+
         fexec = lithops.FunctionExecutor(config=pytest.lithops_config)
         futures = fexec.map_reduce(
             my_map_function_obj,
             data_prefix,
             my_reduce_function,
             obj_chunk_number=OBJ_CHUNK_NUMBER,
             obj_reduce_by_key=True
```

### Comparing `lithops-3.3.0/lithops/tests/test_retries.py` & `lithops-3.4.0/lithops/tests/test_retries.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/tests/test_storage.py` & `lithops-3.4.0/lithops/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/util/ibm_token_manager.py` & `lithops-3.4.0/lithops/util/ibm_token_manager.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/util/joblib/lithops_backend.py` & `lithops-3.4.0/lithops/util/joblib/lithops_backend.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/util/metrics.py` & `lithops-3.4.0/lithops/util/metrics.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/util/ssh_client.py` & `lithops-3.4.0/lithops/util/ssh_client.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/utils.py` & `lithops-3.4.0/lithops/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import shutil
 import base64
 import inspect
 import struct
 import lithops
 import zipfile
 import platform
+import threading
 import logging.config
 import subprocess as sp
 from enum import Enum
 from contextlib import closing
 
 from lithops import constants
 from lithops.version import __version__
@@ -738,8 +739,29 @@
 
 
 class BackendType(Enum):
     BATCH = 'batch'
     FAAS = 'faas'
 
 
+class CountDownLatch:
+    def __init__(self, count):
+        self.count = count
+        self.event = threading.Event()
+        self.lock = threading.Lock()
+
+    def unlock(self):
+        with self.lock:
+            self.count -= 1
+            if self.count == 0:
+                self.event.set()
+
+    def wait(self):
+        if self.count > 0:
+            self.event.wait()
+
+    @property
+    def done(self):
+        return self.count == 0
+
+
 CURRENT_PY_VERSION = version_str(sys.version_info)
```

### Comparing `lithops-3.3.0/lithops/wait.py` & `lithops-3.4.0/lithops/wait.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
          internal_storage: Optional[InternalStorage] = None,
          job_monitor: Optional[JobMonitor] = None,
          throw_except: Optional[bool] = True,
          return_when: Optional[Any] = ALL_COMPLETED,
          download_results: Optional[bool] = False,
          timeout: Optional[int] = None,
          threadpool_size: Optional[int] = THREADPOOL_SIZE,
-         wait_dur_sec: Optional[int] = WAIT_DUR_SEC,
+         wait_dur_sec: Optional[int] = None,
          show_progressbar: Optional[bool] = True,
          futures_from_executor_wait: Optional[bool] = False) -> Tuple[FuturesList, FuturesList]:
     """
     Wait for the Future instances (possibly created by different Executor instances)
     given by fs to complete. Returns a named 2-tuple of sets. The first set, named done,
     contains the futures that completed (finished or cancelled futures) before the wait
     completed. The second set, named not_done, contains the futures that did not complete
@@ -64,15 +64,15 @@
     :param internal_storage: InternalStorage instance. Default None.
     :param job_monitor: JobMonitor instance. Default None.
     :param throw_except: Re-raise exception if call raised. Default True.
     :param return_when: Percentage of done futures
     :param download_results: Download results. Default false (Only get statuses)
     :param timeout: Timeout of waiting for results.
     :param threadpool_size: Number of threads to use. Default 64
-    :param wait_dur_sec: Time interval between each check.
+    :param wait_dur_sec: Time interval between each check. Default 1 second
     :param show_progressbar: whether or not to show the progress bar.
 
     :return: `(fs_done, fs_notdone)`
         where `fs_done` is a list of futures that have completed
         and `fs_notdone` is a list of futures that have not completed.
     :rtype: 2-tuple of list
     """
@@ -109,16 +109,15 @@
         logger.debug(f'Setting waiting timeout to {timeout} seconds')
         error_msg = 'Timeout of {timeout} seconds exceeded waiting for function activations to finish'
         signal.signal(signal.SIGALRM, partial(timeout_handler, error_msg))
         signal.alarm(timeout)
 
     # Setup progress bar
     pbar = None
-    if not is_lithops_worker() and logger.getEffectiveLevel() == logging.INFO \
-       and show_progressbar:
+    if not is_lithops_worker() and show_progressbar and logger.getEffectiveLevel() != logging.DEBUG:
         from tqdm.auto import tqdm
         if not is_notebook():
             print()
         pbar = tqdm(bar_format='  {l_bar}{bar}| {n_fmt}/{total_fmt}  ',
                     total=fs_to_wait, disable=None)
         pbar.update(min(len(fs_done), fs_to_wait))
 
@@ -128,15 +127,16 @@
         if not job_monitor:
             for executor_data in executors_data:
                 job_monitor = JobMonitor(
                     executor_id=executor_data.executor_id,
                     internal_storage=executor_data.internal_storage)
                 job_monitor.start(fs=executor_data.futures)
 
-        sleep_sec = wait_dur_sec if job_monitor.backend == 'storage' else 0.3
+        sleep_sec = wait_dur_sec or WAIT_DUR_SEC if job_monitor.type == 'storage' \
+            and job_monitor.storage_backend != 'localhost' else 0.1
 
         if return_when == ALWAYS:
             for executor_data in executors_data:
                 _get_executor_data(fs, executor_data, pbar=pbar,
                                    throw_except=throw_except,
                                    download_results=download_results,
                                    threadpool_size=threadpool_size)
@@ -183,25 +183,25 @@
 
 
 def get_result(fs: Optional[Union[ResponseFuture, FuturesList, List[ResponseFuture]]] = None,
                internal_storage: Optional[InternalStorage] = None,
                throw_except: Optional[bool] = True,
                timeout: Optional[int] = None,
                threadpool_size: Optional[int] = THREADPOOL_SIZE,
-               wait_dur_sec: Optional[int] = WAIT_DUR_SEC,
+               wait_dur_sec: Optional[int] = None,
                show_progressbar: Optional[bool] = True):
     """
     For getting the results from all function activations
 
     :param fs: Futures list. Default None
     :param internal_storage: InternalStorage instance. Default None.
     :param throw_except: Reraise exception if call raised. Default True.
     :param timeout: Timeout for waiting for results.
     :param threadpool_size: Number of threads to use. Default 128
-    :param wait_dur_sec: Time interval between each check.
+    :param wait_dur_sec: Time interval between each check. Default 1 second
     :param show_progressbar: whether or not to show the progress bar.
 
     :return: The result of the future/s
     """
     if type(fs) is not list and type(fs) is not FuturesList:
         fs = [fs]
```

### Comparing `lithops-3.3.0/lithops/worker/handler.py` & `lithops-3.4.0/lithops/worker/handler.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/worker/invoker.py` & `lithops-3.4.0/lithops/worker/invoker.py`

 * *Files identical despite different names*

### Comparing `lithops-3.3.0/lithops/worker/jobrunner.py` & `lithops-3.4.0/lithops/worker/jobrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import os
 import io
 import sys
+import ast
 import pika
 import time
 import pickle
 import logging
 import inspect
 import requests
 import traceback
@@ -205,15 +206,15 @@
         exception = False
         fn_name = None
 
         try:
             func = pickle.loads(self.job.func)
             data = pickle.loads(self.job.data)
 
-            if eval(os.environ.get('__LITHOPS_REDUCE_JOB', 'False')):
+            if ast.literal_eval(os.environ.get('__LITHOPS_REDUCE_JOB', 'False')):
                 self._wait_futures(data)
             elif is_object_processing_function(func):
                 self._load_object(data)
 
             self._fill_optional_args(func, data)
 
             fn_name = func.__name__ if inspect.isfunction(func) \
```

### Comparing `lithops-3.3.0/lithops/worker/status.py` & `lithops-3.4.0/lithops/worker/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import ast
 import pika
 import json
 import time
 import logging
 from tblib import pickling_support
 from contextlib import contextmanager
 
@@ -40,15 +41,15 @@
             'host_submit_tstamp': job.host_submit_tstamp,
             'call_id': job.call_id,
             'job_id': job.job_id,
             'executor_id': job.executor_id,
             'chunksize': job.chunksize
         }
 
-        if eval(os.environ.get('WARM_CONTAINER', 'False')):
+        if ast.literal_eval(os.environ.get('WARM_CONTAINER', 'False')):
             self.status['worker_cold_start'] = False
         else:
             self.status['worker_cold_start'] = True
             os.environ['WARM_CONTAINER'] = 'True'
 
     def add(self, key, value):
         """ Adds data to the call status"""
```

### Comparing `lithops-3.3.0/lithops/worker/utils.py` & `lithops-3.4.0/lithops/worker/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,31 @@
 def get_function_and_modules(job, internal_storage):
     """
     Gets the function and modules from storage
     """
     logger.info("Getting function and modules")
     backend = job.config['lithops']['backend']
     func_path = '/'.join([LITHOPS_TEMP_DIR, job.func_key])
+    func_obj = None
 
     if job.config[backend].get('runtime_include_function'):
         logger.info("Runtime include function feature activated. Loading "
                     "function/mods from local runtime")
         func_path = '/'.join([SA_INSTALL_DIR, job.func_key])
         with open(func_path, "rb") as f:
             func_obj = f.read()
     elif os.path.exists(func_path):
         logger.info(f"Loading {job.func_key} from local cache")
-        with open(func_path, 'rb') as f:
-            func_obj = f.read()
-    else:
+        try:
+            with open(func_path, 'rb') as f:
+                func_obj = f.read()
+        except Exception:
+            logger.debug(f"Could not load {job.func_key} from local cache")
+
+    if not func_obj:
         logger.info(f"Loading {job.func_key} from storage")
         func_obj = internal_storage.get_func(job.func_key)
         os.makedirs(os.path.dirname(func_path), exist_ok=True)
         with open(func_path, 'wb') as f:
             f.write(func_obj)
 
     loaded_func_all = pickle.loads(func_obj)
```

### Comparing `lithops-3.3.0/lithops.egg-info/PKG-INFO` & `lithops-3.4.0/lithops.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 2.1
 Name: lithops
-Version: 3.3.0
+Version: 3.4.0
 Summary: Lithops lets you transparently run your Python applications in the Cloud
 Home-page: https://github.com/lithops-cloud/lithops
 Author: Gil Vernik, Josep Sampe
 Author-email: gilv@ibm.com, josep.sampe@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.6
 Provides-Extra: aliyun
 Provides-Extra: all
+Provides-Extra: aws
 Provides-Extra: azure
+Provides-Extra: ceph
 Provides-Extra: gcp
+Provides-Extra: ibm
 Provides-Extra: joblib
+Provides-Extra: knative
+Provides-Extra: kubernetes
+Provides-Extra: minio
 Provides-Extra: multiprocessing
 Provides-Extra: oracle
+Provides-Extra: plotting
+Provides-Extra: redis
 Provides-Extra: tests
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `lithops-3.3.0/lithops.egg-info/SOURCES.txt` & `lithops-3.4.0/lithops.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 lithops/libs/inspect/__init__.py
 lithops/libs/inspect/inspect.py
 lithops/libs/multyvac/__init__.py
 lithops/libs/multyvac/module_dependency.py
 lithops/libs/openwhisk/__init__.py
 lithops/libs/openwhisk/client.py
 lithops/localhost/__init__.py
+lithops/localhost/config.py
 lithops/localhost/v1/__init__.py
 lithops/localhost/v1/localhost.py
 lithops/localhost/v1/runner.py
 lithops/localhost/v2/__init__.py
 lithops/localhost/v2/localhost.py
-lithops/localhost/v2/service.py
+lithops/localhost/v2/runner.py
 lithops/multiprocessing/__init__.py
 lithops/multiprocessing/config.py
 lithops/multiprocessing/connection.py
 lithops/multiprocessing/context.py
 lithops/multiprocessing/managers.py
 lithops/multiprocessing/pool.py
 lithops/multiprocessing/process.py
```

### Comparing `lithops-3.3.0/lithops.egg-info/requires.txt` & `lithops-3.4.0/lithops.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 Click
 PyYAML
-boto3
 cloudpickle
-docker
-ibm-code-engine-sdk
-ibm-cos-sdk
-ibm-vpc
-kubernetes
-lxml
-matplotlib
-pandas
 paramiko
 pika
 ps-mem
 psutil
-python-dateutil
-redis
 requests
-seaborn
+six
 tabulate
 tblib
 tblib
 tqdm
 
 [aliyun]
 aliyun-fc2
@@ -31,48 +20,88 @@
 aliyun-fc2
 azure-identity
 azure-mgmt-compute
 azure-mgmt-network
 azure-mgmt-resource
 azure-storage-blob
 azure-storage-queue
+boto3
 diskcache
 google-api-python-client
 google-auth
 google-cloud-pubsub
 google-cloud-storage
 httplib2
+ibm-code-engine-sdk
+ibm-cos-sdk
+ibm-vpc
 joblib
+kubernetes
+matplotlib
 numpy
 oci
 oss2
+pandas
 pynng
 pytest
+redis
+seaborn
+
+[aws]
+boto3
 
 [azure]
 azure-identity
 azure-mgmt-compute
 azure-mgmt-network
 azure-mgmt-resource
 azure-storage-blob
 azure-storage-queue
 
+[ceph]
+boto3
+
 [gcp]
 google-api-python-client
 google-auth
 google-cloud-pubsub
 google-cloud-storage
 httplib2
 
+[ibm]
+ibm-code-engine-sdk
+ibm-cos-sdk
+ibm-vpc
+kubernetes
+
 [joblib]
 diskcache
 joblib
 numpy
 
+[knative]
+kubernetes
+
+[kubernetes]
+kubernetes
+
+[minio]
+boto3
+
 [multiprocessing]
 pynng
+redis
 
 [oracle]
 oci
 
+[plotting]
+matplotlib
+numpy
+pandas
+seaborn
+
+[redis]
+redis
+
 [tests]
 pytest
```

