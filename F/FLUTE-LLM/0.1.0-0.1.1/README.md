# Comparing `tmp/FLUTE-LLM-0.1.0.tar.gz` & `tmp/FLUTE-LLM-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLUTE-LLM-0.1.0.tar", last modified: Tue May 28 14:16:13 2024, max compression
+gzip compressed data, was "FLUTE-LLM-0.1.1.tar", last modified: Thu May 30 11:16:25 2024, max compression
```

## Comparing `FLUTE-LLM-0.1.0.tar` & `FLUTE-LLM-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 14:16:13.498494 FLUTE-LLM-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-28 14:16:13.482868 FLUTE-LLM-0.1.0/FLUTE_LLM.egg-info/
--rw-rw-rw-   0        0        0     3705 2024-05-28 14:16:13.000000 FLUTE-LLM-0.1.0/FLUTE_LLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2024-05-28 14:16:13.000000 FLUTE-LLM-0.1.0/FLUTE_LLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 14:16:13.000000 FLUTE-LLM-0.1.0/FLUTE_LLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-28 14:16:13.000000 FLUTE-LLM-0.1.0/FLUTE_LLM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-28 14:16:13.000000 FLUTE-LLM-0.1.0/FLUTE_LLM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3705 2024-05-28 14:16:13.498494 FLUTE-LLM-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3298 2024-05-28 13:38:39.000000 FLUTE-LLM-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 14:16:13.482868 FLUTE-LLM-0.1.0/flute/
-drwxrwxrwx   0        0        0        0 2024-05-28 14:16:13.498494 FLUTE-LLM-0.1.0/flute/Modules/
--rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.0/flute/Modules/AbstractPromptProcessor.py
--rw-rw-rw-   0        0        0     2450 2024-05-28 13:04:00.000000 FLUTE-LLM-0.1.0/flute/Modules/ClaudePromptProcessor.py
--rw-rw-rw-   0        0        0     2992 2024-05-28 13:18:53.000000 FLUTE-LLM-0.1.0/flute/Modules/GPTPromptProcessor.py
--rw-rw-rw-   0        0        0     3662 2024-05-28 13:29:38.000000 FLUTE-LLM-0.1.0/flute/Modules/GeminiPromptProcessor.py
--rw-rw-rw-   0        0        0     1567 2024-05-28 11:37:39.000000 FLUTE-LLM-0.1.0/flute/Modules/PromptProcessorFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.0/flute/Modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:16:13.498494 FLUTE-LLM-0.1.0/flute/Test/
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.0/flute/Test/__init__.py
--rw-rw-rw-   0        0        0     1427 2024-05-28 12:41:42.000000 FLUTE-LLM-0.1.0/flute/Test/test_prompt_processors.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.0/flute/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-28 14:16:13.498494 FLUTE-LLM-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      704 2024-05-28 14:15:52.000000 FLUTE-LLM-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.281091 FLUTE-LLM-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.213816 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/
+-rw-rw-rw-   0        0        0     3803 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 11:16:25.000000 FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3803 2024-05-30 11:16:25.281091 FLUTE-LLM-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3396 2024-05-30 11:07:52.000000 FLUTE-LLM-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.214817 FLUTE-LLM-0.1.1/flute/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.256104 FLUTE-LLM-0.1.1/flute/Modules/
+-rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.1/flute/Modules/AbstractPromptProcessor.py
+-rw-rw-rw-   0        0        0     2450 2024-05-28 13:04:00.000000 FLUTE-LLM-0.1.1/flute/Modules/ClaudePromptProcessor.py
+-rw-rw-rw-   0        0        0     2992 2024-05-28 13:18:53.000000 FLUTE-LLM-0.1.1/flute/Modules/GPTPromptProcessor.py
+-rw-rw-rw-   0        0        0     3662 2024-05-28 13:29:38.000000 FLUTE-LLM-0.1.1/flute/Modules/GeminiPromptProcessor.py
+-rw-rw-rw-   0        0        0     1824 2024-05-30 10:41:27.000000 FLUTE-LLM-0.1.1/flute/Modules/PromptProcessorFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.1/flute/Modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.270852 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/
+-rw-rw-rw-   0        0        0     4286 2024-05-28 13:00:25.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4188 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4912 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4565 2024-05-28 13:29:45.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2092 2024-05-30 10:59:54.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc
+-rw-rw-rw-   0        0        0      178 2024-05-28 11:35:01.000000 FLUTE-LLM-0.1.1/flute/Modules/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.273661 FLUTE-LLM-0.1.1/flute/Test/
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.1/flute/Test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.277166 FLUTE-LLM-0.1.1/flute/Test/__pycache__/
+-rw-rw-rw-   0        0        0      175 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.1/flute/Test/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14769 2024-05-30 11:03:19.000000 FLUTE-LLM-0.1.1/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc
+-rw-rw-rw-   0        0        0     2786 2024-05-30 11:03:01.000000 FLUTE-LLM-0.1.1/flute/Test/test_prompt_processors.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.1/flute/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:16:25.278949 FLUTE-LLM-0.1.1/flute/__pycache__/
+-rw-rw-rw-   0        0        0      170 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.1/flute/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:16:25.282450 FLUTE-LLM-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      842 2024-05-30 11:15:21.000000 FLUTE-LLM-0.1.1/setup.py
```

### Comparing `FLUTE-LLM-0.1.0/FLUTE_LLM.egg-info/PKG-INFO` & `FLUTE-LLM-0.1.1/FLUTE_LLM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLUTE
 FLUTE: Flexible Language Unified Tuning Elixir. Provides a factory and an abstract object for LLMs, and possibly BCIs in the future.
 
+## Installation
+
+You can install FLUTE using pip:
+```
+pip install FLUTE-LLM
+```
+
 ## Usage
 
 ### Creating a Prompt Processor
 
 To create a prompt processor, use the `PromptProcessorFactory` class and call the `create_prompt_processor` method with the desired model name and API key:
 
 ```python
@@ -36,15 +43,15 @@
 
 ```python
 prompt = "What is the capital of France?"
 response = prompt_processor.generate_response(prompt, max_tokens=100, temperature=0.8)
 print(response)
 ```
 
-The `generate_response` method takes various parameters to control the generation process, such as `max_tokens`, `temperature`, `top_p`, etc. Refer to the specific prompt processor class documentation for more details on the available parameters.
+The `generate_response` method takes various parameters to control the generation process, such as `max_tokens`, `temperature`, `top_p`, `system`, etc. Refer to the specific prompt processor class documentation for more details on the available parameters.
 
 ### Class Diagram
 
 ```mermaid
 classDiagram
     AbstractPromptProcessor <|-- ClaudePromptProcessor
     AbstractPromptProcessor <|-- GPTPromptProcessor
```

### Comparing `FLUTE-LLM-0.1.0/LICENSE` & `FLUTE-LLM-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.0/PKG-INFO` & `FLUTE-LLM-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLUTE
 FLUTE: Flexible Language Unified Tuning Elixir. Provides a factory and an abstract object for LLMs, and possibly BCIs in the future.
 
+## Installation
+
+You can install FLUTE using pip:
+```
+pip install FLUTE-LLM
+```
+
 ## Usage
 
 ### Creating a Prompt Processor
 
 To create a prompt processor, use the `PromptProcessorFactory` class and call the `create_prompt_processor` method with the desired model name and API key:
 
 ```python
@@ -36,15 +43,15 @@
 
 ```python
 prompt = "What is the capital of France?"
 response = prompt_processor.generate_response(prompt, max_tokens=100, temperature=0.8)
 print(response)
 ```
 
-The `generate_response` method takes various parameters to control the generation process, such as `max_tokens`, `temperature`, `top_p`, etc. Refer to the specific prompt processor class documentation for more details on the available parameters.
+The `generate_response` method takes various parameters to control the generation process, such as `max_tokens`, `temperature`, `top_p`, `system`, etc. Refer to the specific prompt processor class documentation for more details on the available parameters.
 
 ### Class Diagram
 
 ```mermaid
 classDiagram
     AbstractPromptProcessor <|-- ClaudePromptProcessor
     AbstractPromptProcessor <|-- GPTPromptProcessor
```

### Comparing `FLUTE-LLM-0.1.0/README.md` & `FLUTE-LLM-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # FLUTE
 FLUTE: Flexible Language Unified Tuning Elixir. Provides a factory and an abstract object for LLMs, and possibly BCIs in the future.
 
+## Installation
+
+You can install FLUTE using pip:
+```
+pip install FLUTE-LLM
+```
+
 ## Usage
 
 ### Creating a Prompt Processor
 
 To create a prompt processor, use the `PromptProcessorFactory` class and call the `create_prompt_processor` method with the desired model name and API key:
 
 ```python
@@ -24,15 +31,15 @@
 
 ```python
 prompt = "What is the capital of France?"
 response = prompt_processor.generate_response(prompt, max_tokens=100, temperature=0.8)
 print(response)
 ```
 
-The `generate_response` method takes various parameters to control the generation process, such as `max_tokens`, `temperature`, `top_p`, etc. Refer to the specific prompt processor class documentation for more details on the available parameters.
+The `generate_response` method takes various parameters to control the generation process, such as `max_tokens`, `temperature`, `top_p`, `system`, etc. Refer to the specific prompt processor class documentation for more details on the available parameters.
 
 ### Class Diagram
 
 ```mermaid
 classDiagram
     AbstractPromptProcessor <|-- ClaudePromptProcessor
     AbstractPromptProcessor <|-- GPTPromptProcessor
```

### Comparing `FLUTE-LLM-0.1.0/flute/Modules/AbstractPromptProcessor.py` & `FLUTE-LLM-0.1.1/flute/Modules/AbstractPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.0/flute/Modules/ClaudePromptProcessor.py` & `FLUTE-LLM-0.1.1/flute/Modules/ClaudePromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.0/flute/Modules/GPTPromptProcessor.py` & `FLUTE-LLM-0.1.1/flute/Modules/GPTPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.0/flute/Modules/GeminiPromptProcessor.py` & `FLUTE-LLM-0.1.1/flute/Modules/GeminiPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.0/flute/Test/test_prompt_processors.py` & `FLUTE-LLM-0.1.1/flute/Test/test_prompt_processors.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,26 +13,46 @@
 
 def test_create_claude_prompt_processor():
     api_key = os.getenv("ANTHROPIC_API_KEY")
     processor = PromptProcessorFactory.create_prompt_processor("claude-3-haiku-20240307", api_key=api_key)
     assert processor.api_key == api_key
     assert processor.model == "claude-3-haiku-20240307"
 
-    response = processor.generate_response("Hello, how are you?")
+    response = processor.generate_response("Hello, how are you?", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
+    assert isinstance(response, str)
+
+def test_create_claude_prompt_processor_without_api_key():
+    processor = PromptProcessorFactory.create_prompt_processor("claude-3-haiku-20240307")
+    assert processor.model == "claude-3-haiku-20240307"
+
+    response = processor.generate_response("Hello, how are you?", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
     assert isinstance(response, str)
 
 def test_create_gpt_prompt_processor():
     api_key = os.getenv("OPENAI_API_KEY")
     processor = PromptProcessorFactory.create_prompt_processor("gpt-4o", api_key=api_key)
     assert processor.api_key == api_key
 
-    response = processor.generate_response("Hello, how are you?", model="gpt-4o")
+    response = processor.generate_response("Hello, how are you?", model="gpt-4o", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
+    assert isinstance(response, str)
+
+def test_create_gpt_prompt_processor_without_api_key():
+    processor = PromptProcessorFactory.create_prompt_processor("gpt-4o")
+
+    response = processor.generate_response("Hello, how are you?", model="gpt-4o", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
     assert isinstance(response, str)
 
 def test_create_gemini_prompt_processor():
     api_key = os.getenv("GOOGLE_API_KEY")
     processor = PromptProcessorFactory.create_prompt_processor("models/gemini-1.5-flash-latest", api_key=api_key)
     assert processor.api_key == api_key
     assert processor.model.model_name == "models/gemini-1.5-flash-latest"
 
-    response = processor.generate_response("Hello, how are you?")
+    response = processor.generate_response("Hello, how are you?", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
+    assert isinstance(response, str)
+
+def test_create_gemini_prompt_processor_without_api_key():
+    processor = PromptProcessorFactory.create_prompt_processor("models/gemini-1.5-flash-latest")
+    assert processor.model.model_name == "models/gemini-1.5-flash-latest"
+
+    response = processor.generate_response("Hello, how are you?", max_tokens=4096, temperature=1.0, top_p=1, system="You are an assistant")
     assert isinstance(response, str)
```

### Comparing `FLUTE-LLM-0.1.0/setup.py` & `FLUTE-LLM-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FLUTE-LLM',
-    version='0.1.0',
+    version='0.1.1',
     description='A package for prompt processing and language model interaction',
     author='The Pioneer',
     url='https://github.com/thepioneerjp/FLUTE',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'openai',
         'anthropic',
         'google-generativeai',
         'python-dotenv',
-        'pytest'
+        'pytest',
     ],
+    package_data={
+        '': ['*.txt', '*.md', '*.json', '*.csv', '*.yaml', '*.yml', "LICENSE"],
+        'flute': ['**/*'],
+    },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
     ],
 )
```

