# Comparing `tmp/degann-1.0.tar.gz` & `tmp/degann-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degann-1.0.tar", last modified: Thu Apr 18 15:16:11 2024, max compression
+gzip compressed data, was "degann-1.1.tar", last modified: Thu May 30 12:59:22 2024, max compression
```

## Comparing `degann-1.0.tar` & `degann-1.1.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.839355 degann-1.0/
--rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-1.0/LICENSE
--rw-rw-rw-   0        0        0     3026 2024-04-18 15:16:11.839355 degann-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2024-04-18 14:22:40.000000 degann-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.814356 degann-1.0/degann/
--rw-rw-rw-   0        0        0       74 2024-03-19 14:02:34.000000 degann-1.0/degann/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.825355 degann-1.0/degann/equations/
--rw-rw-rw-   0        0        0       90 2023-09-27 09:30:32.000000 degann-1.0/degann/equations/__init__.py
--rw-rw-rw-   0        0        0     2934 2023-12-26 18:47:41.000000 degann-1.0/degann/equations/equation_utils.py
--rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-1.0/degann/equations/simple_equation.py
--rw-rw-rw-   0        0        0     4158 2023-06-22 20:01:24.000000 degann-1.0/degann/equations/system_ode.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.829357 degann-1.0/degann/expert/
--rw-rw-rw-   0        0        0      108 2024-03-19 14:02:34.000000 degann-1.0/degann/expert/__init__.py
--rw-rw-rw-   0        0        0     7725 2024-04-13 13:40:21.000000 degann-1.0/degann/expert/generate.py
--rw-rw-rw-   0        0        0     1265 2024-02-26 17:01:06.000000 degann-1.0/degann/expert/nn_code.py
--rw-rw-rw-   0        0        0    19246 2024-04-18 15:08:00.000000 degann-1.0/degann/expert/search_algorithms.py
--rw-rw-rw-   0        0        0     6514 2024-04-18 15:08:00.000000 degann-1.0/degann/expert/selector.py
--rw-rw-rw-   0        0        0    11634 2024-04-17 17:20:26.000000 degann-1.0/degann/expert/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.836356 degann-1.0/degann/networks/
--rw-rw-rw-   0        0        0      203 2024-03-27 15:04:35.000000 degann-1.0/degann/networks/__init__.py
--rw-rw-rw-   0        0        0     1852 2024-02-26 17:40:53.000000 degann-1.0/degann/networks/activations.py
--rw-rw-rw-   0        0        0     2707 2023-09-27 09:30:32.000000 degann-1.0/degann/networks/callbacks.py
--rw-rw-rw-   0        0        0      465 2024-04-18 14:22:40.000000 degann-1.0/degann/networks/config_format.py
--rw-rw-rw-   0        0        0     8267 2024-03-17 08:10:56.000000 degann-1.0/degann/networks/cpp_utils.py
--rw-rw-rw-   0        0        0    13744 2024-04-17 17:09:28.000000 degann-1.0/degann/networks/imodel.py
--rw-rw-rw-   0        0        0     2153 2024-03-26 15:51:27.000000 degann-1.0/degann/networks/layer_creator.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.837355 degann-1.0/degann/networks/layers/
--rw-rw-rw-   0        0        0       25 2024-03-26 15:51:27.000000 degann-1.0/degann/networks/layers/__init__.py
--rw-rw-rw-   0        0        0     5220 2024-03-26 15:50:19.000000 degann-1.0/degann/networks/layers/tf_dense.py
--rw-rw-rw-   0        0        0     3631 2024-04-17 13:40:01.000000 degann-1.0/degann/networks/losses.py
--rw-rw-rw-   0        0        0     2421 2024-02-26 17:40:53.000000 degann-1.0/degann/networks/metrics.py
--rw-rw-rw-   0        0        0      690 2023-09-27 16:24:36.000000 degann-1.0/degann/networks/optimizers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.838355 degann-1.0/degann/networks/topology/
--rw-rw-rw-   0        0        0       28 2024-03-26 15:51:27.000000 degann-1.0/degann/networks/topology/__init__.py
--rw-rw-rw-   0        0        0    14102 2024-04-17 17:10:30.000000 degann-1.0/degann/networks/topology/tf_densenet.py
--rw-rw-rw-   0        0        0     2201 2024-02-26 17:40:53.000000 degann-1.0/degann/networks/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 15:16:11.822362 degann-1.0/degann.egg-info/
--rw-rw-rw-   0        0        0     3026 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 15:16:11.000000 degann-1.0/degann.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 15:16:11.839355 degann-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1517 2024-04-18 14:43:31.000000 degann-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.768611 degann-1.1/
+-rw-rw-rw-   0        0        0     1090 2023-09-27 09:30:32.000000 degann-1.1/LICENSE
+-rw-rw-rw-   0        0        0     3003 2024-05-30 12:59:22.767610 degann-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2166 2024-05-30 12:53:17.000000 degann-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.745610 degann-1.1/degann/
+-rw-rw-rw-   0        0        0      108 2024-05-11 12:06:42.000000 degann-1.1/degann/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.748610 degann-1.1/degann/degann.egg-info/
+-rw-rw-rw-   0        0        0     3003 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1219 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2024-05-30 12:59:22.000000 degann-1.1/degann/degann.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.751613 degann-1.1/degann/equations/
+-rw-rw-rw-   0        0        0       90 2023-09-27 09:30:32.000000 degann-1.1/degann/equations/__init__.py
+-rw-rw-rw-   0        0        0     3200 2024-05-30 08:54:39.000000 degann-1.1/degann/equations/equation_utils.py
+-rw-rw-rw-   0        0        0     6581 2023-06-22 20:01:24.000000 degann-1.1/degann/equations/simple_equation.py
+-rw-rw-rw-   0        0        0     4162 2024-05-30 08:54:39.000000 degann-1.1/degann/equations/system_ode.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.753610 degann-1.1/degann/expert/
+-rw-rw-rw-   0        0        0       25 2024-05-11 11:57:48.000000 degann-1.1/degann/expert/__init__.py
+-rw-rw-rw-   0        0        0     3697 2024-05-30 08:28:46.000000 degann-1.1/degann/expert/pipeline.py
+-rw-rw-rw-   0        0        0     5066 2024-05-30 12:37:38.000000 degann-1.1/degann/expert/selector.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.759610 degann-1.1/degann/networks/
+-rw-rw-rw-   0        0        0      203 2024-03-27 15:04:35.000000 degann-1.1/degann/networks/__init__.py
+-rw-rw-rw-   0        0        0     1852 2024-02-26 17:40:53.000000 degann-1.1/degann/networks/activations.py
+-rw-rw-rw-   0        0        0     3066 2024-05-30 12:37:38.000000 degann-1.1/degann/networks/callbacks.py
+-rw-rw-rw-   0        0        0      465 2024-05-30 09:00:10.000000 degann-1.1/degann/networks/config_format.py
+-rw-rw-rw-   0        0        0    13061 2024-05-30 12:37:38.000000 degann-1.1/degann/networks/cpp_utils.py
+-rw-rw-rw-   0        0        0    12985 2024-05-30 07:46:52.000000 degann-1.1/degann/networks/imodel.py
+-rw-rw-rw-   0        0        0     2153 2024-03-26 15:51:27.000000 degann-1.1/degann/networks/layer_creator.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.760610 degann-1.1/degann/networks/layers/
+-rw-rw-rw-   0        0        0       25 2024-03-26 15:51:27.000000 degann-1.1/degann/networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     5347 2024-05-30 07:46:52.000000 degann-1.1/degann/networks/layers/tf_dense.py
+-rw-rw-rw-   0        0        0     3927 2024-05-30 12:37:38.000000 degann-1.1/degann/networks/losses.py
+-rw-rw-rw-   0        0        0     2215 2024-05-30 10:09:34.000000 degann-1.1/degann/networks/metrics.py
+-rw-rw-rw-   0        0        0     1128 2024-05-30 10:56:52.000000 degann-1.1/degann/networks/optimizers.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.762610 degann-1.1/degann/networks/topology/
+-rw-rw-rw-   0        0        0       28 2024-03-26 15:51:27.000000 degann-1.1/degann/networks/topology/__init__.py
+-rw-rw-rw-   0        0        0    14206 2024-05-30 07:46:52.000000 degann-1.1/degann/networks/topology/tf_densenet.py
+-rw-rw-rw-   0        0        0     2201 2024-02-26 17:40:53.000000 degann-1.1/degann/networks/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:59:22.767610 degann-1.1/degann/search_algorithms/
+-rw-rw-rw-   0        0        0      174 2024-05-30 07:46:52.000000 degann-1.1/degann/search_algorithms/__init__.py
+-rw-rw-rw-   0        0        0    10642 2024-05-30 12:37:38.000000 degann-1.1/degann/search_algorithms/generate.py
+-rw-rw-rw-   0        0        0     8015 2024-05-30 08:12:30.000000 degann-1.1/degann/search_algorithms/grid_search.py
+-rw-rw-rw-   0        0        0     2021 2024-05-30 08:12:31.000000 degann-1.1/degann/search_algorithms/nn_code.py
+-rw-rw-rw-   0        0        0    10916 2024-05-30 12:37:38.000000 degann-1.1/degann/search_algorithms/pattern_search.py
+-rw-rw-rw-   0        0        0     9378 2024-05-30 10:47:43.000000 degann-1.1/degann/search_algorithms/random_search.py
+-rw-rw-rw-   0        0        0    10070 2024-05-30 12:37:37.000000 degann-1.1/degann/search_algorithms/simulated_annealing.py
+-rw-rw-rw-   0        0        0     1458 2024-05-30 10:56:23.000000 degann-1.1/degann/search_algorithms/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:59:22.768611 degann-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1504 2024-05-06 17:03:35.000000 degann-1.1/setup.py
```

### Comparing `degann-1.0/LICENSE` & `degann-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `degann-1.0/PKG-INFO` & `degann-1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 1.0
+Version: 1.1
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DEGANN
 
 [![Check tests](https://github.com/Krekep/degann/actions/workflows/tests.yml/badge.svg)](https://github.com/Krekep/degann/actions/workflows/tests.yml)
 [![License](https://img.shields.io/badge/license-MIT-orange)](https://github.com/Krekep/degann/blob/main/LICENSE)
-[![Package](https://img.shields.io/badge/pypi%20package-1.0-%233776ab)](https://pypi.org/project/degann/)
+[![Package](https://img.shields.io/badge/pypi%20package-1.1-%233776ab)](https://pypi.org/project/degann/)
 
 **DEGANN** is a library generating neural networks for approximating solutions to differential equations. As a backend for working with neural networks, tensorflow is used, but with the ability to expand with your own tools.
 
 **Features**
 - Generation of neural networks by parameters.
 - Construction of tables with the numerical solution of ordinary differential equations of the first order
 - Construction of tables with numerical solution of systems of ordinary differential equations of the first order
@@ -54,9 +53,7 @@
 
 ### Via pip
 Use command
 ```bash
 pip install degann
 ```
 Now you can use the `degann` package
-
-
```

### Comparing `degann-1.0/README.md` & `degann-1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # DEGANN
 
 [![Check tests](https://github.com/Krekep/degann/actions/workflows/tests.yml/badge.svg)](https://github.com/Krekep/degann/actions/workflows/tests.yml)
 [![License](https://img.shields.io/badge/license-MIT-orange)](https://github.com/Krekep/degann/blob/main/LICENSE)
-[![Package](https://img.shields.io/badge/pypi%20package-1.0-%233776ab)](https://pypi.org/project/degann/)
+[![Package](https://img.shields.io/badge/pypi%20package-1.1-%233776ab)](https://pypi.org/project/degann/)
 
 **DEGANN** is a library generating neural networks for approximating solutions to differential equations. As a backend for working with neural networks, tensorflow is used, but with the ability to expand with your own tools.
 
 **Features**
 - Generation of neural networks by parameters.
 - Construction of tables with the numerical solution of ordinary differential equations of the first order
 - Construction of tables with numerical solution of systems of ordinary differential equations of the first order
```

### Comparing `degann-1.0/degann/equations/equation_utils.py` & `degann-1.1/degann/equations/equation_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,25 +7,38 @@
 import numpy as np
 from matplotlib import pyplot as plt
 
 from degann.networks import imodel
 
 
 def system_ode_from_string(system: str) -> List[List[str]]:
+    """
+    Splits the passed multi-line system of differential equations into a list of strings
+
+    Parameters
+    ----------
+    system: str
+        SODE as string
+
+    Returns
+    -------
+    list_sode: str
+        SODE as list of strings
+    """
     s = system.split("\n")
     parsed_s = []
     for eq in s:
         parsed_s.append(eq.split())
     return parsed_s
 
 
 def extract_iv(eq: str) -> Tuple[float, float]:
     """
     Extract initial value for Cauchy problem
-    Format --- yi(value1)=value2 without spaces
+    Format --- `yi(value1)=value2` without spaces
 
     Parameters
     ----------
     eq: str
         Condition
     Returns
     -------
```

### Comparing `degann-1.0/degann/equations/simple_equation.py` & `degann-1.1/degann/equations/simple_equation.py`

 * *Files identical despite different names*

### Comparing `degann-1.0/degann/equations/system_ode.py` & `degann-1.1/degann/equations/system_ode.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Parse passed equations and build functions for them
 
         Parameters
         ----------
         n: int
             System size
         equations: list[list[str]]
-            System of equations. Equation yi' = f(x, yj...) and Cauchy initial value yi(x0) = yi0
+            System of equations. Equation `yi' = f(x, yj...)` and Cauchy initial value `yi(x0) = yi0`
         """
         self._size = n
         self._func_arguments = ""
         for i in range(n):
             self._func_arguments += f"y{i}, "
         self._func_arguments = self._func_arguments[:-2]
```

### Comparing `degann-1.0/degann/expert/selector.py` & `degann-1.1/degann/expert/selector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,198 +1,143 @@
 from itertools import product
-from typing import List
 
-from degann.expert.nn_code import alph_n_full, alphabet_activations
-from degann.expert.search_algorithms import (
-    random_search_endless,
-    simulated_annealing,
-    full_search,
-)
+from degann.search_algorithms.nn_code import alph_n_full, alphabet_activations
 
-tags = {
-    "type": {
+expert_system_tags = {
+    "type": [
         "sin",
         "lin",
         "exp",
         "log",
         "gauss",
         "hyperbol",
         "const",
         "sig",
         "unknown",
-    },
-    "precision": {"maximal", "median", "minimal"},
-    "work time": {"long", "medium", "short"},
-    "data size": {"big", "median", "small", "very small", "auto"},
+    ],
+    "precision": ["maximal", "median", "minimal"],
+    "work time": ["long", "medium", "short"],
+    "data size": ["very small", "small", "median", "big", "auto"],
 }
 
-
-_base_iteration_count = 5
-_base_min_epoch_count = 200
-_base_max_epoch_count = 700
-_base_nn_max_length = 4
-_base_nn_min_length = 2
-_base_nn_block_size = 1
-_base_block_size_offset = 8
-_base_alphabet = ["".join(elem) for elem in product(alph_n_full, alphabet_activations)]
-_base_random_launch = 2
-_base_sim_launch = 2
-_base_loss_function = "MaxAbsoluteDeviation"
-_base_loss_threshold = 1
-_base_optimizer = "Adam"
+base_sam_parameters = {
+    "distance_to_neighbor": "distance_const",
+    "dist_offset": 300,
+    "dist_scale": 0,
+    "temperature_reduction_method": "temperature_lin",
+    "temperature_speed": 0,
+}
+base_parameters = {
+    "launch_count_random_search": 2,
+    "launch_count_simulated_annealing": 2,
+    "nn_max_length": 4,
+    "nn_min_length": 1,
+    "nn_alphabet_block_size": 1,
+    "nn_alphabet_offset": 8,
+    "nn_alphabet": [
+        "".join(elem) for elem in product(alph_n_full, alphabet_activations)
+    ],
+    "min_train_epoch": 200,
+    "max_train_epoch": 500,
+    "iteration_count": 5,
+    "loss_function": "MaxAbsoluteDeviation",
+    "loss_threshold": 1,
+    "optimizer": "Adam",
+    "simulated_annealing_params": base_sam_parameters,
+}
 
 
 def suggest_parameters(
+    data: tuple = None,
     tags: dict[str, str] = None,
 ) -> dict:
+    """
+    Builds many parameters of search algorithms using labels supplied by the user,
+     describing the requirements for the result and hints on the data.
+
+    Parameters
+    ----------
+    data: Optional[tuple]
+        Dataset
+    tags: dict[str, str]
+        A subset of tags described in expert_system_tags
+
+    Returns
+    -------
+    parameters: dict
+        Parameters for search algorithms
+    """
     if tags is None:
         tags = {
             "type": "unknown",
             "precision": "maximal",
             "work time": "long",
             "data size": "auto",
         }
 
-    launch_count_random_search = _base_random_launch
-    launch_count_simulated_annealing = _base_sim_launch
+    parameters = base_parameters.copy()
 
-    nn_max_length = _base_nn_max_length
-    nn_min_length = _base_nn_min_length
+    simulated_annealing_params = base_sam_parameters.copy()
 
-    nn_alphabet_block_size = _base_nn_block_size
-    nn_alphabet_offset = _base_block_size_offset
-    nn_alphabet: list[str] = _base_alphabet
-
-    min_train_epoch = _base_min_epoch_count
-    max_train_epoch = _base_max_epoch_count
-
-    iteration_count = _base_iteration_count
-    loss_threshold = _base_loss_threshold
-
-    simulated_annealing_params = {
-        # "distance_to_neighbor": [distance_const(150)],
-        # "temperature_reduction_method": [temperature_lin],
-        "distance_to_neighbor": "distance_const",
-        "dist_offset": 150,
-        "dist_scale": 0,
-        "temperature_reduction_method": "temperature_lin",
-        "temperature_speed": 0,
-    }
-
-    if tags["type"] in ["sin", "unknown"]:
-        min_train_epoch *= 2
-        nn_max_length += 1
-        iteration_count += 10
+    if tags["type"] in ["sin", "multidim", "unknown"]:
+        parameters["min_train_epoch"] *= 2
+        parameters["max_train_epoch"] = 700
+        parameters["nn_max_length"] += 1
+        parameters["iteration_count"] += 10
 
         # simulated_annealing_params["distance_to_neighbor"] = [distance_const(300), distance_lin(50, 400)]
         # simulated_annealing_params["temperature_reduction_method"] = [temperature_exp(0.95), temperature_exp(0.95)]
         simulated_annealing_params["distance_to_neighbor"] = "distance_lin"
         simulated_annealing_params["dist_offset"] = 50
         simulated_annealing_params["dist_scale"] = 400
         simulated_annealing_params["temperature_reduction_method"] = "temperature_exp"
         simulated_annealing_params["temperature_speed"] = 0.95
 
-        launch_count_random_search += 2
-        launch_count_simulated_annealing = 10
+        parameters["launch_count_random_search"] += 2
+        parameters["launch_count_simulated_annealing"] = 10
+    elif tags["type"] in ["exp", "lin"]:
+        parameters["iteration_count"] += 30
 
     if tags["precision"] == "minimal":
-        loss_threshold *= 2
+        parameters["loss_threshold"] *= 2
     if tags["precision"] == "median":
-        iteration_count = int(10 * iteration_count)
+        parameters["iteration_count"] = int(10 * parameters["iteration_count"])
     if tags["precision"] == "maximal":
-        loss_threshold /= 2
-        iteration_count = int(40 * iteration_count)
+        parameters["loss_threshold"] /= 10
+        parameters["iteration_count"] = int(40 * parameters["iteration_count"])
+        parameters["max_train_epoch"] = 700
 
     if tags["work time"] == "short":
-        nn_max_length -= 1
-        nn_min_length -= 1
+        parameters["nn_max_length"] -= 1
+        parameters["nn_min_length"] -= 1
     elif tags["work time"] == "long":
-        nn_max_length += 1
+        parameters["nn_max_length"] += 1
 
-    return {
-        "launch_count_random_search": launch_count_random_search,
-        "launch_count_simulated_annealing": launch_count_simulated_annealing,
-        "nn_max_length": nn_max_length,
-        "nn_min_length": nn_min_length,
-        "nn_alphabet_block_size": nn_alphabet_block_size,
-        "nn_alphabet_offset": nn_alphabet_offset,
-        "nn_alphabet": nn_alphabet,
-        "min_train_epoch": min_train_epoch,
-        "max_train_epoch": max_train_epoch,
-        "iteration_count": iteration_count,
-        "loss_function": _base_loss_function,
-        "loss_threshold": loss_threshold,
-        "optimizer": _base_optimizer,
-        "simulated_annealing_params": simulated_annealing_params,
-    }
-
-
-def execute_pipeline(
-    input_size: int,
-    output_size: int,
-    data,
-    parameters: dict,
-    values: dict = None,
-    additional_losses: List[str] = None,
-    additional_optimizers: List[str] = None,
-    val_data=None,
-    **kwargs
-) -> tuple[float, dict]:
-    if values is None:
-        values = {
-            "loss": parameters["loss_function"],
-            "threshold": parameters["loss_threshold"],
-            "opt": parameters["optimizer"],
-        }
-    values["in_size"] = input_size
-    values["out_size"] = output_size
-    values["data"] = data
-    values["val_data"] = val_data
-
-    search_algorithm_arguments = {
-        "max_iter": parameters["iteration_count"],
-        "min_epoch": parameters["min_train_epoch"],
-        "max_epoch": parameters["max_train_epoch"],
-        "nn_min_length": parameters["nn_min_length"],
-        "nn_max_length": parameters["nn_max_length"],
-        "nn_alphabet": parameters["nn_alphabet"],
-        "alphabet_block_size": parameters["nn_alphabet_block_size"],
-        "alphabet_offset": parameters["nn_alphabet_offset"],
-    }
-
-    for i in range(parameters["launch_count_random_search"]):
-        (
-            train_loss,
-            count_epoch,
-            loss_function,
-            optimizer,
-            result_nn,
-            last_iteration,
-        ) = random_search_endless(**values, **search_algorithm_arguments, **kwargs)
-        if train_loss <= values["threshold"]:
-            return train_loss, result_nn
-
-    for i in range(parameters["launch_count_simulated_annealing"]):
-        (
-            train_loss,
-            count_epoch,
-            loss_function,
-            optimizer,
-            result_nn,
-            last_iteration,
-        ) = simulated_annealing(**values, **search_algorithm_arguments, **kwargs)
-        if train_loss <= values["threshold"]:
-            return train_loss, result_nn
-
-    values["loss"] = [values["loss"]] + additional_losses
-    values["opt"] = [values["opt"]] + additional_optimizers
-    search_algorithm_arguments.pop("max_iter")
-    (
-        train_loss,
-        count_epoch,
-        loss_function,
-        optimizer,
-        result_nn,
-        last_iteration,
-    ) = full_search(**values, **search_algorithm_arguments, **kwargs)
+    if tags["data size"] == "auto":
+        if data is None:
+            tags["data size"] = "small"
+        else:
+            size = len(data[0])
+            size_id = (
+                0 + int(size // 100 > 0) + int(size // 300 > 0) + int(size // 900 > 0)
+            )
+            tags["data size"] = expert_system_tags["data size"][size_id]
+    if tags["data size"] == "very small":
+        parameters["min_train_epoch"] *= 2
+        parameters["max_train_epoch"] = 700
+        parameters["iteration_count"] += 10
+        parameters["launch_count_random_search"] += 2
+        parameters["launch_count_simulated_annealing"] += 2
+    elif tags["data size"] == "small":
+        parameters["min_train_epoch"] = int(parameters["min_train_epoch"] * 1.5)
+        parameters["iteration_count"] += 10
+        parameters["launch_count_random_search"] += 1
+        parameters["launch_count_simulated_annealing"] += 1
+    elif tags["data size"] == "median":
+        parameters["min_train_epoch"] = int(parameters["min_train_epoch"] * 1.25)
+        parameters["iteration_count"] += 10
+        parameters["launch_count_random_search"] += 1
+    elif tags["data size"] == "big":
+        parameters["launch_count_random_search"] += 1
 
-    return train_loss, result_nn
+    parameters["simulated_annealing_params"] = simulated_annealing_params
+    return parameters
```

### Comparing `degann-1.0/degann/expert/trainer.py` & `degann-1.1/degann/search_algorithms/pattern_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,15 @@
-"""
-Module for training neural networks
-"""
 import random
-from typing import Union, Tuple, List, Dict, Any
+from typing import Union, Any, Tuple, List
 
 import numpy as np
 import tensorflow as tf
 
-from degann.networks import activations, losses
-from degann.networks import imodel
-from degann.networks.callbacks import MemoryCleaner
-from degann.networks.metrics import get_all_metric_functions
-from degann.networks.optimizers import get_all_optimizers
+from degann import MemoryCleaner, get_all_optimizers, get_all_metric_functions
+from degann.networks import activations, imodel, losses
 
 _default_shapes = [
     [10, 10, 10, 10, 10, 10],
     [80, 80, 80],
     [32, 16, 8, 4],
     [4, 8, 16, 32],
     [10, 10],
@@ -61,25 +55,14 @@
     act.append("linear")
     decorator_param.append(None)
 
     nets_param = [shape, act, decorator_param]
     return nets_param
 
 
-def _normalize_two_array(
-    x: np.ndarray, y: np.ndarray
-) -> Tuple[np.ndarray, np.ndarray, float]:
-    m = max(abs(np.amax(x)), abs(np.amax(y)))
-    if m < 1:
-        m = 1
-    x = x / m
-    y = y / m
-    return x, y, m
-
-
 def _normalize_array(x: np.ndarray) -> Tuple[np.ndarray, float]:
     """
     Scale array from [a, b] to [0, 1]
 
     Parameters
     ----------
     x: np.ndarray
@@ -117,15 +100,14 @@
         History of training for this network
     """
     # default config
     args = {
         "debug": False,
         "eps": 1e-2,
         "epochs": 100,
-        "validation_split": 0.2,
         "normalize": False,
         "name_salt": "",
         "loss_function": "MeanSquaredError",
         "optimizer": "SGD",
         "metrics": [
             "MeanSquaredError",
             "MeanAbsoluteError",
@@ -133,15 +115,14 @@
         ],
         "validation_metrics": [
             "MeanSquaredError",
             "MeanAbsoluteError",
             "CosineSimilarity",
         ],
         "use_rand_net": True,
-        "experiments": False,
         "net_type": "DenseNet",
         "nets_param": [
             [
                 shape,  # shape
                 ["sigmoid"] * len(shape) + ["linear"],  # activation functions
                 [None] * (len(shape) + 1),  # decorator parameters for activation
             ]
@@ -287,15 +268,14 @@
     args = {
         "loss_functions": [key for key in losses.get_all_loss_functions()],
         "optimizers": [key for key in get_all_optimizers()],
         "metrics": [key for key in get_all_metric_functions()],
         "validation_metrics": [key for key in get_all_metric_functions()],
         "net_shapes": _default_shapes,
         "activations": [key for key in activations.get_all_activations()],
-        "validation_split": [0.2],
         "rates": [1e-2, 5e-3, 1e-3],
         "epochs": [50, 200],
         "normalize": [False],
     }
 
     for arg in args:
         if kwargs.get(arg) is not None:
@@ -327,30 +307,28 @@
                 ]
             )
 
     metaparams = []
     for loss_func in args["loss_functions"]:
         for normalize in args["normalize"]:
             for optimizer in args["optimizers"]:
-                for validation_split in args["validation_split"]:
-                    for epochs in args["epochs"]:
-                        for rate in args["rates"]:
-                            metaparams.append(dict())
-                            metaparams[-1]["loss_function"] = loss_func
-                            metaparams[-1]["normalize"] = normalize
-                            metaparams[-1]["optimizer"] = optimizer
-                            metaparams[-1]["validation_split"] = validation_split
-                            metaparams[-1]["epochs"] = epochs
-                            metaparams[-1]["eps"] = rate
-                            metaparams[-1]["metrics"] = args["metrics"]
-                            metaparams[-1]["validation_metrics"] = args[
-                                "validation_metrics"
-                            ]
-                            metaparams[-1]["nets_param"] = nets_param
-                            metaparams[-1].update(kwargs)
+                for epochs in args["epochs"]:
+                    for rate in args["rates"]:
+                        metaparams.append(dict())
+                        metaparams[-1]["loss_function"] = loss_func
+                        metaparams[-1]["normalize"] = normalize
+                        metaparams[-1]["optimizer"] = optimizer
+                        metaparams[-1]["epochs"] = epochs
+                        metaparams[-1]["eps"] = rate
+                        metaparams[-1]["metrics"] = args["metrics"]
+                        metaparams[-1]["validation_metrics"] = args[
+                            "validation_metrics"
+                        ]
+                        metaparams[-1]["nets_param"] = nets_param
+                        metaparams[-1].update(kwargs)
 
     best_nets: List[List[dict, float, float, imodel.IModel]] = []
     if kwargs.get("debug"):
         print(f"Grid search size {len(metaparams)}")
         print("Amount of networks for each set of parameters", len(nets_param))
     for i, params in enumerate(metaparams):
         if kwargs.get("debug"):
```

### Comparing `degann-1.0/degann/networks/activations.py` & `degann-1.1/degann/networks/activations.py`

 * *Files identical despite different names*

### Comparing `degann-1.0/degann/networks/callbacks.py` & `degann-1.1/degann/networks/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 class MemoryCleaner(Callback):
     def on_epoch_end(self, epoch, logs=None):
         gc.collect()
         k.clear_session()
 
 
 class MeasureTrainTime(Callback):
+    """
+    Callback for measuring time.
+    Supports measuring training time,
+    measuring the time of each epoch during training,
+    and measuring the running time of the predict method
+    """
+
     def __init__(self):
         super(MeasureTrainTime, self).__init__()
         self.start_train_time = 0
         self.end_train_time = 0
 
         self.start_evaluate_time = 0
         self.end_evaluate_time = 0
@@ -65,14 +72,20 @@
         self.end_train_time = time.perf_counter()
         self.model.trained_time["train_time"] = (
             self.end_train_time - self.start_train_time
         )
 
 
 class LightHistory(History):
+    """
+    Class based on Keras.History,
+    but which only stores information about the last training epoch,
+    not the entire process
+    """
+
     def __init__(self):
         super(History, self).__init__()
         self.history = {}
 
     def on_train_begin(self, logs=None):
         self.epoch = 0
```

### Comparing `degann-1.0/degann/networks/imodel.py` & `degann-1.1/degann/networks/imodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         Parameters
         ----------
         path: str
             path to file with name, without extension
         array_type: str
             c-style or cpp-style ("[]" or "vector")
         path_to_compiler: str
-            path to c/c++ compiler
+            path to c/c++ compiler, if `None` then the resulting code will not be compiled
         kwargs
 
         Returns
         -------
 
         """
         self.network.export_to_cpp(path, array_type, path_to_compiler)
@@ -487,33 +487,10 @@
             weight_init=weight,
             decorator_params=decorator_params,
             **kwargs,
         )
 
         return res
 
-    # perceptron activation is discrete and has no derivatives (gradient)
-    # @classmethod
-    # def create_perceptron(cls, input_size, output_size, shape, threshold=1, **kwargs):
-    #     activation, decorator_params, weight, biases, kwargs = _get_act_and_init(
-    #         kwargs,
-    #         activations.perceptron_threshold,
-    #         [{"threshold": threshold}],
-    #         tf.random_normal_initializer(),
-    #     )
-    #
-    #     res = cls(
-    #         input_size=input_size,
-    #         block_size=shape,
-    #         output_size=output_size,
-    #         activation_func=activation,
-    #         bias_init=biases,
-    #         weight_init=weight,
-    #         decorator_params=decorator_params,
-    #         **kwargs,
-    #     )
-    #
-    #     return res
-
 
 _create_functions = defaultdict(lambda: TensorflowDenseNet)
 _create_functions["DenseNet"] = TensorflowDenseNet
```

### Comparing `degann-1.0/degann/networks/layer_creator.py` & `degann-1.1/degann/networks/layer_creator.py`

 * *Files identical despite different names*

### Comparing `degann-1.0/degann/networks/layers/tf_dense.py` & `degann-1.1/degann/networks/layers/tf_dense.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, List, Tuple, Dict
 
+import numpy as np
 import tensorflow as tf
 from tensorflow import keras
 
 from degann.networks import activations
 from degann.networks.config_format import LAYER_DICT_NAMES
 
 
@@ -50,23 +51,29 @@
             raise "Additional parameters for activation function must be dictionary"
 
         if input_dim == 0 or units == 0:
             raise "Layer cannot have zero inputs or zero size"
 
         super(TensorflowDense, self).__init__(**kwargs)
         w_init = weight_initializer
-        self.w = tf.Variable(
-            initial_value=w_init(shape=(input_dim, units), dtype="float32"),
+        self.w = self.add_weight(
+            shape=(input_dim, units),
+            initializer=w_init,
+            dtype="float32",
+            # initial_value=w_init(shape=(input_dim, units), dtype="float32"),
             name=f"Var_w_{self.name}",
             trainable=True,
         )
         b_init = bias_initializer
-        self.b = tf.Variable(
-            initial_value=b_init(shape=(units,), dtype="float32"),
-            name=f"Var_w_{self.name}",
+        self.b = self.add_weight(
+            shape=(units,),
+            initializer=b_init,
+            dtype="float32",
+            # initial_value=b_init(shape=(units,), dtype="float32"),
+            name=f"Var_b_{self.name}",
             trainable=True,
         )
 
         self.units = units
         self.input_dim = input_dim
         self._is_debug = is_debug
         self.activation_func = activations.get(activation_func)
@@ -107,16 +114,16 @@
         """
         Export layer to dictionary of parameters
         Returns
         -------
         config: dict
             dictionary of parameters
         """
-        w = self.w.value().numpy()
-        b = self.b.value().numpy()
+        w = self.w.value.numpy()
+        b = self.b.value.numpy()
         res = {
             LAYER_DICT_NAMES["shape"]: self.units,
             LAYER_DICT_NAMES["inp_size"]: self.input_dim,
             LAYER_DICT_NAMES["weights"]: w.tolist(),
             LAYER_DICT_NAMES["biases"]: b.tolist(),
             LAYER_DICT_NAMES["layer_type"]: type(self).__name__,
             LAYER_DICT_NAMES["dtype"]: w.dtype.name,
@@ -138,26 +145,22 @@
         ----------
         config
 
         Returns
         -------
 
         """
-        w = config[LAYER_DICT_NAMES["weights"]]
-        b = config[LAYER_DICT_NAMES["biases"]]
+        w = np.array(config[LAYER_DICT_NAMES["weights"]])
+        b = np.array(config[LAYER_DICT_NAMES["biases"]])
         act = config[LAYER_DICT_NAMES["activation"]]
         dec_params = _dec_params_from_list(config[LAYER_DICT_NAMES["decorator_params"]])
-        self.w = tf.Variable(
-            initial_value=w,
-            dtype=config[LAYER_DICT_NAMES["dtype"]],
-            trainable=True,
-        )
-        self.b = tf.Variable(
-            initial_value=b, dtype=config[LAYER_DICT_NAMES["dtype"]], trainable=True
-        )
+        self.set_weights([w, b])
+        # self.b = tf.Variable(
+        #     initial_value=b, dtype=config[LAYER_DICT_NAMES["dtype"]], trainable=True
+        # )
         self.activation_func = activations.get(act)
         self.activation_name = act
         self.decorator_params = dec_params
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
```

### Comparing `degann-1.0/degann/networks/losses.py` & `degann-1.1/degann/networks/losses.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,33 +5,20 @@
 from tensorflow import keras
 
 
 def sign(x):
     return tf.where(x < 0.0, -1.0, 1.0)
 
 
-class RelativeError(tf.keras.losses.Loss, ABC):
-    def __init__(
-        self,
-        reduction=tf.keras.losses.Reduction.NONE,
-        name="relative",
-        eps=1e-6,
-        **kwargs
-    ):
-        super(RelativeError, self).__init__(reduction=reduction, name=name, **kwargs)
-        self.eps = eps
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        y_upd = tf.where(abs(y_true) <= self.eps, 1.0 * sign(y_true), y_true)
-        y = tf.math.divide(y_pred, y_upd)
-        loss = tf.math.reduce_mean(tf.abs(y - 1))
-        return loss
-
-
 class RelativeAbsoluteError(tf.keras.losses.Loss, ABC):
+    """
+    This class provides RAE loss function:
+    $$ RAE = \frac{\Sum^n_{i=1} |y_i - \hat(y)_i|}{\Sum^n_{i=1} |y_i - \bar(y)|}
+    """
+
     def __init__(self, reduction=tf.keras.losses.Reduction.NONE, name="rae", **kwargs):
         super(RelativeAbsoluteError, self).__init__(
             reduction=reduction, name=name, **kwargs
         )
 
     def __call__(self, y_true, y_pred, sample_weight=None):
         true_mean = tf.reduce_mean(y_true)
@@ -45,43 +32,56 @@
         )
 
         loss = squared_error_num / squared_error_den
         return loss
 
 
 class MaxAbsoluteDeviation(tf.keras.losses.Loss, ABC):
+    """
+    This class provides Max Absolute Deviation loss function:
+    $$ MAD = \max |y - \hat(y)|
+    """
+
     def __init__(
         self, reduction=tf.keras.losses.Reduction.NONE, name="my_mae", **kwargs
     ):
         super(MaxAbsoluteDeviation, self).__init__(
             reduction=reduction, name=name, **kwargs
         )
 
     def __call__(self, y_true, y_pred, sample_weight=None):
         loss = tf.math.reduce_max(tf.math.abs(y_true - y_pred))
         return loss
 
 
 class MaxAbsolutePercentageError(tf.keras.losses.Loss, ABC):
+    """
+    This class provides Max Absolute Percentage Error loss function:
+    $$ MAD = \max |\frac{y - \hat(y)}{y}|
+    """
+
     def __init__(
         self, reduction=tf.keras.losses.Reduction.NONE, name="maxAPE", **kwargs
     ):
         super(MaxAbsolutePercentageError, self).__init__(
             reduction=reduction, name=name, **kwargs
         )
 
     def __call__(self, y_true, y_pred, sample_weight=None):
-        loss = tf.math.reduce_max(tf.math.abs((y_true - y_pred) / y_true))
+        loss = tf.math.reduce_max(tf.math.abs((y_true - y_pred) / y_true)) * 100.0
         return loss
 
 
 class RMSE(tf.keras.losses.Loss, ABC):
-    def __init__(
-        self, reduction=tf.keras.losses.Reduction.NONE, name="maxAPE", **kwargs
-    ):
+    """
+    This class provides Root Mean squared Error loss function:
+    $$ MAD = \sqrt{MSE}
+    """
+
+    def __init__(self, reduction=tf.keras.losses.Reduction.NONE, name="RMSE", **kwargs):
         super(RMSE, self).__init__(reduction=reduction, name=name, **kwargs)
 
     def __call__(self, y_true, y_pred, sample_weight=None):
         loss = tf.math.sqrt(tf.math.reduce_mean((y_pred - y_true) ** 2))
         return loss
 
 
@@ -91,19 +91,40 @@
     "LogCosh": keras.losses.LogCosh(),
     "MeanAbsoluteError": keras.losses.MeanAbsoluteError(),
     "MeanAbsolutePercentageError": keras.losses.MeanAbsolutePercentageError(),
     "MaxAbsolutePercentageError": MaxAbsolutePercentageError(),
     "MeanSquaredError": keras.losses.MeanSquaredError(),
     "RootMeanSquaredError": RMSE(),
     "MeanSquaredLogarithmicError": keras.losses.MeanSquaredLogarithmicError(),
-    "RelativeError": RelativeError(),
     "RelativeAbsoluteError": RelativeAbsoluteError(),
     "MaxAbsoluteDeviation": MaxAbsoluteDeviation(),
 }
 
 
 def get_loss(name: str):
+    """
+    Get loss function by name
+    Parameters
+    ----------
+    name: str
+        Name of loss function
+
+    Returns
+    -------
+    loss_class: tf.keras.losses.Loss
+        Result loss function
+    """
     return _losses.get(name)
 
 
-def get_all_loss_functions() -> dict[str, Callable]:
+def get_all_loss_functions() -> dict[str, tf.keras.losses.Loss]:
+    """
+    Get all loss functions
+    Parameters
+    ----------
+
+    Returns
+    -------
+    loss_class: dict[str, tf.keras.losses.Loss]
+        All loss functions
+    """
     return _losses
```

### Comparing `degann-1.0/degann/networks/metrics.py` & `degann-1.1/degann/networks/metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,77 +3,80 @@
 
 import tensorflow as tf
 from tensorflow import keras
 
 from degann.networks.losses import get_all_loss_functions
 
 
-# Non-differentiable
-class InlierRatio(tf.keras.losses.Loss, ABC):
-    def __init__(
-        self,
-        reduction=tf.keras.losses.Reduction.NONE,
-        name="inlier_ratio",
-        threshold=0.05,
-        **kwargs
-    ):
-        super(InlierRatio, self).__init__(reduction=reduction, name=name, **kwargs)
-        self.threshold = threshold
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        y = tf.math.divide((y_true - y_pred), tf.where(y_true == 0.0, 1.0, y_true))
-        loss = tf.math.reduce_mean(tf.where(tf.abs(y) <= self.threshold, 0.0, 1.0))
-        return loss
-
-
-class MaxDeviation(tf.keras.losses.Loss, ABC):
-    def __init__(
-        self,
-        reduction=tf.keras.losses.Reduction.NONE,
-        name="max_deviation",
-        treeshold=0.05,
-        **kwargs
-    ):
-        super(MaxDeviation, self).__init__(reduction=reduction, name=name, **kwargs)
-        self.treeshold = treeshold
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        y = tf.math.divide((y_true - y_pred), tf.where(y_true == 0.0, 1.0, y_true))
-        loss = tf.math.reduce_max(tf.where(tf.abs(y) <= self.treeshold, 0.0, abs(y)))
-        return loss
-
-
-class MeanDeviation(tf.keras.losses.Loss, ABC):
-    def __init__(
-        self,
-        reduction=tf.keras.losses.Reduction.NONE,
-        name="mean_deviation",
-        treeshold=0.05,
-        **kwargs
-    ):
-        super(MeanDeviation, self).__init__(reduction=reduction, name=name, **kwargs)
-        self.treeshold = treeshold
-
-    def __call__(self, y_true, y_pred, sample_weight=None):
-        y = tf.math.divide((y_true - y_pred), tf.where(y_true == 0.0, 1.0, y_true))
-        loss = tf.math.reduce_mean(
-            tf.where(tf.abs(y) <= self.treeshold, self.treeshold, abs(y))
-        )
-        return loss
+# class MaxDeviation(tf.keras.losses.Loss, ABC):
+#     def __init__(
+#         self,
+#         reduction=tf.keras.losses.Reduction.NONE,
+#         name="max_deviation",
+#         treeshold=0.05,
+#         **kwargs
+#     ):
+#         super(MaxDeviation, self).__init__(reduction=reduction, name=name, **kwargs)
+#         self.treeshold = treeshold
+#
+#     def __call__(self, y_true, y_pred, sample_weight=None):
+#         y = tf.math.divide((y_true - y_pred), tf.where(y_true == 0.0, 1.0, y_true))
+#         loss = tf.math.reduce_max(tf.where(tf.abs(y) <= self.treeshold, 0.0, abs(y)))
+#         return loss
+#
+#
+# class MeanDeviation(tf.keras.losses.Loss, ABC):
+#     def __init__(
+#         self,
+#         reduction=tf.keras.losses.Reduction.NONE,
+#         name="mean_deviation",
+#         treeshold=0.05,
+#         **kwargs
+#     ):
+#         super(MeanDeviation, self).__init__(reduction=reduction, name=name, **kwargs)
+#         self.treeshold = treeshold
+#
+#     def __call__(self, y_true, y_pred, sample_weight=None):
+#         y = tf.math.divide((y_true - y_pred), tf.where(y_true == 0.0, 1.0, y_true))
+#         loss = tf.math.reduce_mean(
+#             tf.where(tf.abs(y) <= self.treeshold, self.treeshold, abs(y))
+#         )
+#         return loss
 
 
 _metrics: dict = {
     "RootMeanSquaredError": keras.metrics.RootMeanSquaredError(),
-    "InlierRatio": InlierRatio(),
-    "MaxDeviation": MaxDeviation(),
-    "MeanDeviation": MeanDeviation(),
+    # "MaxDeviation": MaxDeviation(),
+    # "MeanDeviation": MeanDeviation(),
 }
 
 _metrics = dict(get_all_loss_functions(), **_metrics)
 
 
 def get_metric(name: str):
+    """
+    Get metric by name
+    Parameters
+    ----------
+    name: str
+        Name of metric
+
+    Returns
+    -------
+    metric_class: tf.keras.losses.Loss
+        Result metric
+    """
     return _metrics.get(name)
 
 
 def get_all_metric_functions() -> dict[str, Callable]:
+    """
+    Get all metrics
+    Parameters
+    ----------
+
+    Returns
+    -------
+    metric_class: dict[str, tf.keras.losses.Loss]
+        All metrics
+    """
     return _metrics
```

### Comparing `degann-1.0/degann/networks/topology/tf_densenet.py` & `degann-1.1/degann/networks/topology/tf_densenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,23 +167,27 @@
         # Unpack the data. Its structure depends on your model and
         # on what you pass to `fit()`.
         x, y = data
         with tf.GradientTape() as tape:
             y_pred = self(x, training=True)  # Forward pass
             # Compute the loss value
             # (the loss function is configured in `compile()`)
-            loss = self.compiled_loss(y, y_pred, regularization_losses=self.losses)
+            loss = self.compute_loss(y=y, y_pred=y_pred)
 
         # Compute gradients
         trainable_vars = self.trainable_variables
         gradients = tape.gradient(loss, trainable_vars)
         # Update weights
         self.optimizer.apply_gradients(zip(gradients, trainable_vars))
         # Update metrics (includes the metric that tracks the loss)
-        self.compiled_metrics.update_state(y, y_pred)
+        for metric in self.metrics:
+            if metric.name == "loss":
+                metric.update_state(loss)
+            else:
+                metric.update_state(y, y_pred)
         # Return a dict mapping metric names to current value
         return {m.name: m.result() for m in self.metrics}
 
     def set_name(self, new_name):
         self._name = new_name
 
     def __str__(self):
```

### Comparing `degann-1.0/degann/networks/utils.py` & `degann-1.1/degann/networks/utils.py`

 * *Files identical despite different names*

### Comparing `degann-1.0/degann.egg-info/PKG-INFO` & `degann-1.1/degann/degann.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: degann
-Version: 1.0
+Version: 1.1
 Summary: Library for generating artificial neural networks for modeling the behavior of dynamic systems
 Home-page: https://github.com/Krekep/degann
 Author: Pavel Alimov
 Author-email: <pashaalimov@gmail.com>
 License: MIT
 Keywords: python,ode,differential equation,neural network
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DEGANN
 
 [![Check tests](https://github.com/Krekep/degann/actions/workflows/tests.yml/badge.svg)](https://github.com/Krekep/degann/actions/workflows/tests.yml)
 [![License](https://img.shields.io/badge/license-MIT-orange)](https://github.com/Krekep/degann/blob/main/LICENSE)
-[![Package](https://img.shields.io/badge/pypi%20package-1.0-%233776ab)](https://pypi.org/project/degann/)
+[![Package](https://img.shields.io/badge/pypi%20package-1.1-%233776ab)](https://pypi.org/project/degann/)
 
 **DEGANN** is a library generating neural networks for approximating solutions to differential equations. As a backend for working with neural networks, tensorflow is used, but with the ability to expand with your own tools.
 
 **Features**
 - Generation of neural networks by parameters.
 - Construction of tables with the numerical solution of ordinary differential equations of the first order
 - Construction of tables with numerical solution of systems of ordinary differential equations of the first order
@@ -54,9 +53,7 @@
 
 ### Via pip
 Use command
 ```bash
 pip install degann
 ```
 Now you can use the `degann` package
-
-
```

### Comparing `degann-1.0/degann.egg-info/SOURCES.txt` & `degann-1.1/degann/degann.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 LICENSE
 README.md
 setup.py
 degann/__init__.py
-degann.egg-info/PKG-INFO
-degann.egg-info/SOURCES.txt
-degann.egg-info/dependency_links.txt
-degann.egg-info/requires.txt
-degann.egg-info/top_level.txt
+degann/degann.egg-info/PKG-INFO
+degann/degann.egg-info/SOURCES.txt
+degann/degann.egg-info/dependency_links.txt
+degann/degann.egg-info/requires.txt
+degann/degann.egg-info/top_level.txt
 degann/equations/__init__.py
 degann/equations/equation_utils.py
 degann/equations/simple_equation.py
 degann/equations/system_ode.py
 degann/expert/__init__.py
-degann/expert/generate.py
-degann/expert/nn_code.py
-degann/expert/search_algorithms.py
+degann/expert/pipeline.py
 degann/expert/selector.py
-degann/expert/trainer.py
 degann/networks/__init__.py
 degann/networks/activations.py
 degann/networks/callbacks.py
 degann/networks/config_format.py
 degann/networks/cpp_utils.py
 degann/networks/imodel.py
 degann/networks/layer_creator.py
 degann/networks/losses.py
 degann/networks/metrics.py
 degann/networks/optimizers.py
 degann/networks/utils.py
 degann/networks/layers/__init__.py
 degann/networks/layers/tf_dense.py
 degann/networks/topology/__init__.py
-degann/networks/topology/tf_densenet.py
+degann/networks/topology/tf_densenet.py
+degann/search_algorithms/__init__.py
+degann/search_algorithms/generate.py
+degann/search_algorithms/grid_search.py
+degann/search_algorithms/nn_code.py
+degann/search_algorithms/pattern_search.py
+degann/search_algorithms/random_search.py
+degann/search_algorithms/simulated_annealing.py
+degann/search_algorithms/utils.py
```

### Comparing `degann-1.0/setup.py` & `degann-1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pathlib
-from setuptools import setup, find_packages
+from setuptools import setup
 from degann.networks.config_format import VERSION
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 with open(HERE / "README.md", "r", encoding="utf-8") as fh:
@@ -19,15 +19,15 @@
     author="Pavel Alimov",
     author_email="<pashaalimov@gmail.com>",
     url="https://github.com/Krekep/degann",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="MIT",
-    packages=find_packages(),
+    package_dir={"": "degann"},
     install_requires=[
         "keras~=2.12.0",
         "matplotlib~=3.7.1",
         "numpy~=1.23.5",
         "scipy~=1.10.1",
         "tensorflow~=2.12.0",
     ],
```

