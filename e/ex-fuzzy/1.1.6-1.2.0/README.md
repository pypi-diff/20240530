# Comparing `tmp/ex_fuzzy-1.1.6.tar.gz` & `tmp/ex_fuzzy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.1.6.tar", last modified: Tue May 21 15:50:10 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.2.0.tar", last modified: Wed May 29 16:29:40 2024, max compression
```

## Comparing `ex_fuzzy-1.1.6.tar` & `ex_fuzzy-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.714138 ex_fuzzy-1.1.6/
--rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     4185 2024-05-21 15:50:10.714138 ex_fuzzy-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3284 2024-04-22 14:14:00.000000 ex_fuzzy-1.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.658262 ex_fuzzy-1.1.6/ex_fuzzy/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.707284 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0        0        0    15878 2024-04-18 15:39:28.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0        0        0     2693 2024-04-24 13:08:01.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0        0        0    43154 2024-05-20 11:58:00.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0        0        0    18159 2024-05-07 18:39:25.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0        0        0    41778 2024-05-21 15:45:06.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0        0        0    26136 2024-05-06 15:11:07.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0        0        0    16171 2024-04-24 14:42:34.000000 ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.691594 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/
--rw-rw-rw-   0        0        0     4185 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 15:50:10.000000 ex_fuzzy-1.1.6/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 15:50:10.714138 ex_fuzzy-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1773 2024-05-21 15:49:10.000000 ex_fuzzy-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:50:10.713136 ex_fuzzy-1.1.6/tests/
--rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_centroids.py
--rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_classification.py
--rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_eval_tools.py
--rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_fuzzy_sets.py
--rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.6/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:29:40.788379 ex_fuzzy-1.2.0/
+-rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4185 2024-05-29 16:29:40.787376 ex_fuzzy-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2024-04-22 14:14:00.000000 ex_fuzzy-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 16:29:40.729065 ex_fuzzy-1.2.0/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-05-29 16:29:40.762154 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15920 2024-05-29 15:38:40.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2693 2024-04-24 13:08:01.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    43154 2024-05-20 11:58:00.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    18673 2024-05-23 14:06:20.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    41778 2024-05-21 15:45:06.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    29861 2024-05-29 16:18:28.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    16171 2024-04-24 14:42:34.000000 ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:29:40.743169 ex_fuzzy-1.2.0/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     4185 2024-05-29 16:29:40.000000 ex_fuzzy-1.2.0/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-05-29 16:29:40.000000 ex_fuzzy-1.2.0/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:29:40.000000 ex_fuzzy-1.2.0/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-29 16:29:40.000000 ex_fuzzy-1.2.0/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 16:29:40.000000 ex_fuzzy-1.2.0/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 16:29:40.788379 ex_fuzzy-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-05-29 16:28:18.000000 ex_fuzzy-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:29:40.778698 ex_fuzzy-1.2.0/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.2.0/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.2.0/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.2.0/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.2.0/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.2.0/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.1.6/LICENSE` & `ex_fuzzy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/PKG-INFO` & `ex_fuzzy-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex_fuzzy
-Version: 1.1.6
+Version: 1.2.0
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ex_fuzzy-1.1.6/README.md` & `ex_fuzzy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/cognitive_maps.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/cognitive_maps.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_rules.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/eval_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         Returns the matthews correlation coefficient for a classification task using
         the rules evaluated.
 
         :return: mattews correlation coefficient. (float in [-1, 1])
         '''
         from sklearn.metrics import matthews_corrcoef
         self.add_rule_weights()
-        preds = self.mrule_base.winning_rule_predict(self.X)
+        preds = self.mrule_base.winning_rule_predict(self.X, precomputed_truth=self.precomputed_truth)
 
         return matthews_corrcoef(self.y, preds)
 
 
     def size_antecedents_eval(self, tolerance=0.1) -> float:
         '''
         Returns a score between 0 and 1, where 1 means that the rule base only contains almost no antecedents.
```

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/fuzzy_sets.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/fuzzy_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 like computing the FM function, etc.
 
 """
 import enum
 from typing import Generator
 
 import numpy as np
+import pandas as pd
 
 try:
     from . import maintenance as mnt
 except:
     import maintenance as mnt
 
 # You dont require torch to use this module, however, we need to import it to give support in case you feed these methods with torch tensors.
@@ -60,14 +61,19 @@
     aux1 = (x - a) / (b - a)
     aux2 = (d - x) / (d - c)
 
     if isinstance(x, np.ndarray):
         return np.clip(np.minimum(aux1, aux2), 0.0, 1.0)
     elif isinstance(x, torch.Tensor):
         return torch.clamp(torch.min(aux1, aux2), 0.0, 1.0)
+    elif isinstance(x, list):
+        return [np.clip(min(aux1, aux2), 0.0, 1.0) for elem in x]
+    else: # Single value
+        return np.clip(min(aux1, aux2), 0.0, 1.0)
+
 
 
 def __gaussian2(x, params: list[float]) -> np.array:
     '''
     Gaussian membership functions.
 
     :param mean:  real number, mean of the gaussian function.
@@ -150,18 +156,23 @@
         '''
         Computes the membership of a point or vector of elements.
 
         :param x: input values in the referencial domain.
         '''
         if isinstance(x, np.ndarray):
             res = np.equal(x, self.category).astype(float)
-        if torch_available:
-            if isinstance(x, torch.Tensor):
-                res = torch.eq(x, self.category).float()
-
+        elif isinstance(x, torch.Tensor):
+            res = torch.eq(x, self.category).float()
+        elif isinstance(x, list):
+            res = [1.0 if elem == self.category else 0.0 for elem in x]
+        elif isinstance(x, float) or isinstance(x, int):
+            res = 1.0 if x == self.category else 0.0
+        elif isinstance(x, pd.Series):
+            res = x.apply(lambda elem: 1.0 if elem == self.category else 0.0)
+            
         return res
 
 
     def type(self) -> FUZZY_SETS:
         '''
         Returns the corresponding fuzzy set type according to FUZZY_SETS enum.
         '''
```

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/rules.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,14 +90,61 @@
                                  2] = quantile_numbers[pointer + 2]
             partition_parameters[:, partition,
                                  3] = quantile_numbers[pointer + 3]
 
     return partition_parameters
 
 
+def compute_quantiles(x, n_partitions):
+    '''
+    Computes the quantiles needed for n-partition fuzzy membership.
+    
+    :param x: numpy array, vector of shape (samples, ).
+    :param n_partitions: int, number of partitions.
+    :return: numpy array, quantiles for partitioning.
+    '''
+    quantiles = np.linspace(0, 100, n_partitions + 2)
+    return np.percentile(x, quantiles, axis=0)
+
+
+def t1_n_partition_parameters(x, n_partitions):
+    '''
+    Partitions the fuzzy variable in n trapezoidal memberships.
+
+    :param x: numpy array, matrix of shape (samples, variables).
+    :param n_partitions: int, number of partitions.
+    :return: numpy array, tensor of shape (variables, n_partitions, 4) containing the trapezoidal parameters.
+    '''
+    trap_memberships_size = 4
+    n_variables = x.shape[1]
+    quantile_numbers = compute_quantiles(x, n_partitions)
+    
+    # Initialize the array for partition parameters
+    partition_parameters = np.zeros((n_variables, n_partitions, trap_memberships_size))
+
+    for partition in range(n_partitions):
+        if partition == 0:  # First partition
+            partition_parameters[:, partition, 0] = quantile_numbers[0, :]
+            partition_parameters[:, partition, 1] = quantile_numbers[0, :]
+            partition_parameters[:, partition, 2] = quantile_numbers[1, :]
+            partition_parameters[:, partition, 3] = quantile_numbers[2, :]
+        elif partition == n_partitions - 1:  # Last partition
+            partition_parameters[:, partition, 0] = quantile_numbers[partition, :]
+            partition_parameters[:, partition, 1] = quantile_numbers[partition + 1, :]
+            partition_parameters[:, partition, 2] = quantile_numbers[partition + 2, :]
+            partition_parameters[:, partition, 3] = quantile_numbers[partition + 2, :]
+        else:  # Intermediate partitions
+            partition_parameters[:, partition, 0] = quantile_numbers[partition, :]
+            partition_parameters[:, partition, 1] = (quantile_numbers[partition, :] + quantile_numbers[partition + 1, :] ) / 2
+            partition_parameters[:, partition, 2] = (quantile_numbers[partition + 1, :] + quantile_numbers[partition + 2, :] ) / 2
+            partition_parameters[:, partition, 3] = quantile_numbers[partition + 2, :]
+
+    return partition_parameters
+
+
 def t1_three_partition(x: np.array) -> np.array:
     '''
     Partitions the fuzzy variable in three trapezoidal memberships.
 
     :param x: numpy array, vector of shape (samples, ).
     :return: numpy array, vector of shape (variables, 3, 4).
     '''
@@ -125,147 +172,158 @@
             partition_parameters[:, partition, 1] = quantile_numbers[3]
             partition_parameters[:, partition, 2] = quantile_numbers[4]
             partition_parameters[:, partition, 3] = quantile_numbers[4]
 
     return partition_parameters
 
 
-def t2_simple_partition(x: np.array) -> np.array:
+def t2_n_partition_parameters(x, n_partitions):
     '''
-    Partitions the fuzzy variable in three trapezoidal memberships.
+    Partitions the fuzzy variable in n trapezoidal memberships.
 
-    :param x: numpy array, vector of shape (samples, ).
-    :return: numpy array, vector of shape (variables, 3, 4, 2).
+    :param x: numpy array, matrix of shape (samples, variables).
+    :param n_partitions: int, number of partitions.
+    :return: numpy array, tensor of shape (variables, n_partitions, 4, 2) containing the trapezoidal parameters.
     '''
-    n_partitions = 3
     trap_memberships_size = 4
-    quantile_numbers = partition3_quantile_compute(x)
+    n_variables = x.shape[1]
+    quantile_numbers = compute_quantiles(x, n_partitions)
+    
+    # Initialize the array for partition parameters
+    partition_parameters = np.zeros((n_variables, n_partitions, trap_memberships_size, 2))
 
-    partition_parameters = np.zeros(
-        (x.shape[1], n_partitions, trap_memberships_size, 2))
     for partition in range(n_partitions):
-        if partition == 0:
+        if partition == 0:  # First partition
             partition_parameters[:, partition, 0, 1] = quantile_numbers[0]
             partition_parameters[:, partition, 1, 1] = quantile_numbers[0]
             partition_parameters[:, partition, 2, 1] = quantile_numbers[1]
             partition_parameters[:, partition, 3, 1] = quantile_numbers[2]
 
             partition_parameters[:, partition, 0, 0] = quantile_numbers[0]
             partition_parameters[:, partition, 1, 0] = quantile_numbers[0]
             partition_parameters[:, partition, 2, 0] = quantile_numbers[1]
             partition_parameters[:, partition, 3, 0] = quantile_numbers[1] + \
                 0.9 * (quantile_numbers[2] - quantile_numbers[1])
-
-        elif partition == 1:
-            partition_parameters[:, partition, 0, 1] = quantile_numbers[1]
-            partition_parameters[:, partition, 1, 1] = (
-                quantile_numbers[1] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 2, 1] = (
-                quantile_numbers[2] + quantile_numbers[3]) / 2
-            partition_parameters[:, partition, 3, 1] = quantile_numbers[3]
-
-            partition_parameters[:, partition, 0, 0] = quantile_numbers[1] + \
-                0.1 * (quantile_numbers[2] - quantile_numbers[1])
-            partition_parameters[:, partition, 1, 0] = (
-                quantile_numbers[1] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 2, 0] = (
-                quantile_numbers[3] + quantile_numbers[2]) / 2
-            partition_parameters[:, partition, 3, 0] = quantile_numbers[2] + \
-                0.9 * (quantile_numbers[3] - quantile_numbers[2])
-
-        else:
-            partition_parameters[:, partition, 0, 1] = quantile_numbers[2]
-            partition_parameters[:, partition, 1, 1] = quantile_numbers[3]
-            partition_parameters[:, partition, 2, 1] = quantile_numbers[4]
-            partition_parameters[:, partition, 3, 1] = quantile_numbers[4]
-
-            partition_parameters[:, partition, 0, 0] = quantile_numbers[2] + \
-                0.1 * (quantile_numbers[3] - quantile_numbers[2])
-            partition_parameters[:, partition, 1, 0] = quantile_numbers[3]
-            partition_parameters[:, partition, 2, 0] = quantile_numbers[4]
-            partition_parameters[:, partition, 3, 0] = quantile_numbers[4]
+        elif partition == n_partitions - 1:  # Last partition
+            partition_parameters[:, partition, 0, 1] = quantile_numbers[partition]
+            partition_parameters[:, partition, 1, 1] = quantile_numbers[partition + 1]
+            partition_parameters[:, partition, 2, 1] = quantile_numbers[partition + 2]
+            partition_parameters[:, partition, 3, 1] = quantile_numbers[partition + 2]
+
+            partition_parameters[:, partition, 0, 0] = quantile_numbers[partition] + \
+                0.1 * (quantile_numbers[partition + 1] - quantile_numbers[partition])
+            partition_parameters[:, partition, 1, 0] = quantile_numbers[partition + 1]
+            partition_parameters[:, partition, 2, 0] = quantile_numbers[partition + 2]
+            partition_parameters[:, partition, 3, 0] = quantile_numbers[partition + 2]
+        else:  # Intermediate partitions
+            partition_parameters[:, partition, 0, 1] = quantile_numbers[partition]
+            partition_parameters[:, partition, 1, 1] = (quantile_numbers[partition] + quantile_numbers[partition + 1]) / 2
+            partition_parameters[:, partition, 2, 1] = (quantile_numbers[partition + 1] + quantile_numbers[partition + 2]) / 2
+            partition_parameters[:, partition, 3, 1] = quantile_numbers[partition + 2]
+
+            partition_parameters[:, partition, 0, 0] = quantile_numbers[partition] + \
+                0.1 * (quantile_numbers[partition + 1] - quantile_numbers[partition])
+            partition_parameters[:, partition, 1, 0] = (quantile_numbers[partition] + quantile_numbers[partition + 1]) / 2
+            partition_parameters[:, partition, 2, 0] = (quantile_numbers[partition + 1] + quantile_numbers[partition + 2]) / 2
+            partition_parameters[:, partition, 3, 0] = quantile_numbers[partition + 2] + \
+                0.9 * (quantile_numbers[partition + 3] - quantile_numbers[partition + 2])
 
     return partition_parameters
 
 
-def t1_fuzzy_partitions_dataset(x0: np.array) -> list[fs.fuzzyVariable]:
+def t1_fuzzy_partitions_dataset(x0: np.array, n_partition=3) -> list[fs.fuzzyVariable]:
     '''
     Partitions the dataset features into different fuzzy variables. Parameters are prefixed.
     Use it for simple testing and initial solution.
 
     :param x: numpy array|pandas dataframe, shape samples x features.
+    :param n_partition: number of partitions to use in the fuzzy variables.
     :return: list of fuzzy variables.
     '''
-    tripartition_names = ['Low', 'Medium', 'High']
+    if n_partition == 3:
+        partition_names = ['Low', 'Medium', 'High']
+    elif n_partition == 5:
+        partition_names = ['Very Low', 'Low', 'Medium', 'High', 'Very High']
+    else:
+        partition_names = [str(ix) for ix in range(n_partition)]
+
     try:
         fv_names = x0.columns
         x = x0.values
     except AttributeError:
         fv_names = [str(ix) for ix in range(x0.shape[1])]
         x = x0
 
     mins = np.min(x, axis=0)
     maxs = np.max(x, axis=0)
-    fz_memberships = t1_three_partition(x)
+    fz_memberships = t1_n_partition_parameters(x, n_partitions=n_partition)
     res = []
     for fz_parameter in range(fz_memberships.shape[0]):
-        fzs = [fs.FS(tripartition_names[ix], fz_memberships[fz_parameter, ix, :], [
+        fzs = [fs.FS(partition_names[ix], fz_memberships[fz_parameter, ix, :], [
                      mins[fz_parameter], maxs[fz_parameter]]) for ix in range(fz_memberships.shape[1])]
         res.append(fs.fuzzyVariable(fv_names[fz_parameter], fzs))
 
     return res
 
 
-def t2_fuzzy_partitions_dataset(x0: np.array) -> list[fs.fuzzyVariable]:
+def t2_fuzzy_partitions_dataset(x0: np.array, n_partition=3) -> list[fs.fuzzyVariable]:
     '''
     Partitions the dataset features into different fuzzy variables using iv fuzzy sets. Parameters are prefixed.
     Use it for simple testing and initial solution.
 
     :param x: numpy array|pandas dataframe, shape samples x features.
+    :param n_partition: number of partitions to use in the fuzzy variables.
     :return: list of fuzzy variables.
     '''
-    tripartition_names = ['Low', 'Medium', 'High']
+    if n_partition == 3:
+        partition_names = ['Low', 'Medium', 'High']
+    elif n_partition == 5:
+        partition_names = ['Very Low', 'Low', 'Medium', 'High', 'Very High']
+    else:
+        partition_names = [str(ix) for ix in range(n_partition)]
+
     try:
         fv_names = x0.columns
         x = x0.values
     except AttributeError:
         fv_names = [str(ix) for ix in range(x0.shape[1])]
         x = x0
 
     mins = np.min(x, axis=0)
     maxs = np.max(x, axis=0)
-    fz_memberships = t2_simple_partition(x)
+    fz_memberships = t2_n_partition_parameters(x, n_partition)
     res = []
     for fz_parameter in range(fz_memberships.shape[0]):
-        fzs = [fs.IVFS(tripartition_names[ix], fz_memberships[fz_parameter, ix, :, 0], fz_memberships[fz_parameter, ix, :, 1], [
+        fzs = [fs.IVFS(partition_names[ix], fz_memberships[fz_parameter, ix, :, 0], fz_memberships[fz_parameter, ix, :, 1], [
                        mins[fz_parameter], maxs[fz_parameter]], lower_height=0.8) for ix in range(fz_memberships.shape[1])]
         res.append(fs.fuzzyVariable(fv_names[fz_parameter], fzs))
 
     return res
 
 
-def gt2_fuzzy_partitions_dataset(x0: np.array, resolution_exp:int=1) -> list[fs.fuzzyVariable]:
+def gt2_fuzzy_partitions_dataset(x0: np.array, resolution_exp:int=2, n_partition=3) -> list[fs.fuzzyVariable]:
     '''
     Partitions the dataset features into different fuzzy variables using gt2 fuzzy sets. Parameters are prefixed.
     Use it for simple testing and initial solution.
 
     :param x: numpy array|pandas dataframe, shape samples x features.
-    :param resolution_exp: exponent of the resolution of the partition. Default is -2, which means 0.01. (Number of significant decimals)
+    :param resolution_exp: exponent of the resolution of the partition. Default is 2, which means 0.01. (Number of significant decimals)
+    :param n_partition: number of partitions to use in the fuzzy variables.
     :return: list of fuzzy variables.
     '''
     try:
         fv_names = x0.columns
         x = x0.values
     except AttributeError:
         fv_names = [str(ix) for ix in range(x0.shape[1])]
         x = x0
 
     mins = np.min(x, axis=0)
     maxs = np.max(x, axis=0)
-    iv_simple_partition = t2_fuzzy_partitions_dataset(x)
+    iv_simple_partition = t2_fuzzy_partitions_dataset(x, n_partition=n_partition)
     resolution = 10.0**-np.abs(resolution_exp)
     res = []
     # We iterate through all possible variables
     for ix_var, fz_var in enumerate(iv_simple_partition):
         domain_resolution = np.arange(
             mins[ix_var], maxs[ix_var] + resolution, resolution)
         fzs = []
@@ -281,21 +339,22 @@
                        mins[ix_var], maxs[ix_var]], significant_decimals=np.abs(resolution_exp), unit_resolution=0.01))
 
         res.append(fs.fuzzyVariable(fv_names[ix_var], fzs))
 
     return res
 
 
-def construct_partitions(X : np.array, fz_type_studied:fs.FUZZY_SETS, categorical_mask: np.array=None) -> list[fs.fuzzyVariable]:
+def construct_partitions(X : np.array, fz_type_studied:fs.FUZZY_SETS=fs.FUZZY_SETS.t1, categorical_mask: np.array=None, n_partitions=3) -> list[fs.fuzzyVariable]:
     '''
     Returns a list of linguistic variables according to the kind of fuzzy specified.
 
     :param X: numpy array|pandas dataframe, shape samples x features.
     :param fz_type_studied: fuzzy set type studied.
     :param categorial_mask: a boolean mask vector that indicates for each variables if its categorical or not.
+    :param n_partitions: number of partitions to use in the fuzzy set.
     '''
     if mnt.save_usage_flag:
         mnt.usage_data[mnt.usage_categories.Funcs]['precompute_labels'] += 1
         mnt.usage_data[mnt.usage_categories.FuzzySets][fz_type_studied.name] += 1
 
     if isinstance(X, pd.DataFrame):
         feat_names = X.columns
@@ -306,19 +365,19 @@
     # Get the X dataframe without the categorical variables
     if categorical_mask is not None:
         X_numerical = X[:, np.logical_not(categorical_mask)]
     else:
         X_numerical = X
 
     if fz_type_studied == fs.FUZZY_SETS.t1:
-        precomputed_partitions = t1_fuzzy_partitions_dataset(X_numerical)
+        precomputed_partitions = t1_fuzzy_partitions_dataset(X_numerical, n_partitions)
     elif fz_type_studied == fs.FUZZY_SETS.t2:
-        precomputed_partitions = t2_fuzzy_partitions_dataset(X_numerical)
+        precomputed_partitions = t2_fuzzy_partitions_dataset(X_numerical, n_partitions)
     elif fz_type_studied == fs.FUZZY_SETS.gt2:
-        precomputed_partitions = gt2_fuzzy_partitions_dataset(X_numerical)
+        precomputed_partitions = gt2_fuzzy_partitions_dataset(X_numerical, n_partitions)
 
 
     if categorical_mask is not None:
         categorical_partition = {}
         for ix, elem in enumerate(categorical_mask):
             if elem:
                 if isinstance(X, pd.DataFrame):
```

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.2.0/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy.egg-info/PKG-INFO` & `ex_fuzzy-1.2.0/ex_fuzzy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex-fuzzy
-Version: 1.1.6
+Version: 1.2.0
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ex_fuzzy-1.1.6/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.2.0/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/setup.py` & `ex_fuzzy-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DISTNAME = "ex_fuzzy"
 DESCRIPTION = "Library to perform explainable AI using fuzzy logic."
 MAINTAINER = "Javier Fumanal Idocin"
 MAINTAINER_EMAIL = "javierfumanalidocin@gmail.com"
 URL = "https://github.com/Fuminides/ex-fuzzy"
 LICENSE = "GPL-3.0"
 DOWNLOAD_URL = "https://pypi.org/project/ex-fuzzy/"
-VERSION = "1.1.6"
+VERSION = "1.2.0"
 INSTALL_REQUIRES = ["numpy", "networkx", "matplotlib", "pymoo", "pandas", "scikit-learn"]
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
```

### Comparing `ex_fuzzy-1.1.6/tests/test_centroids.py` & `ex_fuzzy-1.2.0/tests/test_centroids.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/tests/test_classification.py` & `ex_fuzzy-1.2.0/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/tests/test_eval_tools.py` & `ex_fuzzy-1.2.0/tests/test_eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.2.0/tests/test_fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.6/tests/test_utils.py` & `ex_fuzzy-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

