# Comparing `tmp/cellarium_ml-0.0.5.tar.gz` & `tmp/cellarium_ml-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellarium_ml-0.0.5.tar", last modified: Tue May 21 15:11:38 2024, max compression
+gzip compressed data, was "cellarium_ml-0.0.7.tar", last modified: Thu May 30 14:57:08 2024, max compression
```

## Comparing `cellarium_ml-0.0.5.tar` & `cellarium_ml-0.0.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.774249 cellarium_ml-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-21 15:11:38.774249 cellarium_ml-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.758249 cellarium_ml-0.0.5/cellarium/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/callbacks/prediction_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/callbacks/variance_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20755 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/core/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/core/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/data/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/dadc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/distributed_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/data/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.762250 cellarium_ml-0.0.5/cellarium/ml/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributed/gather.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/distributions/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/distributions/negative_binomial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/linear_lr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/geneformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/incremental_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/mu_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/onepass_mean_var_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/probabilistic_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/models/tdigest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/preprocessing/highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.766250 cellarium_ml-0.0.5/cellarium/ml/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/divide_by_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/log1p.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/normalize_total.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/transforms/z_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.770249 cellarium_ml-0.0.5/cellarium/ml/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/cellarium/ml/utilities/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.770249 cellarium_ml-0.0.5/cellarium_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 15:11:38.000000 cellarium_ml-0.0.5/cellarium_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:11:38.774249 cellarium_ml-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:11:38.770249 cellarium_ml-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_distributed_anndata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_geneformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_ipca.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_mup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_onepass_mean_var_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_ppca.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_read_h5ad.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_tdigest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-21 15:11:34.000000 cellarium_ml-0.0.5/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.744487 cellarium_ml-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-30 14:57:08.744487 cellarium_ml-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.728487 cellarium_ml-0.0.7/cellarium/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.732487 cellarium_ml-0.0.7/cellarium/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.732487 cellarium_ml-0.0.7/cellarium/ml/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/callbacks/prediction_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/callbacks/variance_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20755 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.732487 cellarium_ml-0.0.7/cellarium/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/core/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/core/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.732487 cellarium_ml-0.0.7/cellarium/ml/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18136 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/data/dadc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/data/distributed_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/data/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/data/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.736487 cellarium_ml-0.0.7/cellarium/ml/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/distributed/gather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.736487 cellarium_ml-0.0.7/cellarium/ml/distributions/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/distributions/negative_binomial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.736487 cellarium_ml-0.0.7/cellarium/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/lr_schedulers/linear_lr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.736487 cellarium_ml-0.0.7/cellarium/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/geneformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/incremental_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/mu_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/onepass_mean_var_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8375 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/probabilistic_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/models/tdigest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.736487 cellarium_ml-0.0.7/cellarium/ml/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/preprocessing/highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.736487 cellarium_ml-0.0.7/cellarium/ml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/transforms/divide_by_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/transforms/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/transforms/log1p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/transforms/normalize_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/transforms/z_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.740487 cellarium_ml-0.0.7/cellarium/ml/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/utilities/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/cellarium/ml/utilities/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.744487 cellarium_ml-0.0.7/cellarium_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-30 14:57:08.000000 cellarium_ml-0.0.7/cellarium_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-30 14:57:08.000000 cellarium_ml-0.0.7/cellarium_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:57:08.000000 cellarium_ml-0.0.7/cellarium_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 14:57:08.000000 cellarium_ml-0.0.7/cellarium_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 14:57:08.000000 cellarium_ml-0.0.7/cellarium_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 14:57:08.000000 cellarium_ml-0.0.7/cellarium_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:57:08.744487 cellarium_ml-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:57:08.744487 cellarium_ml-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_distributed_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_geneformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_ipca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_mup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_onepass_mean_var_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_ppca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_read_h5ad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_tdigest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 14:57:02.000000 cellarium_ml-0.0.7/tests/test_transforms.py
```

### Comparing `cellarium_ml-0.0.5/LICENSE.md` & `cellarium_ml-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/PKG-INFO` & `cellarium_ml-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellarium-ml
-Version: 0.0.5
+Version: 0.0.7
 Summary: Machine learning library for single-cell data analysis
 Author-email: Yerdos Ordabayev <yordabay@broadinstitute.org>, Mehrtash Babadi <mehrtash@broadinstitute.org>
 License: Copyright (c) 2023, Broad Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -43,15 +43,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 Requires-Dist: anndata
 Requires-Dist: boltons
 Requires-Dist: braceexpand
 Requires-Dist: crick>=0.0.4
 Requires-Dist: google-cloud-storage
-Requires-Dist: jsonargparse[signatures]
+Requires-Dist: jsonargparse[signatures]==4.27.7
 Requires-Dist: lightning>=2.2.0
 Requires-Dist: pyro-ppl
 Requires-Dist: pytest
 Requires-Dist: torch>=2.2.0
 Requires-Dist: transformers
 Provides-Extra: lint
 Requires-Dist: ruff; extra == "lint"
```

### Comparing `cellarium_ml-0.0.5/README.rst` & `cellarium_ml-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/callbacks/prediction_writer.py` & `cellarium_ml-0.0.7/cellarium/ml/callbacks/prediction_writer.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/callbacks/variance_monitor.py` & `cellarium_ml-0.0.7/cellarium/ml/callbacks/variance_monitor.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/cli.py` & `cellarium_ml-0.0.7/cellarium/ml/cli.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/core/datamodule.py` & `cellarium_ml-0.0.7/cellarium/ml/core/datamodule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 
+from typing import Literal
+
 import lightning.pytorch as pl
 import torch
 from anndata import AnnData
 
 from cellarium.ml.data import DistributedAnnDataCollection, IterableDistributedAnnDataCollectionDataset
 from cellarium.ml.utilities.core import train_val_split
 from cellarium.ml.utilities.data import AnnDataField, collate_fn
@@ -28,14 +30,15 @@
         ...     ),
         ...     max_cache_size=2,
         ...     batch_keys={
         ...         "x_ng": AnnDataField(attr="X", convert_fn=densify),
         ...         "var_names_g": AnnDataField(attr="var_names"),
         ...     },
         ...     batch_size=5000,
+        ...     iteration_strategy="cache_efficient",
         ...     shuffle=True,
         ...     seed=0,
         ...     drop_last=True,
         ...     num_workers=4,
         ... )
         >>> dm.setup()
         >>> for batch in dm.train_dataloader():
@@ -47,14 +50,18 @@
         batch_keys:
             Dictionary that specifies which attributes and keys of the :attr:`dadc` to return
             in the batch data and how to convert them. Keys must correspond to
             the input keys of the transforms or the model. Values must be instances of
             :class:`cellarium.ml.utilities.data.AnnDataField`.
         batch_size:
             How many samples per batch to load.
+        iteration_strategy:
+            Strategy to use for iterating through the dataset. Options are ``same_order`` and ``cache_efficient``.
+            ``same_order`` will iterate through the dataset in the same order independent of the number of replicas
+            and workers. ``cache_efficient`` will try to minimize the amount of anndata files fetched by each worker.
         shuffle:
             If ``True``, the data is reshuffled at every epoch.
         seed:
             Random seed used to shuffle the sampler if :attr:`shuffle=True`.
         drop_last:
             If ``True``, then the sampler will drop the tail of the data
             to make it evenly divisible across the number of replicas. If ``False``,
@@ -78,14 +85,15 @@
 
     def __init__(
         self,
         dadc: DistributedAnnDataCollection | AnnData,
         # IterableDistributedAnnDataCollectionDataset args
         batch_keys: dict[str, AnnDataField] | None = None,
         batch_size: int = 1,
+        iteration_strategy: Literal["same_order", "cache_efficient"] = "cache_efficient",
         shuffle: bool = False,
         seed: int = 0,
         drop_last: bool = False,
         train_size: float | int | None = None,
         val_size: float | int | None = None,
         test_mode: bool = False,
         # DataLoader args
@@ -96,60 +104,64 @@
         # Don't save dadc to the checkpoint
         self.hparams["dadc"] = None
 
         self.dadc = dadc
         # IterableDistributedAnnDataCollectionDataset args
         self.batch_keys = batch_keys or {}
         self.batch_size = batch_size
+        self.iteration_strategy = iteration_strategy
         self.shuffle = shuffle
         self.seed = seed
         self.drop_last = drop_last
         self.n_train, self.n_val = train_val_split(len(dadc), train_size, val_size)
         self.test_mode = test_mode
         # DataLoader args
         self.num_workers = num_workers
 
     def setup(self, stage: str | None = None) -> None:
         """
         .. note::
            setup is called from every process across all the nodes. Setting state here is recommended.
 
         .. note::
-            :attr:`val_dataset` is not shuffled.
+            :attr:`val_dataset` is not shuffled and uses the ``same_order`` iteration strategy.
 
         """
         if stage == "fit":
             self.train_dataset = IterableDistributedAnnDataCollectionDataset(
                 dadc=self.dadc,
                 batch_keys=self.batch_keys,
                 batch_size=self.batch_size,
+                iteration_strategy=self.iteration_strategy,
                 shuffle=self.shuffle,
                 seed=self.seed,
                 drop_last=self.drop_last,
                 test_mode=self.test_mode,
                 start_idx=0,
                 end_idx=self.n_train,
             )
             self.val_dataset = IterableDistributedAnnDataCollectionDataset(
                 dadc=self.dadc,
                 batch_keys=self.batch_keys,
                 batch_size=self.batch_size,
+                iteration_strategy="same_order",
                 shuffle=False,
                 seed=self.seed,
                 drop_last=False,
                 test_mode=self.test_mode,
                 start_idx=self.n_train,
                 end_idx=self.n_train + self.n_val,
             )
 
         if stage == "predict":
             self.predict_dataset = IterableDistributedAnnDataCollectionDataset(
                 dadc=self.dadc,
                 batch_keys=self.batch_keys,
                 batch_size=self.batch_size,
+                iteration_strategy=self.iteration_strategy,
                 shuffle=self.shuffle,
                 seed=self.seed,
                 drop_last=self.drop_last,
                 test_mode=self.test_mode,
             )
 
     def train_dataloader(self) -> torch.utils.data.DataLoader:
```

### Comparing `cellarium_ml-0.0.5/cellarium/ml/core/module.py` & `cellarium_ml-0.0.7/cellarium/ml/core/module.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/core/pipeline.py` & `cellarium_ml-0.0.7/cellarium/ml/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/data/__init__.py` & `cellarium_ml-0.0.7/cellarium/ml/data/__init__.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/data/distributed_anndata.py` & `cellarium_ml-0.0.7/cellarium/ml/data/distributed_anndata.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/data/fileio.py` & `cellarium_ml-0.0.7/cellarium/ml/data/fileio.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/data/schema.py` & `cellarium_ml-0.0.7/cellarium/ml/data/schema.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/distributed/gather.py` & `cellarium_ml-0.0.7/cellarium/ml/distributed/gather.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/distributions/negative_binomial.py` & `cellarium_ml-0.0.7/cellarium/ml/distributions/negative_binomial.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/lr_schedulers/linear_lr.py` & `cellarium_ml-0.0.7/cellarium/ml/lr_schedulers/linear_lr.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/__init__.py` & `cellarium_ml-0.0.7/cellarium/ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/geneformer.py` & `cellarium_ml-0.0.7/cellarium/ml/models/geneformer.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/incremental_pca.py` & `cellarium_ml-0.0.7/cellarium/ml/models/incremental_pca.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/logistic_regression.py` & `cellarium_ml-0.0.7/cellarium/ml/models/logistic_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,16 @@
 
         # loss
         self.elbo = pyro.infer.Trace_ELBO()
 
         self.log_metrics = log_metrics
 
     def reset_parameters(self) -> None:
-        rng = torch.Generator()
+        rng_device = self.W_gc.device.type if self.W_gc.device.type != "meta" else "cpu"
+        rng = torch.Generator(device=rng_device)
         rng.manual_seed(self.seed)
         self.W_prior_scale.fill_(self._W_prior_scale)
         self.W_gc.data.normal_(0, self.W_init_scale, generator=rng)
         self.b_c.data.zero_()
 
     def forward(self, x_ng: torch.Tensor, var_names_g: np.ndarray, y_n: torch.Tensor) -> dict[str, torch.Tensor | None]:
         """
```

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/model.py` & `cellarium_ml-0.0.7/cellarium/ml/models/model.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/mu_linear.py` & `cellarium_ml-0.0.7/cellarium/ml/models/mu_linear.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/onepass_mean_var_std.py` & `cellarium_ml-0.0.7/cellarium/ml/models/onepass_mean_var_std.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/probabilistic_pca.py` & `cellarium_ml-0.0.7/cellarium/ml/models/probabilistic_pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,16 @@
         self.W_init_scale = W_init_scale
         self.sigma_init_scale = sigma_init_scale
         self.W_kg = torch.nn.Parameter(torch.empty(n_components, n_vars))
         self.sigma = PyroParam(torch.empty(()), constraint=constraints.positive)  # type: ignore[call-arg]
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
-        rng = torch.Generator()
+        rng_device = self.W_kg.device.type if self.W_kg.device.type != "meta" else "cpu"
+        rng = torch.Generator(device=rng_device)
         rng.manual_seed(self.seed)
         if isinstance(self.mean_g, torch.nn.Parameter):
             self.mean_g.data.zero_()
         self.W_kg.data.normal_(0, self.W_init_scale, generator=rng)
         self.sigma_unconstrained.data.fill_(_unconstrain(torch.as_tensor(self.sigma_init_scale), constraints.positive))
 
     def forward(self, x_ng: torch.Tensor, var_names_g: np.ndarray) -> dict[str, torch.Tensor | None]:
```

### Comparing `cellarium_ml-0.0.5/cellarium/ml/models/tdigest.py` & `cellarium_ml-0.0.7/cellarium/ml/models/tdigest.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/preprocessing/highly_variable_genes.py` & `cellarium_ml-0.0.7/cellarium/ml/preprocessing/highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/transforms/divide_by_scale.py` & `cellarium_ml-0.0.7/cellarium/ml/transforms/divide_by_scale.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/transforms/filter.py` & `cellarium_ml-0.0.7/cellarium/ml/transforms/filter.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/transforms/log1p.py` & `cellarium_ml-0.0.7/cellarium/ml/transforms/log1p.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/transforms/normalize_total.py` & `cellarium_ml-0.0.7/cellarium/ml/transforms/normalize_total.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/transforms/z_score.py` & `cellarium_ml-0.0.7/cellarium/ml/transforms/z_score.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/utilities/core.py` & `cellarium_ml-0.0.7/cellarium/ml/utilities/core.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/utilities/data.py` & `cellarium_ml-0.0.7/cellarium/ml/utilities/data.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium/ml/utilities/testing.py` & `cellarium_ml-0.0.7/cellarium/ml/utilities/testing.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/cellarium_ml.egg-info/PKG-INFO` & `cellarium_ml-0.0.7/cellarium_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellarium-ml
-Version: 0.0.5
+Version: 0.0.7
 Summary: Machine learning library for single-cell data analysis
 Author-email: Yerdos Ordabayev <yordabay@broadinstitute.org>, Mehrtash Babadi <mehrtash@broadinstitute.org>
 License: Copyright (c) 2023, Broad Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
@@ -43,15 +43,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 Requires-Dist: anndata
 Requires-Dist: boltons
 Requires-Dist: braceexpand
 Requires-Dist: crick>=0.0.4
 Requires-Dist: google-cloud-storage
-Requires-Dist: jsonargparse[signatures]
+Requires-Dist: jsonargparse[signatures]==4.27.7
 Requires-Dist: lightning>=2.2.0
 Requires-Dist: pyro-ppl
 Requires-Dist: pytest
 Requires-Dist: torch>=2.2.0
 Requires-Dist: transformers
 Provides-Extra: lint
 Requires-Dist: ruff; extra == "lint"
```

### Comparing `cellarium_ml-0.0.5/cellarium_ml.egg-info/SOURCES.txt` & `cellarium_ml-0.0.7/cellarium_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/pyproject.toml` & `cellarium_ml-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 dependencies = [
   "anndata",
   "boltons",
   "braceexpand",
   "crick>=0.0.4",
   "google-cloud-storage",
-  "jsonargparse[signatures]",
+  "jsonargparse[signatures]==4.27.7",
   "lightning>=2.2.0",
   "pyro-ppl",
   "pytest",
   "torch>=2.2.0",
   "transformers",
 ]
```

### Comparing `cellarium_ml-0.0.5/tests/test_cli.py` & `cellarium_ml-0.0.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_core.py` & `cellarium_ml-0.0.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_dataset.py` & `cellarium_ml-0.0.7/tests/test_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright Contributors to the Cellarium project.
 # SPDX-License-Identifier: BSD-3-Clause
 
 import math
 import os
 from pathlib import Path
+from typing import Literal
 
 import lightning.pytorch as pl
 import numpy as np
 import pytest
 import torch
 from anndata import AnnData
 
@@ -38,72 +39,87 @@
         sliced_adata.write(os.path.join(tmp_path, f"adata.00{i}.h5ad"))
 
     # distributed anndata
     filenames = str(os.path.join(tmp_path, f"adata.{{000..00{len(limits)-1}}}.h5ad"))
     dadc = DistributedAnnDataCollection(
         filenames,
         limits,
-        max_cache_size=2,
+        max_cache_size=3,
         cache_size_strictly_enforced=True,
     )
     return dadc
 
 
+@pytest.mark.parametrize("iteration_strategy", ["same_order", "cache_efficient"])
 @pytest.mark.parametrize("shuffle", [False, True], ids=["no shuffle", "shuffle"])
 @pytest.mark.parametrize("num_workers", [0, 1, 2], ids=["zero workers", "one worker", "two workers"])
 @pytest.mark.parametrize("batch_size", [1, 2, 3], ids=["batch size 1", "batch size 2", "batch size 3"])
-def test_iterable_dataset(dadc: DistributedAnnDataCollection, shuffle: bool, num_workers: int, batch_size: int):
+def test_iterable_dataset(
+    dadc: DistributedAnnDataCollection,
+    iteration_strategy: Literal["same_order", "cache_efficient"],
+    shuffle: bool,
+    num_workers: int,
+    batch_size: int,
+):
     n_obs = len(dadc)
     dataset = IterableDistributedAnnDataCollectionDataset(
         dadc,
+        iteration_strategy=iteration_strategy,
         batch_keys={"x_ng": AnnDataField("X")},
         batch_size=batch_size,
         shuffle=shuffle,
         test_mode=True,
     )
     data_loader = torch.utils.data.DataLoader(
         dataset,
         num_workers=num_workers,
         collate_fn=collate_fn,
     )
 
-    miss_counts = list(int(i) for batch in data_loader for i in batch["miss_count"])
+    miss_counts = list(int(batch["miss_count"]) for batch in data_loader for _ in batch["x_ng"])
+    actual_idx = list(int(i) for batch in data_loader for i in batch["x_ng"])
 
     if num_workers > 1:
-        worker_ids = list(int(i) for batch in data_loader for i in batch["worker_id"])
+        worker_ids = list(int(batch["worker_id"]) for batch in data_loader for _ in batch["x_ng"])
+        adatas_oidx = np.searchsorted([0] + dadc.limits, actual_idx, side="right")
         for worker in range(num_workers):
             miss_count = max(c for c, w in zip(miss_counts, worker_ids) if w == worker)
-            assert miss_count == math.ceil(len(dadc.limits) / num_workers)
+            assert miss_count == len(set([o for o, w in zip(adatas_oidx, worker_ids) if w == worker]))
     else:
         miss_count = max(miss_counts)
         assert miss_count == len(dadc.limits)
 
-    actual_idx = list(int(i) for batch in data_loader for i in batch["x_ng"])
     expected_idx = list(range(n_obs))
 
     # assert entire dataset is sampled
-    assert len(expected_idx) == len(actual_idx)
-    assert set(expected_idx) == set(actual_idx)
+    if not shuffle and iteration_strategy == "same_order":
+        assert expected_idx == actual_idx
+    else:
+        assert len(expected_idx) == len(actual_idx)
+        assert set(expected_idx) == set(actual_idx)
 
 
+@pytest.mark.parametrize("iteration_strategy", ["same_order", "cache_efficient"])
 @pytest.mark.parametrize("shuffle", [False, True], ids=["no shuffle", "shuffle"])
 @pytest.mark.parametrize("num_workers", [0, 1, 2], ids=["zero workers", "one worker", "two workers"])
 @pytest.mark.parametrize("batch_size", [1, 2, 3], ids=["batch size 1", "batch size 2", "batch size 3"])
 @pytest.mark.parametrize("drop_last", [False, True], ids=["no drop last", "drop last"])
 def test_iterable_dataset_multi_device(
     dadc: DistributedAnnDataCollection,
+    iteration_strategy: Literal["same_order", "cache_efficient"],
     shuffle: bool,
     num_workers: int,
     batch_size: int,
     drop_last: bool,
 ):
     devices = int(os.environ.get("TEST_DEVICES", "1"))
     n_obs = len(dadc)
     dataset = IterableDistributedAnnDataCollectionDataset(
         dadc,
+        iteration_strategy=iteration_strategy,
         batch_keys={"x_ng": AnnDataField("X")},
         batch_size=batch_size,
         shuffle=shuffle,
         drop_last=drop_last,
         test_mode=True,
     )
     data_loader = torch.utils.data.DataLoader(
```

### Comparing `cellarium_ml-0.0.5/tests/test_distributed_anndata.py` & `cellarium_ml-0.0.7/tests/test_distributed_anndata.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_geneformer.py` & `cellarium_ml-0.0.7/tests/test_geneformer.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_highly_variable_genes.py` & `cellarium_ml-0.0.7/tests/test_highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_ipca.py` & `cellarium_ml-0.0.7/tests/test_ipca.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_mup.py` & `cellarium_ml-0.0.7/tests/test_mup.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_onepass_mean_var_std.py` & `cellarium_ml-0.0.7/tests/test_onepass_mean_var_std.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_ppca.py` & `cellarium_ml-0.0.7/tests/test_ppca.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_schema.py` & `cellarium_ml-0.0.7/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_tdigest.py` & `cellarium_ml-0.0.7/tests/test_tdigest.py`

 * *Files identical despite different names*

### Comparing `cellarium_ml-0.0.5/tests/test_transforms.py` & `cellarium_ml-0.0.7/tests/test_transforms.py`

 * *Files identical despite different names*

