# Comparing `tmp/imy-0.3.5.tar.gz` & `tmp/imy-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.3.5.tar", max compression
+gzip compressed data, was "imy-0.3.6.tar", max compression
```

## Comparing `imy-0.3.5.tar` & `imy-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.5/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.5/README.md
--rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.5/imy/__init__.py
--rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.5/imy/assets.py
--rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.5/imy/async_utils.py
--rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.5/imy/config.py
--rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.5/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     7144 2024-05-25 14:29:09.469900 imy-0.3.5/imy/docstrings/data_models.py
--rw-r--r--   0        0        0    17737 2024-05-25 14:29:09.469900 imy-0.3.5/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.5/imy/inject.py
--rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.5/imy/logs.py
--rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.5/imy/package_metadata.py
--rw-r--r--   0        0        0      753 2024-05-25 14:29:28.280049 imy-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.3.6/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 13:27:52.000000 imy-0.3.6/imy/__init__.py
+-rw-r--r--   0        0        0     6727 2024-04-26 06:20:02.579623 imy-0.3.6/imy/assets.py
+-rw-r--r--   0        0        0     6395 2024-04-29 15:43:18.799268 imy-0.3.6/imy/async_utils.py
+-rw-r--r--   0        0        0     9840 2024-04-22 13:49:54.000000 imy-0.3.6/imy/config.py
+-rw-r--r--   0        0        0     1112 2024-04-29 16:01:49.458562 imy-0.3.6/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     6853 2024-05-30 03:57:34.696703 imy-0.3.6/imy/docstrings/data_models.py
+-rw-r--r--   0        0        0    17737 2024-05-25 14:29:09.469900 imy-0.3.6/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8578 2024-04-25 19:05:06.904544 imy-0.3.6/imy/inject.py
+-rw-r--r--   0        0        0    14594 2024-04-29 15:43:49.552681 imy-0.3.6/imy/logs.py
+-rw-r--r--   0        0        0     3185 2024-04-22 13:27:52.000000 imy-0.3.6/imy/package_metadata.py
+-rw-r--r--   0        0        0      753 2024-05-30 03:57:34.696703 imy-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 imy-0.3.6/PKG-INFO
```

### Comparing `imy-0.3.5/LICENSE` & `imy-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/assets.py` & `imy-0.3.6/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/async_utils.py` & `imy-0.3.6/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/config.py` & `imy-0.3.6/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/docstrings/__init__.py` & `imy-0.3.6/imy/docstrings/__init__.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/docstrings/data_models.py` & `imy-0.3.6/imy/docstrings/data_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import *  # type: ignore
 
 import introspection.types
 import introspection.typing
 
 from . import parsers
 
@@ -33,57 +33,45 @@
     """
     Some metadata such as whether an object is public or not is shared between
     different types of objects. This class is used to hold that metadata.
     """
 
     # Whether the object is meant to be used by users of the library, or if it's
     # an internal implementation detail.
-    public: bool
+    public: bool = True
 
     # If `True`, this object is not yet ready for public use. Its API may change
     # between even patch releases.
-    experimental: bool
+    experimental: bool = False
+
+    # Contains all `key: value` pairs that don't correspond to known fields
+    extras: dict[str, str] = field(default_factory=dict)
 
     @staticmethod
-    def _parse_bool(
-        metadata: dict[str, str],
-        key_name: str,
-        default_value: bool | None,
-    ) -> bool:
+    def _parse_bool(value: str) -> bool:
         """
         Attempts to parse a boolean value from metadata.
 
         ## Raises
 
-        `ValueError`: If the key is missing or invalid.
+        `ValueError`: If the key is invalid.
         """
-
-        # Try to get the value
-        try:
-            raw = metadata[key_name]
-        except KeyError:
-            # No value provided
-            if default_value is None:
-                raise ValueError(f"Missing value for `{key_name}` in metadata")
-
-            return default_value
-
         # Postprocess the value
-        if isinstance(raw, str):
-            raw = raw.strip()
+        if isinstance(value, str):
+            value = value.strip()
 
         # Recognized strings
-        if raw == "True":
+        if value == "True":
             return True
 
-        if raw == "False":
+        if value == "False":
             return False
 
         # Invalid value
-        raise ValueError(f'Invalid value for `{key_name}` in metadata: "{raw}"')
+        raise ValueError(f"Cannot parse {value!r} as a boolean")
 
     @staticmethod
     def _parse_literal(
         metadata: dict[str, str],
         key_name: str,
         options: Set[str],
         default_value: str | None,
@@ -112,52 +100,58 @@
 
         # Check if the value is valid
         if raw not in options:
             raise ValueError(f'Invalid value for `{key_name}` in metadata: "{raw}"')
 
         return raw
 
-    @staticmethod
-    def from_dictionary(metadata: dict[str, Any]) -> CommonMetadata:
+    @classmethod
+    def from_dictionary(cls, metadata: dict[str, Any]) -> Self:
         """
         Parses a `CommonMetadata` object from a dictionary. This is useful for
         parsing metadata from a docstring key section.
         """
 
-        # Parse all values
-        public = CommonMetadata._parse_bool(metadata, "public", default_value=True)
-        experimental = CommonMetadata._parse_bool(
-            metadata, "experimental", default_value=False
-        )
+        kwargs = {}
+        extras = {}
+
+        type_hints = get_type_hints(cls)
+
+        for key, value in metadata.items():
+            try:
+                annotation = type_hints[key]
+            except KeyError:
+                # Unknown field
+                extras[key] = value
+                continue
+
+            try:
+                if annotation is bool:
+                    parsed_value = cls._parse_bool(value)
+                else:
+                    raise NotImplementedError(
+                        f"Can't parse values of type {annotation} yet"
+                    )
+            except ValueError:
+                raise ValueError(f"Invalid value for {key!r}: {value!r}")
+
+            kwargs[key] = parsed_value
 
         # Construct the result
-        return CommonMetadata(
-            public=public,
-            experimental=experimental,
-        )
+        return cls(**kwargs, extras=extras)
 
 
 @dataclass
 class FunctionMetadata(CommonMetadata):
-    @staticmethod
-    def from_dictionary(metadata: dict[str, Any]) -> FunctionMetadata:
-        result = CommonMetadata.from_dictionary(metadata)
-        result.__class__ = FunctionMetadata
-        assert isinstance(result, FunctionMetadata)
-        return result
+    decorator: bool = False
 
 
 @dataclass
 class ClassMetadata(CommonMetadata):
-    @staticmethod
-    def from_dictionary(metadata: dict[str, Any]) -> ClassMetadata:
-        result = CommonMetadata.from_dictionary(metadata)
-        result.__class__ = ClassMetadata
-        assert isinstance(result, ClassMetadata)
-        return result
+    pass
 
 
 @dataclass
 class Docstring:
     """
     A generic docstring object.
```

### Comparing `imy-0.3.5/imy/docstrings/parsers.py` & `imy-0.3.6/imy/docstrings/parsers.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/inject.py` & `imy-0.3.6/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/logs.py` & `imy-0.3.6/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/imy/package_metadata.py` & `imy-0.3.6/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.3.5/pyproject.toml` & `imy-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.3.5"
+version = "0.3.6"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.3.5/PKG-INFO` & `imy-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.3.5
+Version: 0.3.6
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

