# Comparing `tmp/dataverk_airflow-1.7.0.tar.gz` & `tmp/dataverk_airflow-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverk_airflow-1.7.0.tar", max compression
+gzip compressed data, was "dataverk_airflow-1.7.1.tar", max compression
```

## Comparing `dataverk_airflow-1.7.0.tar` & `dataverk_airflow-1.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1061 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/LICENSE
--rw-r--r--   0        0        0     8443 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/README.md
--rw-r--r--   0        0        0      381 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/__init__.py
--rw-r--r--   0        0        0      752 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/bucket_read.py
--rw-r--r--   0        0        0     1264 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/git_clone.py
--rw-r--r--   0        0        0    10042 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/kubernetes_operator.py
--rw-r--r--   0        0        0     4377 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/notebook_operator.py
--rw-r--r--   0        0        0     1058 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/notifications.py
--rw-r--r--   0        0        0     4206 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/python_operator.py
--rw-r--r--   0        0        0     5871 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/quarto_operator.py
--rw-r--r--   0        0        0      877 2024-05-21 10:54:35.111521 dataverk_airflow-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     9419 1970-01-01 00:00:00.000000 dataverk_airflow-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/LICENSE
+-rw-r--r--   0        0        0     8443 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/README.md
+-rw-r--r--   0        0        0      381 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/__init__.py
+-rw-r--r--   0        0        0      752 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/bucket_read.py
+-rw-r--r--   0        0        0     1264 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/git_clone.py
+-rw-r--r--   0        0        0    10042 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/kubernetes_operator.py
+-rw-r--r--   0        0        0     4668 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/notebook_operator.py
+-rw-r--r--   0        0        0     1058 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/notifications.py
+-rw-r--r--   0        0        0     4206 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/python_operator.py
+-rw-r--r--   0        0        0     5871 2024-05-30 08:50:30.303370 dataverk_airflow-1.7.1/dataverk_airflow/quarto_operator.py
+-rw-r--r--   0        0        0      877 2024-05-30 08:50:30.563370 dataverk_airflow-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9419 1970-01-01 00:00:00.000000 dataverk_airflow-1.7.1/PKG-INFO
```

### Comparing `dataverk_airflow-1.7.0/LICENSE` & `dataverk_airflow-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.7.0/README.md` & `dataverk_airflow-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.7.0/dataverk_airflow/bucket_read.py` & `dataverk_airflow-1.7.1/dataverk_airflow/bucket_read.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.7.0/dataverk_airflow/git_clone.py` & `dataverk_airflow-1.7.1/dataverk_airflow/git_clone.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.7.0/dataverk_airflow/kubernetes_operator.py` & `dataverk_airflow-1.7.1/dataverk_airflow/kubernetes_operator.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.7.0/dataverk_airflow/notebook_operator.py` & `dataverk_airflow-1.7.1/dataverk_airflow/python_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,83 +5,79 @@
 
 from airflow import DAG
 from kubernetes import client
 
 from dataverk_airflow.kubernetes_operator import kubernetes_operator, VALID_PYTHON_VERSIONS
 
 
-def notebook_operator(
+def python_operator(
         dag: DAG,
         name: str,
-        nb_path: str,
+        script_path: str,
         repo: str = None,
-        log_output: bool = False,
         image: str = None,
         branch: str = "main",
         email: str = None,
         slack_channel: str = None,
         extra_envs: dict = {},
         allowlist: list = [],
         requirements_path: str = None,
         python_version: str = "3.11",
         resources: client.V1ResourceRequirements = None,
         startup_timeout_seconds: int = None,
         retries: int = None,
         delete_on_finish: bool = True,
         retry_delay: timedelta = None,
         do_xcom_push: bool = False,
-        on_success_callback: Callable = None,
         container_uid: int = 50000,
+        on_success_callback: Callable = None,
         use_uv_pip_install: bool = False,
 ):
-    """Operator for executing Jupyter notebooks.
+    """Operator for executing Python scripts.
 
     :param dag: DAG: owner DAG
     :param name: str: Name of task
     :param repo: str: Github repo
-    :param nb_path: str: Path to notebook in repo
-    :param log_output: bool: Write logs from notebook to stdout, default False
+    :param script_path: str: Path to script in repo
     :param image: str: Dockerimage the pod should use
     :param branch: str: Branch in repo, default "main"
     :param email: str: Email of owner
     :param slack_channel: str: Name of Slack channel, default None (no Slack notification)
     :param extra_envs: dict: dict with environment variables example: {"key": "value", "key2": "value2"}
     :param allowlist: list: list of hosts and port the task needs to reach on the format host:port
     :param requirements_path: bool: Path (including filename) to your requirements.txt
     :param python_version: str: desired Python version for the environment your code will be running in when using the default image. We offer only supported versions of Python, and default to the latest version if this parameter is omitted. See https://devguide.python.org/versions/ for available versions.
-    :param resources: dict: Specify cpu and memory resource usage (dict: request/limit: {"memory": "", "cpu": "", "ephemeral-storage": ""}), default None
+    :param resources: dict: Specify required cpu and memory requirements (keys in dict: request_memory, request_cpu, limit_memory, limit_cpu), default None
     :param startup_timeout_seconds: int: pod startup timeout
     :param retries: int: Number of retries for task before DAG fails, default 3
     :param delete_on_finish: bool: Whether to delete pod on completion
     :param retry_delay: timedelta: Time inbetween retries, default 5 seconds
     :param do_xcom_push: bool: Enable xcom push of content in file '/airflow/xcom/return.json', default False
     :param container_uid: int: User ID for the container image. Root (id = 0) is not allowed, defaults to 50000 (standard uid for airflow).
     :param on_success_callback: Callable
     :param use_uv_pip_install: bool: Use uv pip install, default False
 
     :return: KubernetesPodOperator
     """
     if not image:
         if python_version not in VALID_PYTHON_VERSIONS:
             raise ValueError(
-                f"When using the default image the python_version argument must be set to "
+                f"When using the default image the python_version argument must be set to " \
                 f"{', '.join(VALID_PYTHON_VERSIONS[:-1])} or {VALID_PYTHON_VERSIONS[-1]}: value '{python_version}' is not supported" 
             )
         try:
             image = os.environ["DATAVERK_IMAGE_PYTHON_" + python_version.replace(".","")]
         except KeyError:
             image = os.getenv("KNADA_AIRFLOW_OPERATOR_IMAGE")
 
-    cmds = [f"papermill {Path(nb_path).name} output.ipynb"]
-    if log_output:
-        cmds[-1] += " --log-output"
+    cmds = [f"python {Path(script_path).name}"]
 
     kwargs = {
         "dag": dag, "name": name, "repo": repo, "image": image, "cmds": cmds, "branch": branch, "email": email,
         "slack_channel": slack_channel, "extra_envs": extra_envs, "allowlist": allowlist, "requirements_path": requirements_path,
         "resources": resources, "startup_timeout_seconds": startup_timeout_seconds, 
         "retries": retries, "delete_on_finish": delete_on_finish, "retry_delay": retry_delay, "do_xcom_push": do_xcom_push,
-        "on_success_callback": on_success_callback, "working_dir": str(Path(nb_path).parent), "container_uid": container_uid, "use_uv_pip_install": use_uv_pip_install,
+        "on_success_callback": on_success_callback, "working_dir": str(Path(script_path).parent), "container_uid": container_uid, "use_uv_pip_install": use_uv_pip_install,
     }
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
     return kubernetes_operator(**kwargs)
```

### Comparing `dataverk_airflow-1.7.0/dataverk_airflow/notifications.py` & `dataverk_airflow-1.7.1/dataverk_airflow/notifications.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.7.0/dataverk_airflow/python_operator.py` & `dataverk_airflow-1.7.1/dataverk_airflow/notebook_operator.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,79 +5,87 @@
 
 from airflow import DAG
 from kubernetes import client
 
 from dataverk_airflow.kubernetes_operator import kubernetes_operator, VALID_PYTHON_VERSIONS
 
 
-def python_operator(
+def notebook_operator(
         dag: DAG,
         name: str,
-        script_path: str,
+        nb_path: str,
         repo: str = None,
+        log_output: bool = False,
         image: str = None,
         branch: str = "main",
         email: str = None,
         slack_channel: str = None,
         extra_envs: dict = {},
         allowlist: list = [],
         requirements_path: str = None,
         python_version: str = "3.11",
         resources: client.V1ResourceRequirements = None,
         startup_timeout_seconds: int = None,
         retries: int = None,
         delete_on_finish: bool = True,
         retry_delay: timedelta = None,
         do_xcom_push: bool = False,
-        container_uid: int = 50000,
         on_success_callback: Callable = None,
+        container_uid: int = 50000,
         use_uv_pip_install: bool = False,
+        override_notebook_kernelspec: bool = True,
 ):
-    """Operator for executing Python scripts.
+    """Operator for executing Jupyter notebooks.
 
     :param dag: DAG: owner DAG
     :param name: str: Name of task
     :param repo: str: Github repo
-    :param script_path: str: Path to script in repo
+    :param nb_path: str: Path to notebook in repo
+    :param log_output: bool: Write logs from notebook to stdout, default False
     :param image: str: Dockerimage the pod should use
     :param branch: str: Branch in repo, default "main"
     :param email: str: Email of owner
     :param slack_channel: str: Name of Slack channel, default None (no Slack notification)
     :param extra_envs: dict: dict with environment variables example: {"key": "value", "key2": "value2"}
     :param allowlist: list: list of hosts and port the task needs to reach on the format host:port
     :param requirements_path: bool: Path (including filename) to your requirements.txt
     :param python_version: str: desired Python version for the environment your code will be running in when using the default image. We offer only supported versions of Python, and default to the latest version if this parameter is omitted. See https://devguide.python.org/versions/ for available versions.
-    :param resources: dict: Specify required cpu and memory requirements (keys in dict: request_memory, request_cpu, limit_memory, limit_cpu), default None
+    :param resources: dict: Specify cpu and memory resource usage (dict: request/limit: {"memory": "", "cpu": "", "ephemeral-storage": ""}), default None
     :param startup_timeout_seconds: int: pod startup timeout
     :param retries: int: Number of retries for task before DAG fails, default 3
     :param delete_on_finish: bool: Whether to delete pod on completion
     :param retry_delay: timedelta: Time inbetween retries, default 5 seconds
     :param do_xcom_push: bool: Enable xcom push of content in file '/airflow/xcom/return.json', default False
     :param container_uid: int: User ID for the container image. Root (id = 0) is not allowed, defaults to 50000 (standard uid for airflow).
     :param on_success_callback: Callable
     :param use_uv_pip_install: bool: Use uv pip install, default False
+    :param override_notebook_kernelspec: bool: Whether to override the kernelspec in the notebook metadata, default True (will ensure that python3 kernel is used)
 
     :return: KubernetesPodOperator
     """
     if not image:
         if python_version not in VALID_PYTHON_VERSIONS:
             raise ValueError(
-                f"When using the default image the python_version argument must be set to " \
+                f"When using the default image the python_version argument must be set to "
                 f"{', '.join(VALID_PYTHON_VERSIONS[:-1])} or {VALID_PYTHON_VERSIONS[-1]}: value '{python_version}' is not supported" 
             )
         try:
             image = os.environ["DATAVERK_IMAGE_PYTHON_" + python_version.replace(".","")]
         except KeyError:
             image = os.getenv("KNADA_AIRFLOW_OPERATOR_IMAGE")
 
-    cmds = [f"python {Path(script_path).name}"]
+    cmds = [f"papermill {Path(nb_path).name} output.ipynb"]
+    if log_output:
+        cmds[-1] += " --log-output"
+    if override_notebook_kernelspec:
+        cmds[-1] += " --kernel python3"
 
     kwargs = {
         "dag": dag, "name": name, "repo": repo, "image": image, "cmds": cmds, "branch": branch, "email": email,
         "slack_channel": slack_channel, "extra_envs": extra_envs, "allowlist": allowlist, "requirements_path": requirements_path,
         "resources": resources, "startup_timeout_seconds": startup_timeout_seconds, 
         "retries": retries, "delete_on_finish": delete_on_finish, "retry_delay": retry_delay, "do_xcom_push": do_xcom_push,
-        "on_success_callback": on_success_callback, "working_dir": str(Path(script_path).parent), "container_uid": container_uid, "use_uv_pip_install": use_uv_pip_install,
+        "on_success_callback": on_success_callback, "working_dir": str(Path(nb_path).parent), "container_uid": container_uid, "use_uv_pip_install": use_uv_pip_install,
     }
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
     return kubernetes_operator(**kwargs)
```

### Comparing `dataverk_airflow-1.7.0/dataverk_airflow/quarto_operator.py` & `dataverk_airflow-1.7.1/dataverk_airflow/quarto_operator.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.7.0/pyproject.toml` & `dataverk_airflow-1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataverk-airflow"
-version = "1.7.0"
+version = "1.7.1"
 description = ""
 authors = ["NAV", "NADA"]
 readme = "README.md"
 packages = [{include = "dataverk_airflow"}]
 repository = "https://github.com/navikt/dataverk-airflow"
 classifiers = [
   'Development Status :: 5 - Production/Stable',
@@ -15,20 +15,20 @@
 [tool.poetry.dependencies]
 apache-airflow-providers-cncf-kubernetes = "^7.3.0"
 kubernetes = ">=21.7.0,<24"
 pathlib = "^1.0.1"
 python = "^3.8,<3.12"
 apache-airflow-providers-slack = "^8.1.0"
 exceptiongroup = "^1.1.3"
-knatch = "^1.0.1"
+knatch = "^1.0.5"
 
 [tool.poetry.group.test.dependencies]
 pyaml = "^23.9.7"
 pytest = ">=7.4.2,<9.0.0"
 pytest-datafiles = "^3.0.0"
 
 [tool.poetry.group.integration-test.dependencies]
-apache-airflow = "^2.7.3"
+apache-airflow = "^2.9.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dataverk_airflow-1.7.0/PKG-INFO` & `dataverk_airflow-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverk-airflow
-Version: 1.7.0
+Version: 1.7.1
 Summary: 
 Home-page: https://github.com/navikt/dataverk-airflow
 Author: NAV
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apache-airflow-providers-cncf-kubernetes (>=7.3.0,<8.0.0)
 Requires-Dist: apache-airflow-providers-slack (>=8.1.0,<9.0.0)
 Requires-Dist: exceptiongroup (>=1.1.3,<2.0.0)
-Requires-Dist: knatch (>=1.0.1,<2.0.0)
+Requires-Dist: knatch (>=1.0.5,<2.0.0)
 Requires-Dist: kubernetes (>=21.7.0,<24)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Project-URL: Repository, https://github.com/navikt/dataverk-airflow
 Description-Content-Type: text/markdown
 
 # Dataverk airflow
```

