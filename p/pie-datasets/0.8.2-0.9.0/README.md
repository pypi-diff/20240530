# Comparing `tmp/pie_datasets-0.8.2.tar.gz` & `tmp/pie_datasets-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pie_datasets-0.8.2.tar", max compression
+gzip compressed data, was "pie_datasets-0.9.0.tar", max compression
```

## Comparing `pie_datasets-0.8.2.tar` & `pie_datasets-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1067 2024-02-20 10:39:02.231224 pie_datasets-0.8.2/LICENSE
--rw-r--r--   0        0        0    16610 2024-02-20 10:39:02.231224 pie_datasets-0.8.2/README.md
--rw-r--r--   0        0        0     1845 2024-02-20 10:39:14.631294 pie_datasets-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       36 2024-02-20 10:39:02.247224 pie_datasets-0.8.2/src/pie_datasets/__init__.py
--rw-r--r--   0        0        0       42 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/builders/__init__.py
--rw-r--r--   0        0        0    12725 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/builders/brat.py
--rw-r--r--   0        0        0      306 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/core/__init__.py
--rw-r--r--   0        0        0    12178 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/core/builder.py
--rw-r--r--   0        0        0    20816 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/core/dataset.py
--rw-r--r--   0        0        0    29425 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/core/dataset_dict.py
--rw-r--r--   0        0        0      823 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/core/document_formatter.py
--rw-r--r--   0        0        0        0 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/document/__init__.py
--rw-r--r--   0        0        0       49 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/document/processing/__init__.py
--rw-r--r--   0        0        0     2136 2024-02-20 10:39:02.251224 pie_datasets-0.8.2/src/pie_datasets/document/processing/generic.py
--rw-r--r--   0        0        0    17567 1970-01-01 00:00:00.000000 pie_datasets-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-21 21:26:38.638465 pie_datasets-0.9.0/LICENSE
+-rw-r--r--   0        0        0    16610 2024-03-21 21:26:38.638465 pie_datasets-0.9.0/README.md
+-rw-r--r--   0        0        0     1864 2024-03-21 21:26:50.098468 pie_datasets-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-03-21 21:26:38.654465 pie_datasets-0.9.0/src/pie_datasets/__init__.py
+-rw-r--r--   0        0        0       42 2024-03-21 21:26:38.654465 pie_datasets-0.9.0/src/pie_datasets/builders/__init__.py
+-rw-r--r--   0        0        0    12726 2024-03-21 21:26:38.654465 pie_datasets-0.9.0/src/pie_datasets/builders/brat.py
+-rw-r--r--   0        0        0      306 2024-03-21 21:26:38.654465 pie_datasets-0.9.0/src/pie_datasets/core/__init__.py
+-rw-r--r--   0        0        0    12178 2024-03-21 21:26:38.654465 pie_datasets-0.9.0/src/pie_datasets/core/builder.py
+-rw-r--r--   0        0        0    20816 2024-03-21 21:26:38.658465 pie_datasets-0.9.0/src/pie_datasets/core/dataset.py
+-rw-r--r--   0        0        0    29425 2024-03-21 21:26:38.658465 pie_datasets-0.9.0/src/pie_datasets/core/dataset_dict.py
+-rw-r--r--   0        0        0      823 2024-03-21 21:26:38.658465 pie_datasets-0.9.0/src/pie_datasets/core/document_formatter.py
+-rw-r--r--   0        0        0        0 2024-03-21 21:26:38.658465 pie_datasets-0.9.0/src/pie_datasets/document/__init__.py
+-rw-r--r--   0        0        0       49 2024-03-21 21:26:38.658465 pie_datasets-0.9.0/src/pie_datasets/document/processing/__init__.py
+-rw-r--r--   0        0        0     2136 2024-03-21 21:26:38.658465 pie_datasets-0.9.0/src/pie_datasets/document/processing/generic.py
+-rw-r--r--   0        0        0    17567 1970-01-01 00:00:00.000000 pie_datasets-0.9.0/PKG-INFO
```

### Comparing `pie_datasets-0.8.2/LICENSE` & `pie_datasets-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pie_datasets-0.8.2/README.md` & `pie_datasets-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pie_datasets-0.8.2/pyproject.toml` & `pie_datasets-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pie-datasets"
-version = "0.8.2"
+version = "0.9.0"
 description = "Building scripts for PyTorch-IE Datasets"
 authors = ["Arne Binder <arne.binder@dfki.de>"]
 readme = "README.md"
 homepage = "https://github.com/arnebinder/pie-datasets"
 repository = "https://github.com/arnebinder/pie-datasets"
 packages = [
     { include = "pie_datasets", from = "src" },
@@ -20,22 +20,22 @@
 ]
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/arnebinder/pie-datasets/issues"
 "Changelog" = "https://github.com/arnebinder/pie-datasets/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pytorch-ie = "^0.29.2"
+pytorch-ie = ">=0.29.4,<0.31.0"
 # <2.16.0 because of https://github.com/ArneBinder/pie-datasets/issues/93
 datasets = ">=2.14.0,<2.16.0"
 # this was manually added because we get a conflict with pyarrow otherwise
 pyarrow = "^13"
 
 [tool.poetry.group.dev.dependencies]
-pie-modules = "^0.8.3"
+pie-modules = ">=0.10.8,<0.12.0"
 torch = {version = "^2.1.0+cpu", source = "pytorch"}
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.4.0"
 
 [[tool.poetry.source]]
 name = "pytorch"
```

### Comparing `pie_datasets-0.8.2/src/pie_datasets/builders/brat.py` & `pie_datasets-0.9.0/src/pie_datasets/builders/brat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 import logging
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import datasets
-from pytorch_ie.annotations import BinaryRelation, LabeledMultiSpan, LabeledSpan
+from pie_modules.annotations import BinaryRelation, LabeledMultiSpan, LabeledSpan
 from pytorch_ie.core import Annotation, AnnotationList, annotation_field
 from pytorch_ie.documents import TextBasedDocument
 
 from pie_datasets import GeneratorBasedBuilder
 
 logger = logging.getLogger(__name__)
```

### Comparing `pie_datasets-0.8.2/src/pie_datasets/core/builder.py` & `pie_datasets-0.9.0/src/pie_datasets/core/builder.py`

 * *Files identical despite different names*

### Comparing `pie_datasets-0.8.2/src/pie_datasets/core/dataset.py` & `pie_datasets-0.9.0/src/pie_datasets/core/dataset.py`

 * *Files identical despite different names*

### Comparing `pie_datasets-0.8.2/src/pie_datasets/core/dataset_dict.py` & `pie_datasets-0.9.0/src/pie_datasets/core/dataset_dict.py`

 * *Files identical despite different names*

### Comparing `pie_datasets-0.8.2/src/pie_datasets/core/document_formatter.py` & `pie_datasets-0.9.0/src/pie_datasets/core/document_formatter.py`

 * *Files identical despite different names*

### Comparing `pie_datasets-0.8.2/src/pie_datasets/document/processing/generic.py` & `pie_datasets-0.9.0/src/pie_datasets/document/processing/generic.py`

 * *Files identical despite different names*

### Comparing `pie_datasets-0.8.2/PKG-INFO` & `pie_datasets-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pie-datasets
-Version: 0.8.2
+Version: 0.9.0
 Summary: Building scripts for PyTorch-IE Datasets
 Home-page: https://github.com/arnebinder/pie-datasets
 Author: Arne Binder
 Author-email: arne.binder@dfki.de
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: datasets (>=2.14.0,<2.16.0)
 Requires-Dist: pyarrow (>=13,<14)
-Requires-Dist: pytorch-ie (>=0.29.2,<0.30.0)
+Requires-Dist: pytorch-ie (>=0.29.4,<0.31.0)
 Project-URL: Bug Tracker, https://github.com/arnebinder/pie-datasets/issues
 Project-URL: Changelog, https://github.com/arnebinder/pie-datasets/releases
 Project-URL: Repository, https://github.com/arnebinder/pie-datasets
 Description-Content-Type: text/markdown
 
 # pie-datasets
```

