# Comparing `tmp/pyanfis-0.1.5.tar.gz` & `tmp/pyanfis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanfis-0.1.5.tar", last modified: Fri May 24 12:03:12 2024, max compression
+gzip compressed data, was "pyanfis-0.1.6.tar", last modified: Wed May 29 11:34:48 2024, max compression
```

## Comparing `pyanfis-0.1.5.tar` & `pyanfis-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.831744 pyanfis-0.1.5/
--rw-r--r--   0 vicente    (501) staff       (20)     1073 2024-05-20 13:06:33.000000 pyanfis-0.1.5/LICENSE
--rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-24 12:03:12.831552 pyanfis-0.1.5/PKG-INFO
--rw-r--r--   0 vicente    (501) staff       (20)     1193 2024-05-13 09:31:46.000000 pyanfis-0.1.5/README.md
--rw-r--r--   0 vicente    (501) staff       (20)      457 2024-05-24 12:03:06.000000 pyanfis-0.1.5/pyproject.toml
--rw-r--r--   0 vicente    (501) staff       (20)       38 2024-05-24 12:03:12.831782 pyanfis-0.1.5/setup.cfg
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.824463 pyanfis-0.1.5/src/
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.825653 pyanfis-0.1.5/src/pyanfis/
--rw-r--r--   0 vicente    (501) staff       (20)       45 2024-05-22 16:48:25.000000 pyanfis-0.1.5/src/pyanfis/__init__.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.826982 pyanfis-0.1.5/src/pyanfis/algorithms/
--rw-r--r--   0 vicente    (501) staff       (20)     1136 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/algorithms/LSTSQ.py
--rw-r--r--   0 vicente    (501) staff       (20)     1207 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/algorithms/RLSE.py
--rw-r--r--   0 vicente    (501) staff       (20)       76 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/algorithms/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)    20000 2024-05-24 11:56:58.000000 pyanfis-0.1.5/src/pyanfis/anfis.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.827251 pyanfis-0.1.5/src/pyanfis/antecedents/
--rwxr-xr-x   0 vicente    (501) staff       (20)       63 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/antecedents/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)     1760 2024-05-22 17:02:39.000000 pyanfis-0.1.5/src/pyanfis/antecedents/antecedents.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.827519 pyanfis-0.1.5/src/pyanfis/consequents/
--rwxr-xr-x   0 vicente    (501) staff       (20)      212 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/consequents/__init__.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1869 2024-05-24 12:02:29.000000 pyanfis-0.1.5/src/pyanfis/consequents/consequents.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.828080 pyanfis-0.1.5/src/pyanfis/consequents/types/
--rwxr-xr-x   0 vicente    (501) staff       (20)     1085 2024-05-22 17:06:25.000000 pyanfis-0.1.5/src/pyanfis/consequents/types/algorithm.py
--rw-r--r--   0 vicente    (501) staff       (20)      841 2024-05-22 17:06:33.000000 pyanfis-0.1.5/src/pyanfis/consequents/types/lee.py
--rw-r--r--   0 vicente    (501) staff       (20)     1600 2024-05-22 17:42:19.000000 pyanfis-0.1.5/src/pyanfis/consequents/types/takagi_sugeno.py
--rw-r--r--   0 vicente    (501) staff       (20)     2156 2024-05-24 12:01:33.000000 pyanfis-0.1.5/src/pyanfis/consequents/types/tsukamoto.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.829642 pyanfis-0.1.5/src/pyanfis/functions/
--rw-r--r--   0 vicente    (501) staff       (20)      287 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/functions/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)      979 2024-05-17 09:25:31.000000 pyanfis-0.1.5/src/pyanfis/functions/bell.py
--rw-r--r--   0 vicente    (501) staff       (20)     1462 2024-05-24 11:41:24.000000 pyanfis-0.1.5/src/pyanfis/functions/gauss.py
--rw-r--r--   0 vicente    (501) staff       (20)     1567 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/functions/heaviside.py
--rw-r--r--   0 vicente    (501) staff       (20)     1164 2024-05-17 09:21:58.000000 pyanfis-0.1.5/src/pyanfis/functions/linear_s.py
--rw-r--r--   0 vicente    (501) staff       (20)     1186 2024-05-17 09:22:02.000000 pyanfis-0.1.5/src/pyanfis/functions/linear_z.py
--rw-r--r--   0 vicente    (501) staff       (20)      837 2024-05-17 09:22:06.000000 pyanfis-0.1.5/src/pyanfis/functions/sigmoid.py
--rw-r--r--   0 vicente    (501) staff       (20)     3461 2024-05-13 17:43:56.000000 pyanfis-0.1.5/src/pyanfis/functions/universe.py
--rw-r--r--   0 vicente    (501) staff       (20)      293 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/functions/utils.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.830111 pyanfis-0.1.5/src/pyanfis/optimizers/
--rw-r--r--   0 vicente    (501) staff       (20)       54 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/optimizers/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)     6877 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/optimizers/fuzzySGD.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.830908 pyanfis-0.1.5/src/pyanfis/rules/
--rwxr-xr-x   0 vicente    (501) staff       (20)       46 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/rules/__init__.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     2904 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/rules/intersection_algorithms.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1527 2024-05-13 09:31:46.000000 pyanfis-0.1.5/src/pyanfis/rules/relation_algorithms.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1917 2024-05-22 17:05:40.000000 pyanfis-0.1.5/src/pyanfis/rules/rules.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 12:03:12.831370 pyanfis-0.1.5/src/pyanfis.egg-info/
--rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-24 12:03:12.000000 pyanfis-0.1.5/src/pyanfis.egg-info/PKG-INFO
--rw-r--r--   0 vicente    (501) staff       (20)     1144 2024-05-24 12:03:12.000000 pyanfis-0.1.5/src/pyanfis.egg-info/SOURCES.txt
--rw-r--r--   0 vicente    (501) staff       (20)        1 2024-05-24 12:03:12.000000 pyanfis-0.1.5/src/pyanfis.egg-info/dependency_links.txt
--rw-r--r--   0 vicente    (501) staff       (20)        8 2024-05-24 12:03:12.000000 pyanfis-0.1.5/src/pyanfis.egg-info/top_level.txt
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.383859 pyanfis-0.1.6/
+-rw-r--r--   0 vicente    (501) staff       (20)     1073 2024-05-20 13:06:33.000000 pyanfis-0.1.6/LICENSE
+-rw-r--r--   0 vicente    (501) staff       (20)     2315 2024-05-29 11:34:48.383616 pyanfis-0.1.6/PKG-INFO
+-rw-r--r--   0 vicente    (501) staff       (20)     1849 2024-05-29 10:58:12.000000 pyanfis-0.1.6/README.md
+-rw-r--r--   0 vicente    (501) staff       (20)      456 2024-05-27 04:45:38.000000 pyanfis-0.1.6/pyproject.toml
+-rw-r--r--   0 vicente    (501) staff       (20)       38 2024-05-29 11:34:48.383900 pyanfis-0.1.6/setup.cfg
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.377384 pyanfis-0.1.6/src/
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.378471 pyanfis-0.1.6/src/pyanfis/
+-rw-r--r--   0 vicente    (501) staff       (20)       45 2024-05-22 16:48:25.000000 pyanfis-0.1.6/src/pyanfis/__init__.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.379466 pyanfis-0.1.6/src/pyanfis/algorithms/
+-rw-r--r--   0 vicente    (501) staff       (20)     1136 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/algorithms/LSTSQ.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1234 2024-05-28 13:58:26.000000 pyanfis-0.1.6/src/pyanfis/algorithms/RLSE.py
+-rw-r--r--   0 vicente    (501) staff       (20)      146 2024-05-28 13:51:52.000000 pyanfis-0.1.6/src/pyanfis/algorithms/__init__.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1135 2024-05-28 13:56:36.000000 pyanfis-0.1.6/src/pyanfis/algorithms/algorithm.py
+-rw-r--r--   0 vicente    (501) staff       (20)    19942 2024-05-29 05:18:17.000000 pyanfis-0.1.6/src/pyanfis/anfis.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.379767 pyanfis-0.1.6/src/pyanfis/antecedents/
+-rwxr-xr-x   0 vicente    (501) staff       (20)       63 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/antecedents/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1760 2024-05-22 17:02:39.000000 pyanfis-0.1.6/src/pyanfis/antecedents/antecedents.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.380066 pyanfis-0.1.6/src/pyanfis/consequents/
+-rwxr-xr-x   0 vicente    (501) staff       (20)      212 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/consequents/__init__.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1869 2024-05-24 12:02:29.000000 pyanfis-0.1.6/src/pyanfis/consequents/consequents.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.380532 pyanfis-0.1.6/src/pyanfis/consequents/types/
+-rw-r--r--   0 vicente    (501) staff       (20)      841 2024-05-22 17:06:33.000000 pyanfis-0.1.6/src/pyanfis/consequents/types/lee.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1625 2024-05-29 09:36:38.000000 pyanfis-0.1.6/src/pyanfis/consequents/types/takagi_sugeno.py
+-rw-r--r--   0 vicente    (501) staff       (20)     2156 2024-05-24 12:01:33.000000 pyanfis-0.1.6/src/pyanfis/consequents/types/tsukamoto.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.381697 pyanfis-0.1.6/src/pyanfis/functions/
+-rw-r--r--   0 vicente    (501) staff       (20)      287 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/functions/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)      979 2024-05-17 09:25:31.000000 pyanfis-0.1.6/src/pyanfis/functions/bell.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1462 2024-05-24 11:41:24.000000 pyanfis-0.1.6/src/pyanfis/functions/gauss.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1567 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/functions/heaviside.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1164 2024-05-27 04:44:06.000000 pyanfis-0.1.6/src/pyanfis/functions/linear_s.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1186 2024-05-17 09:22:02.000000 pyanfis-0.1.6/src/pyanfis/functions/linear_z.py
+-rw-r--r--   0 vicente    (501) staff       (20)      837 2024-05-17 09:22:06.000000 pyanfis-0.1.6/src/pyanfis/functions/sigmoid.py
+-rw-r--r--   0 vicente    (501) staff       (20)     3461 2024-05-13 17:43:56.000000 pyanfis-0.1.6/src/pyanfis/functions/universe.py
+-rw-r--r--   0 vicente    (501) staff       (20)      293 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/functions/utils.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.382152 pyanfis-0.1.6/src/pyanfis/pyplot/
+-rw-r--r--   0 vicente    (501) staff       (20)      139 2024-05-29 08:25:26.000000 pyanfis-0.1.6/src/pyanfis/pyplot/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1015 2024-05-28 12:58:03.000000 pyanfis-0.1.6/src/pyanfis/pyplot/functions_plotting.py
+-rw-r--r--   0 vicente    (501) staff       (20)     4391 2024-05-29 08:24:13.000000 pyanfis-0.1.6/src/pyanfis/pyplot/structure_plotting.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.382771 pyanfis-0.1.6/src/pyanfis/rules/
+-rwxr-xr-x   0 vicente    (501) staff       (20)       46 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/rules/__init__.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     2904 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/rules/intersection_algorithms.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1527 2024-05-13 09:31:46.000000 pyanfis-0.1.6/src/pyanfis/rules/relation_algorithms.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1917 2024-05-22 17:05:40.000000 pyanfis-0.1.6/src/pyanfis/rules/rules.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-29 11:34:48.383364 pyanfis-0.1.6/src/pyanfis.egg-info/
+-rw-r--r--   0 vicente    (501) staff       (20)     2315 2024-05-29 11:34:48.000000 pyanfis-0.1.6/src/pyanfis.egg-info/PKG-INFO
+-rw-r--r--   0 vicente    (501) staff       (20)     1180 2024-05-29 11:34:48.000000 pyanfis-0.1.6/src/pyanfis.egg-info/SOURCES.txt
+-rw-r--r--   0 vicente    (501) staff       (20)        1 2024-05-29 11:34:48.000000 pyanfis-0.1.6/src/pyanfis.egg-info/dependency_links.txt
+-rw-r--r--   0 vicente    (501) staff       (20)        8 2024-05-29 11:34:48.000000 pyanfis-0.1.6/src/pyanfis.egg-info/top_level.txt
```

### Comparing `pyanfis-0.1.5/LICENSE` & `pyanfis-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/algorithms/LSTSQ.py` & `pyanfis-0.1.6/src/pyanfis/algorithms/LSTSQ.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/algorithms/RLSE.py` & `pyanfis-0.1.6/src/pyanfis/algorithms/RLSE.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     Returns
     -------
     torch.tensor
         a tensor of equal size to the input tensor
     """
     def __init__(self, n_vars, initial_gamma=1000.):
         super().__init__()
-        self.S = torch.eye(n_vars) * initial_gamma
-        self.theta = torch.zeros((n_vars, 1))
-        self.gamma = 1000
+        self.S = torch.eye(n_vars, dtype=float) * initial_gamma
+        self.theta = torch.zeros((n_vars, 1), dtype=float)
+        self.gamma = 1000.0
 
     def forward(self, A, B,):
         batch, row, _ = A.size()
 
         for ba in range(batch):
             for i in range(row):
                 a = A[ba, i, :].view(1, -1)  # Reshape a to match the dimensions for matrix operations
                 b = B[ba, i].unsqueeze(0)
                 
                 self.S = self.S - (torch.matmul(torch.matmul(torch.matmul(self.S, a.T), a), self.S)) / (1 + torch.matmul(torch.matmul(a, self.S), a.T))
                 self.theta =  self.theta + torch.matmul(self.S, torch.matmul(a.T, (b - torch.matmul(a, self.theta))))
 
-        #return self.theta
+        return self.theta
```

### Comparing `pyanfis-0.1.5/src/pyanfis/anfis.py` & `pyanfis-0.1.6/src/pyanfis/anfis.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         elif dimensions == 1:
             return tensor_list.view(1,shape[0],-1)
         elif dimensions == 2:
             return tensor_list.view(shape[0], shape[1],-1)
         elif dimensions == 3:
             return tensor_list.view(shape[0], shape[1] * shape[2] , -1) 
         
-    def _prepare_keywords_matrices(self, **kwargs):
+    def _prepare_kwargs_matrices(self, **kwargs):
         antecedents_tensor = []
         for universe in self.antecedents.universes.values():
             if universe.name not in list(kwargs.keys()):
                 raise ValueError(f"Universe name {universe.name} not present in input variables {list(kwargs.keys())}")
             antecedents_tensor.append(kwargs[universe.name])
             del kwargs[universe.name]
         
@@ -164,15 +164,15 @@
             consequents_tensor.append(kwargs[universe.name])
             del kwargs[universe.name]
 
         return self.smart_concat(antecedents_tensor), self.smart_concat(consequents_tensor)
 
     def get_fired_rules(self, **kwargs):
         self.training = False
-        X, _ = self._prepare_keywords_matrices(**kwargs)
+        X, _ = self._prepare_kwargs_matrices(**kwargs)
         if X.size(1) != 1:
             raise ValueError(f"Only one row can be evaluated at a time")
 
         f = self.antecedents(X)
 
         self.rules.active_rules = self.active_rules
         f, _ = self.rules(f) # col_indexes = rule place on each col
@@ -360,37 +360,37 @@
         f = self.normalisation(f, dim=2, p=1)
 
         self.consequents.consequents.active_rules = self.active_rules_consequents
         output = self.consequents(f, X, Y)
 
         return output
     
-    
+    def _prepare_args_matrices(self, args):
+        if len(args) > 2:
+            raise ValueError("Please provide as input either a matrix with the input arguments or two matrices, one with input arguments and one with objective arguments")
+
+        if self.parameters_update == "backward" and len(args) >= 2:
+            raise ValueError(f"The selected propagation is {self.parameters_update} but you provided more than one tensor as input. Please, join all the input tensors before feeding them into the system.") 
+
+        if self.parameters_update == "backward" or len(args) == 1:
+            return args[0], None
+        
+        else:
+            return args[0], args[1]
+
     def __call__(self, *args, **kwargs):
-        '''
-        In the call step I will preprocess the data and discern if 
-        I am being asked a control/regression or a classification task.
-        '''
 
         if args and kwargs:
             raise ValueError("All the arguments must be either arguments or keyword arguments, but you cannot mix between both")
 
         if args and not isinstance(args[0], torch.Tensor):
             raise ValueError(f"Expected torch.Tensor as input but recived {type(args)}")
         
         if kwargs:
-            X, Y = self._prepare_keywords_matrices(**kwargs)
+            X, Y = self._prepare_kwargs_matrices(**kwargs)
         
         else:
-            if len(args) > 2:
-                raise ValueError("Please provide as input either a matrix with the input arguments or two matrices, one with input arguments and one with objective arguments")
-
-            if self.parameters_update == "backward" and len(args) >= 2:
-                raise ValueError(f"The selected propagation is {self.parameters_update} but you provided more than one tensor as input. Please, join all the input tensors before feeding them into the system.") 
-
-            if self.parameters_update == "backward":
-                X, Y = args[0], None
-            else:
-                X, Y = args
-        #X, Y = self._sanity_check(X), self._sanity_check(Y)
+            X, Y = self._prepare_args_matrices(args)
+            
+        X, Y = self._sanity_check(X), self._sanity_check(Y)
 
         return self.forward(X, Y)
```

### Comparing `pyanfis-0.1.5/src/pyanfis/antecedents/antecedents.py` & `pyanfis-0.1.6/src/pyanfis/antecedents/antecedents.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/consequents/consequents.py` & `pyanfis-0.1.6/src/pyanfis/consequents/consequents.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/consequents/types/algorithm.py` & `pyanfis-0.1.6/src/pyanfis/algorithms/algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import torch
 
-from pyanfis.algorithms import LSTSQ, RLSE
+from .LSTSQ import LSTSQ
+from .RLSE import RLSE
 
 ALGORITHMS = {
     "LSTSQ": lambda n_vars: LSTSQ(n_vars),
     "RLSE":  lambda n_vars: RLSE(n_vars),
 }
 
 class TakagiSugenoAlgorithm(torch.nn.Module):
-    def __init__(self, n_vars, parameters_update,  algorithm="LSTSQ") -> None:
+    def __init__(self, n_vars, parameters_update,  algorithm="RLSE") -> None:
         super().__init__()
         self.name = algorithm
         self.parameters_update = parameters_update
 
         self.algorithm_name = algorithm
         if self.name not in ALGORITHMS:
             raise ValueError(f"Invalid algorithm name: {self.name}. Supported algorithms are {list(ALGORITHMS.keys())}")
@@ -24,8 +25,9 @@
         if self.parameters_update == "backward":
             self.theta = torch.nn.Parameter(torch.zeros((n_vars, 1), requires_grad=True))
         else:
             self.algorithm = ALGORITHMS[self.algorithm_name](n_vars)
 
     def forward(self, x, y=None):
         if self.parameters_update != "backward":
-            self.theta = self.algorithm(x.clone().detach(), y.clone().detach())
+            self.theta = self.algorithm(x.clone().detach(), y.clone().detach())
+            print(self.algorithm, self.theta)
```

### Comparing `pyanfis-0.1.5/src/pyanfis/consequents/types/lee.py` & `pyanfis-0.1.6/src/pyanfis/consequents/types/lee.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/consequents/types/takagi_sugeno.py` & `pyanfis-0.1.6/src/pyanfis/consequents/types/takagi_sugeno.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from .algorithm import TakagiSugenoAlgorithm 
+from pyanfis.algorithms import TakagiSugenoAlgorithm 
 
 
 class TakagiSugeno(torch.nn.Module):
     """
     This class will compute the learnable parameters using the Takagi-Sugeno approach.
 
     Attributes
@@ -37,10 +37,11 @@
         #output = {f"Output {i+1}": torch.zeros((x_b, x_i , 1)) for i in range(self.num_outputs)}
         outputs = torch.zeros(f.size(0), f.size(1), self.num_outputs)
         X = torch.einsum('bri, brj -> brij', f, X).view(x_b, x_i, -1)
 
         for i, (algorithm) in enumerate(self.universes.values()):
             if Y is not None:
                 algorithm(X, Y[:, :, i:i+1])
-            outputs[:, :, i:i+1] = outputs[:, :, i:i+1] + torch.einsum('bij, jk -> bik', X, algorithm.theta)
+
+            outputs[:, :, i:i+1] = outputs[:, :, i:i+1] + torch.einsum('bij, jk -> bik', X.float(), algorithm.theta.float())
    
         return outputs
```

### Comparing `pyanfis-0.1.5/src/pyanfis/consequents/types/tsukamoto.py` & `pyanfis-0.1.6/src/pyanfis/consequents/types/tsukamoto.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/functions/bell.py` & `pyanfis-0.1.6/src/pyanfis/functions/bell.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/functions/gauss.py` & `pyanfis-0.1.6/src/pyanfis/functions/gauss.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/functions/heaviside.py` & `pyanfis-0.1.6/src/pyanfis/functions/heaviside.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/functions/linear_s.py` & `pyanfis-0.1.6/src/pyanfis/functions/linear_s.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/functions/linear_z.py` & `pyanfis-0.1.6/src/pyanfis/functions/linear_z.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/functions/sigmoid.py` & `pyanfis-0.1.6/src/pyanfis/functions/sigmoid.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/functions/universe.py` & `pyanfis-0.1.6/src/pyanfis/functions/universe.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/rules/intersection_algorithms.py` & `pyanfis-0.1.6/src/pyanfis/rules/intersection_algorithms.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/rules/relation_algorithms.py` & `pyanfis-0.1.6/src/pyanfis/rules/relation_algorithms.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis/rules/rules.py` & `pyanfis-0.1.6/src/pyanfis/rules/rules.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.5/src/pyanfis.egg-info/SOURCES.txt` & `pyanfis-0.1.6/src/pyanfis.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 src/pyanfis.egg-info/PKG-INFO
 src/pyanfis.egg-info/SOURCES.txt
 src/pyanfis.egg-info/dependency_links.txt
 src/pyanfis.egg-info/top_level.txt
 src/pyanfis/algorithms/LSTSQ.py
 src/pyanfis/algorithms/RLSE.py
 src/pyanfis/algorithms/__init__.py
+src/pyanfis/algorithms/algorithm.py
 src/pyanfis/antecedents/__init__.py
 src/pyanfis/antecedents/antecedents.py
 src/pyanfis/consequents/__init__.py
 src/pyanfis/consequents/consequents.py
-src/pyanfis/consequents/types/algorithm.py
 src/pyanfis/consequents/types/lee.py
 src/pyanfis/consequents/types/takagi_sugeno.py
 src/pyanfis/consequents/types/tsukamoto.py
 src/pyanfis/functions/__init__.py
 src/pyanfis/functions/bell.py
 src/pyanfis/functions/gauss.py
 src/pyanfis/functions/heaviside.py
 src/pyanfis/functions/linear_s.py
 src/pyanfis/functions/linear_z.py
 src/pyanfis/functions/sigmoid.py
 src/pyanfis/functions/universe.py
 src/pyanfis/functions/utils.py
-src/pyanfis/optimizers/__init__.py
-src/pyanfis/optimizers/fuzzySGD.py
+src/pyanfis/pyplot/__init__.py
+src/pyanfis/pyplot/functions_plotting.py
+src/pyanfis/pyplot/structure_plotting.py
 src/pyanfis/rules/__init__.py
 src/pyanfis/rules/intersection_algorithms.py
 src/pyanfis/rules/relation_algorithms.py
 src/pyanfis/rules/rules.py
```

