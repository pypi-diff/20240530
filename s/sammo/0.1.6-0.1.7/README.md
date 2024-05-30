# Comparing `tmp/sammo-0.1.6.tar.gz` & `tmp/sammo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sammo-0.1.6.tar", max compression
+gzip compressed data, was "sammo-0.1.7.tar", max compression
```

## Comparing `sammo-0.1.6.tar` & `sammo-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1141 2024-03-28 17:14:20.281101 sammo-0.1.6/LICENSE
--rw-r--r--   0        0        0     4419 2024-03-28 17:14:20.281101 sammo-0.1.6/README.md
--rw-r--r--   0        0        0     1841 2024-03-28 17:14:20.281101 sammo-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1388 2024-03-28 17:14:20.281101 sammo-0.1.6/sammo/__init__.py
--rw-r--r--   0        0        0    13149 2024-03-28 17:14:20.281101 sammo-0.1.6/sammo/base.py
--rw-r--r--   0        0        0     8341 2024-03-28 17:14:20.281101 sammo-0.1.6/sammo/compactbars.py
--rw-r--r--   0        0        0     2043 2024-03-28 17:14:20.281101 sammo-0.1.6/sammo/compactbars_test.py
--rw-r--r--   0        0        0    11881 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/components.py
--rw-r--r--   0        0        0      776 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/components_test.py
--rw-r--r--   0        0        0    14788 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/data.py
--rw-r--r--   0        0        0     5265 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/data_tests.py
--rw-r--r--   0        0        0    11530 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/dataformatters.py
--rw-r--r--   0        0        0     5253 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/dataformatters_test.py
--rw-r--r--   0        0        0    16511 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/extractors.py
--rw-r--r--   0        0        0     3459 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/extractors_test.py
--rw-r--r--   0        0        0     8473 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/instructions.py
--rw-r--r--   0        0        0     4526 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/instructions_test.py
--rw-r--r--   0        0        0    35556 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/mutators.py
--rw-r--r--   0        0        0     1445 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/mutators_test.py
--rw-r--r--   0        0        0    17948 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/runners.py
--rw-r--r--   0        0        0     4354 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/runners_test.py
--rw-r--r--   0        0        0     4307 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/scheduler.py
--rw-r--r--   0        0        0    18219 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/search.py
--rw-r--r--   0        0        0     4264 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/search_op.py
--rw-r--r--   0        0        0     1698 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/search_op_test.py
--rw-r--r--   0        0        0     7344 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/store.py
--rw-r--r--   0        0        0     3563 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/store_test.py
--rw-r--r--   0        0        0     9171 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/throttler.py
--rw-r--r--   0        0        0     3405 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/throttler_test.py
--rw-r--r--   0        0        0     3523 2024-03-28 17:14:20.285101 sammo-0.1.6/sammo/utils.py
--rw-r--r--   0        0        0     5700 1970-01-01 00:00:00.000000 sammo-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1141 2024-05-30 20:28:44.079116 sammo-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4419 2024-05-30 20:28:44.079116 sammo-0.1.7/README.md
+-rw-r--r--   0        0        0     1881 2024-05-30 20:28:44.083116 sammo-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1434 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/__init__.py
+-rw-r--r--   0        0        0    13181 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/base.py
+-rw-r--r--   0        0        0     8475 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/compactbars.py
+-rw-r--r--   0        0        0     2043 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/compactbars_test.py
+-rw-r--r--   0        0        0    12029 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/components.py
+-rw-r--r--   0        0        0      776 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/components_test.py
+-rw-r--r--   0        0        0    14863 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/data.py
+-rw-r--r--   0        0        0     5265 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/data_tests.py
+-rw-r--r--   0        0        0    11565 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/dataformatters.py
+-rw-r--r--   0        0        0     5253 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/dataformatters_test.py
+-rw-r--r--   0        0        0    16546 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/extractors.py
+-rw-r--r--   0        0        0     3459 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/extractors_test.py
+-rw-r--r--   0        0        0     8508 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/instructions.py
+-rw-r--r--   0        0        0     4526 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/instructions_test.py
+-rw-r--r--   0        0        0    35606 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/mutators.py
+-rw-r--r--   0        0        0     1445 2024-05-30 20:28:44.083116 sammo-0.1.7/sammo/mutators_test.py
+-rw-r--r--   0        0        0    18033 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/runners.py
+-rw-r--r--   0        0        0     4354 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/runners_test.py
+-rw-r--r--   0        0        0     4322 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/scheduler.py
+-rw-r--r--   0        0        0    18269 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/search.py
+-rw-r--r--   0        0        0     4299 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/search_op.py
+-rw-r--r--   0        0        0     1698 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/search_op_test.py
+-rw-r--r--   0        0        0     7391 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/store.py
+-rw-r--r--   0        0        0     3563 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/store_test.py
+-rw-r--r--   0        0        0     9241 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/throttler.py
+-rw-r--r--   0        0        0     3420 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/throttler_test.py
+-rw-r--r--   0        0        0     3523 2024-05-30 20:28:44.087116 sammo-0.1.7/sammo/utils.py
+-rw-r--r--   0        0        0     5880 1970-01-01 00:00:00.000000 sammo-0.1.7/PKG-INFO
```

### Comparing `sammo-0.1.6/LICENSE` & `sammo-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/README.md` & `sammo-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/pyproject.toml` & `sammo-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "sammo"
-version = "0.1.6"
+version = "0.1.7"
 description = "A flexible, easy-to-use library for running and optimizing prompts for Large Language Models (LLMs)."
 authors = ["Tobias Schnabel"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/microsoft/sammo/"
 documentation = "https://microsoft.github.io/sammo/docs/"
 packages = [
     { include = "sammo" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11,<3.12"
+python = "^3.9,<3.12"
 beartype = "^0.15"
 benepar = {version = "^0.2", optional = true}
 filelock = "^3.12"
 frozendict = "^2.3"
 jsonpath_ng = "^1.5"
 markdown-it-py = "^2.2"
 more-itertools = "^10.1"
@@ -26,14 +26,16 @@
 pyglove = "^0.4"
 spacy = "^3.6"
 tabulate = "^0.9"
 xmltodict = "^0.13"
 PyYAML = "^6.0"
 aiohttp = "^3.6"
 diskcache = "^5.2"
+quattro = "^24"
+async-timeout = "^4.0.3"
 
 [tool.poetry.extras]
 parser = ["benepar"]
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `sammo-0.1.6/sammo/__init__.py` & `sammo-0.1.7/sammo/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 import logging
 import beartype
+from beartype.typing import Union
 import sammo.utils as utils
 from pathlib import Path
 
 PROMPT_LOGGER_NAME = "prompt_logger"
 
 
 @beartype.beartype
 def setup_logger(
-    default_level: int | str = "DEBUG",
+    default_level: Union[int, str] = "DEBUG",
     log_prompts_to_file: bool = False,
-    prompt_level: int | str = "DEBUG",
+    prompt_level: Union[int, str] = "DEBUG",
     prompt_logfile_name: str = None,
 ) -> logging.Logger:
     if log_prompts_to_file:
         if prompt_logfile_name is None:
             prompt_logfile_name = (utils.MAIN_PATH / "logs" / utils.MAIN_NAME).with_suffix(".log")
         log_prompts_to_file = Path(prompt_logfile_name)
         log_prompts_to_file.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `sammo-0.1.6/sammo/base.py` & `sammo-0.1.7/sammo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+from __future__ import annotations
 import abc
 import copy
 import re
 
-from beartype.typing import Callable, Self
+from beartype.typing import Callable, Any
 from frozendict import frozendict
 import pyglove as pg
 import pybars
 from tabulate import tabulate
 
 # monkey-patch pybars to disable HTML escaping
 pybars.Compiler._builder.add_escaped_expand = pybars.Compiler._builder.add_expand
@@ -190,15 +191,15 @@
     __slots__ = "query", "child_selector"
 
     def __init__(self, query, child_selector=None):
         self.query = query
         self.child_selector = child_selector
 
     @classmethod
-    def from_path(cls, path_descriptor: str | dict | Self):
+    def from_path(cls, path_descriptor: str | dict | Any):
         if isinstance(path_descriptor, CompiledQuery):
             return path_descriptor
         elif isinstance(path_descriptor, str):
             path_descriptor = {"regex": path_descriptor}
         child_selector = path_descriptor.pop("_child", None)
         if path_descriptor.get("regex", None) is not None:
             regex = path_descriptor["regex"]
@@ -232,15 +233,15 @@
     Args:
         child: Child component. This can be another component or a string.
         name: The name of the component. If not provided, the class name is used.
     """
 
     NEEDS_SCHEDULING = False
 
-    def __init__(self, child: Self | str, name: str | None = None):
+    def __init__(self, child: Any | str, name: str | None = None):
         if name is None:
             self._name = self.__class__.__name__
         else:
             self._name = name
 
         # auto convert strings
         if isinstance(child, (list, tuple)):
```

### Comparing `sammo-0.1.6/sammo/compactbars.py` & `sammo-0.1.7/sammo/compactbars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """
 Provides a way of displaying multiple progress bars in a single line. Works in both interactive and non-interactive
 environments.
 """
+from __future__ import annotations
 import collections
 import datetime
 import io
 import math
 import shutil
 import sys
 import time
 from beartype import beartype
+from beartype.typing import Union
 
 from sammo import utils
 
 __all__ = ["CompactProgressBars", "SubProgressBar"]
 
 
 @beartype
@@ -187,15 +189,15 @@
     """
     A class that represents a set of progress bars drawn next to each in a single line.
 
     :param width: The total width of the progress bar layout in characters.
     :param refresh_interval: The minimum time interval between display refreshes.
     """
 
-    def __init__(self, width: int | None = None, refresh_interval: float = 1 / 50):
+    def __init__(self, width: Union[int, None] = None, refresh_interval: float = 1 / 50):
         self._bars = collections.OrderedDict()
         self._printer = LinePrinter()
         self._last_update = 0
         self._refresh_interval = refresh_interval
 
         if width is None:
             self._width = self._printer.get_terminal_width()
@@ -211,15 +213,20 @@
     def _should_refresh(self) -> bool:
         if time.monotonic() - self._last_update > self._refresh_interval:
             self._last_update = time.monotonic()
             return True
         return False
 
     def get(
-        self, id: str, total: int | None = None, position: int | None = None, display_name: str | None = None, **kwargs
+        self,
+        id: str,
+        total: Union[int, None] = None,
+        position: Union[int, None] = None,
+        display_name: Union[str, None] = None,
+        **kwargs,
     ) -> SubProgressBar:
         """
         Gets existing or creates a new progress bar given an id.
 
         :param id: The id of the progress bar for later reference.
         :param total: Number of increments.
         :param position: Truncate existing bars beyond index and insert this one at the position.
```

### Comparing `sammo-0.1.6/sammo/compactbars_test.py` & `sammo-0.1.7/sammo/compactbars_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/components.py` & `sammo-0.1.7/sammo/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+from __future__ import annotations
 import asyncio
+import quattro
 import logging
 import math
 import warnings
 
 import beartype
 from beartype.typing import Callable, Literal
+from beartype.typing import Union as TUnion
 from frozendict import frozendict
 
 import sammo.utils as utils
 from sammo.base import (
     Component,
     LLMResult,
     ListComponent,
@@ -45,16 +48,16 @@
 
     NEEDS_SCHEDULING = True
 
     def __init__(
         self,
         child: ScalarComponent,
         name=None,
-        system_prompt: str | None = None,
-        history: ScalarComponent | None = None,
+        system_prompt: TUnion[str, None] = None,
+        history: TUnion[ScalarComponent, None] = None,
         seed=0,
         randomness: float = 0,
         max_tokens=None,
         json_mode: bool = False,
         on_error: Literal["raise", "empty_result"] = "empty_result",
     ):
         super().__init__(child, name)
@@ -158,15 +161,15 @@
         collection = await self._collection(runner, context, dynamic_context)
         tasks = []
         if dynamic_context is None:
             dynamic_context = {}
         if not isinstance(collection, list):
             collection = [collection]
 
-        async with asyncio.TaskGroup() as tg:
+        async with quattro.TaskGroup() as tg:
             for x in collection:
                 tasks.append(
                     tg.create_task(
                         self._operator(
                             runner,
                             context,
                             frozendict({**dynamic_context, self._loop_variable: x}),
@@ -231,18 +234,18 @@
         self.row_batch_size = minibatch_size
         self.reshaping_needed = minibatch_size > 1
         self._on_error = on_error
 
     def run(
         self,
         runner: Runner,
-        data: DataTable | list | None = None,
-        progress_callback: Callable | bool = True,
+        data: TUnion[DataTable, list, None] = None,
+        progress_callback: TUnion[Callable, bool] = True,
         priority: int = 0,
-        on_error: Literal["raise", "empty_result", "backoff"] | None = None,
+        on_error: TUnion[Literal["raise", "empty_result", "backoff"], None] = None,
     ) -> DataTable:
         """Synchronous version of `arun`."""
         return utils.sync(self.arun(runner, data, progress_callback, priority, on_error))
 
     def n_minibatches(self, table: DataTable) -> int:
         """Return the number of minibatches that will be run on the given table.
 
@@ -250,18 +253,18 @@
         """
         n_rows = len(table)
         return math.ceil(n_rows / self.row_batch_size)
 
     async def arun(
         self,
         runner: Runner,
-        data: DataTable | list | None = None,
-        progress_callback: Callable | bool = True,
+        data: TUnion[DataTable, list, None] = None,
+        progress_callback: TUnion[Callable, bool] = True,
         priority: int = 0,
-        on_error: Literal["raise", "empty_result", "backoff"] | None = None,
+        on_error: TUnion[Literal["raise", "empty_result", "backoff"], None] = None,
     ):
         """
         Run the component asynchronously and return a DataTable with the results.
 
         :param runner: The runner to use.
         :param data: The input data to run on. Can be empty.
         :param progress_callback: Called after each minibatch. If True, shows default progress bar.
```

### Comparing `sammo-0.1.6/sammo/components_test.py` & `sammo-0.1.7/sammo/components_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/data.py` & `sammo-0.1.7/sammo/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """
 DataTables are the primary data structure used in SAMMO.
 They are essentially a wrapper around a list of inputs and outputs (labels), with some additional functionality.
 """
+from __future__ import annotations
 import copy
 import hashlib
 import math
 
 from beartype import beartype
-from beartype.typing import Callable, Iterator, Self
+from beartype.typing import Callable, Iterator, Union
 import more_itertools
 import orjson
 import pyglove as pg
 import random
 import tabulate
 
 from sammo.utils import serialize_json
@@ -32,16 +33,16 @@
 
 
 @beartype
 class DataTable(pg.JSONConvertible):
     def __init__(
         self,
         inputs: list,
-        outputs: list | None = None,
-        constants: dict | None = None,
+        outputs: Union[list, None] = None,
+        constants: Union[dict, None] = None,
         seed=42,
     ):
         inputs = DataTable._ensure_list(inputs)
         outputs = DataTable._ensure_list(outputs or [None] * len(inputs))
 
         if len(inputs) != len(outputs):
             raise ValueError(f"Input fields have {len(inputs)} rows, but output fields have {len(outputs)} rows.")
@@ -69,15 +70,15 @@
 
     @property
     def outputs(self):
         """Access output data."""
         return self._outputs
 
     @property
-    def constants(self) -> dict | None:
+    def constants(self) -> Union[dict, None]:
         """Access constants."""
         return self._data["constants"]
 
     def to_json(self, **kwargs):
         """Convert to a JSON-serializable object.
 
         .. note::
@@ -97,17 +98,17 @@
         data = json_value["records"]
         return cls.from_records(data, constants=json_value["constants"], seed=json_value["seed"])
 
     @classmethod
     def from_pandas(
         cls,
         df: "pandas.DataFrame",
-        output_fields: list[str] | str = "output",
-        input_fields: list[str] | str | None = None,
-        constants: dict | None = None,
+        output_fields: Union[list[str], str] = "output",
+        input_fields: Union[list[str], str, None] = None,
+        constants: Union[dict, None] = None,
         seed=42,
     ):
         """Create a DataTable from a pandas DataFrame.
 
         :param df: Pandas DataFrame.
         :param input_fields: Columns from pandas DataFrame that will be used as inputs.
         :param output_fields: Columns that will be used as outputs or targets (e.g., labels).
@@ -126,16 +127,16 @@
         max_idx = len(self)
         return list(range(key.start or 0, min(key.stop or max_idx, max_idx), key.step or 1))
 
     @classmethod
     def from_records(
         cls,
         records: list[dict],
-        output_fields: list[str] | str = "output",
-        input_fields: list[str] | str | None = None,
+        output_fields: Union[list[str], str] = "output",
+        input_fields: Union[list[str], str, None] = None,
         **kwargs,
     ):
         if len(records) == 0:
             return cls(records, **kwargs)
 
         if input_fields is None:
             input_fields = [k for k in records[0].keys() if k not in output_fields]
@@ -191,28 +192,28 @@
             table = tabulate.tabulate(
                 table_data[:max_rows], headers="keys", maxcolwidths=max_col_width, tablefmt="grid"
             )
         else:
             table = "<empty DataTable>"
         return f"{table}\nConstants: {DataTable._truncate(self.constants, max_col_width)}"
 
-    def _to_explicit_idx(self, key: int | slice | list[int]):
+    def _to_explicit_idx(self, key: Union[int, slice, list[int]]):
         if isinstance(key, int):
             return [key]
         elif isinstance(key, slice):
             key = self._slice_to_explicit_idx(key)
         return key
 
     def __getitem__(self, key):
         idx = self._to_explicit_idx(key)
         new_inputs = [self._data["inputs"][i] for i in idx]
         new_outputs = [self._data["outputs"][i] for i in idx]
         return DataTable(new_inputs, new_outputs, self.constants, self._seed)
 
-    def sample(self, k: int, seed: int | None = None) -> Self:
+    def sample(self, k: int, seed: Union[int, None] = None):
         """Sample rows without replacement.
 
         :param k: Number of rows to sample.
         :param seed: Random seed. If not provided, instance seed is used.
         """
         if k > len(self):
             raise ValueError("Sample size must be less than or equal to the number of rows.")
@@ -220,15 +221,15 @@
             rng = random.Random(seed)
         else:
             rng = self._rng
         selected_idx = rng.sample(range(len(self)), k=k)
 
         return self[selected_idx]
 
-    def shuffle(self, seed: int | None = None) -> Self:
+    def shuffle(self, seed: Union[int, None] = None):
         """Shuffle rows.
 
         :param seed: Random seed. If not provided, instance seed is used.
         """
         return self.sample(len(self), seed=seed)
 
     def random_split(self, *sizes: int, seed=None) -> tuple:
@@ -238,15 +239,15 @@
         :param seed: Random seed. If not provided, instance seed is used.
         :return: Tuple of splits.
         """
         sampled = self.sample(sum(sizes), seed=seed)
         splits = [slice(sum(sizes[:i]), sum(sizes[: i + 1])) for i in range(len(sizes))]
         return tuple(sampled[split] for split in splits)
 
-    def copy(self) -> Self:
+    def copy(self):
         return copy.deepcopy(self)
 
     def get_minibatch_iterator(self, minibatch_size):
         return MinibatchIterator(self, minibatch_size)
 
 
 DataTable.register("DataTable", DataTable)
```

### Comparing `sammo-0.1.6/sammo/data_tests.py` & `sammo-0.1.7/sammo/data_tests.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/dataformatters.py` & `sammo-0.1.7/sammo/dataformatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """
 DataFormatters are components that take a DataTable or dict and format it into a string. They also provide a
 get_extractor method that can be used to parse the LLM responses in this format.
 
 """
+from __future__ import annotations
 import collections
 import json
 
 from beartype.typing import Sequence, Literal
 from frozendict import frozendict
 import xmltodict
```

### Comparing `sammo-0.1.6/sammo/dataformatters_test.py` & `sammo-0.1.7/sammo/dataformatters_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/extractors.py` & `sammo-0.1.7/sammo/extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """
 This module contains components that extract data from the output of other components, typically from LLM calls.
 Common formats such as JSON, XML, or Markdown are supported and require no data format specification. If validation is
 required, it should happen downstream of the extraction step.
 """
+from __future__ import annotations
 import abc
 import ast
 import fractions
 import json
 import logging
 import re
```

### Comparing `sammo-0.1.6/sammo/extractors_test.py` & `sammo-0.1.7/sammo/extractors_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/instructions.py` & `sammo-0.1.7/sammo/instructions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+from __future__ import annotations
 import hashlib
 import math
 
 import numpy as np
 from beartype.typing import Literal, MutableMapping
 from frozendict import frozendict
 import pyglove as pg
```

### Comparing `sammo-0.1.6/sammo/instructions_test.py` & `sammo-0.1.7/sammo/instructions_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/mutators.py` & `sammo-0.1.7/sammo/mutators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+from __future__ import annotations
 import abc
 import asyncio
+import quattro
 import collections
 import logging
 import random
 import re
 import textwrap
 
 from beartype.typing import Callable, Literal, Any
@@ -834,15 +836,15 @@
             selected_mutators = [bag[i] for i in idx]
 
         if n_mutations == 1:
             return await selected_mutators[0].mutate(candidate, data, runner, random_state)
         else:
             selected_mutators = collections.Counter(selected_mutators)
             tasks = list()
-            async with asyncio.TaskGroup() as tg:
+            async with quattro.TaskGroup() as tg:
                 for i, (mut, n_mut) in enumerate(selected_mutators.items()):
                     mut.objective = self._objective
                     tasks.append(tg.create_task(mut.mutate(candidate, data, runner, n_mut, random_state + i)))
             return sum([t.result() for t in tasks], [])
 
 
 class StopwordsCompressor(Component):
```

### Comparing `sammo-0.1.6/sammo/mutators_test.py` & `sammo-0.1.7/sammo/mutators_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/runners.py` & `sammo-0.1.7/sammo/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+from __future__ import annotations
 import abc
 import base64
 import re
 import warnings
 from abc import abstractmethod
 import asyncio
+import async_timeout
 from collections.abc import MutableMapping
 import json
 import logging
 import os
 import pathlib
 from contextlib import asynccontextmanager
 
 import aiohttp
 import orjson
 from beartype import beartype
-from beartype.typing import Literal
+from beartype.typing import Literal, Union
 
 from sammo import PROMPT_LOGGER_NAME
 from sammo.base import LLMResult, Costs, Runner
 from sammo.store import PersistentDict, SqlLiteDict
 from sammo.throttler import AtMost, Throttler
 from sammo.utils import serialize_json
 
@@ -44,15 +46,14 @@
     def __class__(self) -> type:
         return Runner
 
     async def generate_text(self, prompt: str, *args, **kwargs):
         return LLMResult(self.return_value)
 
 
-@beartype
 class BaseRunner(Runner):
     """Base class for OpenAI API runners.
 
     :param model_id: Model specifier as listed in the API documentation.
     :param cache: A dict-like object to use for storing results.
     :param api_config: The path to the API config file or a dictionary containing the API information.
     :param rate_limit: The rate limit to use. If an integer, it specifies max calls per second.
@@ -69,21 +70,21 @@
     RETRY_ERRORS = ()
     DEFAULT_CACHE = PersistentDict
 
     def __init__(
         self,
         model_id: str,
         api_config: dict | str | pathlib.Path,
-        cache: None | MutableMapping | str | os.PathLike = None,
-        equivalence_class: str | Literal["major", "exact"] = "major",
-        rate_limit: AtMost | list[AtMost] | Throttler | int = 2,
+        cache: Union[None, MutableMapping, str, os.PathLike] = None,
+        equivalence_class: Union[str, Literal["major", "exact"]] = "major",
+        rate_limit: Union[AtMost, list[AtMost], Throttler, int] = 2,
         max_retries: int = 50,
-        max_context_window: int | None = None,
+        max_context_window: Union[int, None] = None,
         retry: bool = True,
-        timeout: float | int = 60,
+        timeout: Union[float, int] = 60,
         max_timeout_retries: int = 1,
         use_cached_timeouts: bool = True,
     ):
         super().__init__()
 
         if isinstance(api_config, dict):
             self._api_config = dict(api_config)
@@ -146,15 +147,15 @@
 
             n_timeouts = 0
             for cur_try in range(self._max_retries):
                 retry_on = self._retry_on if cur_try < self._max_retries - 1 else tuple()
 
                 try:
                     job_handle = await self._throttler.wait_in_line(priority)
-                    async with asyncio.timeout(self._timeout):
+                    async with async_timeout.timeout(self._timeout):
                         json = await self._call_backend(request)
                     response_obj = self._llm_result(request, json, fingerprint)
                     response_obj.retries = cur_try
                     self._throttler.update_job_stats(job_handle, cost=response_obj.costs.total)
                     self._costs += response_obj.costs
                     if self._cache is not None:
                         self._cache[fingerprint] = json
```

### Comparing `sammo-0.1.6/sammo/runners_test.py` & `sammo-0.1.7/sammo/runners_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
-from asyncio import TaskGroup
+from quattro import TaskGroup
 from unittest.mock import AsyncMock, MagicMock
 
 import pytest
 
 from sammo.runners import BaseRunner, OpenAIChat, OpenAIEmbedding
 from sammo.base import Costs
 from sammo.store import InMemoryDict
```

### Comparing `sammo-0.1.6/sammo/scheduler.py` & `sammo-0.1.7/sammo/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 import asyncio
+import quattro
 import collections
 import json
 import pathlib
 import webbrowser
 from graphlib import TopologicalSorter
 import logging
 
@@ -132,15 +133,15 @@
         return IFrameRenderer(self._to_html())
 
     async def run_node(self, node):
         await node.job(self._runner, node.compute_context, None)
         await self.finalized_tasks_queue.put(node)
 
     async def arun(self):
-        async with asyncio.TaskGroup() as tg:
+        async with quattro.TaskGroup() as tg:
             while self.tasks.is_active():
                 for compute_node in self.tasks.get_ready():
                     if compute_node.job.NEEDS_SCHEDULING:
                         tg.create_task(self.run_node(compute_node))
                     else:
                         await self.finalized_tasks_queue.put(compute_node)
```

### Comparing `sammo-0.1.6/sammo/search.py` & `sammo-0.1.7/sammo/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
+from __future__ import annotations
 import asyncio
 import collections
 import copy
 import logging
 import random
 from collections.abc import Callable
 import datetime
 from pathlib import Path
+import quattro
 
 from beartype import beartype
 from beartype.typing import Literal
 from orjson import orjson
 import pyglove as pg
 from tabulate import tabulate
 
@@ -175,15 +177,15 @@
         if colbar is None:
             colbar = CompactProgressBars()
         update_when_done = colbar.get("eval", total=len(candidates), position=1, show_time=False).update
         subtasks_total = sum([m.n_minibatches(dataset) for m in candidates])
         subtasks_cb = colbar.get("tasks", total=subtasks_total).update
 
         evaluation_tasks = list()
-        async with asyncio.TaskGroup() as g:
+        async with quattro.TaskGroup() as g:
             for i, candidate in enumerate(candidates):
                 task = g.create_task(candidate.arun(runner, dataset, subtasks_cb, i))
                 task.add_done_callback(update_when_done)
                 evaluation_tasks.append(task)
 
         scored_mutations = list()
         for candidate, y_pred in zip(candidates, evaluation_tasks):
@@ -264,15 +266,15 @@
 
         for d in range(self._depth):
             # Mutate candidates in parallel
             mutation_tasks = list()
             update_pbar = colbar.get("mutate", total=len(active_set), show_time=False, position=1).update
 
             candidates_for_mutation = self._pick_candidates_for_mutation(active_set, rng)
-            async with asyncio.TaskGroup() as g:
+            async with quattro.TaskGroup() as g:
                 for i, x in enumerate(candidates_for_mutation):
                     task = g.create_task(
                         self._mutator.mutate(
                             x["candidate"],
                             dataset,
                             self._runner,
                             n_mutations=self._n_mutations,
@@ -445,15 +447,15 @@
                     "iteration": iteration,
                     "action": action,
                     **self._candidate_record(candidate, dataset, y_pred),
                 }
 
         running_tasks = list()
         total_minibatches = 0
-        async with asyncio.TaskGroup() as tg:
+        async with quattro.TaskGroup() as tg:
             for i, search_context in enumerate(
                 pg.iter(
                     traced_search_space,
                     num_examples=self._max_trials,
                     algorithm=pg.geno.Random(self._random_state) if self._algorithm == "random" else None,
                 ),
             ):
```

### Comparing `sammo-0.1.6/sammo/search_op.py` & `sammo-0.1.7/sammo/search_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """
 This module contains a variety of search operators that can be used to define a discrete search space for `GridSearch`
 or define a set of initial candidates for other search algorithms.
 """
+from __future__ import annotations
 import pyglove as pg
 from sammo.base import Component
 from beartype.typing import Iterable, Any, Callable
 from pyglove.core.hyper import OneOf, ManyOf
 
 __all__ = ["one_of", "many_of", "permutate", "optional", "get_points_from_search_space", "get_first_point"]
```

### Comparing `sammo-0.1.6/sammo/search_op_test.py` & `sammo-0.1.7/sammo/search_op_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/store.py` & `sammo-0.1.7/sammo/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 """Implements two different types of dictionaries that can store either data in memory or on disk. Allows keys to be
 arbitrary JSON-serializable objects that get rendered to byte strings for indexing.
 Mainly used to cache LLM API calls, but can be used for other purposes as well.
 """
+from __future__ import annotations
 from collections.abc import MutableMapping
 from contextlib import ExitStack
 from io import BytesIO
 import logging
 import os
 import threading
 import warnings
 from pathlib import Path
 
 import diskcache
-from beartype.typing import Callable
+from beartype.typing import Callable, Union
 import filelock
 import orjson
 from pyglove import JSONConvertible
 
 from sammo.utils import CodeTimer
 from sammo.utils import serialize_json as serialize_json_obj
 
@@ -196,15 +197,15 @@
     """
     Implements a dictionary that is persisted to disk a SQLite DB. It is a bit slower for shorter entries than using
     PersistentDict which is all buffered in memory, but preferable when storing larger objects, such as vectors.
 
     :param directory: path for the stored data. If none, uses a temporary directory.
     """
 
-    def __init__(self, directory: os.PathLike | str | None = None):
+    def __init__(self, directory: Union[os.PathLike, str, None] = None):
         if directory and Path(directory).exists() and not Path(directory).is_dir():
             raise ValueError(f"{directory} is not a directory.")
         self._filename = directory
         self._dict = diskcache.Cache(directory, eviction_policy="none")
 
     def vacuum(self) -> None:
         pass
```

### Comparing `sammo-0.1.6/sammo/store_test.py` & `sammo-0.1.7/sammo/store_test.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/sammo/throttler.py` & `sammo-0.1.7/sammo/throttler.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 # Licensed under the MIT License.
 """
 Provides a context manager for throttling async jobs. The throttling is defined by a list of AtMost instance and
 can be used to limit the number of concurrent jobs, the number of jobs per time period, the total cost of jobs per
 time period, or the number of failed jobs per time period. The context manager will block until there is capacity
 to run the job. The jobs are run in order of priority, breaking ties with creation time.
 """
+
+from __future__ import annotations
 import asyncio
 import bisect
 from collections import deque
 from dataclasses import dataclass, field
 import enum
 import logging
 import threading
 import time
 
 from beartype import beartype
-from beartype.typing import Literal
+from beartype.typing import Literal, Union
+
 
 __all__ = ["Throttler", "AtMost"]
 
 logger = logging.getLogger(__name__)
 
 
 class JobStatus(enum.Enum):
@@ -64,18 +67,18 @@
 
 
 @beartype
 @dataclass
 class AtMost:
     """Class for defining a throttling limit."""
 
-    value: float | int
+    value: Union[float, int]
     type: Literal["calls", "running", "failed", "rejected"]
-    period: float | int = 1
-    pause_for: float | int = 0
+    period: Union[float, int] = 1
+    pause_for: Union[float, int] = 0
 
 
 @beartype
 class Throttler:
     """Class that provides flexible throttling for async jobs.
 
     :param limits: A list of :class:`sammo.throttler.AtMost` instances that define the throttling limits.
@@ -89,15 +92,15 @@
 
     def __init__(
         self,
         limits: list[AtMost],
         sleep_interval: float = 0.01,
         impute_pending_costs: bool = True,
         n_cost_samples: int = 10,
-        rejection_window: int | float = 0.5,
+        rejection_window: Union[int, float] = 0.5,
     ):
         self._limits = limits
         self._max_history_window = max([x.period for x in limits] + [60])
         self._sleep_interval = sleep_interval
         self._lock = threading.Lock()
         self._task_logs = deque()
         self._wait_list = deque()
@@ -129,15 +132,15 @@
                 break
 
     @staticmethod
     async def sleep(delay: float):
         """A more precise sleep function on Windows"""
         await asyncio.get_running_loop().run_in_executor(None, time.sleep, delay)
 
-    def update_job_stats(self, job: Job, cost: float | int = 0, failed: bool = False) -> None:
+    def update_job_stats(self, job: Job, cost: Union[float, int], failed: bool = False) -> None:
         """Update the stats for a job. Needs to be called when a job is finished.
 
         :param job: Job instance to update.
         :param cost: The cost of the job.
         :param failed: Whether the job failed, default is False.
         """
         job.cost = cost
```

### Comparing `sammo-0.1.6/sammo/throttler_test.py` & `sammo-0.1.7/sammo/throttler_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 import asyncio
+import quattro
 import threading
 import time
 
 import pytest
 from pytest import approx
 
 from sammo.throttler import Throttler, AtMost
@@ -28,44 +29,44 @@
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("n_jobs,completion_time", [(10, 0.1), (11, 0.2), (20, 0.3)])
 async def test_basic_call_limit(n_jobs, completion_time):
     throttler = Throttler([AtMost(10, "calls", 0.1)])
 
-    async with asyncio.TaskGroup() as g:
+    async with quattro.TaskGroup() as g:
         jobs = [g.create_task(simple_job(i, throttler)) for i in range(n_jobs)]
     jobs = [j.result() for j in jobs]
     durations = [j["duration"] for j in jobs]
     # provide a relaxed upper bound for max duration to account for differences
     # in executors across test environments
     assert max(durations) <= (completion_time * 2)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("n_jobs,completion_time", [(10, 0.06), (12, 0.11)])
 async def test_basic_running_limit(n_jobs, completion_time, job_duration=0.05):
     throttler = Throttler([AtMost(10, "running")], sleep_interval=0.001)
 
-    async with asyncio.TaskGroup() as g:
+    async with quattro.TaskGroup() as g:
         jobs = [g.create_task(simple_job(i, throttler, delay=job_duration)) for i in range(n_jobs)]
     jobs = [j.result() for j in jobs]
 
     durations = [j["duration"] for j in jobs]
     # provide a relaxed upper bound for max duration to account for differences
     # in executors across test environments
     assert max(durations) <= (completion_time * 2)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("jobs_with_flags,completion_time", [([True] * 2 + [False] * 5, 0.21)])
 async def test_basic_failed_limit(jobs_with_flags, completion_time):
     throttler = Throttler([AtMost(1, "failed", 0.1)], rejection_window=-1, sleep_interval=0.001)
 
-    async with asyncio.TaskGroup() as g:
+    async with quattro.TaskGroup() as g:
         jobs = [g.create_task(simple_job(i, throttler, fail=j)) for i, j in enumerate(jobs_with_flags)]
     jobs = [j.result() for j in jobs]
 
     durations = [j["duration"] for j in jobs]
     # provide a relaxed upper bound for max duration to account for differences
     # in executors across test environments
     assert max(durations) <= (completion_time * 2)
@@ -75,14 +76,14 @@
 @pytest.mark.parametrize(
     "jobs_with_flags,completion_time",
     [([True, False] * 1, 0.11), ([True] * 2 + [False] * 1, 0.21), ([True] * 1 + [False] * 5, 0.11)],
 )
 async def test_basic_rejected_limit(jobs_with_flags, completion_time):
     throttler = Throttler([AtMost(1, "rejected", 0.1, 0.1)], rejection_window=1, sleep_interval=0.001)
 
-    async with asyncio.TaskGroup() as g:
+    async with quattro.TaskGroup() as g:
         jobs = [g.create_task(simple_job(i, throttler, fail=j)) for i, j in enumerate(jobs_with_flags)]
     jobs = [j.result() for j in jobs]
     durations = [j["duration"] for j in jobs]
     # provide a relaxed upper bound for max duration to account for differences
     # in executors across test environments
     assert max(durations) <= (completion_time * 2)
```

### Comparing `sammo-0.1.6/sammo/utils.py` & `sammo-0.1.7/sammo/utils.py`

 * *Files identical despite different names*

### Comparing `sammo-0.1.6/PKG-INFO` & `sammo-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: sammo
-Version: 0.1.6
+Version: 0.1.7
 Summary: A flexible, easy-to-use library for running and optimizing prompts for Large Language Models (LLMs).
 Home-page: https://github.com/microsoft/sammo/
 License: MIT
 Author: Tobias Schnabel
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: parser
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: aiohttp (>=3.6,<4.0)
+Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: beartype (>=0.15,<0.16)
 Requires-Dist: benepar (>=0.2,<0.3) ; extra == "parser"
 Requires-Dist: diskcache (>=5.2,<6.0)
 Requires-Dist: filelock (>=3.12,<4.0)
 Requires-Dist: frozendict (>=2.3,<3.0)
 Requires-Dist: jsonpath_ng (>=1.5,<2.0)
 Requires-Dist: markdown-it-py (>=2.2,<3.0)
 Requires-Dist: more-itertools (>=10.1,<11.0)
 Requires-Dist: numpy (>=1.25,<2.0)
 Requires-Dist: orjson (>=3.9,<4.0)
 Requires-Dist: pybars3 (>=0.9,<0.10)
 Requires-Dist: pyglove (>=0.4,<0.5)
+Requires-Dist: quattro (>=24,<25)
 Requires-Dist: spacy (>=3.6,<4.0)
 Requires-Dist: tabulate (>=0.9,<0.10)
 Requires-Dist: xmltodict (>=0.13,<0.14)
 Project-URL: Documentation, https://microsoft.github.io/sammo/docs/
 Project-URL: Repository, https://github.com/microsoft/sammo/
 Description-Content-Type: text/markdown
```

