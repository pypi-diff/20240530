# Comparing `tmp/FLUTE-LLM-0.1.1.tar.gz` & `tmp/FLUTE-LLM-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLUTE-LLM-0.1.1.tar", last modified: Thu May 30 11:16:25 2024, max compression
+gzip compressed data, was "FLUTE-LLM-0.1.2.tar", last modified: Thu May 30 11:25:26 2024, max compression
```

## Comparing `FLUTE-LLM-0.1.1.tar` & `FLUTE-LLM-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.281091 FLUTE-LLM-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.213816 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/
--rw-rw-rw-   0        0        0     3803 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3803 2024-05-30 11:16:25.281091 FLUTE-LLM-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3396 2024-05-30 11:07:52.000000 FLUTE-LLM-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.214817 FLUTE-LLM-0.1.1/flute/
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.256104 FLUTE-LLM-0.1.1/flute/Modules/
--rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.1/flute/Modules/AbstractPromptProcessor.py
--rw-rw-rw-   0        0        0     2450 2024-05-28 13:04:00.000000 FLUTE-LLM-0.1.1/flute/Modules/ClaudePromptProcessor.py
--rw-rw-rw-   0        0        0     2992 2024-05-28 13:18:53.000000 FLUTE-LLM-0.1.1/flute/Modules/GPTPromptProcessor.py
--rw-rw-rw-   0        0        0     3662 2024-05-28 13:29:38.000000 FLUTE-LLM-0.1.1/flute/Modules/GeminiPromptProcessor.py
--rw-rw-rw-   0        0        0     1824 2024-05-30 10:41:27.000000 FLUTE-LLM-0.1.1/flute/Modules/PromptProcessorFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.1/flute/Modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.270852 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/
--rw-rw-rw-   0        0        0     4286 2024-05-28 13:00:25.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4188 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4912 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4565 2024-05-28 13:29:45.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     2092 2024-05-30 10:59:54.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc
--rw-rw-rw-   0        0        0      178 2024-05-28 11:35:01.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.273661 FLUTE-LLM-0.1.1/flute/Test/
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.1/flute/Test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.277166 FLUTE-LLM-0.1.1/flute/Test/__pycache__/
--rw-rw-rw-   0        0        0      175 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.1/flute/Test/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    14769 2024-05-30 11:03:19.000000 FLUTE-LLM-0.1.1/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc
--rw-rw-rw-   0        0        0     2786 2024-05-30 11:03:01.000000 FLUTE-LLM-0.1.1/flute/Test/test_prompt_processors.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.1/flute/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.278949 FLUTE-LLM-0.1.1/flute/__pycache__/
--rw-rw-rw-   0        0        0      170 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.1/flute/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       42 2024-05-30 11:16:25.282450 FLUTE-LLM-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      842 2024-05-30 11:15:21.000000 FLUTE-LLM-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.379386 FLUTE-LLM-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.344123 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/
+-rw-rw-rw-   0        0        0     4055 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4055 2024-05-30 11:25:26.379386 FLUTE-LLM-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3648 2024-05-30 11:24:01.000000 FLUTE-LLM-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.344123 FLUTE-LLM-0.1.2/flute/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.360294 FLUTE-LLM-0.1.2/flute/Modules/
+-rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.2/flute/Modules/AbstractPromptProcessor.py
+-rw-rw-rw-   0        0        0     2450 2024-05-28 13:04:00.000000 FLUTE-LLM-0.1.2/flute/Modules/ClaudePromptProcessor.py
+-rw-rw-rw-   0        0        0     2992 2024-05-28 13:18:53.000000 FLUTE-LLM-0.1.2/flute/Modules/GPTPromptProcessor.py
+-rw-rw-rw-   0        0        0     3662 2024-05-28 13:29:38.000000 FLUTE-LLM-0.1.2/flute/Modules/GeminiPromptProcessor.py
+-rw-rw-rw-   0        0        0     1824 2024-05-30 10:41:27.000000 FLUTE-LLM-0.1.2/flute/Modules/PromptProcessorFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.2/flute/Modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.368981 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/
+-rw-rw-rw-   0        0        0     4286 2024-05-28 13:00:25.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4188 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4912 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4565 2024-05-28 13:29:45.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2092 2024-05-30 10:59:54.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc
+-rw-rw-rw-   0        0        0      178 2024-05-28 11:35:01.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.371442 FLUTE-LLM-0.1.2/flute/Test/
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.2/flute/Test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.371442 FLUTE-LLM-0.1.2/flute/Test/__pycache__/
+-rw-rw-rw-   0        0        0      175 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.2/flute/Test/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14769 2024-05-30 11:03:19.000000 FLUTE-LLM-0.1.2/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc
+-rw-rw-rw-   0        0        0     2786 2024-05-30 11:03:01.000000 FLUTE-LLM-0.1.2/flute/Test/test_prompt_processors.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.2/flute/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.371442 FLUTE-LLM-0.1.2/flute/__pycache__/
+-rw-rw-rw-   0        0        0      170 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.2/flute/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:25:26.379386 FLUTE-LLM-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      842 2024-05-30 11:25:10.000000 FLUTE-LLM-0.1.2/setup.py
```

### Comparing `FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/PKG-INFO` & `FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -31,14 +31,23 @@
 
 model_name = "claude-3-haiku-20240307"
 api_key = "your_api_key"
 
 prompt_processor = PromptProcessorFactory.create_prompt_processor(model_name, api_key)
 ```
 
+For Claude, GPT, and Gemini, you may simply write:
+```python
+from PromptProcessorFactory import PromptProcessorFactory
+
+model_name = "claude-3-haiku-20240307"
+
+prompt_processor = PromptProcessorFactory.create_prompt_processor(model_name)
+```
+
 The `create_prompt_processor` method will return an instance of the appropriate prompt processor class based on the provided model name.
 
 ### Generating a Response
 
 To generate a response using the prompt processor, call the `generate_response` method with the desired parameters:
 
 ```python
```

### Comparing `FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/SOURCES.txt` & `FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/LICENSE` & `FLUTE-LLM-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/PKG-INFO` & `FLUTE-LLM-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -31,14 +31,23 @@
 
 model_name = "claude-3-haiku-20240307"
 api_key = "your_api_key"
 
 prompt_processor = PromptProcessorFactory.create_prompt_processor(model_name, api_key)
 ```
 
+For Claude, GPT, and Gemini, you may simply write:
+```python
+from PromptProcessorFactory import PromptProcessorFactory
+
+model_name = "claude-3-haiku-20240307"
+
+prompt_processor = PromptProcessorFactory.create_prompt_processor(model_name)
+```
+
 The `create_prompt_processor` method will return an instance of the appropriate prompt processor class based on the provided model name.
 
 ### Generating a Response
 
 To generate a response using the prompt processor, call the `generate_response` method with the desired parameters:
 
 ```python
```

### Comparing `FLUTE-LLM-0.1.1/README.md` & `FLUTE-LLM-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 
 model_name = "claude-3-haiku-20240307"
 api_key = "your_api_key"
 
 prompt_processor = PromptProcessorFactory.create_prompt_processor(model_name, api_key)
 ```
 
+For Claude, GPT, and Gemini, you may simply write:
+```python
+from PromptProcessorFactory import PromptProcessorFactory
+
+model_name = "claude-3-haiku-20240307"
+
+prompt_processor = PromptProcessorFactory.create_prompt_processor(model_name)
+```
+
 The `create_prompt_processor` method will return an instance of the appropriate prompt processor class based on the provided model name.
 
 ### Generating a Response
 
 To generate a response using the prompt processor, call the `generate_response` method with the desired parameters:
 
 ```python
```

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/AbstractPromptProcessor.py` & `FLUTE-LLM-0.1.2/flute/Modules/AbstractPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/ClaudePromptProcessor.py` & `FLUTE-LLM-0.1.2/flute/Modules/ClaudePromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/GPTPromptProcessor.py` & `FLUTE-LLM-0.1.2/flute/Modules/GPTPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/GeminiPromptProcessor.py` & `FLUTE-LLM-0.1.2/flute/Modules/GeminiPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/PromptProcessorFactory.py` & `FLUTE-LLM-0.1.2/flute/Modules/PromptProcessorFactory.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc` & `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc` & `FLUTE-LLM-0.1.2/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/flute/Test/test_prompt_processors.py` & `FLUTE-LLM-0.1.2/flute/Test/test_prompt_processors.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.1/setup.py` & `FLUTE-LLM-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FLUTE-LLM',
-    version='0.1.1',
+    version='0.1.2',
     description='A package for prompt processing and language model interaction',
     author='The Pioneer',
     url='https://github.com/thepioneerjp/FLUTE',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

