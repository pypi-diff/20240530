# Comparing `tmp/resmda-0.0.3.tar.gz` & `tmp/resmda-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resmda-0.0.3.tar", last modified: Fri May 24 19:38:10 2024, max compression
+gzip compressed data, was "resmda-0.0.4.tar", last modified: Wed May 29 15:18:14 2024, max compression
```

## Comparing `resmda-0.0.3.tar` & `resmda-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:38:10.435236 resmda-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 19:38:03.000000 resmda-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-24 19:38:10.435236 resmda-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-24 19:38:03.000000 resmda-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:38:10.435236 resmda-0.0.3/resmda/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/data_assimilation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/reservoir_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:38:10.435236 resmda-0.0.3/resmda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:38:10.435236 resmda-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-24 19:38:03.000000 resmda-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:14.839341 resmda-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 15:18:01.000000 resmda-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-29 15:18:14.839341 resmda-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-29 15:18:01.000000 resmda-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:14.835342 resmda-0.0.4/resmda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/data_assimilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/reservoir_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-29 15:18:01.000000 resmda-0.0.4/resmda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:18:14.839341 resmda-0.0.4/resmda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 15:18:14.000000 resmda-0.0.4/resmda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:18:14.839341 resmda-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-29 15:18:01.000000 resmda-0.0.4/setup.py
```

### Comparing `resmda-0.0.3/LICENSE` & `resmda-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `resmda-0.0.3/PKG-INFO` & `resmda-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.0.3/README.rst` & `resmda-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `resmda-0.0.3/resmda/__init__.py` & `resmda-0.0.4/resmda/__init__.py`

 * *Files identical despite different names*

### Comparing `resmda-0.0.3/resmda/data_assimilation.py` & `resmda-0.0.4/resmda/data_assimilation.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 
 
 def __dir__():
     return __all__
 
 
 def esmda(model_prior, forward, data_obs, sigma, alphas=4, data_prior=None,
-          callback_post=None, return_post_data=False, random=None,
-          enable_localization=False, localization_matrix=None):
+          callback_post=None, return_post_data=True, return_steps=False,
+          random=None, enable_localization=False, localization_matrix=None):
     """ESMDA algorithm (Emerick and Reynolds, 2013) with optional localization.
 
+    ES-MDA as presented by [EmRe13]_.
+
 
     Parameters
     ----------
     model_prior : ndarray
         Prior models of dimension ``(ne, ...)``, where ``ne`` is the number of
         ensembles.
     forward : callable
@@ -47,16 +49,19 @@
         Standard deviation(s) of the observation noise.
     alphas : {int, ndarray}, default: 4
         Inflation factors for ES-MDA.
     data_prior : ndarray, default: None
         Prior data ensemble, of shape (ne, nd).
     callback_post : function, default: None
         Function to be executed after each ESMDA iteration.
-    return_post_data : bool, default: False
+    return_post_data : bool, default: True
         If true, returns data
+    return_steps : bool, default: False
+        If true, returns model (and data) of all ESMDA steps.
+        Setting ``return_steps`` to True wil enforce ``return_post_data``.
     random : {None, int,  np.random.Generator}, default: None
         Seed or random generator for reproducibility.
     enable_localization : bool, default: False
         If True, apply localization to the Kalman gain matrix.
     localization_matrix : ???, default: None
         Localization matrix.
 
@@ -84,15 +89,15 @@
         alphas = np.asarray(alphas)
 
     # Copy prior as start of post (output)
     model_post = model_prior.copy()
 
     # Loop over alphas
     for i, alpha in enumerate(alphas):
-        print(f"ESMDA step {i+1}; α={alpha}")
+        print(f"ESMDA step {i+1: 3d}; α={alpha}")
 
         # == Step (a) of Emerick & Reynolds, 2013 ==
         # Run the ensemble from time zero.
 
         # Get data
         if i > 0 or data_prior is None:
             data_prior = forward(model_post)
@@ -138,16 +143,30 @@
         # Update the ensemble parameters
         model_post += np.moveaxis(K @ (data_pert - data_prior).T, -1, 0)
 
         # Apply model parameter bounds.
         if callback_post:
             callback_post(model_post)
 
-    # Return posterior model and corresponding data
-    return model_post, forward(model_post)
+        if return_steps:
+            if i == 0:
+                all_models = np.zeros((alphas.size+1, *model_post.shape))
+                all_models[0, ...] = model_prior
+                all_data = np.zeros((alphas.size+1, *data_prior.shape))
+            all_models[i+1, ...] = model_post.copy()
+            all_data[i, ...] = data_prior
+
+    # Return posterior model and corresponding data (if wanted)
+    if return_steps:
+        all_data[-1, ...] = forward(model_post)
+        return all_models, all_data
+    elif return_post_data:
+        return model_post, forward(model_post)
+    else:
+        return model_post
 
 
 def convert_positions_to_indices(positions, grid_dimensions):
     """Convert 2D grid positions to 1D indices assuming zero-indexed positions.
 
     Parameters
     ----------
```

### Comparing `resmda-0.0.3/resmda/reservoir_simulator.py` & `resmda-0.0.4/resmda/reservoir_simulator.py`

 * *Files identical despite different names*

### Comparing `resmda-0.0.3/resmda/utils.py` & `resmda-0.0.4/resmda/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,14 @@
 __all__ = ['Report', 'rng']
 
 
 def __dir__():
     return __all__
 
 
-# Instantiate a random number generator ONCE
-RANDOM_NUMBER_GENERATOR = np.random.default_rng()
-
-
 def rng(random=None):
     """Module-wide Random Number Generator.
 
     Mainly meant for internal use.
 
 
     Parameters
@@ -61,15 +57,17 @@
 
     """
     if isinstance(random, int):
         return np.random.default_rng(random)
     elif isinstance(random, np.random.Generator):
         return random
     else:
-        return RANDOM_NUMBER_GENERATOR
+        if not hasattr(rng, '_rng'):
+            rng._rng = np.random.default_rng()
+        return rng._rng
 
 
 class Report(ScoobyReport):
     """Print a Scooby report; see ``scooby.Report()`` for info."""
 
     def __init__(self, **kwargs):
         """Initiate a scooby.Report instance."""
```

### Comparing `resmda-0.0.3/resmda.egg-info/PKG-INFO` & `resmda-0.0.4/resmda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.0.3/setup.py` & `resmda-0.0.4/setup.py`

 * *Files identical despite different names*

