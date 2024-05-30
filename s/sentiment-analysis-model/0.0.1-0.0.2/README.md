# Comparing `tmp/sentiment_analysis_model-0.0.1.tar.gz` & `tmp/sentiment_analysis_model-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analysis_model-0.0.1.tar", last modified: Thu May 30 07:08:21 2024, max compression
+gzip compressed data, was "sentiment_analysis_model-0.0.2.tar", last modified: Thu May 30 08:04:49 2024, max compression
```

## Comparing `sentiment_analysis_model-0.0.1.tar` & `sentiment_analysis_model-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 07:08:21.692258 sentiment_analysis_model-0.0.1/
--rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      241 2024-05-30 07:08:21.692258 sentiment_analysis_model-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.1/README.md
--rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-30 07:08:21.691259 sentiment_analysis_model-0.0.1/sentiment_analysis_model.egg-info/
--rw-rw-rw-   0        0        0      241 2024-05-30 07:08:21.000000 sentiment_analysis_model-0.0.1/sentiment_analysis_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2024-05-30 07:08:21.000000 sentiment_analysis_model-0.0.1/sentiment_analysis_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 07:08:21.000000 sentiment_analysis_model-0.0.1/sentiment_analysis_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-30 07:08:21.000000 sentiment_analysis_model-0.0.1/sentiment_analysis_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-30 07:08:21.000000 sentiment_analysis_model-0.0.1/sentiment_analysis_model.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 07:08:21.677260 sentiment_analysis_model-0.0.1/sentiment_model/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_model-0.0.1/sentiment_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:08:21.680260 sentiment_analysis_model-0.0.1/sentiment_model/config/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.1/sentiment_model/config/__init__.py
--rw-rw-rw-   0        0        0      772 2024-05-24 14:24:34.000000 sentiment_analysis_model-0.0.1/sentiment_model/config/core.py
--rw-rw-rw-   0        0        0      245 2024-05-30 07:08:01.000000 sentiment_analysis_model-0.0.1/sentiment_model/config.yml
--rw-rw-rw-   0        0        0      419 2024-05-24 15:14:18.000000 sentiment_analysis_model-0.0.1/sentiment_model/pipeline.py
--rw-rw-rw-   0        0        0      551 2024-05-30 04:30:07.000000 sentiment_analysis_model-0.0.1/sentiment_model/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:08:21.686258 sentiment_analysis_model-0.0.1/sentiment_model/processing/
--rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.1/sentiment_model/processing/__init__.py
--rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.1/sentiment_model/processing/features.py
--rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_model-0.0.1/sentiment_model/processing/validation.py
--rw-rw-rw-   0        0        0     1723 2024-05-30 02:55:20.000000 sentiment_analysis_model-0.0.1/sentiment_model/train_pipeline.py
--rw-rw-rw-   0        0        0       86 2024-05-30 07:08:21.693257 sentiment_analysis_model-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-30 07:06:58.000000 sentiment_analysis_model-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 07:08:21.689258 sentiment_analysis_model-0.0.1/tests/
--rw-rw-rw-   0        0        0      154 2024-05-24 11:23:44.000000 sentiment_analysis_model-0.0.1/tests/test_pipeline.py
--rw-rw-rw-   0        0        0      246 2024-05-24 11:23:52.000000 sentiment_analysis_model-0.0.1/tests/test_processing.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.283592 sentiment_analysis_model-0.0.2/
+-rw-rw-rw-   0        0        0       81 2024-05-24 11:27:30.000000 sentiment_analysis_model-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      241 2024-05-30 08:04:49.282561 sentiment_analysis_model-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        2 2024-05-24 11:24:36.000000 sentiment_analysis_model-0.0.2/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-24 11:27:42.000000 sentiment_analysis_model-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.267563 sentiment_analysis_model-0.0.2/sentiment_analysis_model/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:26.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.275561 sentiment_analysis_model-0.0.2/sentiment_analysis_model/config/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:34.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/config/__init__.py
+-rw-rw-rw-   0        0        0      766 2024-05-30 07:39:39.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/config/core.py
+-rw-rw-rw-   0        0        0      428 2024-05-30 07:45:43.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/pipeline.py
+-rw-rw-rw-   0        0        0      548 2024-05-30 07:45:21.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.278569 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/
+-rw-rw-rw-   0        0        0        0 2024-05-24 14:20:48.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/__init__.py
+-rw-rw-rw-   0        0        0      530 2024-05-24 15:15:54.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/features.py
+-rw-rw-rw-   0        0        0      355 2024-05-24 11:22:44.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/validation.py
+-rw-rw-rw-   0        0        0     1692 2024-05-30 07:50:16.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.282561 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/
+-rw-rw-rw-   0        0        0      241 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 08:04:49.000000 sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-30 08:04:49.284562 sentiment_analysis_model-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-30 08:01:47.000000 sentiment_analysis_model-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 08:04:49.280563 sentiment_analysis_model-0.0.2/tests/
+-rw-rw-rw-   0        0        0      163 2024-05-30 07:54:26.000000 sentiment_analysis_model-0.0.2/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      255 2024-05-30 07:54:37.000000 sentiment_analysis_model-0.0.2/tests/test_processing.py
```

### Comparing `sentiment_analysis_model-0.0.1/sentiment_analysis_model.egg-info/SOURCES.txt` & `sentiment_analysis_model-0.0.2/sentiment_analysis_model.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+sentiment_analysis_model/__init__.py
+sentiment_analysis_model/pipeline.py
+sentiment_analysis_model/predict.py
+sentiment_analysis_model/train_pipeline.py
 sentiment_analysis_model.egg-info/PKG-INFO
 sentiment_analysis_model.egg-info/SOURCES.txt
 sentiment_analysis_model.egg-info/dependency_links.txt
 sentiment_analysis_model.egg-info/requires.txt
 sentiment_analysis_model.egg-info/top_level.txt
-sentiment_model/__init__.py
-sentiment_model/config.yml
-sentiment_model/pipeline.py
-sentiment_model/predict.py
-sentiment_model/train_pipeline.py
-sentiment_model/config/__init__.py
-sentiment_model/config/core.py
-sentiment_model/processing/__init__.py
-sentiment_model/processing/features.py
-sentiment_model/processing/validation.py
+sentiment_analysis_model/config/__init__.py
+sentiment_analysis_model/config/core.py
+sentiment_analysis_model/processing/__init__.py
+sentiment_analysis_model/processing/features.py
+sentiment_analysis_model/processing/validation.py
 tests/test_pipeline.py
 tests/test_processing.py
```

### Comparing `sentiment_analysis_model-0.0.1/sentiment_model/config/core.py` & `sentiment_analysis_model-0.0.2/sentiment_analysis_model/config/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from strictyaml import load, YAML
+from strictyaml import load
 
 class TrainingConfig(BaseModel):
     batch_size: int
     epochs: int
     learning_rate: float
 
 class ModelConfig(BaseModel):
```

### Comparing `sentiment_analysis_model-0.0.1/sentiment_model/predict.py` & `sentiment_analysis_model-0.0.2/sentiment_analysis_model/predict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import pandas as pd
 from joblib import load
-from sentiment_model.config.core import fetch_config_from_yaml
+from sentiment_analysis_model.config.core import fetch_config_from_yaml
 
-config = fetch_config_from_yaml('./sentiment_model/config.yml')
+config = fetch_config_from_yaml('./sentiment_analysis_model/config.yml')
 model = load(f"{config.model.name}_{config.model.version}.pkl")
 
 def predict(texts):
     predictions = model.predict(texts)
     sentiment_map = {0: 'negative', 1: 'positive'}
     return [sentiment_map[pred] for pred in predictions]
```

### Comparing `sentiment_analysis_model-0.0.1/sentiment_model/processing/features.py` & `sentiment_analysis_model-0.0.2/sentiment_analysis_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `sentiment_analysis_model-0.0.1/sentiment_model/train_pipeline.py` & `sentiment_analysis_model-0.0.2/sentiment_analysis_model/train_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import logging
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from joblib import dump
-from sentiment_model.config.core import fetch_config_from_yaml
-from sentiment_model.pipeline import create_pipeline
-from sentiment_model.processing.features import preprocess_text  # Import the preprocess_text function
-import numpy as np
-import csv
+from sentiment_analysis_model.config.core import fetch_config_from_yaml
+from sentiment_analysis_model.pipeline import create_pipeline
+from sentiment_analysis_model.processing.features import preprocess_text  
 
 # Configure logging
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
-config = fetch_config_from_yaml('sentiment_model/config.yml')
+config = fetch_config_from_yaml('./sentiment_analysis_model/config.yml')
 
 def train():
     logger.info("Starting training process.")
     # Read the dataset
     data1 = pd.read_csv(config.data.dataset_path, encoding='ISO-8859-1', header=None, nrows=5000)
     data2 = pd.read_csv(config.data.dataset_path, encoding='ISO-8859-1', header=None, skiprows=798622, nrows=5000)
     data = pd.concat([data1, data2])
```

