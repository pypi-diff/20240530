# Comparing `tmp/fdk_asgi-0.6.0.tar.gz` & `tmp/fdk_asgi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_asgi-0.6.0.tar", max compression
+gzip compressed data, was "fdk_asgi-0.7.0.tar", max compression
```

## Comparing `fdk_asgi-0.6.0.tar` & `fdk_asgi-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/LICENSE
--rw-r--r--   0        0        0     7648 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/README.md
--rw-r--r--   0        0        0     2562 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/src/fdk_asgi/__init__.py
--rw-r--r--   0        0        0     5300 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/app.py
--rw-r--r--   0        0        0     5955 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/cli.py
--rw-r--r--   0        0        0      880 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/exceptions.py
--rw-r--r--   0        0        0      621 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/types.py
--rw-r--r--   0        0        0     2227 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/utils.py
--rw-r--r--   0        0        0     8478 1970-01-01 00:00:00.000000 fdk_asgi-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7648 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/README.md
+-rw-r--r--   0        0        0     2710 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/__init__.py
+-rw-r--r--   0        0        0     5547 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/app.py
+-rw-r--r--   0        0        0     6099 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/cli.py
+-rw-r--r--   0        0        0      880 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/py.typed
+-rw-r--r--   0        0        0      621 2024-05-30 12:27:13.308253 fdk_asgi-0.7.0/src/fdk_asgi/types.py
+-rw-r--r--   0        0        0     2262 2024-05-30 12:27:13.308253 fdk_asgi-0.7.0/src/fdk_asgi/utils.py
+-rw-r--r--   0        0        0     8554 1970-01-01 00:00:00.000000 fdk_asgi-0.7.0/PKG-INFO
```

### Comparing `fdk_asgi-0.6.0/LICENSE` & `fdk_asgi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.6.0/README.md` & `fdk_asgi-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.6.0/pyproject.toml` & `fdk_asgi-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "fdk-asgi"
 requires-python = ">=3.8"
 
 [tool.poetry]
 name = "fdk-asgi"
-version = "0.6.0"
+version = "0.7.0"
 description = "An alternative FDK to easily run any ASGI application on OCI Functions behind an API Gateway."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "fdk_asgi", from = "src"}]
 
 [tool.poetry.scripts]
 fdk-asgi-serve = 'fdk_asgi.cli:app'
@@ -16,14 +16,15 @@
 [tool.poetry.dependencies]
 python = ">=3.8"
 asgiref = "^3.7.2"
 httptools = "^0.6.0"
 typer = { version = "^0.9.0", optional = true }
 uvicorn = { version = "^0.25", optional = true }
 strenum = "^0.4.15"
+typing-extensions = {version = "^4.12.0", python = "<3.9"}
 
 [tool.poetry.extras]
 cli = ["typer", "uvicorn"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 httpx = "^0.26"
@@ -39,17 +40,21 @@
 uvicorn = "*"
 mypy = "^1.10.0"
 
 [tool.coverage.run]
 source = ["src", "tests"]
 
 [tool.mypy]
-files = "src"
+files = ["src", "tests"]
 strict = true
 
+[[tool.mypy.overrides]]
+module = ["httptools"]
+ignore_missing_imports = true
+
 [tool.pytest.ini_options]
 addopts = [
     "--cov",
     "--cov-report=term:skip-covered",
     "--import-mode=importlib",
     "--strict-config",
     "--strict-markers",
```

### Comparing `fdk_asgi-0.6.0/src/fdk_asgi/app.py` & `fdk_asgi-0.7.0/src/fdk_asgi/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from __future__ import annotations
 
 import logging
 from http import HTTPStatus
 from importlib.metadata import version
 
-from asgiref.typing import HTTPResponseStartEvent, HTTPScope
+from asgiref.typing import (
+    ASGI3Application,
+    ASGIReceiveCallable,
+    ASGISendCallable,
+    ASGISendEvent,
+    HTTPResponseBodyEvent,
+    HTTPResponseStartEvent,
+    HTTPScope,
+    Scope,
+)
 from httptools import parse_url
 
 from fdk_asgi.exceptions import (
     FnMiddlewareError,
     MethodNotAllowedError,
     MissingMethodError,
     MissingUrlError,
     PathNotFoundError,
 )
-from fdk_asgi.types import ASGIApp, Message, Receive, Scope, Send
 from fdk_asgi.utils import get_client_addr, get_path_with_query_string
 
 FN_FDK_VERSION_HEADER = (
     b"fn-fdk-version",
     f"fdk-asgi/{version(__package__)}".encode(),
 )
 
@@ -36,44 +44,47 @@
 logger_access = logging.getLogger(f"{__package__}.access")
 
 
 class FnMiddleware:
     """A pure ASGI middleware, wrapping a regular ASGI application
     and translating Fn <-> REST."""
 
-    def __init__(self, app: ASGIApp, prefix: str = ""):
+    def __init__(self, app: ASGI3Application, prefix: str = ""):
         self.app = app
         self.prefix = prefix
 
-    async def __call__(self, scope: Scope, receive: Receive, send: Send):
+    async def __call__(
+        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
+    ) -> None:
         # leave all but HTTP connection scopes untouched
         # note that websockets are not supported by fn
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
-        scope: HTTPScope
 
         try:
             mapped_scope = self._map_http_scope(scope)
         except FnMiddlewareError as exception:
             logger.critical(exception)
-            await send(
-                {
-                    "type": "http.response.start",
-                    "status": exception.code,
-                    "headers": [
-                        [b"content-type", b"text/plain"],
-                    ],
-                }
-            )
-            await send(
-                {
-                    "type": "http.response.body",
-                    "body": str(exception).encode(),
-                }
-            )
+            start_message: HTTPResponseStartEvent
+            start_message = {
+                "type": "http.response.start",
+                "status": exception.code,
+                "headers": [
+                    (b"content-type", b"text/plain"),
+                ],
+                "trailers": False,
+            }
+            await send(start_message)
+            body_message: HTTPResponseBodyEvent
+            body_message = {
+                "type": "http.response.body",
+                "body": str(exception).encode(),
+                "more_body": False,
+            }
+            await send(body_message)
             return
         await self.app(mapped_scope, receive, self._wrap_send(send, scope))
 
     def _map_http_scope(self, scope: HTTPScope) -> HTTPScope:
         """Transforms headers etc. sent by Fn/API Gateway
         so that ASGI apps can understand them."""
 
@@ -116,21 +127,19 @@
         # scope has precedence over environment variable
         scope["root_path"] = self.prefix
         scope["headers"] = http_headers
 
         return scope
 
     @staticmethod
-    def _wrap_send(send: Send, scope: HTTPScope) -> Send:
-        async def wrapped_send(message: Message):
+    def _wrap_send(send: ASGISendCallable, scope: HTTPScope) -> ASGISendCallable:
+        async def wrapped_send(message: ASGISendEvent) -> None:
             # only process messages of type=http.response.start,
             # leave message of other types untouched
             if message["type"] == "http.response.start":
-                message: HTTPResponseStartEvent
-
                 new_headers = [
                     (key, value)
                     if key.lower() == b"content-type"
                     else (FN_HTTP_H_ + key, value)
                     for key, value in message["headers"]
                 ]
                 new_headers.append((FN_HTTP_STATUS, str(message["status"]).encode()))
```

### Comparing `fdk_asgi-0.6.0/src/fdk_asgi/cli.py` & `fdk_asgi-0.7.0/src/fdk_asgi/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import logging
+import os
+import sys
 from pathlib import Path
-from typing import Annotated, Optional
+from typing import Optional
+
+if sys.version_info >= (3, 9):
+    from typing import Annotated
+else:
+    from typing_extensions import Annotated
 
 try:
     import typer
 except ModuleNotFoundError as exception:  # pragma: no cover
     msg = f"Using {__name__} requires the typer package to be installed."
     raise RuntimeError(msg) from exception
 
@@ -15,15 +22,15 @@
     msg = f"Using {__name__} requires the uvicorn package to be installed."
     raise RuntimeError(msg) from exception
 
 from fdk_asgi.app import FnMiddleware
 from fdk_asgi.types import HTTPProtocolType, LifespanType, LoopSetupType
 
 UDS_PREFIX = "unix:"
-DEFAULT_LOGGING_CONFIG: dict[str, any] = {
+DEFAULT_LOGGING_CONFIG = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         "default": {
             "()": "uvicorn.logging.DefaultFormatter",
             "fmt": "%(levelprefix)s %(message)s",
             "use_colors": None,
@@ -126,15 +133,15 @@
             help="Treat APP as an application factory, "
             "i.e. a () -> <ASGI app> callable.",
         ),
     ] = False,
     h11_max_incomplete_event_size: Annotated[
         Optional[int], typer.Option(envvar="FDK_ASGI_H11_MAX_INCOMPLETE_EVENT_SIZE")
     ] = None,
-):
+) -> None:
     asgi_app = import_from_string(app_uri)
     if factory:
         asgi_app = asgi_app()
     fn_asgi_app = FnMiddleware(asgi_app, prefix)
 
     socket = Path(uds[len(UDS_PREFIX) :]) if uds.startswith(UDS_PREFIX) else Path(uds)
     # os.umask(0o666)  # todo: check if this is necessary
@@ -143,15 +150,17 @@
         app=fn_asgi_app,
         uds=str(socket),
         loop=loop.value,
         http=http.value,
         ws="none",
         lifespan=lifespan.value,
         env_file=env_file,
-        log_config=DEFAULT_LOGGING_CONFIG if log_config is None else log_config,
+        log_config=DEFAULT_LOGGING_CONFIG
+        if log_config is None
+        else os.fspath(log_config),
         log_level=log_level,
         access_log=False,
         # use_colors: Optional[bool] = None,
         interface="asgi3",
         workers=1,
         proxy_headers=proxy_headers,  # todo: check if Functions supports this header
         server_header=server_header,  # todo: check if Functions supports this header
```

### Comparing `fdk_asgi-0.6.0/src/fdk_asgi/exceptions.py` & `fdk_asgi-0.7.0/src/fdk_asgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.6.0/src/fdk_asgi/types.py` & `fdk_asgi-0.7.0/src/fdk_asgi/types.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.6.0/src/fdk_asgi/utils.py` & `fdk_asgi-0.7.0/src/fdk_asgi/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 def get_client_addr(scope: WWWScope) -> str:
     client = scope.get("client")
     if not client:
         return ""
-    # TestClient produces a list instead of a tuple
-    # convert to tuple as a workaround
-    return "%s:%d" % tuple(client)
+    # asgiref types scope["client"] as a Tuple[str, int],
+    # but the spec types it as an Iterable[Unicode string, int]
+    return "{!s}:{:d}".format(*client)
 
 
 def get_path_with_query_string(scope: WWWScope) -> str:
     path_with_query_string = urllib.parse.quote(scope["path"])
     if scope["query_string"]:
         path_with_query_string = "{}?{}".format(
             path_with_query_string, scope["query_string"].decode("ascii")
```

### Comparing `fdk_asgi-0.6.0/PKG-INFO` & `fdk_asgi-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdk-asgi
-Version: 0.6.0
+Version: 0.7.0
 Summary: An alternative FDK to easily run any ASGI application on OCI Functions behind an API Gateway.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: httptools (>=0.6.0,<0.7.0)
 Requires-Dist: strenum (>=0.4.15,<0.5.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0) ; extra == "cli"
+Requires-Dist: typing-extensions (>=4.12.0,<5.0.0) ; python_version < "3.9"
 Requires-Dist: uvicorn (>=0.25,<0.26) ; extra == "cli"
 Description-Content-Type: text/markdown
 
 # fdk-asgi
 
 [![pipeline status](https://github.com/bjoern-reetz/fdk-asgi/actions/workflows/publish.yml/badge.svg?main)](https://github.com/bjoern-reetz/fdk-asgi/actions/workflows/publish.yml)
 [![latest package version](https://img.shields.io/pypi/v/fdk-asgi)](https://pypi.org/project/fdk-asgi/)
```

