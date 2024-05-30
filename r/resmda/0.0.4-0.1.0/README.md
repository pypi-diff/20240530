# Comparing `tmp/resmda-0.0.4.tar.gz` & `tmp/resmda-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resmda-0.0.4.tar", last modified: Wed May 29 15:18:14 2024, max compression
+gzip compressed data, was "resmda-0.1.0.tar", last modified: Thu May 30 07:25:44 2024, max compression
```

## Comparing `resmda-0.0.4.tar` & `resmda-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:14.839341 resmda-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 15:18:01.000000 resmda-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-29 15:18:14.839341 resmda-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-29 15:18:01.000000 resmda-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:14.835342 resmda-0.0.4/resmda/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/data_assimilation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/reservoir_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:14.839341 resmda-0.0.4/resmda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:18:14.839341 resmda-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-29 15:18:01.000000 resmda-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:25:44.268974 resmda-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 07:25:35.000000 resmda-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 07:25:44.268974 resmda-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-30 07:25:35.000000 resmda-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:25:44.268974 resmda-0.1.0/resmda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 07:25:35.000000 resmda-0.1.0/resmda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-30 07:25:35.000000 resmda-0.1.0/resmda/data_assimilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-30 07:25:35.000000 resmda-0.1.0/resmda/reservoir_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-30 07:25:35.000000 resmda-0.1.0/resmda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 07:25:44.000000 resmda-0.1.0/resmda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:25:44.268974 resmda-0.1.0/resmda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 07:25:44.000000 resmda-0.1.0/resmda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-30 07:25:44.000000 resmda-0.1.0/resmda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:25:44.000000 resmda-0.1.0/resmda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 07:25:44.000000 resmda-0.1.0/resmda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 07:25:44.000000 resmda-0.1.0/resmda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:25:44.268974 resmda-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-30 07:25:35.000000 resmda-0.1.0/setup.py
```

### Comparing `resmda-0.0.4/LICENSE` & `resmda-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resmda-0.0.4/PKG-INFO` & `resmda-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.0.4
+Version: 0.1.0
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.0.4/README.rst` & `resmda-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `resmda-0.0.4/resmda/__init__.py` & `resmda-0.1.0/resmda/__init__.py`

 * *Files identical despite different names*

### Comparing `resmda-0.0.4/resmda/data_assimilation.py` & `resmda-0.1.0/resmda/data_assimilation.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def __dir__():
     return __all__
 
 
 def esmda(model_prior, forward, data_obs, sigma, alphas=4, data_prior=None,
           callback_post=None, return_post_data=True, return_steps=False,
-          random=None, enable_localization=False, localization_matrix=None):
+          random=None, localization_matrix=None):
     """ESMDA algorithm (Emerick and Reynolds, 2013) with optional localization.
 
     ES-MDA as presented by [EmRe13]_.
 
 
     Parameters
     ----------
@@ -56,18 +56,16 @@
     return_post_data : bool, default: True
         If true, returns data
     return_steps : bool, default: False
         If true, returns model (and data) of all ESMDA steps.
         Setting ``return_steps`` to True wil enforce ``return_post_data``.
     random : {None, int,  np.random.Generator}, default: None
         Seed or random generator for reproducibility.
-    enable_localization : bool, default: False
-        If True, apply localization to the Kalman gain matrix.
-    localization_matrix : ???, default: None
-        Localization matrix.
+    localization_matrix : {ndarray, None}, default: None
+        If provided, apply localization to the Kalman gain matrix.
 
 
     Returns
     -------
     model_post : ndarray
         Posterior model ensemble.
     data_post : ndarray, only returned if ``return_post_data=True``
@@ -128,43 +126,46 @@
         # - a subspace inversions with Woodbury matrix identity, or
         # - Moore-Penrose via np.linalg.pinv, sp.linalg.pinv, spp.linalg.pinvh.
         Cinv = np.linalg.inv(CDD + CD)
 
         # Calculate the Kalman gain
         K = CMD@Cinv
 
-        # TODO: Implement localization
-        if enable_localization and localization_matrix is not None:
-            localization_matrix = localization_matrix
-            K = K.reshape(-1, nd)
-            K = K * localization_matrix
-            # Reshape back to original shape
-            K = K.reshape(model_prior.shape[1], model_prior.shape[2], nd)
+        # Apply localization if provided
+        if localization_matrix is not None:
+            K *= localization_matrix[..., None]
 
         # Update the ensemble parameters
         model_post += np.moveaxis(K @ (data_pert - data_prior).T, -1, 0)
 
-        # Apply model parameter bounds.
+        # Apply any provided post-checks
         if callback_post:
             callback_post(model_post)
 
+        # If intermediate steps are wanted, store results
         if return_steps:
+            # Initiate output if first iteration
             if i == 0:
                 all_models = np.zeros((alphas.size+1, *model_post.shape))
                 all_models[0, ...] = model_prior
                 all_data = np.zeros((alphas.size+1, *data_prior.shape))
-            all_models[i+1, ...] = model_post.copy()
+            all_models[i+1, ...] = model_post
             all_data[i, ...] = data_prior
 
+    # Compute posterior data if wanted
+    if return_post_data or return_steps:
+        data_post = forward(model_post)
+        if return_steps:
+            all_data[-1, ...] = forward(model_post)
+
     # Return posterior model and corresponding data (if wanted)
     if return_steps:
-        all_data[-1, ...] = forward(model_post)
         return all_models, all_data
     elif return_post_data:
-        return model_post, forward(model_post)
+        return model_post, data_post
     else:
         return model_post
 
 
 def convert_positions_to_indices(positions, grid_dimensions):
     """Convert 2D grid positions to 1D indices assuming zero-indexed positions.
```

### Comparing `resmda-0.0.4/resmda/reservoir_simulator.py` & `resmda-0.1.0/resmda/reservoir_simulator.py`

 * *Files identical despite different names*

### Comparing `resmda-0.0.4/resmda/utils.py` & `resmda-0.1.0/resmda/utils.py`

 * *Files identical despite different names*

### Comparing `resmda-0.0.4/resmda.egg-info/PKG-INFO` & `resmda-0.1.0/resmda.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.0.4
+Version: 0.1.0
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.0.4/setup.py` & `resmda-0.1.0/setup.py`

 * *Files identical despite different names*

