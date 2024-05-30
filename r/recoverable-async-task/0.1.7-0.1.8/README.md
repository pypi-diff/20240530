# Comparing `tmp/recoverable_async_task-0.1.7.tar.gz` & `tmp/recoverable_async_task-0.1.8.tar.gz`

## Comparing `recoverable_async_task-0.1.7.tar` & `recoverable_async_task-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/recoverable_async_task.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/.gitignore
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/README.md
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11555 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.8/recoverable_async_task.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.8/.gitignore
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.8/README.md
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 recoverable_async_task-0.1.8/PKG-INFO
```

### Comparing `recoverable_async_task-0.1.7/recoverable_async_task.py` & `recoverable_async_task-0.1.8/recoverable_async_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,15 @@
 
     def __init__(
         self,
         task_function: Callable[[ID_T], Coroutine[None, None, T]],
         max_workers: int = 10,
         max_qps: float = 0,
         retry_n: int = 3,
+        raise_after_retry=False,
         checkpoint_path_name: str | None = None,
     ) -> None:
         """
         Initialize a RecoverableAsyncTask instance.
 
         Parameters:
         - task_function: A coroutine function that takes an int or str as input and returns a result.
@@ -294,15 +295,17 @@
 
         @functools.wraps(task_function)
         async def _task_with_checkpoint(id: ID_T):
             result = await task_function(id)
             self.checkpoint.add(result, id=id)
             return result
 
-        super().__init__(_task_with_checkpoint, max_workers, max_qps, retry_n)
+        super().__init__(
+            _task_with_checkpoint, max_workers, max_qps, retry_n, raise_after_retry
+        )
 
     def push(self, id: ID_T):
         """
         Push a task with the given ID to be processed if it hasn't been processed before.
 
         Parameters:
         - id: ID of the task to be processed.
```

### Comparing `recoverable_async_task-0.1.7/README.md` & `recoverable_async_task-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,9 +55,14 @@
 You may notice that even with `retry_n=3` set, some tasks may still fail due to random issues. In such cases, you can simply execute the tasks again, and they will automatically read the checkpoint file and resume from where they were interrupted. You can repeat this process manually or programmatically until all tasks are successfully completed.
 
 ## Contributing Guidelines
 
 If you wish to contribute to the `recoverable-async-task` library, please follow the setup instructions below to prepare your development environment:
 
 ```bash
-source dev-setup.sh
+source setup-env-rye.sh
 ```
+
+## plan
+
+[] Support custom progress bar statistics
+[] Supports passing in custom error handling logic
```

### Comparing `recoverable_async_task-0.1.7/pyproject.toml` & `recoverable_async_task-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `recoverable_async_task-0.1.7/PKG-INFO` & `recoverable_async_task-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: recoverable-async-task
-Version: 0.1.7
+Version: 0.1.8
 Summary: `recoverable-async-task` is a Python library that streamlines the handling of asynchronous tasks through its `RecoverableAsyncTask` class, with the added benefit of **supporting task checkpointing and resumption**. This feature ensures that tasks can pick up from where they left off in the event of unexpected failures.
 Project-URL: Homepage, https://github.com/Haskely/recoverable-async-task
 Project-URL: Bug Reports, https://github.com/Haskely/recoverable-async-task/issues
 Project-URL: Source, https://github.com/Haskely/recoverable-async-task
 Author-email: Haskely <Haskely@live.com>
 Requires-Python: >=3.10
 Requires-Dist: loguru>=0.7.2
@@ -69,9 +69,14 @@
 You may notice that even with `retry_n=3` set, some tasks may still fail due to random issues. In such cases, you can simply execute the tasks again, and they will automatically read the checkpoint file and resume from where they were interrupted. You can repeat this process manually or programmatically until all tasks are successfully completed.
 
 ## Contributing Guidelines
 
 If you wish to contribute to the `recoverable-async-task` library, please follow the setup instructions below to prepare your development environment:
 
 ```bash
-source dev-setup.sh
+source setup-env-rye.sh
 ```
+
+## plan
+
+[] Support custom progress bar statistics
+[] Supports passing in custom error handling logic
```

