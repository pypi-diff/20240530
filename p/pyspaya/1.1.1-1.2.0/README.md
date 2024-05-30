# Comparing `tmp/pyspaya-1.1.1.tar.gz` & `tmp/pyspaya-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspaya-1.1.1.tar", max compression
+gzip compressed data, was "pyspaya-1.2.0.tar", max compression
```

## Comparing `pyspaya-1.1.1.tar` & `pyspaya-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2024-03-05 15:00:43.912172 pyspaya-1.1.1/LICENSE
--rw-r--r--   0        0        0     6345 2024-03-05 15:00:43.912172 pyspaya-1.1.1/README.md
--rw-r--r--   0        0        0      257 2024-03-05 15:00:43.912172 pyspaya-1.1.1/iktos/__init__.py
--rw-r--r--   0        0        0      953 2024-03-05 15:00:43.912172 pyspaya-1.1.1/iktos/spaya/__init__.py
--rw-r--r--   0        0        0     1101 2024-03-05 15:00:43.912172 pyspaya-1.1.1/iktos/spaya/authorization.py
--rw-r--r--   0        0        0    24566 2024-03-05 15:00:43.912172 pyspaya-1.1.1/iktos/spaya/model.py
--rw-r--r--   0        0        0        0 2024-03-05 15:00:43.912172 pyspaya-1.1.1/iktos/spaya/py.typed
--rw-r--r--   0        0        0    23117 2024-03-05 15:00:43.916172 pyspaya-1.1.1/iktos/spaya/spaya_client.py
--rw-r--r--   0        0        0    19909 2024-03-05 15:00:43.916172 pyspaya-1.1.1/iktos/spaya/spaya_client_async.py
--rw-r--r--   0        0        0     7498 2024-03-05 15:00:43.916172 pyspaya-1.1.1/iktos/spaya/spaya_client_callback.py
--rw-r--r--   0        0        0    18601 2024-03-05 15:00:43.916172 pyspaya-1.1.1/iktos/spaya/spaya_client_rest.py
--rw-r--r--   0        0        0     1448 2024-03-05 15:00:43.916172 pyspaya-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6919 1970-01-01 00:00:00.000000 pyspaya-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-30 12:17:15.948412 pyspaya-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6345 2024-05-30 12:17:15.948412 pyspaya-1.2.0/README.md
+-rw-r--r--   0        0        0      257 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/authorization.py
+-rw-r--r--   0        0        0    24837 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/model.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/py.typed
+-rw-r--r--   0        0        0    23117 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/spaya_client.py
+-rw-r--r--   0        0        0    19909 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/spaya_client_async.py
+-rw-r--r--   0        0        0     7498 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/spaya_client_callback.py
+-rw-r--r--   0        0        0    18601 2024-05-30 12:17:15.948412 pyspaya-1.2.0/iktos/spaya/spaya_client_rest.py
+-rw-r--r--   0        0        0     1448 2024-05-30 12:17:15.948412 pyspaya-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6919 1970-01-01 00:00:00.000000 pyspaya-1.2.0/PKG-INFO
```

### Comparing `pyspaya-1.1.1/LICENSE` & `pyspaya-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/README.md` & `pyspaya-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/iktos/spaya/__init__.py` & `pyspaya-1.2.0/iktos/spaya/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/iktos/spaya/authorization.py` & `pyspaya-1.2.0/iktos/spaya/authorization.py`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/iktos/spaya/model.py` & `pyspaya-1.2.0/iktos/spaya/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 
 class RetrosynthesisParameters:
     """
     Parameters for a retrosynthesis
     """
 
     __slots__: List[str] = [
+        "model",
         "max_depth",
         "max_nb_iterations",
         "early_stopping_score",
         "early_stopping_timeout",
         "intermediate_smiles",
         "imposed_structures",
         "forbidden_structures",
@@ -225,14 +226,15 @@
         "name_reactions_exclude",
         "name_reactions_at_least",
         "filter_regio_issues",
     ]
 
     def __init__(
         self,
+        model: Optional[str] = None,
         max_depth: Optional[int] = None,
         max_nb_iterations: Optional[int] = None,
         early_stopping_score: Optional[float] = None,
         early_stopping_timeout: Optional[float] = None,
         intermediate_smiles: Optional[List[str]] = None,
         imposed_structures: Optional[List[str]] = None,
         forbidden_structures: Optional[List[str]] = None,
@@ -246,14 +248,15 @@
         name_reactions_only: Optional[List[str]] = None,
         name_reactions_exclude: Optional[List[str]] = None,
         name_reactions_at_least: Optional[List[str]] = None,
         filter_regio_issues: Optional[bool] = None,
     ):
         """
         Args:
+            model: Spaya's retrosynthesis engine (model) version to use
             max_depth: Maximum route depth
             max_nb_iterations: Maximum number of steps
             early_stopping_score: Score threshold to stop the retrosynthesis of a SMILES
             early_stopping_timeout: Timeout to stop the retrosynthesis of a SMILES
              in minutes
             intermediate_smiles: Desired intermediate products (as a list of SMILES).
              This will force our models to only find routes which have at least one of
@@ -273,14 +276,15 @@
             cc_extra_compounds_smiles: A list of smiles to add as commercial compounds
             remove_chirality : When True, remove the chirality from all inputs
             name_reactions_only: List of allowed name reactions
             name_reactions_exclude: List of excluded name reactions
             name_reactions_at_least: List of mandatory name reactions
             filter_regio_issues: When True, disables the regioselectivity
         """
+        self.model = model
         self.max_depth = max_depth
         self.max_nb_iterations = max_nb_iterations
         self.early_stopping_score = early_stopping_score
         self.early_stopping_timeout = early_stopping_timeout
         self.intermediate_smiles = intermediate_smiles
         self.forbidden_structures = forbidden_structures
         self.imposed_structures = imposed_structures
@@ -298,14 +302,16 @@
 
     def to_dict(self) -> Dict:
         """
         Returns:
             A dictionary for serialization
         """
         result: Dict[str, Union[int, float, str, List[str], List[int]]] = dict()
+        if self.model is not None:
+            result["model"] = self.model
         if self.max_depth is not None:
             result["max_depth"] = self.max_depth
         if self.max_nb_iterations is not None:
             result["max_nb_iterations"] = self.max_nb_iterations
         if self.early_stopping_score is not None:
             result["early_stopping_score"] = self.early_stopping_score
         if self.early_stopping_timeout is not None:
@@ -355,15 +361,16 @@
         Args:
             other: other parameters to compare with
 
         Returns:
             True if all parameters others than timing restriction are equal
         """
         return (
-            self.max_depth == other.max_depth
+            self.model == other.model
+            and self.max_depth == other.max_depth
             and self.early_stopping_score == other.early_stopping_score
             and self.intermediate_smiles == other.intermediate_smiles
             and self.imposed_structures == other.imposed_structures
             and self.forbidden_structures == other.forbidden_structures
             and self.first_disconnections == other.first_disconnections
             and self.cc_providers == other.cc_providers
             and self.cc_max_price_per_g == other.cc_max_price_per_g
```

### Comparing `pyspaya-1.1.1/iktos/spaya/spaya_client.py` & `pyspaya-1.2.0/iktos/spaya/spaya_client.py`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/iktos/spaya/spaya_client_async.py` & `pyspaya-1.2.0/iktos/spaya/spaya_client_async.py`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/iktos/spaya/spaya_client_callback.py` & `pyspaya-1.2.0/iktos/spaya/spaya_client_callback.py`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/iktos/spaya/spaya_client_rest.py` & `pyspaya-1.2.0/iktos/spaya/spaya_client_rest.py`

 * *Files identical despite different names*

### Comparing `pyspaya-1.1.1/pyproject.toml` & `pyspaya-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyspaya"
-version = "1.1.1"
+version = "1.2.0"
 description = "Python client for Spaya"
 authors = ["Iktos"]
 readme = "README.md"
 packages = [
     { include = "iktos" },
     { include = "iktos/**/*.py" },
 ]
```

### Comparing `pyspaya-1.1.1/PKG-INFO` & `pyspaya-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspaya
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python client for Spaya
 Author: Iktos
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

