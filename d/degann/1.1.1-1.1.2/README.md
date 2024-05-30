# Comparing `tmp/degann-1.1.1.tar.gz` & `tmp/degann-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degann-1.1.1.tar", last modified: Thu May 30 15:43:36 2024, max compression
+gzip compressed data, was "degann-1.1.2.tar", last modified: Thu May 30 16:12:53 2024, max compression
```

## Comparing `degann-1.1.1.tar` & `degann-1.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.402185 degann-1.1.1/
--rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3005 2024-05-30 15:43:36.402185 degann-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2024-05-30 14:18:28.000000 degann-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.378185 degann-1.1.1/degann/
--rw-rw-rw-   0        0        0      108 2024-05-30 14:11:47.000000 degann-1.1.1/degann/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.381185 degann-1.1.1/degann/degann.egg-info/
--rw-rw-rw-   0        0        0     3005 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1219 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/requires.txt
--rw-rw-rw-   0        0        0       53 2024-05-30 15:43:36.000000 degann-1.1.1/degann/degann.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.384187 degann-1.1.1/degann/equations/
--rw-rw-rw-   0        0        0       90 2023-09-27 09:30:32.000000 degann-1.1.1/degann/equations/__init__.py
--rw-rw-rw-   0        0        0     3200 2024-05-30 14:03:10.000000 degann-1.1.1/degann/equations/equation_utils.py
--rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-1.1.1/degann/equations/simple_equation.py
--rw-rw-rw-   0        0        0     4162 2024-05-30 14:03:10.000000 degann-1.1.1/degann/equations/system_ode.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.386185 degann-1.1.1/degann/expert/
--rw-rw-rw-   0        0        0       50 2024-05-30 14:10:58.000000 degann-1.1.1/degann/expert/__init__.py
--rw-rw-rw-   0        0        0     3736 2024-05-30 14:28:38.000000 degann-1.1.1/degann/expert/pipeline.py
--rw-rw-rw-   0        0        0     5066 2024-05-30 14:10:53.000000 degann-1.1.1/degann/expert/selector.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.393187 degann-1.1.1/degann/networks/
--rw-rw-rw-   0        0        0      203 2024-03-27 15:04:35.000000 degann-1.1.1/degann/networks/__init__.py
--rw-rw-rw-   0        0        0     1852 2024-02-26 17:40:53.000000 degann-1.1.1/degann/networks/activations.py
--rw-rw-rw-   0        0        0     3066 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/callbacks.py
--rw-rw-rw-   0        0        0      467 2024-05-30 15:42:42.000000 degann-1.1.1/degann/networks/config_format.py
--rw-rw-rw-   0        0        0    13061 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/cpp_utils.py
--rw-rw-rw-   0        0        0    12985 2024-05-30 14:13:44.000000 degann-1.1.1/degann/networks/imodel.py
--rw-rw-rw-   0        0        0     2153 2024-03-26 15:51:27.000000 degann-1.1.1/degann/networks/layer_creator.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.395185 degann-1.1.1/degann/networks/layers/
--rw-rw-rw-   0        0        0       25 2024-03-26 15:51:27.000000 degann-1.1.1/degann/networks/layers/__init__.py
--rw-rw-rw-   0        0        0     5347 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/layers/tf_dense.py
--rw-rw-rw-   0        0        0     3927 2024-05-30 14:14:02.000000 degann-1.1.1/degann/networks/losses.py
--rw-rw-rw-   0        0        0     2215 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/metrics.py
--rw-rw-rw-   0        0        0     1128 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/optimizers.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.396185 degann-1.1.1/degann/networks/topology/
--rw-rw-rw-   0        0        0       28 2024-03-26 15:51:27.000000 degann-1.1.1/degann/networks/topology/__init__.py
--rw-rw-rw-   0        0        0    14206 2024-05-30 14:03:10.000000 degann-1.1.1/degann/networks/topology/tf_densenet.py
--rw-rw-rw-   0        0        0     2201 2024-02-26 17:40:53.000000 degann-1.1.1/degann/networks/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 15:43:36.401187 degann-1.1.1/degann/search_algorithms/
--rw-rw-rw-   0        0        0      174 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/__init__.py
--rw-rw-rw-   0        0        0    10974 2024-05-30 14:12:27.000000 degann-1.1.1/degann/search_algorithms/generate.py
--rw-rw-rw-   0        0        0     8015 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/grid_search.py
--rw-rw-rw-   0        0        0     2021 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/nn_code.py
--rw-rw-rw-   0        0        0    10916 2024-05-30 14:12:57.000000 degann-1.1.1/degann/search_algorithms/pattern_search.py
--rw-rw-rw-   0        0        0     9378 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/random_search.py
--rw-rw-rw-   0        0        0    10070 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/simulated_annealing.py
--rw-rw-rw-   0        0        0     1458 2024-05-30 14:03:10.000000 degann-1.1.1/degann/search_algorithms/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-30 15:43:36.402185 degann-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1503 2024-05-30 15:13:20.000000 degann-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.079258 degann-1.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3005 2024-05-30 16:12:53.079258 degann-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2166 2024-05-30 14:18:28.000000 degann-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.056259 degann-1.1.2/degann/
+-rw-rw-rw-   0        0        0      703 2024-05-30 16:10:02.000000 degann-1.1.2/degann/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.060258 degann-1.1.2/degann/degann.egg-info/
+-rw-rw-rw-   0        0        0     3005 2024-05-30 16:12:53.000000 degann-1.1.2/degann/degann.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1219 2024-05-30 16:12:53.000000 degann-1.1.2/degann/degann.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:12:53.000000 degann-1.1.2/degann/degann.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-30 16:12:53.000000 degann-1.1.2/degann/degann.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2024-05-30 16:12:53.000000 degann-1.1.2/degann/degann.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.062258 degann-1.1.2/degann/equations/
+-rw-rw-rw-   0        0        0      277 2024-05-30 16:07:13.000000 degann-1.1.2/degann/equations/__init__.py
+-rw-rw-rw-   0        0        0     3200 2024-05-30 14:03:10.000000 degann-1.1.2/degann/equations/equation_utils.py
+-rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-1.1.2/degann/equations/simple_equation.py
+-rw-rw-rw-   0        0        0     4162 2024-05-30 14:03:10.000000 degann-1.1.2/degann/equations/system_ode.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.064258 degann-1.1.2/degann/expert/
+-rw-rw-rw-   0        0        0      166 2024-05-30 16:07:13.000000 degann-1.1.2/degann/expert/__init__.py
+-rw-rw-rw-   0        0        0     3736 2024-05-30 14:28:38.000000 degann-1.1.2/degann/expert/pipeline.py
+-rw-rw-rw-   0        0        0     5066 2024-05-30 14:10:53.000000 degann-1.1.2/degann/expert/selector.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.071258 degann-1.1.2/degann/networks/
+-rw-rw-rw-   0        0        0      538 2024-05-30 16:02:49.000000 degann-1.1.2/degann/networks/__init__.py
+-rw-rw-rw-   0        0        0     1852 2024-02-26 17:40:53.000000 degann-1.1.2/degann/networks/activations.py
+-rw-rw-rw-   0        0        0     3066 2024-05-30 14:03:10.000000 degann-1.1.2/degann/networks/callbacks.py
+-rw-rw-rw-   0        0        0      467 2024-05-30 16:10:21.000000 degann-1.1.2/degann/networks/config_format.py
+-rw-rw-rw-   0        0        0    13061 2024-05-30 14:03:10.000000 degann-1.1.2/degann/networks/cpp_utils.py
+-rw-rw-rw-   0        0        0    12985 2024-05-30 14:13:44.000000 degann-1.1.2/degann/networks/imodel.py
+-rw-rw-rw-   0        0        0     2153 2024-03-26 15:51:27.000000 degann-1.1.2/degann/networks/layer_creator.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.072259 degann-1.1.2/degann/networks/layers/
+-rw-rw-rw-   0        0        0       25 2024-03-26 15:51:27.000000 degann-1.1.2/degann/networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     5347 2024-05-30 14:03:10.000000 degann-1.1.2/degann/networks/layers/tf_dense.py
+-rw-rw-rw-   0        0        0     3927 2024-05-30 14:14:02.000000 degann-1.1.2/degann/networks/losses.py
+-rw-rw-rw-   0        0        0     2215 2024-05-30 14:03:10.000000 degann-1.1.2/degann/networks/metrics.py
+-rw-rw-rw-   0        0        0     1128 2024-05-30 14:03:10.000000 degann-1.1.2/degann/networks/optimizers.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.073260 degann-1.1.2/degann/networks/topology/
+-rw-rw-rw-   0        0        0       28 2024-03-26 15:51:27.000000 degann-1.1.2/degann/networks/topology/__init__.py
+-rw-rw-rw-   0        0        0    14206 2024-05-30 14:03:10.000000 degann-1.1.2/degann/networks/topology/tf_densenet.py
+-rw-rw-rw-   0        0        0     2201 2024-02-26 17:40:53.000000 degann-1.1.2/degann/networks/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:12:53.078258 degann-1.1.2/degann/search_algorithms/
+-rw-rw-rw-   0        0        0      659 2024-05-30 16:07:13.000000 degann-1.1.2/degann/search_algorithms/__init__.py
+-rw-rw-rw-   0        0        0    10974 2024-05-30 14:12:27.000000 degann-1.1.2/degann/search_algorithms/generate.py
+-rw-rw-rw-   0        0        0     8015 2024-05-30 14:03:10.000000 degann-1.1.2/degann/search_algorithms/grid_search.py
+-rw-rw-rw-   0        0        0     2021 2024-05-30 14:03:10.000000 degann-1.1.2/degann/search_algorithms/nn_code.py
+-rw-rw-rw-   0        0        0    10963 2024-05-30 16:11:18.000000 degann-1.1.2/degann/search_algorithms/pattern_search.py
+-rw-rw-rw-   0        0        0     9378 2024-05-30 14:03:10.000000 degann-1.1.2/degann/search_algorithms/random_search.py
+-rw-rw-rw-   0        0        0    10070 2024-05-30 14:03:10.000000 degann-1.1.2/degann/search_algorithms/simulated_annealing.py
+-rw-rw-rw-   0        0        0     1458 2024-05-30 14:03:10.000000 degann-1.1.2/degann/search_algorithms/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 16:12:53.080258 degann-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1503 2024-05-30 15:13:20.000000 degann-1.1.2/setup.py
```

### Comparing `degann-1.1.1/LICENSE` & `degann-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/PKG-INFO` & `degann-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `degann-1.1.1/README.md` & `degann-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/degann.egg-info/PKG-INFO` & `degann-1.1.2/degann/degann.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `degann-1.1.1/degann/degann.egg-info/SOURCES.txt` & `degann-1.1.2/degann/degann.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/equations/equation_utils.py` & `degann-1.1.2/degann/equations/equation_utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/equations/simple_equation.py` & `degann-1.1.2/degann/equations/simple_equation.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/equations/system_ode.py` & `degann-1.1.2/degann/equations/system_ode.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/expert/pipeline.py` & `degann-1.1.2/degann/expert/pipeline.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/expert/selector.py` & `degann-1.1.2/degann/expert/selector.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/activations.py` & `degann-1.1.2/degann/networks/activations.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/callbacks.py` & `degann-1.1.2/degann/networks/callbacks.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/cpp_utils.py` & `degann-1.1.2/degann/networks/cpp_utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/imodel.py` & `degann-1.1.2/degann/networks/imodel.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/layer_creator.py` & `degann-1.1.2/degann/networks/layer_creator.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/layers/tf_dense.py` & `degann-1.1.2/degann/networks/layers/tf_dense.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/losses.py` & `degann-1.1.2/degann/networks/losses.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/metrics.py` & `degann-1.1.2/degann/networks/metrics.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/optimizers.py` & `degann-1.1.2/degann/networks/optimizers.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/topology/tf_densenet.py` & `degann-1.1.2/degann/networks/topology/tf_densenet.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/networks/utils.py` & `degann-1.1.2/degann/networks/utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/search_algorithms/generate.py` & `degann-1.1.2/degann/search_algorithms/generate.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/search_algorithms/grid_search.py` & `degann-1.1.2/degann/search_algorithms/grid_search.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/search_algorithms/nn_code.py` & `degann-1.1.2/degann/search_algorithms/nn_code.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/search_algorithms/pattern_search.py` & `degann-1.1.2/degann/search_algorithms/pattern_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 from typing import Union, Any, Tuple, List
 
 import numpy as np
 import tensorflow as tf
 
-from degann import MemoryCleaner, get_all_optimizers, get_all_metric_functions
+from degann.networks.callbacks import MemoryCleaner
+from degann.networks import get_all_optimizers, get_all_metric_functions
 from degann.networks import activations, imodel, losses
 
 _default_shapes = [
     [10, 10, 10, 10, 10, 10],
     [80, 80, 80],
     [32, 16, 8, 4],
     [4, 8, 16, 32],
```

### Comparing `degann-1.1.1/degann/search_algorithms/random_search.py` & `degann-1.1.2/degann/search_algorithms/random_search.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/search_algorithms/simulated_annealing.py` & `degann-1.1.2/degann/search_algorithms/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/degann/search_algorithms/utils.py` & `degann-1.1.2/degann/search_algorithms/utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.1.1/setup.py` & `degann-1.1.2/setup.py`

 * *Files identical despite different names*

