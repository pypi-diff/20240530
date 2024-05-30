# Comparing `tmp/aiohttp_pydantic-2.1.0-py3-none-any.whl.zip` & `tmp/aiohttp_pydantic-2.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20933 bytes, number of entries: 18
--rw-r--r--  2.0 unx       97 b- defN 24-Apr-28 14:45 aiohttp_pydantic/__init__.py
--rw-r--r--  2.0 unx    10157 b- defN 24-Apr-28 13:51 aiohttp_pydantic/injectors.py
+Zip file size: 20956 bytes, number of entries: 18
+-rw-r--r--  2.0 unx       97 b- defN 24-May-30 20:44 aiohttp_pydantic/__init__.py
+-rw-r--r--  2.0 unx    10232 b- defN 24-May-30 20:13 aiohttp_pydantic/injectors.py
 -rw-r--r--  2.0 unx      444 b- defN 24-Feb-06 19:08 aiohttp_pydantic/utils.py
 -rw-r--r--  2.0 unx     5037 b- defN 24-Apr-28 13:51 aiohttp_pydantic/view.py
 -rw-r--r--  2.0 unx     1111 b- defN 24-Apr-28 13:51 aiohttp_pydantic/oas/__init__.py
 -rw-r--r--  2.0 unx      178 b- defN 24-Feb-06 19:08 aiohttp_pydantic/oas/__main__.py
 -rw-r--r--  2.0 unx     3414 b- defN 24-Apr-28 13:51 aiohttp_pydantic/oas/cmd.py
 -rw-r--r--  2.0 unx      678 b- defN 24-Apr-28 14:45 aiohttp_pydantic/oas/definition.py
 -rw-r--r--  2.0 unx     4031 b- defN 24-Feb-06 19:08 aiohttp_pydantic/oas/docstring_parser.py
 -rw-r--r--  2.0 unx     1823 b- defN 24-Feb-06 19:08 aiohttp_pydantic/oas/index.j2
 -rw-r--r--  2.0 unx     8440 b- defN 24-Feb-06 19:08 aiohttp_pydantic/oas/struct.py
 -rw-r--r--  2.0 unx     1226 b- defN 24-Feb-06 19:08 aiohttp_pydantic/oas/typing.py
 -rw-r--r--  2.0 unx     7613 b- defN 24-Apr-28 14:45 aiohttp_pydantic/oas/view.py
--rw-r--r--  2.0 unx     1072 b- defN 24-Apr-28 14:47 aiohttp_pydantic-2.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    14386 b- defN 24-Apr-28 14:47 aiohttp_pydantic-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 14:47 aiohttp_pydantic-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-28 14:47 aiohttp_pydantic-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1557 b- defN 24-Apr-28 14:47 aiohttp_pydantic-2.1.0.dist-info/RECORD
-18 files, 61373 bytes uncompressed, 18359 bytes compressed:  70.1%
+-rw-r--r--  2.0 unx     1072 b- defN 24-May-30 20:50 aiohttp_pydantic-2.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14386 b- defN 24-May-30 20:50 aiohttp_pydantic-2.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 20:50 aiohttp_pydantic-2.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-30 20:50 aiohttp_pydantic-2.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1557 b- defN 24-May-30 20:50 aiohttp_pydantic-2.1.1.dist-info/RECORD
+18 files, 61448 bytes uncompressed, 18382 bytes compressed:  70.1%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: aiohttp_pydantic/oas/typing.py
 Comment: 
 
 Filename: aiohttp_pydantic/oas/view.py
 Comment: 
 
-Filename: aiohttp_pydantic-2.1.0.dist-info/LICENSE
+Filename: aiohttp_pydantic-2.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: aiohttp_pydantic-2.1.0.dist-info/METADATA
+Filename: aiohttp_pydantic-2.1.1.dist-info/METADATA
 Comment: 
 
-Filename: aiohttp_pydantic-2.1.0.dist-info/WHEEL
+Filename: aiohttp_pydantic-2.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: aiohttp_pydantic-2.1.0.dist-info/top_level.txt
+Filename: aiohttp_pydantic-2.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aiohttp_pydantic-2.1.0.dist-info/RECORD
+Filename: aiohttp_pydantic-2.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiohttp_pydantic/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .view import PydanticView
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 __all__ = ("PydanticView", "__version__")
```

## aiohttp_pydantic/injectors.py

```diff
@@ -129,17 +129,19 @@
         """
         Return a dict with list as value from the MultiDict.
 
         The value will be wrapped in a list if the args spec is define as a list or if
         the multiple values are sent (i.e ?foo=1&foo=2)
         """
         return {
-            key: values
-            if len(values := query.getall(key)) > 1 or key in self._is_multiple
-            else value
+            key: (
+                values
+                if len(values := query.getall(key)) > 1 or key in self._is_multiple
+                else value
+            )
             for key, value in query.items()
         }
 
 
 class HeadersGetter(AbstractInjector):
     """
     Validates and injects the HTTP headers inside the view kwargs.
@@ -187,29 +189,32 @@
 
     class PetView(PydanticView):
         def get(self, page: Pagination):
             ...
     """
 
 
+_NOT_SET = object()
+
+
 def _get_group_signature(cls) -> Tuple[dict, dict]:
     """
     Analyse Group subclass annotations and return them with default values.
     """
 
     sig = {}
     defaults = {}
     mro = getmro(cls)
     for base in reversed(mro[: mro.index(Group)]):
         attrs = vars(base)
 
         # Use __annotations__ to know if an attribute is
         # overwrite to remove the default value.
         for attr_name, type_ in base.__annotations__.items():
-            if (default := attrs.get(attr_name)) is None:
+            if (default := attrs.get(attr_name, _NOT_SET)) is _NOT_SET:
                 defaults.pop(attr_name, None)
             else:
                 defaults[attr_name] = default
 
         # Use get_type_hints to have postponed annotations.
         for attr_name, type_ in get_type_hints(base).items():
             sig[attr_name] = type_
@@ -222,15 +227,15 @@
 ) -> Tuple[dict, dict, dict, dict, dict]:
     """
     Analyse function signature and returns 5-tuple:
         0 - arguments will be set from the url path
         1 - argument will be set from the request body.
         2 - argument will be set from the query string.
         3 - argument will be set from the HTTP headers.
-        4 - Default value for each parameters
+        4 - Default value for each parameter
     """
 
     path_args = {}
     body_args = {}
     qs_args = {}
     header_args = {}
     defaults = {}
```

## Comparing `aiohttp_pydantic-2.1.0.dist-info/LICENSE` & `aiohttp_pydantic-2.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiohttp_pydantic-2.1.0.dist-info/METADATA` & `aiohttp_pydantic-2.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp_pydantic
-Version: 2.1.0
+Version: 2.1.1
 Summary: Aiohttp View using pydantic to validate request body and query sting regarding method annotations.
 Home-page: https://github.com/Maillol/aiohttp-pydantic
 Author: Vincent Maillol
 Author-email: vincent.maillol@gmail.com
 License: MIT
 Keywords: aiohttp,pydantic,annotations,validation
 Classifier: Intended Audience :: Developers
```

## Comparing `aiohttp_pydantic-2.1.0.dist-info/RECORD` & `aiohttp_pydantic-2.1.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-aiohttp_pydantic/__init__.py,sha256=6QlEWubu72z9F8q4OX6oGXxbjkceBau4o_bTSx6aUHU,97
-aiohttp_pydantic/injectors.py,sha256=uycWGPruDErQNopSkV_IifNeVHC6XBZ5sBMBes7D99o,10157
+aiohttp_pydantic/__init__.py,sha256=JHtrVvfgDjYsCx1BZpT4a3hvWMLVmORXwyRpW2fwjlc,97
+aiohttp_pydantic/injectors.py,sha256=RTCmY0BZOS6T8d3v5squmpDG-0cG977kMhfNaLBY4BM,10232
 aiohttp_pydantic/utils.py,sha256=BepxYvj4raIV5Vz4MMhCC1ewwuvQdtRZFbyolbhC0ig,444
 aiohttp_pydantic/view.py,sha256=dwEtXrtG4rgbqa6vqISN6AxZDAZyn0ZtM9jxdq6l8fM,5037
 aiohttp_pydantic/oas/__init__.py,sha256=VTA-_57MvoU4Fv7mJLiyuaq5KK4wpSr08hMQ8KQK7eE,1111
 aiohttp_pydantic/oas/__main__.py,sha256=xENdUU4gUJUDlkwu-gkQ-uTb8E0V2VudanaJR7JV814,178
 aiohttp_pydantic/oas/cmd.py,sha256=3W0RST8bQHzpfGXdt4byhgqB5RF6WtlH6lR0Zh6alos,3414
 aiohttp_pydantic/oas/definition.py,sha256=bj94Bol95Bf2pw0oCazize1gr9ZponevpeBH0kEYTsU,678
 aiohttp_pydantic/oas/docstring_parser.py,sha256=U5DPOk3T1_6iEPWOLYib2Y4jT_loQPZNMJL3a7atwsc,4031
 aiohttp_pydantic/oas/index.j2,sha256=qL1bXKnWjUGo_iMCnZTZrUCQwDyJJUa445-1nzLDjvo,1823
 aiohttp_pydantic/oas/struct.py,sha256=_8iyUJfWAv2AyTFJoKQblt1c7OSmSSFzyNUGQQ2a33s,8440
 aiohttp_pydantic/oas/typing.py,sha256=4WZPNk-nycfKm2jSu8ex0FQCSY6Lyt7h1QW5M0tOy1o,1226
 aiohttp_pydantic/oas/view.py,sha256=2UOZbP8x-c7_V3q27airvye3tqFZ8AFLxj4Xswh9rrU,7613
-aiohttp_pydantic-2.1.0.dist-info/LICENSE,sha256=n7KxVZHGC5OISzqDX7cQ4RbWdXxg1FkFEnMKpnosff8,1072
-aiohttp_pydantic-2.1.0.dist-info/METADATA,sha256=EaBQWpjuRx1LfKBH67SCyH0h99_J0oWXOQ0nVxqpBMg,14386
-aiohttp_pydantic-2.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-aiohttp_pydantic-2.1.0.dist-info/top_level.txt,sha256=EuM8hK21eeaLnsdWoGwj2zz8xWsdxbGNHRpFq4ysjSw,17
-aiohttp_pydantic-2.1.0.dist-info/RECORD,,
+aiohttp_pydantic-2.1.1.dist-info/LICENSE,sha256=n7KxVZHGC5OISzqDX7cQ4RbWdXxg1FkFEnMKpnosff8,1072
+aiohttp_pydantic-2.1.1.dist-info/METADATA,sha256=AVbZWlr2oHfwiFHLtdXb8696lC9PcPxITFIj5CXOdKA,14386
+aiohttp_pydantic-2.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aiohttp_pydantic-2.1.1.dist-info/top_level.txt,sha256=EuM8hK21eeaLnsdWoGwj2zz8xWsdxbGNHRpFq4ysjSw,17
+aiohttp_pydantic-2.1.1.dist-info/RECORD,,
```

