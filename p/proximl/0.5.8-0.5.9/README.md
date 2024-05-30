# Comparing `tmp/proximl-0.5.8.tar.gz` & `tmp/proximl-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proximl-0.5.8.tar", last modified: Mon May  6 15:16:30 2024, max compression
+gzip compressed data, was "proximl-0.5.9.tar", last modified: Tue May 14 00:35:54 2024, max compression
```

## Comparing `proximl-0.5.8.tar` & `proximl-0.5.9.tar`

### file list

```diff
@@ -1,126 +1,148 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.341098 proximl-0.5.8/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-05-06 15:15:25.000000 proximl-0.5.8/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-05-06 15:16:30.340949 proximl-0.5.8/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-05-06 15:15:25.000000 proximl-0.5.8/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.322954 proximl-0.5.8/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-05-06 15:15:25.000000 proximl-0.5.8/examples/training_inference_pipeline.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.326257 proximl-0.5.8/proximl/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8667 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.328879 proximl-0.5.8/proximl/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.329991 proximl-0.5.8/proximl/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/data_connector.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/cloudbender/service.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.330268 proximl-0.5.8/proximl/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cli/volume.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.331869 proximl-0.5.8/proximl/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/data_connectors.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/cloudbender/services.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8477 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8161 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6585 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-05-06 15:15:25.000000 proximl-0.5.8/proximl/volumes.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.327087 proximl-0.5.8/proximl.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3619 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-05-06 15:16:30.000000 proximl-0.5.8/proximl.egg-info/top_level.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-05-06 15:15:25.000000 proximl-0.5.8/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-05-06 15:16:30.341146 proximl-0.5.8/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-05-06 15:15:25.000000 proximl-0.5.8/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.321222 proximl-0.5.8/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.333292 proximl-0.5.8/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.333549 proximl-0.5.8/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/integration/test_volumes_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.336503 proximl-0.5.8/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.337892 proximl-0.5.8/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.338787 proximl-0.5.8/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_project_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cli/test_cli_volume_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:16:30.340722 proximl-0.5.8/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/cloudbender/test_services_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10743 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-05-06 15:15:25.000000 proximl-0.5.8/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.486497 proximl-0.5.9/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-05-14 00:34:50.000000 proximl-0.5.9/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-05-14 00:35:54.486353 proximl-0.5.9/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-05-14 00:34:50.000000 proximl-0.5.9/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.466962 proximl-0.5.9/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-05-14 00:34:50.000000 proximl-0.5.9/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-05-14 00:34:50.000000 proximl-0.5.9/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-05-14 00:34:50.000000 proximl-0.5.9/examples/training_inference_pipeline.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.469601 proximl-0.5.9/proximl/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8667 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.471598 proximl-0.5.9/proximl/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.472668 proximl-0.5.9/proximl/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      592 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3606 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/data_connector.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3147 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/cloudbender/service.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.472932 proximl-0.5.9/proximl/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/model.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.473410 proximl-0.5.9/proximl/cli/project/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3402 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/project/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3203 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/project/key.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1621 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/project/secret.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.474788 proximl-0.5.9/proximl/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      717 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3297 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/data_connectors.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5126 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/cloudbender/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8477 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    18056 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8161 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/models.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.475828 proximl-0.5.9/proximl/projects/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       75 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/projects/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1662 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/projects/data_connectors.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1560 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/projects/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2157 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/projects/keys.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2755 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/projects/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2157 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/projects/secrets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1679 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/projects/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8312 2024-05-14 00:34:50.000000 proximl-0.5.9/proximl/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.470353 proximl-0.5.9/proximl.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-05-14 00:35:54.000000 proximl-0.5.9/proximl.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4389 2024-05-14 00:35:54.000000 proximl-0.5.9/proximl.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-05-14 00:35:54.000000 proximl-0.5.9/proximl.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-05-14 00:35:54.000000 proximl-0.5.9/proximl.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-05-14 00:35:54.000000 proximl-0.5.9/proximl.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-05-14 00:35:54.000000 proximl-0.5.9/proximl.egg-info/top_level.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1037 2024-05-14 00:34:50.000000 proximl-0.5.9/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-05-14 00:35:54.486541 proximl-0.5.9/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-05-14 00:34:50.000000 proximl-0.5.9/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.465450 proximl-0.5.9/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.477028 proximl-0.5.9/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.477300 proximl-0.5.9/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/conftest.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.478006 proximl-0.5.9/tests/integration/projects/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/projects/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      208 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/projects/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1241 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/projects/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1423 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/projects/test_projects_keys_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1478 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/projects/test_projects_secrets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    25117 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.480425 proximl-0.5.9/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.482015 proximl-0.5.9/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.483026 proximl-0.5.9/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_service_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.485075 proximl-0.5.9/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5783 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_data_connectors_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5220 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/cloudbender/test_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    33174 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/conftest.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:35:54.486127 proximl-0.5.9/tests/unit/projects/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/projects/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3385 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/projects/test_project_data_connectors_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3129 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/projects/test_project_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3161 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/projects/test_project_keys_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3276 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/projects/test_project_secrets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3331 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/projects/test_project_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3823 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/projects/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_auth_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_proximl_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-05-14 00:34:50.000000 proximl-0.5.9/tests/unit/test_volumes_unit.py
```

### Comparing `proximl-0.5.8/LICENSE` & `proximl-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/PKG-INFO` & `proximl-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.8
+Version: 0.5.9
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.8 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.9 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.8/README.md` & `proximl-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/examples/create_dataset_and_training_job.py` & `proximl-0.5.9/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/examples/local_storage.py` & `proximl-0.5.9/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/examples/training_inference_pipeline.py` & `proximl-0.5.9/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/auth.py` & `proximl-0.5.9/proximl/auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/checkpoints.py` & `proximl-0.5.9/proximl/checkpoints.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/__init__.py` & `proximl-0.5.9/proximl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/checkpoint.py` & `proximl-0.5.9/proximl/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/__init__.py` & `proximl-0.5.9/proximl/cli/cloudbender/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/data_connector.py` & `proximl-0.5.9/proximl/cli/cloudbender/data_connector.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/datastore.py` & `proximl-0.5.9/proximl/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/device.py` & `proximl-0.5.9/proximl/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/node.py` & `proximl-0.5.9/proximl/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/provider.py` & `proximl-0.5.9/proximl/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/region.py` & `proximl-0.5.9/proximl/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/cloudbender/service.py` & `proximl-0.5.9/proximl/cli/cloudbender/service.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/connection.py` & `proximl-0.5.9/proximl/cli/connection.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/dataset.py` & `proximl-0.5.9/proximl/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/environment.py` & `proximl-0.5.9/proximl/cli/environment.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/gpu.py` & `proximl-0.5.9/proximl/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/job/__init__.py` & `proximl-0.5.9/proximl/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/job/create.py` & `proximl-0.5.9/proximl/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/model.py` & `proximl-0.5.9/proximl/cli/model.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cli/project.py` & `proximl-0.5.9/proximl/cli/project/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,7 +143,11 @@
         )
 
     for row in data:
         click.echo(
             "{: >38.36} {: >30.28} {: >30.28} {: >38.36}" "".format(*row),
             file=config.stdout,
         )
+
+
+from proximl.cli.project.secret import secret
+from proximl.cli.project.key import key
```

### Comparing `proximl-0.5.8/proximl/cli/volume.py` & `proximl-0.5.9/proximl/cli/volume.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/cloudbender.py` & `proximl-0.5.9/proximl/cloudbender/cloudbender.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/data_connectors.py` & `proximl-0.5.9/proximl/cloudbender/data_connectors.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/datastores.py` & `proximl-0.5.9/proximl/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/device_configs.py` & `proximl-0.5.9/proximl/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/devices.py` & `proximl-0.5.9/proximl/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/nodes.py` & `proximl-0.5.9/proximl/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/providers.py` & `proximl-0.5.9/proximl/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/regions.py` & `proximl-0.5.9/proximl/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/cloudbender/services.py` & `proximl-0.5.9/proximl/cloudbender/services.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/connections.py` & `proximl-0.5.9/proximl/connections.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/datasets.py` & `proximl-0.5.9/proximl/datasets.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/environments.py` & `proximl-0.5.9/proximl/environments.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/exceptions.py` & `proximl-0.5.9/proximl/exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/gpu_types.py` & `proximl-0.5.9/proximl/gpu_types.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/jobs.py` & `proximl-0.5.9/proximl/jobs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/models.py` & `proximl-0.5.9/proximl/models.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/proximl.py` & `proximl-0.5.9/proximl/proximl.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl/volumes.py` & `proximl-0.5.9/proximl/volumes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/proximl.egg-info/PKG-INFO` & `proximl-0.5.9/proximl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.8
+Version: 0.5.9
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.8 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.9 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.8/proximl.egg-info/SOURCES.txt` & `proximl-0.5.9/proximl.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 proximl/connections.py
 proximl/datasets.py
 proximl/environments.py
 proximl/exceptions.py
 proximl/gpu_types.py
 proximl/jobs.py
 proximl/models.py
-proximl/projects.py
 proximl/proximl.py
 proximl/volumes.py
 proximl.egg-info/PKG-INFO
 proximl.egg-info/SOURCES.txt
 proximl.egg-info/dependency_links.txt
 proximl.egg-info/entry_points.txt
 proximl.egg-info/requires.txt
@@ -29,61 +28,73 @@
 proximl/cli/__init__.py
 proximl/cli/checkpoint.py
 proximl/cli/connection.py
 proximl/cli/dataset.py
 proximl/cli/environment.py
 proximl/cli/gpu.py
 proximl/cli/model.py
-proximl/cli/project.py
 proximl/cli/volume.py
 proximl/cli/cloudbender/__init__.py
 proximl/cli/cloudbender/data_connector.py
 proximl/cli/cloudbender/datastore.py
 proximl/cli/cloudbender/device.py
 proximl/cli/cloudbender/node.py
 proximl/cli/cloudbender/provider.py
 proximl/cli/cloudbender/region.py
 proximl/cli/cloudbender/service.py
 proximl/cli/job/__init__.py
 proximl/cli/job/create.py
+proximl/cli/project/__init__.py
+proximl/cli/project/key.py
+proximl/cli/project/secret.py
 proximl/cloudbender/__init__.py
 proximl/cloudbender/cloudbender.py
 proximl/cloudbender/data_connectors.py
 proximl/cloudbender/datastores.py
 proximl/cloudbender/device_configs.py
 proximl/cloudbender/devices.py
 proximl/cloudbender/nodes.py
 proximl/cloudbender/providers.py
 proximl/cloudbender/regions.py
 proximl/cloudbender/services.py
+proximl/projects/__init__.py
+proximl/projects/data_connectors.py
+proximl/projects/datastores.py
+proximl/projects/keys.py
+proximl/projects/projects.py
+proximl/projects/secrets.py
+proximl/projects/services.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/test_checkpoints_integration.py
 tests/integration/test_datasets_integration.py
 tests/integration/test_environments_integration.py
 tests/integration/test_gpu_types_integration.py
 tests/integration/test_jobs_integration.py
 tests/integration/test_models_integration.py
-tests/integration/test_projects_integration.py
 tests/integration/test_volumes_integration.py
 tests/integration/cloudbender/__init__.py
 tests/integration/cloudbender/test_providers_integration.py
+tests/integration/projects/__init__.py
+tests/integration/projects/conftest.py
+tests/integration/projects/test_projects_integration.py
+tests/integration/projects/test_projects_keys_integration.py
+tests/integration/projects/test_projects_secrets_integration.py
 tests/unit/__init__.py
 tests/unit/conftest.py
-tests/unit/test_auth.py
+tests/unit/test_auth_unit.py
 tests/unit/test_checkpoints_unit.py
 tests/unit/test_connections_unit.py
 tests/unit/test_datasets_unit.py
 tests/unit/test_environments_unit.py
 tests/unit/test_exceptions.py
 tests/unit/test_gpu_types_unit.py
 tests/unit/test_jobs_unit.py
 tests/unit/test_models_unit.py
-tests/unit/test_projects_unit.py
-tests/unit/test_proximl.py
+tests/unit/test_proximl_unit.py
 tests/unit/test_volumes_unit.py
 tests/unit/cli/__init__.py
 tests/unit/cli/conftest.py
 tests/unit/cli/test_cli_checkpoint_unit.py
 tests/unit/cli/test_cli_datasets_unit.py
 tests/unit/cli/test_cli_environment_unit.py
 tests/unit/cli/test_cli_gpu_unit.py
@@ -102,8 +113,15 @@
 tests/unit/cloudbender/test_data_connectors_unit.py
 tests/unit/cloudbender/test_datastores_unit.py
 tests/unit/cloudbender/test_device_configs_unit.py
 tests/unit/cloudbender/test_devices_unit.py
 tests/unit/cloudbender/test_nodes_unit.py
 tests/unit/cloudbender/test_providers_unit.py
 tests/unit/cloudbender/test_regions_unit.py
-tests/unit/cloudbender/test_services_unit.py
+tests/unit/cloudbender/test_services_unit.py
+tests/unit/projects/__init__.py
+tests/unit/projects/test_project_data_connectors_unit.py
+tests/unit/projects/test_project_datastores_unit.py
+tests/unit/projects/test_project_keys_unit.py
+tests/unit/projects/test_project_secrets_unit.py
+tests/unit/projects/test_project_services_unit.py
+tests/unit/projects/test_projects_unit.py
```

### Comparing `proximl-0.5.8/pyproject.toml` & `proximl-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/setup.py` & `proximl-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/cloudbender/test_providers_integration.py` & `proximl-0.5.9/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/conftest.py` & `proximl-0.5.9/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/test_checkpoints_integration.py` & `proximl-0.5.9/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/test_datasets_integration.py` & `proximl-0.5.9/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/test_environments_integration.py` & `proximl-0.5.9/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/test_gpu_types_integration.py` & `proximl-0.5.9/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/test_jobs_integration.py` & `proximl-0.5.9/tests/integration/test_jobs_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/test_models_integration.py` & `proximl-0.5.9/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/integration/test_projects_integration.py` & `proximl-0.5.9/tests/integration/projects/test_projects_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 
 pytestmark = [mark.sdk, mark.integration, mark.projects]
 
 
 @mark.create
 @mark.asyncio
 class GetProjectsTests:
-    @fixture(scope="class")
-    async def project(self, proximl):
-        project = await proximl.projects.create(name="New Project", copy_keys=False)
-        yield project
-        await project.remove()
-
     async def test_get_projects(self, proximl):
         projects = await proximl.projects.list()
         assert len(projects) > 0
 
     async def test_get_project(self, proximl, project):
         response = await proximl.projects.get(project.id)
         assert response.id == project.id
```

### Comparing `proximl-0.5.8/tests/integration/test_volumes_integration.py` & `proximl-0.5.9/tests/integration/test_volumes_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/cloudbender/test_cli_service_unit.py` & `proximl-0.5.9/tests/unit/cli/cloudbender/test_cli_service_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_checkpoint_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_datasets_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_environment_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_gpu_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_job_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_model_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_project_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_project_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cli/test_cli_volume_unit.py` & `proximl-0.5.9/tests/unit/cli/test_cli_volume_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_data_connectors_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_data_connectors_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_datastores_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_device_configs_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_devices_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_nodes_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_providers_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_regions_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/cloudbender/test_services_unit.py` & `proximl-0.5.9/tests/unit/cloudbender/test_services_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/conftest.py` & `proximl-0.5.9/tests/unit/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 from proximl.gpu_types import GpuType, GpuTypes
 from proximl.environments import Environment, Environments
 from proximl.jobs import Job, Jobs
 from proximl.connections import Connections
 from proximl.projects import (
     Projects,
     Project,
-    ProjectDatastore,
-    ProjectService,
 )
+from proximl.projects.datastores import ProjectDatastore
+from proximl.projects.services import ProjectService
+from proximl.projects.data_connectors import ProjectDataConnector
+
 from proximl.cloudbender import Cloudbender
 from proximl.cloudbender.providers import Provider, Providers
 from proximl.cloudbender.regions import Region, Regions
 from proximl.cloudbender.nodes import Node, Nodes
 from proximl.cloudbender.devices import Device, Devices
 from proximl.cloudbender.datastores import Datastore, Datastores
 from proximl.cloudbender.services import Service, Services
+from proximl.cloudbender.data_connectors import DataConnector, DataConnectors
 from proximl.cloudbender.device_configs import DeviceConfig, DeviceConfigs
 
 
 pytestmark = mark.unit
 
 
 @fixture(scope="session")
@@ -945,14 +948,76 @@
                 "hostname": "service-b.local",
             },
         ),
     ]
 
 
 @fixture(scope="session")
+def mock_data_connectors():
+    proximl = Mock()
+    yield [
+        DataConnector(
+            proximl,
+            **{
+                "provider_uuid": "prov-id-1",
+                "region_uuid": "reg-id-1",
+                "connector_id": "con-id-1",
+                "type": "custom",
+                "name": "On-Prem Connection A",
+                "protocol": "TCP",
+                "port_range": "8000-8099",
+                "cidr": "10.0.3.0/24",
+            },
+        ),
+        DataConnector(
+            proximl,
+            **{
+                "provider_uuid": "prov-id-2",
+                "region_uuid": "reg-id-2",
+                "connector_id": "con-id-2",
+                "type": "custom",
+                "name": "Cloud Connection B",
+                "protocol": "UDP",
+                "port_range": "5000",
+                "cidr": "10.0.2.0/24",
+            },
+        ),
+    ]
+
+
+@fixture(
+    scope="session",
+)
+def mock_project_data_connectors():
+    proximl = Mock()
+    yield [
+        ProjectDataConnector(
+            proximl,
+            **{
+                "project_uuid": "proj-id-1",
+                "region_uuid": "reg-id-1",
+                "id": "con-id-1",
+                "type": "custom",
+                "name": "On-Prem Connection A",
+            },
+        ),
+        ProjectDataConnector(
+            proximl,
+            **{
+                "project_uuid": "proj-id-1",
+                "region_uuid": "reg-id-2",
+                "id": "con-id-2",
+                "type": "custom",
+                "name": "Cloud Connection B",
+            },
+        ),
+    ]
+
+
+@fixture(scope="session")
 def mock_device_configs():
     proximl = Mock()
     yield [
         DeviceConfig(
             proximl,
             **{
                 "provider_uuid": "prov-id-1",
@@ -987,14 +1052,15 @@
     mock_projects,
     mock_providers,
     mock_regions,
     mock_nodes,
     mock_devices,
     mock_datastores,
     mock_services,
+    mock_data_connectors,
     mock_device_configs,
 ):
     proximl = create_autospec(ProxiML)
     proximl.active_project = "proj-id-1"
     proximl.project = "proj-id-1"
     proximl.datasets = create_autospec(Datasets)
     proximl.checkpoints = create_autospec(Checkpoints)
@@ -1026,12 +1092,16 @@
     proximl.cloudbender.nodes.list = AsyncMock(return_value=mock_nodes)
     proximl.cloudbender.devices = create_autospec(Nodes)
     proximl.cloudbender.devices.list = AsyncMock(return_value=mock_devices)
     proximl.cloudbender.datastores = create_autospec(Datastores)
     proximl.cloudbender.datastores.list = AsyncMock(return_value=mock_datastores)
     proximl.cloudbender.services = create_autospec(Services)
     proximl.cloudbender.services.list = AsyncMock(return_value=mock_services)
+    proximl.cloudbender.data_connectors = create_autospec(DataConnectors)
+    proximl.cloudbender.data_connectors.list = AsyncMock(
+        return_value=mock_data_connectors
+    )
     proximl.cloudbender.device_configs = create_autospec(DeviceConfigs)
     proximl.cloudbender.device_configs.list = AsyncMock(
         return_value=mock_device_configs
     )
     yield proximl
```

### Comparing `proximl-0.5.8/tests/unit/test_auth.py` & `proximl-0.5.9/tests/unit/test_auth_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_checkpoints_unit.py` & `proximl-0.5.9/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_connections_unit.py` & `proximl-0.5.9/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_datasets_unit.py` & `proximl-0.5.9/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_environments_unit.py` & `proximl-0.5.9/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_exceptions.py` & `proximl-0.5.9/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_gpu_types_unit.py` & `proximl-0.5.9/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_jobs_unit.py` & `proximl-0.5.9/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_models_unit.py` & `proximl-0.5.9/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_proximl.py` & `proximl-0.5.9/tests/unit/test_proximl_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.8/tests/unit/test_volumes_unit.py` & `proximl-0.5.9/tests/unit/test_volumes_unit.py`

 * *Files identical despite different names*

