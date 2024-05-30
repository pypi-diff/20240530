# Comparing `tmp/replit_river-0.2.1.tar.gz` & `tmp/replit_river-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.2.1.tar", max compression
+gzip compressed data, was "replit_river-0.2.2.tar", max compression
```

## Comparing `replit_river-0.2.1.tar` & `replit_river-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.2.1/LICENSE
--rw-r--r--   0        0        0     1830 2024-05-28 18:58:27.630238 replit_river-0.2.1/README.md
--rw-r--r--   0        0        0     1743 2024-05-28 18:58:27.630432 replit_river-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-17 00:20:58.071349 replit_river-0.2.1/replit_river/__init__.py
--rw-r--r--   0        0        0     3948 2024-05-20 18:10:16.102006 replit_river-0.2.1/replit_river/client.py
--rw-r--r--   0        0        0    10471 2024-05-10 03:47:14.291086 replit_river-0.2.1/replit_river/client_session.py
--rw-r--r--   0        0        0    10838 2024-05-16 17:24:05.935756 replit_river-0.2.1/replit_river/client_transport.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.2.1/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.2.1/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13487 2024-05-28 18:58:27.631495 replit_river-0.2.1/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.2.1/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5356 2024-05-03 21:34:57.699549 replit_river-0.2.1/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12624 2024-05-03 21:34:57.728664 replit_river-0.2.1/replit_river/codegen/server.py
--rw-r--r--   0        0        0      547 2024-04-30 17:01:06.486105 replit_river-0.2.1/replit_river/error_schema.py
--rw-r--r--   0        0        0     1482 2024-05-02 05:31:22.056992 replit_river-0.2.1/replit_river/message_buffer.py
--rw-r--r--   0        0        0     3329 2024-05-02 05:31:22.057415 replit_river-0.2.1/replit_river/messages.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.2.1/replit_river/py.typed
--rw-r--r--   0        0        0     3625 2024-05-16 17:24:05.936350 replit_river-0.2.1/replit_river/rate_limiter.py
--rw-r--r--   0        0        0    13076 2024-05-28 18:58:27.631698 replit_river-0.2.1/replit_river/rpc.py
--rw-r--r--   0        0        0     2293 2024-05-06 23:37:30.281093 replit_river-0.2.1/replit_river/seq_manager.py
--rw-r--r--   0        0        0     2733 2024-05-10 03:59:49.021884 replit_river-0.2.1/replit_river/server.py
--rw-r--r--   0        0        0     5947 2024-05-10 03:47:14.293359 replit_river-0.2.1/replit_river/server_transport.py
--rw-r--r--   0        0        0    19664 2024-05-28 18:58:27.632031 replit_river-0.2.1/replit_river/session.py
--rw-r--r--   0        0        0     3827 2024-05-10 03:47:14.294335 replit_river-0.2.1/replit_river/task_manager.py
--rw-r--r--   0        0        0     5350 2024-05-10 03:47:14.294944 replit_river-0.2.1/replit_river/transport.py
--rw-r--r--   0        0        0     1676 2024-05-10 03:47:14.295278 replit_river-0.2.1/replit_river/transport_options.py
--rw-r--r--   0        0        0      901 2024-05-03 21:53:04.428732 replit_river-0.2.1/replit_river/websocket_wrapper.py
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 replit_river-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1830 2024-05-28 18:58:27.630238 replit_river-0.2.2/README.md
+-rw-r--r--   0        0        0     1743 2024-05-30 05:40:08.435621 replit_river-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-17 00:20:58.071349 replit_river-0.2.2/replit_river/__init__.py
+-rw-r--r--   0        0        0     3948 2024-05-20 18:10:16.102006 replit_river-0.2.2/replit_river/client.py
+-rw-r--r--   0        0        0    10471 2024-05-10 03:47:14.291086 replit_river-0.2.2/replit_river/client_session.py
+-rw-r--r--   0        0        0    10838 2024-05-16 17:24:05.935756 replit_river-0.2.2/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.2.2/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.2.2/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13631 2024-05-30 05:31:15.317139 replit_river-0.2.2/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.2.2/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5356 2024-05-03 21:34:57.699549 replit_river-0.2.2/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12624 2024-05-03 21:34:57.728664 replit_river-0.2.2/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      547 2024-04-30 17:01:06.486105 replit_river-0.2.2/replit_river/error_schema.py
+-rw-r--r--   0        0        0     1482 2024-05-02 05:31:22.056992 replit_river-0.2.2/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     3329 2024-05-02 05:31:22.057415 replit_river-0.2.2/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.2.2/replit_river/py.typed
+-rw-r--r--   0        0        0     3625 2024-05-16 17:24:05.936350 replit_river-0.2.2/replit_river/rate_limiter.py
+-rw-r--r--   0        0        0    13076 2024-05-28 18:58:27.631698 replit_river-0.2.2/replit_river/rpc.py
+-rw-r--r--   0        0        0     2293 2024-05-06 23:37:30.281093 replit_river-0.2.2/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     2733 2024-05-10 03:59:49.021884 replit_river-0.2.2/replit_river/server.py
+-rw-r--r--   0        0        0     5947 2024-05-10 03:47:14.293359 replit_river-0.2.2/replit_river/server_transport.py
+-rw-r--r--   0        0        0    19664 2024-05-28 18:58:27.632031 replit_river-0.2.2/replit_river/session.py
+-rw-r--r--   0        0        0     3827 2024-05-10 03:47:14.294335 replit_river-0.2.2/replit_river/task_manager.py
+-rw-r--r--   0        0        0     5350 2024-05-10 03:47:14.294944 replit_river-0.2.2/replit_river/transport.py
+-rw-r--r--   0        0        0     1676 2024-05-10 03:47:14.295278 replit_river-0.2.2/replit_river/transport_options.py
+-rw-r--r--   0        0        0      901 2024-05-03 21:53:04.428732 replit_river-0.2.2/replit_river/websocket_wrapper.py
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 replit_river-0.2.2/PKG-INFO
```

### Comparing `replit_river-0.2.1/LICENSE` & `replit_river-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/README.md` & `replit_river-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/pyproject.toml` & `replit_river-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.2.1"
+version="0.2.2"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.2.1/replit_river/client.py` & `replit_river-0.2.2/replit_river/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/client_session.py` & `replit_river-0.2.2/replit_river/client_session.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/client_transport.py` & `replit_river-0.2.2/replit_river/client_transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/codegen/client.py` & `replit_river-0.2.2/replit_river/codegen/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
             if type.const:
                 return (f"Literal['{type.const}']", ())
             else:
                 return ("str", ())
         if type.type == "Uint8Array":
             return ("bytes", ())
         if type.type == "number":
+            if type.const is not None:
+                # enums are represented as const number in the schema
+                return ("int", ())
             return ("float", ())
         if type.type == "integer":
             return ("int", ())
         if type.type == "boolean":
             return ("bool", ())
         if type.type == "Date":
             return ("datetime.datetime", ())
```

### Comparing `replit_river-0.2.1/replit_river/codegen/run.py` & `replit_river-0.2.2/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/codegen/schema.py` & `replit_river-0.2.2/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/codegen/server.py` & `replit_river-0.2.2/replit_river/codegen/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/error_schema.py` & `replit_river-0.2.2/replit_river/error_schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/message_buffer.py` & `replit_river-0.2.2/replit_river/message_buffer.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/messages.py` & `replit_river-0.2.2/replit_river/messages.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/rate_limiter.py` & `replit_river-0.2.2/replit_river/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/rpc.py` & `replit_river-0.2.2/replit_river/rpc.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/seq_manager.py` & `replit_river-0.2.2/replit_river/seq_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/server.py` & `replit_river-0.2.2/replit_river/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/server_transport.py` & `replit_river-0.2.2/replit_river/server_transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/session.py` & `replit_river-0.2.2/replit_river/session.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/task_manager.py` & `replit_river-0.2.2/replit_river/task_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/transport.py` & `replit_river-0.2.2/replit_river/transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/transport_options.py` & `replit_river-0.2.2/replit_river/transport_options.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/replit_river/websocket_wrapper.py` & `replit_river-0.2.2/replit_river/websocket_wrapper.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.2.1/PKG-INFO` & `replit_river-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.2.1
+Version: 0.2.2
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

