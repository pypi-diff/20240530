# Comparing `tmp/nadl-1.5.5.tar.gz` & `tmp/nadl-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.5.5.tar", last modified: Thu May 30 05:25:26 2024, max compression
+gzip compressed data, was "nadl-1.5.6.tar", last modified: Thu May 30 18:15:22 2024, max compression
```

## Comparing `nadl-1.5.5.tar` & `nadl-1.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2302 2024-05-30 05:25:26.610291 nadl-1.5.5/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.5/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.5/src/nadl/.DS_Store
--rw-r--r--   0        0        0     2169 2024-05-30 05:24:56.505746 nadl-1.5.5/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.5/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.5/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.5/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.5/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.5/src/nadl/loops.py
--rw-r--r--   0        0        0     9714 2024-05-30 05:23:40.076474 nadl-1.5.5/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.5/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.5/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.5/src/nadl/py.typed
--rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.5/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.5/src/nadl/transformers.py
--rw-r--r--   0        0        0     2693 2024-05-29 21:56:24.398032 nadl-1.5.5/src/nadl/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-05-30 18:15:22.024683 nadl-1.5.6/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.6/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.6/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2113 2024-05-30 18:14:45.467011 nadl-1.5.6/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.6/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.6/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.6/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.6/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.6/src/nadl/loops.py
+-rw-r--r--   0        0        0     5264 2024-05-30 18:13:31.214975 nadl-1.5.6/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.6/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.6/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.6/src/nadl/py.typed
+-rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.6/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.6/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.5.6/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.6/PKG-INFO
```

### Comparing `nadl-1.5.5/pyproject.toml` & `nadl-1.5.6/pyproject.toml`

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
-version = "1.5.5"
+version = "1.5.6"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.5.5/readme.org` & `nadl-1.5.6/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/.DS_Store` & `nadl-1.5.6/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/__init__.py` & `nadl-1.5.6/src/nadl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,18 +35,15 @@
 NADL
 """
 
 from .data import DState, IdxDataloader, es_loop
 from .keys import Keys, new_key
 from .loops import PG, RESC, PGThread
 from .metrics import (
-  AbstractMetric,
-  AccRocPR,
   Accuracy,
-  GroupMetric,
   Metric,
   average_precision_score,
   convert,
   dice_coef,
   iou_coef,
   pr_auc_score,
   roc_auc_score,
@@ -57,37 +54,37 @@
   min_max_scaler,
   normalizer,
   select_scaler,
   standard_scaler,
 )
 from .states import BaseTrainState, state_fn
 from .utils import (
+  all_array,
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.5.5"
+__version__ = "1.5.6"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
-  "AbstractMetric",
-  "AccRocPR",
   "Accuracy",
   "BaseTrainState",
   "DState",
-  "GroupMetric",
   "IdxDataloader",
   "Keys",
   "Metric",
+  "Metric",
   "PGThread",
+  "all_array",
   "average_precision_score",
   "classit",
   "convert",
   "dice_coef",
   "es_loop",
   "filter_concat",
   "identity_scaler",
```

### Comparing `nadl-1.5.5/src/nadl/blocks.py` & `nadl-1.5.6/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/data.py` & `nadl-1.5.6/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/images.py` & `nadl-1.5.6/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/keys.py` & `nadl-1.5.6/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/loops.py` & `nadl-1.5.6/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/nets.py` & `nadl-1.5.6/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/preprocessing.py` & `nadl-1.5.6/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/states.py` & `nadl-1.5.6/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/transformers.py` & `nadl-1.5.6/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.5/src/nadl/utils.py` & `nadl-1.5.6/src/nadl/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,9 +89,14 @@
 def filter_concat[T](
   xs: Sequence[T],
   filter_spec: Callable[[Any], bool] = eqx.is_array,
   select_idx: int = -1,
 ) -> T:
   """Filter concat."""
   t1, t2 = eqx.partition(xs, filter_spec=filter_spec)
-  t1 = jax.tree.map(lambda *x: jnp.r_[x], *t1)
+  t1 = jax.tree.map(lambda *x: jnp.r_[*x], *t1)
   return eqx.combine(t1, t2[select_idx])
+
+
+def all_array(x: PyTree) -> list[jax.Array]:
+  """All array."""
+  return jax.tree.leaves(eqx.filter(x, eqx.is_array))
```

### Comparing `nadl-1.5.5/PKG-INFO` & `nadl-1.5.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.5.5
+Version: 1.5.6
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

