# Comparing `tmp/FLUTE-LLM-0.1.2.tar.gz` & `tmp/FLUTE-LLM-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLUTE-LLM-0.1.2.tar", last modified: Thu May 30 11:25:26 2024, max compression
+gzip compressed data, was "FLUTE-LLM-0.1.3.tar", last modified: Thu May 30 11:48:23 2024, max compression
```

## Comparing `FLUTE-LLM-0.1.2.tar` & `FLUTE-LLM-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.379386 FLUTE-LLM-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.344123 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/
--rw-rw-rw-   0        0        0     4055 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-30 11:25:26.000000 FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4055 2024-05-30 11:25:26.379386 FLUTE-LLM-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3648 2024-05-30 11:24:01.000000 FLUTE-LLM-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.344123 FLUTE-LLM-0.1.2/flute/
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.360294 FLUTE-LLM-0.1.2/flute/Modules/
--rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.2/flute/Modules/AbstractPromptProcessor.py
--rw-rw-rw-   0        0        0     2450 2024-05-28 13:04:00.000000 FLUTE-LLM-0.1.2/flute/Modules/ClaudePromptProcessor.py
--rw-rw-rw-   0        0        0     2992 2024-05-28 13:18:53.000000 FLUTE-LLM-0.1.2/flute/Modules/GPTPromptProcessor.py
--rw-rw-rw-   0        0        0     3662 2024-05-28 13:29:38.000000 FLUTE-LLM-0.1.2/flute/Modules/GeminiPromptProcessor.py
--rw-rw-rw-   0        0        0     1824 2024-05-30 10:41:27.000000 FLUTE-LLM-0.1.2/flute/Modules/PromptProcessorFactory.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.2/flute/Modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.368981 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/
--rw-rw-rw-   0        0        0     4286 2024-05-28 13:00:25.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4188 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4912 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     4565 2024-05-28 13:29:45.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc
--rw-rw-rw-   0        0        0     2092 2024-05-30 10:59:54.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc
--rw-rw-rw-   0        0        0      178 2024-05-28 11:35:01.000000 FLUTE-LLM-0.1.2/flute/Modules/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.371442 FLUTE-LLM-0.1.2/flute/Test/
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.2/flute/Test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.371442 FLUTE-LLM-0.1.2/flute/Test/__pycache__/
--rw-rw-rw-   0        0        0      175 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.2/flute/Test/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    14769 2024-05-30 11:03:19.000000 FLUTE-LLM-0.1.2/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc
--rw-rw-rw-   0        0        0     2786 2024-05-30 11:03:01.000000 FLUTE-LLM-0.1.2/flute/Test/test_prompt_processors.py
--rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.2/flute/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:25:26.371442 FLUTE-LLM-0.1.2/flute/__pycache__/
--rw-rw-rw-   0        0        0      170 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.2/flute/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       42 2024-05-30 11:25:26.379386 FLUTE-LLM-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      842 2024-05-30 11:25:10.000000 FLUTE-LLM-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.144719 FLUTE-LLM-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.079213 FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/
+-rw-rw-rw-   0        0        0     4055 2024-05-30 11:48:22.000000 FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2024-05-30 11:48:22.000000 FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 11:48:22.000000 FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-30 11:48:22.000000 FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-30 11:48:22.000000 FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3774 2024-05-28 10:54:43.000000 FLUTE-LLM-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4055 2024-05-30 11:48:23.143044 FLUTE-LLM-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3648 2024-05-30 11:24:01.000000 FLUTE-LLM-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.079213 FLUTE-LLM-0.1.3/flute/
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.117834 FLUTE-LLM-0.1.3/flute/Modules/
+-rw-rw-rw-   0        0        0     2606 2024-05-28 13:00:12.000000 FLUTE-LLM-0.1.3/flute/Modules/AbstractPromptProcessor.py
+-rw-rw-rw-   0        0        0     2478 2024-05-30 11:46:57.000000 FLUTE-LLM-0.1.3/flute/Modules/ClaudePromptProcessor.py
+-rw-rw-rw-   0        0        0     3020 2024-05-30 11:47:07.000000 FLUTE-LLM-0.1.3/flute/Modules/GPTPromptProcessor.py
+-rw-rw-rw-   0        0        0     3690 2024-05-30 11:46:55.000000 FLUTE-LLM-0.1.3/flute/Modules/GeminiPromptProcessor.py
+-rw-rw-rw-   0        0        0     1894 2024-05-30 11:45:52.000000 FLUTE-LLM-0.1.3/flute/Modules/PromptProcessorFactory.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.3/flute/Modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.134683 FLUTE-LLM-0.1.3/flute/Modules/__pycache__/
+-rw-rw-rw-   0        0        0     4286 2024-05-28 13:00:25.000000 FLUTE-LLM-0.1.3/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4188 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.3/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4912 2024-05-28 13:19:39.000000 FLUTE-LLM-0.1.3/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4565 2024-05-28 13:29:45.000000 FLUTE-LLM-0.1.3/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2263 2024-05-30 11:47:26.000000 FLUTE-LLM-0.1.3/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc
+-rw-rw-rw-   0        0        0      178 2024-05-28 11:35:01.000000 FLUTE-LLM-0.1.3/flute/Modules/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.135221 FLUTE-LLM-0.1.3/flute/Test/
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.3/flute/Test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.139783 FLUTE-LLM-0.1.3/flute/Test/__pycache__/
+-rw-rw-rw-   0        0        0      175 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.3/flute/Test/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14769 2024-05-30 11:03:19.000000 FLUTE-LLM-0.1.3/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc
+-rw-rw-rw-   0        0        0     2786 2024-05-30 11:03:01.000000 FLUTE-LLM-0.1.3/flute/Test/test_prompt_processors.py
+-rw-rw-rw-   0        0        0        0 2024-05-28 11:14:08.000000 FLUTE-LLM-0.1.3/flute/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:48:23.141535 FLUTE-LLM-0.1.3/flute/__pycache__/
+-rw-rw-rw-   0        0        0      170 2024-05-28 11:16:17.000000 FLUTE-LLM-0.1.3/flute/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:48:23.144719 FLUTE-LLM-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      842 2024-05-30 11:48:12.000000 FLUTE-LLM-0.1.3/setup.py
```

### Comparing `FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/PKG-INFO` & `FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `FLUTE-LLM-0.1.2/FLUTE_LLM.egg-info/SOURCES.txt` & `FLUTE-LLM-0.1.3/FLUTE_LLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/LICENSE` & `FLUTE-LLM-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/PKG-INFO` & `FLUTE-LLM-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUTE-LLM
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for prompt processing and language model interaction
 Home-page: https://github.com/thepioneerjp/FLUTE
 Author: The Pioneer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `FLUTE-LLM-0.1.2/README.md` & `FLUTE-LLM-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/AbstractPromptProcessor.py` & `FLUTE-LLM-0.1.3/flute/Modules/AbstractPromptProcessor.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/ClaudePromptProcessor.py` & `FLUTE-LLM-0.1.3/flute/Modules/ClaudePromptProcessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # ClaudePromptProcessor.py
 
 from typing import List, Union, Optional
-from AbstractPromptProcessor import AbstractPromptProcessor
+import flute
+from flute.Modules.AbstractPromptProcessor import AbstractPromptProcessor
 
 try:
     import anthropic
 except ImportError:
     anthropic = None
 
 class ClaudePromptProcessor(AbstractPromptProcessor):
```

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/GPTPromptProcessor.py` & `FLUTE-LLM-0.1.3/flute/Modules/GPTPromptProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # GPTPromptProcessor.py
 
 from typing import List, Union, Optional
-from AbstractPromptProcessor import AbstractPromptProcessor
+import flute
+from flute.Modules.AbstractPromptProcessor import AbstractPromptProcessor
 
 try:
     import openai
 except ImportError:
     openai = None
 
 class GPTPromptProcessor(AbstractPromptProcessor):
```

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/GeminiPromptProcessor.py` & `FLUTE-LLM-0.1.3/flute/Modules/GeminiPromptProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # GeminiPromptProcessor.py
 
 from typing import List, Union, Optional
-from AbstractPromptProcessor import AbstractPromptProcessor
+import flute
+from flute.Modules.AbstractPromptProcessor import AbstractPromptProcessor
 
 try:
     import google.generativeai as genai
     import google.generativeai.types as genai_types
     from google.generativeai.types import HarmCategory, HarmBlockThreshold
     import google.ai.generativelanguage as genai_lang
 except ImportError:
```

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/PromptProcessorFactory.py` & `FLUTE-LLM-0.1.3/flute/Modules/PromptProcessorFactory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # PromptProcessorFactory.py
 
 from typing import Optional
 from dotenv import load_dotenv
 import os
 
-from AbstractPromptProcessor import AbstractPromptProcessor
-from ClaudePromptProcessor import ClaudePromptProcessor
-from GPTPromptProcessor import GPTPromptProcessor
-from GeminiPromptProcessor import GeminiPromptProcessor
+import flute
+from flute.Modules.AbstractPromptProcessor import AbstractPromptProcessor
+from flute.Modules.ClaudePromptProcessor import ClaudePromptProcessor
+from flute.Modules.GPTPromptProcessor import GPTPromptProcessor
+from flute.Modules.GeminiPromptProcessor import GeminiPromptProcessor
 
 class PromptProcessorFactory:
     @staticmethod
     def create_prompt_processor(model_name: str, api_key: Optional[str] = None):
         if api_key is None:
             load_dotenv()
```

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.3/flute/Modules/__pycache__/AbstractPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.3/flute/Modules/__pycache__/ClaudePromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.3/flute/Modules/__pycache__/GPTPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc` & `FLUTE-LLM-0.1.3/flute/Modules/__pycache__/GeminiPromptProcessor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc` & `FLUTE-LLM-0.1.3/flute/Modules/__pycache__/PromptProcessorFactory.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xd7575866 (Thu May 30 10:41:27 2024 UTC)
-files sz: 1824
+moddate:  0xf0665866 (Thu May 30 11:45:52 2024 UTC)
+files sz: 1894
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
-      036c045a04640064046c056d055a050100640064056c066d065a06010064
-      0064066c076d075a070100640064076c086d085a08010002004700640884
-      006409a6020000ab0200000000000000005a0964035300
+      036c045a04640064036c055a05640064046c066d075a070100640064056c
+      086d095a090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d01
+      0002004700640884006409a6020000ab0200000000000000005a0e640353
+      00
      0           0 RESUME                   0
    
      3           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Optional',))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (Optional)
                 10 STORE_NAME               1 (Optional)
@@ -29,51 +30,56 @@
    
      5          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               3 (None)
                 30 IMPORT_NAME              4 (os)
                 32 STORE_NAME               4 (os)
    
      7          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               4 (('AbstractPromptProcessor',))
-                38 IMPORT_NAME              5 (AbstractPromptProcessor)
-                40 IMPORT_FROM              5 (AbstractPromptProcessor)
-                42 STORE_NAME               5 (AbstractPromptProcessor)
-                44 POP_TOP
-   
-     8          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               5 (('ClaudePromptProcessor',))
-                50 IMPORT_NAME              6 (ClaudePromptProcessor)
-                52 IMPORT_FROM              6 (ClaudePromptProcessor)
-                54 STORE_NAME               6 (ClaudePromptProcessor)
-                56 POP_TOP
-   
-     9          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               6 (('GPTPromptProcessor',))
-                62 IMPORT_NAME              7 (GPTPromptProcessor)
-                64 IMPORT_FROM              7 (GPTPromptProcessor)
-                66 STORE_NAME               7 (GPTPromptProcessor)
-                68 POP_TOP
-   
-    10          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               7 (('GeminiPromptProcessor',))
-                74 IMPORT_NAME              8 (GeminiPromptProcessor)
-                76 IMPORT_FROM              8 (GeminiPromptProcessor)
-                78 STORE_NAME               8 (GeminiPromptProcessor)
-                80 POP_TOP
-   
-    12          82 PUSH_NULL
-                84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               8 (<code object PromptProcessorFactory, file "C:\Users\j_matsumoto\Documents\GitHub\FLUTE\flute\Test\..\Modules\PromptProcessorFactory.py", line 12>)
-                88 MAKE_FUNCTION            0
-                90 LOAD_CONST               9 ('PromptProcessorFactory')
-                92 PRECALL                  2
-                96 CALL                     2
-               106 STORE_NAME               9 (PromptProcessorFactory)
-               108 LOAD_CONST               3 (None)
-               110 RETURN_VALUE
+                36 LOAD_CONST               3 (None)
+                38 IMPORT_NAME              5 (flute)
+                40 STORE_NAME               5 (flute)
+   
+     8          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               4 (('AbstractPromptProcessor',))
+                46 IMPORT_NAME              6 (flute.Modules.AbstractPromptProcessor)
+                48 IMPORT_FROM              7 (AbstractPromptProcessor)
+                50 STORE_NAME               7 (AbstractPromptProcessor)
+                52 POP_TOP
+   
+     9          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               5 (('ClaudePromptProcessor',))
+                58 IMPORT_NAME              8 (flute.Modules.ClaudePromptProcessor)
+                60 IMPORT_FROM              9 (ClaudePromptProcessor)
+                62 STORE_NAME               9 (ClaudePromptProcessor)
+                64 POP_TOP
+   
+    10          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               6 (('GPTPromptProcessor',))
+                70 IMPORT_NAME             10 (flute.Modules.GPTPromptProcessor)
+                72 IMPORT_FROM             11 (GPTPromptProcessor)
+                74 STORE_NAME              11 (GPTPromptProcessor)
+                76 POP_TOP
+   
+    11          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               7 (('GeminiPromptProcessor',))
+                82 IMPORT_NAME             12 (flute.Modules.GeminiPromptProcessor)
+                84 IMPORT_FROM             13 (GeminiPromptProcessor)
+                86 STORE_NAME              13 (GeminiPromptProcessor)
+                88 POP_TOP
+   
+    13          90 PUSH_NULL
+                92 LOAD_BUILD_CLASS
+                94 LOAD_CONST               8 (<code object PromptProcessorFactory, file "C:\Users\j_matsumoto\Documents\GitHub\FLUTE\flute\Test\..\Modules\PromptProcessorFactory.py", line 13>)
+                96 MAKE_FUNCTION            0
+                98 LOAD_CONST               9 ('PromptProcessorFactory')
+               100 PRECALL                  2
+               104 CALL                     2
+               114 STORE_NAME              14 (PromptProcessorFactory)
+               116 LOAD_CONST               3 (None)
+               118 RETURN_VALUE
    consts
       0
       ('Optional',)
       ('load_dotenv',)
       None
       ('AbstractPromptProcessor',)
       ('ClaudePromptProcessor',)
@@ -84,37 +90,37 @@
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a0265036405640265046403650565041900000000
             0000000000660464048405a6000000ab0000000000000000005a06640153
             00
-          12           0 RESUME                   0
+          13           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('PromptProcessorFactory')
                        8 STORE_NAME               2 (__qualname__)
          
-          13          10 LOAD_NAME                3 (staticmethod)
+          14          10 LOAD_NAME                3 (staticmethod)
          
-          14          12 LOAD_CONST               5 ((None,))
+          15          12 LOAD_CONST               5 ((None,))
                       14 LOAD_CONST               2 ('model_name')
                       16 LOAD_NAME                4 (str)
                       18 LOAD_CONST               3 ('api_key')
                       20 LOAD_NAME                5 (Optional)
                       22 LOAD_NAME                4 (str)
                       24 BINARY_SUBSCR
                       34 BUILD_TUPLE              4
-                      36 LOAD_CONST               4 (<code object create_prompt_processor, file "C:\Users\j_matsumoto\Documents\GitHub\FLUTE\flute\Test\..\Modules\PromptProcessorFactory.py", line 13>)
+                      36 LOAD_CONST               4 (<code object create_prompt_processor, file "C:\Users\j_matsumoto\Documents\GitHub\FLUTE\flute\Test\..\Modules\PromptProcessorFactory.py", line 14>)
                       38 MAKE_FUNCTION            5 (defaults, annotations)
          
-          13          40 PRECALL                  0
+          14          40 PRECALL                  0
                       44 CALL                     0
          
-          14          54 STORE_NAME               6 (create_prompt_processor)
+          15          54 STORE_NAME               6 (create_prompt_processor)
                       56 LOAD_CONST               1 (None)
                       58 RETURN_VALUE
          consts
             'PromptProcessorFactory'
             None
             'model_name'
             'api_key'
@@ -130,84 +136,84 @@
                   00000000007c017c00ac03a6020000ab02000000000000000053007c0064
                   04760072247403000000000000000000006a0200000000000000006405a6
                   010000ab0100000000000000007d017409000000000000000000007c01ac
                   06a6010000ab01000000000000000053007c006407760072257403000000
                   000000000000006a0200000000000000006408a6010000ab010000000000
                   0000007d01740b000000000000000000007c017c00ac03a6020000ab0200
                   00000000000000530064005300
-                13           0 RESUME                   0
+                14           0 RESUME                   0
                
-                15           2 LOAD_FAST                1 (api_key)
+                16           2 LOAD_FAST                1 (api_key)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 34)
                
-                16           6 LOAD_GLOBAL              1 (NULL + load_dotenv)
+                17           6 LOAD_GLOBAL              1 (NULL + load_dotenv)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 POP_TOP
                
-                18     >>   34 LOAD_FAST                0 (model_name)
+                19     >>   34 LOAD_FAST                0 (model_name)
                             36 LOAD_CONST               1 (('claude-3-opus-20240229', 'claude-3-sonnet-20240229', 'claude-3-haiku-20240307'))
                             38 CONTAINS_OP              0
                             40 POP_JUMP_FORWARD_IF_FALSE    37 (to 116)
                
-                23          42 LOAD_GLOBAL              3 (NULL + os)
+                24          42 LOAD_GLOBAL              3 (NULL + os)
                             54 LOAD_ATTR                2 (getenv)
                             64 LOAD_CONST               2 ('ANTHROPIC_API_KEY')
                             66 PRECALL                  1
                             70 CALL                     1
                             80 STORE_FAST               1 (api_key)
                
-                24          82 LOAD_GLOBAL              7 (NULL + ClaudePromptProcessor)
+                25          82 LOAD_GLOBAL              7 (NULL + ClaudePromptProcessor)
                             94 LOAD_FAST                1 (api_key)
                             96 LOAD_FAST                0 (model_name)
                             98 KW_NAMES                 3
                            100 PRECALL                  2
                            104 CALL                     2
                            114 RETURN_VALUE
                
-                25     >>  116 LOAD_FAST                0 (model_name)
+                26     >>  116 LOAD_FAST                0 (model_name)
                            118 LOAD_CONST               4 (('gpt-4o', 'gpt-4o-2024-05-13', 'gpt-4-turbo', 'gpt-4-turbo-2024-04-09', 'gpt-4-turbo-preview', 'gpt-4-0125-preview', 'gpt-4-1106-preview', 'gpt-4-vision-preview', 'gpt-4-1106-vision-preview', 'gpt-4', 'gpt-4-0613', 'gpt-4-32k', 'gpt-4-32k-0613'))
                            120 CONTAINS_OP              0
                            122 POP_JUMP_FORWARD_IF_FALSE    36 (to 196)
                
-                40         124 LOAD_GLOBAL              3 (NULL + os)
+                41         124 LOAD_GLOBAL              3 (NULL + os)
                            136 LOAD_ATTR                2 (getenv)
                            146 LOAD_CONST               5 ('OPENAI_API_KEY')
                            148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               1 (api_key)
                
-                41         164 LOAD_GLOBAL              9 (NULL + GPTPromptProcessor)
+                42         164 LOAD_GLOBAL              9 (NULL + GPTPromptProcessor)
                            176 LOAD_FAST                1 (api_key)
                            178 KW_NAMES                 6
                            180 PRECALL                  1
                            184 CALL                     1
                            194 RETURN_VALUE
                
-                42     >>  196 LOAD_FAST                0 (model_name)
+                43     >>  196 LOAD_FAST                0 (model_name)
                            198 LOAD_CONST               7 (('models/gemini-1.5-pro-latest', 'models/gemini-1.5-flash-latest', 'models/gemini-pro', 'models/gemini-pro-vision'))
                            200 CONTAINS_OP              0
                            202 POP_JUMP_FORWARD_IF_FALSE    37 (to 278)
                
-                48         204 LOAD_GLOBAL              3 (NULL + os)
+                49         204 LOAD_GLOBAL              3 (NULL + os)
                            216 LOAD_ATTR                2 (getenv)
                            226 LOAD_CONST               8 ('GOOGLE_API_KEY')
                            228 PRECALL                  1
                            232 CALL                     1
                            242 STORE_FAST               1 (api_key)
                
-                49         244 LOAD_GLOBAL             11 (NULL + GeminiPromptProcessor)
+                50         244 LOAD_GLOBAL             11 (NULL + GeminiPromptProcessor)
                            256 LOAD_FAST                1 (api_key)
                            258 LOAD_FAST                0 (model_name)
                            260 KW_NAMES                 3
                            262 PRECALL                  2
                            266 CALL                     2
                            276 RETURN_VALUE
                
-                52     >>  278 LOAD_CONST               0 (None)
+                53     >>  278 LOAD_CONST               0 (None)
                            280 RETURN_VALUE
                consts
                   None
                   ('claude-3-opus-20240229', 'claude-3-sonnet-20240229', 'claude-3-haiku-20240307')
                   'ANTHROPIC_API_KEY'
                   ('api_key', 'model')
                   ('gpt-4o', 'gpt-4o-2024-05-13', 'gpt-4-turbo', 'gpt-4-turbo-2024-04-09', 'gpt-4-turbo-preview', 'gpt-4-0125-preview', 'gpt-4-1106-preview', 'gpt-4-vision-preview', 'gpt-4-1106-vision-preview', 'gpt-4', 'gpt-4-0613', 'gpt-4-32k', 'gpt-4-32k-0613')
@@ -217,27 +223,27 @@
                   'GOOGLE_API_KEY'
                names      ('load_dotenv', 'os', 'getenv', 'ClaudePromptProcessor', 'GPTPromptProcessor', 'GeminiPromptProcessor')
                varnames   ('model_name', 'api_key')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\j_matsumoto\\Documents\\GitHub\\FLUTE\\flute\\Test\\..\\Modules\\PromptProcessorFactory.py'
                name       'create_prompt_processor'
-               firstlineno 13
+               firstlineno 14
                lnotab 0x020204011c02080528012201080f28012001080628012203
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'str', 'Optional', 'create_prompt_processor')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\j_matsumoto\\Documents\\GitHub\\FLUTE\\flute\\Test\\..\\Modules\\PromptProcessorFactory.py'
          name       'PromptProcessorFactory'
-         firstlineno 12
+         firstlineno 13
          lnotab 0x0a0102011cff0e01
       'PromptProcessorFactory'
-   names      ('typing', 'Optional', 'dotenv', 'load_dotenv', 'os', 'AbstractPromptProcessor', 'ClaudePromptProcessor', 'GPTPromptProcessor', 'GeminiPromptProcessor', 'PromptProcessorFactory')
+   names      ('typing', 'Optional', 'dotenv', 'load_dotenv', 'os', 'flute', 'flute.Modules.AbstractPromptProcessor', 'AbstractPromptProcessor', 'flute.Modules.ClaudePromptProcessor', 'ClaudePromptProcessor', 'flute.Modules.GPTPromptProcessor', 'GPTPromptProcessor', 'flute.Modules.GeminiPromptProcessor', 'GeminiPromptProcessor', 'PromptProcessorFactory')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\j_matsumoto\\Documents\\GitHub\\FLUTE\\flute\\Test\\..\\Modules\\PromptProcessorFactory.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02030c010c0108020c010c010c010c02
+   lnotab 0x00ff02030c010c01080208010c010c010c010c02
```

### Comparing `FLUTE-LLM-0.1.2/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc` & `FLUTE-LLM-0.1.3/flute/Test/__pycache__/test_prompt_processors.cpython-311-pytest-8.2.1.pyc`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/flute/Test/test_prompt_processors.py` & `FLUTE-LLM-0.1.3/flute/Test/test_prompt_processors.py`

 * *Files identical despite different names*

### Comparing `FLUTE-LLM-0.1.2/setup.py` & `FLUTE-LLM-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FLUTE-LLM',
-    version='0.1.2',
+    version='0.1.3',
     description='A package for prompt processing and language model interaction',
     author='The Pioneer',
     url='https://github.com/thepioneerjp/FLUTE',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
```

