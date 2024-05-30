# Comparing `tmp/stencila_plugin-2.0.0a33.tar.gz` & `tmp/stencila_plugin-2.0.0a34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stencila_plugin-2.0.0a33.tar", last modified: Tue May 21 05:09:52 2024, max compression
+gzip compressed data, was "stencila_plugin-2.0.0a34.tar", last modified: Thu May 30 04:40:22 2024, max compression
```

## Comparing `stencila_plugin-2.0.0a33.tar` & `stencila_plugin-2.0.0a34.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      890 2024-03-26 01:26:24.321915 stencila_plugin-2.0.0a33/README.md
--rw-r--r--   0        0        0     1865 2024-05-21 05:09:52.186250 stencila_plugin-2.0.0a33/pyproject.toml
--rw-r--r--   0        0        0      319 2024-05-21 03:23:15.043705 stencila_plugin-2.0.0a33/src/stencila_plugin/__init__.py
--rw-r--r--   0        0        0     4085 2024-05-21 03:23:15.043904 stencila_plugin-2.0.0a33/src/stencila_plugin/assistant.py
--rw-r--r--   0        0        0     5721 2024-03-26 03:21:24.057751 stencila_plugin-2.0.0a33/src/stencila_plugin/kernel.py
--rw-r--r--   0        0        0    12223 2024-05-21 03:23:15.044355 stencila_plugin-2.0.0a33/src/stencila_plugin/plugin.py
--rw-r--r--   0        0        0     8224 2024-03-26 01:26:24.323664 stencila_plugin-2.0.0a33/src/stencila_plugin/testing.py
--rw-r--r--   0        0        0        0 2024-03-26 01:26:24.323733 stencila_plugin-2.0.0a33/tests/__init__.py
--rw-r--r--   0        0        0      875 2024-03-26 01:26:24.323815 stencila_plugin-2.0.0a33/tests/conftest.py
--rw-r--r--   0        0        0     1126 2024-05-21 03:23:15.044616 stencila_plugin-2.0.0a33/tests/plugin_example.py
--rw-r--r--   0        0        0     3261 2024-05-21 03:23:15.045065 stencila_plugin-2.0.0a33/tests/test_plugin.py
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a33/PKG-INFO
+-rw-r--r--   0        0        0      890 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/README.md
+-rw-r--r--   0        0        0     1865 2024-05-30 04:40:22.492480 stencila_plugin-2.0.0a34/pyproject.toml
+-rw-r--r--   0        0        0      319 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/src/stencila_plugin/__init__.py
+-rw-r--r--   0        0        0     4085 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/src/stencila_plugin/assistant.py
+-rw-r--r--   0        0        0     5721 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/src/stencila_plugin/kernel.py
+-rw-r--r--   0        0        0    12347 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/src/stencila_plugin/plugin.py
+-rw-r--r--   0        0        0     8274 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/src/stencila_plugin/testing.py
+-rw-r--r--   0        0        0        0 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/tests/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/tests/conftest.py
+-rw-r--r--   0        0        0     1126 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/tests/plugin_example.py
+-rw-r--r--   0        0        0     3261 2024-05-30 04:39:54.880469 stencila_plugin-2.0.0a34/tests/test_plugin.py
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 stencila_plugin-2.0.0a34/PKG-INFO
```

### Comparing `stencila_plugin-2.0.0a33/README.md` & `stencila_plugin-2.0.0a34/README.md`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a33/pyproject.toml` & `stencila_plugin-2.0.0a34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "stencila_plugin"
-version = "2.0.0a33"
+version = "2.0.0a34"
 description = "Library for building Stencila Plugins"
 readme = "README.md"
 authors = [
     { name = "Nokome Bentley", email = "nokome@stencila.io" },
     { name = "Brett Calcott", email = "brett@dragonfly.co.nz" },
 ]
 dependencies = [
     "aiohttp>=3.9.3",
-    "stencila-types==2.0.0a30",
+    "stencila-types==2.0.0a31",
 ]
 requires-python = ">=3.10"
 keywords = [
     "programmable",
     "reproducible",
     "interactive",
     "documents",
```

### Comparing `stencila_plugin-2.0.0a33/src/stencila_plugin/assistant.py` & `stencila_plugin-2.0.0a34/src/stencila_plugin/assistant.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a33/src/stencila_plugin/kernel.py` & `stencila_plugin-2.0.0a34/src/stencila_plugin/kernel.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a33/src/stencila_plugin/plugin.py` & `stencila_plugin-2.0.0a34/src/stencila_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,19 +254,23 @@
     if method is None:
         return _error(None, RPCErrorCodes.METHOD_NOT_FOUND, "No method sent")
 
     # This can be None
     msg_id: IdType = request.get("id")  # type: ignore
 
     # According to the standard, the params can be an Array or an Object (a dict).
-    # We also handle None.
+    # We handle None as by converting to an empty dict.
     params = request.get("params")
+    if params is None:
+        params = {}
 
     if not isinstance(params, dict):
-        return _error(None, RPCErrorCodes.INVALID_PARAMS, "")
+        return _error(
+            None, RPCErrorCodes.INVALID_PARAMS, "Did not recieve a dict or null"
+        )
 
     # Hm. Still struggling with typing here.
     return await _handle_rpc(plugin, method, params=params, msg_id=msg_id)  # type: ignore
 
 
 async def _handle_rpc(
     plugin: Plugin,
```

### Comparing `stencila_plugin-2.0.0a33/src/stencila_plugin/testing.py` & `stencila_plugin-2.0.0a34/src/stencila_plugin/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,17 @@
         Args:
             method (str): Name of the method to call.
             params (ParamsType, optional): Parameters to pass to the method.
 
         Returns:
             JSONDict: The result of the RPC call (if successful).
         """
+        if not kwargs:
+            kwargs = None
+
         request = {
             "jsonrpc": "2.0",
             "method": method,
             "params": kwargs,
             "id": self.next_id,
         }
         self.next_id += 1
```

### Comparing `stencila_plugin-2.0.0a33/tests/conftest.py` & `stencila_plugin-2.0.0a34/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a33/tests/plugin_example.py` & `stencila_plugin-2.0.0a34/tests/plugin_example.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a33/tests/test_plugin.py` & `stencila_plugin-2.0.0a34/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `stencila_plugin-2.0.0a33/PKG-INFO` & `stencila_plugin-2.0.0a34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: stencila_plugin
-Version: 2.0.0a33
+Version: 2.0.0a34
 Summary: Library for building Stencila Plugins
 Keywords: programmable,reproducible,interactive,documents,python,SDK
 Author-Email: Nokome Bentley <nokome@stencila.io>, Brett Calcott <brett@dragonfly.co.nz>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Homepage, https://github.com/stencila/stencila/tree/main/python#readme
 Project-URL: Repository, https://github.com/stencila/stencila
 Requires-Python: >=3.10
 Requires-Dist: aiohttp>=3.9.3
-Requires-Dist: stencila-types==2.0.0a30
+Requires-Dist: stencila-types==2.0.0a31
 Description-Content-Type: text/markdown
 
 # Stencila Plugin
 
 [![stencila_plugin](https://img.shields.io/pypi/v/stencila_plugin.svg?logo=python&label=stencila_plugin&style=for-the-badge&color=1d3bd1&logoColor=66ff66&labelColor=3219a8)](https://pypi.org/project/stencila_plugin/)
 
 ## Introduction
```

