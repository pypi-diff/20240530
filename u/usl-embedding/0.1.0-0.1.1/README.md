# Comparing `tmp/usl_embedding-0.1.0.tar.gz` & `tmp/usl_embedding-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usl_embedding-0.1.0.tar", last modified: Thu May 30 15:22:18 2024, max compression
+gzip compressed data, was "usl_embedding-0.1.1.tar", last modified: Thu May 30 15:37:56 2024, max compression
```

## Comparing `usl_embedding-0.1.0.tar` & `usl_embedding-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:22:18.053866 usl_embedding-0.1.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1089 2024-05-30 14:51:10.000000 usl_embedding-0.1.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2024-05-30 15:22:18.053866 usl_embedding-0.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2589 2024-05-30 15:07:03.000000 usl_embedding-0.1.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:22:18.053866 usl_embedding-0.1.0/methods/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 12:26:34.000000 usl_embedding-0.1.0/methods/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3551 2024-05-30 14:48:27.000000 usl_embedding-0.1.0/methods/usl.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13478 2024-05-30 14:42:31.000000 usl_embedding-0.1.0/methods/usl_t.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:22:18.053866 usl_embedding-0.1.0/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 12:56:17.000000 usl_embedding-0.1.0/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:22:18.053866 usl_embedding-0.1.0/models/ssl_t_models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 12:56:17.000000 usl_embedding-0.1.0/models/ssl_t_models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2024-05-30 14:26:14.000000 usl_embedding-0.1.0/models/ssl_t_models/clustering_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-30 15:22:18.053866 usl_embedding-0.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      865 2024-05-30 15:13:58.000000 usl_embedding-0.1.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:22:18.053866 usl_embedding-0.1.0/usl_embedding.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2024-05-30 15:22:18.000000 usl_embedding-0.1.0/usl_embedding.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      393 2024-05-30 15:22:18.000000 usl_embedding-0.1.0/usl_embedding.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-30 15:22:18.000000 usl_embedding-0.1.0/usl_embedding.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2024-05-30 15:22:18.000000 usl_embedding-0.1.0/usl_embedding.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-05-30 15:22:18.000000 usl_embedding-0.1.0/usl_embedding.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-05-30 15:22:18.000000 usl_embedding-0.1.0/usl_embedding.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:37:56.259128 usl_embedding-0.1.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1089 2024-05-30 14:51:10.000000 usl_embedding-0.1.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3452 2024-05-30 15:37:56.259128 usl_embedding-0.1.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2024-05-30 15:31:20.000000 usl_embedding-0.1.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:37:56.259128 usl_embedding-0.1.1/methods/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 12:26:34.000000 usl_embedding-0.1.1/methods/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3551 2024-05-30 14:48:27.000000 usl_embedding-0.1.1/methods/usl.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13478 2024-05-30 14:42:31.000000 usl_embedding-0.1.1/methods/usl_t.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:37:56.259128 usl_embedding-0.1.1/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 12:56:17.000000 usl_embedding-0.1.1/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:37:56.259128 usl_embedding-0.1.1/models/ssl_t_models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 12:56:17.000000 usl_embedding-0.1.1/models/ssl_t_models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2024-05-30 14:26:14.000000 usl_embedding-0.1.1/models/ssl_t_models/clustering_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-30 15:37:56.259128 usl_embedding-0.1.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      865 2024-05-30 15:35:27.000000 usl_embedding-0.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 15:37:56.259128 usl_embedding-0.1.1/usl_embedding.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3452 2024-05-30 15:37:56.000000 usl_embedding-0.1.1/usl_embedding.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      393 2024-05-30 15:37:56.000000 usl_embedding-0.1.1/usl_embedding.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-30 15:37:56.000000 usl_embedding-0.1.1/usl_embedding.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2024-05-30 15:37:56.000000 usl_embedding-0.1.1/usl_embedding.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-05-30 15:37:56.000000 usl_embedding-0.1.1/usl_embedding.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-05-30 15:37:56.000000 usl_embedding-0.1.1/usl_embedding.egg-info/top_level.txt
```

### Comparing `usl_embedding-0.1.0/LICENSE` & `usl_embedding-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `usl_embedding-0.1.0/PKG-INFO` & `usl_embedding-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usl_embedding
-Version: 0.1.0
+Version: 0.1.1
 Summary: Implements the USL Technique for embeddings of any data, be it text, image, etc.
 Home-page: https://github.com/Hosseini1373/usl_for_embedding
 Author: Ahmad Hosseini, ZHAW
 Author-email: s.ahmad.hosseini94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,21 +34,24 @@
 ## Usage
 
 The `usl_for_embedding` function is designed to process embedding arrays for clustering. It can be used directly by importing from the `selective_labeling.py`:
 
 ```python
 from selective_labeling import usl_for_embedding
 
-# Example usage:
-embeddings = # your embedding data here
-method = 'usl'  # or 'usl-t'
-n_clusters = 5  # number of clusters to form
+# Generate 10 embeddings, each with 10 random floating-point numbers
+data = {'embedding': [list(np.random.rand(10)) for _ in range(10)]}
 
-selected_indices = usl_for_embedding(embeddings, method=method, n_clusters=n_clusters)
-print("Selected indices for clustering:", selected_indices)
+# method is 'usl' or 'usl-t'
+# n_clusters is the number of samples that should be selected for labeling
+selected_indices = usl_for_embedding(data['embedding'],method='usl',n_clusters=2,
+                            learning_rate=0.001,batch_size=64,n_init=10,m_reg=0.9,k=10,lambda_=0.5,
+                            epsilon=1e-5,alpha=0.75,num_epochs_cluster=100,num_heads=3)
+
+print(selected_indices)
 ```
 
 ### Parameters
 - **embeddings (array-like)**: Input data, embeddings to be clustered.
 - **method (str)**: The clustering method to use ('usl' or 'usl-t').
 - **n_clusters (int)**: Number of clusters to form.
 - Additional parameters include learning rate, batch size, initialization runs, regularization term, and more described in `main.py`.
```

### Comparing `usl_embedding-0.1.0/README.md` & `usl_embedding-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -16,21 +16,24 @@
 ## Usage
 
 The `usl_for_embedding` function is designed to process embedding arrays for clustering. It can be used directly by importing from the `selective_labeling.py`:
 
 ```python
 from selective_labeling import usl_for_embedding
 
-# Example usage:
-embeddings = # your embedding data here
-method = 'usl'  # or 'usl-t'
-n_clusters = 5  # number of clusters to form
+# Generate 10 embeddings, each with 10 random floating-point numbers
+data = {'embedding': [list(np.random.rand(10)) for _ in range(10)]}
 
-selected_indices = usl_for_embedding(embeddings, method=method, n_clusters=n_clusters)
-print("Selected indices for clustering:", selected_indices)
+# method is 'usl' or 'usl-t'
+# n_clusters is the number of samples that should be selected for labeling
+selected_indices = usl_for_embedding(data['embedding'],method='usl',n_clusters=2,
+                            learning_rate=0.001,batch_size=64,n_init=10,m_reg=0.9,k=10,lambda_=0.5,
+                            epsilon=1e-5,alpha=0.75,num_epochs_cluster=100,num_heads=3)
+
+print(selected_indices)
 ```
 
 ### Parameters
 - **embeddings (array-like)**: Input data, embeddings to be clustered.
 - **method (str)**: The clustering method to use ('usl' or 'usl-t').
 - **n_clusters (int)**: Number of clusters to form.
 - Additional parameters include learning rate, batch size, initialization runs, regularization term, and more described in `main.py`.
```

### Comparing `usl_embedding-0.1.0/methods/usl.py` & `usl_embedding-0.1.1/methods/usl.py`

 * *Files identical despite different names*

### Comparing `usl_embedding-0.1.0/methods/usl_t.py` & `usl_embedding-0.1.1/methods/usl_t.py`

 * *Files identical despite different names*

### Comparing `usl_embedding-0.1.0/models/ssl_t_models/clustering_model.py` & `usl_embedding-0.1.1/models/ssl_t_models/clustering_model.py`

 * *Files identical despite different names*

### Comparing `usl_embedding-0.1.0/setup.py` & `usl_embedding-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='usl_embedding',
-    version='0.1.0',
+    version='0.1.1',
     author='Ahmad Hosseini, ZHAW',
     author_email='s.ahmad.hosseini94@gmail.com',
     packages=find_packages(),
     install_requires=[
         'numpy', 'pandas', 'scikit-learn', 'torch',
     ],
     python_requires='>=3.6',
```

### Comparing `usl_embedding-0.1.0/usl_embedding.egg-info/PKG-INFO` & `usl_embedding-0.1.1/usl_embedding.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usl_embedding
-Version: 0.1.0
+Version: 0.1.1
 Summary: Implements the USL Technique for embeddings of any data, be it text, image, etc.
 Home-page: https://github.com/Hosseini1373/usl_for_embedding
 Author: Ahmad Hosseini, ZHAW
 Author-email: s.ahmad.hosseini94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -34,21 +34,24 @@
 ## Usage
 
 The `usl_for_embedding` function is designed to process embedding arrays for clustering. It can be used directly by importing from the `selective_labeling.py`:
 
 ```python
 from selective_labeling import usl_for_embedding
 
-# Example usage:
-embeddings = # your embedding data here
-method = 'usl'  # or 'usl-t'
-n_clusters = 5  # number of clusters to form
+# Generate 10 embeddings, each with 10 random floating-point numbers
+data = {'embedding': [list(np.random.rand(10)) for _ in range(10)]}
 
-selected_indices = usl_for_embedding(embeddings, method=method, n_clusters=n_clusters)
-print("Selected indices for clustering:", selected_indices)
+# method is 'usl' or 'usl-t'
+# n_clusters is the number of samples that should be selected for labeling
+selected_indices = usl_for_embedding(data['embedding'],method='usl',n_clusters=2,
+                            learning_rate=0.001,batch_size=64,n_init=10,m_reg=0.9,k=10,lambda_=0.5,
+                            epsilon=1e-5,alpha=0.75,num_epochs_cluster=100,num_heads=3)
+
+print(selected_indices)
 ```
 
 ### Parameters
 - **embeddings (array-like)**: Input data, embeddings to be clustered.
 - **method (str)**: The clustering method to use ('usl' or 'usl-t').
 - **n_clusters (int)**: Number of clusters to form.
 - Additional parameters include learning rate, batch size, initialization runs, regularization term, and more described in `main.py`.
```

