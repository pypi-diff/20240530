# Comparing `tmp/processing_pypelines-0.0.59.tar.gz` & `tmp/processing_pypelines-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing_pypelines-0.0.59.tar", last modified: Tue May 28 16:22:55 2024, max compression
+gzip compressed data, was "processing_pypelines-0.0.60.tar", last modified: Wed May 29 21:12:05 2024, max compression
```

## Comparing `processing_pypelines-0.0.59.tar` & `processing_pypelines-0.0.60.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/LICENSE
--rw-r--r--   0        0        0      118 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/README.md
--rw-r--r--   0        0        0     1152 2024-05-28 16:22:55.231646 processing_pypelines-0.0.59/pyproject.toml
--rw-r--r--   0        0        0      367 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/src/pypelines/__init__.py
--rw-r--r--   0        0        0     4483 2024-05-28 16:22:45.799740 processing_pypelines-0.0.59/src/pypelines/accessors.py
--rw-r--r--   0        0        0     4671 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/arguments.py
--rw-r--r--   0        0        0    34226 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/celery_tasks.py
--rw-r--r--   0        0        0    11851 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/disk.py
--rw-r--r--   0        0        0     6647 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/examples.py
--rw-r--r--   0        0        0   352259 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/feature_test.ipynb
--rw-r--r--   0        0        0     7880 2024-05-28 16:22:45.803740 processing_pypelines-0.0.59/src/pypelines/graphs.py
--rw-r--r--   0        0        0    17073 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/loggs.py
--rw-r--r--   0        0        0     5985 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/multisession.py
--rw-r--r--   0        0        0    18914 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/pickle_backend.py
--rw-r--r--   0        0        0     6559 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/pipelines.py
--rw-r--r--   0        0        0     9444 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/pipes.py
--rw-r--r--   0        0        0     3084 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/sessions.py
--rw-r--r--   0        0        0    37032 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/steps.py
--rw-r--r--   0        0        0     3915 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/tasks.py
--rw-r--r--   0        0        0     7360 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/src/pypelines/versions.py
--rw-r--r--   0        0        0        0 2024-05-28 16:22:45.879739 processing_pypelines-0.0.59/tests/__init__.py
--rw-r--r--   0        0        0      962 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/tests/tests.py
--rw-r--r--   0        0        0     1230 2024-05-28 16:22:45.807740 processing_pypelines-0.0.59/tests/versions_example.json
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.59/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-29 21:11:56.073603 processing_pypelines-0.0.60/LICENSE
+-rw-r--r--   0        0        0      118 2024-05-29 21:11:56.073603 processing_pypelines-0.0.60/README.md
+-rw-r--r--   0        0        0     1152 2024-05-29 21:12:05.097519 processing_pypelines-0.0.60/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/__init__.py
+-rw-r--r--   0        0        0     4483 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/accessors.py
+-rw-r--r--   0        0        0     4671 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/arguments.py
+-rw-r--r--   0        0        0    34226 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/celery_tasks.py
+-rw-r--r--   0        0        0    11851 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/disk.py
+-rw-r--r--   0        0        0     6647 2024-05-29 21:11:56.077603 processing_pypelines-0.0.60/src/pypelines/examples.py
+-rw-r--r--   0        0        0   352259 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/feature_test.ipynb
+-rw-r--r--   0        0        0     7880 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/graphs.py
+-rw-r--r--   0        0        0    17073 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/loggs.py
+-rw-r--r--   0        0        0     5985 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/multisession.py
+-rw-r--r--   0        0        0    18914 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/pickle_backend.py
+-rw-r--r--   0        0        0     6662 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/pipelines.py
+-rw-r--r--   0        0        0     9547 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/pipes.py
+-rw-r--r--   0        0        0     3084 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/sessions.py
+-rw-r--r--   0        0        0    37044 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/steps.py
+-rw-r--r--   0        0        0     3915 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/tasks.py
+-rw-r--r--   0        0        0     7360 2024-05-29 21:11:56.081603 processing_pypelines-0.0.60/src/pypelines/versions.py
+-rw-r--r--   0        0        0        0 2024-05-29 21:11:56.133603 processing_pypelines-0.0.60/tests/__init__.py
+-rw-r--r--   0        0        0      962 2024-05-29 21:11:56.085603 processing_pypelines-0.0.60/tests/tests.py
+-rw-r--r--   0        0        0     1230 2024-05-29 21:11:56.085603 processing_pypelines-0.0.60/tests/versions_example.json
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 processing_pypelines-0.0.60/PKG-INFO
```

### Comparing `processing_pypelines-0.0.59/LICENSE` & `processing_pypelines-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/pyproject.toml` & `processing_pypelines-0.0.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 maintainers = [
     { name = "Timothé Jost-Mousseau", email = "timothe.jost-mousseau@pasteur.fr" },
 ]
 description = "Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api"
 readme = "README.md"
 requires-python = ">=3.10"
 dynamic = []
-version = "0.0.59"
+version = "0.0.60"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 celery = [
     "celery>=5.3.5",
```

### Comparing `processing_pypelines-0.0.59/src/pypelines/accessors.py` & `processing_pypelines-0.0.60/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/arguments.py` & `processing_pypelines-0.0.60/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/celery_tasks.py` & `processing_pypelines-0.0.60/src/pypelines/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/disk.py` & `processing_pypelines-0.0.60/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/examples.py` & `processing_pypelines-0.0.60/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/feature_test.ipynb` & `processing_pypelines-0.0.60/src/pypelines/feature_test.ipynb`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/graphs.py` & `processing_pypelines-0.0.60/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/loggs.py` & `processing_pypelines-0.0.60/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/multisession.py` & `processing_pypelines-0.0.60/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/pickle_backend.py` & `processing_pypelines-0.0.60/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/pipelines.py` & `processing_pypelines-0.0.60/src/pypelines/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 
 if TYPE_CHECKING:
     from .pipes import BasePipe
     from .steps import BaseStep
     from .graphs import PipelineGraph
 
 
-class Pipeline:
+class PipelineType(Protocol):
+
+    def __getattr__(self, name: str) -> "BasePipe": ...
+
+
+class Pipeline(PipelineType):
     pipes: Dict[str, "BasePipe"]
     runner_backend_class = BaseTaskBackend
 
     def __init__(self, name: str, **runner_args):
         """Initialize the pipeline with the given name and runner arguments.
 
         Args:
```

### Comparing `processing_pypelines-0.0.59/src/pypelines/pipes.py` & `processing_pypelines-0.0.60/src/pypelines/pipes.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 from typing import Callable, Type, Iterable, Protocol, TYPE_CHECKING, Literal, Dict
 from types import MethodType
 
 if TYPE_CHECKING:
     from .pipelines import Pipeline
 
 
-class BasePipe(metaclass=ABCMeta):
+class BasePipeType(Protocol):
+
+    def __getattr__(self, name: str) -> "BaseStep": ...
+
+
+class BasePipe(BasePipeType, metaclass=ABCMeta):
     # this class must implements only the logic to link steps together.
 
     default_extra = None
 
     # single_step: bool = False  # a flag to tell the initializer to bind the unique step of this pipe in place
     # of the pipe itself, to the registered pipeline.
     step_class: Type[BaseStep] = BaseStep
```

### Comparing `processing_pypelines-0.0.59/src/pypelines/sessions.py` & `processing_pypelines-0.0.60/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/steps.py` & `processing_pypelines-0.0.60/src/pypelines/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .arguments import autoload_arguments
 
 import logging, inspect
 from pandas import DataFrame
 from dataclasses import dataclass
 
 from types import MethodType
-from typing import Callable, Type, Iterable, Protocol, List, TYPE_CHECKING
+from typing import Callable, Type, Iterable, Protocol, List, TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from .pipelines import Pipeline
     from .pipes import BasePipe
     from .disk import BaseDiskObject
     from .tasks import BaseStepTaskManager
 
@@ -240,15 +240,15 @@
             strict: A boolean flag indicating whether to strictly load the disk object (default is False).
 
         Returns:
             The wrapped function for loading disk objects.
         """
 
         @wraps(self.pipe.disk_class.load)
-        def wrapper(session, extra=None, strict=False):
+        def wrapper(session, extra=None, strict=False) -> Any:
             """Wrapper function to load disk object with session and optional extra parameters.
 
             Args:
                 session: The session to use for loading the disk object.
                 extra (optional): Extra parameters to be passed for loading the disk object. Defaults to None.
                 strict (bool, optional): Flag to indicate strict loading. Defaults to False.
```

### Comparing `processing_pypelines-0.0.59/src/pypelines/tasks.py` & `processing_pypelines-0.0.60/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/src/pypelines/versions.py` & `processing_pypelines-0.0.60/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/tests/tests.py` & `processing_pypelines-0.0.60/tests/tests.py`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/tests/versions_example.json` & `processing_pypelines-0.0.60/tests/versions_example.json`

 * *Files identical despite different names*

### Comparing `processing_pypelines-0.0.59/PKG-INFO` & `processing_pypelines-0.0.60/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.59
+Version: 0.0.60
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Home-page: https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Author-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 Maintainer-Email: =?utf-8?q?Timoth=C3=A9_Jost-Mousseau?= <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: Homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: Repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

