# Comparing `tmp/lazy_schema-0.3.0.tar.gz` & `tmp/lazy_schema-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_schema-0.3.0.tar", max compression
+gzip compressed data, was "lazy_schema-0.3.1.tar", max compression
```

## Comparing `lazy_schema-0.3.0.tar` & `lazy_schema-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4137 2024-05-23 01:52:28.879909 lazy_schema-0.3.0/README.md
--rw-r--r--   0        0        0       71 2024-05-23 01:52:28.619910 lazy_schema-0.3.0/lazy_schema/__init__.py
--rw-r--r--   0        0        0     5229 2024-05-23 01:52:28.619910 lazy_schema-0.3.0/lazy_schema/schema.py
--rw-r--r--   0        0        0     2669 2024-05-23 01:52:28.619910 lazy_schema-0.3.0/lazy_schema/schema_pool.py
--rw-r--r--   0        0        0      278 2024-05-23 01:52:28.855909 lazy_schema-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4636 1970-01-01 00:00:00.000000 lazy_schema-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4137 2024-05-23 01:52:28.879909 lazy_schema-0.3.1/README.md
+-rw-r--r--   0        0        0       71 2024-05-23 01:52:28.619910 lazy_schema-0.3.1/lazy_schema/__init__.py
+-rw-r--r--   0        0        0     5361 2024-05-30 03:11:59.226253 lazy_schema-0.3.1/lazy_schema/schema.py
+-rw-r--r--   0        0        0     2687 2024-05-30 03:09:15.417609 lazy_schema-0.3.1/lazy_schema/schema_pool.py
+-rw-r--r--   0        0        0      278 2024-05-30 03:13:45.631548 lazy_schema-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4636 1970-01-01 00:00:00.000000 lazy_schema-0.3.1/PKG-INFO
```

### Comparing `lazy_schema-0.3.0/README.md` & `lazy_schema-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lazy_schema-0.3.0/lazy_schema/schema.py` & `lazy_schema-0.3.1/lazy_schema/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Any, NamedTuple, Union, Dict, TYPE_CHECKING
+from typing import Any, NamedTuple, Optional, Union, Dict, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from schema_pool import SchemaPool
 
 
 def _null_coalesce(*args):
     for arg in args:
@@ -18,15 +18,15 @@
     default_fields: dict
     discrete: bool
     no_default: bool
     no_null: bool
 
     def __call__(
         self,
-        *args: dict,
+        *args: Optional[dict],
         __discrete__: bool = None,  # type: ignore
         __no_default__: bool = None,  # type: ignore
         __no_null__: bool = None,  # type: ignore
         **kwargs,
     ) -> dict:
         """
         :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
@@ -34,14 +34,17 @@
         :__no_default__: When `true`, default values are excluded.
 
         :__no_null__: When `true`, `null` values will never be included.
         """
         fields: Dict[str, Any] = {}
 
         for arg in args:
+            if arg == None:
+                continue
+
             for key in arg:
                 fields[key] = arg[key]
 
         for key in kwargs:
             fields[key] = kwargs[key]
 
         __discrete__ = _null_coalesce(
@@ -93,15 +96,15 @@
         name: str,
         pool: "SchemaPool",
     ):
         return pool.add_schema(name, self)
 
     @staticmethod
     def new(
-        *args: Union[str, dict],
+        *args: Union[str, dict, None],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
         """
         :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
@@ -116,15 +119,15 @@
             __no_default__=__no_default__,
             __no_null__=__no_null__,
             **kwargs,
         )
 
 
 def schema(
-    *args: Union[str, dict],
+    *args: Union[str, dict, None],
     __discrete__: bool = None,  # type: ignore
     __no_default__: bool = None,  # type: ignore
     __no_null__: bool = None,  # type: ignore
     **kwargs,
 ):
     """
     :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
@@ -134,14 +137,17 @@
     :__no_null__: When `true`, `null` values will never be included.
     """
     # Get all fields.
 
     all_fields: dict[str, Any] = {}
 
     for arg in args:
+        if arg == None:
+            continue
+
         if isinstance(arg, str):
             with open(arg, "r") as f:
                 json_fields = json.loads(f.read())
 
                 for key in json_fields:
                     all_fields[key] = json_fields[key]
```

### Comparing `lazy_schema-0.3.0/lazy_schema/schema_pool.py` & `lazy_schema-0.3.1/lazy_schema/schema_pool.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         raise Exception(f"Schema '{key}' does not exist!")
 
     def pymongo(
         self,
         mongo_collection,
         field_value: str,
         field_name="__name__",
-        *args: Union[str, dict],
+        *args: Union[str, dict, None],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
         return self.pymongo_query(
             mongo_collection,
@@ -49,15 +49,15 @@
             **kwargs,
         )
 
     def pymongo_query(
         self,
         mongo_collection,
         query,
-        *args: Union[str, dict],
+        *args: Union[str, dict, None],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
         document = _load_document(mongo_collection, query)
 
@@ -83,15 +83,15 @@
         setattr(self, name, schema)
 
         return schema
 
     def set(
         self,
         name: str,
-        *args: Union[str, dict],
+        *args: Union[str, dict, None],
         __discrete__=False,
         __no_default__=False,
         __no_null__=False,
         **kwargs,
     ):
         """
         :__discrete__: When `true`, excludes fields with a `null` default value. Explicitly setting the value to `null` will include it.
```

### Comparing `lazy_schema-0.3.0/PKG-INFO` & `lazy_schema-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-schema
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

