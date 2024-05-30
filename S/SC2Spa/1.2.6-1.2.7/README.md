# Comparing `tmp/sc2spa-1.2.6.tar.gz` & `tmp/sc2spa-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc2spa-1.2.6.tar", last modified: Tue May 28 20:59:56 2024, max compression
+gzip compressed data, was "sc2spa-1.2.7.tar", last modified: Thu May 30 03:32:05 2024, max compression
```

## Comparing `sc2spa-1.2.6.tar` & `sc2spa-1.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 20:59:56.673950 sc2spa-1.2.6/
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1525 2024-05-28 00:26:30.000000 sc2spa-1.2.6/LICENSE
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 20:59:56.673950 sc2spa-1.2.6/PKG-INFO
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1229 2024-05-28 00:26:30.000000 sc2spa-1.2.6/README.md
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 20:59:56.673950 sc2spa-1.2.6/SC2Spa/
--rw-r--r--   0 linbu     (1000) linbu     (1000)      211 2024-05-28 00:26:30.000000 sc2spa-1.2.6/SC2Spa/__init__.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)      461 2024-05-28 20:59:26.000000 sc2spa-1.2.6/SC2Spa/__metadata__.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)    20205 2024-05-28 00:26:30.000000 sc2spa-1.2.6/SC2Spa/bm.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     8248 2024-05-28 00:26:30.000000 sc2spa-1.2.6/SC2Spa/me.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)    23478 2024-05-28 00:26:30.000000 sc2spa-1.2.6/SC2Spa/pl.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     3062 2024-05-28 00:26:30.000000 sc2spa-1.2.6/SC2Spa/pp.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     4381 2024-05-28 00:26:30.000000 sc2spa-1.2.6/SC2Spa/sva.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)    51773 2024-05-28 20:59:10.000000 sc2spa-1.2.6/SC2Spa/tl.py
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 20:59:56.673950 sc2spa-1.2.6/SC2Spa.egg-info/
--rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-28 20:59:56.000000 sc2spa-1.2.6/SC2Spa.egg-info/PKG-INFO
--rw-r--r--   0 linbu     (1000) linbu     (1000)      317 2024-05-28 20:59:56.000000 sc2spa-1.2.6/SC2Spa.egg-info/SOURCES.txt
--rw-r--r--   0 linbu     (1000) linbu     (1000)        1 2024-05-28 20:59:56.000000 sc2spa-1.2.6/SC2Spa.egg-info/dependency_links.txt
--rw-r--r--   0 linbu     (1000) linbu     (1000)        7 2024-05-28 20:59:56.000000 sc2spa-1.2.6/SC2Spa.egg-info/top_level.txt
--rw-r--r--   0 linbu     (1000) linbu     (1000)      691 2024-05-28 20:59:41.000000 sc2spa-1.2.6/pyproject.toml
--rw-r--r--   0 linbu     (1000) linbu     (1000)       38 2024-05-28 20:59:56.673950 sc2spa-1.2.6/setup.cfg
-drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-28 20:59:56.673950 sc2spa-1.2.6/tests/
--rw-r--r--   0 linbu     (1000) linbu     (1000)     3122 2024-05-28 00:26:31.000000 sc2spa-1.2.6/tests/test_loading.py
--rw-r--r--   0 linbu     (1000) linbu     (1000)     3545 2024-05-28 00:26:31.000000 sc2spa-1.2.6/tests/test_mapping.py
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-30 03:32:05.393992 sc2spa-1.2.7/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1525 2024-05-28 00:26:30.000000 sc2spa-1.2.7/LICENSE
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-30 03:32:05.393992 sc2spa-1.2.7/PKG-INFO
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1229 2024-05-28 00:26:30.000000 sc2spa-1.2.7/README.md
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-30 03:32:05.393992 sc2spa-1.2.7/SC2Spa/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      211 2024-05-28 00:26:30.000000 sc2spa-1.2.7/SC2Spa/__init__.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      461 2024-05-30 03:31:33.000000 sc2spa-1.2.7/SC2Spa/__metadata__.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    20205 2024-05-28 00:26:30.000000 sc2spa-1.2.7/SC2Spa/bm.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     8248 2024-05-28 00:26:30.000000 sc2spa-1.2.7/SC2Spa/me.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    23478 2024-05-28 00:26:30.000000 sc2spa-1.2.7/SC2Spa/pl.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3062 2024-05-28 00:26:30.000000 sc2spa-1.2.7/SC2Spa/pp.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     4381 2024-05-28 00:26:30.000000 sc2spa-1.2.7/SC2Spa/sva.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)    46553 2024-05-30 03:30:35.000000 sc2spa-1.2.7/SC2Spa/tl.py
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-30 03:32:05.393992 sc2spa-1.2.7/SC2Spa.egg-info/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     1773 2024-05-30 03:32:05.000000 sc2spa-1.2.7/SC2Spa.egg-info/PKG-INFO
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      317 2024-05-30 03:32:05.000000 sc2spa-1.2.7/SC2Spa.egg-info/SOURCES.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)        1 2024-05-30 03:32:05.000000 sc2spa-1.2.7/SC2Spa.egg-info/dependency_links.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)        7 2024-05-30 03:32:05.000000 sc2spa-1.2.7/SC2Spa.egg-info/top_level.txt
+-rw-r--r--   0 linbu     (1000) linbu     (1000)      691 2024-05-30 03:31:47.000000 sc2spa-1.2.7/pyproject.toml
+-rw-r--r--   0 linbu     (1000) linbu     (1000)       38 2024-05-30 03:32:05.393992 sc2spa-1.2.7/setup.cfg
+drwxr-xr-x   0 linbu     (1000) linbu     (1000)        0 2024-05-30 03:32:05.393992 sc2spa-1.2.7/tests/
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3122 2024-05-28 00:26:31.000000 sc2spa-1.2.7/tests/test_loading.py
+-rw-r--r--   0 linbu     (1000) linbu     (1000)     3545 2024-05-28 00:26:31.000000 sc2spa-1.2.7/tests/test_mapping.py
```

### Comparing `sc2spa-1.2.6/LICENSE` & `sc2spa-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/PKG-INFO` & `sc2spa-1.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.6
+Version: 1.2.7
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `sc2spa-1.2.6/README.md` & `sc2spa-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/SC2Spa/bm.py` & `sc2spa-1.2.7/SC2Spa/bm.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/SC2Spa/me.py` & `sc2spa-1.2.7/SC2Spa/me.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/SC2Spa/pl.py` & `sc2spa-1.2.7/SC2Spa/pl.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/SC2Spa/pp.py` & `sc2spa-1.2.7/SC2Spa/pp.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/SC2Spa/sva.py` & `sc2spa-1.2.7/SC2Spa/sva.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/SC2Spa/tl.py` & `sc2spa-1.2.7/SC2Spa/tl.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             if shuffle:
                 np.random.shuffle(sample_index)
             counter = 0
 
 def CrossValidation(X: np.array, Y: np.array, train_indices, test_indices,
                     l1_reg = 1e-5, l2_reg = 0, dropout = 0.05, lrr_patience = 20,
                     ES_patience = 50, min_lr = 1e-9,
-                    epoch = 20, batch_size = 4096,
+                    epoch = 20, batch_size = 4096, loss = rmse, loss_name = 'rmse',
                     nodes = [4096, 1024, 256, 64, 16, 4], seed = None):
     '''
     Perform Cross-validation using fully connected neural network
 
     Parameters
     ----------
     X
@@ -464,149 +464,14 @@
         Y = pp.MinMaxNorm(RTheta_ref, RTheta_ref)
     else:
         Y = pp.MinMaxNorm(Y_ref, Y_ref)
         RTheta_ref = None
 
     return X, Y, Y_ref, RTheta_ref
 
-def Self_Mapping(adata: anndata.AnnData, sparse = True, model_path = None,
-            root = 'Model_SI/', name = 'SI_Overall', l1_reg = 1e-5, l2_reg = 0, dropout = 0.05, epoch = 500,
-            batch_size = 4096, nodes = [4096, 1024, 256, 64, 16, 4], lrr_patience = 20, ES_patience = 50,
-            min_lr = 1e-5, save = False, polar = True, seed = None):
-
-    '''
-    Map ST beads to spatial locations. A fully connected neural network trained on all
-    all ST beads will be applied to the same set of beads. A model will be trained and
-    saved to `root+name+'.h5'` if model_path is None and save is True.
-    The predicted coordinates will be saved in adata.obsm['spatial_self_mapping']
-
-    Parameters
-    ----------
-    adata
-        Reference anndata object. Gene expression matrix should be the shape of (cell, gene).
-        Spatial information should be stored in adata_ref.obsm['spatial'] in `np.array` format
-    model_path
-        The path of a trained model. If not None, parameters for training will be ignored.
-    root
-        the root path to save the model
-    name
-        the name used to save the model
-    l1_reg
-        l1 regularization factor
-    l2_reg
-        l2 regularization factor
-    nodes
-        a list that contains the numbers of the nodes of hidden layers
-    lrr_patience
-        The patience for learning rate reduction
-    min_lr
-        minimum learning rate
-    ES_patience
-        The patience for early stopping
-
-    Returns
-    -------
-    model
-        a trained fully connected neural network
-
-    '''
-
-    #Extract values
-    X, Y, Y_ref, RTheta_ref = ExtractXY(adata=adata, sparse = sparse, polar=polar)
-
-    if(model_path != None):
-        model = load_model(model_path, compile=False)
-    else:
-        model = Train(X=X, Y=Y, root = root, name = name, l1_reg = l1_reg,
-                      l2_reg = l2_reg, dropout = dropout, epoch = epoch,
-                      batch_size = batch_size, nodes = nodes, lrr_patience = lrr_patience,
-                      ES_patience = ES_patience, min_lr = min_lr, save = save, seed = seed)
-    Ref_pred_Y = BatchPredict(model, X)
-    if(polar):
-        Ref_pred_Y = pp.RePolarTrans(pp.ReMMNorm(RTheta_ref, Ref_pred_Y))
-    else:
-        Ref_pred_Y = pp.ReMMNorm(Y_ref, Ref_pred_Y)
-
-    #Write prediction into adata
-    adata.obsm['spatial_mapping'] = Ref_pred_Y
-
-    return model
-
-def Mapping(adata_ref, adata_query, sparse = True, model_path = None, WD_cutoff = None,
-            root = 'Model_SI/', name = 'SI', l1_reg = 1e-5, l2_reg = 0, dropout = 0.05, epoch = 500,
-            batch_size = 4096, nodes = [4096, 1024, 256, 64, 16, 4], lrr_patience = 20, ES_patience = 50,
-            min_lr = 1e-5, save = False, polar = True, seed = None):
-
-    '''
-    Map single cells to spatial locations.
-    A model will be trained and saved to `root+name+'.h5'` if model_path is None and save is True.
-    The predicted coordinates will be saved in adata_query.obsm['spatial_mapping']
-
-    Parameters
-    ----------
-    adata_ref
-        Reference anndata object. Gene expression matrix should be the shape of (cell, gene).
-        Spatial information should be stored in adata_ref.obsm['spatial'] in `np.array` format
-    adata_query
-        Query anndata object. Gene expression matrix should be the shape of (cell, gene).
-    sparse
-        if gene expression is saved in sparse format
-    model_path
-        The path of a trained model. If not None, parameters for training will be ignored.
-    WD_cutoff
-        genes with Wasserstein distance lower than the cutoff will be used for mapping
-    root
-        the root path to save the model
-    name
-        the name used to save the model
-    l1_reg
-        l1 regularization factor
-    l2_reg
-        l2 regularization factor
-    nodes
-        a list that contains the numbers of the nodes of hidden layers
-    lrr_patience
-        The patience for learning rate reduction
-    min_lr
-        minimum learning rate
-    ES_patience
-        The patience for early stopping
-
-    Returns
-    -------
-    None
-
-    '''
-
-    #Extract values
-    X_ref, X_query, Y_ref = pp_Mapping(adata_ref, adata_query,
-                                       sparse = sparse, WD_cutoff = WD_cutoff)
-
-    if(polar):
-        RTheta_ref = pp.PolarTrans(Y_ref)
-        Y = pp.MinMaxNorm(RTheta_ref, RTheta_ref)
-    else:
-        Y = pp.MinMaxNorm(Y_ref, Y_ref)
-
-    if(model_path != None):
-        model = load_model(model_path, compile=False)
-    else:
-        model = Train(X=X_ref, Y=Y, root = root, name = name, l1_reg = l1_reg,
-                      l2_reg = l2_reg, dropout = dropout, epoch = epoch,
-                      batch_size = batch_size, nodes = nodes, lrr_patience = lrr_patience,
-                      ES_patience = ES_patience, min_lr = min_lr, save = save, seed = seed)
-    Query_pred_Y = BatchPredict(model, X_query)
-    if(polar):
-        Query_pred_Y = pp.RePolarTrans(pp.ReMMNorm(RTheta_ref, Query_pred_Y))
-    else:
-        Query_pred_Y = pp.ReMMNorm(Y_ref, Query_pred_Y)
-
-    #Write prediction into adata
-    adata_query.obsm['spatial_mapping'] = Query_pred_Y
-
 
 def Reconstruct_scST(adata_ref, adata_query, n_neighbors=1000,
                      dis_cutoff=15, n_layer_cell= [1, 4], cell_radius=5,
                      seed=2023):
     '''
     Reconstruct ST data at single cell resolution
 
@@ -736,17 +601,16 @@
 
         adata_query.obs.loc[temp, 'Recon_scST'] = True
         adata_query.obs.loc[temp, 'Recon_scST_layer'] = layer
 
 def FineMapping(adata_ref, adata_query, sparse = True, model_path = None, WD_cutoff = None, JGs = None,
                 root = 'Model_SI/', name = 'SI', l1_reg = 1e-5, l2_reg = 0, dropout = 0.05, epoch = 500,
                 batch_size = 4096, nodes = [4096, 1024, 256, 64, 16, 4], lrr_patience = 20, ES_patience = 50,
-                min_lr = 1e-5, save = True, loss = 'mse', loss_name = 'mse', NormMethod = 'BN', polar = True, FM = True,
-                n_layer_cell = [1, 4],
-                cell_radius = 5, n_neighbors = 1000, dis_cutoff = 15, seed = 2023):
+                min_lr = 1e-5, save = True, loss = rmse, loss_name = 'rmse', NormMethod = 'BN', polar = True, FM = True,
+                n_layer_cell = [1, 4], cell_radius = 5, n_neighbors = 1000, dis_cutoff = 15, seed = 2023):
 
     '''
     Finely map single cells to spatial locations and Reconstruct ST data at single cell resolution
 
     1. Finely map single cells to spatial locations.
     A model will be trained and saved to `root+name+'.h5'` if model_path is None and save is True.
     The predicted coordinates of single cells will be saved in adata_query.obsm['spatial_mapping']
```

### Comparing `sc2spa-1.2.6/SC2Spa.egg-info/PKG-INFO` & `sc2spa-1.2.7/SC2Spa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.2.6
+Version: 1.2.7
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `sc2spa-1.2.6/pyproject.toml` & `sc2spa-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sc2spa-1.2.6/tests/test_loading.py` & `sc2spa-1.2.7/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `sc2spa-1.2.6/tests/test_mapping.py` & `sc2spa-1.2.7/tests/test_mapping.py`

 * *Files identical despite different names*

