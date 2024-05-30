# Comparing `tmp/degann-1.1.tar.gz` & `tmp/degann-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degann-1.1.tar", last modified: Thu May 30 12:59:22 2024, max compression
+gzip compressed data, was "degann-1.1.1.tar", last modified: Thu May 30 15:43:36 2024, max compression
```

## Comparing `degann-1.1.tar` & `degann-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.768611 degann-1.1/
--rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-1.1/LICENSE
--rw-rw-rw-   0        0        0     3003 2024-05-30 12:59:22.767610 degann-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2024-05-30 12:53:17.000000 degann-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.745610 degann-1.1/degann/
--rw-rw-rw-   0        0        0      108 2024-05-11 12:06:42.000000 degann-1.1/degann/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.748610 degann-1.1/degann/degann.egg-info/
--rw-rw-rw-   0        0        0     3003 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/requires.txt
--rw-rw-rw-   0        0        0       53 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.751613 degann-1.1/degann/equations/
--rw-rw-rw-   0        0        0       90 2023-09-27 09:30:32.000000 degann-1.1/degann/equations/__init__.py
--rw-rw-rw-   0        0        0     3200 2024-05-30 08:54:39.000000 degann-1.1/degann/equations/equation_utils.py
--rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-1.1/degann/equations/simple_equation.py
--rw-rw-rw-   0        0        0     4162 2024-05-30 08:54:39.000000 degann-1.1/degann/equations/system_ode.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.753610 degann-1.1/degann/expert/
--rw-rw-rw-   0        0        0       25 2024-05-11 11:57:48.000000 degann-1.1/degann/expert/__init__.py
--rw-rw-rw-   0        0        0     3697 2024-05-30 08:28:46.000000 degann-1.1/degann/expert/pipeline.py
--rw-rw-rw-   0        0        0     5066 2024-05-30 12:37:38.000000 degann-1.1/degann/expert/selector.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.759610 degann-1.1/degann/networks/
--rw-rw-rw-   0        0        0      203 2024-03-27 15:04:35.000000 degann-1.1/degann/networks/__init__.py
--rw-rw-rw-   0        0        0     1852 2024-02-26 17:40:53.000000 degann-1.1/degann/networks/activations.py
--rw-rw-rw-   0        0        0     3066 2024-05-30 12:37:38.000000 degann-1.1/degann/networks/callbacks.py
--rw-rw-rw-   0        0        0      465 2024-05-30 09:00:10.000000 degann-1.1/degann/networks/config_format.py
--rw-rw-rw-   0        0        0    13061 2024-05-30 12:37:38.000000 degann-1.1/degann/networks/cpp_utils.py
--rw-rw-rw-   0        0        0    12985 2024-05-30 07:46:52.000000 degann-1.1/degann/networks/imodel.py
--rw-rw-rw-   0        0        0     2153 2024-03-26 15:51:27.000000 degann-1.1/degann/networks/layer_creator.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.760610 degann-1.1/degann/networks/layers/
--rw-rw-rw-   0        0        0       25 2024-03-26 15:51:27.000000 degann-1.1/degann/networks/layers/__init__.py
--rw-rw-rw-   0        0        0     5347 2024-05-30 07:46:52.000000 degann-1.1/degann/networks/layers/tf_dense.py
--rw-rw-rw-   0        0        0     3927 2024-05-30 12:37:38.000000 degann-1.1/degann/networks/losses.py
--rw-rw-rw-   0        0        0     2215 2024-05-30 10:09:34.000000 degann-1.1/degann/networks/metrics.py
--rw-rw-rw-   0        0        0     1128 2024-05-30 10:56:52.000000 degann-1.1/degann/networks/optimizers.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.762610 degann-1.1/degann/networks/topology/
--rw-rw-rw-   0        0        0       28 2024-03-26 15:51:27.000000 degann-1.1/degann/networks/topology/__init__.py
--rw-rw-rw-   0        0        0    14206 2024-05-30 07:46:52.000000 degann-1.1/degann/networks/topology/tf_densenet.py
--rw-rw-rw-   0        0        0     2201 2024-02-26 17:40:53.000000 degann-1.1/degann/networks/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.767610 degann-1.1/degann/search_algorithms/
--rw-rw-rw-   0        0        0      174 2024-05-30 07:46:52.000000 degann-1.1/degann/search_algorithms/__init__.py
--rw-rw-rw-   0        0        0    10642 2024-05-30 12:37:38.000000 degann-1.1/degann/search_algorithms/generate.py
--rw-rw-rw-   0        0        0     8015 2024-05-30 08:12:30.000000 degann-1.1/degann/search_algorithms/grid_search.py
--rw-rw-rw-   0        0        0     2021 2024-05-30 08:12:31.000000 degann-1.1/degann/search_algorithms/nn_code.py
--rw-rw-rw-   0        0        0    10916 2024-05-30 12:37:38.000000 degann-1.1/degann/search_algorithms/pattern_search.py
--rw-rw-rw-   0        0        0     9378 2024-05-30 10:47:43.000000 degann-1.1/degann/search_algorithms/random_search.py
--rw-rw-rw-   0        0        0    10070 2024-05-30 12:37:37.000000 degann-1.1/degann/search_algorithms/simulated_annealing.py
--rw-rw-rw-   0        0        0     1458 2024-05-30 10:56:23.000000 degann-1.1/degann/search_algorithms/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-30 12:59:22.768611 degann-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1504 2024-05-06 17:03:35.000000 degann-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.402185 degann-1.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3005 2024-05-30 15:43:36.402185 degann-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2166 2024-05-30 14:18:28.000000 degann-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.378185 degann-1.1.1/degann/
+-rw-rw-rw-   0        0        0      108 2024-05-30 14:11:47.000000 degann-1.1.1/degann/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.381185 degann-1.1.1/degann/degann.egg-info/
+-rw-rw-rw-   0        0        0     3005 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1219 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.384187 degann-1.1.1/degann/equations/
+-rw-rw-rw-   0        0        0       90 2023-09-27 09:30:32.000000 degann-1.1.1/degann/equations/__init__.py
+-rw-rw-rw-   0        0        0     3200 2024-05-30 14:03:10.000000 degann-1.1.1/degann/equations/equation_utils.py
+-rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-1.1.1/degann/equations/simple_equation.py
+-rw-rw-rw-   0        0        0     4162 2024-05-30 14:03:10.000000 degann-1.1.1/degann/equations/system_ode.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.386185 degann-1.1.1/degann/expert/
+-rw-rw-rw-   0        0        0       50 2024-05-30 14:10:58.000000 degann-1.1.1/degann/expert/__init__.py
+-rw-rw-rw-   0        0        0     3736 2024-05-30 14:28:38.000000 degann-1.1.1/degann/expert/pipeline.py
+-rw-rw-rw-   0        0        0     5066 2024-05-30 14:10:53.000000 degann-1.1.1/degann/expert/selector.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.393187 degann-1.1.1/degann/networks/
+-rw-rw-rw-   0        0        0      203 2024-03-27 15:04:35.000000 degann-1.1.1/degann/networks/__init__.py
+-rw-rw-rw-   0        0        0     1852 2024-02-26 17:40:53.000000 degann-1.1.1/degann/networks/activations.py
+-rw-rw-rw-   0        0        0     3066 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/callbacks.py
+-rw-rw-rw-   0        0        0      467 2024-05-30 15:42:42.000000 degann-1.1.1/degann/networks/config_format.py
+-rw-rw-rw-   0        0        0    13061 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/cpp_utils.py
+-rw-rw-rw-   0        0        0    12985 2024-05-30 14:13:44.000000 degann-1.1.1/degann/networks/imodel.py
+-rw-rw-rw-   0        0        0     2153 2024-03-26 15:51:27.000000 degann-1.1.1/degann/networks/layer_creator.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.395185 degann-1.1.1/degann/networks/layers/
+-rw-rw-rw-   0        0        0       25 2024-03-26 15:51:27.000000 degann-1.1.1/degann/networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     5347 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/layers/tf_dense.py
+-rw-rw-rw-   0        0        0     3927 2024-05-30 14:14:02.000000 degann-1.1.1/degann/networks/losses.py
+-rw-rw-rw-   0        0        0     2215 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/metrics.py
+-rw-rw-rw-   0        0        0     1128 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/optimizers.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.396185 degann-1.1.1/degann/networks/topology/
+-rw-rw-rw-   0        0        0       28 2024-03-26 15:51:27.000000 degann-1.1.1/degann/networks/topology/__init__.py
+-rw-rw-rw-   0        0        0    14206 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/topology/tf_densenet.py
+-rw-rw-rw-   0        0        0     2201 2024-02-26 17:40:53.000000 degann-1.1.1/degann/networks/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.401187 degann-1.1.1/degann/search_algorithms/
+-rw-rw-rw-   0        0        0      174 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/__init__.py
+-rw-rw-rw-   0        0        0    10974 2024-05-30 14:12:27.000000 degann-1.1.1/degann/search_algorithms/generate.py
+-rw-rw-rw-   0        0        0     8015 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/grid_search.py
+-rw-rw-rw-   0        0        0     2021 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/nn_code.py
+-rw-rw-rw-   0        0        0    10916 2024-05-30 14:12:57.000000 degann-1.1.1/degann/search_algorithms/pattern_search.py
+-rw-rw-rw-   0        0        0     9378 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/random_search.py
+-rw-rw-rw-   0        0        0    10070 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/simulated_annealing.py
+-rw-rw-rw-   0        0        0     1458 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 15:43:36.402185 degann-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2024-05-30 15:13:20.000000 degann-1.1.1/setup.py
```

### Comparing `degann-1.1/LICENSE` & `degann-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `degann-1.1/PKG-INFO` & `degann-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 1.1
+Version: 1.1.1
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `degann-1.1/README.md` & `degann-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/degann.egg-info/PKG-INFO` & `degann-1.1.1/degann/degann.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 1.1
+Version: 1.1.1
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `degann-1.1/degann/degann.egg-info/SOURCES.txt` & `degann-1.1.1/degann/degann.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/equations/equation_utils.py` & `degann-1.1.1/degann/equations/equation_utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/equations/simple_equation.py` & `degann-1.1.1/degann/equations/simple_equation.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/equations/system_ode.py` & `degann-1.1.1/degann/equations/system_ode.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/expert/pipeline.py` & `degann-1.1.1/degann/expert/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import List
 
-from degann import random_search_endless, simulated_annealing, grid_search
+from degann.search_algorithms import (
+    random_search_endless,
+    simulated_annealing,
+    grid_search,
+)
 
 
 def execute_pipeline(
     input_size: int,
     output_size: int,
     data: tuple,
     parameters: dict,
```

### Comparing `degann-1.1/degann/expert/selector.py` & `degann-1.1.1/degann/expert/selector.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/activations.py` & `degann-1.1.1/degann/networks/activations.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/callbacks.py` & `degann-1.1.1/degann/networks/callbacks.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/cpp_utils.py` & `degann-1.1.1/degann/networks/cpp_utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/imodel.py` & `degann-1.1.1/degann/networks/imodel.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/layer_creator.py` & `degann-1.1.1/degann/networks/layer_creator.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/layers/tf_dense.py` & `degann-1.1.1/degann/networks/layers/tf_dense.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/losses.py` & `degann-1.1.1/degann/networks/losses.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/metrics.py` & `degann-1.1.1/degann/networks/metrics.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/optimizers.py` & `degann-1.1.1/degann/networks/optimizers.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/topology/tf_densenet.py` & `degann-1.1.1/degann/networks/topology/tf_densenet.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/networks/utils.py` & `degann-1.1.1/degann/networks/utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/search_algorithms/generate.py` & `degann-1.1.1/degann/search_algorithms/generate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,332 +1,332 @@
-import math
-import random
-from typing import Union, Callable
-
-from degann.search_algorithms.nn_code import decode, alphabet_activations
-
-
-class MetaParameter:
-    """
-    Abstract class for parameters in parameter space of neural networks
-    """
-
-    def distance(self, other):
-        pass
-
-    def value(self):
-        pass
-
-
-class CodeParameter(MetaParameter):
-    """
-    Topology parameter --- size of layers with activations
-    """
-
-    block_size = 1
-    exp_size = 10
-
-    def __init__(self, s: Union[str, "CodeParameter"]):
-        if isinstance(s, CodeParameter):
-            s = s.value()
-        self.code = s
-        self.blocks = [
-            self.code[i : i + self.block_size + 1]
-            for i in range(0, len(self.code), self.block_size + 1)
-        ]
-
-    def distance(self, other) -> float:
-        """
-        Distance between `self` topology and `other` topology
-
-        Parameters
-        ----------
-        other: CodeParameter | str
-            other neural network topology
-
-        Returns
-        -------
-        distance: float
-            distance between topologies
-        """
-        if isinstance(other, str):
-            other = CodeParameter(other)
-        val_a = 0
-        act_a = []
-        for block in self.blocks:
-            dec = decode(block, block_size=self.block_size, offset=8)
-            val_a += sum(dec[0])
-            act_a.append(*dec[1])
-
-        val_b = 0
-        act_b = []
-        for block in other.blocks:
-            dec = decode(block, block_size=self.block_size, offset=8)
-            val_b += sum(dec[0])
-            act_b.append(*dec[1])
-
-        diff = 0
-        for i in range(min(len(act_a), len(act_b))):
-            if act_a[i] != act_b[i]:
-                diff += 1
-        diff += CodeParameter.exp_size ** abs(len(act_a) - len(act_b))
-        return abs(val_a - val_b) + diff
-
-    def value(self) -> str:
-        """
-        Present CodeParameter as string code
-
-        Returns
-        -------
-        str_topology: str
-            topology as str
-        """
-        return "".join(self.blocks)
-
-
-class EpochParameter(MetaParameter):
-    """
-    Epoch parameter --- count of epoch in training
-    """
-
-    log_value = 1.1
-    pow_scale = 3
-
-    def __init__(self, epoch: int):
-        self.epoch = epoch
-
-    def distance(self, other: Union[int, "EpochParameter"]) -> float:
-        """
-        Distance between `self` epoch and `other` epoch
-
-        Parameters
-        ----------
-        other: EpochParameter | int
-            other neural network topology
-
-        Returns
-        -------
-        distance: float
-            distance between epochs
-        """
-        if isinstance(other, int):
-            return math.log(
-                self.epoch**EpochParameter.pow_scale, EpochParameter.log_value
-            ) - math.log(other**EpochParameter.pow_scale, EpochParameter.log_value)
-        return math.log(
-            self.epoch**EpochParameter.pow_scale, EpochParameter.log_value
-        ) - math.log(other.epoch**EpochParameter.pow_scale, EpochParameter.log_value)
-
-    def value(self) -> int:
-        """
-        Present EpochParameter as int value
-
-        Returns
-        -------
-        str_topology: int
-            epoch as int value
-        """
-        return self.epoch
-
-
-def choose_neighbor(method: Callable, **kwargs):
-    """
-    Wrapper that returns a method with kwargs applied to it
-
-    Parameters
-    ----------
-    method: Callable
-       Method for determining the distance to another neural network
-    kwargs
-
-    Returns
-    -------
-    method: Callable
-        Method with applied kwargs
-    """
-    return method(**kwargs)
-
-
-def random_generate(
-    alphabet: list[str],
-    min_epoch: int = 100,
-    max_epoch: int = 700,
-    min_length: int = 1,
-    max_length: int = 6,
-) -> tuple[CodeParameter, EpochParameter]:
-    """
-    Random point generator in the parameter space of neural networks
-
-    Parameters
-    ----------
-    alphabet: list[str]
-        Alphabet defining possible layers of a neural network
-    min_epoch: int
-        Minimum number of training epochs
-    max_epoch: int
-        Maximum number of training epochs
-    min_length: int
-        Minimum count of hidden layers in neural network
-    max_length: int
-        Maximum count of hidden layers in neural network
-
-    Returns
-    -------
-    point: tuple[CodeParameter, EpochParameter]
-        random generated point
-    """
-    block = random.randint(min_length, max_length)
-    code = ""
-
-    for i in range(block):
-        code += alphabet[random.randint(0, len(alphabet) - 1)]
-    epoch = random.randint(min_epoch, max_epoch)
-    return CodeParameter(code), EpochParameter(epoch)
-
-
-def generate_neighbor(
-    alphabet: list[str],
-    parameters: tuple[str, int],
-    distance: int = 150,
-    min_epoch: int = 100,
-    max_epoch: int = 700,
-    min_length: int = 1,
-    max_length: int = 6,
-):
-    """
-    Generator of a point in the neighborhood of the current one in the parameter space of neural networks
-
-    Parameters
-    ----------
-    alphabet: list[str]
-        Alphabet defining possible layers of a neural network
-    parameters: tuple[str, int]
-        Start point
-    distance: int
-        Maximum distance from the starting point
-    min_epoch: int
-        Minimum number of training epochs
-    max_epoch: int
-        Maximum number of training epochs
-    min_length: int
-        Minimum count of hidden layers in neural network
-    max_length: int
-        Maximum count of hidden layers in neural network
-
-    Returns
-    -------
-    point: tuple[CodeParameter, EpochParameter]
-        neighbor of start point
-    """
-    code = parameters[0]
-    epoch = parameters[1]
-    is_stop = 0
-    new_epoch = EpochParameter(epoch)
-    new_code = CodeParameter(code)
-
-    while distance > 0 and is_stop == 0:
-        branch = random.random()
-        curr_code = CodeParameter(new_code.value())
-        if branch < 0.33:  # change epoch
-            sign = random.random()
-            if sign < 0.66:  # new epoch more than previous
-                new_epoch = EpochParameter(
-                    min(
-                        random.randint(
-                            epoch,
-                            int(EpochParameter.log_value ** min(distance, 70) * epoch),
-                        ),  # need to rewrite this formula
-                        max_epoch,
-                    )
-                )
-            else:  # new epoch less than previous
-                new_epoch = EpochParameter(
-                    max(
-                        random.randint(
-                            int(
-                                epoch / (EpochParameter.log_value ** min(distance, 70))
-                            ),
-                            epoch,
-                        ),  # need to rewrite this formula
-                        min_epoch,
-                    )
-                )
-            distance -= abs(new_epoch.distance(epoch))
-        elif branch < 1 and distance >= 1:  # change code of neural network
-            chosen_block = random.randint(0, len(curr_code.blocks) - 1)
-
-            command = random.randint(1, 5)
-            match command:
-                case 1:  # add block
-                    if len(curr_code.blocks) < max_length:
-                        new_block = alphabet[random.randint(0, len(alphabet) - 1)]
-                        curr_code = CodeParameter("".join(curr_code.blocks) + new_block)
-                case 2:  # increase block size
-                    current_block_size = int(curr_code.blocks[chosen_block][:-1], 16)
-                    max_block_size = 15**CodeParameter.block_size
-                    max_block_increase = min(max_block_size, int(distance))
-                    new_block = (
-                        hex(current_block_size + random.randint(0, max_block_increase))[
-                            2:
-                        ]
-                        + curr_code.blocks[chosen_block][-1]
-                    )
-                    new_block = (
-                        "0" * (CodeParameter.block_size - len(new_block) + 1)
-                        + new_block
-                    )
-                    if new_block in alphabet:
-                        curr_code.blocks[chosen_block] = new_block
-                case 3:  # decrease size of block
-                    current_block_size = int(curr_code.blocks[chosen_block][:-1], 16)
-                    min_block_size = 0
-                    max_block_decrease = min(current_block_size, int(distance))
-                    new_block = (
-                        hex(
-                            max(
-                                current_block_size
-                                - random.randint(0, max_block_decrease),
-                                min_block_size,
-                            )
-                        )[2:]
-                        + curr_code.blocks[chosen_block][-1]
-                    )
-                    new_block = (
-                        "0" * (CodeParameter.block_size - len(new_block) + 1)
-                        + new_block
-                    )
-                    if new_block in alphabet:
-                        curr_code.blocks[chosen_block] = new_block
-                case 4:  # remove last block
-                    if len(curr_code.blocks) > min_length:
-                        temp = CodeParameter(curr_code.value())
-                        temp.blocks.pop()
-                        if abs(temp.distance(curr_code)) < distance:
-                            curr_code.blocks.pop()
-                case 5:  # change activation for block
-                    new_block = (
-                        curr_code.blocks[chosen_block][:-1]
-                        + alphabet_activations[
-                            random.randint(0, len(alphabet_activations) - 1)
-                        ]
-                    )
-                    if new_block in alphabet:
-                        curr_code.blocks[chosen_block] = new_block
-                case _:
-                    pass
-            distance -= abs(new_code.distance(curr_code))
-            if distance < 0:
-                distance += abs(new_code.distance(curr_code))
-                temp_dist = abs(new_code.distance(curr_code))
-                # print(
-                #     "DEBUG",
-                #     new_code.blocks,
-                #     curr_code.blocks,
-                #     chosen_block,
-                #     command,
-                #     distance,
-                #     temp_dist,
-                # )
-                distance -= temp_dist
-            new_code = curr_code
-        is_stop = random.randint(0, 3)
-    return new_code, new_epoch
+import math
+import random
+from typing import Union, Callable
+
+from degann.search_algorithms.nn_code import decode, alphabet_activations
+
+
+class MetaParameter:
+    """
+    Abstract class for parameters in parameter space of neural networks
+    """
+
+    def distance(self, other):
+        pass
+
+    def value(self):
+        pass
+
+
+class CodeParameter(MetaParameter):
+    """
+    Topology parameter --- size of layers with activations
+    """
+
+    block_size = 1
+    exp_size = 10
+
+    def __init__(self, s: Union[str, "CodeParameter"]):
+        if isinstance(s, CodeParameter):
+            s = s.value()
+        self.code = s
+        self.blocks = [
+            self.code[i : i + self.block_size + 1]
+            for i in range(0, len(self.code), self.block_size + 1)
+        ]
+
+    def distance(self, other) -> float:
+        """
+        Distance between `self` topology and `other` topology
+
+        Parameters
+        ----------
+        other: CodeParameter | str
+            other neural network topology
+
+        Returns
+        -------
+        distance: float
+            distance between topologies
+        """
+        if isinstance(other, str):
+            other = CodeParameter(other)
+        val_a = 0
+        act_a = []
+        for block in self.blocks:
+            dec = decode(block, block_size=self.block_size, offset=8)
+            val_a += sum(dec[0])
+            act_a.append(*dec[1])
+
+        val_b = 0
+        act_b = []
+        for block in other.blocks:
+            dec = decode(block, block_size=self.block_size, offset=8)
+            val_b += sum(dec[0])
+            act_b.append(*dec[1])
+
+        diff = 0
+        for i in range(min(len(act_a), len(act_b))):
+            if act_a[i] != act_b[i]:
+                diff += 1
+        diff += CodeParameter.exp_size ** abs(len(act_a) - len(act_b))
+        return abs(val_a - val_b) + diff
+
+    def value(self) -> str:
+        """
+        Present CodeParameter as string code
+
+        Returns
+        -------
+        str_topology: str
+            topology as str
+        """
+        return "".join(self.blocks)
+
+
+class EpochParameter(MetaParameter):
+    """
+    Epoch parameter --- count of epoch in training
+    """
+
+    log_value = 1.1
+    pow_scale = 3
+
+    def __init__(self, epoch: int):
+        self.epoch = epoch
+
+    def distance(self, other: Union[int, "EpochParameter"]) -> float:
+        """
+        Distance between `self` epoch and `other` epoch
+
+        Parameters
+        ----------
+        other: EpochParameter | int
+            other neural network topology
+
+        Returns
+        -------
+        distance: float
+            distance between epochs
+        """
+        if isinstance(other, int):
+            return math.log(
+                self.epoch**EpochParameter.pow_scale, EpochParameter.log_value
+            ) - math.log(other**EpochParameter.pow_scale, EpochParameter.log_value)
+        return math.log(
+            self.epoch**EpochParameter.pow_scale, EpochParameter.log_value
+        ) - math.log(other.epoch**EpochParameter.pow_scale, EpochParameter.log_value)
+
+    def value(self) -> int:
+        """
+        Present EpochParameter as int value
+
+        Returns
+        -------
+        str_topology: int
+            epoch as int value
+        """
+        return self.epoch
+
+
+def choose_neighbor(method: Callable, **kwargs):
+    """
+    Wrapper that returns a method with kwargs applied to it
+
+    Parameters
+    ----------
+    method: Callable
+       Method for determining the distance to another neural network
+    kwargs
+
+    Returns
+    -------
+    method: Callable
+        Method with applied kwargs
+    """
+    return method(**kwargs)
+
+
+def random_generate(
+    alphabet: list[str],
+    min_epoch: int = 100,
+    max_epoch: int = 700,
+    min_length: int = 1,
+    max_length: int = 6,
+) -> tuple[CodeParameter, EpochParameter]:
+    """
+    Random point generator in the parameter space of neural networks
+
+    Parameters
+    ----------
+    alphabet: list[str]
+        Alphabet defining possible layers of a neural network
+    min_epoch: int
+        Minimum number of training epochs
+    max_epoch: int
+        Maximum number of training epochs
+    min_length: int
+        Minimum count of hidden layers in neural network
+    max_length: int
+        Maximum count of hidden layers in neural network
+
+    Returns
+    -------
+    point: tuple[CodeParameter, EpochParameter]
+        random generated point
+    """
+    block = random.randint(min_length, max_length)
+    code = ""
+
+    for i in range(block):
+        code += alphabet[random.randint(0, len(alphabet) - 1)]
+    epoch = random.randint(min_epoch, max_epoch)
+    return CodeParameter(code), EpochParameter(epoch)
+
+
+def generate_neighbor(
+    alphabet: list[str],
+    parameters: tuple[str, int],
+    distance: int = 150,
+    min_epoch: int = 100,
+    max_epoch: int = 700,
+    min_length: int = 1,
+    max_length: int = 6,
+):
+    """
+    Generator of a point in the neighborhood of the current one in the parameter space of neural networks
+
+    Parameters
+    ----------
+    alphabet: list[str]
+        Alphabet defining possible layers of a neural network
+    parameters: tuple[str, int]
+        Start point
+    distance: int
+        Maximum distance from the starting point
+    min_epoch: int
+        Minimum number of training epochs
+    max_epoch: int
+        Maximum number of training epochs
+    min_length: int
+        Minimum count of hidden layers in neural network
+    max_length: int
+        Maximum count of hidden layers in neural network
+
+    Returns
+    -------
+    point: tuple[CodeParameter, EpochParameter]
+        neighbor of start point
+    """
+    code = parameters[0]
+    epoch = parameters[1]
+    is_stop = 0
+    new_epoch = EpochParameter(epoch)
+    new_code = CodeParameter(code)
+
+    while distance > 0 and is_stop == 0:
+        branch = random.random()
+        curr_code = CodeParameter(new_code.value())
+        if branch < 0.33:  # change epoch
+            sign = random.random()
+            if sign < 0.66:  # new epoch more than previous
+                new_epoch = EpochParameter(
+                    min(
+                        random.randint(
+                            epoch,
+                            int(EpochParameter.log_value ** min(distance, 70) * epoch),
+                        ),  # need to rewrite this formula
+                        max_epoch,
+                    )
+                )
+            else:  # new epoch less than previous
+                new_epoch = EpochParameter(
+                    max(
+                        random.randint(
+                            int(
+                                epoch / (EpochParameter.log_value ** min(distance, 70))
+                            ),
+                            epoch,
+                        ),  # need to rewrite this formula
+                        min_epoch,
+                    )
+                )
+            distance -= abs(new_epoch.distance(epoch))
+        elif branch < 1 and distance >= 1:  # change code of neural network
+            chosen_block = random.randint(0, len(curr_code.blocks) - 1)
+
+            command = random.randint(1, 5)
+            match command:
+                case 1:  # add block
+                    if len(curr_code.blocks) < max_length:
+                        new_block = alphabet[random.randint(0, len(alphabet) - 1)]
+                        curr_code = CodeParameter("".join(curr_code.blocks) + new_block)
+                case 2:  # increase block size
+                    current_block_size = int(curr_code.blocks[chosen_block][:-1], 16)
+                    max_block_size = 15**CodeParameter.block_size
+                    max_block_increase = min(max_block_size, int(distance))
+                    new_block = (
+                        hex(current_block_size + random.randint(0, max_block_increase))[
+                            2:
+                        ]
+                        + curr_code.blocks[chosen_block][-1]
+                    )
+                    new_block = (
+                        "0" * (CodeParameter.block_size - len(new_block) + 1)
+                        + new_block
+                    )
+                    if new_block in alphabet:
+                        curr_code.blocks[chosen_block] = new_block
+                case 3:  # decrease size of block
+                    current_block_size = int(curr_code.blocks[chosen_block][:-1], 16)
+                    min_block_size = 0
+                    max_block_decrease = min(current_block_size, int(distance))
+                    new_block = (
+                        hex(
+                            max(
+                                current_block_size
+                                - random.randint(0, max_block_decrease),
+                                min_block_size,
+                            )
+                        )[2:]
+                        + curr_code.blocks[chosen_block][-1]
+                    )
+                    new_block = (
+                        "0" * (CodeParameter.block_size - len(new_block) + 1)
+                        + new_block
+                    )
+                    if new_block in alphabet:
+                        curr_code.blocks[chosen_block] = new_block
+                case 4:  # remove last block
+                    if len(curr_code.blocks) > min_length:
+                        temp = CodeParameter(curr_code.value())
+                        temp.blocks.pop()
+                        if abs(temp.distance(curr_code)) < distance:
+                            curr_code.blocks.pop()
+                case 5:  # change activation for block
+                    new_block = (
+                        curr_code.blocks[chosen_block][:-1]
+                        + alphabet_activations[
+                            random.randint(0, len(alphabet_activations) - 1)
+                        ]
+                    )
+                    if new_block in alphabet:
+                        curr_code.blocks[chosen_block] = new_block
+                case _:
+                    pass
+            distance -= abs(new_code.distance(curr_code))
+            if distance < 0:
+                distance += abs(new_code.distance(curr_code))
+                temp_dist = abs(new_code.distance(curr_code))
+                # print(
+                #     "DEBUG",
+                #     new_code.blocks,
+                #     curr_code.blocks,
+                #     chosen_block,
+                #     command,
+                #     distance,
+                #     temp_dist,
+                # )
+                distance -= temp_dist
+            new_code = curr_code
+        is_stop = random.randint(0, 3)
+    return new_code, new_epoch
```

### Comparing `degann-1.1/degann/search_algorithms/grid_search.py` & `degann-1.1.1/degann/search_algorithms/grid_search.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/search_algorithms/nn_code.py` & `degann-1.1.1/degann/search_algorithms/nn_code.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/search_algorithms/pattern_search.py` & `degann-1.1.1/degann/search_algorithms/pattern_search.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/search_algorithms/random_search.py` & `degann-1.1.1/degann/search_algorithms/random_search.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/search_algorithms/simulated_annealing.py` & `degann-1.1.1/degann/search_algorithms/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/degann/search_algorithms/utils.py` & `degann-1.1.1/degann/search_algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1/setup.py` & `degann-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     url="https://github.com/Krekep/degann",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="MIT",
     package_dir={"": "degann"},
     install_requires=[
-        "keras~=2.12.0",
+        "keras~=3.3.3",
         "matplotlib~=3.7.1",
-        "numpy~=1.23.5",
-        "scipy~=1.10.1",
-        "tensorflow~=2.12.0",
+        "numpy~=1.26.4",
+        "scipy~=1.13.1",
+        "tensorflow~=2.16.1",
     ],
     python_requires=">=3.10",
     keywords=["python", "ode", "differential equation", "neural network"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
```

