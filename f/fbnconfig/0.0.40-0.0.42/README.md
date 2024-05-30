# Comparing `tmp/fbnconfig-0.0.40.tar.gz` & `tmp/fbnconfig-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbnconfig-0.0.40.tar", max compression
+gzip compressed data, was "fbnconfig-0.0.42.tar", max compression
```

## Comparing `fbnconfig-0.0.40.tar` & `fbnconfig-0.0.42.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      176 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig/__init__.py
--rw-r--r--   0        0        0     6600 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig/access.py
--rw-r--r--   0        0        0     9838 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig/configuration.py
--rw-r--r--   0        0        0     4191 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/deploy.py
--rw-r--r--   0        0        0     8124 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/drive.py
--rw-r--r--   0        0        0     7488 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/identity.py
--rw-r--r--   0        0        0     1057 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/load_module.py
--rw-r--r--   0        0        0     9681 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/log.py
--rw-r--r--   0        0        0     8283 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/main.py
--rw-r--r--   0        0        0     6618 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/property.py
--rw-r--r--   0        0        0      771 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/resource_abc.py
--rw-r--r--   0        0        0    14708 2024-04-15 07:44:42.792177 fbnconfig-0.0.40/fbnconfig/scheduler.py
--rw-r--r--   0        0        0     9716 2024-04-15 07:44:42.791177 fbnconfig-0.0.40/fbnconfig.md
--rw-r--r--   0        0        0     1070 2024-04-15 07:48:05.118508 fbnconfig-0.0.40/pyproject.toml
--rw-r--r--   0        0        0    10248 1970-01-01 00:00:00.000000 fbnconfig-0.0.40/PKG-INFO
+-rw-r--r--   0        0        0      181 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/__init__.py
+-rw-r--r--   0        0        0     6600 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/access.py
+-rw-r--r--   0        0        0     9838 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/configuration.py
+-rw-r--r--   0        0        0     3473 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/deploy.py
+-rw-r--r--   0        0        0     8124 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/drive.py
+-rw-r--r--   0        0        0     1415 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/http_client.py
+-rw-r--r--   0        0        0     7488 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/identity.py
+-rw-r--r--   0        0        0     1057 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/load_module.py
+-rw-r--r--   0        0        0     9681 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/log.py
+-rw-r--r--   0        0        0    14460 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/lumi.py
+-rw-r--r--   0        0        0     8338 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/main.py
+-rw-r--r--   0        0        0     6618 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/property.py
+-rw-r--r--   0        0        0      785 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/resource_abc.py
+-rw-r--r--   0        0        0    14708 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig/scheduler.py
+-rw-r--r--   0        0        0     9716 2024-05-30 08:29:53.000000 fbnconfig-0.0.42/fbnconfig.md
+-rw-r--r--   0        0        0     1070 2024-05-30 08:40:12.312160 fbnconfig-0.0.42/pyproject.toml
+-rw-r--r--   0        0        0    10248 1970-01-01 00:00:00.000000 fbnconfig-0.0.42/PKG-INFO
```

### Comparing `fbnconfig-0.0.40/fbnconfig/access.py` & `fbnconfig-0.0.42/fbnconfig/access.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig/configuration.py` & `fbnconfig-0.0.42/fbnconfig/configuration.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig/deploy.py` & `fbnconfig-0.0.42/fbnconfig/deploy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import httpx
-import os
 import json
 from types import SimpleNamespace
 from typing import NamedTuple, List, Union
 from . import log
 from .resource_abc import Resource, Ref
+from . import http_client
 
 # import all resources here, so they are available in globals()
 from .drive import FolderResource, FileResource  # noqa: F401
 from .scheduler import ImageResource, JobResource, ScheduleResource  # noqa: F401
 from .access import PolicyResource, RoleResource  # noqa: F401
 from .identity import IdentityRoleResource, UserResource, RoleAssignment  # noqa: F401
 from .configuration import SetResource, ItemResource, SystemConfigResource  # noqa: F401
 from .property import DefinitionResource  # noqa: F401
+from .lumi import ViewResource # noqa: F401
 
 Deployment = NamedTuple("Deployment", [("id", str), ("resources", List[Union[Resource, Ref]])])
 deployments = []
 
 
 def deployment(id, resources):
     d = Deployment(id, resources)
@@ -54,41 +55,14 @@
                 seen.add(e.resource_id)
                 ordered.append(e)
 
     helper(entries)
     return ordered
 
 
-# Throw an exception whenever the response code is 4xx or 5xx
-def response_hook(response: httpx.Response) -> None:
-    if response.is_error:
-        response.read()
-        response.raise_for_status()
-
-
-def create_client(lusid_url: str, token: str) -> httpx.Client:
-    if token is None or lusid_url is None:
-        raise (
-            RuntimeError(
-                "Both FBN_ACCESS_TOKEN and LUSID_ENV variables need to be set"
-            )
-        )
-
-    return httpx.Client(
-        base_url=lusid_url,
-        timeout=20,
-        headers={
-            "authorization": "Bearer " + os.getenv("FBN_ACCESS_TOKEN", default=""),
-            "accept": "application/json",
-            "content-type": "application/json",
-        },
-        event_hooks={"response": [response_hook]},
-    )
-
-
 def run(client: httpx.Client, deployment):
     resources = deployment.resources
     deploy_state = log.list_resources_for_deployment(client, deployment.id)
     all_resources = recurse_resources(resources)
     for resource in all_resources:
         if isinstance(resource, Ref):
             resource.attach(client)
@@ -111,15 +85,15 @@
             klas = globals()[deployed.resource_type]
             print("deploy: remove", deployed.resource_type, deployed.resource_id)
             klas.delete(client, deployed.state)
             log.remove(client, deployment.id, deployed.resource_id)
 
 # called as a library
 def deploy(deployment: Deployment, lusid_url: str, access_token: str):
-    client = create_client(lusid_url, access_token)
+    client = http_client.create_client(lusid_url, access_token)
     run(client, deployment)
 
 
 def load_vars(vars_file):
     if vars_file:
         host_vars = SimpleNamespace(**json.load(vars_file))
     else:
```

### Comparing `fbnconfig-0.0.40/fbnconfig/drive.py` & `fbnconfig-0.0.42/fbnconfig/drive.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig/identity.py` & `fbnconfig-0.0.42/fbnconfig/identity.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig/load_module.py` & `fbnconfig-0.0.42/fbnconfig/load_module.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig/log.py` & `fbnconfig-0.0.42/fbnconfig/log.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig/main.py` & `fbnconfig-0.0.42/fbnconfig/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 import os
 import functools
-from .deploy import load_vars, create_client
+from .deploy import load_vars
+from .http_client import create_client
 from . import deploy
 from . import log as deployment_log
 from httpx import RequestError, HTTPStatusError
 from json import dumps
 from .load_module import load_module
 
 help_footer = "environment defaults to $LUSID_ENV and token defaults to $FBN_ACCESS_TOKEN"
@@ -13,15 +14,16 @@
 
 def http_exception_handler(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except RequestError as exc:
-            msg = f"An error occurred while requesting {exc.request.url!r} before we got a response"
+            msg = f"An error occurred while requesting {exc.request.url!r}" \
+                  f"before we got a response - {exc}"
             raise click.ClickException(msg)
         except HTTPStatusError as exc:
             status = exc.response.status_code
             base_msg = " ".join([
                 f"The server responded with {exc.response.status_code}",
                 f"while requesting {exc.request.method} {exc.request.url!r}",
             ])
```

### Comparing `fbnconfig-0.0.40/fbnconfig/property.py` & `fbnconfig-0.0.42/fbnconfig/property.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig/resource_abc.py` & `fbnconfig-0.0.42/fbnconfig/resource_abc.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     def deps(self):
         return []
 
 
 class Resource(ABC):
     @abstractmethod
-    def read(self, client: httpx.Client, old_state: SimpleNamespace) -> None:
+    def read(self, client: httpx.Client, old_state: SimpleNamespace) -> None|Dict[str,Any]:
         pass
 
     @abstractmethod
     def create(self, client) -> Optional[Dict[str, Any]]:
         pass
 
     @abstractmethod
```

### Comparing `fbnconfig-0.0.40/fbnconfig/scheduler.py` & `fbnconfig-0.0.42/fbnconfig/scheduler.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/fbnconfig.md` & `fbnconfig-0.0.42/fbnconfig.md`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.40/pyproject.toml` & `fbnconfig-0.0.42/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fbnconfig"
-version = "0.0.40"
+version = "0.0.42"
 description = "fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment"
 authors = ["FINBOURNE Technology <engineering@finbourne.com>"]
 readme = "fbnconfig.md"
 
 [tool.poetry.scripts]
 fbnconfig = 'fbnconfig.main:cli'
```

### Comparing `fbnconfig-0.0.40/PKG-INFO` & `fbnconfig-0.0.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbnconfig
-Version: 0.0.40
+Version: 0.0.42
 Summary: fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment
 Author: FINBOURNE Technology
 Author-email: engineering@finbourne.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

