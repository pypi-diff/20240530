# Comparing `tmp/llama_parse-0.4.2.tar.gz` & `tmp/llama_parse-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_parse-0.4.2.tar", max compression
+gzip compressed data, was "llama_parse-0.4.3.tar", max compression
```

## Comparing `llama_parse-0.4.2.tar` & `llama_parse-0.4.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-25 02:41:07.980219 llama_parse-0.4.2/LICENSE
--rw-r--r--   0        0        0     2858 2024-04-25 02:41:07.980219 llama_parse-0.4.2/README.md
--rw-r--r--   0        0        0       92 2024-04-25 02:41:07.992219 llama_parse-0.4.2/llama_parse/__init__.py
--rw-r--r--   0        0        0    12892 2024-04-25 02:41:07.992219 llama_parse-0.4.2/llama_parse/base.py
--rw-r--r--   0        0        0     2819 2024-04-25 02:41:07.996219 llama_parse-0.4.2/llama_parse/utils.py
--rw-r--r--   0        0        0      483 2024-04-25 02:41:07.996219 llama_parse-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 llama_parse-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-14 18:48:16.747032 llama_parse-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2858 2024-05-14 18:48:16.747032 llama_parse-0.4.3/README.md
+-rw-r--r--   0        0        0       92 2024-05-14 18:48:16.759033 llama_parse-0.4.3/llama_parse/__init__.py
+-rw-r--r--   0        0        0    13294 2024-05-14 18:48:16.759033 llama_parse-0.4.3/llama_parse/base.py
+-rw-r--r--   0        0        0     2819 2024-05-14 18:48:16.759033 llama_parse-0.4.3/llama_parse/utils.py
+-rw-r--r--   0        0        0      483 2024-05-14 18:48:16.763033 llama_parse-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3451 1970-01-01 00:00:00.000000 llama_parse-0.4.3/PKG-INFO
```

### Comparing `llama_parse-0.4.2/LICENSE` & `llama_parse-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_parse-0.4.2/README.md` & `llama_parse-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `llama_parse-0.4.2/llama_parse/base.py` & `llama_parse-0.4.3/llama_parse/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,22 @@
     )
     language: Language = Field(
         default=Language.ENGLISH, description="The language of the text to parse."
     )
     parsing_instruction: Optional[str] = Field(
         default="", description="The parsing instruction for the parser."
     )
+    gpt4o_mode: bool = Field(
+        default=False,
+        description="Whether to use gpt-4o extract text from documents.",
+    )
+    gpt4o_api_key: Optional[str] = Field(
+        default=None,
+        description="The API key for the GPT-4o API. Lowers the cost of parsing.",
+    )
     ignore_errors: bool = Field(
         default=True,
         description="Whether or not to ignore and skip errors raised during parsing.",
     )
 
     @validator("api_key", pre=True, always=True)
     def validate_api_key(cls, v: str) -> str:
@@ -109,14 +117,16 @@
                 response = await client.post(
                     url,
                     files=files,
                     headers=headers,
                     data={
                         "language": self.language.value,
                         "parsing_instruction": self.parsing_instruction,
+                        "gpt4o_mode": self.gpt4o_mode,
+                        "gpt4o_api_key": self.gpt4o_api_key,
                     },
                 )
                 if not response.is_success:
                     raise Exception(f"Failed to parse the file: {response.text}")
 
         # check the status of the job, return when done
         job_id = response.json()["id"]
```

### Comparing `llama_parse-0.4.2/llama_parse/utils.py` & `llama_parse-0.4.3/llama_parse/utils.py`

 * *Files identical despite different names*

### Comparing `llama_parse-0.4.2/PKG-INFO` & `llama_parse-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-parse
-Version: 0.4.2
+Version: 0.4.3
 Summary: Parse files into RAG-Optimized formats.
 License: MIT
 Author: Logan Markewich
 Author-email: logan@llamaindex.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

