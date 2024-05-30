# Comparing `tmp/llm_elasticsearch_cache-0.2.5.tar.gz` & `tmp/llm_elasticsearch_cache-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_elasticsearch_cache-0.2.5.tar", max compression
+gzip compressed data, was "llm_elasticsearch_cache-0.2.6.tar", max compression
```

## Comparing `llm_elasticsearch_cache-0.2.5.tar` & `llm_elasticsearch_cache-0.2.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-02-12 12:29:42.006502 llm_elasticsearch_cache-0.2.5/LICENSE
--rw-r--r--   0        0        0     4792 2024-05-09 09:47:51.709916 llm_elasticsearch_cache-0.2.5/README.md
--rw-r--r--   0        0        0     1381 2024-05-09 10:00:11.973596 llm_elasticsearch_cache-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-12 12:54:53.592163 llm_elasticsearch_cache-0.2.5/src/llmescache/__init__.py
--rw-r--r--   0        0        0      185 2024-02-28 08:37:18.743318 llm_elasticsearch_cache-0.2.5/src/llmescache/langchain/__init__.py
--rw-r--r--   0        0        0     1128 2024-03-26 08:12:00.625891 llm_elasticsearch_cache-0.2.5/src/llmescache/langchain/base.py
--rw-r--r--   0        0        0     5384 2024-03-26 08:12:00.626922 llm_elasticsearch_cache-0.2.5/src/llmescache/langchain/cache.py
--rw-r--r--   0        0        0     6094 2024-04-08 10:11:31.752144 llm_elasticsearch_cache-0.2.5/src/llmescache/langchain/storage.py
--rw-r--r--   0        0        0        0 2024-02-20 16:20:08.430038 llm_elasticsearch_cache-0.2.5/src/llmescache/py.typed
--rw-r--r--   0        0        0     6059 1970-01-01 00:00:00.000000 llm_elasticsearch_cache-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-12 12:29:42.006502 llm_elasticsearch_cache-0.2.6/LICENSE
+-rw-r--r--   0        0        0     4793 2024-05-30 10:43:39.525806 llm_elasticsearch_cache-0.2.6/README.md
+-rw-r--r--   0        0        0     1381 2024-05-30 10:44:00.259985 llm_elasticsearch_cache-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-12 12:54:53.592163 llm_elasticsearch_cache-0.2.6/src/llmescache/__init__.py
+-rw-r--r--   0        0        0      185 2024-02-28 08:37:18.743318 llm_elasticsearch_cache-0.2.6/src/llmescache/langchain/__init__.py
+-rw-r--r--   0        0        0     1128 2024-03-26 08:12:00.625891 llm_elasticsearch_cache-0.2.6/src/llmescache/langchain/base.py
+-rw-r--r--   0        0        0     5384 2024-03-26 08:12:00.626922 llm_elasticsearch_cache-0.2.6/src/llmescache/langchain/cache.py
+-rw-r--r--   0        0        0     6094 2024-04-08 10:11:31.752144 llm_elasticsearch_cache-0.2.6/src/llmescache/langchain/storage.py
+-rw-r--r--   0        0        0        0 2024-02-20 16:20:08.430038 llm_elasticsearch_cache-0.2.6/src/llmescache/py.typed
+-rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 llm_elasticsearch_cache-0.2.6/PKG-INFO
```

### Comparing `llm_elasticsearch_cache-0.2.5/LICENSE` & `llm_elasticsearch_cache-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.5/README.md` & `llm_elasticsearch_cache-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 > [!IMPORTANT]
-> ## This library is now part of LangChain, follow the official documentation, e.g. [for the LLM cache](https://python.langchain.com/docs/integrations/llms/llm_caching/#elasticsearch-cache)
+> ## This library is now part of LangChain, follow the official documentation, e.g. [for the LLM cache](https://python.langchain.com/v0.2/docs/integrations/llm_caching/#elasticsearch-cache)
 
 # llm-elasticsearch-cache
 
 A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models.
 
 ## Install
 
 ```shell
 pip install llm-elasticsearch-cache
 ```
 
 ## Chat cache usage
 
 The LangChain cache can be used similarly to the
-[other cache integrations](https://python.langchain.com/docs/integrations/llms/llm_caching).
+[other cache integrations](https://python.langchain.com/v0.2/docs/integrations/llm_caching/).
 
 ### Basic example
 
 ```python
 from langchain.globals import set_llm_cache
 from llmescache.langchain import ElasticsearchCache
 from elasticsearch import Elasticsearch
```

### Comparing `llm_elasticsearch_cache-0.2.5/pyproject.toml` & `llm_elasticsearch_cache-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-elasticsearch-cache"
-version = "0.2.5"
+version = "0.2.6"
 description = "[IMPORTANT: This library is now part of LangChain, follow its official documentation] A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models."
 packages = [{include = "llmescache", from = "./src"}]
 authors = ["SpazioDati s.r.l."]
 maintainers = ["Giacomo Berardi <berardi@spaziodati.eu>", "Gabriele Ghisleni <gabriele.ghisleni@spaziodati.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/SpazioDati/llm-elasticsearch-cache"
```

### Comparing `llm_elasticsearch_cache-0.2.5/src/llmescache/langchain/base.py` & `llm_elasticsearch_cache-0.2.6/src/llmescache/langchain/base.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.5/src/llmescache/langchain/cache.py` & `llm_elasticsearch_cache-0.2.6/src/llmescache/langchain/cache.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.5/src/llmescache/langchain/storage.py` & `llm_elasticsearch_cache-0.2.6/src/llmescache/langchain/storage.py`

 * *Files identical despite different names*

### Comparing `llm_elasticsearch_cache-0.2.5/PKG-INFO` & `llm_elasticsearch_cache-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-elasticsearch-cache
-Version: 0.2.5
+Version: 0.2.6
 Summary: [IMPORTANT: This library is now part of LangChain, follow its official documentation] A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models.
 Home-page: https://github.com/SpazioDati/llm-elasticsearch-cache
 License: MIT
 Keywords: langchain,elasticsearch,openai,llm,chatgpt
 Author: SpazioDati s.r.l.
 Maintainer: Giacomo Berardi
 Maintainer-email: berardi@spaziodati.eu
@@ -22,30 +22,30 @@
 Classifier: Topic :: Software Development
 Requires-Dist: elasticsearch (>6)
 Requires-Dist: langchain (>=0.1,<0.2)
 Project-URL: Repository, https://github.com/SpazioDati/llm-elasticsearch-cache
 Description-Content-Type: text/markdown
 
 > [!IMPORTANT]
-> ## This library is now part of LangChain, follow the official documentation, e.g. [for the LLM cache](https://python.langchain.com/docs/integrations/llms/llm_caching/#elasticsearch-cache)
+> ## This library is now part of LangChain, follow the official documentation, e.g. [for the LLM cache](https://python.langchain.com/v0.2/docs/integrations/llm_caching/#elasticsearch-cache)
 
 # llm-elasticsearch-cache
 
 A caching layer for LLMs that exploits Elasticsearch, fully compatible with LangChain caching, both for chat and embeddings models.
 
 ## Install
 
 ```shell
 pip install llm-elasticsearch-cache
 ```
 
 ## Chat cache usage
 
 The LangChain cache can be used similarly to the
-[other cache integrations](https://python.langchain.com/docs/integrations/llms/llm_caching).
+[other cache integrations](https://python.langchain.com/v0.2/docs/integrations/llm_caching/).
 
 ### Basic example
 
 ```python
 from langchain.globals import set_llm_cache
 from llmescache.langchain import ElasticsearchCache
 from elasticsearch import Elasticsearch
```

