# Comparing `tmp/giza_datasets-0.3.0.tar.gz` & `tmp/giza_datasets-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_datasets-0.3.0.tar", max compression
+gzip compressed data, was "giza_datasets-0.3.1.tar", max compression
```

## Comparing `giza_datasets-0.3.0.tar` & `giza_datasets-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/LICENSE
--rw-r--r--   0        0        0     3951 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/README.md
--rw-r--r--   0        0        0      136 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/__init__.py
--rw-r--r--   0        0        0     2854 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/cache_manager.py
--rw-r--r--   0        0        0   151371 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/constants.py
--rw-r--r--   0        0        0      635 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/defillama_constants.py
--rw-r--r--   0        0        0     3240 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/hub.py
--rw-r--r--   0        0        0     5984 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/loaders.py
--rw-r--r--   0        0        0     1442 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/models.py
--rw-r--r--   0        0        0      560 2024-05-22 13:55:03.528908 giza_datasets-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3951 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/README.md
+-rw-r--r--   0        0        0      136 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/giza/datasets/__init__.py
+-rw-r--r--   0        0        0     2854 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/giza/datasets/cache_manager.py
+-rw-r--r--   0        0        0   151371 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/giza/datasets/constants.py
+-rw-r--r--   0        0        0      635 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/giza/datasets/defillama_constants.py
+-rw-r--r--   0        0        0     3240 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/giza/datasets/hub.py
+-rw-r--r--   0        0        0     6091 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/giza/datasets/loaders.py
+-rw-r--r--   0        0        0     1442 2024-05-30 10:05:16.159443 giza_datasets-0.3.1/giza/datasets/models.py
+-rw-r--r--   0        0        0      560 2024-05-30 10:05:16.163443 giza_datasets-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.3.1/PKG-INFO
```

### Comparing `giza_datasets-0.3.0/LICENSE` & `giza_datasets-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.3.0/README.md` & `giza_datasets-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.3.0/giza/datasets/cache_manager.py` & `giza_datasets-0.3.1/giza/datasets/cache_manager.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.3.0/giza/datasets/constants.py` & `giza_datasets-0.3.1/giza/datasets/constants.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.3.0/giza/datasets/defillama_constants.py` & `giza_datasets-0.3.1/giza/datasets/defillama_constants.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.3.0/giza/datasets/hub.py` & `giza_datasets-0.3.1/giza/datasets/hub.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.3.0/giza/datasets/loaders.py` & `giza_datasets-0.3.1/giza/datasets/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 class DatasetsLoader:
     """
     DatasetsLoader is a class for loading datasets from Google Cloud Storage (GCS).
     It uses the GCSFileSystem for accessing files and Polars for handling data.
     """
 
     def __init__(self, use_cache=True, cache_dir=None):
-        self.fs = gcsfs.GCSFileSystem(verify=False)
+        # Token is set to "anon" to allow anonymous access to GCS as bucket should be public
+        self.fs = gcsfs.GCSFileSystem(verify=False, token="anon")
         self.dataset_hub = DATASET_HUB
         self.use_cache = use_cache
         self.cache_dir = (
             cache_dir
             if cache_dir is not None
             else os.path.join(os.path.expanduser("~"), ".cache/giza.datasets")
         )
```

### Comparing `giza_datasets-0.3.0/giza/datasets/models.py` & `giza_datasets-0.3.1/giza/datasets/models.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.3.0/pyproject.toml` & `giza_datasets-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-datasets"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Fran Algaba <f.algaba@outlook.es>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "giza"}]
 
 [tool.poetry.dependencies]
```

### Comparing `giza_datasets-0.3.0/PKG-INFO` & `giza_datasets-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-datasets
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Author: Fran Algaba
 Author-email: f.algaba@outlook.es
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

