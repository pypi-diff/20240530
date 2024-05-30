# Comparing `tmp/baml_py-0.1.9-cp38-abi3-win_amd64.whl.zip` & `tmp/baml_py-0.30.0-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 4286269 bytes, number of entries: 12
--rw-r--r--  4.6 unx      336 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/WHEEL
--rw-r--r--  4.6 unx       54 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11556 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11556 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx     3272 b- defN 24-May-26 23:13 baml_py/async_context_vars.py
--rw-r--r--  4.6 unx     2641 b- defN 24-May-26 23:13 baml_py/baml_py.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-May-26 23:13 baml_py/py.typed
--rw-r--r--  4.6 unx     2275 b- defN 24-May-26 23:13 baml_py/stream.py
--rw-r--r--  4.6 unx      518 b- defN 24-May-26 23:13 baml_py/__init__.py
--rwxr-xr-x  4.6 unx 11260928 b- defN 24-May-26 23:13 baml_py/baml_py.pyd
--rw-r--r--  4.6 unx      967 b- defN 24-May-26 23:13 baml_py-0.1.9.dist-info/RECORD
-12 files, 11294197 bytes uncompressed, 4284655 bytes compressed:  62.1%
+Zip file size: 4450385 bytes, number of entries: 13
+-rw-r--r--  4.6 unx      337 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx       54 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     3422 b- defN 24-May-30 08:33 baml_py/async_context_vars.py
+-rw-r--r--  4.6 unx     4095 b- defN 24-May-30 08:33 baml_py/baml_py.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-30 08:33 baml_py/py.typed
+-rw-r--r--  4.6 unx     2474 b- defN 24-May-30 08:33 baml_py/stream.py
+-rw-r--r--  4.6 unx     4330 b- defN 24-May-30 08:33 baml_py/type_builder.py
+-rw-r--r--  4.6 unx      506 b- defN 24-May-30 08:33 baml_py/__init__.py
+-rwxr-xr-x  4.6 unx 11762688 b- defN 24-May-30 08:33 baml_py/baml_py.pyd
+-rw-r--r--  4.6 unx     1053 b- defN 24-May-30 08:33 baml_py-0.30.0.dist-info/RECORD
+13 files, 11802165 bytes uncompressed, 4448637 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,37 +1,40 @@
-Filename: baml_py-0.1.9.dist-info/METADATA
+Filename: baml_py-0.30.0.dist-info/METADATA
 Comment: 
 
-Filename: baml_py-0.1.9.dist-info/WHEEL
+Filename: baml_py-0.30.0.dist-info/WHEEL
 Comment: 
 
-Filename: baml_py-0.1.9.dist-info/entry_points.txt
+Filename: baml_py-0.30.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: baml_py-0.1.9.dist-info/license_files/LICENSE
+Filename: baml_py-0.30.0.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: baml_py-0.1.9.dist-info/license_files/LICENSE
+Filename: baml_py-0.30.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: baml_py/async_context_vars.py
 Comment: 
 
 Filename: baml_py/baml_py.pyi
 Comment: 
 
 Filename: baml_py/py.typed
 Comment: 
 
 Filename: baml_py/stream.py
 Comment: 
 
+Filename: baml_py/type_builder.py
+Comment: 
+
 Filename: baml_py/__init__.py
 Comment: 
 
 Filename: baml_py/baml_py.pyd
 Comment: 
 
-Filename: baml_py-0.1.9.dist-info/RECORD
+Filename: baml_py-0.30.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## baml_py/async_context_vars.py

```diff
@@ -2,52 +2,58 @@
 # This helps ensure we correctly instantiate the span and context for each thread.
 
 import asyncio
 import contextvars
 import functools
 import inspect
 import typing
-from .baml_py import RuntimeContextManagerPy, BamlRuntimePy, BamlSpanPy
+from .baml_py import RuntimeContextManager, BamlRuntime, BamlSpan
 import atexit
 
 F = typing.TypeVar("F", bound=typing.Callable[..., typing.Any])
 
 
 class CtxManager:
-    def __init__(self, rt: BamlRuntimePy):
+    def __init__(self, rt: BamlRuntime):
         self.rt = rt
-        self.ctx = contextvars.ContextVar[RuntimeContextManagerPy](
+        self.ctx = contextvars.ContextVar[RuntimeContextManager](
             "baml_ctx", default=rt.create_context_manager()
         )
         atexit.register(self.rt.flush)
 
     def upsert_tags(self, tags: typing.Dict[str, str]) -> None:
         mngr = self.ctx.get()
         mngr.upsert_tags(tags)
 
-    def get(self) -> RuntimeContextManagerPy:
+    def get(self) -> RuntimeContextManager:
         return self.ctx.get()
 
     def start_trace_sync(
         self, name: str, args: typing.Dict[str, typing.Any]
-    ) -> BamlSpanPy:
+    ) -> BamlSpan:
         mng = self.ctx.get()
-        return BamlSpanPy.new(self.rt, name, args, mng)
+        return BamlSpan.new(self.rt, name, args, mng)
 
     def start_trace_async(
         self, name: str, args: typing.Dict[str, typing.Any]
-    ) -> BamlSpanPy:
+    ) -> BamlSpan:
         mng = self.ctx.get()
         cln = mng.deep_clone()
         self.ctx.set(cln)
-        return BamlSpanPy.new(self.rt, name, args, cln)
+        return BamlSpan.new(self.rt, name, args, cln)
 
-    async def end_trace(self, span: BamlSpanPy, response: typing.Any) -> None:
+    async def end_trace(self, span: BamlSpan, response: typing.Any) -> None:
         await span.finish(response, self.ctx.get())
 
+    def end_trace_sync(self, span: BamlSpan, response: typing.Any) -> None:
+        span.finish_sync(response, self.ctx.get())
+
+    def flush(self) -> None:
+        self.rt.flush()
+
     def trace_fn(self, func: F) -> F:
         func_name = func.__name__
         signature = inspect.signature(func).parameters
         param_names = list(signature.keys())
 
         if asyncio.iscoroutinefunction(func):
 
@@ -79,14 +85,14 @@
                     param_names[i] if i < len(param_names) else f"<arg:{i}>": arg
                     for i, arg in enumerate(args)
                 }
                 params.update(kwargs)
                 span = self.start_trace_sync(func_name, params)
                 try:
                     response = func(*args, **kwargs)
-                    asyncio.run(self.end_trace(span, response))
+                    self.end_trace_sync(span, response)
                     return response
                 except Exception as e:
-                    asyncio.run(self.end_trace(span, e))
+                    self.end_trace_sync(span, e)
                     raise e
 
             return typing.cast(F, wrapper)
```

## baml_py/baml_py.pyi

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Callable, Dict, Optional
 
-class FunctionResultPy:
+class FunctionResult:
     """The result of a BAML function call.
 
     Represents any of:
 
         - a successful LLM call, with a successful type parse
         - a successful LLM call, with a failed type parse
         - a failed LLM call, due to a provider outage or other network error
@@ -13,68 +13,105 @@
 
     We only expose the parsed result to Python right now.
     """
 
     def __str__(self) -> str: ...
     def parsed(self) -> Any: ...
 
-class FunctionResultStreamPy:
+class FunctionResultStream:
     """The result of a BAML function stream.
 
     Provides a callback interface to receive events from a BAML result stream.
 
     Use `on_event` to set the callback, and `done` to drive the stream to completion.
     """
 
     def __str__(self) -> str: ...
     def on_event(
-        self, on_event: Callable[[FunctionResultPy], None]
-    ) -> FunctionResultStreamPy: ...
-    async def done(self, ctx: RuntimeContextManagerPy) -> FunctionResultPy: ...
+        self, on_event: Callable[[FunctionResult], None]
+    ) -> FunctionResultStream: ...
+    async def done(self, ctx: RuntimeContextManager) -> FunctionResult: ...
 
 class BamlImagePy:
     def __init__(
         self, url: Optional[str] = None, base64: Optional[str] = None
     ) -> None: ...
     @property
     def url(self) -> Optional[str]: ...
     @url.setter
     def url(self, value: Optional[str]) -> None: ...
     @property
     def base64(self) -> Optional[str]: ...
     @base64.setter
     def base64(self, value: Optional[str]) -> None: ...
 
-class RuntimeContextManagerPy:
+class RuntimeContextManager:
     def upsert_tags(self, tags: Dict[str, Any]) -> None: ...
-    def deep_clone(self) -> RuntimeContextManagerPy: ...
+    def deep_clone(self) -> RuntimeContextManager: ...
 
-class BamlRuntimePy:
+class BamlRuntime:
     @staticmethod
-    def from_directory(directory: str, env_vars: Dict[str, str]) -> BamlRuntimePy: ...
+    def from_directory(directory: str, env_vars: Dict[str, str]) -> BamlRuntime: ...
     async def call_function(
         self,
         function_name: str,
         args: Dict[str, Any],
-        ctx: RuntimeContextManagerPy,
-    ) -> FunctionResultPy: ...
+        ctx: RuntimeContextManager,
+        tb: Optional[TypeBuilder],
+    ) -> FunctionResult: ...
     def stream_function(
         self,
         function_name: str,
         args: Dict[str, Any],
-        on_event: Optional[Callable[[FunctionResultPy], None]],
-        ctx: RuntimeContextManagerPy,
-    ) -> FunctionResultStreamPy: ...
-    def create_context_manager(self) -> RuntimeContextManagerPy: ...
+        on_event: Optional[Callable[[FunctionResult], None]],
+        ctx: RuntimeContextManager,
+        tb: Optional[TypeBuilder],
+    ) -> FunctionResultStream: ...
+    def create_context_manager(self) -> RuntimeContextManager: ...
     def flush(self) -> None: ...
 
-class BamlSpanPy:
+class BamlSpan:
     @staticmethod
     def new(
-        runtime: BamlRuntimePy,
+        runtime: BamlRuntime,
         function_name: str,
         args: Dict[str, Any],
-        ctx: RuntimeContextManagerPy,
-    ) -> BamlSpanPy: ...
-    async def finish(self, result: Any, ctx: RuntimeContextManagerPy) -> str | None: ...
+        ctx: RuntimeContextManager,
+    ) -> BamlSpan: ...
+    async def finish(self, result: Any, ctx: RuntimeContextManager) -> str | None: ...
+
+class TypeBuilder:
+    def __init__(self) -> None: ...
+    def enum(self, name: str) -> EnumBuilder: ...
+    def class_(self, name: str) -> ClassBuilder: ...
+    def string(self) -> FieldType: ...
+    def int(self) -> FieldType: ...
+    def float(self) -> FieldType: ...
+    def bool(self) -> FieldType: ...
+    def list(self, element_type: FieldType) -> FieldType: ...
+    def null(self) -> FieldType: ...
+    def optional(self, inner_type: FieldType) -> FieldType: ...
+
+class FieldType:
+    def list(self, element_type: FieldType) -> FieldType: ...
+    def optional(self) -> FieldType: ...
+
+class EnumBuilder:
+    def value(self, name: str) -> EnumValueBuilder: ...
+    def alias(self, alias: Optional[str]) -> EnumBuilder: ...
+    def field(self) -> FieldType: ...
+
+class EnumValueBuilder:
+    def alias(self, alias: Optional[str]) -> EnumValueBuilder: ...
+    def skip(self, skip: Optional[bool] = True) -> EnumValueBuilder: ...
+    def description(self, description: Optional[str]) -> EnumValueBuilder: ...
+
+class ClassBuilder:
+    def field(self) -> FieldType: ...
+    def property(self, name: str) -> ClassPropertyBuilder: ...
+
+class ClassPropertyBuilder:
+    def type(self, field_type: FieldType) -> ClassPropertyBuilder: ...
+    def alias(self, alias: Optional[str]) -> ClassPropertyBuilder: ...
+    def description(self, description: Optional[str]) -> ClassPropertyBuilder: ...
 
 def invoke_runtime_cli() -> None: ...
```

## baml_py/stream.py

```diff
@@ -1,47 +1,58 @@
-from .baml_py import FunctionResultPy, FunctionResultStreamPy, RuntimeContextManagerPy
+from __future__ import annotations
+from .baml_py import (
+    FunctionResult,
+    FunctionResultStream,
+    RuntimeContextManager,
+    TypeBuilder,
+)
 from typing import Callable, Generic, Optional, TypeVar
+
 import asyncio
 
 PartialOutputType = TypeVar("PartialOutputType")
 FinalOutputType = TypeVar("FinalOutputType")
 
 
 class BamlStream(Generic[PartialOutputType, FinalOutputType]):
-    __ffi_stream: FunctionResultStreamPy
-    __partial_coerce: Callable[[FunctionResultPy], PartialOutputType]
-    __final_coerce: Callable[[FunctionResultPy], FinalOutputType]
-    __ctx_manager: RuntimeContextManagerPy
-
-    __task: Optional[asyncio.Task[FunctionResultPy]] = None
-    __event_queue: asyncio.Queue[Optional[FunctionResultPy]] = asyncio.Queue()
+    __ffi_stream: FunctionResultStream
+    __partial_coerce: Callable[[FunctionResult], PartialOutputType]
+    __final_coerce: Callable[[FunctionResult], FinalOutputType]
+    __ctx_manager: RuntimeContextManager
+    __task: Optional[asyncio.Task[FunctionResult]]
+    __event_queue: asyncio.Queue[Optional[FunctionResult]]
+    __tb: Optional[TypeBuilder]
 
     def __init__(
         self,
-        ffi_stream: FunctionResultStreamPy,
-        partial_coerce: Callable[[FunctionResultPy], PartialOutputType],
-        final_coerce: Callable[[FunctionResultPy], FinalOutputType],
-        ctx_manager: RuntimeContextManagerPy,
+        ffi_stream: FunctionResultStream,
+        partial_coerce: Callable[[FunctionResult], PartialOutputType],
+        final_coerce: Callable[[FunctionResult], FinalOutputType],
+        ctx_manager: RuntimeContextManager,
+        tb: Optional[TypeBuilder],
     ):
         self.__ffi_stream = ffi_stream.on_event(self.__enqueue)
         self.__partial_coerce = partial_coerce
         self.__final_coerce = final_coerce
         self.__ctx_manager = ctx_manager
+        self.__task = None
+        self.__event_queue = asyncio.Queue()
+        self.__tb = tb
 
-    def __enqueue(self, data: FunctionResultPy) -> None:
+    def __enqueue(self, data: FunctionResult) -> None:
         self.__event_queue.put_nowait(data)
 
-    async def __drive_to_completion(self) -> FunctionResultPy:
+    async def __drive_to_completion(self) -> FunctionResult:
         try:
             retval = await self.__ffi_stream.done(self.__ctx_manager)
             return retval
         finally:
             self.__event_queue.put_nowait(None)
 
-    def __drive_to_completion_in_bg(self) -> asyncio.Task[FunctionResultPy]:
+    def __drive_to_completion_in_bg(self) -> asyncio.Task[FunctionResult]:
         # Doing this without using a compare-and-swap or lock is safe,
         # because we don't cross an await point during it
         if self.__task is None:
             self.__task = asyncio.create_task(self.__drive_to_completion())
 
         return self.__task
 
@@ -49,10 +60,10 @@
         self.__drive_to_completion_in_bg()
         while True:
             event = await self.__event_queue.get()
             if event is None:
                 break
             yield self.__partial_coerce(event.parsed())
 
-    async def done(self):
+    async def get_final_response(self):
         final = await self.__drive_to_completion_in_bg()
         return self.__final_coerce(final.parsed())
```

## baml_py/__init__.py

```diff
@@ -1,22 +1,22 @@
 # BAML Python API: provides the Python API for the BAML runtime.
 
 # Re-export the pyo3 API
 from .baml_py import (
-    BamlRuntimePy,
-    FunctionResultPy,
-    FunctionResultStreamPy,
+    BamlRuntime,
+    FunctionResult,
+    FunctionResultStream,
     BamlImagePy as Image,
     invoke_runtime_cli,
 )
 from .stream import BamlStream
 from .async_context_vars import CtxManager as BamlCtxManager
 
 __all__ = [
-    "BamlRuntimePy",
+    "BamlRuntime",
     "BamlStream",
     "BamlCtxManager",
-    "FunctionResultPy",
-    "FunctionResultStreamPy",
+    "FunctionResult",
+    "FunctionResultStream",
     "Image",
     "invoke_runtime_cli",
 ]
```

## Comparing `baml_py-0.1.9.dist-info/license_files/LICENSE` & `baml_py-0.30.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `baml_py-0.1.9.dist-info/RECORD` & `baml_py-0.30.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-baml_py-0.1.9.dist-info/METADATA,sha256=poIApPg_sfrbEWC3FoFT-69_g9PGoHGZON08jHKddaI,336
-baml_py-0.1.9.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
-baml_py-0.1.9.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
-baml_py-0.1.9.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py-0.1.9.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py/async_context_vars.py,sha256=CnXmz5can4Hr0-051fHrcTdczothNrTqX_zPa9FCBkc,3272
-baml_py/baml_py.pyi,sha256=mwzKOCJ6bL95g_Hq9ztkiedp0Qs7ukJPULyfHChsqgA,2641
+baml_py-0.30.0.dist-info/METADATA,sha256=lVJEJWOjCw5PuJGyIFwxUFuMwv34DMqOQd02U14eedc,337
+baml_py-0.30.0.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
+baml_py-0.30.0.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
+baml_py-0.30.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py-0.30.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py/async_context_vars.py,sha256=gU_H0abCPxxULNRUArMlsx2aeLNp7E7fIVBY6nLY_F0,3422
+baml_py/baml_py.pyi,sha256=loMZFT2iecP59NwPzqtFxvRvNIjgB8bgLvmufg9Y8sQ,4095
 baml_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-baml_py/stream.py,sha256=xfKe4QvtIAlTTi_n3gKx7JwVRsXx9M15y3yzlgirK7Y,2275
-baml_py/__init__.py,sha256=e6R5i-ssLiaT9XoWWW_k9B6ToPtIe-QlkJTLIPpwgzI,518
-baml_py/baml_py.pyd,sha256=6WSU9nkC_Pcp6Gimjcc1dHOe7_XkOL3Om4ZJvwxb1dg,11260928
-baml_py-0.1.9.dist-info/RECORD,,
+baml_py/stream.py,sha256=B4mpGnqAmU7DFHJPiAAAiNIeX5wgLJhXLZp9Pqb9-AY,2474
+baml_py/type_builder.py,sha256=v3yiY2VtGuCEECr0jh7OB3ueWSiSwj-8IETXQuSIYl0,4330
+baml_py/__init__.py,sha256=-y49naDuvHdmpkmUEqZBESlBNx6W4qsPOPu9KlrMT10,506
+baml_py/baml_py.pyd,sha256=Uqq7VoFkJfBr6N7RMLFU5JEybBgoNkyOeVP-ZytNUZ8,11762688
+baml_py-0.30.0.dist-info/RECORD,,
```

