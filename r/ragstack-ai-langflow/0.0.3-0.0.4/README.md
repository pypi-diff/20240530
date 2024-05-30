# Comparing `tmp/ragstack_ai_langflow-0.0.3.tar.gz` & `tmp/ragstack_ai_langflow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_langflow-0.0.3.tar", max compression
+gzip compressed data, was "ragstack_ai_langflow-0.0.4.tar", max compression
```

## Comparing `ragstack_ai_langflow-0.0.3.tar` & `ragstack_ai_langflow-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3781 2024-05-15 11:38:04.466284 ragstack_ai_langflow-0.0.3/LICENSE.md
--rw-r--r--   0        0        0      286 2024-05-15 11:38:04.466284 ragstack_ai_langflow-0.0.3/README.md
--rw-r--r--   0        0        0     3839 2024-05-15 11:38:28.878575 ragstack_ai_langflow-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       63 2024-05-15 11:38:04.950290 ragstack_ai_langflow-0.0.3/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      339 2024-05-15 11:38:04.950290 ragstack_ai_langflow-0.0.3/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 ragstack_ai_langflow-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3781 2024-05-30 16:46:52.206314 ragstack_ai_langflow-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0      286 2024-05-30 16:46:52.206314 ragstack_ai_langflow-0.0.4/README.md
+-rw-r--r--   0        0        0     3839 2024-05-30 16:47:21.134339 ragstack_ai_langflow-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-30 16:46:52.690314 ragstack_ai_langflow-0.0.4/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      339 2024-05-30 16:46:52.690314 ragstack_ai_langflow-0.0.4/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 ragstack_ai_langflow-0.0.4/PKG-INFO
```

### Comparing `ragstack_ai_langflow-0.0.3/LICENSE.md` & `ragstack_ai_langflow-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai_langflow-0.0.3/pyproject.toml` & `ragstack_ai_langflow-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragstack-ai-langflow"
-version = "0.0.3"
+version = "0.0.4"
 description = "RAGStack Langflow"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 repository = "https://github.com/datastax/ragstack-ai-langflow"
 readme = "README.md"
 keywords = ["nlp", "langchain", "openai", "gpt", "gui"]
 packages = [{ include = "langflow", from = "src/backend" }]
```

### Comparing `ragstack_ai_langflow-0.0.3/PKG-INFO` & `ragstack_ai_langflow-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-langflow
-Version: 0.0.3
+Version: 0.0.4
 Summary: RAGStack Langflow
 Home-page: https://github.com/datastax/ragstack-ai-langflow
 License: BUSL-1.1
 Keywords: nlp,langchain,openai,gpt,gui
 Author: DataStax
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
```

