# Comparing `tmp/yandex-chain-0.0.7.tar.gz` & `tmp/yandex-chain-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yandex-chain-0.0.7.tar", last modified: Sun Apr 28 14:13:33 2024, max compression
+gzip compressed data, was "yandex-chain-0.0.8.tar", last modified: Thu May 30 16:35:23 2024, max compression
```

## Comparing `yandex-chain-0.0.7.tar` & `yandex-chain-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 14:13:33.025991 yandex-chain-0.0.7/
--rw-rw-rw-   0        0        0     1105 2023-10-05 08:54:06.000000 yandex-chain-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       13 2023-10-10 15:43:55.000000 yandex-chain-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5206 2024-04-28 14:13:33.024990 yandex-chain-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4481 2024-04-28 14:12:52.000000 yandex-chain-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 14:13:33.026990 yandex-chain-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1067 2024-04-28 14:13:27.000000 yandex-chain-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:13:32.999110 yandex-chain-0.0.7/yandex_chain/
--rw-rw-rw-   0        0        0     1380 2023-12-11 13:18:45.000000 yandex-chain-0.0.7/yandex_chain/ChatYandexGPT.py
--rw-rw-rw-   0        0        0     4847 2024-04-28 14:07:45.000000 yandex-chain-0.0.7/yandex_chain/YandexGPT.py
--rw-rw-rw-   0        0        0     1966 2023-12-11 11:54:23.000000 yandex-chain-0.0.7/yandex_chain/YandexGPTEmbeddings.py
--rw-rw-rw-   0        0        0      300 2024-04-28 14:13:22.000000 yandex-chain-0.0.7/yandex_chain/__init__.py
--rw-rw-rw-   0        0        0     1532 2023-10-09 20:45:18.000000 yandex-chain-0.0.7/yandex_chain/util.py
-drwxrwxrwx   0        0        0        0 2024-04-28 14:13:33.021952 yandex-chain-0.0.7/yandex_chain.egg-info/
--rw-rw-rw-   0        0        0     5206 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-28 14:13:32.000000 yandex-chain-0.0.7/yandex_chain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 16:35:23.687614 yandex-chain-0.0.8/
+-rw-rw-rw-   0        0        0     1105 2023-10-05 08:54:06.000000 yandex-chain-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       13 2023-10-10 15:43:55.000000 yandex-chain-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5806 2024-05-30 16:35:23.685622 yandex-chain-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5081 2024-05-30 16:25:56.000000 yandex-chain-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 16:35:23.687614 yandex-chain-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2024-05-30 16:35:17.000000 yandex-chain-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:35:23.657613 yandex-chain-0.0.8/yandex_chain/
+-rw-rw-rw-   0        0        0     1380 2023-12-11 13:18:45.000000 yandex-chain-0.0.8/yandex_chain/ChatYandexGPT.py
+-rw-rw-rw-   0        0        0     4977 2024-05-30 16:18:31.000000 yandex-chain-0.0.8/yandex_chain/YandexGPT.py
+-rw-rw-rw-   0        0        0     1966 2023-12-11 11:54:23.000000 yandex-chain-0.0.8/yandex_chain/YandexGPTEmbeddings.py
+-rw-rw-rw-   0        0        0      300 2024-05-30 15:59:45.000000 yandex-chain-0.0.8/yandex_chain/__init__.py
+-rw-rw-rw-   0        0        0     1532 2023-10-09 20:45:18.000000 yandex-chain-0.0.8/yandex_chain/util.py
+drwxrwxrwx   0        0        0        0 2024-05-30 16:35:23.683648 yandex-chain-0.0.8/yandex_chain.egg-info/
+-rw-rw-rw-   0        0        0     5806 2024-05-30 16:35:23.000000 yandex-chain-0.0.8/yandex_chain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-30 16:35:23.000000 yandex-chain-0.0.8/yandex_chain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 16:35:23.000000 yandex-chain-0.0.8/yandex_chain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-30 16:35:23.000000 yandex-chain-0.0.8/yandex_chain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-30 16:35:23.000000 yandex-chain-0.0.8/yandex_chain.egg-info/top_level.txt
```

### Comparing `yandex-chain-0.0.7/LICENSE` & `yandex-chain-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.7/PKG-INFO` & `yandex-chain-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: yandex-chain
-Version: 0.0.7
+Version: 0.0.8
 Summary: Yandex GPT Support for LangChain
 Home-page: https://github.com/yandex-datasphere/yandex-chain
 Author: Dmitri Soshnikov
 Author-email: dmitri@soshnikov.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: langchain==0.1.0
+Requires-Dist: langchain==0.2.1
 Requires-Dist: tenacity
 
 # yandex-chain - LangChain-compatible integrations with YandexGPT and YandexGPT Embeddings
 
 This library is community-maintained Python package that provides support for [Yandex GPT](https://cloud.yandex.ru/docs/yandexgpt/) LLM and Embeddings for [LangChain Framework](https://www.langchain.com/).
 
 > Currently, Yandex GPT is in preview stage, so this library may occasionally break. Please use it at your own risk!
 
 ## What's Included
 
-The library includes the following two main classes:
+The library includes the following three main classes:
 
 * **YandexLLM** is a class representing [YandexGPT Text Generation](https://cloud.yandex.ru/docs/yandexgpt/api-ref/TextGeneration/).
+* **ChatYandexGPT** exposes the same model in chat interface that expects messages as input.
 * **YandexEmbeddings** represents [YandexGPT Embeddings](https://cloud.yandex.ru/docs/yandexgpt/api-ref/Embeddings/) service.
 
 ## Usage
 
 You can use `YandexLLM` in the following manner:
 
 ```python
@@ -47,17 +48,29 @@
 ```python
 from yandex_chain import YandexEmbeddings
 
 embeddings = YandexEmbeddings(...)
 print(embeddings("How are you today?"))
 ```
 
+Use `ChatYandexGPT` to execute a dialog with the model:
+```python
+from yandex_chain import YandexLLM
+
+gpt = ChatYandexGPT(...)
+print(gpt(
+    [
+        HumanMessage(content='Привет! Придумай 10 новых слов для приветствия.')
+    ]))
+
+``` 
+
 ## Authentication
 
-In order to use Yandex GPT, you need to provide one of the following authentication methods, which you can specify as parameters to `YandexLLM` and `YandexEmbeddings` classes:
+In order to use Yandex GPT, you need to provide one of the following authentication methods, which you can specify as parameters to `YandexLLM`, `ChatYandexGPT` and `YandexEmbeddings` classes:
 
 * A pair of `folder_id` and `api_key`
 * A pair of `folder_id` and `iam_token`
 * A path to [`config.json`](tests/config_sample.json) file, which may in turn contain parameters listed above in a convenient JSON format.
 
 ## Complete Example
 
@@ -109,20 +122,21 @@
 This chain can now answer our questions:
 ```python
 chain.invoke(query)
 ```
 
 ## Lite vs. Full Models
 
-YandexGPT model comes in three flavours - YandexGPT Lite, YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
-* **Pro** : `model=YandexGPTModel.Pro`
-* **Lite** : `model=YandexGPTModel.Lite`
-* **Summarization** : `model=YandexGPTModel.Summarization`
+YandexGPT model comes in several flavours - YandexGPT Lite (current and RC), YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
+* **Pro** (based on Yandex GPT 3): `model=YandexGPTModel.Pro`
+* **Lite** (based on Yandex GPT 2): `model=YandexGPTModel.Lite`
+* **Lite RC** (based on Yandex GPT 3): `model=YandexGPTModel.LiteRC`
+* **Summarization** (based on Yandex GPT 2): `model=YandexGPTModel.Summarization`
 
-> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated.
+> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated, and will be removed in the next version.
 
 ## Testing
 
 This repository contains some basic unit tests. To run them, you need to place a configuration file `config.json` with your credentials into `tests` folder. Use `config_sample.json` as a reference. After that, please run the following at the repository root directory:
 
 ```bash
 python -m unittest discover -s tests
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yandex-chain-0.0.7/README.md` & `yandex-chain-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 This library is community-maintained Python package that provides support for [Yandex GPT](https://cloud.yandex.ru/docs/yandexgpt/) LLM and Embeddings for [LangChain Framework](https://www.langchain.com/).
 
 > Currently, Yandex GPT is in preview stage, so this library may occasionally break. Please use it at your own risk!
 
 ## What's Included
 
-The library includes the following two main classes:
+The library includes the following three main classes:
 
 * **YandexLLM** is a class representing [YandexGPT Text Generation](https://cloud.yandex.ru/docs/yandexgpt/api-ref/TextGeneration/).
+* **ChatYandexGPT** exposes the same model in chat interface that expects messages as input.
 * **YandexEmbeddings** represents [YandexGPT Embeddings](https://cloud.yandex.ru/docs/yandexgpt/api-ref/Embeddings/) service.
 
 ## Usage
 
 You can use `YandexLLM` in the following manner:
 
 ```python
@@ -27,17 +28,29 @@
 ```python
 from yandex_chain import YandexEmbeddings
 
 embeddings = YandexEmbeddings(...)
 print(embeddings("How are you today?"))
 ```
 
+Use `ChatYandexGPT` to execute a dialog with the model:
+```python
+from yandex_chain import YandexLLM
+
+gpt = ChatYandexGPT(...)
+print(gpt(
+    [
+        HumanMessage(content='Привет! Придумай 10 новых слов для приветствия.')
+    ]))
+
+``` 
+
 ## Authentication
 
-In order to use Yandex GPT, you need to provide one of the following authentication methods, which you can specify as parameters to `YandexLLM` and `YandexEmbeddings` classes:
+In order to use Yandex GPT, you need to provide one of the following authentication methods, which you can specify as parameters to `YandexLLM`, `ChatYandexGPT` and `YandexEmbeddings` classes:
 
 * A pair of `folder_id` and `api_key`
 * A pair of `folder_id` and `iam_token`
 * A path to [`config.json`](tests/config_sample.json) file, which may in turn contain parameters listed above in a convenient JSON format.
 
 ## Complete Example
 
@@ -89,20 +102,21 @@
 This chain can now answer our questions:
 ```python
 chain.invoke(query)
 ```
 
 ## Lite vs. Full Models
 
-YandexGPT model comes in three flavours - YandexGPT Lite, YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
-* **Pro** : `model=YandexGPTModel.Pro`
-* **Lite** : `model=YandexGPTModel.Lite`
-* **Summarization** : `model=YandexGPTModel.Summarization`
+YandexGPT model comes in several flavours - YandexGPT Lite (current and RC), YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
+* **Pro** (based on Yandex GPT 3): `model=YandexGPTModel.Pro`
+* **Lite** (based on Yandex GPT 2): `model=YandexGPTModel.Lite`
+* **Lite RC** (based on Yandex GPT 3): `model=YandexGPTModel.LiteRC`
+* **Summarization** (based on Yandex GPT 2): `model=YandexGPTModel.Summarization`
 
-> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated.
+> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated, and will be removed in the next version.
 
 ## Testing
 
 This repository contains some basic unit tests. To run them, you need to place a configuration file `config.json` with your credentials into `tests` folder. Use `config_sample.json` as a reference. After that, please run the following at the repository root directory:
 
 ```bash
 python -m unittest discover -s tests
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yandex-chain-0.0.7/setup.py` & `yandex-chain-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 
 import setuptools
 
-with open('README.md') as readme_file:
+with open('README.md',encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name='yandex-chain',
     packages=setuptools.find_namespace_packages('.',exclude=['tests','examples']),
-    version='0.0.7',
-    install_requires=['requests','langchain==0.1.0','tenacity'],
+    version='0.0.8',
+    install_requires=['requests','langchain==0.2.1','tenacity'],
     description='Yandex GPT Support for LangChain',
     author='Dmitri Soshnikov',
     author_email='dmitri@soshnikov.com',
     url='https://github.com/yandex-datasphere/yandex-chain',
     long_description=readme,
     long_description_content_type='text/markdown; charset=UTF-8',
     license='MIT license',
```

### Comparing `yandex-chain-0.0.7/yandex_chain/ChatYandexGPT.py` & `yandex-chain-0.0.8/yandex_chain/ChatYandexGPT.py`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.7/yandex_chain/YandexGPT.py` & `yandex-chain-0.0.8/yandex_chain/YandexGPT.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from tenacity import Retrying, RetryError, stop_after_attempt, wait_fixed
 from enum import Enum
 
 class YandexGPTModel(Enum):
     Lite = 0
     Pro = 1
     Summarization = 2
-    Custom = 3
+    LiteRC = 3
+    Custom = 99
 
 class YandexLLM(LLM):
     temperature : float = 1.0
     max_tokens : int = 1500
     sleep_interval : float = 1.0
     retries = 3
     use_lite : bool = None
@@ -50,14 +51,16 @@
             else:
                 self.model = YandexGPTModel.Lite if self.use_lite else YandexGPTModel.Pro
         if self.instruction_id:
             self.model = YandexGPTModel.Custom
             return f"ds://{self.instruction_id}"
         if self.model == YandexGPTModel.Lite:
             return f"gpt://{self.folder_id}/yandexgpt-lite/latest"
+        if self.model == YandexGPTModel.LiteRC:
+            return f"gpt://{self.folder_id}/yandexgpt-lite/rc"
         elif self.model == YandexGPTModel.Pro:
             return f"gpt://{self.folder_id}/yandexgpt/latest"
         elif self.model == YandexGPTModel.Summarization:
             return f"gpt://{self.folder_id}/summarization/latest"
         else:
             raise YException("Invalid model flag")
```

### Comparing `yandex-chain-0.0.7/yandex_chain/YandexGPTEmbeddings.py` & `yandex-chain-0.0.8/yandex_chain/YandexGPTEmbeddings.py`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.7/yandex_chain/util.py` & `yandex-chain-0.0.8/yandex_chain/util.py`

 * *Files identical despite different names*

### Comparing `yandex-chain-0.0.7/yandex_chain.egg-info/PKG-INFO` & `yandex-chain-0.0.8/yandex_chain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: yandex-chain
-Version: 0.0.7
+Version: 0.0.8
 Summary: Yandex GPT Support for LangChain
 Home-page: https://github.com/yandex-datasphere/yandex-chain
 Author: Dmitri Soshnikov
 Author-email: dmitri@soshnikov.com
 License: MIT license
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: langchain==0.1.0
+Requires-Dist: langchain==0.2.1
 Requires-Dist: tenacity
 
 # yandex-chain - LangChain-compatible integrations with YandexGPT and YandexGPT Embeddings
 
 This library is community-maintained Python package that provides support for [Yandex GPT](https://cloud.yandex.ru/docs/yandexgpt/) LLM and Embeddings for [LangChain Framework](https://www.langchain.com/).
 
 > Currently, Yandex GPT is in preview stage, so this library may occasionally break. Please use it at your own risk!
 
 ## What's Included
 
-The library includes the following two main classes:
+The library includes the following three main classes:
 
 * **YandexLLM** is a class representing [YandexGPT Text Generation](https://cloud.yandex.ru/docs/yandexgpt/api-ref/TextGeneration/).
+* **ChatYandexGPT** exposes the same model in chat interface that expects messages as input.
 * **YandexEmbeddings** represents [YandexGPT Embeddings](https://cloud.yandex.ru/docs/yandexgpt/api-ref/Embeddings/) service.
 
 ## Usage
 
 You can use `YandexLLM` in the following manner:
 
 ```python
@@ -47,17 +48,29 @@
 ```python
 from yandex_chain import YandexEmbeddings
 
 embeddings = YandexEmbeddings(...)
 print(embeddings("How are you today?"))
 ```
 
+Use `ChatYandexGPT` to execute a dialog with the model:
+```python
+from yandex_chain import YandexLLM
+
+gpt = ChatYandexGPT(...)
+print(gpt(
+    [
+        HumanMessage(content='Привет! Придумай 10 новых слов для приветствия.')
+    ]))
+
+``` 
+
 ## Authentication
 
-In order to use Yandex GPT, you need to provide one of the following authentication methods, which you can specify as parameters to `YandexLLM` and `YandexEmbeddings` classes:
+In order to use Yandex GPT, you need to provide one of the following authentication methods, which you can specify as parameters to `YandexLLM`, `ChatYandexGPT` and `YandexEmbeddings` classes:
 
 * A pair of `folder_id` and `api_key`
 * A pair of `folder_id` and `iam_token`
 * A path to [`config.json`](tests/config_sample.json) file, which may in turn contain parameters listed above in a convenient JSON format.
 
 ## Complete Example
 
@@ -109,20 +122,21 @@
 This chain can now answer our questions:
 ```python
 chain.invoke(query)
 ```
 
 ## Lite vs. Full Models
 
-YandexGPT model comes in three flavours - YandexGPT Lite, YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
-* **Pro** : `model=YandexGPTModel.Pro`
-* **Lite** : `model=YandexGPTModel.Lite`
-* **Summarization** : `model=YandexGPTModel.Summarization`
+YandexGPT model comes in several flavours - YandexGPT Lite (current and RC), YandexGPT Pro and Summarization model. By default, YandexGPT Lite is used. If you want to use different model, please specify it in the constructor of `YandexLLM` or `ChatYandexGPT` language model classes:
+* **Pro** (based on Yandex GPT 3): `model=YandexGPTModel.Pro`
+* **Lite** (based on Yandex GPT 2): `model=YandexGPTModel.Lite`
+* **Lite RC** (based on Yandex GPT 3): `model=YandexGPTModel.LiteRC`
+* **Summarization** (based on Yandex GPT 2): `model=YandexGPTModel.Summarization`
 
-> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated.
+> In previous versions, we were using `use_lite` flag to switch between Lite and Pro models. This behavior is still supported, but is deprecated, and will be removed in the next version.
 
 ## Testing
 
 This repository contains some basic unit tests. To run them, you need to place a configuration file `config.json` with your credentials into `tests` folder. Use `config_sample.json` as a reference. After that, please run the following at the repository root directory:
 
 ```bash
 python -m unittest discover -s tests
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

