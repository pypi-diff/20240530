# Comparing `tmp/llama_index_llms_vertex-0.1.7.tar.gz` & `tmp/llama_index_llms_vertex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_vertex-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_llms_vertex-0.1.8.tar", max compression
```

## Comparing `llama_index_llms_vertex-0.1.7.tar` & `llama_index_llms_vertex-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       38 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/README.md
--rw-r--r--   0        0        0       70 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/__init__.py
--rw-r--r--   0        0        0    14285 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/base.py
--rw-r--r--   0        0        0     2098 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/gemini_utils.py
--rw-r--r--   0        0        0     7793 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/utils.py
--rw-r--r--   0        0        0     1477 2024-05-28 18:37:10.319570 llama_index_llms_vertex-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 llama_index_llms_vertex-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-05-30 02:13:55.750596 llama_index_llms_vertex-0.1.8/README.md
+-rw-r--r--   0        0        0       70 2024-05-30 02:13:55.750596 llama_index_llms_vertex-0.1.8/llama_index/llms/vertex/__init__.py
+-rw-r--r--   0        0        0    14098 2024-05-30 02:13:55.750596 llama_index_llms_vertex-0.1.8/llama_index/llms/vertex/base.py
+-rw-r--r--   0        0        0     2098 2024-05-30 02:13:55.750596 llama_index_llms_vertex-0.1.8/llama_index/llms/vertex/gemini_utils.py
+-rw-r--r--   0        0        0     7793 2024-05-30 02:13:55.750596 llama_index_llms_vertex-0.1.8/llama_index/llms/vertex/utils.py
+-rw-r--r--   0        0        0     1477 2024-05-30 02:13:55.750596 llama_index_llms_vertex-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 llama_index_llms_vertex-0.1.8/PKG-INFO
```

### Comparing `llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/base.py` & `llama_index_llms_vertex-0.1.8/llama_index/llms/vertex/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,14 @@
     model: str = Field(description="The vertex model to use.")
     temperature: float = Field(description="The temperature to use for sampling.")
     max_tokens: int = Field(description="The maximum number of tokens to generate.")
     examples: Optional[Sequence[ChatMessage]] = Field(
         description="Example messages for the chat model."
     )
     max_retries: int = Field(default=10, description="The maximum number of retries.")
-    safety_settings: Optional[SafetySettingsType] = Field(
-        default=None, description="Safety settings for the Vertex AI model."
-    )
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict, description="Additional kwargs for the Vertex."
     )
     iscode: bool = Field(
         default=False, description="Flag to determine if current model is a Code Model"
     )
     _is_gemini: bool = PrivateAttr()
@@ -142,15 +139,14 @@
             temperature=temperature,
             max_tokens=max_tokens,
             additional_kwargs=additional_kwargs,
             max_retries=max_retries,
             model=model,
             examples=examples,
             iscode=iscode,
-            safety_settings=safety_settings,
             callback_manager=callback_manager,
             system_prompt=system_prompt,
             messages_to_prompt=messages_to_prompt,
             completion_to_prompt=completion_to_prompt,
             pydantic_program_mode=pydantic_program_mode,
             output_parser=output_parser,
         )
```

### Comparing `llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/gemini_utils.py` & `llama_index_llms_vertex-0.1.8/llama_index/llms/vertex/gemini_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_vertex-0.1.7/llama_index/llms/vertex/utils.py` & `llama_index_llms_vertex-0.1.8/llama_index/llms/vertex/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_vertex-0.1.7/pyproject.toml` & `llama_index_llms_vertex-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms vertex integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-vertex"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 google-cloud-aiplatform = "^1.39.0"
 pyarrow = "^15.0.2"
```

### Comparing `llama_index_llms_vertex-0.1.7/PKG-INFO` & `llama_index_llms_vertex-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-vertex
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index llms vertex integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

