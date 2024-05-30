# Comparing `tmp/mlflow-skinny-2.9.1.tar.gz` & `tmp/mlflow-skinny-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow-skinny-2.9.1.tar", last modified: Thu Dec  7 05:24:34 2023, max compression
+gzip compressed data, was "mlflow-skinny-2.9.2.tar", last modified: Thu Dec 14 05:33:02 2023, max compression
```

## Comparing `mlflow-skinny-2.9.1.tar` & `mlflow-skinny-2.9.2.tar`

### file list

```diff
@@ -1,597 +1,599 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11382 2023-12-07 05:24:31.000000 mlflow-skinny-2.9.1/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      608 2023-12-07 05:24:31.000000 mlflow-skinny-2.9.1/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11887 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10160 2023-12-07 05:24:31.000000 mlflow-skinny-2.9.1/README.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-12-07 05:24:31.000000 mlflow-skinny-2.9.1/README_SKINNY.rst
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.052430 mlflow-skinny-2.9.1/mlflow/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6711 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/__main__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3891 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/_doctor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6785 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/_promptlab.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10014 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/_spark_autologging.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.052430 mlflow-skinny-2.9.1/mlflow/artifacts/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6443 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/artifacts/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.052430 mlflow-skinny-2.9.1/mlflow/azure/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/azure/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11625 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/azure/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.052430 mlflow-skinny-2.9.1/mlflow/catboost/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13660 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/catboost/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24856 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.052430 mlflow-skinny-2.9.1/mlflow/data/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2487 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6885 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/artifact_dataset_sources.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      946 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/code_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4333 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6342 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/dataset_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3533 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8301 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/dataset_source_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3768 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/delta_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4904 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/digest_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2598 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/filesystem_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4438 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/http_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9868 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/huggingface_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4312 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/huggingface_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8569 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/numpy_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8529 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/pandas_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/pyfunc_dataset_mixin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2677 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/schema.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/sources.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15745 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/spark_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2231 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/spark_dataset_source.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3857 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/spark_delta_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11898 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/data/tensorflow_dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      881 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/db.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/deployments/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15582 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16234 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      968 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/constants.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/deployments/databricks/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14118 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/databricks/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4623 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/interface.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/deployments/mlflow/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10774 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/mlflow/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5498 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/plugin_manager.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/deployments/server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/server/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11785 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/server/app.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/server/config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/server/constants.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2834 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/server/runner.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3334 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/deployments/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/diviner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27853 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/diviner/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/entities/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1294 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1394 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/_mlflow_object.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2118 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/dataset.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1510 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/dataset_input.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1048 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/dataset_summary.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3534 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/experiment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      887 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/experiment_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1215 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/file_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/input_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/lifecycle_stage.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/metric.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/entities/model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      528 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      287 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/_model_registry_entity.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6466 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version_stages.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version_status.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      933 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/registered_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/registered_model_alias.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/model_registry/registered_model_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/multipart_upload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1133 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/param.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2136 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/run.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3089 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/run_data.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6173 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/run_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/run_inputs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1540 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/run_status.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/run_tag.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1202 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/source_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1816 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/entities/view_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20975 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/environment_variables.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5351 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/exceptions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/experiments.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.056430 mlflow-skinny-2.9.1/mlflow/fastai/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25447 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/fastai/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5660 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/fastai/callback.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/gateway/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1019 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/app.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1584 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/base_models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1230 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16541 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16208 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/constants.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       52 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/exceptions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7918 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/fluent.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/gateway/providers/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3641 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/ai21labs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5544 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/anthropic.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10576 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/bedrock.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5381 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/cohere.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5029 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/huggingface.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8549 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/mlflow.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10165 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/mosaicml.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/openai.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7579 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/palm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2520 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/providers/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/gateway/schemas/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/schemas/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/schemas/chat.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1674 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/schemas/completions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2696 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/schemas/embeddings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8369 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gateway/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/gluon/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17541 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gluon/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2020 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/gluon/_autolog.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/h2o/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12848 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/h2o/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/johnsnowlabs/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35978 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/johnsnowlabs/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/keras/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      349 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/keras/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/keras_core/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/keras_core/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3895 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/keras_core/callback.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/langchain/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25248 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/langchain/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9333 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/langchain/api_request_parallel_processor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5297 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/langchain/retriever_chain.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14513 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/langchain/runnables.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17110 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/langchain/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/lightgbm/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37623 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/lightgbm/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/llm/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/llm/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/metrics/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1263 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/base.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/metrics/genai/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16511 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/genai_metric.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14540 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/metric_definitions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6365 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/model_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/prompt_template.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.060430 mlflow-skinny-2.9.1/mlflow/metrics/genai/prompts/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/prompts/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21222 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/prompts/v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/genai/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17279 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/metrics/metric_definitions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5987 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/ml_package_versions.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/mleap/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12909 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/mleap/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3615 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9772 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/cli.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/models/container/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9975 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/container/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/models/container/scoring_server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/container/scoring_server/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/container/scoring_server/wsgi.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9756 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/docker_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/models/evaluation/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3204 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/_shap_patch.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/artifacts.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    83924 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    76234 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/default_evaluator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1991 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/evaluator_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6161 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/lift_curve.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10946 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/evaluation/validation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3421 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/flavor_backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2329 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/flavor_backend_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27560 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18476 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/signature.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47232 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11651 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/models/wheeled_model.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/onnx/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24589 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/onnx/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/openai/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34486 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/openai/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15486 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/openai/api_request_parallel_processor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2936 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/openai/retry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8026 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/openai/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/paddle/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22229 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/paddle/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4862 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/paddle/_paddle_autolog.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/pmdarima/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24099 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pmdarima/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/projects/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17340 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11466 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/_project_spec.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/projects/backend/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      271 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/backend/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2211 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/backend/abstract_backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/backend/loader.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17238 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/backend/local.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20186 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/databricks.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6456 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/docker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/env_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6361 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/kubernetes.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3572 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/submitted_run.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12265 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/projects/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.064430 mlflow-skinny-2.9.1/mlflow/prophet/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/prophet/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/protos/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17261 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/databricks_artifacts_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14095 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/databricks_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52871 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/databricks_uc_registry_messages_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15075 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/databricks_uc_registry_service_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16146 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/facet_feature_statistics_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/internal_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16372 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/mlflow_artifacts_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54475 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/model_registry_pb2.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/protos/scalapb/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/scalapb/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3307 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/scalapb/scalapb_pb2.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53666 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/protos/service_pb2.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/pyfunc/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    95819 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      783 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/_mlflow_pyfunc_backend_predict.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16480 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1284 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/mlserver.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20441 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/model.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/pyfunc/scoring_server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17458 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/scoring_server/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5573 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/scoring_server/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/scoring_server/wsgi.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2124 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/spark_model_cache.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1357 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyfunc/stdin_server.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  8045819 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pypi_package_index.json
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/pyspark/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyspark/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/pyspark/ml/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55609 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyspark/ml/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3035 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyspark/ml/_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1886 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pyspark/ml/log_model_allowlist.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/pytorch/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    43245 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pytorch/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17903 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pytorch/_lightning_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2237 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pytorch/_pytorch_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2068 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/pytorch/pickle_module.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/artifacts.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/cards/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10289 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/cards/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4780 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/cards/histogram_generator.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12527 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/cards/pandas_renderer.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/cards/templates/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/cards/templates/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3488 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/cards/templates/base.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/classification/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/classification/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/classification/v1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      122 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/classification/v1/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/classification/v1/recipe.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2928 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18431 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/dag_help_strings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17976 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/recipe.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/regression/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/regression/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/regression/v1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/regression/v1/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22525 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/regression/v1/recipe.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.068431 mlflow-skinny-2.9.1/mlflow/recipes/resources/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12211 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/resources/recipe_dag_template.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14920 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/step.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/recipes/steps/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/recipes/steps/automl/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/automl/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6256 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/automl/flaml.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20651 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/evaluate.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/recipes/steps/ingest/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11107 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/ingest/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26390 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/ingest/datasets.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12109 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/predict.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7627 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/register.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19478 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/split.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59617 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/train.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10571 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/steps/transform.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/recipes/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6350 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28397 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/utils/execution.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8990 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/utils/metrics.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7738 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/utils/step.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12374 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/utils/tracking.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2453 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/recipes/utils/wrapped_recipe_model.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/rfunc/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1115 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/rfunc/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3631 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/rfunc/backend.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2527 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/runs.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/sagemaker/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   136129 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/sagemaker/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12921 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/sagemaker/cli.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/sentence_transformers/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15872 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/sentence_transformers/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/server/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9179 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/server/auth/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30594 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       87 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/__main__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/basic_auth.ini
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      144 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18725 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/config.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/server/auth/db/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      373 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/cli.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3335 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/alembic.ini
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2114 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/env.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/versions/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/versions/8606fa83a998_initial_migration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/versions/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2307 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1408 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/db/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4217 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/entities.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2673 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/logo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/permissions.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1110 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/routes.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10562 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/auth/sqlalchemy_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    80176 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/handlers.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/prometheus_exporter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1116 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/server/validation.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.072430 mlflow-skinny-2.9.1/mlflow/shap/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26545 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/shap/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/sklearn/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    85281 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/sklearn/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37444 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/sklearn/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/spacy/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13880 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/spacy/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/spark/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49863 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/spark/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/statsmodels/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23362 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/statsmodels/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/store/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      227 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33780 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/registry/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7167 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/registry/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/store/artifact/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13427 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6080 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/artifact_repository_registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/azure_blob_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10194 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/azure_data_lake_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5384 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/cli.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10970 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/cloud_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26274 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/databricks_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9668 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/databricks_models_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10152 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/dbfs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5233 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/ftp_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10879 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/gcs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10019 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/hdfs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9000 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/http_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5101 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/local_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3001 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/mlflow_artifacts_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8490 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/models_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11535 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/optimized_s3_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/r2_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6010 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/runs_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12310 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/s3_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5454 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/sftp_artifact_repo.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5743 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/store/artifact/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3924 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/artifact/utils/models.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/store/db/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db/base_sql_model.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db/db_types.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10769 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.076431 mlflow-skinny-2.9.1/mlflow/store/db_migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1634 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/alembic.ini
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2768 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/env.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      924 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2624 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      779 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/2d6e25af4d3e_increase_max_param_val_length.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      940 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1014 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      476 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5716 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1666 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      593 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/acf3f17fdcc7_add_storage_location_field_to_model_.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2830 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/store/entities/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/entities/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/entities/paged_list.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/store/model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      605 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15238 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/abstract_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1440 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/base_rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/databricks_workspace_model_registry_rest_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/store/model_registry/dbmodels/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/dbmodels/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6352 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/dbmodels/models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    41195 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/file_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17006 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50803 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/model_registry/sqlalchemy_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/store/tracking/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1154 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15989 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/abstract_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/store/tracking/dbmodels/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/dbmodels/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8248 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/dbmodels/initial_models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20980 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/dbmodels/models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55188 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/file_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12804 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/rest_store.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    78876 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/store/tracking/sqlalchemy_store.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/system_metrics/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1788 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.080431 mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      805 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/base_metrics_monitor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      776 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/cpu_monitor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      689 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/disk_monitor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1877 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/gpu_monitor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1352 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/network_monitor.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/system_metrics/system_metrics_monitor.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tensorflow/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    60226 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tensorflow/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8493 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tensorflow/_autolog.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3807 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tensorflow/callback.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tracking/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15645 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13101 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/fluent.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3152 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7493 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28028 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2335 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8776 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7540 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/artifact_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   150565 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tracking/context/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/abstract_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_cluster_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_command_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_job_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1713 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_notebook_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1952 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_repo_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1128 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/default_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/git_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      467 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/context/system_environment_context.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       28 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1704 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/abstract_context.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2998 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/registry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    84156 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/fluent.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3489 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/llm_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2244 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/metric_value_conversion_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3516 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/registry.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tracking/request_auth/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_auth/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1051 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_auth/abstract_request_auth_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1926 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_auth/registry.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/tracking/request_header/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_header/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_header/abstract_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_header/databricks_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      484 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_header/default_request_header_provider.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2858 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/tracking/request_header/registry.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/transformers/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   119754 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/transformers/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.084431 mlflow-skinny-2.9.1/mlflow/types/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      363 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/types/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27451 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/types/schema.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20196 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/types/utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.088431 mlflow-skinny-2.9.1/mlflow/utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6992 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/_capture_modules.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/_capture_transformers_modules.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7061 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/_spark_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5003 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/annotations.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/arguments_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.088431 mlflow-skinny-2.9.1/mlflow/utils/async_logging/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       68 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/async_logging/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8550 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/async_logging/async_logging_queue.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/async_logging/run_batch.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/async_logging/run_operations.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27503 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16580 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10891 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13405 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/logging_and_warnings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2584 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/metrics_queue.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47658 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/safety.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3566 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/versioning.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      215 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/class_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6432 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/cli_args.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12089 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/conda.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7404 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/credentials.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/data_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24611 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/databricks_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11468 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/docstring_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1240 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/download_cloud_file_chunk.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/env_manager.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23383 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/environment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35622 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/file_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2344 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/git_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24178 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/gorilla.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/mlflow/utils/import_hooks/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13626 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/import_hooks/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/insecure_hash.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1726 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/lazy_load.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/logging_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1297 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/mime_type_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4072 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/mlflow_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10929 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/model_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/name_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/nfs_on_spark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/os.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5799 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/process.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5605 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/promptlab_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20957 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/proto_json_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8473 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/request_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20880 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/requirements_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12876 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/rest_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    58986 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/search_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2368 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/server_cli_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/string_utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1237 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/time.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16712 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/uri.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19365 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/validation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16227 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/utils/virtualenv.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      146 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/version.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/mlflow/xgboost/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35974 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/xgboost/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2877 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/mlflow/xgboost/_autolog.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11887 2023-12-07 05:24:33.000000 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18301 2023-12-07 05:24:34.000000 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-07 05:24:33.000000 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2023-12-07 05:24:33.000000 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-07 05:24:33.000000 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-12-07 05:24:33.000000 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-12-07 05:24:33.000000 mlflow-skinny-2.9.1/mlflow_skinny.egg-info/top_level.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/pylint_plugins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/pylint_plugins/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3138 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/pylint_plugins/assign_checker.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      840 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/pylint_plugins/errors.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4605 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/pylint_plugins/import_checker.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/requirements/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/requirements/core-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      348 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/requirements/gateway-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/requirements/skinny-requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-12-07 05:24:34.092431 mlflow-skinny-2.9.1/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7663 2023-12-07 05:24:32.000000 mlflow-skinny-2.9.1/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.940518 mlflow-skinny-2.9.2/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11382 2023-12-14 05:33:00.000000 mlflow-skinny-2.9.2/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      608 2023-12-14 05:33:00.000000 mlflow-skinny-2.9.2/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11887 2023-12-14 05:33:02.940518 mlflow-skinny-2.9.2/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10160 2023-12-14 05:33:00.000000 mlflow-skinny-2.9.2/README.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-12-14 05:33:00.000000 mlflow-skinny-2.9.2/README_SKINNY.rst
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6711 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/__main__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3891 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/_doctor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6785 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/_promptlab.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10014 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/_spark_autologging.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/artifacts/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6443 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/artifacts/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/azure/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/azure/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11625 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/azure/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/catboost/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13660 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/catboost/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24856 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/data/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2487 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6885 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/artifact_dataset_sources.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      946 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/code_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4333 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6342 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/dataset_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3533 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8301 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/dataset_source_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3768 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/delta_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4904 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/digest_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2598 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/filesystem_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4555 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/http_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9868 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/huggingface_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4312 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/huggingface_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8569 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/numpy_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8529 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/pandas_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/pyfunc_dataset_mixin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2677 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/schema.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/sources.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15745 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/spark_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2231 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/spark_dataset_source.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3857 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/spark_delta_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11898 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/data/tensorflow_dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      881 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/db.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/deployments/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4758 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15582 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16234 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      968 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/constants.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/deployments/databricks/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14118 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/databricks/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4623 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/interface.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/deployments/mlflow/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10774 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/mlflow/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/deployments/openai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8524 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/openai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5498 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/plugin_manager.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.900518 mlflow-skinny-2.9.2/mlflow/deployments/server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/server/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11785 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/server/app.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/server/config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/server/constants.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2834 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/server/runner.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3334 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/deployments/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.904518 mlflow-skinny-2.9.2/mlflow/diviner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27853 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/diviner/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.904518 mlflow-skinny-2.9.2/mlflow/entities/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1294 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1394 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/_mlflow_object.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2118 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/dataset.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1510 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/dataset_input.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1048 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/dataset_summary.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3534 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/experiment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      887 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/experiment_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1215 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/file_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/input_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/lifecycle_stage.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/metric.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.904518 mlflow-skinny-2.9.2/mlflow/entities/model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      528 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      287 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/_model_registry_entity.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6466 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version_stages.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1523 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version_status.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      933 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/registered_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/registered_model_alias.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/model_registry/registered_model_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/multipart_upload.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1133 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/param.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2136 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/run.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3089 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/run_data.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6173 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/run_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/run_inputs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1540 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/run_status.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/run_tag.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1202 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/source_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1816 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/entities/view_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21534 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/environment_variables.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5351 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/exceptions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/experiments.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.904518 mlflow-skinny-2.9.2/mlflow/fastai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25447 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/fastai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5660 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/fastai/callback.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.904518 mlflow-skinny-2.9.2/mlflow/gateway/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1019 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/app.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1584 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/base_models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1230 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16541 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16208 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/constants.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       52 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/exceptions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7918 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/fluent.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/gateway/providers/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3641 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/ai21labs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5544 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/anthropic.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10576 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/bedrock.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5381 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/cohere.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5029 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/huggingface.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8549 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/mlflow.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10165 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/mosaicml.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/openai.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7579 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/palm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2520 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/providers/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/gateway/schemas/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/schemas/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/schemas/chat.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1674 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/schemas/completions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2696 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/schemas/embeddings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8369 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gateway/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/gluon/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17541 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gluon/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2020 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/gluon/_autolog.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/h2o/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12848 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/h2o/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/johnsnowlabs/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35978 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/johnsnowlabs/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/keras/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      349 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/keras/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/keras_core/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/keras_core/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3895 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/keras_core/callback.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/langchain/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25303 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/langchain/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9333 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/langchain/api_request_parallel_processor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5297 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/langchain/retriever_chain.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14536 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/langchain/runnables.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17110 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/langchain/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/lightgbm/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37623 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/lightgbm/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/llm/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      180 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/llm/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/metrics/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14640 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1263 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/base.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/metrics/genai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16511 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/genai_metric.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14540 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/metric_definitions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6377 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/model_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/prompt_template.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/metrics/genai/prompts/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/prompts/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21222 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/prompts/v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/genai/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17279 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/metrics/metric_definitions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5987 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/ml_package_versions.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/mleap/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12909 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/mleap/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3615 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9772 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/cli.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/models/container/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9975 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/container/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.908518 mlflow-skinny-2.9.2/mlflow/models/container/scoring_server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/container/scoring_server/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/container/scoring_server/wsgi.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9756 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/docker_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/models/evaluation/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      490 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3204 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/_shap_patch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/artifacts.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    83924 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    76234 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/default_evaluator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1991 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/evaluator_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6161 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/lift_curve.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10946 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/evaluation/validation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3421 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/flavor_backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2329 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/flavor_backend_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27560 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18684 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/signature.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47232 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11651 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/models/wheeled_model.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/onnx/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24589 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/onnx/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/openai/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33319 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/openai/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15492 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/openai/api_request_parallel_processor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2936 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/openai/retry.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/paddle/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22229 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/paddle/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4862 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/paddle/_paddle_autolog.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/pmdarima/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24099 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pmdarima/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/projects/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17340 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11466 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/_project_spec.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/projects/backend/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      271 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/backend/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2211 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/backend/abstract_backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1079 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/backend/loader.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17238 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/backend/local.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20186 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/databricks.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6456 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/docker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/env_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6361 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/kubernetes.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3572 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/submitted_run.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12265 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/projects/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/prophet/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/prophet/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/protos/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17261 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/databricks_artifacts_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14095 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/databricks_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52871 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/databricks_uc_registry_messages_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15075 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/databricks_uc_registry_service_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16146 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/facet_feature_statistics_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1361 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/internal_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16372 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/mlflow_artifacts_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54475 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/model_registry_pb2.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.912518 mlflow-skinny-2.9.2/mlflow/protos/scalapb/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/scalapb/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3307 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/scalapb/scalapb_pb2.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53666 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/protos/service_pb2.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/pyfunc/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    95819 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      783 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/_mlflow_pyfunc_backend_predict.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16480 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1284 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/mlserver.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20441 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/model.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/pyfunc/scoring_server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17458 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/scoring_server/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5573 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/scoring_server/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/scoring_server/wsgi.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2124 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/spark_model_cache.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1357 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyfunc/stdin_server.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  8045819 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pypi_package_index.json
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/pyspark/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyspark/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/pyspark/ml/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55609 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyspark/ml/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3035 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyspark/ml/_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1886 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pyspark/ml/log_model_allowlist.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/pytorch/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    43245 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pytorch/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17903 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pytorch/_lightning_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2237 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pytorch/_pytorch_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2068 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/pytorch/pickle_module.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1330 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/artifacts.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/cards/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10356 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/cards/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4780 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/cards/histogram_generator.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12527 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/cards/pandas_renderer.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/cards/templates/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/cards/templates/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3488 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/cards/templates/base.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/classification/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/classification/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/classification/v1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      122 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/classification/v1/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/classification/v1/recipe.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2928 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18431 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/dag_help_strings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17976 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/recipe.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/regression/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/regression/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/regression/v1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      114 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/regression/v1/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22525 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/regression/v1/recipe.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/resources/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12211 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/resources/recipe_dag_template.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14920 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/step.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/steps/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/steps/automl/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/automl/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6256 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/automl/flaml.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20651 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/evaluate.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/steps/ingest/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11107 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/ingest/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26390 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/ingest/datasets.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12109 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/predict.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7627 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/register.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19478 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/split.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    59617 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/train.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10571 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/steps/transform.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.916518 mlflow-skinny-2.9.2/mlflow/recipes/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6350 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28397 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/utils/execution.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8990 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/utils/metrics.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7738 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/utils/step.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12374 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/utils/tracking.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2453 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/recipes/utils/wrapped_recipe_model.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/rfunc/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1115 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/rfunc/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3631 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/rfunc/backend.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2527 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/runs.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/sagemaker/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   136129 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/sagemaker/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12921 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/sagemaker/cli.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/sentence_transformers/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15872 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/sentence_transformers/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/server/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9179 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/server/auth/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30594 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       87 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/__main__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      199 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/basic_auth.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      144 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18725 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/config.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/server/auth/db/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      373 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/cli.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3335 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/alembic.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2114 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/env.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/versions/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/versions/8606fa83a998_initial_migration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/versions/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2307 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1408 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/db/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4217 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/entities.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2673 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/logo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/permissions.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1110 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/routes.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10562 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/auth/sqlalchemy_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    80479 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/handlers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/prometheus_exporter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1116 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/server/validation.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/shap/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26545 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/shap/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/sklearn/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    85281 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/sklearn/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    37444 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/sklearn/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/spacy/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13880 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/spacy/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/spark/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49863 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/spark/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/statsmodels/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23362 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/statsmodels/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/store/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      227 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.920518 mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33780 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/registry/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7167 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/registry/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.924518 mlflow-skinny-2.9.2/mlflow/store/artifact/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13427 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6080 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/artifact_repository_registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/azure_blob_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10278 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/azure_data_lake_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5384 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/cli.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10985 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/cloud_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26483 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/databricks_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9778 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/databricks_models_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10152 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/dbfs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5233 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/ftp_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10879 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/gcs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10019 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/hdfs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9027 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/http_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5101 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/local_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3001 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/mlflow_artifacts_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8490 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/models_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11611 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/optimized_s3_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1480 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/r2_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6010 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/runs_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12310 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/s3_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5454 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/sftp_artifact_repo.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5743 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.924518 mlflow-skinny-2.9.2/mlflow/store/artifact/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3924 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/artifact/utils/models.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.924518 mlflow-skinny-2.9.2/mlflow/store/db/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       71 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db/base_sql_model.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db/db_types.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10769 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.924518 mlflow-skinny-2.9.2/mlflow/store/db_migrations/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1634 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/alembic.ini
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2768 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/env.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.924518 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1990 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      462 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      924 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2624 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      779 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/2d6e25af4d3e_increase_max_param_val_length.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1375 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1201 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      940 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1014 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3092 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      476 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5716 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1666 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      582 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      593 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/acf3f17fdcc7_add_storage_location_field_to_model_.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2830 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.924518 mlflow-skinny-2.9.2/mlflow/store/entities/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/entities/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      479 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/entities/paged_list.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/store/model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      605 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15238 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/abstract_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1440 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/base_rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1703 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/databricks_workspace_model_registry_rest_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/store/model_registry/dbmodels/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/dbmodels/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6352 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/dbmodels/models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    41195 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/file_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17006 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50803 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/model_registry/sqlalchemy_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/store/tracking/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1154 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15989 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/abstract_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/store/tracking/dbmodels/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/dbmodels/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8248 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/dbmodels/initial_models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20980 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/dbmodels/models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    55188 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/file_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12804 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/rest_store.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    78876 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/store/tracking/sqlalchemy_store.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/system_metrics/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1788 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      805 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/base_metrics_monitor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      776 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/cpu_monitor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      689 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/disk_monitor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1877 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/gpu_monitor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1352 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/network_monitor.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/system_metrics/system_metrics_monitor.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/tensorflow/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    60226 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tensorflow/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8493 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tensorflow/_autolog.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3807 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tensorflow/callback.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/tracking/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      753 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       41 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15645 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13101 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/fluent.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3152 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7493 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.928518 mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28028 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2335 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8776 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7540 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/artifact_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   150565 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.932518 mlflow-skinny-2.9.2/mlflow/tracking/context/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1077 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/abstract_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_cluster_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_command_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1965 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_job_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1713 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_notebook_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1952 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_repo_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1128 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/default_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/git_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3738 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      467 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/context/system_environment_context.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.932518 mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       28 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1704 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/abstract_context.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2998 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/registry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    84156 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/fluent.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3489 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/llm_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2244 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/metric_value_conversion_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3516 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/registry.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.932518 mlflow-skinny-2.9.2/mlflow/tracking/request_auth/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_auth/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1051 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_auth/abstract_request_auth_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1926 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_auth/registry.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.932518 mlflow-skinny-2.9.2/mlflow/tracking/request_header/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_header/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_header/abstract_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1336 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_header/databricks_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      484 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_header/default_request_header_provider.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2858 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/tracking/request_header/registry.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.932518 mlflow-skinny-2.9.2/mlflow/transformers/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   119975 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/transformers/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.932518 mlflow-skinny-2.9.2/mlflow/types/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      363 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/types/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27451 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/types/schema.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20196 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/types/utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/mlflow/utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6992 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/_capture_modules.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2274 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/_capture_transformers_modules.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7061 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/_spark_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5003 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/annotations.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      400 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/arguments_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/mlflow/utils/async_logging/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       68 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/async_logging/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8550 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/async_logging/async_logging_queue.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/async_logging/run_batch.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/async_logging/run_operations.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27503 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16580 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10891 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13405 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/logging_and_warnings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2584 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/metrics_queue.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    47658 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/safety.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3566 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/versioning.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      215 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/class_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6432 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/cli_args.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12089 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/conda.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7404 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/credentials.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      430 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/data_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24611 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/databricks_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11468 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/docstring_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1240 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/download_cloud_file_chunk.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/env_manager.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23383 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/environment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35701 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/file_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2344 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/git_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24178 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/gorilla.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/mlflow/utils/import_hooks/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13626 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/import_hooks/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      561 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/insecure_hash.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1726 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/lazy_load.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/logging_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1297 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/mime_type_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4072 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/mlflow_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10929 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/model_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5873 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/name_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/nfs_on_spark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9274 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/openai_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      139 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/os.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5799 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/process.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5605 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/promptlab_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20957 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/proto_json_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8850 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/request_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20880 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/requirements_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12876 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/rest_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    58986 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/search_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2368 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/server_cli_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3805 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/string_utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1237 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/time.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17660 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/uri.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19365 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/validation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16227 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/utils/virtualenv.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      146 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/version.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/mlflow/xgboost/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35974 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/xgboost/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2877 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/mlflow/xgboost/_autolog.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11887 2023-12-14 05:33:02.000000 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18345 2023-12-14 05:33:02.000000 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-14 05:33:02.000000 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      344 2023-12-14 05:33:02.000000 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-12-14 05:33:02.000000 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      812 2023-12-14 05:33:02.000000 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-12-14 05:33:02.000000 mlflow-skinny-2.9.2/mlflow_skinny.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/pylint_plugins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      238 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/pylint_plugins/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3138 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/pylint_plugins/assign_checker.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      840 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/pylint_plugins/errors.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4605 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/pylint_plugins/import_checker.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-12-14 05:33:02.936518 mlflow-skinny-2.9.2/requirements/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/requirements/core-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      359 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/requirements/gateway-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      481 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/requirements/skinny-requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-12-14 05:33:02.940518 mlflow-skinny-2.9.2/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7704 2023-12-14 05:33:01.000000 mlflow-skinny-2.9.2/setup.py
```

### Comparing `mlflow-skinny-2.9.1/LICENSE.txt` & `mlflow-skinny-2.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/MANIFEST.in` & `mlflow-skinny-2.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/PKG-INFO` & `mlflow-skinny-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-skinny
-Version: 2.9.1
+Version: 2.9.2
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow-skinny-2.9.1/README.rst` & `mlflow-skinny-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/README_SKINNY.rst` & `mlflow-skinny-2.9.2/README_SKINNY.rst`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/__init__.py` & `mlflow-skinny-2.9.2/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/_doctor.py` & `mlflow-skinny-2.9.2/mlflow/_doctor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/_promptlab.py` & `mlflow-skinny-2.9.2/mlflow/_promptlab.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/_spark_autologging.py` & `mlflow-skinny-2.9.2/mlflow/_spark_autologging.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/artifacts/__init__.py` & `mlflow-skinny-2.9.2/mlflow/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/azure/client.py` & `mlflow-skinny-2.9.2/mlflow/azure/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/catboost/__init__.py` & `mlflow-skinny-2.9.2/mlflow/catboost/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/cli.py` & `mlflow-skinny-2.9.2/mlflow/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/__init__.py` & `mlflow-skinny-2.9.2/mlflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/artifact_dataset_sources.py` & `mlflow-skinny-2.9.2/mlflow/data/artifact_dataset_sources.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/code_dataset_source.py` & `mlflow-skinny-2.9.2/mlflow/data/code_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/dataset.py` & `mlflow-skinny-2.9.2/mlflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/dataset_registry.py` & `mlflow-skinny-2.9.2/mlflow/data/dataset_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/dataset_source.py` & `mlflow-skinny-2.9.2/mlflow/data/dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/dataset_source_registry.py` & `mlflow-skinny-2.9.2/mlflow/data/dataset_source_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/delta_dataset_source.py` & `mlflow-skinny-2.9.2/mlflow/data/delta_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/digest_utils.py` & `mlflow-skinny-2.9.2/mlflow/data/digest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/filesystem_dataset_source.py` & `mlflow-skinny-2.9.2/mlflow/data/filesystem_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/http_dataset_source.py` & `mlflow-skinny-2.9.2/mlflow/data/http_dataset_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import posixpath
 import re
 from typing import Any, Dict
 from urllib.parse import urlparse
 
 from mlflow.data.dataset_source import DatasetSource
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
@@ -37,14 +36,31 @@
         """
         return self._url
 
     @staticmethod
     def _get_source_type() -> str:
         return "http"
 
+    def _extract_filename(self, response) -> str:
+        """
+        Extracts a filename from the Content-Disposition header or the URL's path.
+        """
+        if content_disposition := response.headers.get("Content-Disposition"):
+            for match in re.finditer(r"filename=(.+)", content_disposition):
+                filename = match[1].strip("'\"")
+                if _is_path(filename):
+                    raise MlflowException.invalid_parameter_value(
+                        f"Invalid filename in Content-Disposition header: {filename}. "
+                        "It must be a file name, not a path."
+                    )
+                return filename
+
+        # Extract basename from URL if no valid filename in Content-Disposition
+        return os.path.basename(urlparse(self.url).path)
+
     def load(self, dst_path=None) -> str:
         """
         Downloads the dataset source to the local filesystem.
 
         :param dst_path: Path of the local filesystem destination directory to which to download the
                          dataset source. If the directory does not exist, it is created. If
                          unspecified, the dataset source is downloaded to a new uniquely-named
@@ -54,29 +70,17 @@
         resp = cloud_storage_http_request(
             method="GET",
             url=self.url,
             stream=True,
         )
         augmented_raise_for_status(resp)
 
-        path = urlparse(self.url).path
-        content_disposition = resp.headers.get("Content-Disposition")
-        if content_disposition is not None and (
-            file_name := next(re.finditer(r"filename=(.+)", content_disposition), None)
-        ):
-            # NB: If the filename is quoted, unquote it
-            basename = file_name[1].strip("'\"")
-            if _is_path(basename):
-                raise MlflowException.invalid_parameter_value(
-                    f"Invalid filename in Content-Disposition header: {basename}. "
-                    "It must be a file name, not a path."
-                )
-        elif path is not None and len(posixpath.basename(path)) > 0:
-            basename = posixpath.basename(path)
-        else:
+        basename = self._extract_filename(resp)
+
+        if not basename:
             basename = "dataset_source"
 
         if dst_path is None:
             dst_path = create_tmp_dir()
 
         dst_path = os.path.join(dst_path, basename)
         with open(dst_path, "wb") as f:
```

### Comparing `mlflow-skinny-2.9.1/mlflow/data/huggingface_dataset.py` & `mlflow-skinny-2.9.2/mlflow/data/huggingface_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/huggingface_dataset_source.py` & `mlflow-skinny-2.9.2/mlflow/data/huggingface_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/numpy_dataset.py` & `mlflow-skinny-2.9.2/mlflow/data/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/pandas_dataset.py` & `mlflow-skinny-2.9.2/mlflow/data/pandas_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/pyfunc_dataset_mixin.py` & `mlflow-skinny-2.9.2/mlflow/data/pyfunc_dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/schema.py` & `mlflow-skinny-2.9.2/mlflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/spark_dataset.py` & `mlflow-skinny-2.9.2/mlflow/data/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/spark_dataset_source.py` & `mlflow-skinny-2.9.2/mlflow/data/spark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/spark_delta_utils.py` & `mlflow-skinny-2.9.2/mlflow/data/spark_delta_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/data/tensorflow_dataset.py` & `mlflow-skinny-2.9.2/mlflow/data/tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/db.py` & `mlflow-skinny-2.9.2/mlflow/db.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/__init__.py` & `mlflow-skinny-2.9.2/mlflow/deployments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 import contextlib
 import json
 
 from mlflow.deployments.base import BaseDeploymentClient
 from mlflow.deployments.databricks import DatabricksDeploymentClient, DatabricksEndpoint
 from mlflow.deployments.interface import get_deploy_client, run_local
+from mlflow.deployments.openai import OpenAIDeploymentClient
 from mlflow.deployments.utils import get_deployments_target, set_deployments_target
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
 
 with contextlib.suppress(Exception):
     # MlflowDeploymentClient depends on optional dependencies and can't be imported
     # if they are not installed.
@@ -96,13 +97,14 @@
 
 
 __all__ = [
     "get_deploy_client",
     "run_local",
     "BaseDeploymentClient",
     "DatabricksDeploymentClient",
+    "OpenAIDeploymentClient",
     "DatabricksEndpoint",
     "MlflowDeploymentClient",
     "PredictionsResponse",
     "get_deployments_target",
     "set_deployments_target",
 ]
```

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/base.py` & `mlflow-skinny-2.9.2/mlflow/deployments/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/cli.py` & `mlflow-skinny-2.9.2/mlflow/deployments/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/constants.py` & `mlflow-skinny-2.9.2/mlflow/deployments/constants.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/databricks/__init__.py` & `mlflow-skinny-2.9.2/mlflow/deployments/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/interface.py` & `mlflow-skinny-2.9.2/mlflow/deployments/interface.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/mlflow/__init__.py` & `mlflow-skinny-2.9.2/mlflow/deployments/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/plugin_manager.py` & `mlflow-skinny-2.9.2/mlflow/deployments/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/server/app.py` & `mlflow-skinny-2.9.2/mlflow/deployments/server/app.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/server/config.py` & `mlflow-skinny-2.9.2/mlflow/deployments/server/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/server/runner.py` & `mlflow-skinny-2.9.2/mlflow/deployments/server/runner.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/deployments/utils.py` & `mlflow-skinny-2.9.2/mlflow/deployments/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/diviner/__init__.py` & `mlflow-skinny-2.9.2/mlflow/diviner/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/__init__.py` & `mlflow-skinny-2.9.2/mlflow/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/_mlflow_object.py` & `mlflow-skinny-2.9.2/mlflow/entities/_mlflow_object.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/dataset.py` & `mlflow-skinny-2.9.2/mlflow/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/dataset_input.py` & `mlflow-skinny-2.9.2/mlflow/entities/dataset_input.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/dataset_summary.py` & `mlflow-skinny-2.9.2/mlflow/entities/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/experiment.py` & `mlflow-skinny-2.9.2/mlflow/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/experiment_tag.py` & `mlflow-skinny-2.9.2/mlflow/entities/experiment_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/file_info.py` & `mlflow-skinny-2.9.2/mlflow/entities/file_info.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/input_tag.py` & `mlflow-skinny-2.9.2/mlflow/entities/input_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/lifecycle_stage.py` & `mlflow-skinny-2.9.2/mlflow/entities/lifecycle_stage.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/metric.py` & `mlflow-skinny-2.9.2/mlflow/entities/metric.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/__init__.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version_stages.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version_stages.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version_status.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version_status.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/model_version_tag.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/model_version_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/registered_model.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/registered_model_alias.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/registered_model_alias.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/model_registry/registered_model_tag.py` & `mlflow-skinny-2.9.2/mlflow/entities/model_registry/registered_model_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/multipart_upload.py` & `mlflow-skinny-2.9.2/mlflow/entities/multipart_upload.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/param.py` & `mlflow-skinny-2.9.2/mlflow/entities/param.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/run.py` & `mlflow-skinny-2.9.2/mlflow/entities/run.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/run_data.py` & `mlflow-skinny-2.9.2/mlflow/entities/run_data.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/run_info.py` & `mlflow-skinny-2.9.2/mlflow/entities/run_info.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/run_inputs.py` & `mlflow-skinny-2.9.2/mlflow/entities/run_inputs.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/run_status.py` & `mlflow-skinny-2.9.2/mlflow/entities/run_status.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/run_tag.py` & `mlflow-skinny-2.9.2/mlflow/entities/run_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/source_type.py` & `mlflow-skinny-2.9.2/mlflow/entities/source_type.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/entities/view_type.py` & `mlflow-skinny-2.9.2/mlflow/entities/view_type.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/environment_variables.py` & `mlflow-skinny-2.9.2/mlflow/environment_variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,11 +479,23 @@
 #: Specifies the minimum file size in bytes to use multipart upload when logging artifacts
 #: (default: ``524_288_000`` (500 MB))
 MLFLOW_MULTIPART_UPLOAD_MINIMUM_FILE_SIZE = _EnvironmentVariable(
     "MLFLOW_MULTIPART_UPLOAD_MINIMUM_FILE_SIZE", int, 500 * 1024**2
 )
 
 #: Specifies the chunk size in bytes to use when performing multipart upload
-#: (default: ``104_857_600`` (100 MB))
+#: (default: ``104_857_60`` (10 MB))
 MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE = _EnvironmentVariable(
-    "MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE", int, 100 * 1024**2
+    "MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE", int, 10 * 1024**2
 )
+
+#: Specifies the chunk size in bytes to use when performing multipart download
+#: (default: ``104_857_600`` (100 MB))
+MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE = _EnvironmentVariable(
+    "MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE", int, 100 * 1024**2
+)
+
+#: Specifies whether or not to allow the MLflow server to follow redirects when
+#: making HTTP requests. If set to False, the server will throw an exception if it
+#: encounters a redirect response.
+#: (default: ``True``)
+MLFLOW_ALLOW_HTTP_REDIRECTS = _BooleanEnvironmentVariable("MLFLOW_ALLOW_HTTP_REDIRECTS", True)
```

### Comparing `mlflow-skinny-2.9.1/mlflow/exceptions.py` & `mlflow-skinny-2.9.2/mlflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/experiments.py` & `mlflow-skinny-2.9.2/mlflow/experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/fastai/__init__.py` & `mlflow-skinny-2.9.2/mlflow/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/fastai/callback.py` & `mlflow-skinny-2.9.2/mlflow/fastai/callback.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/__init__.py` & `mlflow-skinny-2.9.2/mlflow/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/app.py` & `mlflow-skinny-2.9.2/mlflow/gateway/app.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/base_models.py` & `mlflow-skinny-2.9.2/mlflow/gateway/base_models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/cli.py` & `mlflow-skinny-2.9.2/mlflow/gateway/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/client.py` & `mlflow-skinny-2.9.2/mlflow/gateway/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/config.py` & `mlflow-skinny-2.9.2/mlflow/gateway/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/constants.py` & `mlflow-skinny-2.9.2/mlflow/gateway/constants.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/fluent.py` & `mlflow-skinny-2.9.2/mlflow/gateway/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/__init__.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/ai21labs.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/ai21labs.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/anthropic.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/base.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/bedrock.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/bedrock.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/cohere.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/cohere.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/huggingface.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/huggingface.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/mlflow.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/mlflow.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/mosaicml.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/mosaicml.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/openai.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/openai.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/palm.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/palm.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/providers/utils.py` & `mlflow-skinny-2.9.2/mlflow/gateway/providers/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/schemas/chat.py` & `mlflow-skinny-2.9.2/mlflow/gateway/schemas/chat.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/schemas/completions.py` & `mlflow-skinny-2.9.2/mlflow/gateway/schemas/completions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/schemas/embeddings.py` & `mlflow-skinny-2.9.2/mlflow/gateway/schemas/embeddings.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gateway/utils.py` & `mlflow-skinny-2.9.2/mlflow/gateway/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gluon/__init__.py` & `mlflow-skinny-2.9.2/mlflow/gluon/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/gluon/_autolog.py` & `mlflow-skinny-2.9.2/mlflow/gluon/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/h2o/__init__.py` & `mlflow-skinny-2.9.2/mlflow/h2o/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/johnsnowlabs/__init__.py` & `mlflow-skinny-2.9.2/mlflow/johnsnowlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/keras_core/callback.py` & `mlflow-skinny-2.9.2/mlflow/keras_core/callback.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/langchain/__init__.py` & `mlflow-skinny-2.9.2/mlflow/langchain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,19 @@
                                                release without warning.
 
         :return: Model predictions.
         """
         import langchain
         from langchain.schema.retriever import BaseRetriever
 
-        from mlflow.openai.utils import TEST_CONTENT, TEST_INTERMEDIATE_STEPS, TEST_SOURCE_DOCUMENTS
+        from mlflow.utils.openai_utils import (
+            TEST_CONTENT,
+            TEST_INTERMEDIATE_STEPS,
+            TEST_SOURCE_DOCUMENTS,
+        )
 
         from tests.langchain.test_langchain_model_export import _mock_async_request
 
         if isinstance(
             self.lc_model,
             (
                 langchain.chains.llm.LLMChain,
```

### Comparing `mlflow-skinny-2.9.1/mlflow/langchain/api_request_parallel_processor.py` & `mlflow-skinny-2.9.2/mlflow/langchain/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/langchain/retriever_chain.py` & `mlflow-skinny-2.9.2/mlflow/langchain/retriever_chain.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/langchain/runnables.py` & `mlflow-skinny-2.9.2/mlflow/langchain/runnables.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,43 +33,46 @@
 
 _STEPS_FOLDER_NAME = "steps"
 _RUNNABLE_STEPS_FILE_NAME = "steps.yaml"
 _BRANCHES_FOLDER_NAME = "branches"
 _RUNNABLE_BRANCHES_FILE_NAME = "branches.yaml"
 _DEFAULT_BRANCH_NAME = "default"
 
-try:
-    from langchain.prompts.loading import type_to_loader_dict as prompts_types
-except ImportError:
-    prompts_types = {"prompt", "few_shot_prompt"}
-
 
 def _load_model_from_config(path, model_config):
-    from langchain.chains.loading import load_chain
     from langchain.chains.loading import type_to_loader_dict as chains_type_to_loader_dict
-    from langchain.llms.loading import get_type_to_cls_dict as llms_get_type_to_cls_dict
-    from langchain.llms.loading import load_llm
-    from langchain.prompts.loading import load_prompt
+    from langchain.llms import get_type_to_cls_dict as llms_get_type_to_cls_dict
+
+    try:
+        from langchain.prompts.loading import type_to_loader_dict as prompts_types
+    except ImportError:
+        prompts_types = {"prompt", "few_shot_prompt"}
 
     config_path = os.path.join(path, model_config.get(_MODEL_DATA_KEY, _MODEL_DATA_YAML_FILE_NAME))
     # Load runnables from config file
     if config_path.endswith(".yaml"):
         config = _load_from_yaml(config_path)
     elif config_path.endswith(".json"):
         config = _load_from_json(config_path)
     else:
         raise MlflowException(
             f"Cannot load runnable without a config file. Got path {config_path}."
         )
     _type = config.get("_type")
     if _type in chains_type_to_loader_dict:
+        from langchain.chains.loading import load_chain
+
         return load_chain(config_path)
     elif _type in prompts_types:
+        from langchain.prompts.loading import load_prompt
+
         return load_prompt(config_path)
     elif _type in llms_get_type_to_cls_dict():
+        from langchain.llms.loading import load_llm
+
         return load_llm(config_path)
     elif _type in custom_type_to_loader_dict():
         return custom_type_to_loader_dict()[_type](config)
     raise MlflowException(f"Unsupported type {_type} for loading.")
 
 
 def _load_model_from_path(path: str, model_config=None):
```

### Comparing `mlflow-skinny-2.9.1/mlflow/langchain/utils.py` & `mlflow-skinny-2.9.2/mlflow/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/lightgbm/__init__.py` & `mlflow-skinny-2.9.2/mlflow/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/__init__.py` & `mlflow-skinny-2.9.2/mlflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/base.py` & `mlflow-skinny-2.9.2/mlflow/metrics/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/genai/base.py` & `mlflow-skinny-2.9.2/mlflow/metrics/genai/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/genai/genai_metric.py` & `mlflow-skinny-2.9.2/mlflow/metrics/genai/genai_metric.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/genai/metric_definitions.py` & `mlflow-skinny-2.9.2/mlflow/metrics/genai/metric_definitions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/genai/model_utils.py` & `mlflow-skinny-2.9.2/mlflow/metrics/genai/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import urllib.parse
 
 from mlflow.exceptions import MlflowException
-from mlflow.openai.utils import REQUEST_URL_CHAT
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
+from mlflow.utils.openai_utils import REQUEST_URL_CHAT
 
 _logger = logging.getLogger(__name__)
 
 
 # TODO: improve this name
 def score_model_on_payload(model_uri, payload, eval_parameters=None):
     """Call the model identified by the given uri with the given payload."""
@@ -50,15 +50,15 @@
         raise MlflowException(
             "OPENAI_API_KEY environment variable not set",
             error_code=INVALID_PARAMETER_VALUE,
         )
 
     from mlflow.openai import _get_api_config
     from mlflow.openai.api_request_parallel_processor import process_api_requests
-    from mlflow.openai.utils import _OAITokenHolder
+    from mlflow.utils.openai_utils import _OAITokenHolder
 
     api_config = _get_api_config()
     api_token = _OAITokenHolder(api_config.api_type)
 
     payload = {
         "messages": [{"role": "user", "content": payload}],
         **eval_parameters,
```

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/genai/prompt_template.py` & `mlflow-skinny-2.9.2/mlflow/metrics/genai/prompt_template.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/genai/prompts/v1.py` & `mlflow-skinny-2.9.2/mlflow/metrics/genai/prompts/v1.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/metrics/metric_definitions.py` & `mlflow-skinny-2.9.2/mlflow/metrics/metric_definitions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/ml_package_versions.py` & `mlflow-skinny-2.9.2/mlflow/ml_package_versions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/mleap/__init__.py` & `mlflow-skinny-2.9.2/mlflow/mleap/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/__init__.py` & `mlflow-skinny-2.9.2/mlflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/cli.py` & `mlflow-skinny-2.9.2/mlflow/models/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/container/__init__.py` & `mlflow-skinny-2.9.2/mlflow/models/container/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/docker_utils.py` & `mlflow-skinny-2.9.2/mlflow/models/docker_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/evaluation/_shap_patch.py` & `mlflow-skinny-2.9.2/mlflow/models/evaluation/_shap_patch.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/evaluation/artifacts.py` & `mlflow-skinny-2.9.2/mlflow/models/evaluation/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/evaluation/base.py` & `mlflow-skinny-2.9.2/mlflow/models/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/evaluation/default_evaluator.py` & `mlflow-skinny-2.9.2/mlflow/models/evaluation/default_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/evaluation/evaluator_registry.py` & `mlflow-skinny-2.9.2/mlflow/models/evaluation/evaluator_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/evaluation/lift_curve.py` & `mlflow-skinny-2.9.2/mlflow/models/evaluation/lift_curve.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/evaluation/validation.py` & `mlflow-skinny-2.9.2/mlflow/models/evaluation/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/flavor_backend.py` & `mlflow-skinny-2.9.2/mlflow/models/flavor_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/flavor_backend_registry.py` & `mlflow-skinny-2.9.2/mlflow/models/flavor_backend_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/model.py` & `mlflow-skinny-2.9.2/mlflow/models/model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/signature.py` & `mlflow-skinny-2.9.2/mlflow/models/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,18 +309,25 @@
     params = None
     params_key = "params"
     if _contains_params(input_example):
         input_example, params = input_example
 
     input_schema = _infer_schema_from_type_hint(hints.input, input_example) if hints.input else None
     params_schema = _infer_param_schema(params) if params else None
-    if params and params_key in inspect.signature(func).parameters:
-        output_example = func(input_example, params=params) if input_example else None
+    input_arg_name = _get_arg_names(func)[input_arg_index]
+    if input_example:
+        inputs = {input_arg_name: input_example}
+        if params and params_key in inspect.signature(func).parameters:
+            inputs[params_key] = params
+        # This is for PythonModel's predict function
+        if input_arg_index == 1:
+            inputs["context"] = None
+        output_example = func(**inputs)
     else:
-        output_example = func(input_example) if input_example else None
+        output_example = None
     output_schema = (
         _infer_schema_from_type_hint(hints.output, output_example) if hints.output else None
     )
     if not any([input_schema, output_schema, params_schema]):
         return None
     return ModelSignature(inputs=input_schema, outputs=output_schema, params=params_schema)
```

### Comparing `mlflow-skinny-2.9.1/mlflow/models/utils.py` & `mlflow-skinny-2.9.2/mlflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/models/wheeled_model.py` & `mlflow-skinny-2.9.2/mlflow/models/wheeled_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/onnx/__init__.py` & `mlflow-skinny-2.9.2/mlflow/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/openai/__init__.py` & `mlflow-skinny-2.9.2/mlflow/openai/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,34 +31,26 @@
 corresponding environment variable. See https://docs.databricks.com/security/secrets/index.html
 for how to set up secrets on Databricks.
 """
 import itertools
 import logging
 import os
 import warnings
-from enum import Enum
 from string import Formatter
-from typing import Any, Dict, NamedTuple, Optional, Set
+from typing import Any, Dict, Optional, Set
 
 import yaml
 
 import mlflow
 from mlflow import pyfunc
 from mlflow.environment_variables import _MLFLOW_TESTING, MLFLOW_OPENAI_SECRET_SCOPE
 from mlflow.exceptions import MlflowException
 from mlflow.models import Model, ModelInputExample, ModelSignature
 from mlflow.models.model import MLMODEL_FILE_NAME
 from mlflow.models.utils import _save_example
-from mlflow.openai.utils import (
-    REQUEST_URL_CHAT,
-    REQUEST_URL_COMPLETIONS,
-    REQUEST_URL_EMBEDDINGS,
-    _OAITokenHolder,
-    _validate_model_params,
-)
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
 from mlflow.tracking._model_registry import DEFAULT_AWAIT_MAX_SLEEP_SECONDS
 from mlflow.tracking.artifact_utils import _download_artifact_from_uri
 from mlflow.types import ColSpec, Schema, TensorSpec
 from mlflow.utils.annotations import experimental
 from mlflow.utils.databricks_utils import (
     check_databricks_secret_scope_access,
@@ -79,34 +71,32 @@
 from mlflow.utils.file_utils import write_to
 from mlflow.utils.model_utils import (
     _add_code_from_conf_to_system_path,
     _get_flavor_configuration,
     _validate_and_copy_code_paths,
     _validate_and_prepare_target_save_path,
 )
+from mlflow.utils.openai_utils import (
+    REQUEST_URL_CHAT,
+    REQUEST_URL_COMPLETIONS,
+    REQUEST_URL_EMBEDDINGS,
+    _OAITokenHolder,
+    _OpenAIApiConfig,
+    _OpenAIEnvVar,
+    _validate_model_params,
+)
 from mlflow.utils.requirements_utils import _get_pinned_requirement
 
 FLAVOR_NAME = "openai"
 MODEL_FILENAME = "model.yaml"
 _PYFUNC_SUPPORTED_TASKS = ("chat.completions", "embeddings", "completions")
 
 _logger = logging.getLogger(__name__)
 
 
-class _OpenAIApiConfig(NamedTuple):
-    api_type: str
-    batch_size: int
-    max_requests_per_minute: int
-    max_tokens_per_minute: int
-    api_version: Optional[str]
-    api_base: str
-    engine: Optional[str]
-    deployment_id: Optional[str]
-
-
 @experimental
 def get_default_pip_requirements():
     """
     :return: A list of default pip requirements for MLflow Models produced by this flavor.
              Calls to :func:`save_model()` and :func:`log_model()` produce a pip environment
              that, at minimum, contains these requirements.
     """
@@ -227,41 +217,14 @@
     try:
         return openai.__version__
     except AttributeError:
         # openai < 0.27.5 doesn't have a __version__ attribute
         return openai.version.VERSION
 
 
-# See https://github.com/openai/openai-python/blob/cf03fe16a92cd01f2a8867537399c12e183ba58e/openai/__init__.py#L30-L38
-# for the list of environment variables that openai-python uses
-class _OpenAIEnvVar(str, Enum):
-    OPENAI_API_TYPE = "OPENAI_API_TYPE"
-    OPENAI_API_BASE = "OPENAI_API_BASE"
-    OPENAI_API_KEY = "OPENAI_API_KEY"
-    OPENAI_API_KEY_PATH = "OPENAI_API_KEY_PATH"
-    OPENAI_API_VERSION = "OPENAI_API_VERSION"
-    OPENAI_ORGANIZATION = "OPENAI_ORGANIZATION"
-    OPENAI_ENGINE = "OPENAI_ENGINE"
-    # use deployment_name instead of deployment_id to be
-    # consistent with gateway
-    OPENAI_DEPLOYMENT_NAME = "OPENAI_DEPLOYMENT_NAME"
-
-    @property
-    def secret_key(self):
-        return self.value.lower()
-
-    @classmethod
-    def read_environ(cls):
-        env_vars = {}
-        for e in _OpenAIEnvVar:
-            if value := os.getenv(e.value):
-                env_vars[e.value] = value
-        return env_vars
-
-
 def _log_secrets_yaml(local_model_dir, scope):
     with open(os.path.join(local_model_dir, "openai.yaml"), "w") as f:
         yaml.safe_dump({e.value: f"{scope}:{e.secret_key}" for e in _OpenAIEnvVar}, f)
 
 
 def _parse_format_fields(s) -> Set[str]:
     """
@@ -855,15 +818,15 @@
         :param params: Additional parameters to pass to the model for inference.
 
                        .. Note:: Experimental: This parameter may change or be removed in a future
                                                release without warning.
 
         :return: Model predictions.
         """
-        from mlflow.openai.utils import _mock_openai_request
+        from mlflow.utils.openai_utils import _mock_openai_request
 
         with _mock_openai_request():
             return super().predict(data)
 
 
 def _load_pyfunc(path):
     """
```

### Comparing `mlflow-skinny-2.9.1/mlflow/openai/api_request_parallel_processor.py` & `mlflow-skinny-2.9.2/mlflow/openai/api_request_parallel_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 
 import requests
 import tiktoken
 
 import mlflow
-from mlflow.openai.utils import _OAITokenHolder
 from mlflow.protos.databricks_pb2 import UNAUTHENTICATED
+from mlflow.utils.openai_utils import _OAITokenHolder
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
 class StatusTracker:
     """
```

### Comparing `mlflow-skinny-2.9.1/mlflow/openai/retry.py` & `mlflow-skinny-2.9.2/mlflow/openai/retry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/openai/utils.py` & `mlflow-skinny-2.9.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,267 +1,219 @@
-import json
 import os
-import time
-from contextlib import contextmanager
-from unittest import mock
+import logging
+from importlib.machinery import SourceFileLoader
+from setuptools import setup, find_packages, Command
 
-import requests
+_MLFLOW_SKINNY_ENV_VAR = "MLFLOW_SKINNY"
 
-import mlflow
+version = (
+    SourceFileLoader("mlflow.version", os.path.join("mlflow", "version.py")).load_module().VERSION
+)
 
-TEST_CONTENT = "test"
 
-TEST_SOURCE_DOCUMENTS = [
-    {
-        "page_content": "We see the unity among leaders ...",
-        "metadata": {"source": "tests/langchain/state_of_the_union.txt"},
-    },
+# Get a list of all files in the directory to include in our module
+def package_files(directory):
+    """
+    Recursively collects file paths within a directory relative to the mlflow directory.
+    """
+    mlflow_dir = os.path.abspath("mlflow")
+    paths = []
+    for root, _, filenames in os.walk(directory):
+        for filename in filenames:
+            paths.append(os.path.relpath(os.path.join(root, filename), mlflow_dir))
+    return paths
+
+
+def is_comment_or_empty(line):
+    stripped = line.strip()
+    return stripped == "" or stripped.startswith("#")
+
+
+def remove_comments_and_empty_lines(lines):
+    return [line for line in lines if not is_comment_or_empty(line)]
+
+
+# Prints out a set of paths (relative to the mlflow/ directory) of files in mlflow/server/js/build
+# to include in the wheel, e.g. "server/js/build/index.html"
+js_files = package_files("mlflow/server/js/build")
+models_container_server_files = package_files("mlflow/models/container")
+alembic_files = [
+    "store/db_migrations/alembic.ini",
+    "temporary_db_migrations_for_pre_1_users/alembic.ini",
 ]
-TEST_INTERMEDIATE_STEPS = (
-    [
-        {
-            "tool": "Search",
-            "tool_input": "High temperature in SF yesterday",
-            "log": " I need to find the temperature first...",
-            "result": "San Francisco...",
-        },
-    ],
-)
+extra_files = [
+    "pypi_package_index.json",
+    "pyspark/ml/log_model_allowlist.txt",
+    "server/auth/basic_auth.ini",
+    "server/auth/db/migrations/alembic.ini",
+]
+recipes_template_files = package_files("mlflow/recipes/resources")
+recipes_files = package_files("mlflow/recipes/cards/templates")
 
-REQUEST_URL_CHAT = "https://api.openai.com/v1/chat/completions"
-REQUEST_URL_COMPLETIONS = "https://api.openai.com/v1/completions"
-REQUEST_URL_EMBEDDINGS = "https://api.openai.com/v1/embeddings"
-
-REQUEST_FIELDS_CHAT = {
-    "model",
-    "messages",
-    "frequency_penalty",
-    "logit_bias",
-    "max_tokens",
-    "n",
-    "presence_penalty",
-    "response_format",
-    "seed",
-    "stop",
-    "stream",
-    "temperature",
-    "top_p",
-    "tools",
-    "tool_choice",
-    "user",
-    "function_call",
-    "functions",
-}
-REQUEST_FIELDS_COMPLETIONS = {
-    "model",
-    "prompt",
-    "best_of",
-    "echo",
-    "frequency_penalty",
-    "logit_bias",
-    "logprobs",
-    "max_tokens",
-    "n",
-    "presence_penalty",
-    "seed",
-    "stop",
-    "stream",
-    "suffix",
-    "temperature",
-    "top_p",
-    "user",
-}
-REQUEST_FIELDS_EMBEDDINGS = {"input", "model", "encoding_format", "user"}
-REQUEST_FIELDS = REQUEST_FIELDS_CHAT | REQUEST_FIELDS_COMPLETIONS | REQUEST_FIELDS_EMBEDDINGS
-
-
-class _MockResponse:
-    def __init__(self, status_code, json_data):
-        self.status_code = status_code
-        self.content = json.dumps(json_data).encode()
-        self.headers = {"Content-Type": "application/json"}
-        self.text = mlflow.__version__
-        self.json_data = json_data
-
-    def json(self):
-        return self.json_data
-
-
-def _chat_completion_json_sample(content):
-    # https://platform.openai.com/docs/api-reference/chat/create
-    return {
-        "id": "chatcmpl-123",
-        "object": "chat.completion",
-        "created": 1677652288,
-        "choices": [
-            {
-                "index": 0,
-                "message": {"role": "assistant", "content": content},
-                "finish_reason": "stop",
-                "text": content,
-            }
-        ],
-        "usage": {"prompt_tokens": 9, "completion_tokens": 12, "total_tokens": 21},
-    }
 
+"""
+Minimal requirements for the skinny MLflow client which provides a limited
+subset of functionality such as: RESTful client functionality for Tracking and
+Model Registry, as well as support for Project execution against local backends
+and Databricks.
+"""
+with open(os.path.join("requirements", "skinny-requirements.txt")) as f:
+    SKINNY_REQUIREMENTS = remove_comments_and_empty_lines(f.read().splitlines())
 
-def _completion_json_sample(content):
-    return {
-        "id": "cmpl-123",
-        "object": "text_completion",
-        "created": 1589478378,
-        "model": "text-davinci-003",
-        "choices": [{"text": content, "index": 0, "finish_reason": "length"}],
-        "usage": {"prompt_tokens": 5, "completion_tokens": 7, "total_tokens": 12},
-    }
-
-
-def _models_retrieve_json_sample():
-    # https://platform.openai.com/docs/api-reference/models/retrieve
-    return {
-        "id": "gpt-3.5-turbo",
-        "object": "model",
-        "owned_by": "openai",
-        "permission": [],
-    }
-
-
-def _mock_chat_completion_response(content=TEST_CONTENT):
-    return _MockResponse(200, _chat_completion_json_sample(content))
-
-
-def _mock_completion_response(content=TEST_CONTENT):
-    return _MockResponse(200, _completion_json_sample(content))
-
-
-def _mock_embeddings_response(num_texts):
-    return _MockResponse(
-        200,
-        {
-            "object": "list",
-            "data": [
-                {
-                    "object": "embedding",
-                    "embedding": [
-                        0.0,
-                    ],
-                    "index": i,
-                }
-                for i in range(num_texts)
-            ],
-            "model": "text-embedding-ada-002",
-            "usage": {"prompt_tokens": 8, "total_tokens": 8},
-        },
-    )
-
-
-def _mock_models_retrieve_response():
-    return _MockResponse(200, _models_retrieve_json_sample())
-
-
-@contextmanager
-def _mock_request(**kwargs):
-    with mock.patch("requests.Session.request", **kwargs) as m:
-        yield m
-
-
-@contextmanager
-def _mock_request_post(**kwargs):
-    with mock.patch("requests.post", **kwargs) as m:
-        yield m
-
-
-def _mock_openai_request():
-    original = requests.post
-
-    def request(*args, **kwargs):
-        url = kwargs.get("url")
-        for key in kwargs.get("json"):
-            assert key in REQUEST_FIELDS, f"'{key}' is not a valid request field"
-
-        if "/chat/completions" in url:
-            messages = kwargs.get("json").get("messages")
-            return _mock_chat_completion_response(content=json.dumps(messages))
-        elif "/completions" in url:
-            prompt = kwargs.get("json").get("prompt")
-            return _mock_completion_response(content=json.dumps(prompt))
-        elif "/embeddings" in url:
-            inp = kwargs.get("json").get("input")
-            return _mock_embeddings_response(len(inp) if isinstance(inp, list) else 1)
-        else:
-            return original(*args, **kwargs)
-
-    return _mock_request_post(new=request)
-
-
-def _validate_model_params(task, model, params):
-    if not params:
-        return
-
-    if any(key in model for key in params):
-        raise mlflow.MlflowException.invalid_parameter_value(
-            f"Providing any of {list(model.keys())} as parameters in the signature is not "
-            "allowed because they were indicated as part of the OpenAI model. Either remove "
-            "the argument when logging the model or remove the parameter from the signature.",
-        )
-    if "batch_size" in params and task == "chat.completions":
-        raise mlflow.MlflowException.invalid_parameter_value(
-            "Parameter `batch_size` is not supported for task `chat.completions`"
-        )
 
+"""
+These are the core requirements for the complete MLflow platform, which augments
+the skinny client functionality with support for running the MLflow Tracking
+Server & UI. It also adds project backends such as Docker and Kubernetes among
+other capabilities.
+"""
+with open(os.path.join("requirements", "core-requirements.txt")) as f:
+    CORE_REQUIREMENTS = SKINNY_REQUIREMENTS + remove_comments_and_empty_lines(f.read().splitlines())
 
-def _exclude_params_from_envs(params, envs):
-    """
-    params passed at inference time should override envs.
-    """
-    return {k: v for k, v in envs.items() if k not in params} if params else envs
+with open(os.path.join("requirements", "gateway-requirements.txt")) as f:
+    GATEWAY_REQUIREMENTS = remove_comments_and_empty_lines(f.read().splitlines())
+
+_is_mlflow_skinny = bool(os.environ.get(_MLFLOW_SKINNY_ENV_VAR))
+logging.debug("{} env var is set: {}".format(_MLFLOW_SKINNY_ENV_VAR, _is_mlflow_skinny))
+
+
+class ListDependencies(Command):
+    # `python setup.py <command name>` prints out "running <command name>" by default.
+    # This logging message must be hidden by specifying `--quiet` (or `-q`) when piping the output
+    # of this command to `pip install`.
+    description = "List mlflow dependencies"
+    user_options = [
+        ("skinny", None, "List mlflow-skinny dependencies"),
+    ]
+
+    def initialize_options(self):
+        self.skinny = False
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        dependencies = SKINNY_REQUIREMENTS if self.skinny else CORE_REQUIREMENTS
+        print("\n".join(dependencies))
 
 
-class _OAITokenHolder:
-    def __init__(self, api_type):
-        self._api_token = None
-        self._credential = None
-        self._is_azure_ad = api_type in ("azure_ad", "azuread")
-        self._key_configured = "OPENAI_API_KEY" in os.environ
-
-        if self._is_azure_ad and not self._key_configured:
-            try:
-                from azure.identity import DefaultAzureCredential
-            except ImportError:
-                raise mlflow.MlflowException(
-                    "Using API type `azure_ad` or `azuread` requires the package"
-                    " `azure-identity` to be installed."
-                )
-            self._credential = DefaultAzureCredential()
-
-    def validate(self, logger=None):
-        """
-        Validates the token or API key configured for accessing the OpenAI resource.
-        """
-        if self._key_configured:
-            return
-
-        if self._is_azure_ad:
-            if not self._api_token or self._api_token.expires_on < time.time() + 60:
-                from azure.core.exceptions import ClientAuthenticationError
-
-                if logger:
-                    logger.debug(
-                        "Token for Azure AD is either expired or unset. Attempting to "
-                        "acquire a new token."
-                    )
-                try:
-                    self._api_token = self._credential.get_token(
-                        "https://cognitiveservices.azure.com/.default"
-                    )
-                except ClientAuthenticationError as err:
-                    raise mlflow.MlflowException(
-                        "Unable to acquire a valid Azure AD token for the resource due to "
-                        f"the following error: {err.message}"
-                    ) from err
-                os.environ["OPENAI_API_KEY"] = self._api_token.token
-            if logger:
-                logger.debug("Token refreshed successfully")
-        else:
-            raise mlflow.MlflowException(
-                "OpenAI API key must be set in the ``OPENAI_API_KEY`` environment variable."
-            )
+MINIMUM_SUPPORTED_PYTHON_VERSION = "3.8"
+
+
+class MinPythonVersion(Command):
+    description = "Print out the minimum supported Python version"
+    user_options = []
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        print(MINIMUM_SUPPORTED_PYTHON_VERSION)
+
+
+skinny_package_data = [
+    # include alembic files to enable usage of the skinny client with SQL databases
+    # if users install sqlalchemy and alembic independently
+    *alembic_files,
+    *extra_files,
+    *recipes_template_files,
+    *recipes_files,
+]
+
+setup(
+    name="mlflow" if not _is_mlflow_skinny else "mlflow-skinny",
+    version=version,
+    packages=find_packages(exclude=["tests", "tests.*"]),
+    package_data=(
+        {"mlflow": skinny_package_data}
+        if _is_mlflow_skinny
+        else {
+            "mlflow": [
+                *skinny_package_data,
+                *js_files,
+                *models_container_server_files,
+            ]
+        }
+    ),
+    install_requires=CORE_REQUIREMENTS if not _is_mlflow_skinny else SKINNY_REQUIREMENTS,
+    extras_require={
+        "extras": [
+            # Required to log artifacts and models to HDFS artifact locations
+            "pyarrow",
+            # Required to sign outgoing request with SigV4 signature
+            "requests-auth-aws-sigv4",
+            # Required to log artifacts and models to AWS S3 artifact locations
+            "boto3",
+            # Required to log artifacts and models to GCS artifact locations
+            "google-cloud-storage>=1.30.0",
+            "azureml-core>=1.2.0",
+            # Required to log artifacts to SFTP artifact locations
+            "pysftp",
+            # Required by the mlflow.projects module, when running projects against
+            # a remote Kubernetes cluster
+            "kubernetes",
+            # Required to serve models through MLServer
+            # NOTE: remove the upper version pin once protobuf is no longer pinned in mlserver
+            # Reference issue: https://github.com/SeldonIO/MLServer/issues/1089
+            "mlserver>=1.2.0,!=1.3.1",
+            "mlserver-mlflow>=1.2.0,!=1.3.1",
+            "virtualenv",
+            # Required for exporting metrics from the MLflow server to Prometheus
+            # as part of the MLflow server monitoring add-on
+            "prometheus-flask-exporter",
+        ],
+        "databricks": [
+            # Required to write model artifacts to unity catalog locations
+            "azure-storage-file-datalake>12",
+            "google-cloud-storage>=1.30.0",
+            "boto3>1",
+        ],
+        "gateway": GATEWAY_REQUIREMENTS,
+        "genai": GATEWAY_REQUIREMENTS,
+        "sqlserver": ["mlflow-dbstore"],
+        "aliyun-oss": ["aliyunstoreplugin"],
+        "xethub": ["mlflow-xethub"],
+    },
+    entry_points="""
+        [console_scripts]
+        mlflow=mlflow.cli:cli
+
+        [mlflow.app]
+        basic-auth=mlflow.server.auth:create_app
+
+        [mlflow.app.client]
+        basic-auth=mlflow.server.auth.client:AuthServiceClient
+
+        [mlflow.deployments]
+        databricks=mlflow.deployments.databricks
+        http=mlflow.deployments.mlflow
+        https=mlflow.deployments.mlflow
+        openai=mlflow.deployments.openai
+    """,
+    cmdclass={
+        "dependencies": ListDependencies,
+        "min_python_version": MinPythonVersion,
+    },
+    zip_safe=False,
+    author="Databricks",
+    description="MLflow: A Platform for ML Development and Productionization",
+    long_description=open("README.rst").read()
+    if not _is_mlflow_skinny
+    else open("README_SKINNY.rst").read() + open("README.rst").read(),
+    long_description_content_type="text/x-rst",
+    license="Apache License 2.0",
+    classifiers=[
+        "Intended Audience :: Developers",
+        f"Programming Language :: Python :: {MINIMUM_SUPPORTED_PYTHON_VERSION}",
+    ],
+    keywords="ml ai databricks",
+    url="https://mlflow.org/",
+    python_requires=f">={MINIMUM_SUPPORTED_PYTHON_VERSION}",
+    project_urls={
+        "Bug Tracker": "https://github.com/mlflow/mlflow/issues",
+        "Documentation": "https://mlflow.org/docs/latest/index.html",
+        "Source Code": "https://github.com/mlflow/mlflow",
+    },
+)
```

### Comparing `mlflow-skinny-2.9.1/mlflow/paddle/__init__.py` & `mlflow-skinny-2.9.2/mlflow/paddle/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/paddle/_paddle_autolog.py` & `mlflow-skinny-2.9.2/mlflow/paddle/_paddle_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pmdarima/__init__.py` & `mlflow-skinny-2.9.2/mlflow/pmdarima/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/__init__.py` & `mlflow-skinny-2.9.2/mlflow/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/_project_spec.py` & `mlflow-skinny-2.9.2/mlflow/projects/_project_spec.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/backend/abstract_backend.py` & `mlflow-skinny-2.9.2/mlflow/projects/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/backend/loader.py` & `mlflow-skinny-2.9.2/mlflow/projects/backend/loader.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/backend/local.py` & `mlflow-skinny-2.9.2/mlflow/projects/backend/local.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/databricks.py` & `mlflow-skinny-2.9.2/mlflow/projects/databricks.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/docker.py` & `mlflow-skinny-2.9.2/mlflow/projects/docker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/kubernetes.py` & `mlflow-skinny-2.9.2/mlflow/projects/kubernetes.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/submitted_run.py` & `mlflow-skinny-2.9.2/mlflow/projects/submitted_run.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/projects/utils.py` & `mlflow-skinny-2.9.2/mlflow/projects/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/prophet/__init__.py` & `mlflow-skinny-2.9.2/mlflow/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/databricks_artifacts_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/databricks_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/databricks_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/databricks_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/databricks_uc_registry_messages_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/databricks_uc_registry_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/databricks_uc_registry_service_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/databricks_uc_registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/facet_feature_statistics_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/facet_feature_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/internal_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/internal_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/mlflow_artifacts_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/mlflow_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/model_registry_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/model_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/scalapb/scalapb_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/scalapb/scalapb_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/protos/service_pb2.py` & `mlflow-skinny-2.9.2/mlflow/protos/service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/__init__.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/_mlflow_pyfunc_backend_predict.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/_mlflow_pyfunc_backend_predict.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/backend.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/mlserver.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/mlserver.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/model.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/scoring_server/__init__.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/scoring_server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/scoring_server/client.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/scoring_server/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/spark_model_cache.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/spark_model_cache.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyfunc/stdin_server.py` & `mlflow-skinny-2.9.2/mlflow/pyfunc/stdin_server.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pypi_package_index.json` & `mlflow-skinny-2.9.2/mlflow/pypi_package_index.json`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyspark/ml/__init__.py` & `mlflow-skinny-2.9.2/mlflow/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyspark/ml/_autolog.py` & `mlflow-skinny-2.9.2/mlflow/pyspark/ml/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pyspark/ml/log_model_allowlist.txt` & `mlflow-skinny-2.9.2/mlflow/pyspark/ml/log_model_allowlist.txt`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pytorch/__init__.py` & `mlflow-skinny-2.9.2/mlflow/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pytorch/_lightning_autolog.py` & `mlflow-skinny-2.9.2/mlflow/pytorch/_lightning_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pytorch/_pytorch_autolog.py` & `mlflow-skinny-2.9.2/mlflow/pytorch/_pytorch_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/pytorch/pickle_module.py` & `mlflow-skinny-2.9.2/mlflow/pytorch/pickle_module.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/__init__.py` & `mlflow-skinny-2.9.2/mlflow/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/artifacts.py` & `mlflow-skinny-2.9.2/mlflow/recipes/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/cards/__init__.py` & `mlflow-skinny-2.9.2/mlflow/recipes/cards/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,17 +116,18 @@
 
     def to_html(self) -> str:
         """
         Returns a rendered HTML representing the content of the tab.
 
         :return: a HTML string
         """
-        import jinja2
+        from jinja2 import BaseLoader
+        from jinja2.sandbox import SandboxedEnvironment
 
-        j2_env = jinja2.Environment(loader=jinja2.BaseLoader()).from_string(self.template)
+        j2_env = SandboxedEnvironment(loader=BaseLoader()).from_string(self.template)
         return j2_env.render({**self._context})
 
 
 class BaseCard:
     def __init__(self, recipe_name: str, step_name: str) -> None:
         """
         BaseCard Constructor
```

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/cards/histogram_generator.py` & `mlflow-skinny-2.9.2/mlflow/recipes/cards/histogram_generator.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/cards/pandas_renderer.py` & `mlflow-skinny-2.9.2/mlflow/recipes/cards/pandas_renderer.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/cards/templates/base.html` & `mlflow-skinny-2.9.2/mlflow/recipes/cards/templates/base.html`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/classification/v1/recipe.py` & `mlflow-skinny-2.9.2/mlflow/recipes/classification/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/cli.py` & `mlflow-skinny-2.9.2/mlflow/recipes/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/dag_help_strings.py` & `mlflow-skinny-2.9.2/mlflow/recipes/dag_help_strings.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/recipe.py` & `mlflow-skinny-2.9.2/mlflow/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/regression/v1/recipe.py` & `mlflow-skinny-2.9.2/mlflow/recipes/regression/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/resources/recipe_dag_template.html` & `mlflow-skinny-2.9.2/mlflow/recipes/resources/recipe_dag_template.html`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/step.py` & `mlflow-skinny-2.9.2/mlflow/recipes/step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/automl/flaml.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/automl/flaml.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/evaluate.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/evaluate.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/ingest/__init__.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/ingest/datasets.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/ingest/datasets.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/predict.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/predict.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/register.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/register.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/split.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/split.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/train.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/train.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/steps/transform.py` & `mlflow-skinny-2.9.2/mlflow/recipes/steps/transform.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/utils/__init__.py` & `mlflow-skinny-2.9.2/mlflow/recipes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/utils/execution.py` & `mlflow-skinny-2.9.2/mlflow/recipes/utils/execution.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/utils/metrics.py` & `mlflow-skinny-2.9.2/mlflow/recipes/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/utils/step.py` & `mlflow-skinny-2.9.2/mlflow/recipes/utils/step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/utils/tracking.py` & `mlflow-skinny-2.9.2/mlflow/recipes/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/recipes/utils/wrapped_recipe_model.py` & `mlflow-skinny-2.9.2/mlflow/recipes/utils/wrapped_recipe_model.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/rfunc/__init__.py` & `mlflow-skinny-2.9.2/mlflow/rfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/rfunc/backend.py` & `mlflow-skinny-2.9.2/mlflow/rfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/runs.py` & `mlflow-skinny-2.9.2/mlflow/runs.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/sagemaker/__init__.py` & `mlflow-skinny-2.9.2/mlflow/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/sagemaker/cli.py` & `mlflow-skinny-2.9.2/mlflow/sagemaker/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/sentence_transformers/__init__.py` & `mlflow-skinny-2.9.2/mlflow/sentence_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/__init__.py` & `mlflow-skinny-2.9.2/mlflow/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/__init__.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/client.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/config.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/alembic.ini` & `mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/env.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/db/migrations/versions/8606fa83a998_initial_migration.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/db/migrations/versions/8606fa83a998_initial_migration.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/db/models.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/db/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/db/utils.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/entities.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/logo.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/logo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/permissions.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/routes.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/routes.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/auth/sqlalchemy_store.py` & `mlflow-skinny-2.9.2/mlflow/server/auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/server/handlers.py` & `mlflow-skinny-2.9.2/mlflow/server/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 from mlflow.tracking._tracking_service.registry import TrackingStoreRegistry
 from mlflow.tracking.registry import UnsupportedModelRegistryStoreURIException
 from mlflow.utils.file_utils import local_file_uri_to_path
 from mlflow.utils.mime_type_utils import _guess_mime_type
 from mlflow.utils.promptlab_utils import _create_promptlab_run_impl
 from mlflow.utils.proto_json_utils import message_to_json, parse_dict
 from mlflow.utils.string_utils import is_string_type
-from mlflow.utils.uri import is_file_uri, is_local_uri, validate_path_is_safe
+from mlflow.utils.uri import is_file_uri, is_local_uri, validate_path_is_safe, validate_query_string
 from mlflow.utils.validation import _validate_batch_log_api_req
 
 _logger = logging.getLogger(__name__)
 _tracking_store = None
 _model_registry_store = None
 _artifact_repo = None
 STATIC_PREFIX_ENV_VAR = "_MLFLOW_STATIC_PREFIX"
@@ -544,15 +544,15 @@
 def get_artifact_handler():
     from querystring_parser import parser
 
     query_string = request.query_string.decode("utf-8")
     request_dict = parser.parse(query_string, normalized=True)
     run_id = request_dict.get("run_id") or request_dict.get("run_uuid")
     path = request_dict["path"]
-    validate_path_is_safe(path)
+    path = validate_path_is_safe(path)
     run = _get_tracking_store().get_run(run_id)
 
     if _is_servable_proxied_run_artifact_root(run.info.artifact_uri):
         artifact_repo = _get_artifact_repo_mlflow_artifacts()
         artifact_path = _get_proxied_run_artifact_destination_path(
             proxied_artifact_root=run.info.artifact_uri,
             relative_path=path,
@@ -582,14 +582,19 @@
             "name": [_assert_required, _assert_string],
             "artifact_location": [_assert_string],
             "tags": [_assert_array],
         },
     )
 
     tags = [ExperimentTag(tag.key, tag.value) for tag in request_message.tags]
+
+    # Validate query string in artifact location to prevent attacks
+    parsed_artifact_locaion = urllib.parse.urlparse(request_message.artifact_location)
+    validate_query_string(parsed_artifact_locaion.query)
+
     experiment_id = _get_tracking_store().create_experiment(
         request_message.name, request_message.artifact_location, tags
     )
     response_message = CreateExperiment.Response()
     response_message.experiment_id = experiment_id
     response = Response(mimetype="application/json")
     response.set_data(message_to_json(response_message))
@@ -932,15 +937,15 @@
             "path": [_assert_string],
             "page_token": [_assert_string],
         },
     )
     response_message = ListArtifacts.Response()
     if request_message.HasField("path"):
         path = request_message.path
-        validate_path_is_safe(path)
+        path = validate_path_is_safe(path)
     else:
         path = None
     run_id = request_message.run_id or request_message.run_uuid
     run = _get_tracking_store().get_run(run_id)
 
     if _is_servable_proxied_run_artifact_root(run.info.artifact_uri):
         artifact_entities = _list_artifacts_for_proxied_run_artifact_root(
@@ -1227,15 +1232,15 @@
         )
     path = args.get("path")
     if not path:
         raise MlflowException(
             message="Request must specify path.",
             error_code=INVALID_PARAMETER_VALUE,
         )
-    validate_path_is_safe(path)
+    path = validate_path_is_safe(path)
 
     if request.content_length and request.content_length > 10 * 1024 * 1024:
         raise MlflowException(
             message="Artifact size is too large. Max size is 10MB.",
             error_code=INVALID_PARAMETER_VALUE,
         )
 
@@ -1651,15 +1656,15 @@
     from querystring_parser import parser
 
     query_string = request.query_string.decode("utf-8")
     request_dict = parser.parse(query_string, normalized=True)
     name = request_dict.get("name")
     version = request_dict.get("version")
     path = request_dict["path"]
-    validate_path_is_safe(path)
+    path = validate_path_is_safe(path)
     artifact_uri = _get_model_registry_store().get_model_version_download_uri(name, version)
     if _is_servable_proxied_run_artifact_root(artifact_uri):
         artifact_repo = _get_artifact_repo_mlflow_artifacts()
         artifact_path = _get_proxied_run_artifact_destination_path(
             proxied_artifact_root=artifact_uri,
             relative_path=path,
         )
@@ -1877,15 +1882,15 @@
 @catch_mlflow_exception
 @_disable_unless_serve_artifacts
 def _download_artifact(artifact_path):
     """
     A request handler for `GET /mlflow-artifacts/artifacts/<artifact_path>` to download an artifact
     from `artifact_path` (a relative path from the root artifact directory).
     """
-    validate_path_is_safe(artifact_path)
+    artifact_path = validate_path_is_safe(artifact_path)
     tmp_dir = tempfile.TemporaryDirectory()
     artifact_repo = _get_artifact_repo_mlflow_artifacts()
     dst = artifact_repo.download_artifacts(artifact_path, tmp_dir.name)
 
     # Ref: https://stackoverflow.com/a/24613980/6943581
     file_handle = open(dst, "rb")  # noqa: SIM115
 
@@ -1902,15 +1907,15 @@
 @catch_mlflow_exception
 @_disable_unless_serve_artifacts
 def _upload_artifact(artifact_path):
     """
     A request handler for `PUT /mlflow-artifacts/artifacts/<artifact_path>` to upload an artifact
     to `artifact_path` (a relative path from the root artifact directory).
     """
-    validate_path_is_safe(artifact_path)
+    artifact_path = validate_path_is_safe(artifact_path)
     head, tail = posixpath.split(artifact_path)
     with tempfile.TemporaryDirectory() as tmp_dir:
         tmp_path = os.path.join(tmp_dir, tail)
         with open(tmp_path, "wb") as f:
             chunk_size = 1024 * 1024  # 1 MB
             while True:
                 chunk = request.stream.read(chunk_size)
@@ -1928,19 +1933,15 @@
 @_disable_unless_serve_artifacts
 def _list_artifacts_mlflow_artifacts():
     """
     A request handler for `GET /mlflow-artifacts/artifacts?path=<value>` to list artifacts in `path`
     (a relative path from the root artifact directory).
     """
     request_message = _get_request_message(ListArtifactsMlflowArtifacts())
-    if request_message.HasField("path"):
-        validate_path_is_safe(request_message.path)
-        path = request_message.path
-    else:
-        path = None
+    path = validate_path_is_safe(request_message.path) if request_message.HasField("path") else None
     artifact_repo = _get_artifact_repo_mlflow_artifacts()
     files = []
     for file_info in artifact_repo.list_artifacts(path):
         basename = posixpath.basename(file_info.path)
         new_file_info = FileInfo(basename, file_info.is_dir, file_info.file_size)
         files.append(new_file_info.to_proto())
     response_message = ListArtifacts.Response()
@@ -1953,15 +1954,15 @@
 @catch_mlflow_exception
 @_disable_unless_serve_artifacts
 def _delete_artifact_mlflow_artifacts(artifact_path):
     """
     A request handler for `DELETE /mlflow-artifacts/artifacts?path=<value>` to delete artifacts in
     `path` (a relative path from the root artifact directory).
     """
-    validate_path_is_safe(artifact_path)
+    artifact_path = validate_path_is_safe(artifact_path)
     _get_request_message(DeleteArtifact())
     artifact_repo = _get_artifact_repo_mlflow_artifacts()
     artifact_repo.delete_artifacts(artifact_path)
     response_message = DeleteArtifact.Response()
     response = Response(mimetype="application/json")
     response.set_data(message_to_json(response_message))
     return response
@@ -1975,15 +1976,15 @@
 @catch_mlflow_exception
 @_disable_unless_serve_artifacts
 def _create_multipart_upload_artifact(artifact_path):
     """
     A request handler for `POST /mlflow-artifacts/mpu/create` to create a multipart upload
     to `artifact_path` (a relative path from the root artifact directory).
     """
-    validate_path_is_safe(artifact_path)
+    artifact_path = validate_path_is_safe(artifact_path)
 
     request_message = _get_request_message(
         CreateMultipartUpload(),
         schema={
             "path": [_assert_required, _assert_string],
             "num_parts": [_assert_intlike],
         },
@@ -2008,15 +2009,15 @@
 @catch_mlflow_exception
 @_disable_unless_serve_artifacts
 def _complete_multipart_upload_artifact(artifact_path):
     """
     A request handler for `POST /mlflow-artifacts/mpu/complete` to complete a multipart upload
     to `artifact_path` (a relative path from the root artifact directory).
     """
-    validate_path_is_safe(artifact_path)
+    artifact_path = validate_path_is_safe(artifact_path)
 
     request_message = _get_request_message(
         CompleteMultipartUpload(),
         schema={
             "path": [_assert_required, _assert_string],
             "upload_id": [_assert_string],
             "parts": [_assert_required],
@@ -2041,15 +2042,15 @@
 @catch_mlflow_exception
 @_disable_unless_serve_artifacts
 def _abort_multipart_upload_artifact(artifact_path):
     """
     A request handler for `POST /mlflow-artifacts/mpu/abort` to abort a multipart upload
     to `artifact_path` (a relative path from the root artifact directory).
     """
-    validate_path_is_safe(artifact_path)
+    artifact_path = validate_path_is_safe(artifact_path)
 
     request_message = _get_request_message(
         AbortMultipartUpload(),
         schema={
             "path": [_assert_required, _assert_string],
             "upload_id": [_assert_string],
         },
```

### Comparing `mlflow-skinny-2.9.1/mlflow/server/validation.py` & `mlflow-skinny-2.9.2/mlflow/server/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/shap/__init__.py` & `mlflow-skinny-2.9.2/mlflow/shap/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/sklearn/__init__.py` & `mlflow-skinny-2.9.2/mlflow/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/sklearn/utils.py` & `mlflow-skinny-2.9.2/mlflow/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/spacy/__init__.py` & `mlflow-skinny-2.9.2/mlflow/spacy/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/spark/__init__.py` & `mlflow-skinny-2.9.2/mlflow/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/statsmodels/__init__.py` & `mlflow-skinny-2.9.2/mlflow/statsmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/registry/rest_store.py` & `mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/_unity_catalog/registry/utils.py` & `mlflow-skinny-2.9.2/mlflow/store/_unity_catalog/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/artifact_repository_registry.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/artifact_repository_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/azure_blob_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/azure_blob_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/azure_data_lake_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/azure_data_lake_artifact_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import requests
 
 from mlflow.azure.client import patch_adls_file_upload, patch_adls_flush, put_adls_file_creation
 from mlflow.entities import FileInfo
 from mlflow.environment_variables import (
     MLFLOW_ARTIFACT_UPLOAD_DOWNLOAD_TIMEOUT,
     MLFLOW_ENABLE_MULTIPART_UPLOAD,
+    MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE,
 )
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_artifacts_pb2 import ArtifactCredentialInfo
 from mlflow.store.artifact.cloud_artifact_repo import (
-    _MULTIPART_UPLOAD_CHUNK_SIZE,
     CloudArtifactRepository,
     _complete_futures,
     _compute_num_chunks,
 )
 
 
 def _parse_abfss_uri(uri):
@@ -138,15 +138,15 @@
 
     def delete_artifacts(self, artifact_path=None):
         raise NotImplementedError("This artifact repository does not support deleting artifacts")
 
     def _upload_to_cloud(self, cloud_credential_info, src_file_path, artifact_file_path):
         if (
             MLFLOW_ENABLE_MULTIPART_UPLOAD.get()
-            and os.path.getsize(src_file_path) > _MULTIPART_UPLOAD_CHUNK_SIZE
+            and os.path.getsize(src_file_path) > MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
         ):
             self._multipart_upload(cloud_credential_info, src_file_path, artifact_file_path)
         else:
             artifact_subdir = posixpath.dirname(artifact_file_path)
             self.log_artifact(src_file_path, artifact_subdir)
 
     def _retryable_adls_function(self, func, artifact_file_path, **kwargs):
@@ -173,26 +173,28 @@
                 artifact_file_path=artifact_file_path,
                 sas_url=credentials.signed_uri,
                 headers=headers,
             )
             # next try to append the file
             futures = {}
             file_size = os.path.getsize(src_file_path)
-            num_chunks = _compute_num_chunks(src_file_path, _MULTIPART_UPLOAD_CHUNK_SIZE)
+            num_chunks = _compute_num_chunks(
+                src_file_path, MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
+            )
             use_single_part_upload = num_chunks == 1
             for index in range(num_chunks):
-                start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
+                start_byte = index * MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
                 future = self.chunk_thread_pool.submit(
                     self._retryable_adls_function,
                     func=patch_adls_file_upload,
                     artifact_file_path=artifact_file_path,
                     sas_url=credentials.signed_uri,
                     local_file=src_file_path,
                     start_byte=start_byte,
-                    size=_MULTIPART_UPLOAD_CHUNK_SIZE,
+                    size=MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get(),
                     position=start_byte,
                     headers=headers,
                     is_single=use_single_part_upload,
                 )
                 futures[future] = index
 
             _, errors = _complete_futures(futures, src_file_path)
```

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/cli.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/cloud_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/cloud_artifact_repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from abc import abstractmethod
 from collections import namedtuple
 from concurrent.futures import as_completed
 
 from mlflow.environment_variables import (
     MLFLOW_ENABLE_ARTIFACTS_PROGRESS_BAR,
     MLFLOW_ENABLE_MULTIPART_DOWNLOAD,
+    MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE,
+    MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE,
+    MLFLOW_MULTIPART_UPLOAD_MINIMUM_FILE_SIZE,
 )
 from mlflow.exceptions import MlflowException
 from mlflow.store.artifact.artifact_repo import ArtifactRepository
 from mlflow.utils import chunk_list
 from mlflow.utils.file_utils import (
     ArtifactProgressBar,
     download_chunk_retries,
     parallelized_download_file_using_http_uri,
     relative_path_to_artifact_path,
     remove_on_error,
 )
 from mlflow.utils.uri import is_fuse_or_uc_volumes_uri
 
 _logger = logging.getLogger(__name__)
-_DOWNLOAD_CHUNK_SIZE = 100_000_000  # 100 MB
-_MULTIPART_DOWNLOAD_MINIMUM_FILE_SIZE = 500_000_000  # 500 MB
-_MULTIPART_UPLOAD_CHUNK_SIZE = 10_000_000  # 10 MB
 _ARTIFACT_UPLOAD_BATCH_SIZE = (
     50  # Max number of artifacts for which to fetch write credentials at once.
 )
 
 
 def _compute_num_chunks(local_file: os.PathLike, chunk_size: int) -> int:
     """
@@ -47,15 +47,15 @@
     """
     results = {}
     errors = {}
 
     with ArtifactProgressBar.chunks(
         os.path.getsize(file),
         f"Uploading {file}",
-        _MULTIPART_UPLOAD_CHUNK_SIZE,
+        MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get(),
     ) as pbar:
         for future in as_completed(futures_dict):
             key = futures_dict[future]
             try:
                 results[key] = future.result()
                 pbar.update()
             except Exception as e:
@@ -203,15 +203,15 @@
             failed_downloads = parallelized_download_file_using_http_uri(
                 thread_pool_executor=self.chunk_thread_pool,
                 http_uri=cloud_credential_info.signed_uri,
                 download_path=local_path,
                 remote_file_path=remote_file_path,
                 file_size=file_size,
                 uri_type=cloud_credential_info.type,
-                chunk_size=_DOWNLOAD_CHUNK_SIZE,
+                chunk_size=MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE.get(),
                 env=parallel_download_subproc_env,
                 headers=self._extract_headers_from_credentials(cloud_credential_info.headers),
             )
 
             if failed_downloads:
                 new_cloud_creds = self._get_read_credential_infos([remote_file_path])[0]
                 new_signed_uri = new_cloud_creds.signed_uri
@@ -235,15 +235,15 @@
         file_size = file_info[0].file_size if len(file_info) == 1 else None
         # NB: FUSE mounts do not support file write from a non-0th index seek position.
         # Due to this limitation (writes must start at the beginning of a file),
         # offset writes are disabled if FUSE is the local_path destination.
         if (
             not MLFLOW_ENABLE_MULTIPART_DOWNLOAD.get()
             or not file_size
-            or file_size < _MULTIPART_DOWNLOAD_MINIMUM_FILE_SIZE
+            or file_size < MLFLOW_MULTIPART_UPLOAD_MINIMUM_FILE_SIZE.get()
             or is_fuse_or_uc_volumes_uri(local_path)
         ):
             self._download_from_cloud(remote_file_path, local_path)
         else:
             self._parallelized_download_from_cloud(file_size, remote_file_path, local_path)
 
     @abstractmethod
```

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/databricks_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/databricks_artifact_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
     patch_adls_file_upload,
     patch_adls_flush,
     put_adls_file_creation,
     put_block,
     put_block_list,
 )
 from mlflow.entities import FileInfo
+from mlflow.environment_variables import (
+    MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE,
+    MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE,
+)
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_artifacts_pb2 import (
     ArtifactCredentialType,
     CompleteMultipartUpload,
     CreateMultipartUpload,
     DatabricksMlflowArtifactsService,
     GetCredentialsForRead,
@@ -28,16 +32,14 @@
 )
 from mlflow.protos.databricks_pb2 import (
     INTERNAL_ERROR,
     INVALID_PARAMETER_VALUE,
 )
 from mlflow.protos.service_pb2 import GetRun, ListArtifacts, MlflowService
 from mlflow.store.artifact.cloud_artifact_repo import (
-    _DOWNLOAD_CHUNK_SIZE,
-    _MULTIPART_UPLOAD_CHUNK_SIZE,
     CloudArtifactRepository,
     _complete_futures,
     _compute_num_chunks,
 )
 from mlflow.utils import chunk_list
 from mlflow.utils.databricks_utils import get_databricks_host_creds
 from mlflow.utils.file_utils import (
@@ -242,25 +244,25 @@
         is the reason for the first nested try-except block
         Finally, since the prevailing credentials could expire in the time between the last
         stage_block and the commit, a second try-except block refreshes credentials if needed.
         """
         try:
             headers = self._extract_headers_from_credentials(credentials.headers)
             futures = {}
-            num_chunks = _compute_num_chunks(local_file, _MULTIPART_UPLOAD_CHUNK_SIZE)
+            num_chunks = _compute_num_chunks(local_file, MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get())
             for index in range(num_chunks):
-                start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
+                start_byte = index * MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
                 future = self.chunk_thread_pool.submit(
                     self._azure_upload_chunk,
                     credentials=credentials,
                     headers=headers,
                     local_file=local_file,
                     artifact_file_path=artifact_file_path,
                     start_byte=start_byte,
-                    size=_MULTIPART_UPLOAD_CHUNK_SIZE,
+                    size=MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get(),
                 )
                 futures[future] = index
 
             results, errors = _complete_futures(futures, local_file)
             if errors:
                 raise MlflowException(
                     f"Failed to upload at least one part of {local_file}. Errors: {errors}"
@@ -315,26 +317,26 @@
                 sas_url=credentials.signed_uri,
                 headers=headers,
             )
 
             # next try to append the file
             futures = {}
             file_size = os.path.getsize(local_file)
-            num_chunks = _compute_num_chunks(local_file, _MULTIPART_UPLOAD_CHUNK_SIZE)
+            num_chunks = _compute_num_chunks(local_file, MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get())
             use_single_part_upload = num_chunks == 1
             for index in range(num_chunks):
-                start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
+                start_byte = index * MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
                 future = self.chunk_thread_pool.submit(
                     self._retryable_adls_function,
                     func=patch_adls_file_upload,
                     artifact_file_path=artifact_file_path,
                     sas_url=credentials.signed_uri,
                     local_file=local_file,
                     start_byte=start_byte,
-                    size=_MULTIPART_UPLOAD_CHUNK_SIZE,
+                    size=MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get(),
                     position=start_byte,
                     headers=headers,
                     is_single=use_single_part_upload,
                 )
                 futures[future] = index
 
             _, errors = _complete_futures(futures, local_file)
@@ -388,15 +390,15 @@
         if cloud_credential_info.type == ArtifactCredentialType.AZURE_SAS_URI:
             self._azure_upload_file(cloud_credential_info, src_file_path, artifact_file_path)
         elif cloud_credential_info.type == ArtifactCredentialType.AZURE_ADLS_GEN2_SAS_URI:
             self._azure_adls_gen2_upload_file(
                 cloud_credential_info, src_file_path, artifact_file_path
             )
         elif cloud_credential_info.type == ArtifactCredentialType.AWS_PRESIGNED_URL:
-            if os.path.getsize(src_file_path) > _MULTIPART_UPLOAD_CHUNK_SIZE:
+            if os.path.getsize(src_file_path) > MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get():
                 self._multipart_upload(src_file_path, artifact_file_path)
             else:
                 self._signed_url_upload_file(cloud_credential_info, src_file_path)
         elif cloud_credential_info.type == ArtifactCredentialType.GCP_SIGNED_URL:
             self._signed_url_upload_file(cloud_credential_info, src_file_path)
         else:
             raise MlflowException(
@@ -427,15 +429,15 @@
             raise MlflowException(
                 message="Cloud provider not supported.", error_code=INTERNAL_ERROR
             )
         try:
             download_file_using_http_uri(
                 cloud_credential_info.signed_uri,
                 local_path,
-                _DOWNLOAD_CHUNK_SIZE,
+                MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE.get(),
                 self._extract_headers_from_credentials(cloud_credential_info.headers),
             )
         except Exception as err:
             raise MlflowException(err)
 
     def _create_multipart_upload(self, run_id, path, num_parts):
         return self._call_endpoint(
@@ -482,23 +484,23 @@
             )
             return self._upload_part(resp.upload_credential_info, data)
 
     def _upload_parts(self, local_file, create_mpu_resp):
         futures = {}
         for index, cred_info in enumerate(create_mpu_resp.upload_credential_infos):
             part_number = index + 1
-            start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
+            start_byte = index * MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
             future = self.chunk_thread_pool.submit(
                 self._upload_part_retry,
                 cred_info=cred_info,
                 upload_id=create_mpu_resp.upload_id,
                 part_number=part_number,
                 local_file=local_file,
                 start_byte=start_byte,
-                size=_MULTIPART_UPLOAD_CHUNK_SIZE,
+                size=MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get(),
             )
             futures[future] = part_number
 
         results, errors = _complete_futures(futures, local_file)
         if errors:
             raise MlflowException(
                 f"Failed to upload at least one part of {local_file}. Errors: {errors}"
@@ -531,15 +533,15 @@
             augmented_raise_for_status(response)
             return response
 
     def _multipart_upload(self, local_file, artifact_file_path):
         run_relative_artifact_path = posixpath.join(
             self.run_relative_artifact_repo_root_path, artifact_file_path or ""
         )
-        num_parts = _compute_num_chunks(local_file, _MULTIPART_UPLOAD_CHUNK_SIZE)
+        num_parts = _compute_num_chunks(local_file, MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get())
         create_mpu_resp = self._create_multipart_upload(
             self.run_id, run_relative_artifact_path, num_parts
         )
         try:
             part_etags = self._upload_parts(local_file, create_mpu_resp)
             self._complete_multipart_upload(
                 self.run_id,
```

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/databricks_models_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/databricks_models_artifact_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 import logging
 import os
 import posixpath
 
 import mlflow.tracking
 from mlflow.entities import FileInfo
-from mlflow.environment_variables import MLFLOW_ENABLE_MULTIPART_DOWNLOAD
+from mlflow.environment_variables import (
+    MLFLOW_ENABLE_MULTIPART_DOWNLOAD,
+    MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE,
+)
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_pb2 import INVALID_PARAMETER_VALUE
 from mlflow.store.artifact.artifact_repo import ArtifactRepository
 from mlflow.store.artifact.utils.models import (
     get_model_name_and_version,
     is_using_databricks_registry,
 )
@@ -23,15 +26,14 @@
     parallelized_download_file_using_http_uri,
     remove_on_error,
 )
 from mlflow.utils.rest_utils import http_request
 from mlflow.utils.uri import get_databricks_profile_uri_from_artifact_uri
 
 _logger = logging.getLogger(__name__)
-_DOWNLOAD_CHUNK_SIZE = 100_000_000  # 100 MB
 # The constant REGISTRY_LIST_ARTIFACT_ENDPOINT is defined as @developer_stable
 REGISTRY_LIST_ARTIFACTS_ENDPOINT = "/api/2.0/mlflow/model-versions/list-artifacts"
 # The constant REGISTRY_ARTIFACT_PRESIGNED_URI_ENDPOINT is defined as @developer_stable
 REGISTRY_ARTIFACT_PRESIGNED_URI_ENDPOINT = "/api/2.0/mlflow/model-versions/get-signed-download-uri"
 
 
 class DatabricksModelsArtifactRepository(ArtifactRepository):
@@ -150,15 +152,15 @@
                 thread_pool_executor=self.chunk_thread_pool,
                 http_uri=signed_uri,
                 download_path=dst_local_file_path,
                 remote_file_path=dst_run_relative_artifact_path,
                 file_size=file_size,
                 # URI type is not known in this context
                 uri_type=None,
-                chunk_size=_DOWNLOAD_CHUNK_SIZE,
+                chunk_size=MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE.get(),
                 env=parallel_download_subproc_env,
                 headers=headers,
             )
             if failed_downloads:
                 new_signed_uri, new_headers = self._get_signed_download_uri(
                     dst_run_relative_artifact_path
                 )
@@ -179,18 +181,20 @@
             signed_uri, raw_headers = self._get_signed_download_uri(remote_file_path)
             headers = {}
             if raw_headers is not None:
                 # Don't send None to _extract_headers_from_signed_url
                 headers = self._extract_headers_from_signed_url(raw_headers)
             if (
                 not file_size
-                or file_size <= _DOWNLOAD_CHUNK_SIZE
+                or file_size <= MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE.get()
                 or not MLFLOW_ENABLE_MULTIPART_DOWNLOAD.get()
             ):
-                download_file_using_http_uri(signed_uri, local_path, _DOWNLOAD_CHUNK_SIZE, headers)
+                download_file_using_http_uri(
+                    signed_uri, local_path, MLFLOW_MULTIPART_DOWNLOAD_CHUNK_SIZE.get(), headers
+                )
             else:
                 self._parallelized_download_from_cloud(
                     signed_uri,
                     headers,
                     file_size,
                     local_path,
                     remote_file_path,
```

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/dbfs_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/dbfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/ftp_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/ftp_artifact_repo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -102,18 +102,18 @@
     def list_artifacts(self, path=None):
         with self.get_ftp_client() as ftp:
             artifact_dir = self.path
             list_dir = posixpath.join(artifact_dir, path) if path else artifact_dir
             if not self._is_dir(ftp, list_dir):
                 return []
             artifact_files = ftp.nlst(list_dir)
-            artifact_files = list(filter(lambda x: x != "." and x != "..", artifact_files))
             # Make sure artifact_files is a list of file names because ftp.nlst
             # may return absolute paths.
             artifact_files = [os.path.basename(f) for f in artifact_files]
+            artifact_files = list(filter(lambda x: x != "." and x != "..", artifact_files))
             infos = []
             for file_name in artifact_files:
                 file_path = file_name if path is None else posixpath.join(path, file_name)
                 full_file_path = posixpath.join(list_dir, file_name)
                 if self._is_dir(ftp, full_file_path):
                     infos.append(FileInfo(file_path, True, None))
                 else:
```

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/gcs_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/gcs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/hdfs_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/hdfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/http_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/http_artifact_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,17 @@
         root = tail.lstrip("/")
         params = {"path": posixpath.join(root, path) if path else root}
         host_creds = _get_default_host_creds(url)
         resp = http_request(host_creds, endpoint, "GET", params=params)
         augmented_raise_for_status(resp)
         file_infos = []
         for f in resp.json().get("files", []):
-            validate_path_is_safe(f["path"])
+            validated_path = validate_path_is_safe(f["path"])
             file_info = FileInfo(
-                posixpath.join(path, f["path"]) if path else f["path"],
+                posixpath.join(path, validated_path) if path else validated_path,
                 f["is_dir"],
                 int(f["file_size"]) if ("file_size" in f) else None,
             )
             file_infos.append(file_info)
 
         return sorted(file_infos, key=lambda f: f.path)
```

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/local_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/local_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/mlflow_artifacts_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/mlflow_artifacts_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/models_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/optimized_s3_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/optimized_s3_artifact_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import posixpath
 import urllib.parse
 from mimetypes import guess_type
 
 from mlflow.entities import FileInfo
 from mlflow.environment_variables import (
     MLFLOW_ENABLE_MULTIPART_UPLOAD,
+    MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE,
     MLFLOW_S3_UPLOAD_EXTRA_ARGS,
 )
 from mlflow.exceptions import MlflowException
 from mlflow.protos.databricks_artifacts_pb2 import ArtifactCredentialInfo
 from mlflow.store.artifact.cloud_artifact_repo import (
-    _MULTIPART_UPLOAD_CHUNK_SIZE,
     CloudArtifactRepository,
     _complete_futures,
 )
 from mlflow.store.artifact.s3_artifact_repo import _get_s3_client
 from mlflow.utils.file_utils import read_chunk
 from mlflow.utils.request_utils import cloud_storage_http_request
 from mlflow.utils.rest_utils import augmented_raise_for_status
@@ -123,28 +123,30 @@
         return [self._get_s3_client() for _ in remote_file_paths]
 
     def _upload_to_cloud(self, cloud_credential_info, src_file_path, artifact_file_path):
         dest_path = posixpath.join(self.bucket_path, artifact_file_path)
         key = posixpath.normpath(dest_path)
         if (
             MLFLOW_ENABLE_MULTIPART_UPLOAD.get()
-            and os.path.getsize(src_file_path) > _MULTIPART_UPLOAD_CHUNK_SIZE
+            and os.path.getsize(src_file_path) > MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
         ):
             self._multipart_upload(cloud_credential_info, src_file_path, self.bucket, key)
         else:
             self._upload_file(cloud_credential_info, src_file_path, self.bucket, key)
 
     def _multipart_upload(self, cloud_credential_info, local_file, bucket, key):
         # Create multipart upload
         s3_client = cloud_credential_info
         response = s3_client.create_multipart_upload(Bucket=bucket, Key=key)
         upload_id = response["UploadId"]
 
         # Create presigned URL for each part
-        num_parts = math.ceil(os.path.getsize(local_file) / _MULTIPART_UPLOAD_CHUNK_SIZE)
+        num_parts = math.ceil(
+            os.path.getsize(local_file) / MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
+        )
 
         # define helper functions for uploading data
         def _upload_part(part_number, local_file, start_byte, size):
             presigned_url = s3_client.generate_presigned_url(
                 "upload_part",
                 Params={
                     "Bucket": bucket,
@@ -159,21 +161,21 @@
                 return response.headers["ETag"]
 
         try:
             # Upload each part with retries
             futures = {}
             for index in range(num_parts):
                 part_number = index + 1
-                start_byte = index * _MULTIPART_UPLOAD_CHUNK_SIZE
+                start_byte = index * MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get()
                 future = self.chunk_thread_pool.submit(
                     _upload_part,
                     part_number=part_number,
                     local_file=local_file,
                     start_byte=start_byte,
-                    size=_MULTIPART_UPLOAD_CHUNK_SIZE,
+                    size=MLFLOW_MULTIPART_UPLOAD_CHUNK_SIZE.get(),
                 )
                 futures[future] = part_number
 
             results, errors = _complete_futures(futures, local_file)
             if errors:
                 raise MlflowException(
                     f"Failed to upload at least one part of {local_file}. Errors: {errors}"
```

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/r2_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/r2_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/runs_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/runs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/s3_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/s3_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/sftp_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/sftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/unity_catalog_models_artifact_repo.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/unity_catalog_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/artifact/utils/models.py` & `mlflow-skinny-2.9.2/mlflow/store/artifact/utils/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db/utils.py` & `mlflow-skinny-2.9.2/mlflow/store/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/alembic.ini` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/env.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/2d6e25af4d3e_increase_max_param_val_length.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/2d6e25af4d3e_increase_max_param_val_length.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/acf3f17fdcc7_add_storage_location_field_to_model_.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/acf3f17fdcc7_add_storage_location_field_to_model_.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py` & `mlflow-skinny-2.9.2/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/__init__.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/abstract_store.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/base_rest_store.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/base_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/databricks_workspace_model_registry_rest_store.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/databricks_workspace_model_registry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/dbmodels/models.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/file_store.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/rest_store.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/model_registry/sqlalchemy_store.py` & `mlflow-skinny-2.9.2/mlflow/store/model_registry/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/tracking/__init__.py` & `mlflow-skinny-2.9.2/mlflow/store/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/tracking/abstract_store.py` & `mlflow-skinny-2.9.2/mlflow/store/tracking/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/tracking/dbmodels/initial_models.py` & `mlflow-skinny-2.9.2/mlflow/store/tracking/dbmodels/initial_models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/tracking/dbmodels/models.py` & `mlflow-skinny-2.9.2/mlflow/store/tracking/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/tracking/file_store.py` & `mlflow-skinny-2.9.2/mlflow/store/tracking/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/tracking/rest_store.py` & `mlflow-skinny-2.9.2/mlflow/store/tracking/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/store/tracking/sqlalchemy_store.py` & `mlflow-skinny-2.9.2/mlflow/store/tracking/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/system_metrics/__init__.py` & `mlflow-skinny-2.9.2/mlflow/system_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/base_metrics_monitor.py` & `mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/base_metrics_monitor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/cpu_monitor.py` & `mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/cpu_monitor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/disk_monitor.py` & `mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/disk_monitor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/gpu_monitor.py` & `mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/system_metrics/metrics/network_monitor.py` & `mlflow-skinny-2.9.2/mlflow/system_metrics/metrics/network_monitor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/system_metrics/system_metrics_monitor.py` & `mlflow-skinny-2.9.2/mlflow/system_metrics/system_metrics_monitor.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tensorflow/__init__.py` & `mlflow-skinny-2.9.2/mlflow/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tensorflow/_autolog.py` & `mlflow-skinny-2.9.2/mlflow/tensorflow/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tensorflow/callback.py` & `mlflow-skinny-2.9.2/mlflow/tensorflow/callback.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/__init__.py` & `mlflow-skinny-2.9.2/mlflow/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/client.py` & `mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/fluent.py` & `mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/registry.py` & `mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/_model_registry/utils.py` & `mlflow-skinny-2.9.2/mlflow/tracking/_model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/client.py` & `mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/registry.py` & `mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/_tracking_service/utils.py` & `mlflow-skinny-2.9.2/mlflow/tracking/_tracking_service/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/artifact_utils.py` & `mlflow-skinny-2.9.2/mlflow/tracking/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/client.py` & `mlflow-skinny-2.9.2/mlflow/tracking/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/abstract_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_cluster_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_cluster_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_command_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_command_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_job_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_job_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_notebook_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_notebook_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/databricks_repo_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/databricks_repo_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/default_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/default_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/git_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/git_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/context/registry.py` & `mlflow-skinny-2.9.2/mlflow/tracking/context/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/abstract_context.py` & `mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py` & `mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/default_experiment/registry.py` & `mlflow-skinny-2.9.2/mlflow/tracking/default_experiment/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/fluent.py` & `mlflow-skinny-2.9.2/mlflow/tracking/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/llm_utils.py` & `mlflow-skinny-2.9.2/mlflow/tracking/llm_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/metric_value_conversion_utils.py` & `mlflow-skinny-2.9.2/mlflow/tracking/metric_value_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/registry.py` & `mlflow-skinny-2.9.2/mlflow/tracking/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/request_auth/abstract_request_auth_provider.py` & `mlflow-skinny-2.9.2/mlflow/tracking/request_auth/abstract_request_auth_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/request_auth/registry.py` & `mlflow-skinny-2.9.2/mlflow/tracking/request_auth/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/request_header/abstract_request_header_provider.py` & `mlflow-skinny-2.9.2/mlflow/tracking/request_header/abstract_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/request_header/databricks_request_header_provider.py` & `mlflow-skinny-2.9.2/mlflow/tracking/request_header/databricks_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/tracking/request_header/registry.py` & `mlflow-skinny-2.9.2/mlflow/tracking/request_header/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/transformers/__init__.py` & `mlflow-skinny-2.9.2/mlflow/transformers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from functools import lru_cache
 from typing import Any, Dict, List, NamedTuple, Optional, Union
 from urllib.parse import urlparse
 
 import numpy as np
 import pandas as pd
 import yaml
+from packaging.version import Version
 
 from mlflow import pyfunc
 from mlflow.environment_variables import (
     MLFLOW_DEFAULT_PREDICTION_DEVICE,
     MLFLOW_HUGGINGFACE_DEVICE_MAP_STRATEGY,
     MLFLOW_HUGGINGFACE_DISABLE_ACCELERATE_FEATURES,
     MLFLOW_HUGGINGFACE_MODEL_MAX_SHARD_SIZE,
@@ -2718,15 +2719,23 @@
         with disable_discrete_autologging(DISABLED_ANCILLARY_FLAVOR_AUTOLOGGING):
             return original(*args, **kwargs)
 
     with contextlib.suppress(ImportError):
         import setfit
 
         safe_patch(
-            FLAVOR_NAME, setfit.SetFitTrainer, "train", functools.partial(train), manage_run=False
+            FLAVOR_NAME,
+            (
+                setfit.SetFitTrainer
+                if Version(setfit.__version__) < Version("1.0.0")
+                else setfit.Trainer
+            ),
+            "train",
+            functools.partial(train),
+            manage_run=False,
         )
 
     with contextlib.suppress(ImportError):
         import transformers
 
         classes = [transformers.Trainer, transformers.Seq2SeqTrainer]
         methods = ["train"]
```

### Comparing `mlflow-skinny-2.9.1/mlflow/types/schema.py` & `mlflow-skinny-2.9.2/mlflow/types/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/types/utils.py` & `mlflow-skinny-2.9.2/mlflow/types/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/__init__.py` & `mlflow-skinny-2.9.2/mlflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/_capture_modules.py` & `mlflow-skinny-2.9.2/mlflow/utils/_capture_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/_capture_transformers_modules.py` & `mlflow-skinny-2.9.2/mlflow/utils/_capture_transformers_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/_spark_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/_spark_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/annotations.py` & `mlflow-skinny-2.9.2/mlflow/utils/annotations.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/async_logging/async_logging_queue.py` & `mlflow-skinny-2.9.2/mlflow/utils/async_logging/async_logging_queue.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/async_logging/run_batch.py` & `mlflow-skinny-2.9.2/mlflow/utils/async_logging/run_batch.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/async_logging/run_operations.py` & `mlflow-skinny-2.9.2/mlflow/utils/async_logging/run_operations.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/__init__.py` & `mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/client.py` & `mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/client.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/events.py` & `mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/events.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/logging_and_warnings.py` & `mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/logging_and_warnings.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/metrics_queue.py` & `mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/metrics_queue.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/safety.py` & `mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/safety.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/autologging_utils/versioning.py` & `mlflow-skinny-2.9.2/mlflow/utils/autologging_utils/versioning.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/cli_args.py` & `mlflow-skinny-2.9.2/mlflow/utils/cli_args.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/conda.py` & `mlflow-skinny-2.9.2/mlflow/utils/conda.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/credentials.py` & `mlflow-skinny-2.9.2/mlflow/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/databricks_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/docstring_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/download_cloud_file_chunk.py` & `mlflow-skinny-2.9.2/mlflow/utils/download_cloud_file_chunk.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/environment.py` & `mlflow-skinny-2.9.2/mlflow/utils/environment.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/file_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,26 +325,27 @@
     result as a dictionary.
 
     :param root: Root directory of the YAML files
     :param template_name: Name of the template file
     :param context_name: Name of the context file
     :return: Data in yaml file as dictionary
     """
-    import jinja2
+    from jinja2 import FileSystemLoader, StrictUndefined
+    from jinja2.sandbox import SandboxedEnvironment
 
     template_path = os.path.join(root, template_name)
     context_path = os.path.join(root, context_name)
 
     for path in (template_path, context_path):
         if not pathlib.Path(path).is_file():
             raise MissingConfigException(f"Yaml file '{path}' does not exist.")
 
-    j2_env = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(root, encoding=ENCODING),
-        undefined=jinja2.StrictUndefined,
+    j2_env = SandboxedEnvironment(
+        loader=FileSystemLoader(root, encoding=ENCODING),
+        undefined=StrictUndefined,
         line_comment_prefix="#",
     )
 
     def from_json(input_var):
         with open(input_var, encoding="utf-8") as f:
             return json.load(f)
```

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/git_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/gorilla.py` & `mlflow-skinny-2.9.2/mlflow/utils/gorilla.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/import_hooks/__init__.py` & `mlflow-skinny-2.9.2/mlflow/utils/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/insecure_hash.py` & `mlflow-skinny-2.9.2/mlflow/utils/insecure_hash.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/lazy_load.py` & `mlflow-skinny-2.9.2/mlflow/utils/lazy_load.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/logging_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/mime_type_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/mime_type_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/mlflow_tags.py` & `mlflow-skinny-2.9.2/mlflow/utils/mlflow_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/model_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/name_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/name_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/nfs_on_spark.py` & `mlflow-skinny-2.9.2/mlflow/utils/nfs_on_spark.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/process.py` & `mlflow-skinny-2.9.2/mlflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/promptlab_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/promptlab_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/proto_json_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/request_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/request_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -161,14 +161,15 @@
     method,
     url,
     max_retries,
     backoff_factor,
     backoff_jitter,
     retry_codes,
     raise_on_status=True,
+    allow_redirects=None,
     **kwargs,
 ):
     """
     Performs an HTTP request using Python's `requests` module with an automatic retry policy.
 
     :param method: a string indicating the method to use, e.g. "GET", "POST", "PUT".
     :param url: the target URL address for the HTTP request.
@@ -183,15 +184,21 @@
     :param kwargs: Additional keyword arguments to pass to `requests.Session.request()`
 
     :return: requests.Response object.
     """
     session = _get_request_session(
         max_retries, backoff_factor, backoff_jitter, retry_codes, raise_on_status
     )
-    return session.request(method, url, **kwargs)
+
+    # the environment variable is hardcoded here to avoid importing mlflow.
+    # however, documentation is available in environment_variables.py
+    env_value = os.getenv("MLFLOW_ALLOW_HTTP_REDIRECTS", "true").lower() in ["true", "1"]
+    allow_redirects = env_value if allow_redirects is None else allow_redirects
+
+    return session.request(method, url, allow_redirects=allow_redirects, **kwargs)
 
 
 def cloud_storage_http_request(
     method,
     url,
     max_retries=5,
     backoff_factor=2,
```

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/requirements_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/requirements_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/rest_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/search_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/server_cli_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/server_cli_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/string_utils.py` & `mlflow-skinny-2.9.2/mlflow/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/time.py` & `mlflow-skinny-2.9.2/mlflow/utils/time.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/uri.py` & `mlflow-skinny-2.9.2/mlflow/utils/uri.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,14 +257,19 @@
     >>> assert uri2 == "a/posixpath/some/subpath"
     """
     path = ""
     for subpath in paths:
         path = _join_posixpaths_and_append_absolute_suffixes(path, subpath)
 
     parsed_uri = urllib.parse.urlparse(uri)
+
+    # Validate query string not to contain any traveral path (../) before appending
+    # to the end of the path, otherwise they will be resolved as part of the path.
+    validate_query_string(parsed_uri.query)
+
     if len(parsed_uri.scheme) == 0:
         # If the input URI does not define a scheme, we assume that it is a POSIX path
         # and join it with the specified input paths
         return _join_posixpaths_and_append_absolute_suffixes(uri, path)
 
     prefix = ""
     if not parsed_uri.path.startswith("/"):
@@ -423,17 +428,45 @@
     A valid path should:
         not contain separators other than '/'
         not contain .. to navigate to parent dir in path
         not be an absolute path
     """
     from mlflow.utils.file_utils import local_file_uri_to_path
 
+    # We must decode path before validating it
+    path = _decode(path)
+
+    exc = MlflowException("Invalid path", error_code=INVALID_PARAMETER_VALUE)
+    if "#" in path:
+        raise exc
+
     if is_file_uri(path):
         path = local_file_uri_to_path(path)
     if (
         any((s in path) for s in _OS_ALT_SEPS)
         or ".." in path.split("/")
         or pathlib.PureWindowsPath(path).is_absolute()
         or pathlib.PurePosixPath(path).is_absolute()
         or (is_windows() and len(path) >= 2 and path[1] == ":")
     ):
-        raise MlflowException(f"Invalid path: {path}", error_code=INVALID_PARAMETER_VALUE)
+        raise exc
+
+    return path
+
+
+def validate_query_string(query):
+    query = _decode(query)
+    # Block query strings contain any traveral path (../) because they
+    # could be resolved as part of the path and allow path traversal.
+    if ".." in query:
+        raise MlflowException("Invalid query string", error_code=INVALID_PARAMETER_VALUE)
+
+
+def _decode(url):
+    # Keep decoding until the url stops changing (with a max of 10 iterations)
+    for _ in range(10):
+        decoded = urllib.parse.unquote(url)
+        if decoded == url:
+            return url
+        url = decoded
+
+    raise ValueError("Failed to decode url")
```

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/validation.py` & `mlflow-skinny-2.9.2/mlflow/utils/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/utils/virtualenv.py` & `mlflow-skinny-2.9.2/mlflow/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/xgboost/__init__.py` & `mlflow-skinny-2.9.2/mlflow/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow/xgboost/_autolog.py` & `mlflow-skinny-2.9.2/mlflow/xgboost/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/mlflow_skinny.egg-info/PKG-INFO` & `mlflow-skinny-2.9.2/mlflow_skinny.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-skinny
-Version: 2.9.1
+Version: 2.9.2
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow-skinny-2.9.1/mlflow_skinny.egg-info/SOURCES.txt` & `mlflow-skinny-2.9.2/mlflow_skinny.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 mlflow/deployments/cli.py
 mlflow/deployments/constants.py
 mlflow/deployments/interface.py
 mlflow/deployments/plugin_manager.py
 mlflow/deployments/utils.py
 mlflow/deployments/databricks/__init__.py
 mlflow/deployments/mlflow/__init__.py
+mlflow/deployments/openai/__init__.py
 mlflow/deployments/server/__init__.py
 mlflow/deployments/server/app.py
 mlflow/deployments/server/config.py
 mlflow/deployments/server/constants.py
 mlflow/deployments/server/runner.py
 mlflow/diviner/__init__.py
 mlflow/entities/__init__.py
@@ -164,15 +165,14 @@
 mlflow/models/evaluation/evaluator_registry.py
 mlflow/models/evaluation/lift_curve.py
 mlflow/models/evaluation/validation.py
 mlflow/onnx/__init__.py
 mlflow/openai/__init__.py
 mlflow/openai/api_request_parallel_processor.py
 mlflow/openai/retry.py
-mlflow/openai/utils.py
 mlflow/paddle/__init__.py
 mlflow/paddle/_paddle_autolog.py
 mlflow/pmdarima/__init__.py
 mlflow/projects/__init__.py
 mlflow/projects/_project_spec.py
 mlflow/projects/databricks.py
 mlflow/projects/docker.py
@@ -442,14 +442,15 @@
 mlflow/utils/lazy_load.py
 mlflow/utils/logging_utils.py
 mlflow/utils/mime_type_utils.py
 mlflow/utils/mlflow_tags.py
 mlflow/utils/model_utils.py
 mlflow/utils/name_utils.py
 mlflow/utils/nfs_on_spark.py
+mlflow/utils/openai_utils.py
 mlflow/utils/os.py
 mlflow/utils/process.py
 mlflow/utils/promptlab_utils.py
 mlflow/utils/proto_json_utils.py
 mlflow/utils/request_utils.py
 mlflow/utils/requirements_utils.py
 mlflow/utils/rest_utils.py
```

### Comparing `mlflow-skinny-2.9.1/mlflow_skinny.egg-info/requires.txt` & `mlflow-skinny-2.9.2/mlflow_skinny.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -35,21 +35,23 @@
 [gateway]
 pydantic<3,>=1.0
 fastapi<1
 uvicorn[standard]<1
 watchfiles<1
 aiohttp<4
 boto3<2,>=1.28.56
+tiktoken<1
 
 [genai]
 pydantic<3,>=1.0
 fastapi<1
 uvicorn[standard]<1
 watchfiles<1
 aiohttp<4
 boto3<2,>=1.28.56
+tiktoken<1
 
 [sqlserver]
 mlflow-dbstore
 
 [xethub]
 mlflow-xethub
```

### Comparing `mlflow-skinny-2.9.1/pylint_plugins/assign_checker.py` & `mlflow-skinny-2.9.2/pylint_plugins/assign_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/pylint_plugins/errors.py` & `mlflow-skinny-2.9.2/pylint_plugins/errors.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/pylint_plugins/import_checker.py` & `mlflow-skinny-2.9.2/pylint_plugins/import_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow-skinny-2.9.1/requirements/core-requirements.txt` & `mlflow-skinny-2.9.2/requirements/core-requirements.txt`

 * *Files identical despite different names*

