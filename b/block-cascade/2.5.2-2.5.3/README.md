# Comparing `tmp/block_cascade-2.5.2.tar.gz` & `tmp/block_cascade-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block_cascade-2.5.2.tar", max compression
+gzip compressed data, was "block_cascade-2.5.3.tar", max compression
```

## Comparing `block_cascade-2.5.2.tar` & `block_cascade-2.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11357 2024-04-11 20:04:18.933034 block_cascade-2.5.2/LICENSE.txt
--rw-r--r--   0        0        0     4836 2024-04-11 20:04:18.933034 block_cascade-2.5.2/README.md
--rw-r--r--   0        0        0      535 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/__init__.py
--rw-r--r--   0        0        0      516 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/cli/__init__.py
--rw-r--r--   0        0        0     9865 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/cli/crud.py
--rw-r--r--   0        0        0      687 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/concurrency/__init__.py
--rw-r--r--   0        0        0     3122 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/config.py
--rw-r--r--   0        0        0       38 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/consts.py
--rw-r--r--   0        0        0    10462 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/decorators.py
--rw-r--r--   0        0        0      317 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/databricks/__init__.py
--rw-r--r--   0        0        0    10627 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/databricks/executor.py
--rw-r--r--   0        0        0     5392 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/databricks/job.py
--rw-r--r--   0        0        0     5316 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/databricks/resource.py
--rw-r--r--   0        0        0     1537 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/databricks/run.py
--rw-r--r--   0        0        0     3767 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/executor.py
--rw-r--r--   0        0        0       79 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/local/__init__.py
--rw-r--r--   0        0        0     1315 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/local/executor.py
--rw-r--r--   0        0        0      593 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/distributed/__init__.py
--rw-r--r--   0        0        0     9682 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/distributed/distributed_job.py
--rw-r--r--   0        0        0     4625 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/distributed/torch_job.py
--rw-r--r--   0        0        0     2981 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/distributed/torchrun_target.py
--rw-r--r--   0        0        0    13549 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/executor.py
--rw-r--r--   0        0        0     9816 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/job.py
--rw-r--r--   0        0        0     5399 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/resource.py
--rw-r--r--   0        0        0     2821 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/run.py
--rw-r--r--   0        0        0     1190 2024-04-11 20:04:18.933034 block_cascade-2.5.2/block_cascade/executors/vertex/tune.py
--rw-r--r--   0        0        0     2527 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/gcp/__init__.py
--rw-r--r--   0        0        0     7496 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/gcp/monitoring.py
--rw-r--r--   0        0        0      448 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/prefect/__init__.py
--rw-r--r--   0        0        0      613 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/prefect/v1/__init__.py
--rw-r--r--   0        0        0     3073 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/prefect/v1/environment.py
--rw-r--r--   0        0        0     3383 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/prefect/v2/__init__.py
--rw-r--r--   0        0        0     2892 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/prefect/v2/environment.py
--rw-r--r--   0        0        0     2751 2024-04-11 20:04:18.937034 block_cascade-2.5.2/block_cascade/utils.py
--rw-r--r--   0        0        0     1304 2024-04-11 20:04:18.937034 block_cascade-2.5.2/pyproject.toml
--rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 block_cascade-2.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 15:44:04.360609 block_cascade-2.5.3/LICENSE.txt
+-rw-r--r--   0        0        0     4836 2024-05-30 15:44:04.360609 block_cascade-2.5.3/README.md
+-rw-r--r--   0        0        0      535 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/__init__.py
+-rw-r--r--   0        0        0      516 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/cli/__init__.py
+-rw-r--r--   0        0        0     9865 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/cli/crud.py
+-rw-r--r--   0        0        0      687 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/concurrency/__init__.py
+-rw-r--r--   0        0        0     3122 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/config.py
+-rw-r--r--   0        0        0       38 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/consts.py
+-rw-r--r--   0        0        0    10462 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/decorators.py
+-rw-r--r--   0        0        0      317 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/executors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/executors/databricks/__init__.py
+-rw-r--r--   0        0        0    10686 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/executors/databricks/executor.py
+-rw-r--r--   0        0        0     5392 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/executors/databricks/job.py
+-rw-r--r--   0        0        0     5450 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/executors/databricks/resource.py
+-rw-r--r--   0        0        0     1537 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/executors/databricks/run.py
+-rw-r--r--   0        0        0     3767 2024-05-30 15:44:04.360609 block_cascade-2.5.3/block_cascade/executors/executor.py
+-rw-r--r--   0        0        0       79 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/local/__init__.py
+-rw-r--r--   0        0        0     1315 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/local/executor.py
+-rw-r--r--   0        0        0      593 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/distributed/__init__.py
+-rw-r--r--   0        0        0     9682 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/distributed/distributed_job.py
+-rw-r--r--   0        0        0     4625 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/distributed/torch_job.py
+-rw-r--r--   0        0        0     2981 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/distributed/torchrun_target.py
+-rw-r--r--   0        0        0    13549 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/executor.py
+-rw-r--r--   0        0        0     9816 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/job.py
+-rw-r--r--   0        0        0     5399 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/resource.py
+-rw-r--r--   0        0        0     2821 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/run.py
+-rw-r--r--   0        0        0     1190 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/executors/vertex/tune.py
+-rw-r--r--   0        0        0     2527 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/gcp/__init__.py
+-rw-r--r--   0        0        0     7496 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/gcp/monitoring.py
+-rw-r--r--   0        0        0      448 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/prefect/__init__.py
+-rw-r--r--   0        0        0      613 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/prefect/v1/__init__.py
+-rw-r--r--   0        0        0     3073 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/prefect/v1/environment.py
+-rw-r--r--   0        0        0     3383 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/prefect/v2/__init__.py
+-rw-r--r--   0        0        0     2892 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/prefect/v2/environment.py
+-rw-r--r--   0        0        0     2751 2024-05-30 15:44:04.364609 block_cascade-2.5.3/block_cascade/utils.py
+-rw-r--r--   0        0        0     1304 2024-05-30 15:44:04.364609 block_cascade-2.5.3/pyproject.toml
+-rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 block_cascade-2.5.3/PKG-INFO
```

### Comparing `block_cascade-2.5.2/LICENSE.txt` & `block_cascade-2.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/README.md` & `block_cascade-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/__init__.py` & `block_cascade-2.5.3/block_cascade/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/cli/__init__.py` & `block_cascade-2.5.3/block_cascade/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/cli/crud.py` & `block_cascade-2.5.3/block_cascade/cli/crud.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/concurrency/__init__.py` & `block_cascade-2.5.3/block_cascade/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/config.py` & `block_cascade-2.5.3/block_cascade/config.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/decorators.py` & `block_cascade-2.5.3/block_cascade/decorators.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/databricks/executor.py` & `block_cascade-2.5.3/block_cascade/executors/databricks/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,15 @@
             storage_path=self.storage_path,
             storage_key=self.storage_key,
             existing_cluster_id=self.resource.existing_cluster_id,
             cluster_policy_id=self.get_cluster_policy_id_from_policy_name(
                 self.cluster_policy
             ),
             run_path=self.run_path,
+            timeout_seconds=self.resource.timeout_seconds,
         )
 
     def _run(self):
         """
         Create the payload, submit it to the API, and monitor its status while it
         is executing
         """
```

### Comparing `block_cascade-2.5.2/block_cascade/executors/databricks/job.py` & `block_cascade-2.5.3/block_cascade/executors/databricks/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     name: str
     resource: DatabricksResource
     storage_path: str
     storage_key: str
     run_path: str
     cluster_policy_id: str
     existing_cluster_id: Optional[str] = None
-    timeout_seconds: str = 86400
+    timeout_seconds: int = 86400
 
     def create_payload(self):
         """"""
         task = self._task_spec()
         task.update({"existing_cluster_id": self.existing_cluster_id})
         task.update({"new_cluster": self._cluster_spec()})
```

### Comparing `block_cascade-2.5.2/block_cascade/executors/databricks/resource.py` & `block_cascade-2.5.3/block_cascade/executors/databricks/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,16 @@
         in the `cloudpickle_by_value`
     task_args: Optional[dict] = None
         If provided, pass these additional arguments into the databricks task. This can
         be used
     python_libraries: Optional[List[str]] = None
         If provided, install these additional libraries on the cluster when the
         remote task is run
+    timeout_seconds: int = 86400
+        The maximum time this job can run for; default is 24 hours.
 
     """  # noqa: E501
 
     storage_location: str
     worker_count: Optional[Union[int, DatabricksAutoscaleConfig]] = 1
     machine: Optional[str] = "i3.xlarge"
     spark_version: Optional[str] = "11.3.x-scala2.12"
@@ -113,11 +115,12 @@
     secret: Optional[DatabricksSecret] = None
     environment: Optional[str] = "prod"
     s3_credentials: Optional[dict] = None
     cloud_pickle_by_value: Optional[List[str]] = Field(default_factory=list)
     cloud_pickle_infer_base_module: Optional[bool] = True
     task_args: Optional[dict] = None
     python_libraries: Optional[List[str]] = None
+    timeout_seconds: int = 86400
 
     def __post_init__(self):
         if self.group_name is None:
             self.group_name = os.environ.get("DATABRICKS_GROUP", "default-group")
```

### Comparing `block_cascade-2.5.2/block_cascade/executors/databricks/run.py` & `block_cascade-2.5.3/block_cascade/executors/databricks/run.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/executor.py` & `block_cascade-2.5.3/block_cascade/executors/executor.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/local/executor.py` & `block_cascade-2.5.3/block_cascade/executors/local/executor.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/__init__.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/distributed/distributed_job.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/distributed/distributed_job.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/distributed/torch_job.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/distributed/torch_job.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/distributed/torchrun_target.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/distributed/torchrun_target.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/executor.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/executor.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/job.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/job.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/resource.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/resource.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/run.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/run.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/executors/vertex/tune.py` & `block_cascade-2.5.3/block_cascade/executors/vertex/tune.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/gcp/__init__.py` & `block_cascade-2.5.3/block_cascade/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/gcp/monitoring.py` & `block_cascade-2.5.3/block_cascade/gcp/monitoring.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/prefect/v1/__init__.py` & `block_cascade-2.5.3/block_cascade/prefect/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/prefect/v1/environment.py` & `block_cascade-2.5.3/block_cascade/prefect/v1/environment.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/prefect/v2/__init__.py` & `block_cascade-2.5.3/block_cascade/prefect/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/prefect/v2/environment.py` & `block_cascade-2.5.3/block_cascade/prefect/v2/environment.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/block_cascade/utils.py` & `block_cascade-2.5.3/block_cascade/utils.py`

 * *Files identical despite different names*

### Comparing `block_cascade-2.5.2/pyproject.toml` & `block_cascade-2.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "block-cascade"
 packages = [
     {include = "block_cascade"}
 ]
-version = "2.5.2"
+version = "2.5.3"
 description = "Library for model training in multi-cloud environment."
 readme = "README.md"
 authors = ["Block"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 cloudml-hypertune = "==0.1.0.dev6"
```

### Comparing `block_cascade-2.5.2/PKG-INFO` & `block_cascade-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-cascade
-Version: 2.5.2
+Version: 2.5.3
 Summary: Library for model training in multi-cloud environment.
 Author: Block
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

