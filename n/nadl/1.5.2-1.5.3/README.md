# Comparing `tmp/nadl-1.5.2.tar.gz` & `tmp/nadl-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.5.2.tar", last modified: Wed May 29 22:55:53 2024, max compression
+gzip compressed data, was "nadl-1.5.3.tar", last modified: Wed May 29 23:41:11 2024, max compression
```

## Comparing `nadl-1.5.2.tar` & `nadl-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2302 2024-05-29 22:55:53.693534 nadl-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.2/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.2/src/nadl/.DS_Store
--rw-r--r--   0        0        0     2019 2024-05-29 22:55:25.953875 nadl-1.5.2/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.2/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.2/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.2/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.2/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.2/src/nadl/loops.py
--rw-r--r--   0        0        0     8675 2024-05-29 22:49:07.632528 nadl-1.5.2/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.2/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.2/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.2/src/nadl/py.typed
--rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.2/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.2/src/nadl/transformers.py
--rw-r--r--   0        0        0     2693 2024-05-29 21:56:24.398032 nadl-1.5.2/src/nadl/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-05-29 23:41:11.746863 nadl-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.3/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.3/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2019 2024-05-29 23:40:41.702308 nadl-1.5.3/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.3/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.3/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.3/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.3/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.3/src/nadl/loops.py
+-rw-r--r--   0        0        0     8707 2024-05-29 23:40:12.442008 nadl-1.5.3/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.3/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.3/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.3/src/nadl/py.typed
+-rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.3/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.3/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2693 2024-05-29 21:56:24.398032 nadl-1.5.3/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.3/PKG-INFO
```

### Comparing `nadl-1.5.2/pyproject.toml` & `nadl-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.14",
     "scikit-learn>=1.5.0",
 ]
 requires-python = ">=3.12"
-version = "1.5.2"
+version = "1.5.3"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.5.2/readme.org` & `nadl-1.5.3/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/.DS_Store` & `nadl-1.5.3/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/__init__.py` & `nadl-1.5.3/src/nadl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.5.2"
+__version__ = "1.5.3"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "AbstractMetric",
   "AccRocPR",
```

### Comparing `nadl-1.5.2/src/nadl/blocks.py` & `nadl-1.5.3/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/data.py` & `nadl-1.5.3/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/images.py` & `nadl-1.5.3/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/keys.py` & `nadl-1.5.3/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/loops.py` & `nadl-1.5.3/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/metrics.py` & `nadl-1.5.3/src/nadl/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     raise NotImplementedError
 
   def __repr__(self) -> str:
     """Representation."""
     return tree_pformat(self, short_arrays=False)
 
   @abstractmethod
-  def __getitem__(self, idx: int | Int[Array, "#b"]) -> Self:
+  def __getitem__(self, idx: int | Int[Array, "#b"] | slice) -> Self:
     """Get item."""
     raise NotImplementedError
 
 
 class Metric(AbstractMetric):
   """Base Metric."""
 
@@ -179,15 +179,15 @@
     """Best value."""
     return self._max() if self.order == "max" else self._min()
 
   def __repr__(self) -> str:
     """Representation."""
     return tree_pformat(self, short_arrays=False)
 
-  def __getitem__(self, idx: int | Int[Array, "#b"]) -> Self:
+  def __getitem__(self, idx: int | Int[Array, "#b"] | slice) -> Self:
     """Get item."""
     if self.value is None:
       raise ValueError("No value.")
     return tree_at(lambda x: x.value, self, self.value[idx])
 
 
 class Accuracy(Metric):
@@ -211,15 +211,15 @@
       case _:
         raise ValueError(f"Unsupported shape: {target.shape=}")
 
 
 class GroupMetric(AbstractMetric):
   """Group Metric."""
 
-  metrics: list[Metric]
+  metrics: list[AbstractMetric]
   name: str | None = None
 
   def __or__(self, value: Self) -> Self:
     """Or."""
     if tree_equal(*jax.tree.map(jnp.shape, [self.metrics, value.metrics])):
       s1, _ = partition(self, lambda x: is_array(x) and (not jnp.isnan(x).all()))
       return combine(s1, value)
@@ -227,15 +227,15 @@
 
   def __add__(self, value: Self) -> Self:
     """Add."""
     if self.name != value.name:
       raise ValueError(f"Name not match: this {self.name=} != {value.name=}")
     return filter_concat([self, value])
 
-  def __getitem__(self, idx: int | Array) -> Self:
+  def __getitem__(self, idx: int | Array | slice) -> Self:
     """Get item."""
     return tree_at(
       lambda x: x.metrics, self, jax.tree.map(operator.itemgetter(idx), self.metrics)
     )
 
   def best(self, which: int | Callable[[list[Metric]], Metric]) -> Self:
     """Best value."""
```

### Comparing `nadl-1.5.2/src/nadl/nets.py` & `nadl-1.5.3/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/preprocessing.py` & `nadl-1.5.3/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/states.py` & `nadl-1.5.3/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/transformers.py` & `nadl-1.5.3/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/src/nadl/utils.py` & `nadl-1.5.3/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.2/PKG-INFO` & `nadl-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.5.2
+Version: 1.5.3
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

