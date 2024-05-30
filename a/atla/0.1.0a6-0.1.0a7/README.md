# Comparing `tmp/atla-0.1.0a6.tar.gz` & `tmp/atla-0.1.0a7.tar.gz`

## Comparing `atla-0.1.0a6.tar` & `atla-0.1.0a7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/__init__.py
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_base_client.py
--rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_typing.py
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/lib/.keep
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/resources/__init__.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/resources/evaluate.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/types/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/types/evaluate_create_params.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 atla-0.1.0a6/src/atla/types/evaluation.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a6/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 atla-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_base_client.py
+-rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/lib/.keep
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/resources/__init__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/resources/evaluate.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/types/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/types/evaluate_create_params.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/types/evaluation.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a7/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 atla-0.1.0a7/PKG-INFO
```

### Comparing `atla-0.1.0a6/src/atla/__init__.py` & `atla-0.1.0a7/src/atla/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_base_client.py` & `atla-0.1.0a7/src/atla/_base_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_client.py` & `atla-0.1.0a7/src/atla/_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_compat.py` & `atla-0.1.0a7/src/atla/_compat.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_exceptions.py` & `atla-0.1.0a7/src/atla/_exceptions.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_files.py` & `atla-0.1.0a7/src/atla/_files.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_models.py` & `atla-0.1.0a7/src/atla/_models.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_qs.py` & `atla-0.1.0a7/src/atla/_qs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_resource.py` & `atla-0.1.0a7/src/atla/_resource.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_response.py` & `atla-0.1.0a7/src/atla/_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_streaming.py` & `atla-0.1.0a7/src/atla/_streaming.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_types.py` & `atla-0.1.0a7/src/atla/_types.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_utils/__init__.py` & `atla-0.1.0a7/src/atla/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_utils/_logs.py` & `atla-0.1.0a7/src/atla/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_utils/_proxy.py` & `atla-0.1.0a7/src/atla/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_utils/_sync.py` & `atla-0.1.0a7/src/atla/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_utils/_transform.py` & `atla-0.1.0a7/src/atla/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_utils/_typing.py` & `atla-0.1.0a7/src/atla/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/_utils/_utils.py` & `atla-0.1.0a7/src/atla/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/resources/__init__.py` & `atla-0.1.0a7/src/atla/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/resources/evaluate.py` & `atla-0.1.0a7/src/atla/resources/evaluate.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/types/evaluate_create_params.py` & `atla-0.1.0a7/src/atla/types/evaluate_create_params.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/src/atla/types/evaluation.py` & `atla-0.1.0a7/src/atla/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/LICENSE` & `atla-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a6/pyproject.toml` & `atla-0.1.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atla"
-version = "0.1.0-alpha.6"
+version = "0.1.0-alpha.7"
 description = "The official Python library for the atla API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Atla", email = "support@atla.com" },
 ]
 dependencies = [
```

