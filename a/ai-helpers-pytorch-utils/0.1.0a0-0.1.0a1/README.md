# Comparing `tmp/ai_helpers_pytorch_utils-0.1.0a0.tar.gz` & `tmp/ai_helpers_pytorch_utils-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_helpers_pytorch_utils-0.1.0a0.tar", max compression
+gzip compressed data, was "ai_helpers_pytorch_utils-0.1.0a1.tar", max compression
```

## Comparing `ai_helpers_pytorch_utils-0.1.0a0.tar` & `ai_helpers_pytorch_utils-0.1.0a1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1354 2024-05-29 16:01:17.853246 ai_helpers_pytorch_utils-0.1.0a0/README.md
--rw-r--r--   0        0        0     1741 2024-05-29 16:11:05.224106 ai_helpers_pytorch_utils-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      346 2024-05-29 15:51:49.135524 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/__init__.py
--rw-r--r--   0        0        0    21052 2024-05-29 15:46:06.696072 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/data_modules.py
--rw-r--r--   0        0        0    25561 2024-05-29 15:49:29.159494 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/dataset_configurations.py
--rw-r--r--   0        0        0     8296 2024-05-29 15:56:24.504659 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/datasets.py
--rw-r--r--   0        0        0     3004 2024-05-29 15:56:24.503610 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/exceptions.py
--rw-r--r--   0        0        0     7421 2024-05-29 16:00:29.119810 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/logging/loggers.py
--rw-r--r--   0        0        0      845 2024-05-29 16:00:29.118924 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/logging/utils.py
--rw-r--r--   0        0        0      369 2024-05-29 15:46:06.693683 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/miscellaneous.py
--rw-r--r--   0        0        0    39046 2024-05-29 15:46:06.697976 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/modules.py
--rw-r--r--   0        0        0     5410 2024-05-29 15:46:06.694512 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/pandas/data_formatting.py
--rw-r--r--   0        0        0     4837 2024-05-29 15:46:06.694390 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/pandas/utils.py
--rw-r--r--   0        0        0     3856 2024-05-29 15:46:06.694054 ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/utils.py
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 ai_helpers_pytorch_utils-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1334 2024-05-30 12:07:19.966780 ai_helpers_pytorch_utils-0.1.0a1/README.md
+-rw-r--r--   0        0        0     2042 2024-05-30 12:07:19.966780 ai_helpers_pytorch_utils-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/__init__.py
+-rw-r--r--   0        0        0    21052 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/data_modules.py
+-rw-r--r--   0        0        0    25561 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/dataset_configurations.py
+-rw-r--r--   0        0        0     8296 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/datasets.py
+-rw-r--r--   0        0        0     3004 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/exceptions.py
+-rw-r--r--   0        0        0     7421 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/logging/loggers.py
+-rw-r--r--   0        0        0      845 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/logging/utils.py
+-rw-r--r--   0        0        0     9950 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/metrics.py
+-rw-r--r--   0        0        0      369 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/miscellaneous.py
+-rw-r--r--   0        0        0    39046 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/modules.py
+-rw-r--r--   0        0        0     5410 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/pandas/data_formatting.py
+-rw-r--r--   0        0        0     4837 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/pandas/utils.py
+-rw-r--r--   0        0        0     3856 2024-05-30 12:07:19.970780 ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/utils.py
+-rw-r--r--   0        0        0     2286 1970-01-01 00:00:00.000000 ai_helpers_pytorch_utils-0.1.0a1/PKG-INFO
```

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/README.md` & `ai_helpers_pytorch_utils-0.1.0a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# AI Helpers - Pytorch Utils
+# AI Helpers - PyTorch Utils
 
 `pytorch-utils` is a Python module that provides a collection of utilities to simplify and enhance the use of PyTorch. These utilities are designed to make working with PyTorch more efficient and to reduce boilerplate code.
 
-> TODO: tests & export logging
-
 ## Table of Contents
 
-- [AI Helpers - Pytorch Utils](#ai-helpers---pytorch-utils)
+- [AI Helpers - PyTorch Utils](#ai-helpers---pytorch-utils)
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Getting Started](#getting-started)
   - [Utilities](#utilities)
   - [Examples](#examples)
   - [Contributing](#contributing)
 
 ## Installation
 
-You can install the `pytorch-utils` module via pip:
+You can install the `ai-helpers-pytorch-utils` module via pip:
 
 ```bash
 pip install pytorch-utils
 ```
 
 ## Getting Started
 
@@ -45,8 +43,8 @@
 1. Fork the repository.
 2. Create a new branch (`git checkout -b feature-branch`).
 3. Make your changes.
 4. Commit your changes (`git commit -am 'Add some feature'`).
 5. Push to the branch (`git push origin feature-branch`).
 6. Create a new Pull Request.
 
-Please ensure your code follows the project's coding standards and includes appropriate tests.
+Please ensure your code follows the project's coding standards and includes appropriate tests.
```

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pyproject.toml` & `ai_helpers_pytorch_utils-0.1.0a1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 [tool.poetry]
 name = "ai-helpers-pytorch-utils"
-version = "0.1.0a0"
-description = "Common pytorch utils"
+version = "0.1.0a1"
+description = "Common PyTorch utils"
 authors = ["Corentin Vasseur <vasseur.corentin@gmail.com>"]
 packages = [{ include = "pytorch_utils" }]
 readme = "README.md"
+repository = "https://github.com/ai-helpers/pytorch-utils"
+documentation = "https://ai-helpers.github.io/pytorch-utils/"
+keywords = ["machine-learning", "pytorch", "utils"]
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.11"
 pytorch-lightning = "^2.1.3"
 scikit-learn = "1.3.2"
 pandas = "2.0.3" 
 numpy = "1.26.4"
 plotly = "^5.14.1"
 torchinfo = "^1.8.0"
 torch = "2.2.2"
+mlflow = "^2.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.4.3"
 mypy = "^1.9.0"
 ruff = "^0.3.3"
 setuptools = "^70.0.0"
 types-setuptools = "^70.0.0.20240524"
 bandit = "^1.7.8"
 pytest-xdist = "^3.6.1"
 pytest-cov = "^5.0.0"
+hypothesis = "^6.103.0"
 
 [tool.poetry.group.documenters.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 
 [tool.poetry.group.publishers.dependencies]
 twine = "^5.0.0"
```

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/data_modules.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/data_modules.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/dataset_configurations.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/dataset_configurations.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/datasets.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/exceptions.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/logging/loggers.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/logging/loggers.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/logging/utils.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/logging/utils.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/modules.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/modules.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/pandas/data_formatting.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/pandas/data_formatting.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/pandas/utils.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/pytorch_utils/utils.py` & `ai_helpers_pytorch_utils-0.1.0a1/pytorch_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_pytorch_utils-0.1.0a0/PKG-INFO` & `ai_helpers_pytorch_utils-0.1.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: ai-helpers-pytorch-utils
-Version: 0.1.0a0
-Summary: Common pytorch utils
+Version: 0.1.0a1
+Summary: Common PyTorch utils
+Home-page: https://github.com/ai-helpers/pytorch-utils
+Keywords: machine-learning,pytorch,utils
 Author: Corentin Vasseur
 Author-email: vasseur.corentin@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: mlflow (>=2.13.0,<3.0.0)
 Requires-Dist: numpy (==1.26.4)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: pytorch-lightning (>=2.1.3,<3.0.0)
 Requires-Dist: scikit-learn (==1.3.2)
 Requires-Dist: torch (==2.2.2)
 Requires-Dist: torchinfo (>=1.8.0,<2.0.0)
+Project-URL: Documentation, https://ai-helpers.github.io/pytorch-utils/
+Project-URL: Repository, https://github.com/ai-helpers/pytorch-utils
 Description-Content-Type: text/markdown
 
-# AI Helpers - Pytorch Utils
+# AI Helpers - PyTorch Utils
 
 `pytorch-utils` is a Python module that provides a collection of utilities to simplify and enhance the use of PyTorch. These utilities are designed to make working with PyTorch more efficient and to reduce boilerplate code.
 
-> TODO: tests & export logging
-
 ## Table of Contents
 
-- [AI Helpers - Pytorch Utils](#ai-helpers---pytorch-utils)
+- [AI Helpers - PyTorch Utils](#ai-helpers---pytorch-utils)
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Getting Started](#getting-started)
   - [Utilities](#utilities)
   - [Examples](#examples)
   - [Contributing](#contributing)
 
 ## Installation
 
-You can install the `pytorch-utils` module via pip:
+You can install the `ai-helpers-pytorch-utils` module via pip:
 
 ```bash
 pip install pytorch-utils
 ```
 
 ## Getting Started
 
@@ -64,7 +68,8 @@
 2. Create a new branch (`git checkout -b feature-branch`).
 3. Make your changes.
 4. Commit your changes (`git commit -am 'Add some feature'`).
 5. Push to the branch (`git push origin feature-branch`).
 6. Create a new Pull Request.
 
 Please ensure your code follows the project's coding standards and includes appropriate tests.
+
```

