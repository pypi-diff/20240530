# Comparing `tmp/aishalib-0.0.4.tar.gz` & `tmp/aishalib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishalib-0.0.4.tar", last modified: Thu May 30 11:01:44 2024, max compression
+gzip compressed data, was "aishalib-0.0.5.tar", last modified: Thu May 30 15:28:13 2024, max compression
```

## Comparing `aishalib-0.0.4.tar` & `aishalib-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.4/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)     5892 2024-05-30 11:01:44.056093 aishalib-0.0.4/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)     5294 2024-05-30 10:59:59.000000 aishalib-0.0.4/README.md
--rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-30 11:01:36.000000 aishalib-0.0.4/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-30 11:01:44.056093 aishalib-0.0.4/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/src/aishalib/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     3848 2024-05-29 10:48:48.000000 aishalib-0.0.4/src/aishalib/aishalib.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.4/src/aishalib/llmbackend.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 11:01:44.056093 aishalib-0.0.4/src/aishalib.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     5892 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-30 11:01:44.000000 aishalib-0.0.4/src/aishalib.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.5/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-30 15:28:13.683395 aishalib-0.0.5/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6130 2024-05-30 15:27:43.000000 aishalib-0.0.5/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-30 15:28:06.000000 aishalib-0.0.5/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-30 15:28:13.683395 aishalib-0.0.5/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/src/aishalib/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     3848 2024-05-29 10:48:48.000000 aishalib-0.0.5/src/aishalib/aishalib.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.5/src/aishalib/llmbackend.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/src/aishalib.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/top_level.txt
```

### Comparing `aishalib-0.0.4/LICENSE` & `aishalib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.4/PKG-INFO` & `aishalib-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 
 ## Telegram bot example
 ```python
 from aishalib.aishalib import Aisha
 from telegram import Update
 from telegram.ext import Application, MessageHandler, ContextTypes, filters
 
-TG_TOKEN = "6440843851:AAGB_-JvQLwP-j93LeV0p19bWDi2TH6K_bw"
+TG_TOKEN = "YOUR_TG_TOKEN"
 
 SYSTEM_PROMPT = """
 Ты умный бот помощник для общения в телеграме.
 Ты общаешься в групповом чате с другими пользователями.
 Ты отвечаешь на русском языке.
 """
 
@@ -112,14 +112,37 @@
     aisha = cl.user_session.get("aisha")
     aisha.add_user_request(input_msg.content)
     response = await cl.make_async(aisha.completion)(temp=0.5, top_p=0.5)
     output_msg.content = response
     await output_msg.update()
 ```
 
+## Document search example
+```python
+from aisha import Aisha
+
+MODEL_ID = "microsoft/Phi-3-medium-128k-instruct"
+COMPLETION_URL = "http://127.0.0.1:8000/completion"
+
+with open("document.txt") as f:
+    text = f.read()
+
+prompt = f"""Ты - поисковая система.
+Ниже представлен следующий текст по которому необходимо выполнять поиск.
+## Текст:
+{text}
+"""
+
+aisha = Aisha(MODEL_ID, COMPLETION_URL, prompt=prompt, max_context=40000, max_predict=8192)
+user_request = "Вопрос по документу"
+prompt = f"Верни релевантные фрагменты текста, которые наиболее точно соответствуют запросу пользователя: {user_request}."
+aisha.add_user_request(prompt)
+print(aisha.completion(temp=0.0, top_p=0.0))
+```
+
 ## Run Llama.CPP Server backend
 ```console
 llama.cpp/build/bin/server -m model_q5_k_m.gguf -ngl 99 -fa -c 4096 --host 0.0.0.0 --port 8000
 ```
 
 ## Install CUDA toolkit for Llama.cpp compilation
 Please note that the toolkit version must match the driver version. The driver version can be found using the nvidia-smi command.
```

### Comparing `aishalib-0.0.4/README.md` & `aishalib-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ## Telegram bot example
 ```python
 from aishalib.aishalib import Aisha
 from telegram import Update
 from telegram.ext import Application, MessageHandler, ContextTypes, filters
 
-TG_TOKEN = "6440843851:AAGB_-JvQLwP-j93LeV0p19bWDi2TH6K_bw"
+TG_TOKEN = "YOUR_TG_TOKEN"
 
 SYSTEM_PROMPT = """
 Ты умный бот помощник для общения в телеграме.
 Ты общаешься в групповом чате с другими пользователями.
 Ты отвечаешь на русском языке.
 """
 
@@ -95,14 +95,37 @@
     aisha = cl.user_session.get("aisha")
     aisha.add_user_request(input_msg.content)
     response = await cl.make_async(aisha.completion)(temp=0.5, top_p=0.5)
     output_msg.content = response
     await output_msg.update()
 ```
 
+## Document search example
+```python
+from aisha import Aisha
+
+MODEL_ID = "microsoft/Phi-3-medium-128k-instruct"
+COMPLETION_URL = "http://127.0.0.1:8000/completion"
+
+with open("document.txt") as f:
+    text = f.read()
+
+prompt = f"""Ты - поисковая система.
+Ниже представлен следующий текст по которому необходимо выполнять поиск.
+## Текст:
+{text}
+"""
+
+aisha = Aisha(MODEL_ID, COMPLETION_URL, prompt=prompt, max_context=40000, max_predict=8192)
+user_request = "Вопрос по документу"
+prompt = f"Верни релевантные фрагменты текста, которые наиболее точно соответствуют запросу пользователя: {user_request}."
+aisha.add_user_request(prompt)
+print(aisha.completion(temp=0.0, top_p=0.0))
+```
+
 ## Run Llama.CPP Server backend
 ```console
 llama.cpp/build/bin/server -m model_q5_k_m.gguf -ngl 99 -fa -c 4096 --host 0.0.0.0 --port 8000
 ```
 
 ## Install CUDA toolkit for Llama.cpp compilation
 Please note that the toolkit version must match the driver version. The driver version can be found using the nvidia-smi command.
```

### Comparing `aishalib-0.0.4/pyproject.toml` & `aishalib-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aishalib"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
 description = "AI Smart Human Assistant Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `aishalib-0.0.4/src/aishalib/aishalib.py` & `aishalib-0.0.5/src/aishalib/aishalib.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.4/src/aishalib/llmbackend.py` & `aishalib-0.0.5/src/aishalib/llmbackend.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.4/src/aishalib.egg-info/PKG-INFO` & `aishalib-0.0.5/src/aishalib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 
 ## Telegram bot example
 ```python
 from aishalib.aishalib import Aisha
 from telegram import Update
 from telegram.ext import Application, MessageHandler, ContextTypes, filters
 
-TG_TOKEN = "6440843851:AAGB_-JvQLwP-j93LeV0p19bWDi2TH6K_bw"
+TG_TOKEN = "YOUR_TG_TOKEN"
 
 SYSTEM_PROMPT = """
 Ты умный бот помощник для общения в телеграме.
 Ты общаешься в групповом чате с другими пользователями.
 Ты отвечаешь на русском языке.
 """
 
@@ -112,14 +112,37 @@
     aisha = cl.user_session.get("aisha")
     aisha.add_user_request(input_msg.content)
     response = await cl.make_async(aisha.completion)(temp=0.5, top_p=0.5)
     output_msg.content = response
     await output_msg.update()
 ```
 
+## Document search example
+```python
+from aisha import Aisha
+
+MODEL_ID = "microsoft/Phi-3-medium-128k-instruct"
+COMPLETION_URL = "http://127.0.0.1:8000/completion"
+
+with open("document.txt") as f:
+    text = f.read()
+
+prompt = f"""Ты - поисковая система.
+Ниже представлен следующий текст по которому необходимо выполнять поиск.
+## Текст:
+{text}
+"""
+
+aisha = Aisha(MODEL_ID, COMPLETION_URL, prompt=prompt, max_context=40000, max_predict=8192)
+user_request = "Вопрос по документу"
+prompt = f"Верни релевантные фрагменты текста, которые наиболее точно соответствуют запросу пользователя: {user_request}."
+aisha.add_user_request(prompt)
+print(aisha.completion(temp=0.0, top_p=0.0))
+```
+
 ## Run Llama.CPP Server backend
 ```console
 llama.cpp/build/bin/server -m model_q5_k_m.gguf -ngl 99 -fa -c 4096 --host 0.0.0.0 --port 8000
 ```
 
 ## Install CUDA toolkit for Llama.cpp compilation
 Please note that the toolkit version must match the driver version. The driver version can be found using the nvidia-smi command.
```

