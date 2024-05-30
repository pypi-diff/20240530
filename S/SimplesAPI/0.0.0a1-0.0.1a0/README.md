# Comparing `tmp/simplesapi-0.0.0a1.tar.gz` & `tmp/simplesapi-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesapi-0.0.0a1.tar", max compression
+gzip compressed data, was "simplesapi-0.0.1a0.tar", max compression
```

## Comparing `simplesapi-0.0.0a1.tar` & `simplesapi-0.0.1a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      401 2024-05-30 15:41:41.699682 simplesapi-0.0.0a1/pyproject.toml
--rw-r--r--   0        0        0       12 2024-05-30 15:30:50.326578 simplesapi-0.0.0a1/README.md
--rw-r--r--   0        0        0       65 2024-05-30 15:29:19.925959 simplesapi-0.0.0a1/simplesapi/__init__.py
--rw-r--r--   0        0        0      835 2024-05-30 15:29:18.782917 simplesapi-0.0.0a1/simplesapi/app.py
--rw-r--r--   0        0        0     1340 2024-05-30 15:29:16.921041 simplesapi-0.0.0a1/simplesapi/auto_routing.py
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 simplesapi-0.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/README.md
+-rw-r--r--   0        0        0      382 2024-05-30 15:17:50.665460 simplesapi-0.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/simplesapi/__init__.py
+-rw-r--r--   0        0        0      813 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/simplesapi/app.py
+-rw-r--r--   0        0        0     1300 2024-05-30 15:17:38.677459 simplesapi-0.0.1a0/simplesapi/auto_routing.py
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 simplesapi-0.0.1a0/PKG-INFO
```

### Comparing `simplesapi-0.0.0a1/simplesapi/app.py` & `simplesapi-0.0.1a0/simplesapi/app.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-
-from typing import Optional
-from fastapi import FastAPI
-from pydantic import BaseModel, Field
-
-from simplesapi.auto_routing import register_routes
-
-class _Simples(BaseModel):
-    verbose: bool
-    base_path: Optional[str] = Field(default="/")
-    redis_conn: Optional[str] = Field(default=None)
-    postgres_conn: Optional[str] = Field(default=None)
-    mysql_conn: Optional[str] = Field(default=None)
-
-class SimplesAPI(FastAPI):
-    def __init__(self, title="SimplesAPI", version="0.1.0", routes_path=None, base_path=None, redis_conn=None, postgres_conn=None, mysql_conn=None, verbose=False):
-        super().__init__(title=title, version=version)
-        self.simples = _Simples(verbose=verbose)
-        if routes_path:
-            register_routes(self,routes_path)
-
-    def validate_simples(self):
+
+from typing import Optional
+from fastapi import FastAPI
+from pydantic import BaseModel, Field
+
+from simplesapi.auto_routing import register_routes
+
+class _Simples(BaseModel):
+    verbose: bool
+    base_path: Optional[str] = Field(default="/")
+    redis_conn: Optional[str] = Field(default=None)
+    postgres_conn: Optional[str] = Field(default=None)
+    mysql_conn: Optional[str] = Field(default=None)
+
+class SimplesAPI(FastAPI):
+    def __init__(self, title="SimplesAPI", version="0.1.0", routes_path=None, base_path=None, redis_conn=None, postgres_conn=None, mysql_conn=None, verbose=False):
+        super().__init__(title=title, version=version)
+        self.simples = _Simples(verbose=verbose)
+        if routes_path:
+            register_routes(self,routes_path)
+
+    def validate_simples(self):
         ...
```

### Comparing `simplesapi-0.0.0a1/simplesapi/auto_routing.py` & `simplesapi-0.0.1a0/simplesapi/auto_routing.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-
-import importlib
-import os
-
-
-def _import_handler(module_path, handler_name="handler"):
-    spec = importlib.util.spec_from_file_location("routes", module_path)
-    module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
-    return getattr(module, handler_name)
-
-def _create_route_from_file(app, file_path):
-    parts = file_path.split(os.sep)
-    method_file = parts[-1]
-    method = method_file.split('.')[0].split('__')[1].lower() if '__' in method_file else method_file.split('.')[0].lower()
-    
-    route = os.sep.join(parts[:-1])
-    route = route.replace('routes', '')
-    route = route.replace('[', '{').replace(']', '}')
-    route = '/' + route.strip(os.sep)
-
-    handler = _import_handler(file_path)
-    
-    if method == "get":
-        app.get(route)(handler)
-    elif method == "post":
-        app.post(route)(handler)
-    elif method == "put":
-        app.put(route)(handler)
-    elif method == "delete":
-        app.delete(route)(handler)
-    elif method == "patch":
-        app.patch(route)(handler)
-
-def register_routes(app, base_path):
-    for root, _, files in os.walk(base_path):
-        for file in files:
-            if file.endswith('.py'):
-                file_path = os.path.join(root, file)
-                _create_route_from_file(app, file_path)
+
+import importlib
+import os
+
+
+def _import_handler(module_path, handler_name="handler"):
+    spec = importlib.util.spec_from_file_location("routes", module_path)
+    module = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+    return getattr(module, handler_name)
+
+def _create_route_from_file(app, file_path):
+    parts = file_path.split(os.sep)
+    method_file = parts[-1]
+    method = method_file.split('.')[0].split('__')[1].lower() if '__' in method_file else method_file.split('.')[0].lower()
+    
+    route = os.sep.join(parts[:-1])
+    route = route.replace('routes', '')
+    route = route.replace('[', '{').replace(']', '}')
+    route = '/' + route.strip(os.sep)
+
+    handler = _import_handler(file_path)
+    
+    if method == "get":
+        app.get(route)(handler)
+    elif method == "post":
+        app.post(route)(handler)
+    elif method == "put":
+        app.put(route)(handler)
+    elif method == "delete":
+        app.delete(route)(handler)
+    elif method == "patch":
+        app.patch(route)(handler)
+
+def register_routes(app, base_path):
+    for root, _, files in os.walk(base_path):
+        for file in files:
+            if file.endswith('.py'):
+                file_path = os.path.join(root, file)
+                _create_route_from_file(app, file_path)
```

