# Comparing `tmp/mlable-0.1.4.tar.gz` & `tmp/mlable-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlable-0.1.4.tar", max compression
+gzip compressed data, was "mlable-0.2.1.tar", max compression
```

## Comparing `mlable-0.1.4.tar` & `mlable-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,16 @@
--rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.1.4/.github/README.md
--rw-r--r--   0        0        0        0 2024-01-25 21:43:22.740044 mlable-0.1.4/mlable/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 20:33:11.034995 mlable-0.1.4/mlable/keras/__init__.py
--rw-r--r--   0        0        0     5219 2024-03-17 15:32:31.801607 mlable-0.1.4/mlable/keras/models.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:37.881478 mlable-0.1.4/mlable/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 15:44:53.795021 mlable-0.1.4/mlable/models/colonel/__init__.py
--rw-r--r--   0        0        0    17241 2024-03-12 20:42:42.653388 mlable-0.1.4/mlable/models/gpm/README.md
--rw-r--r--   0        0        0        0 2024-02-04 22:08:59.205764 mlable-0.1.4/mlable/models/gpm/__init__.py
--rw-r--r--   0        0        0     9345 2024-03-12 21:16:09.662821 mlable-0.1.4/mlable/models/gpm/main.py
--rw-r--r--   0        0        0        0 2024-01-25 11:56:28.560613 mlable-0.1.4/mlable/models/gpt/__init__.py
--rw-r--r--   0        0        0     4609 2024-03-15 20:59:30.682559 mlable-0.1.4/mlable/models/gpt/rnn.torch.py
--rw-r--r--   0        0        0    33483 2024-02-05 23:20:39.711787 mlable-0.1.4/mlable/models/gpt/sat.keras.ipynb
--rw-r--r--   0        0        0     5407 2024-03-17 15:46:00.373875 mlable-0.1.4/mlable/models/gpt/sat.keras.py
--rw-r--r--   0        0        0     4642 2024-03-12 21:21:28.151800 mlable-0.1.4/mlable/models/gpt/sat.tensorflow.py
--rw-r--r--   0        0        0     4859 2024-03-16 16:19:19.458786 mlable-0.1.4/mlable/models/gpt/sat.torch.py
--rw-r--r--   0        0        0     8689 2024-01-07 22:39:32.640751 mlable-0.1.4/mlable/models/makemore/.old/mlp.batch.tensorflow.py
--rw-r--r--   0        0        0    11306 2024-01-07 22:39:21.714118 mlable-0.1.4/mlable/models/makemore/.old/mlp.regularization.tensorflow.py
--rw-r--r--   0        0        0    10543 2024-01-07 22:38:57.034242 mlable-0.1.4/mlable/models/makemore/.old/mlp.viz.tensorflow.py
--rw-r--r--   0        0        0        0 2024-01-25 21:44:14.973726 mlable-0.1.4/mlable/models/makemore/__init__.py
--rw-r--r--   0        0        0     7600 2024-01-14 14:50:05.071077 mlable-0.1.4/mlable/models/makemore/cnn.keras.py
--rw-r--r--   0        0        0    15313 2024-02-17 10:48:33.230500 mlable-0.1.4/mlable/models/makemore/cnn.tensorflow.py
--rw-r--r--   0        0        0    10039 2024-03-14 22:06:01.118763 mlable-0.1.4/mlable/models/makemore/cnn.torch.py
--rw-r--r--   0        0        0     6271 2024-01-22 21:19:30.047231 mlable-0.1.4/mlable/models/makemore/mlp.keras.py
--rw-r--r--   0        0        0    14087 2024-02-16 15:05:52.419701 mlable-0.1.4/mlable/models/makemore/mlp.tensorflow.py
--rw-r--r--   0        0        0        0 2024-04-09 09:50:53.069681 mlable-0.1.4/mlable/models/sold/__init__.py
--rw-r--r--   0        0        0     7419 2024-04-09 09:52:25.100652 mlable-0.1.4/mlable/models/sold/bytecode.py
--rw-r--r--   0        0        0     6669 2024-04-09 09:50:53.069681 mlable-0.1.4/mlable/models/sold/main.keras.py
--rw-r--r--   0        0        0     2387 2024-04-09 09:56:41.383364 mlable-0.1.4/mlable/models/sold/solidity.py
--rw-r--r--   0        0        0        0 2024-03-18 18:34:21.653083 mlable-0.1.4/mlable/models/tokun/__init__.py
--rw-r--r--   0        0        0      904 2024-05-25 15:34:25.560472 mlable-0.1.4/mlable/models/tokun/evaluation.py
--rw-r--r--   0        0        0        0 2024-05-25 15:34:55.413761 mlable-0.1.4/mlable/models/tokun/export.py
--rw-r--r--   0        0        0     4321 2024-04-29 07:09:43.479546 mlable-0.1.4/mlable/models/tokun/layers.py
--rw-r--r--   0        0        0      566 2024-05-25 15:34:08.443841 mlable-0.1.4/mlable/models/tokun/meta.py
--rw-r--r--   0        0        0        0 2024-05-25 15:34:32.123793 mlable-0.1.4/mlable/models/tokun/model.py
--rw-r--r--   0        0        0     4636 2024-05-25 15:03:05.804689 mlable-0.1.4/mlable/models/tokun/pipeline.py
--rw-r--r--   0        0        0        0 2024-05-25 15:34:55.413761 mlable-0.1.4/mlable/models/tokun/test.py
--rw-r--r--   0        0        0   832982 2024-05-02 11:00:57.733286 mlable-0.1.4/mlable/models/tokun/tokun.train.ipynb
--rw-r--r--   0        0        0    11288 2024-05-02 09:26:23.383872 mlable-0.1.4/mlable/models/tokun/train.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.1.4/mlable/tensorflow/__init__.py
--rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.1.4/mlable/tensorflow/data.py
--rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.1.4/mlable/tensorflow/initializers.py
--rw-r--r--   0        0        0      594 2024-05-10 08:46:46.358956 mlable-0.1.4/mlable/tensorflow/io.py
--rw-r--r--   0        0        0    17572 2024-05-25 16:38:36.114749 mlable-0.1.4/mlable/tensorflow/layers.py
--rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.1.4/mlable/tensorflow/losses.py
--rw-r--r--   0        0        0     4622 2024-01-31 18:01:34.815819 mlable-0.1.4/mlable/tensorflow/models.py
--rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.1.4/mlable/tensorflow/optimizers.py
--rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.1.4/mlable/tensorflow/sampling.py
--rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.1.4/mlable/tensorflow/summary.py
--rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.1.4/mlable/tokens/__init__.py
--rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.1.4/mlable/tokens/bpe.py
--rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.1.4/mlable/tokens/ngrams.py
--rw-r--r--   0        0        0        0 2024-02-25 16:24:42.204319 mlable-0.1.4/mlable/torch/__init__.py
--rw-r--r--   0        0        0      252 2024-03-14 21:37:39.458099 mlable-0.1.4/mlable/torch/data.py
--rw-r--r--   0        0        0    11622 2024-05-25 18:10:35.579019 mlable-0.1.4/mlable/torch/layers.py
--rw-r--r--   0        0        0     2565 2024-03-16 16:03:36.844134 mlable-0.1.4/mlable/torch/optimizers.py
--rw-r--r--   0        0        0      612 2024-03-14 12:49:57.500345 mlable-0.1.4/mlable/torch/sampling.py
--rw-r--r--   0        0        0      453 2024-05-25 16:38:51.118655 mlable-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 mlable-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.2.1/.github/README.md
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.2.1/mlable/__init__.py
+-rw-r--r--   0        0        0     5219 2024-05-29 20:55:39.325361 mlable-0.2.1/mlable/blocks.py
+-rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.2.1/mlable/data.py
+-rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.2.1/mlable/initializers.py
+-rw-r--r--   0        0        0      594 2024-05-10 08:46:46.358956 mlable-0.2.1/mlable/io.py
+-rw-r--r--   0        0        0    17572 2024-05-25 16:38:36.114749 mlable-0.2.1/mlable/layers.py
+-rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.2.1/mlable/losses.py
+-rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.2.1/mlable/optimizers.py
+-rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.2.1/mlable/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.2.1/mlable/preprocessing/bpe.py
+-rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.2.1/mlable/preprocessing/ngrams.py
+-rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.2.1/mlable/sampling.py
+-rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.2.1/mlable/summary.py
+-rw-r--r--   0        0        0      433 2024-05-29 20:57:51.313622 mlable-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 mlable-0.2.1/PKG-INFO
```

### Comparing `mlable-0.1.4/mlable/keras/models.py` & `mlable-0.2.1/mlable/blocks.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/models/sold/solidity.py` & `mlable-0.2.1/mlable/preprocessing/bpe.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/tensorflow/initializers.py` & `mlable-0.2.1/mlable/initializers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/tensorflow/io.py` & `mlable-0.2.1/mlable/io.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/tensorflow/layers.py` & `mlable-0.2.1/mlable/layers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/tensorflow/optimizers.py` & `mlable-0.2.1/mlable/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/tensorflow/sampling.py` & `mlable-0.2.1/mlable/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/tensorflow/summary.py` & `mlable-0.2.1/mlable/summary.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/mlable/tokens/ngrams.py` & `mlable-0.2.1/mlable/preprocessing/ngrams.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.4/PKG-INFO` & `mlable-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: mlable
-Version: 0.1.4
-Summary: Tensorflow and pyTorch libs + atomic projects and drafts.
+Version: 0.2.1
+Summary: Tensorflow libs: layers, blocks, optimizers, etc.
 Author: apehex
 Author-email: apehex@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: tensorflow (>=2.14)
-Requires-Dist: tensorflow-datasets (>=4.9)
-Requires-Dist: torch (>=2.2)
 Description-Content-Type: text/markdown
 
 # MLable
 
 Atomic ML projects to get started.
 
 ## TODO
```

