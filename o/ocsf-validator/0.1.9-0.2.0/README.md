# Comparing `tmp/ocsf_validator-0.1.9.tar.gz` & `tmp/ocsf_validator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocsf_validator-0.1.9.tar", max compression
+gzip compressed data, was "ocsf_validator-0.2.0.tar", max compression
```

## Comparing `ocsf_validator-0.1.9.tar` & `ocsf_validator-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10173 2024-01-08 22:46:31.782602 ocsf_validator-0.1.9/LICENSE
--rw-r--r--   0        0        0     4209 2024-03-22 16:43:23.019386 ocsf_validator-0.1.9/README.md
--rw-r--r--   0        0        0      241 2024-01-08 22:46:31.762238 ocsf_validator-0.1.9/ocsf_validator/__init__.py
--rw-r--r--   0        0        0      584 2024-03-22 16:43:23.019731 ocsf_validator-0.1.9/ocsf_validator/__main__.py
--rw-r--r--   0        0        0     6728 2024-05-01 13:34:34.222601 ocsf_validator-0.1.9/ocsf_validator/errors.py
--rw-r--r--   0        0        0     3184 2024-05-01 13:34:34.223463 ocsf_validator-0.1.9/ocsf_validator/matchers.py
--rw-r--r--   0        0        0    16941 2024-05-01 13:34:34.224122 ocsf_validator-0.1.9/ocsf_validator/processor.py
--rw-r--r--   0        0        0     6956 2024-03-22 16:43:23.020718 ocsf_validator-0.1.9/ocsf_validator/reader.py
--rw-r--r--   0        0        0        0 2024-01-08 22:46:31.766272 ocsf_validator-0.1.9/ocsf_validator/repository.py
--rw-r--r--   0        0        0    12859 2024-05-01 13:34:34.224698 ocsf_validator-0.1.9/ocsf_validator/runner.py
--rw-r--r--   0        0        0     1647 2024-05-01 13:34:34.224869 ocsf_validator-0.1.9/ocsf_validator/type_mapping.py
--rw-r--r--   0        0        0     5128 2024-05-01 13:34:34.225448 ocsf_validator-0.1.9/ocsf_validator/types.py
--rw-r--r--   0        0        0    22446 2024-05-01 13:34:34.226368 ocsf_validator-0.1.9/ocsf_validator/validators.py
--rw-r--r--   0        0        0      594 2024-05-01 13:34:34.226570 ocsf_validator-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 ocsf_validator-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-01-08 22:46:31.782602 ocsf_validator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4209 2024-03-22 16:43:23.019386 ocsf_validator-0.2.0/README.md
+-rw-r--r--   0        0        0      241 2024-01-08 22:46:31.762238 ocsf_validator-0.2.0/ocsf_validator/__init__.py
+-rw-r--r--   0        0        0      584 2024-03-22 16:43:23.019731 ocsf_validator-0.2.0/ocsf_validator/__main__.py
+-rw-r--r--   0        0        0     6658 2024-05-23 20:42:43.406030 ocsf_validator-0.2.0/ocsf_validator/errors.py
+-rw-r--r--   0        0        0     3209 2024-05-09 14:04:48.384165 ocsf_validator-0.2.0/ocsf_validator/matchers.py
+-rw-r--r--   0        0        0    16947 2024-05-09 14:04:48.384597 ocsf_validator-0.2.0/ocsf_validator/processor.py
+-rw-r--r--   0        0        0     6956 2024-03-22 16:43:23.020718 ocsf_validator-0.2.0/ocsf_validator/reader.py
+-rw-r--r--   0        0        0        0 2024-01-08 22:46:31.766272 ocsf_validator-0.2.0/ocsf_validator/repository.py
+-rw-r--r--   0        0        0    12859 2024-05-01 13:34:34.224698 ocsf_validator-0.2.0/ocsf_validator/runner.py
+-rw-r--r--   0        0        0     1647 2024-05-01 13:34:34.224869 ocsf_validator-0.2.0/ocsf_validator/type_mapping.py
+-rw-r--r--   0        0        0     5183 2024-05-30 19:19:07.549921 ocsf_validator-0.2.0/ocsf_validator/types.py
+-rw-r--r--   0        0        0    22477 2024-05-09 14:04:48.385208 ocsf_validator-0.2.0/ocsf_validator/validators.py
+-rw-r--r--   0        0        0      625 2024-05-30 19:26:52.050214 ocsf_validator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 ocsf_validator-0.2.0/PKG-INFO
```

### Comparing `ocsf_validator-0.1.9/LICENSE` & `ocsf_validator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.9/README.md` & `ocsf_validator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.9/ocsf_validator/__main__.py` & `ocsf_validator-0.2.0/ocsf_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.9/ocsf_validator/errors.py` & `ocsf_validator-0.2.0/ocsf_validator/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Iterable, Optional, TypeVar
+from __future__ import annotations
 
-TCollector = TypeVar("TCollector", bound="Collector")
+from typing import Iterable, Optional
 
 
 class Collector:
     """An error collector used by schema operations so that encountered errors
     can be saved for later and displayed as test output.
 
     The default behavior is to `raise` all exceptions, so you shouldn't
     notice the collector until `throw` is `False`.
     """
 
-    default: TCollector  # type: ignore
+    default: Collector
     """Simple singleton used whenever an Optional[Collector] parameter is None."""
 
     def __init__(self, throw: bool = True):
         self._exceptions: list[Exception] = []
         self._throw = throw
 
     def handle(self, err: Exception):
@@ -48,24 +48,21 @@
 
 class ValidationError(Exception):
     """Base class for validation errors."""
 
     ...
 
 
-class InvalidBasePathError(ValidationError):
-    ...
+class InvalidBasePathError(ValidationError): ...
 
 
-class InvalidMetaSchemaError(ValidationError):
-    ...
+class InvalidMetaSchemaError(ValidationError): ...
 
 
-class InvalidMetaSchemaFileError(ValidationError):
-    ...
+class InvalidMetaSchemaFileError(ValidationError): ...
 
 
 class UnusedAttributeError(ValidationError):
     def __init__(self, attr: str):
         self.attr = attr
         super().__init__(f"Unused attribute {attr}")
 
@@ -84,21 +81,16 @@
         self.trail = trail
 
         if trail is None:
             trail_str = ""
         else:
             trail_str = ".".join(trail)
 
-        if cls is None:
-            cls_str = ""
-        else:
-            cls_str = cls.__name__ + "."
-
         super().__init__(
-            f"Missing required key `{cls_str}{key}` at `{trail_str}` in {file}"
+            f"Missing required key `{key}` at `{trail_str}` in {file}.  Make sure required fields in this file and any supporting files such as dictionaries or includes are populated."
         )
 
 
 class UnknownKeyError(ValidationError):
     def __init__(
         self,
         key: str,
@@ -112,21 +104,16 @@
         self.trail = trail
 
         if trail is None:
             trail_str = ""
         else:
             trail_str = ".".join(trail)
 
-        if cls is None:
-            cls_str = ""
-        else:
-            cls_str = cls.__name__
-
         super().__init__(
-            f"Unrecognized key `{key}` of `{cls_str}` at `{trail_str}` in {file}"
+            f"Unrecognized key `{key}` at `{trail_str}` in {file}.  Make sure fields in this file and any supporting files such as dictionaries or includes are valid."
         )
 
 
 class DependencyError(ValidationError):
     def __init__(self, file: str, include: str, message: Optional[str] = None):
         self.file = file
         self.include = include
```

### Comparing `ocsf_validator-0.1.9/ocsf_validator/matchers.py` & `ocsf_validator-0.2.0/ocsf_validator/matchers.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
             self._matchers = []
 
     def match(self, value: str):
         for matcher in self._matchers:
             if matcher.match(value):
                 return True
 
+        return False
+
     def add(self, matcher: Matcher):
         self._matchers.append(matcher)
 
 
 class RegexMatcher(Matcher):
     def __init__(self, pattern: str | re.Pattern):
         if isinstance(pattern, str):
@@ -119,16 +121,18 @@
 class CategoriesMatcher(RegexMatcher, TypeMatcher):
     def __init__(self):
         self._pattern = re.compile(r".*categories.json")
 
     def get_type(self):
         return OcsfCategories
 
+
 class ExcludeMatcher(Matcher):
     """
     A matcher that produces the opposite result of the matcher it's given.
     """
+
     def __init__(self, matcher: Matcher):
         self.matcher = matcher
 
     def match(self, value: str) -> bool:
-        return not self.matcher.match(value)
+        return not self.matcher.match(value)
```

### Comparing `ocsf_validator-0.1.9/ocsf_validator/processor.py` & `ocsf_validator-0.2.0/ocsf_validator/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from pathlib import Path
 from typing import Any, Callable, Optional
 
 from ocsf_validator.errors import *
-from ocsf_validator.matchers import (
-    CategoriesMatcher,
-    ExcludeMatcher
-)
+from ocsf_validator.matchers import CategoriesMatcher, ExcludeMatcher
 from ocsf_validator.reader import Reader
 from ocsf_validator.type_mapping import TypeMapping
 from ocsf_validator.types import (
     ATTRIBUTES_KEY,
     EXTENDS_KEY,
     INCLUDE_KEY,
     PROFILES_KEY,
@@ -255,15 +252,15 @@
         return []
 
 
 class ProfilesParser(MergeParser):
     def applies_to(self, t: type) -> bool:
         if hasattr(t, "__required_keys__") or hasattr(t, "__optional_keys"):
             return (
-                PROFILES_KEY in t.__required_keys__
+                PROFILES_KEY in t.__required_keys__  # type: ignore
                 or PROFILES_KEY in t.__optional_keys__  # type: ignore
             )
         else:
             return False
 
     def found_in(self, path: str) -> bool:
         return PROFILES_KEY in self._reader[path]
@@ -285,15 +282,15 @@
         return targets
 
 
 class AttributesParser(MergeParser):
     def applies_to(self, t: type) -> bool:
         if hasattr(t, "__required_keys__") or hasattr(t, "__optional_keys"):
             return (
-                ATTRIBUTES_KEY in t.__required_keys__
+                ATTRIBUTES_KEY in t.__required_keys__  # type: ignore
                 or ATTRIBUTES_KEY in t.__optional_keys__  # type: ignore
             )
         else:
             return False
 
     def found_in(self, path: str) -> bool:
         return ATTRIBUTES_KEY in self._reader[path]
@@ -464,17 +461,15 @@
         ATTRIBUTES_KEY: AttributesParser(reader, resolver, collector, types),
     }
     fulfilled: set[str] = set()
     dependencies = Dependencies()
 
     # categories cannot be extended with dependencies, and it causes problems
     # if we try to include dictionary attributes in categories
-    matcher = ExcludeMatcher(
-        CategoriesMatcher()
-    )
+    matcher = ExcludeMatcher(CategoriesMatcher())
 
     for path in reader.match(matcher):
         for directive, parser in parsers.items():
             if parser.found_in(path):
                 for target in parser.extract_targets(path):
                     dependencies.add(path, target, directive)
```

### Comparing `ocsf_validator-0.1.9/ocsf_validator/reader.py` & `ocsf_validator-0.2.0/ocsf_validator/reader.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.9/ocsf_validator/runner.py` & `ocsf_validator-0.2.0/ocsf_validator/runner.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.9/ocsf_validator/type_mapping.py` & `ocsf_validator-0.2.0/ocsf_validator/type_mapping.py`

 * *Files identical despite different names*

### Comparing `ocsf_validator-0.1.9/ocsf_validator/types.py` & `ocsf_validator-0.2.0/ocsf_validator/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         # "caption": NotRequired[str],
         "caption": str,
         "default": NotRequired[Any],
         "description": NotRequired[str],
         "enum": NotRequired[Dict[str, OcsfEnumMember]],
         "group": NotRequired[str],
         "is_array": NotRequired[bool],
+        "suppress_checks": NotRequired[Sequence[str]],
         "max_len": NotRequired[int],
         "name": NotRequired[str],
         "notes": NotRequired[str],
         "observable": NotRequired[int],
         "range": NotRequired[Sequence[int]],
         "regex": NotRequired[str],
         "requirement": NotRequired[str],
```

### Comparing `ocsf_validator-0.1.9/ocsf_validator/validators.py` & `ocsf_validator-0.2.0/ocsf_validator/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,15 @@
     TYPES_KEY,
     OcsfEvent,
     OcsfObject,
     is_ocsf_type,
     leaf_type,
 )
 
-
-METASCHEMA_MATCHERS =  {
+METASCHEMA_MATCHERS = {
     "event.schema.json": EventMatcher(),
     "include.schema.json": IncludeMatcher(),
     "object.schema.json": ObjectMatcher(),
     "profile.schema.json": ProfileMatcher(),
     "categories.schema.json": CategoriesMatcher(),
     "dictionary.schema.json": DictionaryMatcher(),
     "extension.schema.json": ExtensionMatcher(),
@@ -265,18 +264,19 @@
             found[t][name].append(file)
 
     reader.apply(validate, AnyMatcher([ObjectMatcher(), EventMatcher()]))
 
 
 def _default_get_registry(reader: Reader, base_uri: str) -> referencing.Registry:
     registry: referencing.Registry = referencing.Registry()
-    for schema_file_path in reader.metaschema_path.glob("*.schema.json"):
+
+    for schema_file_path in reader.metaschema_path.glob("*.schema.json"):  # type: ignore
         with open(schema_file_path, "r") as file:
             schema = json.load(file)
-            resource = referencing.Resource.from_contents(schema)
+            resource = referencing.Resource.from_contents(schema)  # type: ignore
             registry = registry.with_resource(
                 base_uri + schema_file_path.name, resource=resource
             )
     return registry
 
 
 def validate_metaschemas(
```

### Comparing `ocsf_validator-0.1.9/pyproject.toml` & `ocsf_validator-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocsf-validator"
-version = "0.1.9"
+version = "0.2.0"
 description = "OCSF Schema Validation"
 authors = [
     "Jeremy Fisher <jeremy@query.ai>",
     "Alan Pinkert <apinkert@cisco.com>",
     "Rick Mouritzen <rmouritzen@splunk.com>",
 ]
 readme = "README.md"
@@ -20,7 +20,10 @@
 black = ">=23.9.1,<25.0.0"
 pytest = "^7.4.2"
 pyright = "^1.1.327"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
```

### Comparing `ocsf_validator-0.1.9/PKG-INFO` & `ocsf_validator-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocsf-validator
-Version: 0.1.9
+Version: 0.2.0
 Summary: OCSF Schema Validation
 Author: Jeremy Fisher
 Author-email: jeremy@query.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
```

