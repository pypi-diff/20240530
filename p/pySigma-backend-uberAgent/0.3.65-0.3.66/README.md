# Comparing `tmp/pysigma_backend_uberagent-0.3.65.tar.gz` & `tmp/pysigma_backend_uberagent-0.3.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_uberagent-0.3.65.tar", max compression
+gzip compressed data, was "pysigma_backend_uberagent-0.3.66.tar", max compression
```

## Comparing `pysigma_backend_uberagent-0.3.65.tar` & `pysigma_backend_uberagent-0.3.66.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/LICENSE
--rw-r--r--   0        0        0      573 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/pyproject.toml
--rw-r--r--   0        0        0       77 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/sigma/backends/uberagent/__init__.py
--rw-r--r--   0        0        0      320 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/sigma/backends/uberagent/exceptions.py
--rw-r--r--   0        0        0     6944 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/sigma/backends/uberagent/rule.py
--rw-r--r--   0        0        0    15338 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/sigma/backends/uberagent/uberagent.py
--rw-r--r--   0        0        0      411 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/__init__.py
--rw-r--r--   0        0        0     2503 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/condition.py
--rw-r--r--   0        0        0      969 2024-05-30 17:08:34.925018 pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/field.py
--rw-r--r--   0        0        0     1893 2024-05-30 17:08:34.929018 pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/logsource.py
--rw-r--r--   0        0        0     7909 2024-05-30 17:08:34.929018 pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/transformation.py
--rw-r--r--   0        0        0    26786 2024-05-30 17:08:34.929018 pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/uberagent.py
--rw-r--r--   0        0        0     6913 2024-05-30 17:08:34.929018 pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/version.py
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 pysigma_backend_uberagent-0.3.65/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/LICENSE
+-rw-r--r--   0        0        0      573 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/pyproject.toml
+-rw-r--r--   0        0        0       77 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/backends/uberagent/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/backends/uberagent/exceptions.py
+-rw-r--r--   0        0        0     6944 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/backends/uberagent/rule.py
+-rw-r--r--   0        0        0    15338 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/backends/uberagent/uberagent.py
+-rw-r--r--   0        0        0      462 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/__init__.py
+-rw-r--r--   0        0        0     2503 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/condition.py
+-rw-r--r--   0        0        0      969 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/field.py
+-rw-r--r--   0        0        0     1893 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/logsource.py
+-rw-r--r--   0        0        0     7909 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/transformation.py
+-rw-r--r--   0        0        0    27050 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/uberagent.py
+-rw-r--r--   0        0        0     6913 2024-05-30 17:17:07.089055 pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/version.py
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 pysigma_backend_uberagent-0.3.66/PKG-INFO
```

### Comparing `pysigma_backend_uberagent-0.3.65/LICENSE` & `pysigma_backend_uberagent-0.3.66/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/pyproject.toml` & `pysigma_backend_uberagent-0.3.66/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-uberAgent"
-version = "0.3.65"
+version = "0.3.66"
 description = "pySigma uAQL backend"
 authors = ["vast limits GmbH <info@vastlimits.com>"]
 license = "MIT"
 repository = "https://github.com/vastlimits/pySigma-backend-uberAgent"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/backends/uberagent/rule.py` & `pysigma_backend_uberagent-0.3.66/sigma/backends/uberagent/rule.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/backends/uberagent/uberagent.py` & `pysigma_backend_uberagent-0.3.66/sigma/backends/uberagent/uberagent.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/condition.py` & `pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/condition.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/field.py` & `pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/field.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/logsource.py` & `pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/logsource.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/transformation.py` & `pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/transformation.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/uberagent.py` & `pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/uberagent.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,14 +592,24 @@
 
     Returns:
     - ProcessingPipeline: The assembled processing pipeline for version 7.1.
     """
     return make_pipeline(Version(UA_VERSION_7_1))
 
 
+def uberagent720() -> ProcessingPipeline:
+    """
+    Create a processing pipeline for version 7.2 of uberAgent.
+
+    Returns:
+    - ProcessingPipeline: The assembled processing pipeline for version 7.2.
+    """
+    return make_pipeline(Version(UA_VERSION_7_2))
+
+
 def uberagent_develop() -> ProcessingPipeline:
     """
     Create a processing pipeline for the development version of uberAgent.
 
     Returns:
     - ProcessingPipeline: The assembled processing pipeline for the development version.
     """
```

### Comparing `pysigma_backend_uberagent-0.3.65/sigma/pipelines/uberagent/version.py` & `pysigma_backend_uberagent-0.3.66/sigma/pipelines/uberagent/version.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_uberagent-0.3.65/PKG-INFO` & `pysigma_backend_uberagent-0.3.66/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySigma-backend-uberAgent
-Version: 0.3.65
+Version: 0.3.66
 Summary: pySigma uAQL backend
 Home-page: https://github.com/vastlimits/pySigma-backend-uberAgent
 License: MIT
 Author: vast limits GmbH
 Author-email: info@vastlimits.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

