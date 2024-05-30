# Comparing `tmp/langchain_robocorp-0.0.8.tar.gz` & `tmp/langchain_robocorp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_robocorp-0.0.8.tar", max compression
+gzip compressed data, was "langchain_robocorp-0.0.9.tar", max compression
```

## Comparing `langchain_robocorp-0.0.8.tar` & `langchain_robocorp-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/LICENSE
--rw-r--r--   0        0        0      420 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/README.md
--rw-r--r--   0        0        0      102 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/__init__.py
--rw-r--r--   0        0        0     4568 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/_common.py
--rw-r--r--   0        0        0      525 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/_prompts.py
--rw-r--r--   0        0        0        0 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/py.typed
--rw-r--r--   0        0        0     7675 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/toolkits.py
--rw-r--r--   0        0        0     2558 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/LICENSE
+-rw-r--r--   0        0        0      420 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/README.md
+-rw-r--r--   0        0        0      102 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/langchain_robocorp/__init__.py
+-rw-r--r--   0        0        0     5323 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/langchain_robocorp/_common.py
+-rw-r--r--   0        0        0      525 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/langchain_robocorp/_prompts.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/langchain_robocorp/py.typed
+-rw-r--r--   0        0        0     7675 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/langchain_robocorp/toolkits.py
+-rw-r--r--   0        0        0     2558 2024-05-30 16:20:30.422737 langchain_robocorp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.9/PKG-INFO
```

### Comparing `langchain_robocorp-0.0.8/LICENSE` & `langchain_robocorp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.8/langchain_robocorp/_common.py` & `langchain_robocorp-0.0.9/langchain_robocorp/_common.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import time
 from dataclasses import dataclass
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Set, Tuple, Union
 
 from langchain_core.pydantic_v1 import BaseModel, Field, create_model
 from langchain_core.utils.json_schema import dereference_refs
 
 
 @dataclass(frozen=True)
 class ReducedOpenAPISpec:
@@ -89,34 +90,53 @@
         endpoint_spec.get("requestBody", {})
         .get("content", {})
         .get("application/json", {})
         .get("schema", {})
     )
 
 
-def create_field(schema: dict, required: bool) -> Tuple[Any, Any]:
+def create_field(
+    schema: dict, required: bool, created_model_names: Set[str]
+) -> Tuple[Any, Any]:
     """
     Creates a Pydantic field based on the schema definition.
     """
-    field_type = type_mapping.get(schema.get("type", "string"), str)
+    if "anyOf" in schema:
+        field_types = [
+            create_field(sub_schema, required, created_model_names)[0]
+            for sub_schema in schema["anyOf"]
+        ]
+        if len(field_types) == 1:
+            field_type = field_types[0]  # Simplified handling
+        else:
+            field_type = Union[tuple(field_types)]
+    else:
+        field_type = type_mapping.get(schema.get("type", "string"), str)
+
     description = schema.get("description", "")
 
     # Handle nested objects
-    if schema["type"] == "object":
+    if schema.get("type") == "object":
         nested_fields = {
-            k: create_field(v, k in schema.get("required", []))
+            k: create_field(v, k in schema.get("required", []), created_model_names)
             for k, v in schema.get("properties", {}).items()
         }
-        model_name = schema.get("title", "NestedModel")
+        model_name = schema.get("title", f"NestedModel{time.time()}")
+        if model_name in created_model_names:
+            # needs to be unique
+            model_name = model_name + str(time.time())
         nested_model = create_model(model_name, **nested_fields)  # type: ignore
+        created_model_names.add(model_name)
         return nested_model, Field(... if required else None, description=description)
 
     # Handle arrays
-    elif schema["type"] == "array":
-        item_type, _ = create_field(schema["items"], required=True)
+    elif schema.get("type") == "array":
+        item_type, _ = create_field(
+            schema["items"], required=True, created_model_names=created_model_names
+        )
         return List[item_type], Field(  # type: ignore
             ... if required else None, description=description
         )
 
     # Other types
     return field_type, Field(... if required else None, description=description)
 
@@ -124,17 +144,18 @@
 def get_param_fields(endpoint_spec: dict) -> dict:
     """Get an OpenAPI endpoint parameter details"""
     schema = get_schema(endpoint_spec)
     properties = schema.get("properties", {})
     required_fields = schema.get("required", [])
 
     fields = {}
+    created_model_names: Set[str] = set()
     for key, value in properties.items():
         is_required = key in required_fields
-        field_info = create_field(value, is_required)
+        field_info = create_field(value, is_required, created_model_names)
         fields[key] = field_info
 
     return fields
 
 
 def model_to_dict(
     item: Union[BaseModel, List, Dict[str, Any]],
```

### Comparing `langchain_robocorp-0.0.8/langchain_robocorp/_prompts.py` & `langchain_robocorp-0.0.9/langchain_robocorp/_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.8/langchain_robocorp/toolkits.py` & `langchain_robocorp-0.0.9/langchain_robocorp/toolkits.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.8/pyproject.toml` & `langchain_robocorp-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-robocorp"
-version = "0.0.8"
+version = "0.0.9"
 description = "An integration package connecting Robocorp Action Server and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_robocorp-0.0.8/PKG-INFO` & `langchain_robocorp-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-robocorp
-Version: 0.0.8
+Version: 0.0.9
 Summary: An integration package connecting Robocorp Action Server and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

