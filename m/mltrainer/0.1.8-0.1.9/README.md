# Comparing `tmp/mltrainer-0.1.8.tar.gz` & `tmp/mltrainer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltrainer-0.1.8.tar", last modified: Tue Oct 17 14:22:41 2023, max compression
+gzip compressed data, was "mltrainer-0.1.9.tar", last modified: Tue Oct 17 14:44:53 2023, max compression
```

## Comparing `mltrainer-0.1.8.tar` & `mltrainer-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      525 2023-08-22 17:53:26.865719 mltrainer-0.1.8/README.md
--rw-r--r--   0        0        0      177 2023-10-17 14:20:24.442477 mltrainer-0.1.8/mltrainer/__init__.py
--rw-r--r--   0        0        0     1653 2023-08-22 17:53:26.865938 mltrainer-0.1.8/mltrainer/imagemodels.py
--rw-r--r--   0        0        0     1653 2023-08-22 17:53:26.866019 mltrainer-0.1.8/mltrainer/metrics.py
--rw-r--r--   0        0        0     3201 2023-10-17 14:17:23.486325 mltrainer-0.1.8/mltrainer/preprocessors.py
--rw-r--r--   0        0        0     4285 2023-08-22 17:53:26.866119 mltrainer-0.1.8/mltrainer/rnn_models.py
--rw-r--r--   0        0        0     1582 2023-10-17 14:20:08.989319 mltrainer-0.1.8/mltrainer/settings.py
--rw-r--r--   0        0        0     2388 2023-08-22 17:53:26.866317 mltrainer-0.1.8/mltrainer/tokenizer.py
--rw-r--r--   0        0        0     8805 2023-10-17 13:07:14.934862 mltrainer-0.1.8/mltrainer/trainer.py
--rw-r--r--   0        0        0     2489 2023-08-22 17:53:26.866536 mltrainer-0.1.8/mltrainer/vae.py
--rw-r--r--   0        0        0     1151 2023-10-17 14:22:41.956776 mltrainer-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 mltrainer-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      525 2023-08-22 17:53:26.865719 mltrainer-0.1.9/README.md
+-rw-r--r--   0        0        0      177 2023-10-17 14:43:31.698087 mltrainer-0.1.9/mltrainer/__init__.py
+-rw-r--r--   0        0        0     1653 2023-08-22 17:53:26.865938 mltrainer-0.1.9/mltrainer/imagemodels.py
+-rw-r--r--   0        0        0     1653 2023-08-22 17:53:26.866019 mltrainer-0.1.9/mltrainer/metrics.py
+-rw-r--r--   0        0        0     3201 2023-10-17 14:17:23.486325 mltrainer-0.1.9/mltrainer/preprocessors.py
+-rw-r--r--   0        0        0     4285 2023-08-22 17:53:26.866119 mltrainer-0.1.9/mltrainer/rnn_models.py
+-rw-r--r--   0        0        0     1582 2023-10-17 14:20:08.989319 mltrainer-0.1.9/mltrainer/settings.py
+-rw-r--r--   0        0        0     2388 2023-08-22 17:53:26.866317 mltrainer-0.1.9/mltrainer/tokenizer.py
+-rw-r--r--   0        0        0     8831 2023-10-17 14:43:05.924164 mltrainer-0.1.9/mltrainer/trainer.py
+-rw-r--r--   0        0        0     2489 2023-08-22 17:53:26.866536 mltrainer-0.1.9/mltrainer/vae.py
+-rw-r--r--   0        0        0     1151 2023-10-17 14:44:53.501700 mltrainer-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1548 1970-01-01 00:00:00.000000 mltrainer-0.1.9/PKG-INFO
```

### Comparing `mltrainer-0.1.8/README.md` & `mltrainer-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/mltrainer/imagemodels.py` & `mltrainer-0.1.9/mltrainer/imagemodels.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/mltrainer/metrics.py` & `mltrainer-0.1.9/mltrainer/metrics.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/mltrainer/preprocessors.py` & `mltrainer-0.1.9/mltrainer/preprocessors.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/mltrainer/rnn_models.py` & `mltrainer-0.1.9/mltrainer/rnn_models.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/mltrainer/settings.py` & `mltrainer-0.1.9/mltrainer/settings.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/mltrainer/tokenizer.py` & `mltrainer-0.1.9/mltrainer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/mltrainer/trainer.py` & `mltrainer-0.1.9/mltrainer/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Callable, Dict, Iterator, Optional, Tuple
 
 import gin
 import mlflow
 # needed to make summarywriter load without error
 from loguru import logger
-from ray import tune
+import ray
 import torch
 from torch.utils.tensorboard import SummaryWriter
 from tqdm import tqdm
 
 from mltrainer import ReportTypes, TrainerSettings
 
 
@@ -139,19 +139,20 @@
         self, epoch: int, train_loss: float, test_loss: float, metric_dict: Dict
     ) -> None:
         epoch = epoch + self.last_epoch
         reporttypes = self.settings.reporttypes
         self.test_loss = test_loss
 
         if ReportTypes.RAY in reporttypes:
-            tune.report(
-                iterations=epoch,
-                train_loss=train_loss,
-                test_loss=test_loss,
+            ray.train.report(
+                {"iterations" : epoch,
+                "train_loss" : train_loss,
+                "test_loss" : test_loss,
                 **metric_dict,
+                }
             )
 
         if ReportTypes.MLFLOW in reporttypes:
             mlflow.log_metric("Loss/train", train_loss, step=epoch)
             mlflow.log_metric("Loss/test", test_loss, step=epoch)
             for m in metric_dict:
                 mlflow.log_metric(f"metric/{m}", metric_dict[m], step=epoch)
```

### Comparing `mltrainer-0.1.8/mltrainer/vae.py` & `mltrainer-0.1.9/mltrainer/vae.py`

 * *Files identical despite different names*

### Comparing `mltrainer-0.1.8/pyproject.toml` & `mltrainer-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mltrainer"
-version = "0.1.8"
+version = "0.1.9"
 description = "toolkit for training pytorch models"
 authors = [
     { name = "R.Grouls", email = "Raoul.Grouls@han.nl" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
```

### Comparing `mltrainer-0.1.8/PKG-INFO` & `mltrainer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltrainer
-Version: 0.1.8
+Version: 0.1.9
 Summary: toolkit for training pytorch models
 Author-Email: R.Grouls <Raoul.Grouls@han.nl>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python
 Classifier: Typing :: Typed
```

