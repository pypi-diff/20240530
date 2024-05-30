# Comparing `tmp/ai_helpers_jax_utils-0.1.0a0.tar.gz` & `tmp/ai_helpers_jax_utils-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_helpers_jax_utils-0.1.0a0.tar", max compression
+gzip compressed data, was "ai_helpers_jax_utils-0.1.0a1.tar", max compression
```

## Comparing `ai_helpers_jax_utils-0.1.0a0.tar` & `ai_helpers_jax_utils-0.1.0a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1288 2024-05-30 08:25:23.133318 ai_helpers_jax_utils-0.1.0a0/README.md
--rw-r--r--   0        0        0       24 2024-05-30 07:45:34.505558 ai_helpers_jax_utils-0.1.0a0/jax_utils/__init__.py
--rw-r--r--   0        0        0    17323 2024-05-30 08:16:54.737337 ai_helpers_jax_utils-0.1.0a0/jax_utils/common_tensor.py
--rw-r--r--   0        0        0     2485 2024-05-30 08:16:32.247439 ai_helpers_jax_utils-0.1.0a0/jax_utils/compilation.py
--rw-r--r--   0        0        0     4664 2024-05-30 08:20:34.055460 ai_helpers_jax_utils-0.1.0a0/jax_utils/dynamics.py
--rw-r--r--   0        0        0     7007 2024-05-30 08:19:23.450729 ai_helpers_jax_utils-0.1.0a0/jax_utils/gradient.py
--rw-r--r--   0        0        0     7159 2024-05-30 08:20:34.076501 ai_helpers_jax_utils-0.1.0a0/jax_utils/jax_tensor.py
--rw-r--r--   0        0        0     3296 2024-05-30 08:19:09.943017 ai_helpers_jax_utils-0.1.0a0/jax_utils/markov_decision_process.py
--rw-r--r--   0        0        0    20351 2024-05-30 08:19:09.963420 ai_helpers_jax_utils-0.1.0a0/jax_utils/optim.py
--rw-r--r--   0        0        0     2372 2024-05-30 08:16:32.247256 ai_helpers_jax_utils-0.1.0a0/jax_utils/pytree.py
--rw-r--r--   0        0        0     8061 2024-05-30 08:20:11.299503 ai_helpers_jax_utils-0.1.0a0/jax_utils/tranform.py
--rw-r--r--   0        0        0     2306 2024-05-30 08:16:32.247455 ai_helpers_jax_utils-0.1.0a0/jax_utils/typing.py
--rw-r--r--   0        0        0     5996 2024-05-30 08:20:34.076453 ai_helpers_jax_utils-0.1.0a0/jax_utils/vectorization.py
--rw-r--r--   0        0        0     1700 2024-05-30 08:14:16.225179 ai_helpers_jax_utils-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 ai_helpers_jax_utils-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1288 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/README.md
+-rw-r--r--   0        0        0       24 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/__init__.py
+-rw-r--r--   0        0        0    17323 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/common_tensor.py
+-rw-r--r--   0        0        0     2485 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/compilation.py
+-rw-r--r--   0        0        0     4664 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/dynamics.py
+-rw-r--r--   0        0        0     7007 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/gradient.py
+-rw-r--r--   0        0        0     7159 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/jax_tensor.py
+-rw-r--r--   0        0        0     3296 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/markov_decision_process.py
+-rw-r--r--   0        0        0    20351 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/optim.py
+-rw-r--r--   0        0        0     2372 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/pytree.py
+-rw-r--r--   0        0        0     8061 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/tranform.py
+-rw-r--r--   0        0        0     2306 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/typing.py
+-rw-r--r--   0        0        0     5996 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/jax_utils/vectorization.py
+-rw-r--r--   0        0        0     1946 2024-05-30 12:07:14.149456 ai_helpers_jax_utils-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 ai_helpers_jax_utils-0.1.0a1/PKG-INFO
```

### Comparing `ai_helpers_jax_utils-0.1.0a0/README.md` & `ai_helpers_jax_utils-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/common_tensor.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/common_tensor.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/compilation.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/compilation.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/dynamics.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/dynamics.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/gradient.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/gradient.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/jax_tensor.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/jax_tensor.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/markov_decision_process.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/markov_decision_process.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/optim.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/optim.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/pytree.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/pytree.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/tranform.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/tranform.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/typing.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/typing.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/jax_utils/vectorization.py` & `ai_helpers_jax_utils-0.1.0a1/jax_utils/vectorization.py`

 * *Files identical despite different names*

### Comparing `ai_helpers_jax_utils-0.1.0a0/pyproject.toml` & `ai_helpers_jax_utils-0.1.0a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 [tool.poetry]
 name = "ai-helpers-jax-utils"
-version = "0.1.0a0"
+version = "0.1.0a1"
 description = "Common jax utils"
 authors = ["Corentin Vasseur <vasseur.corentin@gmail.com>"]
 packages = [{ include = "jax_utils" }]
 readme = "README.md"
+repository = "https://github.com/ai-helpers/jax-utils"
+documentation = "https://ai-helpers.github.io/jax-utils/"
+keywords = ["machine-learning", "jax", "utils"]
+classifiers = [
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.11"
 jax = "^0.4.28"
 jax-dataclasses = "^1.6.0"
 tqdm = "^4.66.4"
 matplotlib = "^3.9.0"
```

### Comparing `ai_helpers_jax_utils-0.1.0a0/PKG-INFO` & `ai_helpers_jax_utils-0.1.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: ai-helpers-jax-utils
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Common jax utils
+Home-page: https://github.com/ai-helpers/jax-utils
+Keywords: machine-learning,jax,utils
 Author: Corentin Vasseur
 Author-email: vasseur.corentin@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: jax (>=0.4.28,<0.5.0)
 Requires-Dist: jax-dataclasses (>=1.6.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.9.0,<4.0.0)
 Requires-Dist: optax (>=0.2.2,<0.3.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
+Project-URL: Documentation, https://ai-helpers.github.io/jax-utils/
+Project-URL: Repository, https://github.com/ai-helpers/jax-utils
 Description-Content-Type: text/markdown
 
 # AI Helpers - Jax Utils
 
 `jax-utils` is a Python module that provides a collection of utilities to simplify and enhance the use of JAX. These utilities are designed to make working with JAX more efficient and to reduce boilerplate code.
 
 ## Table of Contents
```

