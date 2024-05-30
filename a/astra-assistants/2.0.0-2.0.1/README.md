# Comparing `tmp/astra_assistants-2.0.0.tar.gz` & `tmp/astra_assistants-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astra_assistants-2.0.0.tar", max compression
+gzip compressed data, was "astra_assistants-2.0.1.tar", max compression
```

## Comparing `astra_assistants-2.0.0.tar` & `astra_assistants-2.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3497 2024-05-29 19:29:06.840457 astra_assistants-2.0.0/README.md
--rw-r--r--   0        0        0       26 2024-05-29 18:56:43.423177 astra_assistants-2.0.0/astra_assistants/__init__.py
--rw-r--r--   0        0        0    16119 2024-05-29 19:28:15.235356 astra_assistants-2.0.0/astra_assistants/patch.py
--rw-r--r--   0        0        0      623 2024-05-29 19:00:40.236096 astra_assistants-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4231 1970-01-01 00:00:00.000000 astra_assistants-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3497 2024-05-29 20:29:12.455004 astra_assistants-2.0.1/README.md
+-rw-r--r--   0        0        0       26 2024-05-29 20:29:12.455004 astra_assistants-2.0.1/astra_assistants/__init__.py
+-rw-r--r--   0        0        0    16119 2024-05-29 20:29:12.455004 astra_assistants-2.0.1/astra_assistants/patch.py
+-rw-r--r--   0        0        0      592 2024-05-30 18:31:02.965462 astra_assistants-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 astra_assistants-2.0.1/PKG-INFO
```

### Comparing `astra_assistants-2.0.0/README.md` & `astra_assistants-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `astra_assistants-2.0.0/astra_assistants/patch.py` & `astra_assistants-2.0.1/astra_assistants/patch.py`

 * *Files identical despite different names*

### Comparing `astra_assistants-2.0.0/pyproject.toml` & `astra_assistants-2.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "astra-assistants"
-version = "2.0.0"
+version = "2.0.1"
 description = "Astra Assistants API - drop in replacement for OpenAI Assistants, powered by AstraDB"
 authors = ["phact <estevezsebastian@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.26.0"
 openai = "^1.20.0"
 litellm = "^1.39.2"
 boto3 = "^1.34.31"
-google-generativeai = "^0.4.1"
 aiohttp = "^3.9.4"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 pytest = "^8.0.2"
```

### Comparing `astra_assistants-2.0.0/PKG-INFO` & `astra_assistants-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: astra-assistants
-Version: 2.0.0
+Version: 2.0.1
 Summary: Astra Assistants API - drop in replacement for OpenAI Assistants, powered by AstraDB
 Author: phact
 Author-email: estevezsebastian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: boto3 (>=1.34.31,<2.0.0)
-Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: litellm (>=1.39.2,<2.0.0)
 Requires-Dist: openai (>=1.20.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # astra-assistants
```

