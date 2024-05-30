# Comparing `tmp/kyoslib_py-5.1.1.tar.gz` & `tmp/kyoslib_py-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyoslib_py-5.1.1.tar", max compression
+gzip compressed data, was "kyoslib_py-5.2.0.tar", max compression
```

## Comparing `kyoslib_py-5.1.1.tar` & `kyoslib_py-5.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-04-15 08:11:17.960159 kyoslib_py-5.1.1/LICENSE.txt
--rw-r--r--   0        0        0      945 2024-04-15 08:11:17.960159 kyoslib_py-5.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/__init__.py
--rw-r--r--   0        0        0    10927 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/forward_curve.py
--rw-r--r--   0        0        0    15661 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/front_end.py
--rw-r--r--   0        0        0    24439 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/historical_price.py
--rw-r--r--   0        0        0     3459 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/kyos_api.py
--rw-r--r--   0        0        0     4554 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/kyos_utils.py
--rw-r--r--   0        0        0    45398 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/settings.py
--rw-r--r--   0        0        0    94919 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/simulation.py
--rw-r--r--   0        0        0    21239 2024-04-15 08:11:17.964159 kyoslib_py-5.1.1/kyoslib_py/tradable_product.py
--rw-r--r--   0        0        0    36070 2024-04-15 08:11:17.968159 kyoslib_py-5.1.1/kyoslib_py/valuation_interface.py
--rw-r--r--   0        0        0     1116 2024-04-15 08:11:17.968159 kyoslib_py-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 kyoslib_py-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-30 13:24:49.767453 kyoslib_py-5.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      945 2024-05-30 13:24:49.767453 kyoslib_py-5.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 13:24:49.771453 kyoslib_py-5.2.0/kyoslib_py/__init__.py
+-rw-r--r--   0        0        0    10927 2024-05-30 13:24:49.771453 kyoslib_py-5.2.0/kyoslib_py/forward_curve.py
+-rw-r--r--   0        0        0    15661 2024-05-30 13:24:49.771453 kyoslib_py-5.2.0/kyoslib_py/front_end.py
+-rw-r--r--   0        0        0    24439 2024-05-30 13:24:49.771453 kyoslib_py-5.2.0/kyoslib_py/historical_price.py
+-rw-r--r--   0        0        0     3459 2024-05-30 13:24:49.771453 kyoslib_py-5.2.0/kyoslib_py/kyos_api.py
+-rw-r--r--   0        0        0     6170 2024-05-30 13:24:49.771453 kyoslib_py-5.2.0/kyoslib_py/kyos_utils.py
+-rw-r--r--   0        0        0    45398 2024-05-30 13:24:49.771453 kyoslib_py-5.2.0/kyoslib_py/settings.py
+-rw-r--r--   0        0        0    94919 2024-05-30 13:24:49.775453 kyoslib_py-5.2.0/kyoslib_py/simulation.py
+-rw-r--r--   0        0        0    21239 2024-05-30 13:24:49.775453 kyoslib_py-5.2.0/kyoslib_py/tradable_product.py
+-rw-r--r--   0        0        0    36070 2024-05-30 13:24:49.775453 kyoslib_py-5.2.0/kyoslib_py/valuation_interface.py
+-rw-r--r--   0        0        0     1136 2024-05-30 13:24:49.775453 kyoslib_py-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 kyoslib_py-5.2.0/PKG-INFO
```

### Comparing `kyoslib_py-5.1.1/LICENSE.txt` & `kyoslib_py-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/README.md` & `kyoslib_py-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/forward_curve.py` & `kyoslib_py-5.2.0/kyoslib_py/forward_curve.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/front_end.py` & `kyoslib_py-5.2.0/kyoslib_py/front_end.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/historical_price.py` & `kyoslib_py-5.2.0/kyoslib_py/historical_price.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/kyos_api.py` & `kyoslib_py-5.2.0/kyoslib_py/kyos_api.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/settings.py` & `kyoslib_py-5.2.0/kyoslib_py/settings.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/simulation.py` & `kyoslib_py-5.2.0/kyoslib_py/simulation.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/tradable_product.py` & `kyoslib_py-5.2.0/kyoslib_py/tradable_product.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/kyoslib_py/valuation_interface.py` & `kyoslib_py-5.2.0/kyoslib_py/valuation_interface.py`

 * *Files identical despite different names*

### Comparing `kyoslib_py-5.1.1/pyproject.toml` & `kyoslib_py-5.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kyoslib_py"
-version = "5.1.1"
+version = "5.2.0"
 description = "KYOS shared lib code as python package"
 authors = ["KYOS <support@kyos.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/kyosenergy/kyoslib_py"
 documentation = "https://kyosenergy.github.io/kyoslib_py/"
 
@@ -13,24 +13,25 @@
 numpy = "^1.24.4"
 pandas = "<2.0.0"
 requests = "^2.31.0"
 h5py = "^3.9.0"
 numba = ">=0.57.1,<0.60.0"
 plotly = "^5.16.1"
 mkdocstrings-python = "^1.7.0"
+postmarker = "^1.0"
 
 [tool.poetry.group.dev.dependencies]
 invoke = "^2.2.0"
 pytest = ">=7.4.2,<9.0.0"
 pytest-cov = ">=4.1,<6.0"
 black = ">=23.9.1,<25.0.0"
 isort = "^5.12.0"
 safety = ">=2.3.5,<4.0.0"
 mkdocs-material = "^9.3.1"
-mkdocstrings = ">=0.23,<0.25"
+mkdocstrings = ">=0.23,<0.26"
 darglint = "^1.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `kyoslib_py-5.1.1/PKG-INFO` & `kyoslib_py-5.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kyoslib_py
-Version: 5.1.1
+Version: 5.2.0
 Summary: KYOS shared lib code as python package
 Home-page: http://github.com/kyosenergy/kyoslib_py
 License: MIT
 Author: KYOS
 Author-email: support@kyos.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: h5py (>=3.9.0,<4.0.0)
 Requires-Dist: mkdocstrings-python (>=1.7.0,<2.0.0)
 Requires-Dist: numba (>=0.57.1,<0.60.0)
 Requires-Dist: numpy (>=1.24.4,<2.0.0)
 Requires-Dist: pandas (<2.0.0)
 Requires-Dist: plotly (>=5.16.1,<6.0.0)
+Requires-Dist: postmarker (>=1.0,<2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://kyosenergy.github.io/kyoslib_py/
 Project-URL: Repository, http://github.com/kyosenergy/kyoslib_py
 Description-Content-Type: text/markdown
 
 # kyoslib_py
```

