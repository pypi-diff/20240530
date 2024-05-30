# Comparing `tmp/sonusai_torchl-0.1.0.tar.gz` & `tmp/sonusai_torchl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonusai_torchl-0.1.0.tar", max compression
+gzip compressed data, was "sonusai_torchl-0.3.0.tar", max compression
```

## Comparing `sonusai_torchl-0.1.0.tar` & `sonusai_torchl-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       58 2024-05-08 20:21:31.497254 sonusai_torchl-0.1.0/README.rst
--rw-r--r--   0        0        0     1026 2024-05-10 21:49:54.121903 sonusai_torchl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      389 2024-05-10 15:52:59.561352 sonusai_torchl-0.1.0/sonusai_torchl/__init__.py
--rw-r--r--   0        0        0      153 2024-05-10 22:58:22.791377 sonusai_torchl-0.1.0/sonusai_torchl/data_generator/__init__.py
--rw-r--r--   0        0        0     4279 2023-12-07 22:54:59.048066 sonusai_torchl-0.1.0/sonusai_torchl/data_generator/torch_from_mixdb.py
--rw-r--r--   0        0        0     9036 2024-05-10 23:06:19.969954 sonusai_torchl-0.1.0/sonusai_torchl/torchl_onnx.py
--rw-r--r--   0        0        0    23023 2024-05-10 23:06:19.869564 sonusai_torchl-0.1.0/sonusai_torchl/torchl_predict.py
--rw-r--r--   0        0        0     9658 2024-05-10 23:06:19.965421 sonusai_torchl-0.1.0/sonusai_torchl/torchl_train.py
--rw-r--r--   0        0        0       49 2024-05-08 18:14:51.069971 sonusai_torchl-0.1.0/sonusai_torchl/utils/__init__.py
--rw-r--r--   0        0        0     4188 2024-05-07 22:48:42.411978 sonusai_torchl-0.1.0/sonusai_torchl/utils/torchl_utils.py
--rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 sonusai_torchl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      185 2024-05-30 18:39:48.085592 sonusai_torchl-0.3.0/README.rst
+-rw-r--r--   0        0        0     1080 2024-05-30 18:09:06.572241 sonusai_torchl-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      389 2024-05-21 04:22:48.062841 sonusai_torchl-0.3.0/sonusai_torchl/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-21 04:22:48.062841 sonusai_torchl-0.3.0/sonusai_torchl/data_generator/__init__.py
+-rw-r--r--   0        0        0     4279 2024-05-21 04:22:48.062841 sonusai_torchl-0.3.0/sonusai_torchl/data_generator/torch_from_mixdb.py
+-rw-r--r--   0        0        0     9036 2024-05-28 06:14:24.856712 sonusai_torchl-0.3.0/sonusai_torchl/torchl_onnx-old.py
+-rw-r--r--   0        0        0    15369 2024-05-30 17:47:45.542378 sonusai_torchl-0.3.0/sonusai_torchl/torchl_onnx.py
+-rw-r--r--   0        0        0    23023 2024-05-30 16:29:11.079234 sonusai_torchl-0.3.0/sonusai_torchl/torchl_predict.py
+-rw-r--r--   0        0        0     9658 2024-05-21 04:22:48.062841 sonusai_torchl-0.3.0/sonusai_torchl/torchl_train.py
+-rw-r--r--   0        0        0      232 2024-05-27 20:36:14.049226 sonusai_torchl-0.3.0/sonusai_torchl/utils/__init__.py
+-rw-r--r--   0        0        0    11860 2024-05-30 17:58:44.860127 sonusai_torchl-0.3.0/sonusai_torchl/utils/torchl_utils.py
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 sonusai_torchl-0.3.0/PKG-INFO
```

### Comparing `sonusai_torchl-0.1.0/pyproject.toml` & `sonusai_torchl-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sonusai-torchl"
-version = "0.1.0"
+version = "0.3.0"
 description = "PyTorch Lightning model tools for SonusAI"
 authors = ["Chris Eddington <chris@aaware.com>", "Jason Calderwood <jason@aaware.com>"]
 maintainers = ["Chris Eddington <chris@aaware.com>", "Jason Calderwood <jason@aaware.com>"]
 homepage = "https://aaware.com"
 license = "GPL-3.0-only"
 readme = "README.rst"
 
@@ -12,17 +12,20 @@
 docopt = "^0.6.2"
 h5py = "^3.11.0"
 lightning = "~2.2"
 numpy = "^1.26.4"
 pyaaware = "^1.5.7"
 python = ">=3.9,<3.12"
 pytorch-lightning = "^2.2.4"
-sonusai = ">=0.16.0"
+sonusai = ">=0.17.0"
 torch = "~2.2"
 torchinfo = "^1.8.0"
+onnxconverter-common = "^1.14.0"
+onnxsim = "^0.4.36"
+
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.0"
 mypy-extensions = "^1.0.0"
 pytest = "^8.1.1"
 
 [tool.mypy]
```

### Comparing `sonusai_torchl-0.1.0/sonusai_torchl/data_generator/torch_from_mixdb.py` & `sonusai_torchl-0.3.0/sonusai_torchl/data_generator/torch_from_mixdb.py`

 * *Files identical despite different names*

### Comparing `sonusai_torchl-0.1.0/sonusai_torchl/torchl_onnx.py` & `sonusai_torchl-0.3.0/sonusai_torchl/torchl_onnx-old.py`

 * *Files identical despite different names*

### Comparing `sonusai_torchl-0.1.0/sonusai_torchl/torchl_predict.py` & `sonusai_torchl-0.3.0/sonusai_torchl/torchl_predict.py`

 * *Files identical despite different names*

### Comparing `sonusai_torchl-0.1.0/sonusai_torchl/torchl_train.py` & `sonusai_torchl-0.3.0/sonusai_torchl/torchl_train.py`

 * *Files identical despite different names*

### Comparing `sonusai_torchl-0.1.0/PKG-INFO` & `sonusai_torchl-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonusai-torchl
-Version: 0.1.0
+Version: 0.3.0
 Summary: PyTorch Lightning model tools for SonusAI
 Home-page: https://aaware.com
 License: GPL-3.0-only
 Author: Chris Eddington
 Author-email: chris@aaware.com
 Maintainer: Chris Eddington
 Maintainer-email: chris@aaware.com
@@ -14,16 +14,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: h5py (>=3.11.0,<4.0.0)
 Requires-Dist: lightning (>=2.2,<2.3)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: onnxconverter-common (>=1.14.0,<2.0.0)
+Requires-Dist: onnxsim (>=0.4.36,<0.5.0)
 Requires-Dist: pyaaware (>=1.5.7,<2.0.0)
 Requires-Dist: pytorch-lightning (>=2.2.4,<3.0.0)
-Requires-Dist: sonusai (>=0.16.0)
+Requires-Dist: sonusai (>=0.17.0)
 Requires-Dist: torch (>=2.2,<2.3)
 Requires-Dist: torchinfo (>=1.8.0,<2.0.0)
 Description-Content-Type: text/x-rst
 
 SonusAI Torchl: PyTorch Lightning model tools for SonusAI
 
+
+Uses Poetry to manage and publish to Python PyPi.
+Note use poetry config pypi-token.pypi your-api-token, then poetry publish
+
```

