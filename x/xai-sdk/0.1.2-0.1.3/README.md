# Comparing `tmp/xai_sdk-0.1.2.tar.gz` & `tmp/xai_sdk-0.1.3.tar.gz`

## Comparing `xai_sdk-0.1.2.tar` & `xai_sdk-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/Makefile
--rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/create_bindings.sh
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/__about__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/__init__.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/chat.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/client.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/files.py
--rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/grok.py
--rw-r--r--   0        0        0    17025 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/ide.py
--rw-r--r--   0        0        0    13895 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/sampler.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/compat/__init__.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/compat/chat.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/compat/client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/__init__.py
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.py
--rw-r--r--   0        0        0    13089 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.pyi
--rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2_grpc.py
--rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.py
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.pyi
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2_grpc.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.pyi
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2_grpc.py
--rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.py
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.pyi
--rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2_grpc.py
--rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.py
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.pyi
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2_grpc.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.pyi
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/__init__.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/README.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/Makefile
+-rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/create_bindings.sh
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/__about__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/__init__.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/chat.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/client.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/files.py
+-rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/grok.py
+-rw-r--r--   0        0        0    17025 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/ide.py
+-rw-r--r--   0        0        0    13905 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/sampler.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/compat/__init__.py
+-rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/compat/chat.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/compat/client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/__init__.py
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/chat_pb2.py
+-rw-r--r--   0        0        0    13089 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/chat_pb2.pyi
+-rw-r--r--   0        0        0    15032 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/chat_pb2_grpc.py
+-rw-r--r--   0        0        0     5718 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/compat_chat_pb2.py
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/compat_chat_pb2.pyi
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/compat_chat_pb2_grpc.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/files_pb2.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/files_pb2.pyi
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/files_pb2_grpc.py
+-rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/prod_search_pb2.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/prod_search_pb2.pyi
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/prod_search_pb2_grpc.py
+-rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/sampler_public_pb2.py
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/sampler_public_pb2.pyi
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/sampler_public_pb2_grpc.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/stateless_chat_pb2.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/stateless_chat_pb2.pyi
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/stateless_chat_pb2_grpc.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/x_entities_pb2.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/x_entities_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/x_entities_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/api/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/api/http_pb2.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/src/xai_sdk/proto/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 xai_sdk-0.1.3/PKG-INFO
```

### Comparing `xai_sdk-0.1.2/Makefile` & `xai_sdk-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/create_bindings.sh` & `xai_sdk-0.1.3/create_bindings.sh`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/__init__.py` & `xai_sdk-0.1.3/src/xai_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
     python -c "import xai_sdk; xai_sdk.does_it_work()"
     ```
     """
 
     async def _run():
         prompt = "Yes, it does. Yes, it does. Yes, it does. Yes, it does. Yes, it does."
         print("Does it work?", end="")
-        async for token in Client().sampler.sample(prompt, stop_strings=["."]):
+        async for token in Client().sampler.sample(prompt=prompt, stop_strings=["."]):
             print(token.token_str, end="")
         print("")
 
     asyncio.run(_run())
```

### Comparing `xai_sdk-0.1.2/src/xai_sdk/chat.py` & `xai_sdk-0.1.3/src/xai_sdk/chat.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/client.py` & `xai_sdk-0.1.3/src/xai_sdk/client.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/files.py` & `xai_sdk-0.1.3/src/xai_sdk/files.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/grok.py` & `xai_sdk-0.1.3/src/xai_sdk/grok.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/ide.py` & `xai_sdk-0.1.3/src/xai_sdk/ide.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/sampler.py` & `xai_sdk-0.1.3/src/xai_sdk/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         return [Token.from_proto(token) for token in tokens]
 
     async def sample(
         self,
         *,
         prompt: Union[str, Sequence[int], Sequence["Token"]],
-        inputs: Sequence[Union[str, int, bytes]] = (),
+        inputs: Sequence[Union[str, Sequence[int], bytes]] = (),
         model_name: str = "",
         max_len: int = 256,
         temperature: float = 0.7,
         nucleus_p: float = 0.95,
         stop_tokens: Optional[list[str]] = None,
         stop_strings: Optional[list[str]] = None,
         rng_seed: Optional[int] = None,
```

### Comparing `xai_sdk-0.1.2/src/xai_sdk/compat/chat.py` & `xai_sdk-0.1.3/src/xai_sdk/compat/chat.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/compat/client.py` & `xai_sdk-0.1.3/src/xai_sdk/compat/client.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/chat_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/chat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/chat_pb2_grpc.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/compat_chat_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/compat_chat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/compat_chat_pb2_grpc.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/compat_chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/files_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/files_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/files_pb2_grpc.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/files_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/prod_search_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/prod_search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/prod_search_pb2_grpc.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/prod_search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/sampler_public_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/sampler_public_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/sampler_public_pb2_grpc.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/sampler_public_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/stateless_chat_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/stateless_chat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/stateless_chat_pb2_grpc.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/stateless_chat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/x_entities_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/x_entities_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/x_entities_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/google/api/annotations_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.py` & `xai_sdk-0.1.3/src/xai_sdk/proto/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/src/xai_sdk/proto/google/api/http_pb2.pyi` & `xai_sdk-0.1.3/src/xai_sdk/proto/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/.gitignore` & `xai_sdk-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/LICENSE.txt` & `xai_sdk-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/pyproject.toml` & `xai_sdk-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xai_sdk-0.1.2/PKG-INFO` & `xai_sdk-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xai-sdk
-Version: 0.1.2
+Version: 0.1.3
 Project-URL: Documentation, https://x.ai/api/sdk.html
 Author-email: Toby Pohlen <pohlen@x.ai>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

