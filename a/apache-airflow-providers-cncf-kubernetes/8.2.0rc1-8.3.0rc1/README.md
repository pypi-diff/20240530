# Comparing `tmp/apache_airflow_providers_cncf_kubernetes-8.2.0rc1.tar.gz` & `tmp/apache_airflow_providers_cncf_kubernetes-8.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.2.0rc1.tar", last modified: Tue Apr 30 11:20:04 2024, max compression
+gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.3.0rc1.tar", last modified: Tue May 21 10:24:02 2024, max compression
```

## Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1.tar` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1.tar`

### file list

```diff
@@ -1,57 +1,59 @@
--rw-r--r--   0        0        0     3341 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/LICENSE
--rw-r--r--   0        0        0     1590 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py
--rw-r--r--   0        0        0      785 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0        0        0     4340 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
--rw-r--r--   0        0        0     4094 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/callbacks.py
--rw-r--r--   0        0        0      787 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0        0        0     5780 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0        0        0      787 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
--rw-r--r--   0        0        0    34132 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
--rw-r--r--   0        0        0     1673 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
--rw-r--r--   0        0        0    23564 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
--rw-r--r--   0        0        0    10014 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
--rw-r--r--   0        0        0    17775 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0        0        0    31558 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
--rw-r--r--   0        0        0     2101 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py
--rw-r--r--   0        0        0     5329 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kube_client.py
--rw-r--r--   0        0        0     5225 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kube_config.py
--rw-r--r--   0        0        0      785 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
--rw-r--r--   0        0        0     2567 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
--rw-r--r--   0        0        0     6410 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
--rw-r--r--   0        0        0      787 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0        0        0    15311 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
--rw-r--r--   0        0        0    21432 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/job.py
--rw-r--r--   0        0        0     1269 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0        0        0    51520 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0        0        0     7151 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0        0        0    13262 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0        0        0    24545 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py
--rw-r--r--   0        0        0    11998 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0        0        0    12039 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
--rw-r--r--   0        0        0      785 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
--rw-r--r--   0        0        0     2256 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
--rw-r--r--   0        0        0     2442 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
--rw-r--r--   0        0        0     3020 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
--rw-r--r--   0        0        0     1741 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0        0        0     3460 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
--rw-r--r--   0        0        0      785 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
--rw-r--r--   0        0        0     1873 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
--rw-r--r--   0        0        0     1464 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
--rw-r--r--   0        0        0     1494 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py
--rw-r--r--   0        0        0     5209 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/secret.py
--rw-r--r--   0        0        0      785 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0        0        0     5552 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
--rw-r--r--   0        0        0     2968 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py
--rw-r--r--   0        0        0      785 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py
--rw-r--r--   0        0        0     1266 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0        0        0    13670 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
--rw-r--r--   0        0        0      863 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0        0        0     5195 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0        0        0     1928 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
--rw-r--r--   0        0        0    33608 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0        0        0     2519 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
--rw-r--r--   0        0        0     3178 2024-04-30 11:20:04.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3341 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/LICENSE
+-rw-r--r--   0        0        0     1502 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0        0        0     4340 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+-rw-r--r--   0        0        0     4094 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/callbacks.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/cli/__init__.py
+-rw-r--r--   0        0        0     6984 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/cli/kubernetes_command.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0        0        0     5780 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
+-rw-r--r--   0        0        0    33257 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+-rw-r--r--   0        0        0     1673 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+-rw-r--r--   0        0        0    23442 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+-rw-r--r--   0        0        0    10014 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
+-rw-r--r--   0        0        0    17796 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0        0        0    31879 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0        0        0     2101 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py
+-rw-r--r--   0        0        0     5329 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_client.py
+-rw-r--r--   0        0        0     5225 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_config.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
+-rw-r--r--   0        0        0     2567 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
+-rw-r--r--   0        0        0     6765 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0        0        0    15311 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
+-rw-r--r--   0        0        0    21432 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/job.py
+-rw-r--r--   0        0        0     1269 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0        0        0    51654 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0        0        0     7570 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0        0        0    13262 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0        0        0    24380 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py
+-rw-r--r--   0        0        0    11998 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0        0        0    12039 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
+-rw-r--r--   0        0        0     2256 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
+-rw-r--r--   0        0        0     2442 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
+-rw-r--r--   0        0        0     3020 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
+-rw-r--r--   0        0        0     1741 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0        0        0     3460 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
+-rw-r--r--   0        0        0     1873 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
+-rw-r--r--   0        0        0     1464 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
+-rw-r--r--   0        0        0     1494 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py
+-rw-r--r--   0        0        0     5209 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/secret.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0        0        0     5552 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+-rw-r--r--   0        0        0     2965 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0        0        0     4060 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py
+-rw-r--r--   0        0        0     1266 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0        0        0    13670 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+-rw-r--r--   0        0        0      863 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0        0        0     5195 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0        0        0     1928 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
+-rw-r--r--   0        0        0    33608 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0        0        0     2519 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+-rw-r--r--   0        0        0     3178 2024-05-21 10:24:02.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.3.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/README.rst` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.2.0.rc1``
+Release: ``8.3.0.rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cncf-kubernetes``
@@ -78,8 +78,8 @@
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=28.1.0,<=29.0.0``
 ``kubernetes_asyncio``  ``>=28.1.0,<=29.0.0``
 ``google-re2``          ``>=1.0``
 ======================  =====================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/LICENSE` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "8.2.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "8.3.0"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-cncf-kubernetes:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/callbacks.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/callbacks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,58 +34,36 @@
 from datetime import datetime
 from queue import Empty, Queue
 from typing import TYPE_CHECKING, Any, Sequence
 
 from kubernetes.dynamic import DynamicClient
 from sqlalchemy import select, update
 
-from airflow.providers.cncf.kubernetes.pod_generator import PodMutationHookException, PodReconciliationError
-from airflow.stats import Stats
-
-try:
-    from airflow.cli.cli_config import (
-        ARG_DAG_ID,
-        ARG_EXECUTION_DATE,
-        ARG_OUTPUT_PATH,
-        ARG_SUBDIR,
-        ARG_VERBOSE,
-        ActionCommand,
-        Arg,
-        GroupCommand,
-        lazy_load_command,
-        positive_int,
-    )
-except ImportError:
-    try:
-        from airflow import __version__ as airflow_version
-    except ImportError:
-        from airflow.version import version as airflow_version
-
-    import packaging.version
-
-    from airflow.exceptions import AirflowOptionalProviderFeatureException
-
-    base_version = packaging.version.parse(airflow_version).base_version
-
-    if packaging.version.parse(base_version) < packaging.version.parse("2.7.0"):
-        raise AirflowOptionalProviderFeatureException(
-            "Kubernetes Executor from CNCF Provider should only be used with Airflow 2.7.0+.\n"
-            f"This is Airflow {airflow_version} and Kubernetes and CeleryKubernetesExecutor are "
-            f"available in the 'airflow.executors' package. You should not use "
-            f"the provider's executors in this version of Airflow."
-        )
-    raise
+from airflow.cli.cli_config import (
+    ARG_DAG_ID,
+    ARG_EXECUTION_DATE,
+    ARG_OUTPUT_PATH,
+    ARG_SUBDIR,
+    ARG_VERBOSE,
+    ActionCommand,
+    Arg,
+    GroupCommand,
+    lazy_load_command,
+    positive_int,
+)
 from airflow.configuration import conf
 from airflow.executors.base_executor import BaseExecutor
 from airflow.providers.cncf.kubernetes.executors.kubernetes_executor_types import (
     ADOPTED,
     POD_EXECUTOR_DONE_KEY,
 )
 from airflow.providers.cncf.kubernetes.kube_config import KubeConfig
 from airflow.providers.cncf.kubernetes.kubernetes_helper_functions import annotations_to_key
+from airflow.providers.cncf.kubernetes.pod_generator import PodMutationHookException, PodReconciliationError
+from airflow.stats import Stats
 from airflow.utils.event_scheduler import EventScheduler
 from airflow.utils.log.logging_mixin import remove_escape_codes
 from airflow.utils.session import NEW_SESSION, provide_session
 from airflow.utils.state import TaskInstanceState
 
 if TYPE_CHECKING:
     import argparse
@@ -128,22 +106,22 @@
     ActionCommand(
         name="cleanup-pods",
         help=(
             "Clean up Kubernetes pods "
             "(created by KubernetesExecutor/KubernetesPodOperator) "
             "in evicted/failed/succeeded/pending states"
         ),
-        func=lazy_load_command("airflow.cli.commands.kubernetes_command.cleanup_pods"),
+        func=lazy_load_command("airflow.providers.cncf.kubernetes.cli.kubernetes_command.cleanup_pods"),
         args=(ARG_NAMESPACE, ARG_MIN_PENDING_MINUTES, ARG_VERBOSE),
     ),
     ActionCommand(
         name="generate-dag-yaml",
         help="Generate YAML files for all tasks in DAG. Useful for debugging tasks without "
         "launching into a cluster",
-        func=lazy_load_command("airflow.cli.commands.kubernetes_command.generate_pod_yaml"),
+        func=lazy_load_command("airflow.providers.cncf.kubernetes.cli.kubernetes_command.generate_pod_yaml"),
         args=(ARG_DAG_ID, ARG_EXECUTION_DATE, ARG_SUBDIR, ARG_OUTPUT_PATH, ARG_VERBOSE),
     ),
 )
 
 
 class KubernetesExecutor(BaseExecutor):
     """Executor for Kubernetes."""
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 from __future__ import annotations
 
 import contextlib
 import json
 import multiprocessing
 import time
 from queue import Empty, Queue
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
+from typing import TYPE_CHECKING, Any
 
 from kubernetes import client, watch
 from kubernetes.client.rest import ApiException
 from urllib3.exceptions import ReadTimeoutError
 
 from airflow.exceptions import AirflowException
 from airflow.providers.cncf.kubernetes.kube_client import get_kube_client
 from airflow.providers.cncf.kubernetes.kubernetes_helper_functions import (
     annotations_for_logging_task_metadata,
     annotations_to_key,
-    create_pod_id,
+    create_unique_id,
 )
 from airflow.providers.cncf.kubernetes.pod_generator import PodGenerator
 from airflow.utils.log.logging_mixin import LoggingMixin
+from airflow.utils.singleton import Singleton
 from airflow.utils.state import TaskInstanceState
 
 try:
     from airflow.providers.cncf.kubernetes.executors.kubernetes_executor_types import (
         ADOPTED,
         ALL_NAMESPACES,
         POD_EXECUTOR_DONE_KEY,
@@ -56,30 +57,14 @@
 
     from airflow.providers.cncf.kubernetes.executors.kubernetes_executor_types import (
         KubernetesJobType,
         KubernetesResultsType,
         KubernetesWatchType,
     )
 
-# Singleton here is duplicated version of airflow.utils.singleton.Singleton until
-# min-airflow version is 2.7.0 for the provider. then it can be imported from airflow.utils.singleton.
-
-T = TypeVar("T")
-
-
-class Singleton(type, Generic[T]):
-    """Metaclass that allows to implement singleton pattern."""
-
-    _instances: dict[Singleton[T], T] = {}
-
-    def __call__(cls: Singleton[T], *args, **kwargs) -> T:
-        if cls not in cls._instances:
-            cls._instances[cls] = super().__call__(*args, **kwargs)
-        return cls._instances[cls]
-
 
 class ResourceVersion(metaclass=Singleton):
     """Singleton for tracking resourceVersion from Kubernetes."""
 
     resource_version: dict[str, str] = {}
 
 
@@ -109,17 +94,15 @@
         kube_client: client.CoreV1Api = get_kube_client()
         while True:
             try:
                 self.resource_version = self._run(
                     kube_client, self.resource_version, self.scheduler_job_id, self.kube_config
                 )
             except ReadTimeoutError:
-                self.log.warning(
-                    "There was a timeout error accessing the Kube API. Retrying request.", exc_info=True
-                )
+                self.log.info("Kubernetes watch timed out waiting for events. Restarting watch.")
                 time.sleep(1)
             except Exception:
                 self.log.exception("Unknown error in KubernetesJobWatcher. Failing")
                 self.resource_version = "0"
                 ResourceVersion().resource_version[self.namespace] = "0"
                 raise
             else:
@@ -152,23 +135,31 @@
         kube_client: client.CoreV1Api,
         resource_version: str | None,
         scheduler_job_id: str,
         kube_config: Any,
     ) -> str | None:
         self.log.info("Event: and now my watch begins starting at resource_version: %s", resource_version)
 
-        kwargs = {"label_selector": f"airflow-worker={scheduler_job_id}"}
+        kwargs: dict[str, Any] = {"label_selector": f"airflow-worker={scheduler_job_id}"}
         if resource_version:
             kwargs["resource_version"] = resource_version
         if kube_config.kube_client_request_args:
             for key, value in kube_config.kube_client_request_args.items():
                 kwargs[key] = value
 
         last_resource_version: str | None = None
 
+        # For info about k8s timeout settings see
+        # https://github.com/kubernetes-client/python/blob/v29.0.0/examples/watch/timeout-settings.md
+        # and https://github.com/kubernetes-client/python/blob/v29.0.0/kubernetes/client/api_client.py#L336-L339
+        client_timeout = 30
+        server_conn_timeout = 3600
+        kwargs["_request_timeout"] = client_timeout
+        kwargs["timeout_seconds"] = server_conn_timeout
+
         for event in self._pod_events(kube_client=kube_client, query_kwargs=kwargs):
             task = event["object"]
             self.log.debug("Event: %s had an event of type %s", task.metadata.name, event["type"])
             if event["type"] == "ERROR":
                 return self.process_error(event)
             annotations = task.metadata.annotations
             task_instance_related_annotations = {
@@ -409,15 +400,15 @@
             raise AirflowException(
                 f"could not find a valid worker template yaml at {self.kube_config.pod_template_file}"
             )
 
         pod = PodGenerator.construct_pod(
             namespace=self.namespace,
             scheduler_job_id=self.scheduler_job_id,
-            pod_id=create_pod_id(dag_id, task_id),
+            pod_id=create_unique_id(dag_id, task_id),
             dag_id=dag_id,
             task_id=task_id,
             kube_image=self.kube_config.kube_image,
             try_number=try_number,
             map_index=map_index,
             date=None,
             run_id=run_id,
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714476004,
+        "source-date-epoch": 1716287042,
         "versions": [
+            "8.3.0",
             "8.2.0",
             "8.1.1",
             "8.1.0",
             "8.0.1",
             "8.0.0",
             "7.14.0",
             "7.13.0",
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 import json
 import tempfile
 from functools import cached_property
 from time import sleep
 from typing import TYPE_CHECKING, Any, Generator
 
 import aiofiles
+import tenacity
 from asgiref.sync import sync_to_async
 from kubernetes import client, config, watch
 from kubernetes.config import ConfigException
 from kubernetes_asyncio import client as async_client, config as async_config
 from urllib3.exceptions import HTTPError
 
 from airflow.exceptions import AirflowException, AirflowNotFoundException
 from airflow.hooks.base import BaseHook
 from airflow.models import Connection
 from airflow.providers.cncf.kubernetes.kube_client import _disable_verify_ssl, _enable_tcp_keepalive
+from airflow.providers.cncf.kubernetes.kubernetes_helper_functions import should_retry_creation
 from airflow.providers.cncf.kubernetes.utils.pod_manager import PodOperatorHookProtocol
 from airflow.utils import yaml
 
 if TYPE_CHECKING:
     from kubernetes.client import V1JobList
     from kubernetes.client.models import V1Deployment, V1Job, V1Pod
 
@@ -482,14 +484,20 @@
         try:
             return self.apps_v1_client.read_namespaced_deployment_status(
                 name=name, namespace=namespace, pretty=True, **kwargs
             )
         except Exception as exc:
             raise exc
 
+    @tenacity.retry(
+        stop=tenacity.stop_after_attempt(3),
+        wait=tenacity.wait_random_exponential(),
+        reraise=True,
+        retry=tenacity.retry_if_exception(should_retry_creation),
+    )
     def create_job(
         self,
         job: V1Job,
         **kwargs,
     ) -> V1Job:
         """
         Run Job.
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kube_client.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kube_config.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import logging
 import secrets
 import string
-import warnings
 from typing import TYPE_CHECKING
 
 import pendulum
+from deprecated import deprecated
+from kubernetes.client.rest import ApiException
 from slugify import slugify
 
 from airflow.compat.functools import cache
 from airflow.configuration import conf
 from airflow.exceptions import AirflowProviderDeprecationWarning
 
 if TYPE_CHECKING:
@@ -55,30 +56,27 @@
     :param max_len: maximum length of the pod name
     :meta private:
     """
     suffix = "-" + rand_str(rand_len)
     return name[: max_len - len(suffix)].strip("-.") + suffix
 
 
+@deprecated(
+    reason="This function is deprecated. Please use `add_unique_suffix`",
+    category=AirflowProviderDeprecationWarning,
+)
 def add_pod_suffix(*, pod_name: str, rand_len: int = 8, max_len: int = POD_NAME_MAX_LENGTH) -> str:
     """Add random string to pod name while staying under max length.
 
     :param pod_name: name of the pod
     :param rand_len: length of the random string to append
     :param max_len: maximum length of the pod name
     :meta private:
     """
-    warnings.warn(
-        "This function is deprecated. Please use `add_unique_suffix`.",
-        AirflowProviderDeprecationWarning,
-        stacklevel=2,
-    )
-
-    suffix = "-" + rand_str(rand_len)
-    return pod_name[: max_len - len(suffix)].strip("-.") + suffix
+    return add_unique_suffix(name=pod_name, rand_len=rand_len, max_len=max_len)
 
 
 def create_unique_id(
     dag_id: str | None = None,
     task_id: str | None = None,
     *,
     max_length: int = POD_NAME_MAX_LENGTH,
@@ -105,14 +103,18 @@
     base_name = slugify(name, lowercase=True)[:max_length].strip(".-")
     if unique:
         return add_unique_suffix(name=base_name, rand_len=8, max_len=max_length)
     else:
         return base_name
 
 
+@deprecated(
+    reason="This function is deprecated. Please use `create_unique_id`.",
+    category=AirflowProviderDeprecationWarning,
+)
 def create_pod_id(
     dag_id: str | None = None,
     task_id: str | None = None,
     *,
     max_length: int = POD_NAME_MAX_LENGTH,
     unique: bool = True,
 ) -> str:
@@ -121,34 +123,15 @@
 
     :param dag_id: DAG ID
     :param task_id: Task ID
     :param max_length: max number of characters
     :param unique: whether a random string suffix should be added
     :return: A valid identifier for a kubernetes pod name
     """
-    warnings.warn(
-        "This function is deprecated. Please use `create_unique_id`.",
-        AirflowProviderDeprecationWarning,
-        stacklevel=2,
-    )
-
-    if not (dag_id or task_id):
-        raise ValueError("Must supply either dag_id or task_id.")
-    name = ""
-    if dag_id:
-        name += dag_id
-    if task_id:
-        if name:
-            name += "-"
-        name += task_id
-    base_name = slugify(name, lowercase=True)[:max_length].strip(".-")
-    if unique:
-        return add_pod_suffix(pod_name=base_name, rand_len=8, max_len=max_length)
-    else:
-        return base_name
+    return create_unique_id(dag_id=dag_id, task_id=task_id, max_length=max_length, unique=unique)
 
 
 def annotations_to_key(annotations: dict[str, str]) -> TaskInstanceKey:
     """Build a TaskInstanceKey based on pod annotations."""
     log.debug("Creating task key for annotations %s", annotations)
     dag_id = annotations["dag_id"]
     task_id = annotations["task_id"]
@@ -195,7 +178,22 @@
 
 def annotations_for_logging_task_metadata(annotation_set):
     if get_logs_task_metadata():
         annotations_for_logging = annotation_set
     else:
         annotations_for_logging = "<omitted>"
     return annotations_for_logging
+
+
+def should_retry_creation(exception: BaseException) -> bool:
+    """
+    Check if an Exception indicates a transient error and warrants retrying.
+
+    This function is needed for preventing 'No agent available' error. The error appears time to time
+    when users try to create a Resource or Job. This issue is inside kubernetes and in the current moment
+    has no solution. Like a temporary solution we decided to retry Job or Resource creation request each
+    time when this error appears.
+    More about this issue here: https://github.com/cert-manager/cert-manager/issues/6457
+    """
+    if isinstance(exception, ApiException):
+        return str(exception.status) == "500"
+    return False
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/job.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,43 +549,43 @@
                 return pod
 
         self.log.debug("Starting pod:\n%s", yaml.safe_dump(pod_request_obj.to_dict()))
         self.pod_manager.create_pod(pod=pod_request_obj)
 
         return pod_request_obj
 
-    def await_pod_start(self, pod: k8s.V1Pod):
+    def await_pod_start(self, pod: k8s.V1Pod) -> None:
         try:
             self.pod_manager.await_pod_start(
                 pod=pod,
                 startup_timeout=self.startup_timeout_seconds,
                 startup_check_interval=self.startup_check_interval_seconds,
             )
         except PodLaunchFailedException:
             if self.log_events_on_failure:
                 self._read_pod_events(pod, reraise=False)
             raise
 
-    def extract_xcom(self, pod: k8s.V1Pod):
+    def extract_xcom(self, pod: k8s.V1Pod) -> dict[Any, Any] | None:
         """Retrieve xcom value and kill xcom sidecar container."""
         result = self.pod_manager.extract_xcom(pod)
         if isinstance(result, str) and result.rstrip() == EMPTY_XCOM_RESULT:
             self.log.info("xcom result file is empty.")
             return None
-        else:
-            self.log.info("xcom result: \n%s", result)
-            return json.loads(result)
+
+        self.log.info("xcom result: \n%s", result)
+        return json.loads(result)
 
     def execute(self, context: Context):
         """Based on the deferrable parameter runs the pod asynchronously or synchronously."""
-        if self.deferrable:
-            self.execute_async(context)
-        else:
+        if not self.deferrable:
             return self.execute_sync(context)
 
+        self.execute_async(context)
+
     def execute_sync(self, context: Context):
         result = None
         try:
             if self.pod_request_obj is None:
                 self.pod_request_obj = self.build_pod_request_obj(context)
             if self.pod is None:
                 self.pod = self.get_or_create_pod(  # must set `self.pod` for `on_kill`
@@ -665,15 +665,15 @@
             raise exc
 
     def _refresh_cached_properties(self):
         del self.hook
         del self.client
         del self.pod_manager
 
-    def execute_async(self, context: Context):
+    def execute_async(self, context: Context) -> None:
         self.pod_request_obj = self.build_pod_request_obj(context)
         self.pod = self.get_or_create_pod(  # must set `self.pod` for `on_kill`
             pod_request_obj=self.pod_request_obj,
             context=context,
         )
         if self.callbacks:
             self.callbacks.on_pod_creation(
@@ -683,15 +683,15 @@
             )
         ti = context["ti"]
         ti.xcom_push(key="pod_name", value=self.pod.metadata.name)
         ti.xcom_push(key="pod_namespace", value=self.pod.metadata.namespace)
 
         self.invoke_defer_method()
 
-    def invoke_defer_method(self, last_log_time: DateTime | None = None):
+    def invoke_defer_method(self, last_log_time: DateTime | None = None) -> None:
         """Redefine triggers which are being used in child classes."""
         trigger_start_time = datetime.datetime.now(tz=datetime.timezone.utc)
         self.defer(
             trigger=KubernetesPodTrigger(
                 pod_name=self.pod.metadata.name,  # type: ignore[union-attr]
                 pod_namespace=self.pod.metadata.namespace,  # type: ignore[union-attr]
                 trigger_start_time=trigger_start_time,
@@ -738,15 +738,15 @@
 
             follow = self.logging_interval is None
             last_log_time = event.get("last_log_time")
 
             if event["status"] in ("error", "failed", "timeout"):
                 # fetch some logs when pod is failed
                 if self.get_logs:
-                    self.write_logs(self.pod, follow=follow, since_time=last_log_time)
+                    self._write_logs(self.pod, follow=follow, since_time=last_log_time)
 
                 if self.do_xcom_push:
                     _ = self.extract_xcom(pod=self.pod)
 
                 message = event.get("stack_trace", event["message"])
                 raise AirflowException(message)
 
@@ -766,26 +766,26 @@
                         self.invoke_defer_method(pod_log_status.last_log_time)
                 else:
                     self.invoke_defer_method()
 
             elif event["status"] == "success":
                 # fetch some logs when pod is executed successfully
                 if self.get_logs:
-                    self.write_logs(self.pod, follow=follow, since_time=last_log_time)
+                    self._write_logs(self.pod, follow=follow, since_time=last_log_time)
 
                 if self.do_xcom_push:
                     xcom_sidecar_output = self.extract_xcom(pod=self.pod)
                     return xcom_sidecar_output
                 return
         except TaskDeferred:
             raise
         finally:
             self._clean(event)
 
-    def _clean(self, event: dict[str, Any]):
+    def _clean(self, event: dict[str, Any]) -> None:
         if event["status"] == "running":
             return
         istio_enabled = self.is_istio_enabled(self.pod)
         # Skip await_pod_completion when the event is 'timeout' due to the pod can hang
         # on the ErrImagePull or ContainerCreating step and it will never complete
         if event["status"] != "timeout":
             self.pod = self.pod_manager.await_pod_completion(
@@ -793,43 +793,43 @@
             )
         if self.pod is not None:
             self.post_complete_action(
                 pod=self.pod,
                 remote_pod=self.pod,
             )
 
-    @deprecated(reason="use `trigger_reentry` instead.", category=AirflowProviderDeprecationWarning)
-    def execute_complete(self, context: Context, event: dict, **kwargs):
-        return self.trigger_reentry(context=context, event=event)
-
-    def write_logs(self, pod: k8s.V1Pod, follow: bool = False, since_time: DateTime | None = None):
+    def _write_logs(self, pod: k8s.V1Pod, follow: bool = False, since_time: DateTime | None = None) -> None:
         try:
             since_seconds = (
                 math.ceil((datetime.datetime.now(tz=datetime.timezone.utc) - since_time).total_seconds())
                 if since_time
                 else None
             )
-            logs = self.pod_manager.read_pod_logs(
+            logs = self.client.read_namespaced_pod_log(
+                name=pod.metadata.name,
+                namespace=pod.metadata.namespace,
                 pod=pod,
                 container_name=self.base_container_name,
                 follow=follow,
+                timestamps=False,
                 since_seconds=since_seconds,
+                _preload_content=False,
             )
             for raw_line in logs:
                 line = raw_line.decode("utf-8", errors="backslashreplace").rstrip("\n")
                 if line:
-                    self.log.info("Container logs: %s", line)
+                    self.log.info("[%s] logs: %s", self.base_container_name, line)
         except HTTPError as e:
             self.log.warning(
                 "Reading of logs interrupted with error %r; will retry. "
                 "Set log level to DEBUG for traceback.",
                 e,
             )
 
-    def post_complete_action(self, *, pod, remote_pod, **kwargs):
+    def post_complete_action(self, *, pod, remote_pod, **kwargs) -> None:
         """Actions that must be done after operator finishes logic of the deferrable_execution."""
         self.cleanup(
             pod=pod,
             remote_pod=remote_pod,
         )
         if self.callbacks:
             self.callbacks.on_pod_cleanup(pod=pod, client=self.client, mode=ExecutionMode.SYNC)
@@ -889,15 +889,15 @@
                             error_message if isinstance(error_message, str) else None,
                             f"remote_pod: {remote_pod}" if self.log_pod_spec_on_failure else None,
                         ],
                     )
                 )
             )
 
-    def _read_pod_events(self, pod, *, reraise=True):
+    def _read_pod_events(self, pod, *, reraise=True) -> None:
         """Will fetch and emit events from pod."""
         with _optionally_suppress(reraise=reraise):
             for event in self.pod_manager.read_pod_events(pod).items:
                 if event.type == PodEventType.NORMAL.value:
                     self.log.info("Pod Event: %s - %s", event.reason, event.message)
                 else:
                     self.log.error("Pod Event: %s - %s", event.reason, event.message)
@@ -937,23 +937,19 @@
         resp.close()
         if self.KILL_ISTIO_PROXY_SUCCESS_MSG not in output_str:
             raise AirflowException("Error while deleting istio-proxy sidecar: %s", output_str)
 
     def process_pod_deletion(self, pod: k8s.V1Pod, *, reraise=True):
         with _optionally_suppress(reraise=reraise):
             if pod is not None:
-                should_delete_pod = (
-                    (self.on_finish_action == OnFinishAction.DELETE_POD)
-                    or (
-                        self.on_finish_action == OnFinishAction.DELETE_SUCCEEDED_POD
-                        and pod.status.phase == PodPhase.SUCCEEDED
-                    )
-                    or (
-                        self.on_finish_action == OnFinishAction.DELETE_SUCCEEDED_POD
-                        and container_is_succeeded(pod, self.base_container_name)
+                should_delete_pod = (self.on_finish_action == OnFinishAction.DELETE_POD) or (
+                    self.on_finish_action == OnFinishAction.DELETE_SUCCEEDED_POD
+                    and (
+                        pod.status.phase == PodPhase.SUCCEEDED
+                        or container_is_succeeded(pod, self.base_container_name)
                     )
                 )
                 if should_delete_pod:
                     self.log.info("Deleting pod: %s", pod.metadata.name)
                     self.pod_manager.delete_pod(pod)
                 else:
                     self.log.info("Skipping deleting pod: %s", pod.metadata.name)
@@ -962,16 +958,16 @@
         labels = {
             **self.labels,
             **self._get_ti_pod_labels(context, include_try_number=False),
         }
         label_strings = [f"{label_id}={label}" for label_id, label in sorted(labels.items())]
         labels_value = ",".join(label_strings)
         if exclude_checked:
-            labels_value += f",{self.POD_CHECKED_KEY}!=True"
-        labels_value += ",!airflow-worker"
+            labels_value = f"{labels_value},{self.POD_CHECKED_KEY}!=True"
+        labels_value = f"{labels_value},!airflow-worker"
         return labels_value
 
     @staticmethod
     def _set_name(name: str | None) -> str | None:
         if name is not None:
             validate_key(name, max_length=220)
             return re.sub(r"[^a-z0-9-]+", "-", name.lower())
@@ -1125,36 +1121,40 @@
 
         Does not include labels specific to the task instance (since there isn't
         one in a dry_run) and excludes all empty elements.
         """
         pod = self.build_pod_request_obj()
         print(yaml.dump(prune_dict(pod.to_dict(), mode="strict")))
 
+    @deprecated(reason="use `trigger_reentry` instead.", category=AirflowProviderDeprecationWarning)
+    def execute_complete(self, context: Context, event: dict, **kwargs):
+        return self.trigger_reentry(context=context, event=event)
+
 
 class _optionally_suppress(AbstractContextManager):
     """
     Returns context manager that will swallow and log exceptions.
 
     By default swallows descendents of Exception, but you can provide other classes through
     the vararg ``exceptions``.
 
     Suppression behavior can be disabled with reraise=True.
 
     :meta private:
     """
 
-    def __init__(self, *exceptions, reraise=False):
+    def __init__(self, *exceptions, reraise: bool = False) -> None:
         self._exceptions = exceptions or (Exception,)
         self.reraise = reraise
         self.exception = None
 
     def __enter__(self):
         return self
 
-    def __exit__(self, exctype, excinst, exctb):
+    def __exit__(self, exctype, excinst, exctb) -> bool:
         error = exctype is not None
         matching_error = error and issubclass(exctype, self._exceptions)
         if (error and not matching_error) or (matching_error and self.reraise):
             return False
         elif matching_error:
             self.exception = excinst
             logger = logging.getLogger(__name__)
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 
 from __future__ import annotations
 
 import os
 from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 
+import tenacity
 import yaml
 from kubernetes.utils import create_from_yaml
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.hooks.kubernetes import KubernetesHook
+from airflow.providers.cncf.kubernetes.kubernetes_helper_functions import should_retry_creation
 from airflow.providers.cncf.kubernetes.utils.delete_from import delete_from_yaml
 from airflow.providers.cncf.kubernetes.utils.k8s_resource_iterator import k8s_resource_iterator
 
 if TYPE_CHECKING:
     from kubernetes.client import ApiClient, CustomObjectsApi
 
 __all__ = ["KubernetesCreateResourceOperator", "KubernetesDeleteResourceOperator"]
@@ -122,15 +124,22 @@
     def create_custom_from_yaml_object(self, body: dict):
         group, version, namespace, plural = self.get_crd_fields(body)
         if self.namespaced:
             self.custom_object_client.create_namespaced_custom_object(group, version, namespace, plural, body)
         else:
             self.custom_object_client.create_cluster_custom_object(group, version, plural, body)
 
+    @tenacity.retry(
+        stop=tenacity.stop_after_attempt(3),
+        wait=tenacity.wait_random_exponential(),
+        reraise=True,
+        retry=tenacity.retry_if_exception(should_retry_creation),
+    )
     def _create_objects(self, objects):
+        self.log.info("Starting resource creation")
         if not self.custom_resource_definition:
             create_from_yaml(
                 k8s_client=self.client,
                 yaml_objects=objects,
                 namespace=self.get_namespace(),
             )
         else:
@@ -140,14 +149,15 @@
         if self.yaml_conf:
             self._create_objects(yaml.safe_load_all(self.yaml_conf))
         elif self.yaml_conf_file and os.path.exists(self.yaml_conf_file):
             with open(self.yaml_conf_file) as stream:
                 self._create_objects(yaml.safe_load_all(stream))
         else:
             raise AirflowException("File %s not found", self.yaml_conf_file)
+        self.log.info("Resource was created")
 
 
 class KubernetesDeleteResourceOperator(KubernetesResourceBaseOperator):
     """Delete a resource in a kubernetes."""
 
     def delete_custom_from_yaml_object(self, body: dict):
         name = body["metadata"]["name"]
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 from airflow.exceptions import (
     AirflowConfigException,
     AirflowException,
     AirflowProviderDeprecationWarning,
 )
 from airflow.providers.cncf.kubernetes.kubernetes_helper_functions import (
     POD_NAME_MAX_LENGTH,
-    add_pod_suffix,
     add_unique_suffix,
     rand_str,
 )
 from airflow.providers.cncf.kubernetes.pod_generator_deprecated import (
     PodDefaults as PodDefaultsDeprecated,
     PodGenerator as PodGeneratorDeprecated,
 )
@@ -152,20 +151,23 @@
             self.ud_pod = self.deserialize_model_file(pod_template_file)
         else:
             self.ud_pod = pod
 
         # Attach sidecar
         self.extract_xcom = extract_xcom
 
-    @deprecated(reason="This function is deprecated.", category=AirflowProviderDeprecationWarning)
+    @deprecated(
+        reason="This method is deprecated and will be removed in the future releases",
+        category=AirflowProviderDeprecationWarning,
+    )
     def gen_pod(self) -> k8s.V1Pod:
         """Generate pod."""
         result = self.ud_pod
 
-        result.metadata.name = add_pod_suffix(pod_name=result.metadata.name)
+        result.metadata.name = add_unique_suffix(name=result.metadata.name)
 
         if self.extract_xcom:
             result = self.add_xcom_sidecar(result)
 
         return result
 
     @staticmethod
@@ -206,16 +208,16 @@
         if not k8s_object and not k8s_legacy_object:
             return None
 
         if isinstance(k8s_object, k8s.V1Pod):
             return k8s_object
         elif isinstance(k8s_legacy_object, dict):
             warnings.warn(
-                "Using a dictionary for the executor_config is deprecated and will soon be removed."
-                'please use a `kubernetes.client.models.V1Pod` class with a "pod_override" key'
+                "Using a dictionary for the executor_config is deprecated and will soon be removed. "
+                'Please use a `kubernetes.client.models.V1Pod` class with a "pod_override" key'
                 " instead. ",
                 category=AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             return PodGenerator.from_legacy_obj(obj)
         else:
             raise TypeError(
@@ -571,15 +573,15 @@
         :return: De-serialized k8s.V1Pod
         """
         api_client = ApiClient()
         return api_client._ApiClient__deserialize_model(pod_dict, k8s.V1Pod)
 
     @staticmethod
     @deprecated(
-        reason="This function is deprecated. Use `add_pod_suffix` in `kubernetes_helper_functions`.",
+        reason="This method is deprecated. Use `add_pod_suffix` in `kubernetes_helper_functions`.",
         category=AirflowProviderDeprecationWarning,
     )
     def make_unique_pod_id(pod_id: str) -> str | None:
         r"""
         Generate a unique Pod name.
 
         Kubernetes pod names must consist of one or more lowercase
@@ -591,20 +593,14 @@
 
         For more details, see:
         https://github.com/kubernetes/kubernetes/blob/release-1.1/docs/design/identifiers.md
 
         :param pod_id: requested pod name
         :return: ``str`` valid Pod name of appropriate length
         """
-        warnings.warn(
-            "This function is deprecated. Use `add_pod_suffix` in `kubernetes_helper_functions`.",
-            AirflowProviderDeprecationWarning,
-            stacklevel=2,
-        )
-
         if not pod_id:
             return None
 
         max_pod_id_len = 100  # arbitrarily chosen
         suffix = rand_str(8)  # 8 seems good enough
         base_pod_id_len = max_pod_id_len - len(suffix) - 1  # -1 for separator
         trimmed_pod_id = pod_id[:base_pod_id_len].rstrip("-.")
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/template_rendering.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 from typing import TYPE_CHECKING
 
 from jinja2 import TemplateAssertionError, UndefinedError
 from kubernetes.client.api_client import ApiClient
 
 from airflow.exceptions import AirflowException
 from airflow.providers.cncf.kubernetes.kube_config import KubeConfig
-from airflow.providers.cncf.kubernetes.kubernetes_helper_functions import (
-    create_pod_id,
-)
+from airflow.providers.cncf.kubernetes.kubernetes_helper_functions import create_unique_id
 from airflow.providers.cncf.kubernetes.pod_generator import PodGenerator
 from airflow.utils.session import NEW_SESSION, provide_session
 
 if TYPE_CHECKING:
     from airflow.models.taskinstance import TaskInstance
 
 
@@ -39,15 +37,15 @@
     kube_config = KubeConfig()
     pod = PodGenerator.construct_pod(
         dag_id=task_instance.dag_id,
         run_id=task_instance.run_id,
         task_id=task_instance.task_id,
         map_index=task_instance.map_index,
         date=None,
-        pod_id=create_pod_id(task_instance.dag_id, task_instance.task_id),
+        pod_id=create_unique_id(task_instance.dag_id, task_instance.task_id),
         try_number=task_instance.try_number,
         kube_image=kube_config.kube_image,
         args=task_instance.command_as_list(),
         pod_override_object=PodGenerator.from_obj(task_instance.executor_config),
         scheduler_job_id="0",
         namespace=kube_config.executor_namespace,
         base_worker_pod=PodGenerator.deserialize_model_file(kube_config.pod_template_file),
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/pyproject.toml` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-cncf-kubernetes"
-version = "8.2.0.rc1"
+version = "8.3.0.rc1"
 description = "Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -62,16 +62,16 @@
     "cryptography>=2.0.0",
     "google-re2>=1.0",
     "kubernetes>=28.1.0,<=29.0.0",
     "kubernetes_asyncio>=28.1.0,<=29.0.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.2.0rc1/PKG-INFO` & `apache_airflow_providers_cncf_kubernetes-8.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 8.2.0rc1
+Version: 8.3.0rc1
 Summary: Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow
 Keywords: airflow-provider,cncf.kubernetes,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,16 +25,16 @@
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: asgiref>=3.5.2
 Requires-Dist: cryptography>=2.0.0
 Requires-Dist: google-re2>=1.0
 Requires-Dist: kubernetes>=28.1.0,<=29.0.0
 Requires-Dist: kubernetes_asyncio>=28.1.0,<=29.0.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -76,28 +76,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.2.0.rc1``
+Release: ``8.3.0.rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cncf-kubernetes``
@@ -116,8 +116,8 @@
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=28.1.0,<=29.0.0``
 ``kubernetes_asyncio``  ``>=28.1.0,<=29.0.0``
 ``google-re2``          ``>=1.0``
 ======================  =====================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.3.0/changelog.html>`_.
```

