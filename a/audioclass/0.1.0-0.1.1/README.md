# Comparing `tmp/audioclass-0.1.0.tar.gz` & `tmp/audioclass-0.1.1.tar.gz`

## Comparing `audioclass-0.1.0.tar` & `audioclass-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,69 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 audioclass-0.1.0/.python-version
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 audioclass-0.1.0/Makefile
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 audioclass-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 audioclass-0.1.0/requirements.lock
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 audioclass-0.1.0/scripts/process_directory.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/constants.py
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/postprocess.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/preprocess.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/utils.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/batch/__init__.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/batch/base.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/batch/process.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/batch/simple.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/batch/tensorflow.py
--rw-r--r--   0        0        0    97298 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/data/perch/label.csv
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/models/__init__.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/models/base.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/models/birdnet.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/models/perch.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/models/tensorflow.py
--rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 audioclass-0.1.0/src/audioclass/models/tflite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_postprocess.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_preprocess.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_batch/__init__.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_batch/conftest.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_batch/test_base.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_batch/test_process.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_batch/test_simple.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_batch/test_tensorflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_models/test_birdnet.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_models/test_perch.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 audioclass-0.1.0/tests/test_models/test_tflite.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 audioclass-0.1.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 audioclass-0.1.0/LICENCE
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 audioclass-0.1.0/README.md
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 audioclass-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 audioclass-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 audioclass-0.1.1/.python-version
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 audioclass-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 audioclass-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 audioclass-0.1.1/Makefile
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 audioclass-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 audioclass-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 audioclass-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 audioclass-0.1.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 audioclass-0.1.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 audioclass-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 audioclass-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/getting_started.md
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/usage_guide.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/constants.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/postprocess.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/preprocess.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/utils.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/batch/base.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/batch/index.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/batch/process.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/batch/simple.md
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/batch/tensorflow.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/models/base.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/models/birdnet.md
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/models/index.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/models/perch.md
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/models/tensorflow.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 audioclass-0.1.1/docs/reference/models/tflite.md
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 audioclass-0.1.1/scripts/process_directory.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/__init__.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/constants.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/postprocess.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/preprocess.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/utils.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/batch/__init__.py
+-rw-r--r--   0        0        0    12664 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/batch/base.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/batch/process.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/batch/simple.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/batch/tensorflow.py
+-rw-r--r--   0        0        0    97298 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/data/perch/label.csv
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/models/__init__.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/models/base.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/models/birdnet.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/models/perch.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/models/tensorflow.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 audioclass-0.1.1/src/audioclass/models/tflite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_postprocess.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_preprocess.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_batch/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_batch/conftest.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_batch/test_base.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_batch/test_process.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_batch/test_simple.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_batch/test_tensorflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_models/test_birdnet.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_models/test_perch.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 audioclass-0.1.1/tests/test_models/test_tflite.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 audioclass-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 audioclass-0.1.1/LICENCE
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 audioclass-0.1.1/README.md
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 audioclass-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 audioclass-0.1.1/PKG-INFO
```

### Comparing `audioclass-0.1.0/Makefile` & `audioclass-0.1.1/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 .PHONY: lint-pyright
 lint-pyright:
 	$(ENV_PREFIX)pyright $(PROJECT_NAME)/
 
 .PHONY: lint-ruff
 lint-ruff:
 	$(ENV_PREFIX)ruff check $(PROJECT_NAME)/
-	$(ENV_PREFIX)ruff check tests/
+	$(ENV_PREFIX)ruff check tests/ --ignore "D"
 
 .PHONY: lint
 lint: lint-pyright lint-ruff
 
 .PHONY: test-watch
 test-watch:    ## Run tests and generate coverage report.
 	$(ENV_PREFIX)ptw --runner "$(ENV_PREFIX)coverage run -m pytest -l --tb=long tests/" $(PROJECT_NAME)/ tests/
 
 .PHONY: test
 test:    ## Run tests and generate coverage report.
 	$(ENV_PREFIX)pytest -s -vvv -l --tb=long --maxfail=1 tests/
 
 .PHONY: coverage
 coverage:    ## Run tests and generate coverage report.
-	$(ENV_PREFIX)coverage run -m pytest tests/ --runslow
+	$(ENV_PREFIX)coverage run -m pytest tests/
 
 .PHONY: coverage-report
 coverage-report: coverage
 	$(ENV_PREFIX)coverage html
 	xdg-open http://localhost:8000
 	$(ENV_PREFIX)python -m http.server --directory htmlcov
```

### Comparing `audioclass-0.1.0/requirements-dev.lock` & `audioclass-0.1.1/requirements.lock`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     # via requests
 cffi==1.16.0
     # via soundfile
 cftime==1.6.3
     # via netcdf4
 charset-normalizer==3.3.2
     # via requests
-coverage==7.5.3
-    # via pytest-cov
 cython==3.0.10
     # via soundevent
 dnspython==2.6.1
     # via email-validator
 email-validator==2.1.1
     # via soundevent
 flatbuffers==24.3.25
@@ -46,16 +44,14 @@
     # via tensorflow
 h5py==3.11.0
     # via keras
     # via tensorflow
 idna==3.7
     # via email-validator
     # via requests
-iniconfig==2.0.0
-    # via pytest
 keras==3.3.3
     # via tensorflow
 libclang==18.1.1
     # via tensorflow
 markdown==3.6
     # via tensorboard
 markdown-it-py==3.0.0
@@ -67,16 +63,14 @@
 ml-dtypes==0.3.2
     # via keras
     # via tensorflow
 namex==0.0.8
     # via keras
 netcdf4==1.6.5
     # via audioclass
-nodeenv==1.9.0
-    # via pyright
 numpy==1.24.4
     # via cftime
     # via h5py
     # via keras
     # via ml-dtypes
     # via netcdf4
     # via opt-einsum
@@ -90,56 +84,42 @@
     # via tflite-runtime
     # via xarray
 opt-einsum==3.3.0
     # via tensorflow
 optree==0.11.0
     # via keras
 packaging==24.0
-    # via pytest
     # via tensorflow
     # via xarray
 pandas==2.2.2
     # via audioclass
     # via xarray
-pluggy==1.5.0
-    # via pytest
 protobuf==4.25.3
     # via tensorboard
     # via tensorflow
     # via tensorflow-hub
 pyarrow==16.1.0
     # via audioclass
 pycparser==2.22
     # via cffi
 pydantic==2.7.1
     # via soundevent
 pydantic-core==2.18.2
     # via pydantic
 pygments==2.18.0
     # via rich
-pyright==1.1.365
-pytest==8.2.1
-    # via pytest-cov
-    # via pytest-mock
-pytest-cov==5.0.0
-    # via pytest-cover
-pytest-cover==3.0.0
-    # via pytest-coverage
-pytest-coverage==0.0
-pytest-mock==3.14.0
 python-dateutil==2.9.0.post0
     # via pandas
 pytz==2024.1
     # via pandas
 requests==2.32.2
     # via audioclass
     # via tensorflow
 rich==13.7.1
     # via keras
-ruff==0.4.6
 scipy==1.13.1
     # via soundevent
 setuptools==70.0.0
     # via tensorboard
     # via tensorflow
 six==1.16.0
     # via astunparse
```

### Comparing `audioclass-0.1.0/scripts/process_directory.py` & `audioclass-0.1.1/scripts/process_directory.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/src/audioclass/data/perch/label.csv` & `audioclass-0.1.1/src/audioclass/data/perch/label.csv`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/src/audioclass/models/tflite.py` & `audioclass-0.1.1/src/audioclass/models/tflite.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""Module for defining TensorFlow Lite-based audio classification models.
+
+This module provides classes and functions for creating and using TensorFlow
+Lite models for audio classification tasks. It includes a `TFLiteModel` class
+that wraps a TensorFlow Lite interpreter and a `Signature` dataclass to define
+the model's input and output specifications.
+"""
+
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional
 
 import numpy as np
 from numpy.typing import DTypeLike
 from soundevent import data
@@ -15,70 +23,154 @@
     "Signature",
     "TFLiteModel",
 ]
 
 
 @dataclass
 class Signature:
+    """Defines the input and output signature of a TensorFlow Lite model."""
+
     input_index: int
+    """The index of the input tensor in the model."""
+
     classification_index: int
+    """The index of the tensor containing classification probabilities."""
+
     feature_index: int
+    """The index of the tensor containing extracted features."""
+
     input_length: int
+    """The number of audio samples expected in the input tensor."""
+
     input_dtype: DTypeLike = np.float32
+    """The data type of the input tensor. Defaults to np.float32."""
 
 
 class TFLiteModel(ClipClassificationModel):
+    """A wrapper class for TensorFlow Lite audio classification models.
+
+    This class provides a standardized interface for interacting with
+    TensorFlow Lite models, allowing them to be used seamlessly with the
+    audioclass library.
+    """
+
     interpreter: Interpreter
+    """The TensorFlow Lite interpreter object."""
+
     signature: Signature
+    """The input and output signature of the model."""
 
     def __init__(
         self,
         interpreter: Interpreter,
         signature: Signature,
         tags: List[data.Tag],
         confidence_threshold: float,
         samplerate: int,
         name: str,
         logits: bool = True,
     ):
+        """Initialize a TFLiteModel.
+
+        Parameters
+        ----------
+        interpreter
+            The TensorFlow Lite interpreter object.
+        signature
+            The input and output signature of the model.
+        tags
+            The list of tags that the model can predict.
+        confidence_threshold
+            The minimum confidence threshold for assigning a tag to a clip.
+        samplerate
+            The sample rate of the audio data expected by the model (in Hz).
+        name
+            The name of the model.
+        logits
+            Whether the model outputs logits (True) or probabilities (False).
+            Defaults to True.
+        """
         self.interpreter = interpreter
         self.tags = tags
         self.confidence_threshold = confidence_threshold
         self.samplerate = samplerate
         self.name = name
         self.signature = signature
         self.input_samples = signature.input_length
         self.num_classes = len(tags)
         self.logits = logits
 
         _validate_signature(self.interpreter, self.signature)
 
     def process_array(self, array: np.ndarray) -> ModelOutput:
+        """Process a single audio array and return the model output.
+
+        Parameters
+        ----------
+        array : np.ndarray
+            The audio array to be processed, with shape
+            `(num_frames, input_samples)`.
+
+        Returns
+        -------
+        ModelOutput
+            A `ModelOutput` object containing the class probabilities and
+            extracted features.
+        """
         return process_array(
             self.interpreter,
             self.signature,
             array,
             validate_signature=False,
             logits=self.logits,
         )
 
 
 def load_model(
     path: Path,
     num_threads: Optional[int] = None,
 ) -> Interpreter:
+    """
+    Load a TensorFlow Lite model from a file.
+
+    Parameters
+    ----------
+    path
+        The path to the TensorFlow Lite model file.
+    num_threads
+        The number of threads to use for inference. If None, the default number
+        of threads will be used.
+
+    Returns
+    -------
+    Interpreter
+        The TensorFlow Lite interpreter object.
+    """
     interpreter = Interpreter(model_path=str(path), num_threads=num_threads)
     interpreter.allocate_tensors()
     return interpreter
 
 
 def _validate_signature(
     interpreter: Interpreter, signature: Signature
 ) -> None:
-    """Validate the signature of a TF Lite model."""
+    """Validate the signature of a TF Lite model.
+
+    Parameters
+    ----------
+    interpreter
+        The TF Lite model interpreter.
+    signature
+        The input and output signature of the model.
+
+    Raises
+    ------
+    ValueError
+        If the model signature does not match the expected format.
+    """
     input_details = interpreter.get_input_details()
 
     if not len(input_details) == 1:
         raise ValueError("Model must have exactly one input tensor")
 
     input_details = input_details[0]
 
@@ -98,46 +190,42 @@
 def process_array(
     interpreter: Interpreter,
     signature: Signature,
     array: np.ndarray,
     validate_signature: bool = False,
     logits: bool = True,
 ) -> ModelOutput:
-    """Process a 2D array with a TF Lite model.
+    """Process an array with a TF Lite model.
 
     Parameters
     ----------
     interpreter
         The TF Lite model interpreter.
+    signature
+        The input and output signature of the model.
     array
-        An array of audio data with shape (n_samples) or (batch_size, n_samples).
-        The number of samples should match the input shape of the model which
-        by default is 144000.
+        The audio array to be processed, with shape (num_frames, input_samples)
+        or (input_samples,).
+    validate_signature
+        Whether to validate the model signature. Defaults to False.
+    logits
+        Whether the model outputs logits (True) or probabilities (False).
+        Defaults to True.
 
     Returns
     -------
-    class_probs
-        The probability of each class for each sample. This is stored
-        in a 2D array with shape (batch_size, n_classes). The values are
-        between 0 and 1. The value at index (i, j) is the probability that
-        the class j is present in the sample i. The probability scores
-        should be interpreted as the confidence of the model in the presence
-        of the class in the sample. Caution should be taken when interpreting
-        these values as probabilities.
-    features
-        The features extracted from the audio data. This is stored in a 2D
-        array with shape (batch_size, n_features). The features are extracted
-        from the last layer of the model and can be used for further analysis.
-        The default number of features is 1024.
+    ModelOutput
+        A `ModelOutput` object containing the class probabilities and extracted
+        features.
 
     Raises
     ------
     ValueError
-        If the input array does not have 2 dimensions or if the number of
-        samples does not match the input shape of the model.
+        If the input array has the wrong shape or if the model signature is
+        invalid.
     """
     if array.ndim == 1:
         array = array[np.newaxis, :]
 
     if not array.ndim == 2:
         raise ValueError("Input array must have 2 dimensions")
```

### Comparing `audioclass-0.1.0/tests/conftest.py` & `audioclass-0.1.1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,38 +4,14 @@
 from typing import Optional
 
 import numpy as np
 import pytest
 import soundfile as sf
 
 
-def pytest_addoption(parser):
-    parser.addoption(
-        "--runslow",
-        action="store_true",
-        default=False,
-        help="run slow tests",
-    )
-
-
-def pytest_configure(config):
-    config.addinivalue_line("markers", "slow: mark test as slow to run")
-
-
-def pytest_collection_modifyitems(config, items):
-    if config.getoption("--runslow"):
-        # --runslow given in cli: do not skip slow tests
-        return
-
-    skip_slow = pytest.mark.skip(reason="need --runslow option to run")
-    for item in items:
-        if "slow" in item.keywords:
-            item.add_marker(skip_slow)
-
-
 def random_string():
     """Generate a random string of fixed length."""
     options = string.ascii_uppercase + string.digits
     return "".join(random.choice(options) for _ in range(10))
 
 
 def write_random_wave(
```

### Comparing `audioclass-0.1.0/tests/test_postprocess.py` & `audioclass-0.1.1/tests/test_postprocess.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_preprocess.py` & `audioclass-0.1.1/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_utils.py` & `audioclass-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_batch/conftest.py` & `audioclass-0.1.1/tests/test_batch/conftest.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_batch/test_base.py` & `audioclass-0.1.1/tests/test_batch/test_base.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_batch/test_process.py` & `audioclass-0.1.1/tests/test_batch/test_process.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_batch/test_simple.py` & `audioclass-0.1.1/tests/test_batch/test_simple.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_batch/test_tensorflow.py` & `audioclass-0.1.1/tests/test_batch/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/tests/test_models/test_birdnet.py` & `audioclass-0.1.1/tests/test_models/test_birdnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,49 @@
 import datetime
 
 import numpy as np
-import pytest
 import xarray as xr
 from audioclass.models.birdnet import BirdNET
 from soundevent import data
 
 
-@pytest.mark.slow
 def test_can_instantiate_birdnet_model_from_model_files():
     model = BirdNET.load()
     assert isinstance(model, BirdNET)
 
 
-@pytest.mark.slow
 def test_birdnet_model_can_process_random_array():
     model = BirdNET.load(confidence_threshold=0)
     array = np.random.rand(1, 144000).astype(np.float32)
     results = model.process_array(array)
     class_probs, features = results
 
     assert isinstance(features, np.ndarray)
     assert isinstance(class_probs, np.ndarray)
     assert features.shape == (1, 1024)
     assert class_probs.shape == (1, 6522)
 
 
-@pytest.mark.slow
 def test_birdnet_model_can_process_file(random_wav_factory):
     model = BirdNET.load()
     path = random_wav_factory(duration=10)
     clip_predictions = model.process_file(path)
     assert len(clip_predictions) == 4
     assert all(isinstance(cp, data.ClipPrediction) for cp in clip_predictions)
 
 
-@pytest.mark.slow
 def test_birdnet_model_can_process_recording(random_wav_factory):
     model = BirdNET.load()
     path = random_wav_factory(duration=10)
     recording = data.Recording.from_file(path)
     clip_predictions = model.process_recording(recording)
     assert len(clip_predictions) == 4
     assert all(isinstance(cp, data.ClipPrediction) for cp in clip_predictions)
 
 
-@pytest.mark.slow
 def test_birdnet_model_can_process_clip(random_wav_factory):
     model = BirdNET.load()
     path = random_wav_factory(duration=10)
     clip = data.Clip(
         recording=data.Recording.from_file(path),
         start_time=1,
         end_time=4,
@@ -59,30 +53,28 @@
 
     clip_prediction = clip_predictions[0]
     assert isinstance(clip_prediction, data.ClipPrediction)
     assert clip_prediction.clip.start_time == 1
     assert clip_prediction.clip.end_time == 4
 
 
-@pytest.mark.slow
 def test_birdnet_process_clip_with_dataset_output(random_wav_factory):
     model = BirdNET.load()
     path = random_wav_factory(duration=10)
     clip = data.Clip(
         recording=data.Recording.from_file(path),
         start_time=1,
         end_time=4,
     )
     dataset = model.process_clip(clip, fmt="dataset")
     assert isinstance(dataset, xr.Dataset)
     assert "features" in dataset
     assert "probabilities" in dataset
 
 
-@pytest.mark.slow
 def test_birdnet_can_process_recording_with_metadata(random_wav_factory):
     model = BirdNET.load()
     path = random_wav_factory(duration=10)
     recording = data.Recording.from_file(
         path,
         latitude=0,
         longitude=0,
```

### Comparing `audioclass-0.1.0/tests/test_models/test_perch.py` & `audioclass-0.1.1/tests/test_models/test_perch.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,55 +8,50 @@
 
 
 @pytest.fixture(scope="module")
 def perch() -> Perch:
     return Perch.load()
 
 
-@pytest.mark.slow
 def test_loaded_perch_model_has_correct_signature(perch: Perch):
     assert perch.callable is not None
     assert perch.signature is not None
     assert perch.signature.input_length == 160_000
     assert perch.signature.input_dtype == np.float32
     assert perch.signature.input_name == "inputs"
     assert perch.signature.classification_name == "output_0"
     assert perch.signature.feature_name == "output_1"
 
 
-@pytest.mark.slow
 def test_perch_model_can_process_random_array(perch: Perch):
     array = np.random.rand(1, 160000).astype(np.float32)
     results = perch.process_array(array)
     class_probs, features = results
 
     assert isinstance(features, np.ndarray)
     assert isinstance(class_probs, np.ndarray)
     assert features.shape == (1, 1280)
     assert class_probs.shape == (1, 10932)
 
 
-@pytest.mark.slow
 def test_perch_model_can_process_file(random_wav_factory, perch: Perch):
     path = random_wav_factory(duration=10)
     clip_predictions = perch.process_file(path)
     assert len(clip_predictions) == 2
     assert all(isinstance(cp, data.ClipPrediction) for cp in clip_predictions)
 
 
-@pytest.mark.slow
 def test_perch_model_can_process_recording(random_wav_factory, perch: Perch):
     path = random_wav_factory(duration=10)
     recording = data.Recording.from_file(path)
     clip_predictions = perch.process_recording(recording)
     assert len(clip_predictions) == 2
     assert all(isinstance(cp, data.ClipPrediction) for cp in clip_predictions)
 
 
-@pytest.mark.slow
 def test_perch_model_can_process_clip(random_wav_factory, perch: Perch):
     path = random_wav_factory(duration=10)
     clip = data.Clip(
         recording=data.Recording.from_file(path),
         start_time=1,
         end_time=6,
     )
@@ -65,15 +60,14 @@
 
     clip_prediction = clip_predictions[0]
     assert isinstance(clip_prediction, data.ClipPrediction)
     assert clip_prediction.clip.start_time == 1
     assert clip_prediction.clip.end_time == 6
 
 
-@pytest.mark.slow
 def test_perch_process_clip_with_dataset_output(
     random_wav_factory, perch: Perch
 ):
     path = random_wav_factory(duration=10)
     clip = data.Clip(
         recording=data.Recording.from_file(path),
         start_time=1,
@@ -81,15 +75,14 @@
     )
     dataset = perch.process_clip(clip, fmt="dataset")
     assert isinstance(dataset, xr.Dataset)
     assert "features" in dataset
     assert "probabilities" in dataset
 
 
-@pytest.mark.slow
 def test_perch_can_process_recording_with_metadata(
     random_wav_factory, perch: Perch
 ):
     path = random_wav_factory(duration=10)
     recording = data.Recording.from_file(
         path,
         latitude=0,
```

### Comparing `audioclass-0.1.0/tests/test_models/test_tflite.py` & `audioclass-0.1.1/tests/test_models/test_tflite.py`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/.gitignore` & `audioclass-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/LICENCE` & `audioclass-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `audioclass-0.1.0/pyproject.toml` & `audioclass-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "audioclass"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package providing a common interface for running machine learning models for audio classification tasks."
 authors = [
     { name = "Santiago Martinez Balvanera", email = "santiago.mbal@gmail.com" },
 ]
 dependencies = [
     "pandas>=2.2.2",
     "netcdf4>=1.6.5",
     "soundevent[audio,array]>=2.0.0",
     "tqdm>=4.66.4",
     "pyarrow>=16.1.0",
     "requests>=2.32.2",
 ]
 readme = "README.md"
-requires-python = ">= 3.8"
+requires-python = ">= 3.9"
 license = { text = "MIT" }
 
 [project.optional-dependencies]
 tensorflow = ["tensorflow>=2.16.1", "tensorflow-hub>=0.16.1"]
 tflite = ["tflite>=2.10.0", "tflite-runtime>=2.14.0"]
 birdnet = ["audioclass[tflite]"]
 perch = ["audioclass[tensorflow]"]
@@ -39,32 +39,36 @@
 dev-dependencies = [
     "pytest>=8.2.1",
     "coverage>=7.5.3",
     "pytest-coverage>=0.0",
     "pytest-mock>=3.14.0",
     "ruff>=0.4.6",
     "pyright>=1.1.365",
+    "mkdocs>=1.6.0",
+    "mkdocstrings[python]>=0.25.1",
+    "mkdocs-material>=9.5.25",
 ]
 
 [tool.ruff]
 line-length = 79
-target-version = "py38"
+target-version = "py39"
 
 [tool.ruff.format]
 docstring-code-format = true
 docstring-code-line-length = 79
 
 [tool.ruff.lint]
-select = ["E4", "E7", "E9", "F", "B", "Q", "I"]
+select = ["E4", "E7", "E9", "F", "B", "Q", "I", "D"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.pyright]
 venvPath = "."
 venv = ".venv"
 exclude = [".venv"]
+pythonVersion = "3.9"
 
 [tool.coverage.run]
 branch = true
 source = ["src/audioclass"]
 command_line = "-m pytest"
```

