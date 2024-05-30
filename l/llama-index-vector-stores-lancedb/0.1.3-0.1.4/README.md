# Comparing `tmp/llama_index_vector_stores_lancedb-0.1.3.tar.gz` & `tmp/llama_index_vector_stores_lancedb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_lancedb-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_lancedb-0.1.4.tar", max compression
```

## Comparing `llama_index_vector_stores_lancedb-0.1.3.tar` & `llama_index_vector_stores_lancedb-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       48 2024-03-12 22:45:13.541975 llama_index_vector_stores_lancedb-0.1.3/README.md
--rw-r--r--   0        0        0      104 2024-03-12 22:45:13.541975 llama_index_vector_stores_lancedb-0.1.3/llama_index/vector_stores/lancedb/__init__.py
--rw-r--r--   0        0        0     8559 2024-03-12 22:45:13.545975 llama_index_vector_stores_lancedb-0.1.3/llama_index/vector_stores/lancedb/base.py
--rw-r--r--   0        0        0     1482 2024-03-12 22:45:13.545975 llama_index_vector_stores_lancedb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 llama_index_vector_stores_lancedb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-30 02:24:42.114590 llama_index_vector_stores_lancedb-0.1.4/README.md
+-rw-r--r--   0        0        0      104 2024-05-30 02:24:42.114590 llama_index_vector_stores_lancedb-0.1.4/llama_index/vector_stores/lancedb/__init__.py
+-rw-r--r--   0        0        0    17216 2024-05-30 02:24:42.114590 llama_index_vector_stores_lancedb-0.1.4/llama_index/vector_stores/lancedb/base.py
+-rw-r--r--   0        0        0      333 2024-05-30 02:24:42.114590 llama_index_vector_stores_lancedb-0.1.4/llama_index/vector_stores/lancedb/util.py
+-rw-r--r--   0        0        0     1517 2024-05-30 02:24:42.114590 llama_index_vector_stores_lancedb-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_vector_stores_lancedb-0.1.4/PKG-INFO
```

### Comparing `llama_index_vector_stores_lancedb-0.1.3/pyproject.toml` & `llama_index_vector_stores_lancedb-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,28 +23,30 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores lancedb integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-lancedb"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 lancedb = "^0.5.1"
+tantivy = "*"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
 pytest = "7.2.1"
+pytest-asyncio = "*"
 pytest-mock = "3.11.1"
 ruff = "0.0.292"
 tree-sitter-languages = "^1.8.0"
 types-Deprecated = ">=0.1.0"
 types-PyYAML = "^6.0.12.12"
 types-protobuf = "^4.24.0.4"
 types-redis = "4.5.5.0"
```

### Comparing `llama_index_vector_stores_lancedb-0.1.3/PKG-INFO` & `llama_index_vector_stores_lancedb-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-lancedb
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index vector_stores lancedb integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lancedb (>=0.5.1,<0.6.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: tantivy
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Lancedb
```

