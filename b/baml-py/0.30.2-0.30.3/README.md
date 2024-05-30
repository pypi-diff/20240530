# Comparing `tmp/baml_py-0.30.2-cp38-abi3-win_amd64.whl.zip` & `tmp/baml_py-0.30.3-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 4450387 bytes, number of entries: 13
--rw-r--r--  4.6 unx      354 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/WHEEL
--rw-r--r--  4.6 unx       54 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11556 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11556 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx     3422 b- defN 24-May-30 16:08 baml_py/async_context_vars.py
--rw-r--r--  4.6 unx     4070 b- defN 24-May-30 16:08 baml_py/baml_py.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-May-30 16:08 baml_py/py.typed
--rw-r--r--  4.6 unx     2474 b- defN 24-May-30 16:08 baml_py/stream.py
--rw-r--r--  4.6 unx     4330 b- defN 24-May-30 16:08 baml_py/type_builder.py
--rw-r--r--  4.6 unx      506 b- defN 24-May-30 16:08 baml_py/__init__.py
--rwxr-xr-x  4.6 unx 11762688 b- defN 24-May-30 16:08 baml_py/baml_py.pyd
--rw-r--r--  4.6 unx     1053 b- defN 24-May-30 16:08 baml_py-0.30.2.dist-info/RECORD
-13 files, 11802157 bytes uncompressed, 4448639 bytes compressed:  62.3%
+Zip file size: 4442501 bytes, number of entries: 13
+-rw-r--r--  4.6 unx      354 b- defN 24-May-30 19:06 baml_py-0.30.3.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-30 19:06 baml_py-0.30.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx       54 b- defN 24-May-30 19:06 baml_py-0.30.3.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-30 19:06 baml_py-0.30.3.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-30 19:06 baml_py-0.30.3.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     3406 b- defN 24-May-30 19:06 baml_py/async_context_vars.py
+-rw-r--r--  4.6 unx     4210 b- defN 24-May-30 19:06 baml_py/baml_py.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-30 19:06 baml_py/py.typed
+-rw-r--r--  4.6 unx     2474 b- defN 24-May-30 19:06 baml_py/stream.py
+-rw-r--r--  4.6 unx     4330 b- defN 24-May-30 19:06 baml_py/type_builder.py
+-rw-r--r--  4.6 unx      506 b- defN 24-May-30 19:06 baml_py/__init__.py
+-rwxr-xr-x  4.6 unx 11735040 b- defN 24-May-30 19:06 baml_py/baml_py.pyd
+-rw-r--r--  4.6 unx     1053 b- defN 24-May-30 19:06 baml_py-0.30.3.dist-info/RECORD
+13 files, 11774633 bytes uncompressed, 4440753 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: baml_py-0.30.2.dist-info/METADATA
+Filename: baml_py-0.30.3.dist-info/METADATA
 Comment: 
 
-Filename: baml_py-0.30.2.dist-info/WHEEL
+Filename: baml_py-0.30.3.dist-info/WHEEL
 Comment: 
 
-Filename: baml_py-0.30.2.dist-info/entry_points.txt
+Filename: baml_py-0.30.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: baml_py-0.30.2.dist-info/license_files/LICENSE
+Filename: baml_py-0.30.3.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: baml_py-0.30.2.dist-info/license_files/LICENSE
+Filename: baml_py-0.30.3.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: baml_py/async_context_vars.py
 Comment: 
 
 Filename: baml_py/baml_py.pyi
 Comment: 
@@ -30,11 +30,11 @@
 
 Filename: baml_py/__init__.py
 Comment: 
 
 Filename: baml_py/baml_py.pyd
 Comment: 
 
-Filename: baml_py-0.30.2.dist-info/RECORD
+Filename: baml_py-0.30.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## baml_py/async_context_vars.py

```diff
@@ -16,15 +16,15 @@
     def __init__(self, rt: BamlRuntime):
         self.rt = rt
         self.ctx = contextvars.ContextVar[RuntimeContextManager](
             "baml_ctx", default=rt.create_context_manager()
         )
         atexit.register(self.rt.flush)
 
-    def upsert_tags(self, tags: typing.Dict[str, str]) -> None:
+    def upsert_tags(self, **tags: str) -> None:
         mngr = self.ctx.get()
         mngr.upsert_tags(tags)
 
     def get(self) -> RuntimeContextManager:
         return self.ctx.get()
 
     def start_trace_sync(
```

## baml_py/baml_py.pyi

```diff
@@ -54,14 +54,18 @@
     async def call_function(
         self,
         function_name: str,
         args: Dict[str, Any],
         ctx: RuntimeContextManager,
         tb: Optional[TypeBuilder],
     ) -> FunctionResult: ...
+    @staticmethod
+    def from_files(
+        root_path: str, files: Dict[str, str], env_vars: Dict[str, str]
+    ) -> BamlRuntime: ...
     def stream_function(
         self,
         function_name: str,
         args: Dict[str, Any],
         on_event: Optional[Callable[[FunctionResult], None]],
         ctx: RuntimeContextManager,
         tb: Optional[TypeBuilder],
```

## Comparing `baml_py-0.30.2.dist-info/license_files/LICENSE` & `baml_py-0.30.3.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `baml_py-0.30.2.dist-info/RECORD` & `baml_py-0.30.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-baml_py-0.30.2.dist-info/METADATA,sha256=OT4XjteRU8DL6x5-WBSI3wVmCB38IRXYvvSzJsgBsK0,354
-baml_py-0.30.2.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
-baml_py-0.30.2.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
-baml_py-0.30.2.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py-0.30.2.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py/async_context_vars.py,sha256=gU_H0abCPxxULNRUArMlsx2aeLNp7E7fIVBY6nLY_F0,3422
-baml_py/baml_py.pyi,sha256=wGHs0y6RjeTl3-aqY9tCAdvo-fCqeb6i4k0fvK-m93Q,4070
+baml_py-0.30.3.dist-info/METADATA,sha256=Oa3XWW3Gu0VoJShdEHzkejjK18bD_JAu-9PAnGZLXbI,354
+baml_py-0.30.3.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
+baml_py-0.30.3.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
+baml_py-0.30.3.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py-0.30.3.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py/async_context_vars.py,sha256=QfnNjQIT9MtpqbfuD4v0hWlZIdn2JmNu8U-iKpHjTrc,3406
+baml_py/baml_py.pyi,sha256=qzfYhh5rOQ2dZWSYNqMdUPBirqq4lII3vM2_VUk32m8,4210
 baml_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 baml_py/stream.py,sha256=B4mpGnqAmU7DFHJPiAAAiNIeX5wgLJhXLZp9Pqb9-AY,2474
 baml_py/type_builder.py,sha256=v3yiY2VtGuCEECr0jh7OB3ueWSiSwj-8IETXQuSIYl0,4330
 baml_py/__init__.py,sha256=-y49naDuvHdmpkmUEqZBESlBNx6W4qsPOPu9KlrMT10,506
-baml_py/baml_py.pyd,sha256=XLtuC_XkQw2dM5bQY9UCV2dsOkLUZUi8KV5KnFO9vwM,11762688
-baml_py-0.30.2.dist-info/RECORD,,
+baml_py/baml_py.pyd,sha256=DZDyeRseUEM7g2BrVT6B__tHerJ_anr6bz6D_3HbBHc,11735040
+baml_py-0.30.3.dist-info/RECORD,,
```

