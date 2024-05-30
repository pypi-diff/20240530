# Comparing `tmp/fjformer-0.0.8.tar.gz` & `tmp/fjformer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fjformer-0.0.8.tar", last modified: Thu Nov 23 11:31:42 2023, max compression
+gzip compressed data, was "fjformer-0.0.9.tar", last modified: Thu Nov 23 13:17:26 2023, max compression
```

## Comparing `fjformer-0.0.8.tar` & `fjformer-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.444800 fjformer-0.0.8/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-11-05 07:38:31.000000 fjformer-0.0.8/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3626 2023-11-23 11:31:42.444800 fjformer-0.0.8/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2960 2023-11-05 07:38:31.000000 fjformer-0.0.8/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.440800 fjformer-0.0.8/fjformer/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      821 2023-11-23 11:28:14.000000 fjformer-0.0.8/fjformer/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.440800 fjformer-0.0.8/fjformer/attention/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      196 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/attention/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7133 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/attention/efficient_attention.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    25511 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/attention/flash_attention_0.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.440800 fjformer-0.0.8/fjformer/bits/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      631 2023-11-23 11:27:44.000000 fjformer-0.0.8/fjformer/bits/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4072 2023-11-23 11:10:47.000000 fjformer-0.0.8/fjformer/bits/bits.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1717 2023-11-23 09:56:15.000000 fjformer-0.0.8/fjformer/bits/calibration.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12529 2023-11-23 11:10:47.000000 fjformer-0.0.8/fjformer/bits/config.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2889 2023-11-23 09:56:15.000000 fjformer-0.0.8/fjformer/bits/int_numerics.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17562 2023-11-23 11:02:42.000000 fjformer-0.0.8/fjformer/bits/q_dot_general.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7919 2023-11-23 11:11:01.000000 fjformer-0.0.8/fjformer/bits/q_flax.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-11-23 09:53:47.000000 fjformer-0.0.8/fjformer/bits/stochastic_rounding.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.440800 fjformer-0.0.8/fjformer/datasets/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       37 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/datasets/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2153 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/datasets/datasets.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.440800 fjformer-0.0.8/fjformer/func/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       74 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/func/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      822 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/func/_func.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    16730 2023-11-06 08:29:46.000000 fjformer-0.0.8/fjformer/func/loss_func.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.444800 fjformer-0.0.8/fjformer/load/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      192 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/load/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3250 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/load/_load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8926 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/load/streamer.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.444800 fjformer-0.0.8/fjformer/monitor/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       82 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/monitor/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2962 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/monitor/tracker.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.444800 fjformer-0.0.8/fjformer/optimizers/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      646 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/optimizers/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8759 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/optimizers/adafactor.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5847 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/optimizers/adamw.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5909 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/optimizers/lion.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1064 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/optimizers/optimizer_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.444800 fjformer-0.0.8/fjformer/partition_utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      367 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/partition_utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7166 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/partition_utils/mesh_utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    46443 2023-11-06 08:35:29.000000 fjformer-0.0.8/fjformer/partition_utils/t5x_partitioning.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1515 2023-11-05 07:38:31.000000 fjformer-0.0.8/fjformer/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 11:31:42.440800 fjformer-0.0.8/fjformer.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3626 2023-11-23 11:31:42.000000 fjformer-0.0.8/fjformer.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1125 2023-11-23 11:31:42.000000 fjformer-0.0.8/fjformer.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-11-23 11:31:42.000000 fjformer-0.0.8/fjformer.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      124 2023-11-23 11:31:42.000000 fjformer-0.0.8/fjformer.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        9 2023-11-23 11:31:42.000000 fjformer-0.0.8/fjformer.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-11-05 07:38:31.000000 fjformer-0.0.8/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-11-23 11:31:42.444800 fjformer-0.0.8/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1205 2023-11-23 11:28:14.000000 fjformer-0.0.8/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.471517 fjformer-0.0.9/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-11-05 07:38:31.000000 fjformer-0.0.9/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3626 2023-11-23 13:17:26.471517 fjformer-0.0.9/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2960 2023-11-05 07:38:31.000000 fjformer-0.0.9/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.467517 fjformer-0.0.9/fjformer/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      821 2023-11-23 13:09:26.000000 fjformer-0.0.9/fjformer/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.467517 fjformer-0.0.9/fjformer/attention/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      196 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/attention/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7133 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/attention/efficient_attention.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    25511 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/attention/flash_attention_0.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.467517 fjformer-0.0.9/fjformer/bits/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      631 2023-11-23 11:27:44.000000 fjformer-0.0.9/fjformer/bits/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4072 2023-11-23 11:10:47.000000 fjformer-0.0.9/fjformer/bits/bits.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1749 2023-11-23 13:09:14.000000 fjformer-0.0.9/fjformer/bits/calibration.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12559 2023-11-23 13:09:14.000000 fjformer-0.0.9/fjformer/bits/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2889 2023-11-23 09:56:15.000000 fjformer-0.0.9/fjformer/bits/int_numerics.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17562 2023-11-23 11:02:42.000000 fjformer-0.0.9/fjformer/bits/q_dot_general.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8046 2023-11-23 13:09:14.000000 fjformer-0.0.9/fjformer/bits/q_flax.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-11-23 09:53:47.000000 fjformer-0.0.9/fjformer/bits/stochastic_rounding.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.471517 fjformer-0.0.9/fjformer/datasets/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       37 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/datasets/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2153 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/datasets/datasets.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.471517 fjformer-0.0.9/fjformer/func/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       74 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/func/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      822 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/func/_func.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    16730 2023-11-06 08:29:46.000000 fjformer-0.0.9/fjformer/func/loss_func.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.471517 fjformer-0.0.9/fjformer/load/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      192 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/load/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3250 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/load/_load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8926 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/load/streamer.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.471517 fjformer-0.0.9/fjformer/monitor/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       82 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/monitor/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2962 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/monitor/tracker.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.471517 fjformer-0.0.9/fjformer/optimizers/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      646 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/optimizers/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8759 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/optimizers/adafactor.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5847 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/optimizers/adamw.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5909 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/optimizers/lion.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1064 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/optimizers/optimizer_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.471517 fjformer-0.0.9/fjformer/partition_utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      367 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/partition_utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7166 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/partition_utils/mesh_utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    46443 2023-11-06 08:35:29.000000 fjformer-0.0.9/fjformer/partition_utils/t5x_partitioning.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1515 2023-11-05 07:38:31.000000 fjformer-0.0.9/fjformer/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-11-23 13:17:26.467517 fjformer-0.0.9/fjformer.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3626 2023-11-23 13:17:26.000000 fjformer-0.0.9/fjformer.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1125 2023-11-23 13:17:26.000000 fjformer-0.0.9/fjformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-11-23 13:17:26.000000 fjformer-0.0.9/fjformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      124 2023-11-23 13:17:26.000000 fjformer-0.0.9/fjformer.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        9 2023-11-23 13:17:26.000000 fjformer-0.0.9/fjformer.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-11-05 07:38:31.000000 fjformer-0.0.9/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-11-23 13:17:26.471517 fjformer-0.0.9/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1205 2023-11-23 13:09:26.000000 fjformer-0.0.9/setup.py
```

### Comparing `fjformer-0.0.8/LICENSE` & `fjformer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/PKG-INFO` & `fjformer-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fjformer
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fjformer-0.0.8/README.md` & `fjformer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/__init__.py` & `fjformer-0.0.9/fjformer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
     transpose, global_norm, average_metrics
 )
 
 from .utils import (
     JaxRNG, GenerateRNG, init_rng, next_rng, count_num_params
 )
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
```

### Comparing `fjformer-0.0.8/fjformer/attention/efficient_attention.py` & `fjformer-0.0.9/fjformer/attention/efficient_attention.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/attention/flash_attention_0.py` & `fjformer-0.0.9/fjformer/attention/flash_attention_0.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/bits/__init__.py` & `fjformer-0.0.9/fjformer/bits/__init__.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/bits/bits.py` & `fjformer-0.0.9/fjformer/bits/bits.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/bits/calibration.py` & `fjformer-0.0.9/fjformer/bits/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Quantization calibration methods."""
 
 import abc
+from typing import Union
+
 import flax.struct
 import jax.numpy as jnp
 
 
 class Calibration(abc.ABC):
 
     @abc.abstractmethod
     def get_bound(self, x, shared_axes) -> jnp.ndarray:
         pass
 
 
 @flax.struct.dataclass
 class ConstantCalibration(Calibration):
-    bound: jnp.ndarray | float
+    bound: Union[jnp.ndarray, float]
 
     def get_bound(self, x, shared_axes) -> jnp.ndarray:
         """Calibration."""
         del shared_axes
         assert self.bound > 0, 'Bound should be positive.'
         return jnp.asarray(self.bound).reshape((1,) * len(x.shape))
```

### Comparing `fjformer-0.0.8/fjformer/bits/config.py` & `fjformer-0.0.9/fjformer/bits/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,16 @@
     if rhs_bits is not None:
         cfg.dlhs.rhs.use_fwd_quant = use_fwd_quant
     return cfg
 
 
 def fully_quantized(
         *,
-        fwd_bits: int | None = 8,
-        bwd_bits: int | None = 8,
+        fwd_bits: Union[int, None] = 8,
+        bwd_bits: Union[int, None] = 8,
         use_fwd_quant: bool = True,
         use_stochastic_rounding: Optional[bool] = True,
         # Typically we have (but it's a caller's responsibility to check):
         # - vjp_lhs_stochastic_rounding is referring to the gradient and
         # - vjp_rhs_stochastic_rounding is referring to the activations/weights.
         vjp_lhs_stochastic_rounding: Optional[bool] = None,
         vjp_rhs_stochastic_rounding: Optional[bool] = None,
@@ -328,17 +328,17 @@
         set_static_bound(cfg, 1.0)
 
     return cfg
 
 
 def config_v3(
         *,
-        fwd_bits: int | None,
-        dlhs_bits: int | None,
-        drhs_bits: int | None,
+        fwd_bits: Union[int, None],
+        dlhs_bits: Union[int, None],
+        drhs_bits: Union[int, None],
         use_dummy_static_bound: bool = False,
         rng_type: str = 'jax.uniform',  # 'custom-1'
         dlhs_local_q: Optional[LocalQ] = None,
         drhs_local_q: Optional[LocalQ] = None,
         fwd_accumulator_dtype: ... = jnp.int32,
         dlhs_accumulator_dtype: ... = jnp.int32,
         drhs_accumulator_dtype: ... = jnp.int32,
```

### Comparing `fjformer-0.0.8/fjformer/bits/int_numerics.py` & `fjformer-0.0.9/fjformer/bits/int_numerics.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/bits/q_dot_general.py` & `fjformer-0.0.9/fjformer/bits/q_dot_general.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/bits/q_flax.py` & `fjformer-0.0.9/fjformer/bits/q_flax.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import functools
 from . import q_dot_general
 from . import calibration
 from . import config
 from . import int_numerics
 import flax.linen as nn
 import jax.numpy as jnp
+from typing import Optional, Union
 
 
 class Freezer(nn.Module, config.Preprocess):
     """Identity function that can freeze its input.
 
     On default it is an identity function that saves the input in a variable.
     In 'use_frozen=True' mode, ignores the input and returns the frozen value. It
@@ -49,16 +50,16 @@
             frozen.value = inputs
         return frozen.value
 
 
 class QDotGeneral(nn.Module):
     """A layer that can be injected into flax.nn.Dense, etc."""
 
-    cfg: config.DotGeneral | None = None
-    prng_name: str | None = 'params'
+    cfg: Optional[Union[config.DotGeneral, None]] = None
+    prng_name: Optional[Union[str, None]] = None
 
     @nn.compact
     def __call__(
             self,
             lhs,
             rhs,
             dimension_numbers,
@@ -77,16 +78,16 @@
             preferred_element_type=preferred_element_type,
         )
 
 
 class QEinsum(nn.Module):
     """Quantized Einsum class for model injection."""
 
-    cfg: config.DotGeneral | None = None
-    prng_name: str | None = 'params'
+    cfg: Optional[Union[config.DotGeneral, None]] = None
+    prng_name: Optional[Union[str, None]] = None
 
     @nn.compact
     def __call__(self, eqn, lhs, rhs):
         key = self.make_rng(self.prng_name) if self.prng_name is not None else None
         context = q_dot_general.Context(key=key, train_step=None)
         q_dg = q_dot_general.make_dot_general(self.cfg)
         q_dg = functools.partial(q_dg, context=context)
@@ -124,32 +125,32 @@
 ):
     cfg.fwd.lhs.preprocess_quant_cls = mk_freezer('lhs', collection, mode)
     cfg.fwd.lhs.preprocess_scale_cls = mk_freezer('lhs_scale', collection, mode)
 
 
 def config_v4(
         *,
-        fwd_bits: int | None,
-        dlhs_bits: int | None,
-        drhs_bits: int | None,
+        fwd_bits: Union[int, None],
+        dlhs_bits: Union[int, None],
+        drhs_bits: Union[int, None],
         # The dummy static bound flag is for performance benchmarking.
         use_dummy_static_bound: bool = False,
         rng_type: str = 'jax.uniform',  # 'custom-1'
-        dlhs_local_q: config.LocalQ | None = None,
-        drhs_local_q: config.LocalQ | None = None,
+        dlhs_local_q: Union[config.LocalQ, None] = None,
+        drhs_local_q: Union[config.LocalQ, None] = None,
         fwd_accumulator_dtype: ... = jnp.int32,
         dlhs_accumulator_dtype: ... = jnp.int32,
         drhs_accumulator_dtype: ... = jnp.int32,
         lhs_quant_mode: QuantMode = QuantMode.DYNAMIC,
         rhs_quant_mode: QuantMode = QuantMode.DYNAMIC,
         freeze_collection: str = 'q',
 ) -> config.DotGeneral:
     """Version 4 of user-visible AQT config."""
 
-    def tensor_config(bits: int | None) -> config.Tensor:
+    def tensor_config(bits: Union[int, None]) -> config.Tensor:
         assert bits is None or bits >= 2, 'Need at least 2 bits.'
         if bits is None:
             numerics = config.NoNumerics()
         else:
             numerics = int_numerics.IntNumerics(
                 bits=bits,
                 preserve_zero=True,
```

### Comparing `fjformer-0.0.8/fjformer/bits/stochastic_rounding.py` & `fjformer-0.0.9/fjformer/bits/stochastic_rounding.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/datasets/datasets.py` & `fjformer-0.0.9/fjformer/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/func/_func.py` & `fjformer-0.0.9/fjformer/func/_func.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/func/loss_func.py` & `fjformer-0.0.9/fjformer/func/loss_func.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/load/_load.py` & `fjformer-0.0.9/fjformer/load/_load.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/load/streamer.py` & `fjformer-0.0.9/fjformer/load/streamer.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/monitor/tracker.py` & `fjformer-0.0.9/fjformer/monitor/tracker.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/optimizers/__init__.py` & `fjformer-0.0.9/fjformer/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/optimizers/adafactor.py` & `fjformer-0.0.9/fjformer/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/optimizers/adamw.py` & `fjformer-0.0.9/fjformer/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/optimizers/lion.py` & `fjformer-0.0.9/fjformer/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/optimizers/optimizer_utils.py` & `fjformer-0.0.9/fjformer/optimizers/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/partition_utils/mesh_utils.py` & `fjformer-0.0.9/fjformer/partition_utils/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/partition_utils/t5x_partitioning.py` & `fjformer-0.0.9/fjformer/partition_utils/t5x_partitioning.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer/utils.py` & `fjformer-0.0.9/fjformer/utils.py`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/fjformer.egg-info/PKG-INFO` & `fjformer-0.0.9/fjformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fjformer
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fjformer-0.0.8/fjformer.egg-info/SOURCES.txt` & `fjformer-0.0.9/fjformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/pyproject.toml` & `fjformer-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fjformer-0.0.8/setup.py` & `fjformer-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fjformer",
-    version='0.0.8',
+    version='0.0.9',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
```

