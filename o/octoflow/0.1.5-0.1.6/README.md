# Comparing `tmp/octoflow-0.1.5.tar.gz` & `tmp/octoflow-0.1.6.tar.gz`

## Comparing `octoflow-0.1.5.tar` & `octoflow-0.1.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/config.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/constants.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/core.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/exceptions.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/logging.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/plugin.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/typing.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/base.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/dataclass.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/dataset.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/expression.py
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/loaders.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/metadata.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/sampler.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/schema.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/types.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/__init__.py
--rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/artifact/__init__.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/artifact/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/cache.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/collections.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/config.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/func.py
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/hashing.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/objects.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/rsync.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/string.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.5/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.5/AUTHORS.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.5/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.5/README.md
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/__init__.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/config.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/constants.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/core.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/exceptions.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/logging.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/plugin.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/typing.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/base.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/dataclass.py
+-rw-r--r--   0        0        0    22523 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/dataset.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/expression.py
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/loaders.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/metadata.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/sampler.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/schema.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/data/types.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/tracking/__init__.py
+-rw-r--r--   0        0        0    12441 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/tracking/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/tracking/artifact/__init__.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/tracking/artifact/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/cache.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/collections.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/config.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/func.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/hashing.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/objects.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/rsync.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.6/octoflow/utils/string.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.6/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.6/AUTHORS.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.6/README.md
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.6/PKG-INFO
```

### Comparing `octoflow-0.1.5/octoflow/__init__.py` & `octoflow-0.1.6/octoflow/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import contextlib
 
 from octoflow import logging
 from octoflow.config import config
+from octoflow.core import Module, Task
 from octoflow.utils.config import Config
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 __all__ = [
     "Config",
+    "Module",
+    "Task",
     "config",
     "logger",
     "logging",
 ]
 
 logging.logger = logging.get_logger(
     name="octoflow",
```

### Comparing `octoflow-0.1.5/octoflow/config.py` & `octoflow-0.1.6/octoflow/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     # for user data
     cache: CacheConfig = field(default_factory=CacheConfig)
 
 
 @dataclass
 class LoggingConfig:
     level: str = "INFO"
-    format: str = "%(asctime)s %(levelname)s %(name)s [%(pathname)s:%(lineno)s] %(message)s"
+    format: str = (
+        "%(asctime)s %(levelname)s %(name)s [%(pathname)s:%(lineno)s] "
+        "%(message)s"
+    )
 
 
 @dataclass
 class OctoFlowConfig:
     resources: ResourcesConfig = field(default_factory=ResourcesConfig)
     logging: LoggingConfig = field(default_factory=LoggingConfig)
```

### Comparing `octoflow-0.1.5/octoflow/core.py` & `octoflow-0.1.6/octoflow/core.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/logging.py` & `octoflow-0.1.6/octoflow/logging.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/plugin.py` & `octoflow-0.1.6/octoflow/plugin.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/__init__.py` & `octoflow-0.1.6/octoflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/base.py` & `octoflow-0.1.6/octoflow/data/base.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/dataclass.py` & `octoflow-0.1.6/octoflow/data/dataclass.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/dataset.py` & `octoflow-0.1.6/octoflow/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,34 +362,38 @@
         func : Any
             The function to map over the dataset.
         batch_size : int
             Number of rows to map at a time.
         batched : bool
             Whether the function is batched.
         verbose : bool | int
-            Whether to show a progress bar.
+            Whether to show a progress bar or not. When set to 0, no progress
+            bar is shown. When set to 1, a progress bar is shown but all traces
+            of the progress bar are removed upon termination of iteration. When
+            set to 2, the progress bar is shown and keeps all traces of the
+            progress bar upon termination of iteration
 
         Returns
         -------
         Dataset
             A new dataset containing the mapped rows.
         """
         path = gen_unique_cached_path(
             self.path, func, cache_dir=self.cache_dir
         )
         num_steps = (self.count_rows() + batch_size - 1) // batch_size
         batch_iter = self._wrapped.to_batches(batch_size=batch_size)
-        progress_bar = None
-        if verbose:
-            progress_bar = tqdm.tqdm(
-                batch_iter,
-                total=num_steps,
-                desc=f"Mapping [{path.name}]",
-            )
-        batch_iter = batch_iter if progress_bar is None else progress_bar
+        progress_bar = tqdm.tqdm(
+            batch_iter,
+            total=num_steps,
+            desc=f"Mapping [{path.name}]",
+            disable=int(verbose) < 1,
+            leave=int(verbose) > 1,
+        )
+        batch_iter = progress_bar
         if batched:
             batch_iter = (
                 create_mapped_table(
                     func(batch),
                     batch,
                     keep_cols=keep_cols,
                     exclude_cols=exclude_cols,
@@ -411,17 +415,15 @@
             )
         state = write_dataset(path, batch_iter, format=self.format)
         if not state:
             logger.warning(
                 f"existing dataset found at '{path}', "
                 "loading existing file(s)"
             )
-        if progress_bar is not None:
-            progress_bar.update(num_steps)
-            progress_bar.close()
+        progress_bar.close()
         return type(self).load_dataset(
             path, format=self.format, cache_dir=self.cache_dir
         )
 
     def filter(self, expression: Expression = None) -> Dataset:
         """
         Filter the dataset.
```

### Comparing `octoflow-0.1.5/octoflow/data/expression.py` & `octoflow-0.1.6/octoflow/data/expression.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/loaders.py` & `octoflow-0.1.6/octoflow/data/loaders.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/metadata.py` & `octoflow-0.1.6/octoflow/data/metadata.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/sampler.py` & `octoflow-0.1.6/octoflow/data/sampler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/schema.py` & `octoflow-0.1.6/octoflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/data/types.py` & `octoflow-0.1.6/octoflow/data/types.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/tracking/models.py` & `octoflow-0.1.6/octoflow/tracking/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,20 @@
     get_handler_type,
     get_handler_type_by_object,
     get_handler_type_by_path,
 )
 from octoflow.utils import hashing, string
 from octoflow.utils.collections import flatten
 
+__all__ = [
+    "Experiment",
+    "Run",
+    "RunState",
+]
+
 
 class RunState(enum.Enum):
     COMPLETED = "completed"
     FAILED = "failed"
     RUNNING = "running"
```

### Comparing `octoflow-0.1.5/octoflow/tracking/artifact/handler.py` & `octoflow-0.1.6/octoflow/tracking/artifact/handler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/cache.py` & `octoflow-0.1.6/octoflow/utils/cache.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/collections.py` & `octoflow-0.1.6/octoflow/utils/collections.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/config.py` & `octoflow-0.1.6/octoflow/utils/config.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/func.py` & `octoflow-0.1.6/octoflow/utils/func.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/hashing.py` & `octoflow-0.1.6/octoflow/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/objects.py` & `octoflow-0.1.6/octoflow/utils/objects.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/rsync.py` & `octoflow-0.1.6/octoflow/utils/rsync.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/octoflow/utils/string.py` & `octoflow-0.1.6/octoflow/utils/string.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/.gitignore` & `octoflow-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/LICENSE` & `octoflow-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/README.md` & `octoflow-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/pyproject.toml` & `octoflow-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.5/PKG-INFO` & `octoflow-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoflow
-Version: 0.1.5
+Version: 0.1.6
 Summary: Streamlining machine learning tracking for seamless experiment management.
 Project-URL: Documentation, https://github.com/ysenarath/octoflow
 Project-URL: Source, https://github.com/ysenarath/octoflow
 Author-email: Yasas Senarath <email@example.com>
 License-Expression: MIT
 License-File: AUTHORS.md
 License-File: LICENSE
```

