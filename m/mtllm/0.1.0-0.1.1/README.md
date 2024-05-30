# Comparing `tmp/mtllm-0.1.0.tar.gz` & `tmp/mtllm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtllm-0.1.0.tar", max compression
+gzip compressed data, was "mtllm-0.1.1.tar", max compression
```

## Comparing `mtllm-0.1.0.tar` & `mtllm-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2024-05-30 01:07:24.247957 mtllm-0.1.0/LICENSE
--rw-r--r--   0        0        0       21 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/__init__.py
--rw-r--r--   0        0        0      330 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/__init__.py
--rw-r--r--   0        0        0     1991 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/anthropic.py
--rw-r--r--   0        0        0     2156 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/groq.py
--rw-r--r--   0        0        0     2668 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/huggingface.py
--rw-r--r--   0        0        0     2703 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/ollama.py
--rw-r--r--   0        0        0     1987 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/openai.py
--rw-r--r--   0        0        0     2017 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/togetherai.py
--rw-r--r--   0        0        0      219 2024-05-30 01:07:24.247957 mtllm-0.1.0/mtllm/llms/utils.py
--rw-r--r--   0        0        0      534 2024-05-30 01:07:24.251957 mtllm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      258 1970-01-01 00:00:00.000000 mtllm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-30 01:33:43.749666 mtllm-0.1.1/LICENSE
+-rw-r--r--   0        0        0       21 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/__init__.py
+-rw-r--r--   0        0        0      330 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/__init__.py
+-rw-r--r--   0        0        0     1991 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/anthropic.py
+-rw-r--r--   0        0        0     2156 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/groq.py
+-rw-r--r--   0        0        0     2668 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/huggingface.py
+-rw-r--r--   0        0        0     2703 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/ollama.py
+-rw-r--r--   0        0        0     1987 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/openai.py
+-rw-r--r--   0        0        0     2017 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/togetherai.py
+-rw-r--r--   0        0        0      219 2024-05-30 01:33:43.749666 mtllm-0.1.1/mtllm/llms/utils.py
+-rw-r--r--   0        0        0      664 2024-05-30 01:33:43.749666 mtllm-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 mtllm-0.1.1/PKG-INFO
```

### Comparing `mtllm-0.1.0/LICENSE` & `mtllm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mtllm-0.1.0/mtllm/llms/anthropic.py` & `mtllm-0.1.1/mtllm/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `mtllm-0.1.0/mtllm/llms/groq.py` & `mtllm-0.1.1/mtllm/llms/groq.py`

 * *Files identical despite different names*

### Comparing `mtllm-0.1.0/mtllm/llms/huggingface.py` & `mtllm-0.1.1/mtllm/llms/huggingface.py`

 * *Files identical despite different names*

### Comparing `mtllm-0.1.0/mtllm/llms/ollama.py` & `mtllm-0.1.1/mtllm/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `mtllm-0.1.0/mtllm/llms/openai.py` & `mtllm-0.1.1/mtllm/llms/openai.py`

 * *Files identical despite different names*

### Comparing `mtllm-0.1.0/mtllm/llms/togetherai.py` & `mtllm-0.1.1/mtllm/llms/togetherai.py`

 * *Files identical despite different names*

### Comparing `mtllm-0.1.0/pyproject.toml` & `mtllm-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "mtllm"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "MTLLM Provides Easy to use APIs for different LLM Providers to be used with Jaseci's Jaclang Programming Language."
 authors = ["Chandra Irugalbandara <irugalbandara@ascii.ai>", "Kugesan Sivasothynathan <kugesan.sivasothynathan@jaseci.org>"]
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.12.0"
-
-[tool.poetry.dev-dependencies]
 jaclang = "^0.6.0"
-pytest = "^8.2.1"
 openai = "^1.30.4"
 anthropic = "^0.26.1"
 ollama = "^0.2.0"
 together = "^1.2.0"
 transformers = "^4.41.1"
 groq = "^0.8.0"
 loguru = "^0.7.2"
 
+[tool.poetry.dev-dependencies]
+pytest = "^8.2.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

