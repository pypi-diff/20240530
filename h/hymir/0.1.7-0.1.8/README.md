# Comparing `tmp/hymir-0.1.7.tar.gz` & `tmp/hymir-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hymir-0.1.7.tar", max compression
+gzip compressed data, was "hymir-0.1.8.tar", max compression
```

## Comparing `hymir-0.1.7.tar` & `hymir-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1082 2024-04-22 17:58:46.132038 hymir-0.1.7/LICENSE
--rw-r--r--   0        0        0      464 2024-04-22 17:58:46.132038 hymir-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-04-22 17:58:46.132038 hymir-0.1.7/hymir/__init__.py
--rw-r--r--   0        0        0     1092 2024-04-22 17:58:46.132038 hymir-0.1.7/hymir/config.py
--rw-r--r--   0        0        0      344 2024-04-22 17:58:46.132038 hymir-0.1.7/hymir/errors.py
--rw-r--r--   0        0        0     9250 2024-04-22 17:58:46.132038 hymir-0.1.7/hymir/executor.py
--rw-r--r--   0        0        0        0 2024-04-22 17:58:46.132038 hymir-0.1.7/hymir/executors/__init__.py
--rw-r--r--   0        0        0     8560 2024-04-22 17:58:46.132038 hymir-0.1.7/hymir/executors/celery.py
--rw-r--r--   0        0        0     8072 2024-04-22 17:58:46.136038 hymir-0.1.7/hymir/job.py
--rw-r--r--   0        0        0      146 2024-04-22 17:58:46.136038 hymir-0.1.7/hymir/types.py
--rw-r--r--   0        0        0      373 2024-04-22 17:58:46.136038 hymir-0.1.7/hymir/utils.py
--rw-r--r--   0        0        0     1564 2024-04-22 17:58:46.136038 hymir-0.1.7/hymir/visualize.py
--rw-r--r--   0        0        0     7742 2024-04-22 17:58:46.136038 hymir-0.1.7/hymir/workflow.py
--rw-r--r--   0        0        0      692 2024-04-22 17:58:46.136038 hymir-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 hymir-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-29 23:44:25.868806 hymir-0.1.8/LICENSE
+-rw-r--r--   0        0        0      464 2024-05-29 23:44:25.868806 hymir-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/__init__.py
+-rw-r--r--   0        0        0     1092 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/config.py
+-rw-r--r--   0        0        0      344 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/errors.py
+-rw-r--r--   0        0        0     9250 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/executor.py
+-rw-r--r--   0        0        0        0 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/executors/__init__.py
+-rw-r--r--   0        0        0     9355 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/executors/celery.py
+-rw-r--r--   0        0        0     8412 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/job.py
+-rw-r--r--   0        0        0      146 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/types.py
+-rw-r--r--   0        0        0      373 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/utils.py
+-rw-r--r--   0        0        0     1564 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/visualize.py
+-rw-r--r--   0        0        0     7742 2024-05-29 23:44:25.872806 hymir-0.1.8/hymir/workflow.py
+-rw-r--r--   0        0        0      692 2024-05-29 23:44:25.872806 hymir-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 hymir-0.1.8/PKG-INFO
```

### Comparing `hymir-0.1.7/LICENSE` & `hymir-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hymir-0.1.7/hymir/config.py` & `hymir-0.1.8/hymir/config.py`

 * *Files identical despite different names*

### Comparing `hymir-0.1.7/hymir/executor.py` & `hymir-0.1.8/hymir/executor.py`

 * *Files identical despite different names*

### Comparing `hymir-0.1.7/hymir/executors/celery.py` & `hymir-0.1.8/hymir/executors/celery.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import random
 import traceback
 from functools import partial
 from typing import Optional
 
-from celery import shared_task
+from celery import shared_task, Task
 from celery.utils import gen_unique_id
 from celery.utils.log import get_task_logger
 
 from hymir.config import get_configuration
 from hymir.job import Success, Failure, Retry, CheckLater
 
 from hymir.errors import InvalidJobReturn, InvalidWorkflow, WorkflowDoesNotExist
@@ -28,30 +28,44 @@
         this file, or the tasks will not be available to the Celery worker.
         You can do this by adding the following to your Celery configuration:
 
         .. code-block:: python
 
             celery_app.autodiscover_tasks(["hymir.executors.celery"])
 
+    :param queue: The name of the queue to use for the workflow's main monitor
+                  task. [default: None]
+    :param priority: The priority of the workflow's main monitor task.
+                     [default: None]
     """
 
+    def __init__(
+        self, *, queue: Optional[str] = None, priority: Optional[int] = None
+    ):
+        self.queue = queue
+        self.priority = priority
+
     def run(self, workflow: Workflow) -> str:
         workflow_id = gen_unique_id()
         self.store_workflow(workflow_id, workflow)
 
         state = self.workflow_state(workflow_id)
         state.status = WorkflowState.Status.RUNNING
         self.store_workflow_state(workflow_id, state)
 
-        monitor_workflow.delay(workflow_id=workflow_id)
+        monitor_workflow.apply_async(
+            kwargs={"workflow_id": workflow_id},
+            queue=self.queue,
+            priority=self.priority,
+        )
         return workflow_id
 
 
-@shared_task()
-def monitor_workflow(*, workflow_id: str, iterations: int = 1):
+@shared_task(bind=True)
+def monitor_workflow(self: Task, *, workflow_id: str, iterations: int = 1):
     """
     Monitor the progress of a workflow, identified by the `workflow_id`.
 
     Once started, this task will re-run itself until the workflow has
     completed. As dependencies in the workflow are resolved, this task will
     start tasks that were previously blocked by the dependency until the entire
     workflow is complete.
@@ -103,15 +117,18 @@
             continue
 
         state.status = JobState.Status.STARTING
         CeleryExecutor.store_job_state(workflow_id, job_id, state)
         jobs_to_start.append(job_id)
 
     for job_id in jobs_to_start:
-        job_wrapper.delay(workflow_id, job_id)
+        job_wrapper.apply_async(
+            args=(workflow_id, job_id),
+            **(workflow[job_id].meta or {}).get("celery", {}),
+        )
 
     if all(job.is_finished for job in jobs.values()):
         ws.status = WorkflowState.Status.SUCCESS
         if on_finished:
             on_finished(
                 crumb_getter=partial(
                     _crumb_getter,
@@ -127,14 +144,16 @@
     if not ws.is_finished:
         # If running an excessive number of workflows, the usage of countdown
         # here may lead to memory issues on workers due to Celery pretfetching
         # tasks that need scheduling.
         monitor_workflow.apply_async(
             kwargs={"workflow_id": workflow_id, "iterations": iterations + 1},
             countdown=min(iterations * 2, 60),
+            queue=self.request.delivery_info["routing_key"],
+            priority=self.request.delivery_info["priority"],
         )
 
 
 @shared_task()
 def job_wrapper(workflow_id: str, job_id: str):
     """
     Wrapper around a job to handle the state transitions and dependencies.
@@ -194,14 +213,15 @@
         CeleryExecutor.store_job_state(workflow_id, job_id, state)
 
         job_wrapper.apply_async(
             (workflow_id, job_id),
             countdown=random.randint(
                 max(0, ret.wait_min), max(1, ret.wait_max)
             ),
+            **(job.meta or {}).get("celery", {}),
         )
     elif isinstance(ret, CheckLater):
         # The job is not ready to run yet, so we'll check back later.
         # This is useful for implementing workflows that are waiting for
         # external events to occur before they can proceed. We don't consider
         # this a retry, so we don't increment the retry count.
         state.status = JobState.Status.PENDING
```

### Comparing `hymir-0.1.7/hymir/job.py` & `hymir-0.1.8/hymir/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,17 @@
     kwargs: dict = dataclasses.field(default_factory=dict)
     # If provided, the output of the job will be stored in this variable,
     # which can be used as the input to other jobs.
     output: str = None
     # If provided, the keyword arguments that match these strings will be
     # replaced with matching outputs from other jobs.
     inputs: list[str] = None
+    # Extra metadata about the job, typically used to provide executor-specific
+    # overrides.
+    meta: dict = None
 
     def __call__(self, crumb_getter: Callable[[str], Any] = None):
         mod_name, func_name = self.name.rsplit(".", 1)
         mod = __import__(mod_name, fromlist=[func_name])
         func = getattr(mod, func_name)
 
         kwargs = self.kwargs
@@ -174,27 +177,29 @@
         return cls(
             name=data["n"],
             identity=data["i"],
             args=data["a"],
             kwargs=data["k"],
             output=data[">"],
             inputs=data["<"],
+            meta=data.get("m", {}),
         )
 
     def serialize(self):
         """
         Serialize the job to a dictionary.
         """
         return {
             "n": self.name,
             "i": self.identity,
             "a": self.args,
             "k": self.kwargs,
             ">": self.output,
             "<": self.inputs,
+            "m": self.meta,
         }
 
     def with_output(self, name: str) -> "Job":
         """
         Capture the output of this job in a variable, replacing any existing
         output variable if one is set.
 
@@ -206,14 +211,20 @@
         """
         Bind the inputs of this job to the outputs of other jobs.
 
         :param inputs: The names of the outputs to bind to the inputs.
         """
         return dataclasses.replace(self, inputs=list(inputs))
 
+    def with_meta(self, **meta: Any) -> "Job":
+        """
+        Add metadata to the job.
+        """
+        return dataclasses.replace(self, meta=meta)
+
     def set(self, *args, **kwargs: Any) -> "Job":
         """
         Set the arguments for the job.
         """
         return dataclasses.replace(self, args=args, kwargs=kwargs)
 
     @classmethod
```

### Comparing `hymir-0.1.7/hymir/visualize.py` & `hymir-0.1.8/hymir/visualize.py`

 * *Files identical despite different names*

### Comparing `hymir-0.1.7/hymir/workflow.py` & `hymir-0.1.8/hymir/workflow.py`

 * *Files identical despite different names*

### Comparing `hymir-0.1.7/pyproject.toml` & `hymir-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hymir"
-version = "0.1.7"
+version = "0.1.8"
 description = "Simple workflows."
 authors = ["Tyler Kennedy <tk@tkte.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `hymir-0.1.7/PKG-INFO` & `hymir-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymir
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple workflows.
 License: MIT
 Author: Tyler Kennedy
 Author-email: tk@tkte.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

