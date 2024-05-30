# Comparing `tmp/nadl-1.5.3.tar.gz` & `tmp/nadl-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.5.3.tar", last modified: Wed May 29 23:41:11 2024, max compression
+gzip compressed data, was "nadl-1.5.4.tar", last modified: Thu May 30 02:58:19 2024, max compression
```

## Comparing `nadl-1.5.3.tar` & `nadl-1.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2302 2024-05-29 23:41:11.746863 nadl-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.3/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.3/src/nadl/.DS_Store
--rw-r--r--   0        0        0     2019 2024-05-29 23:40:41.702308 nadl-1.5.3/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.3/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.3/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.3/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.3/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.3/src/nadl/loops.py
--rw-r--r--   0        0        0     8707 2024-05-29 23:40:12.442008 nadl-1.5.3/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.3/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.3/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.3/src/nadl/py.typed
--rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.3/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.3/src/nadl/transformers.py
--rw-r--r--   0        0        0     2693 2024-05-29 21:56:24.398032 nadl-1.5.3/src/nadl/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-05-30 02:58:19.380451 nadl-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.4/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.4/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2169 2024-05-30 02:56:53.683385 nadl-1.5.4/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.4/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.4/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.4/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.4/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.4/src/nadl/loops.py
+-rw-r--r--   0        0        0     9159 2024-05-30 02:37:05.286003 nadl-1.5.4/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.4/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.4/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.4/src/nadl/py.typed
+-rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.4/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.4/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2693 2024-05-29 21:56:24.398032 nadl-1.5.4/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.4/PKG-INFO
```

### Comparing `nadl-1.5.3/pyproject.toml` & `nadl-1.5.4/pyproject.toml`

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
-version = "1.5.3"
+version = "1.5.4"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.5.3/readme.org` & `nadl-1.5.4/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/.DS_Store` & `nadl-1.5.4/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/__init__.py` & `nadl-1.5.4/src/nadl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,20 +36,24 @@
 """
 
 from .data import DState, IdxDataloader, es_loop
 from .keys import Keys, new_key
 from .loops import PG, RESC, PGThread
 from .metrics import (
   AbstractMetric,
+  AccRocPR,
+  Accuracy,
   GroupMetric,
   Metric,
+  average_precision_score,
+  convert,
   dice_coef,
   iou_coef,
-  Accuracy,
-  AccRocPR,
+  pr_auc_score,
+  roc_auc_score,
 )
 from .preprocessing import (
   SCALER,
   identity_scaler,
   min_max_scaler,
   normalizer,
   select_scaler,
@@ -60,15 +64,15 @@
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.5.3"
+__version__ = "1.5.4"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "AbstractMetric",
   "AccRocPR",
@@ -76,23 +80,27 @@
   "BaseTrainState",
   "DState",
   "GroupMetric",
   "IdxDataloader",
   "Keys",
   "Metric",
   "PGThread",
+  "average_precision_score",
   "classit",
+  "convert",
   "dice_coef",
   "es_loop",
   "filter_concat",
   "identity_scaler",
   "iou_coef",
   "min_max_scaler",
   "new_key",
   "normalizer",
   "pformat",
+  "pr_auc_score",
   "rle",
   "rle_array",
+  "roc_auc_score",
   "select_scaler",
   "standard_scaler",
   "state_fn",
 ]
```

### Comparing `nadl-1.5.3/src/nadl/blocks.py` & `nadl-1.5.4/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/data.py` & `nadl-1.5.4/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/images.py` & `nadl-1.5.4/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/keys.py` & `nadl-1.5.4/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/loops.py` & `nadl-1.5.4/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/metrics.py` & `nadl-1.5.4/src/nadl/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,31 +109,34 @@
     ),
   )
   return jax.pure_callback(
     m.auc, jax.ShapeDtypeStruct((), jnp.float32), recall, precision
   )
 
 
-class AbstractMetric(Module):
+class AbstractMetric[**P](Module):
   """Abstract Metric."""
 
   name: AbstractVar[str | None]
 
   @abstractmethod
   def __or__(self, value: Self) -> Self:
     """Or."""
     raise NotImplementedError
 
   @abstractmethod
   def __add__(self, value: Self) -> Self:
     """Add."""
     raise NotImplementedError
 
-  @abstractmethod
-  def best(self) -> Self:
+  def best(self, *args: P.args, **kwgs: P.kwargs) -> Self:
+    """Best value."""
+    return self[self.best_idx(*args, **kwgs)]
+
+  def best_idx(self, *args: P.args, **kwgs: P.kwargs) -> Int[Array, "1"]:
     """Best value."""
     raise NotImplementedError
 
   def __repr__(self) -> str:
     """Representation."""
     return tree_pformat(self, short_arrays=False)
 
@@ -167,18 +170,14 @@
     """Best value."""
     return jnp.nanargmax(self.value)
 
   def _min(self) -> Int[Array, "1"]:
     """Worst value."""
     return jnp.nanargmin(self.value)
 
-  def best(self) -> Self:
-    """Best value."""
-    return self[self.best_idx()]
-
   def best_idx(self) -> Int[Array, "1"]:
     """Best value."""
     return self._max() if self.order == "max" else self._min()
 
   def __repr__(self) -> str:
     """Representation."""
     return tree_pformat(self, short_arrays=False)
@@ -207,14 +206,22 @@
       case 1:
         return cls(value=jnp.mean(target == pred), name=name)
       case 2:
         return cls(value=jnp.mean(target == pred, axis=1), name=name)
       case _:
         raise ValueError(f"Unsupported shape: {target.shape=}")
 
+  @classmethod
+  def create_empty(cls, name: str = "accuracy") -> Self:
+    """Create empty."""
+    return cls(
+      value=jnp.nan,
+      name=name
+    )
+
 
 class GroupMetric(AbstractMetric):
   """Group Metric."""
 
   metrics: list[AbstractMetric]
   name: str | None = None
 
@@ -233,19 +240,17 @@
 
   def __getitem__(self, idx: int | Array | slice) -> Self:
     """Get item."""
     return tree_at(
       lambda x: x.metrics, self, jax.tree.map(operator.itemgetter(idx), self.metrics)
     )
 
-  def best(self, which: int | Callable[[list[Metric]], Metric]) -> Self:
-    """Best value."""
-    return self[self.best_idx(which)]
-
-  def best_idx(self, which: int | Callable[[list[Metric]], Metric]) -> Int[Array, "1"]:
+  def best_idx(
+    self, which: int | Callable[[list[AbstractMetric]], Metric]
+  ) -> Int[Array, "1"]:
     """Best value."""
     match which:
       case Callable():
         return which(self.metrics).best_idx()
       case int():
         return self.metrics[which].best_idx()
       case _:
@@ -256,15 +261,15 @@
   """Accuracy, ROC, PR."""
 
   @classmethod
   def create(
     cls,
     target: Num[Array, "*b a"],
     pred: Num[Array, "*b a"],
-    name: str = "rocpr",
+    name: str = "accrocpr",
   ) -> Self:
     """Create from data."""
     if target.shape != pred.shape:
       raise ValueError(f"Shape not match: {target.shape=} != {pred.shape=}")
     match target.ndim:
       case 1:
         return cls(
@@ -285,14 +290,27 @@
             Metric(value=filter_vmap(average_precision_score)(target, pred), name="ap"),
           ],
           name=name,
         )
       case _:
         raise ValueError(f"Unsupported shape: {target.shape=}")
 
+  @classmethod
+  def create_empty(cls, name: str = "accrocpr") -> Self:
+    """Create empty."""
+    return cls(
+      metrics=[
+        Metric(value=jnp.nan, name="acc"),
+        Metric(value=jnp.nan, name="roc"),
+        Metric(value=jnp.nan, name="pr"),
+        Metric(value=jnp.nan, name="ap"),
+      ],
+      name=name
+    )
+
 
 def dice_coef(y_true: jax.Array, y_pred: jax.Array, eps: float = 1e-8) -> jax.Array:
   """Compute dice coefficient."""
   y_true = jnp.asarray(y_true)
   y_pred = jnp.asarray(y_pred)
 
   intersection = jnp.sum(y_true * y_pred)
```

### Comparing `nadl-1.5.3/src/nadl/nets.py` & `nadl-1.5.4/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/preprocessing.py` & `nadl-1.5.4/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/states.py` & `nadl-1.5.4/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/transformers.py` & `nadl-1.5.4/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/src/nadl/utils.py` & `nadl-1.5.4/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.3/PKG-INFO` & `nadl-1.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.5.3
+Version: 1.5.4
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

