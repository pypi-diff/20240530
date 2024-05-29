# Comparing `tmp/nadl-1.5.1.tar.gz` & `tmp/nadl-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.5.1.tar", last modified: Wed May 29 18:48:10 2024, max compression
+gzip compressed data, was "nadl-1.5.2.tar", last modified: Wed May 29 22:55:53 2024, max compression
```

## Comparing `nadl-1.5.1.tar` & `nadl-1.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2275 2024-05-29 18:48:10.242432 nadl-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.1/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.1/src/nadl/.DS_Store
--rw-r--r--   0        0        0     1952 2024-05-29 18:47:22.424968 nadl-1.5.1/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.1/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.1/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.1/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.1/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.1/src/nadl/loops.py
--rw-r--r--   0        0        0     5751 2024-05-29 18:06:13.669773 nadl-1.5.1/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.1/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.1/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.1/src/nadl/py.typed
--rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.1/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.1/src/nadl/transformers.py
--rw-r--r--   0        0        0     2699 2024-05-29 17:08:54.829295 nadl-1.5.1/src/nadl/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-05-29 22:55:53.693534 nadl-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.2/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.2/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2019 2024-05-29 22:55:25.953875 nadl-1.5.2/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.2/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.2/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.2/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.2/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.2/src/nadl/loops.py
+-rw-r--r--   0        0        0     8675 2024-05-29 22:49:07.632528 nadl-1.5.2/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.2/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.2/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.2/src/nadl/py.typed
+-rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.2/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.2/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2693 2024-05-29 21:56:24.398032 nadl-1.5.2/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.2/PKG-INFO
```

### Comparing `nadl-1.5.1/pyproject.toml` & `nadl-1.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     "rich>=13.7.1",
     "jaxtyping>=0.2.29",
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.14",
+    "scikit-learn>=1.5.0",
 ]
 requires-python = ">=3.12"
-version = "1.5.1"
+version = "1.5.2"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.5.1/readme.org` & `nadl-1.5.2/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/.DS_Store` & `nadl-1.5.2/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/__init__.py` & `nadl-1.5.2/src/nadl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,15 +34,23 @@
 
 NADL
 """
 
 from .data import DState, IdxDataloader, es_loop
 from .keys import Keys, new_key
 from .loops import PG, RESC, PGThread
-from .metrics import AbstractMetric, GroupMetric, Metric, dice_coef, iou_coef
+from .metrics import (
+  AbstractMetric,
+  GroupMetric,
+  Metric,
+  dice_coef,
+  iou_coef,
+  Accuracy,
+  AccRocPR,
+)
 from .preprocessing import (
   SCALER,
   identity_scaler,
   min_max_scaler,
   normalizer,
   select_scaler,
   standard_scaler,
@@ -52,21 +60,23 @@
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.5.1"
+__version__ = "1.5.2"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "AbstractMetric",
+  "AccRocPR",
+  "Accuracy",
   "BaseTrainState",
   "DState",
   "GroupMetric",
   "IdxDataloader",
   "Keys",
   "Metric",
   "PGThread",
```

### Comparing `nadl-1.5.1/src/nadl/blocks.py` & `nadl-1.5.2/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/data.py` & `nadl-1.5.2/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/images.py` & `nadl-1.5.2/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/keys.py` & `nadl-1.5.2/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/loops.py` & `nadl-1.5.2/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/nets.py` & `nadl-1.5.2/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/preprocessing.py` & `nadl-1.5.2/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/states.py` & `nadl-1.5.2/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/transformers.py` & `nadl-1.5.2/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.1/src/nadl/utils.py` & `nadl-1.5.2/src/nadl/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,24 @@
 filename : utils.py
 project  : nadl
 license  : GPL-3.0+
 
 Utils
 """
 
-from collections.abc import Callable, Mapping, Sequence
-from typing import Any, Literal
+from collections.abc import Callable, Sequence
+
+import equinox as eqx
 import jax
 import jax.numpy as jnp
-from rich.console import Console
+
 from jaxtyping import PyTree
-import equinox as eqx
+from typing import Any, Literal
+
+from rich.console import Console
 
 
 def rle_array(x: jax.Array, shift: int = 1) -> jax.Array:
   """Run length encoding array."""
   x = x.flatten()
   x = jnp.pad(x, (1, 1), mode="constant")
   x = jnp.argwhere(x[1:] != x[:-1]).flatten() + shift
```

### Comparing `nadl-1.5.1/PKG-INFO` & `nadl-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.5.1
+Version: 1.5.2
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: jaxtyping>=0.2.29
 Requires-Dist: optax>=0.2.2
 Requires-Dist: equinox>=0.11.4
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: scikit-image>=0.23.2
 Requires-Dist: orbax-checkpoint>=0.5.14
+Requires-Dist: scikit-learn>=1.5.0
 Requires-Dist: mkdocs-material>=9.5.25; extra == "doc"
 Requires-Dist: mkdocs>=1.6.0; extra == "doc"
 Requires-Dist: mike>=2.1.1; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.25.1; extra == "doc"
 Provides-Extra: doc
 Description-Content-Type: text/plain
```

