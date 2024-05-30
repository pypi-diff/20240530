# Comparing `tmp/llama_index_embeddings_ipex_llm-0.1.2.tar.gz` & `tmp/llama_index_embeddings_ipex_llm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_ipex_llm-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_embeddings_ipex_llm-0.1.3.tar", max compression
```

## Comparing `llama_index_embeddings_ipex_llm-0.1.2.tar` & `llama_index_embeddings_ipex_llm-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      324 2024-05-23 02:04:05.953688 llama_index_embeddings_ipex_llm-0.1.2/README.md
--rw-r--r--   0        0        0       17 2024-05-23 02:04:05.953688 llama_index_embeddings_ipex_llm-0.1.2/llama_index/embeddings/ipex_llm/BUILD
--rw-r--r--   0        0        0       99 2024-05-23 02:04:05.953688 llama_index_embeddings_ipex_llm-0.1.2/llama_index/embeddings/ipex_llm/__init__.py
--rw-r--r--   0        0        0     5319 2024-05-23 02:04:05.953688 llama_index_embeddings_ipex_llm-0.1.2/llama_index/embeddings/ipex_llm/base.py
--rw-r--r--   0        0        0     2391 2024-05-23 02:04:05.953688 llama_index_embeddings_ipex_llm-0.1.2/llama_index/embeddings/ipex_llm/utils.py
--rw-r--r--   0        0        0     2460 2024-05-23 02:04:05.953688 llama_index_embeddings_ipex_llm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 llama_index_embeddings_ipex_llm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      324 2024-05-30 17:35:54.890061 llama_index_embeddings_ipex_llm-0.1.3/README.md
+-rw-r--r--   0        0        0       17 2024-05-30 17:35:54.890061 llama_index_embeddings_ipex_llm-0.1.3/llama_index/embeddings/ipex_llm/BUILD
+-rw-r--r--   0        0        0       99 2024-05-30 17:35:54.890061 llama_index_embeddings_ipex_llm-0.1.3/llama_index/embeddings/ipex_llm/__init__.py
+-rw-r--r--   0        0        0     5319 2024-05-30 17:35:54.890061 llama_index_embeddings_ipex_llm-0.1.3/llama_index/embeddings/ipex_llm/base.py
+-rw-r--r--   0        0        0     2391 2024-05-30 17:35:54.890061 llama_index_embeddings_ipex_llm-0.1.3/llama_index/embeddings/ipex_llm/utils.py
+-rw-r--r--   0        0        0     2546 2024-05-30 17:35:54.890061 llama_index_embeddings_ipex_llm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 llama_index_embeddings_ipex_llm-0.1.3/PKG-INFO
```

### Comparing `llama_index_embeddings_ipex_llm-0.1.2/llama_index/embeddings/ipex_llm/base.py` & `llama_index_embeddings_ipex_llm-0.1.3/llama_index/embeddings/ipex_llm/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_ipex_llm-0.1.2/llama_index/embeddings/ipex_llm/utils.py` & `llama_index_embeddings_ipex_llm-0.1.3/llama_index/embeddings/ipex_llm/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_ipex_llm-0.1.2/pyproject.toml` & `llama_index_embeddings_ipex_llm-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,28 +26,29 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings ipex-llm integration"
 license = "MIT"
 name = "llama-index-embeddings-ipex-llm"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.0"
-ipex-llm = {allow-prereleases = true, extras = ["llama-index"], version = ">=2.1.0b20240514"}
+ipex-llm = {allow-prereleases = true, extras = ["llama-index"], version = ">=2.1.0b20240529"}
 torch = {optional = true, source = "ipex-xpu-src-us", version = "2.1.0a0"}
 torchvision = {optional = true, source = "ipex-xpu-src-us", version = "0.16.0a0"}
 intel_extension_for_pytorch = {optional = true, source = "ipex-xpu-src-us", version = "2.1.10+xpu"}
 bigdl-core-xe-21 = {optional = true, version = "*"}
-bigdl-core-xe-esimd-21 = {optional = true, version = "*"}
+bigdl-core-xe-batch-21 = {optional = true, version = "*"}
+bigdl-core-xe-addons-21 = {optional = true, version = "*"}
 
 [tool.poetry.extras]
-xpu = ["bigdl-core-xe-21", "bigdl-core-xe-esimd-21", "intel_extension_for_pytorch", "torch", "torchvision"]
+xpu = ["bigdl-core-xe-21", "bigdl-core-xe-addons-21", "bigdl-core-xe-batch-21", "intel_extension_for_pytorch", "torch", "torchvision"]
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_embeddings_ipex_llm-0.1.2/PKG-INFO` & `llama_index_embeddings_ipex_llm-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-ipex-llm
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index embeddings ipex-llm integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: xpu
 Requires-Dist: bigdl-core-xe-21 ; extra == "xpu"
-Requires-Dist: bigdl-core-xe-esimd-21 ; extra == "xpu"
+Requires-Dist: bigdl-core-xe-addons-21 ; extra == "xpu"
+Requires-Dist: bigdl-core-xe-batch-21 ; extra == "xpu"
 Requires-Dist: intel_extension_for_pytorch (==2.1.10+xpu) ; extra == "xpu"
-Requires-Dist: ipex-llm[llama-index] (>=2.1.0b20240514)
+Requires-Dist: ipex-llm[llama-index] (>=2.1.0b20240529)
 Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
 Requires-Dist: torch (==2.1.0a0) ; extra == "xpu"
 Requires-Dist: torchvision (==0.16.0a0) ; extra == "xpu"
 Description-Content-Type: text/markdown
 
 # LlamaIndex Embeddings Integration: Ipex_Llm
```

