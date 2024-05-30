# Comparing `tmp/lima_api-0.0.1.tar.gz` & `tmp/lima_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lima_api-0.0.1.tar", last modified: Thu May 23 11:43:44 2024, max compression
+gzip compressed data, was "lima_api-0.0.2.tar", last modified: Thu May 30 08:55:22 2024, max compression
```

## Comparing `lima_api-0.0.1.tar` & `lima_api-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.638361 lima_api-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.630361 lima_api-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.634361 lima_api-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 11:43:40.000000 lima_api-0.0.1/.github/ISSUE_TEMPLATE/bug-report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-23 11:43:40.000000 lima_api-0.0.1/.github/ISSUE_TEMPLATE/feature-request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.634361 lima_api-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-23 11:43:40.000000 lima_api-0.0.1/.github/workflows/code_testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-23 11:43:40.000000 lima_api-0.0.1/.github/workflows/publish_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-23 11:43:40.000000 lima_api-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-23 11:43:40.000000 lima_api-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 11:43:44.638361 lima_api-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-23 11:43:40.000000 lima_api-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-23 11:43:40.000000 lima_api-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:43:44.638361 lima_api-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.630361 lima_api-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.634361 lima_api-0.0.1/src/lima_api/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-23 11:43:40.000000 lima_api-0.0.1/src/lima_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 11:43:40.000000 lima_api-0.0.1/src/lima_api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12665 2024-05-23 11:43:40.000000 lima_api-0.0.1/src/lima_api/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-23 11:43:40.000000 lima_api-0.0.1/src/lima_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-23 11:43:40.000000 lima_api-0.0.1/src/lima_api/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-23 11:43:40.000000 lima_api-0.0.1/src/lima_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.638361 lima_api-0.0.1/src/lima_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 11:43:44.000000 lima_api-0.0.1/src/lima_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 11:43:44.000000 lima_api-0.0.1/src/lima_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:43:44.000000 lima_api-0.0.1/src/lima_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 11:43:44.000000 lima_api-0.0.1/src/lima_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 11:43:44.000000 lima_api-0.0.1/src/lima_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:43:44.634361 lima_api-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-05-23 11:43:40.000000 lima_api-0.0.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.772181 lima_api-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.764181 lima_api-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.764181 lima_api-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-30 08:55:18.000000 lima_api-0.0.2/.github/ISSUE_TEMPLATE/bug-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-30 08:55:18.000000 lima_api-0.0.2/.github/ISSUE_TEMPLATE/feature-request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.768180 lima_api-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-30 08:55:18.000000 lima_api-0.0.2/.github/workflows/code_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-30 08:55:18.000000 lima_api-0.0.2/.github/workflows/publish_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-30 08:55:18.000000 lima_api-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-30 08:55:18.000000 lima_api-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-30 08:55:22.768180 lima_api-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 08:55:18.000000 lima_api-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-30 08:55:18.000000 lima_api-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:55:22.772181 lima_api-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.764181 lima_api-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.768180 lima_api-0.0.2/src/lima_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-30 08:55:18.000000 lima_api-0.0.2/src/lima_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-30 08:55:18.000000 lima_api-0.0.2/src/lima_api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-30 08:55:18.000000 lima_api-0.0.2/src/lima_api/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-30 08:55:18.000000 lima_api-0.0.2/src/lima_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-30 08:55:18.000000 lima_api-0.0.2/src/lima_api/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-30 08:55:18.000000 lima_api-0.0.2/src/lima_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.768180 lima_api-0.0.2/src/lima_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-30 08:55:22.000000 lima_api-0.0.2/src/lima_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-30 08:55:22.000000 lima_api-0.0.2/src/lima_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:55:22.000000 lima_api-0.0.2/src/lima_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 08:55:22.000000 lima_api-0.0.2/src/lima_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 08:55:22.000000 lima_api-0.0.2/src/lima_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:55:22.768180 lima_api-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-30 08:55:18.000000 lima_api-0.0.2/tests/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-05-30 08:55:18.000000 lima_api-0.0.2/tests/test_api.py
```

### Comparing `lima_api-0.0.1/.github/ISSUE_TEMPLATE/bug-report.yaml` & `lima_api-0.0.2/.github/ISSUE_TEMPLATE/bug-report.yaml`

 * *Files identical despite different names*

### Comparing `lima_api-0.0.1/.github/ISSUE_TEMPLATE/feature-request.yaml` & `lima_api-0.0.2/.github/ISSUE_TEMPLATE/feature-request.yaml`

 * *Files identical despite different names*

### Comparing `lima_api-0.0.1/.github/workflows/code_testing.yml` & `lima_api-0.0.2/.github/workflows/code_testing.yml`

 * *Files identical despite different names*

### Comparing `lima_api-0.0.1/.github/workflows/publish_package.yml` & `lima_api-0.0.2/.github/workflows/publish_package.yml`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
+      uses: sigstore/gh-action-sigstore-python@v2.1.4
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Upload artifact signatures to GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
```

### Comparing `lima_api-0.0.1/.gitignore` & `lima_api-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lima_api-0.0.1/LICENSE` & `lima_api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lima_api-0.0.1/PKG-INFO` & `lima_api-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lima-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lima-API is sync and async library that allows implements Rest APIs libs with python typing.
 Author-email: Cesar Gonzalez <cgonzalez@paradigmadigital.com>, Victor Torre <vatorre@paradigmadigital.com>
 License: MIT License
         
         Copyright (c) 2023 Paradigma Digital S.L.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lima_api-0.0.1/pyproject.toml` & `lima_api-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ]
 all = [
     "lima_api[test, pydantic2]",
 ]
 
 [tool.ruff]
 line-length = 120
-include = ["pyproject.toml", "src/**/*.py"]
+include = ["pyproject.toml", "src/**/*.py", "tests/**/*.py"]
 
 [tool.ruff.lint]
 select = [
     "E", # pycodestyle errors
     "W", # pycodestyle warnings
     "F", # pyflakes
     "I", # isort
@@ -68,9 +68,12 @@
     "UP", # pyupgrade
     "ASYNC", # flake8-async
     "S", # flake8-bandit
     "DTZ", # flake8-datetimez
     "SIM", # flake8-simplify
 ]
 ignore = [
-
+    "B008",  # do not perform function calls in argument defaults
 ]
+
+[tool.ruff.lint.extend-per-file-ignores]
+"tests/**/*.py" = ["S101", "S106", "UP035", "UP006"]
```

### Comparing `lima_api-0.0.1/src/lima_api/core.py` & `lima_api-0.0.2/src/lima_api/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,61 +21,86 @@
 DEFAULT_HTTP_RETRIES = settings.lima_default_http_retries
 DEFAULT_HTTP_TIMEOUT = settings.lima_default_http_timeout
 DEFAULT_RESPONSE_CODE = settings.lima_default_response_code
 DEFAULT_UNDEFINED_VALUES: tuple[Any, ...] = (None, "")
 
 
 class LimaApiBase:
+    headers: dict[str, str]
+    response_mapping: dict[int, type[LimaException]]
+    client_kwargs: dict
+    retries: int = DEFAULT_HTTP_RETRIES
+    timeout: int = DEFAULT_HTTP_TIMEOUT
+    default_response_code: int = DEFAULT_RESPONSE_CODE
+    undefined_values: tuple[Any, ...] = DEFAULT_UNDEFINED_VALUES
+    default_exception: type[LimaException] = LimaException
+
+    def __new__(cls, *args, **kwargs):
+        new_class = super().__new__(cls)
+        if not hasattr(new_class, "headers"):
+            new_class.headers = {}
+        if not hasattr(new_class, "response_mapping"):
+            new_class.response_mapping = {}
+        if not hasattr(new_class, "client_kwargs"):
+            new_class.client_kwargs = {}
+        return new_class
+
     def __init__(
         self,
         base_url: str,
-        retries: int = DEFAULT_HTTP_RETRIES,
-        timeout: int = DEFAULT_HTTP_TIMEOUT,
+        *,
+        retries: Optional[int] = None,
+        timeout: Optional[int] = None,
         headers: Optional[dict[str, str]] = None,
-        default_response_code: int = DEFAULT_RESPONSE_CODE,
+        default_response_code: Optional[int] = None,
         response_mapping: Optional[dict[int, type[LimaException]]] = None,
-        undefined_values: tuple[Any, ...] = DEFAULT_UNDEFINED_VALUES,
-        default_exception: type[LimaException] = LimaException,
+        undefined_values: tuple[Any, ...] = None,
+        default_exception: Optional[type[LimaException]] = None,
         client_kwargs: Optional[dict] = None,
     ):
         self.base_url: str = base_url
 
-        self.retries = retries
-        self.timeout = timeout
-        self.default_response_code = default_response_code
-        self.default_exception = default_exception or LimaException
-        if response_mapping is None:
-            response_mapping = {}
-        self.response_mapping: dict[int, type[LimaException]] = response_mapping
-        self.undefined_values = undefined_values
-        self.headers = headers
+        if retries is not None:
+            self.retries = retries
+        if timeout is not None:
+            self.timeout = timeout
+        if default_response_code is not None:
+            self.default_response_code = default_response_code
+        if default_exception is not None:
+            self.default_exception = default_exception
+        if undefined_values is not None:
+            self.undefined_values = undefined_values
+
+        self.response_mapping.update(response_mapping or {})
+        self.headers.update(headers or {})
         self.transport: Optional[Union[SyncOpenTelemetryTransport, AsyncOpenTelemetryTransport]] = None
         self.client: Optional[Union[httpx.Client, httpx.AsyncClient]] = None
-        self.client_kwargs = client_kwargs or {}
+        self.client_kwargs.update(client_kwargs or {})
 
     def _create_request(
         self,
+        *,
         sync: bool,
         method: str,
         path: str,
         path_params_mapping: dict,
         kwargs: dict,
         body_mapping: Optional[dict] = None,
         query_params_mapping: list[dict] = None,
         undefined_values: Optional[tuple[Any, ...]] = None,
         headers: Optional[dict[str, str]] = None,
         timeout: Optional[int] = None,
     ) -> httpx.Request:
         if self.client is None:
-            raise LimaException("Cliente no inicializado")
+            raise LimaException("uninitialized client")
 
         if sync and inspect.iscoroutinefunction(self.client.send):
-            raise LimaException("Función síncrona en cliente asíncrono")
+            raise LimaException("sync function in async client")
         elif not sync and not inspect.iscoroutinefunction(self.client.send):
-            raise LimaException("Función asíncrona en cliente síncrono")
+            raise LimaException("async function in sync client")
 
         params = get_request_params(
             query_params_mapping,
             kwargs,
             undefined_values if undefined_values is not None else self.undefined_values,
         )
 
@@ -108,14 +133,15 @@
             timeout=timeout if timeout is not None else self.timeout,
             **body_kwarg,
         )
         return api_request
 
     def _create_response(
         self,
+        *,
         api_response: httpx.Response,
         return_class: Any,
         response_mapping: Optional[dict[int, type[LimaException]]] = None,
         default_response_code: Optional[int] = None,
         default_exception: Optional[type[LimaException]] = None,
     ):
         mapping = self.response_mapping
@@ -140,38 +166,17 @@
                 status_code=api_response.status_code,
                 content=api_response.content,
             )
         return response
 
 
 class LimaApi(LimaApiBase):
-    def __init__(
-        self,
-        base_url: str,
-        retries: int = DEFAULT_HTTP_RETRIES,
-        timeout: int = DEFAULT_HTTP_TIMEOUT,
-        headers: Optional[dict[str, str]] = None,
-        default_response_code: int = DEFAULT_RESPONSE_CODE,
-        response_mapping: Optional[dict[int, type[LimaException]]] = None,
-        undefined_values: tuple[Any, ...] = DEFAULT_UNDEFINED_VALUES,
-        default_exception: type[LimaException] = LimaException,
-        client_kwargs: Optional[dict] = None,
-    ):
-        super().__init__(
-            base_url=base_url,
-            retries=retries,
-            timeout=timeout,
-            headers=headers,
-            default_response_code=default_response_code,
-            response_mapping=response_mapping,
-            undefined_values=undefined_values,
-            default_exception=default_exception,
-            client_kwargs=client_kwargs,
-        )
-        transport = httpx.AsyncHTTPTransport(retries=retries)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        transport = httpx.AsyncHTTPTransport(retries=self.retries)
         self.transport: AsyncOpenTelemetryTransport = AsyncOpenTelemetryTransport(transport)
         self.client: Optional[httpx.AsyncClient] = None
 
     async def start_client(self) -> None:
         client_kwargs = self.client_kwargs.copy()
         client_kwargs["timeout"] = self.timeout
         client_kwargs["transport"] = self.transport
@@ -186,38 +191,17 @@
         return self
 
     async def __aexit__(self, exc_type, exc, tb) -> None:
         await self.stop_client()
 
 
 class SyncLimaApi(LimaApiBase):
-    def __init__(
-        self,
-        base_url: str,
-        retries: int = DEFAULT_HTTP_RETRIES,
-        timeout: int = DEFAULT_HTTP_TIMEOUT,
-        headers: Optional[dict[str, str]] = None,
-        default_response_code: int = DEFAULT_RESPONSE_CODE,
-        response_mapping: Optional[dict[int, type[LimaException]]] = None,
-        undefined_values: tuple[Any, ...] = DEFAULT_UNDEFINED_VALUES,
-        default_exception: type[LimaException] = LimaException,
-        client_kwargs: Optional[dict] = None,
-    ):
-        super().__init__(
-            base_url=base_url,
-            retries=retries,
-            timeout=timeout,
-            headers=headers,
-            default_response_code=default_response_code,
-            response_mapping=response_mapping,
-            undefined_values=undefined_values,
-            default_exception=default_exception,
-            client_kwargs=client_kwargs,
-        )
-        transport = httpx.HTTPTransport(retries=retries)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        transport = httpx.HTTPTransport(retries=self.retries)
         self.transport: SyncOpenTelemetryTransport = SyncOpenTelemetryTransport(transport)
         self.client: Optional[httpx.Client] = None
 
     def start_client(self) -> None:
         client_kwargs = self.client_kwargs.copy()
         client_kwargs["timeout"] = self.timeout
         client_kwargs["transport"] = self.transport
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lima_api-0.0.1/src/lima_api/parameters.py` & `lima_api-0.0.2/src/lima_api/parameters.py`

 * *Files identical despite different names*

### Comparing `lima_api-0.0.1/src/lima_api/utils.py` & `lima_api-0.0.2/src/lima_api/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return parse_raw_as(parse_class, data)
 
 
 def get_request_params(query_params_mapping: list[dict], kwargs: dict, undefined_values: tuple[Any, ...]) -> dict:
     params = {}
     for param_map in query_params_mapping:
         if param_map["kwargs_name"] not in kwargs and "default" not in param_map:
-            raise TypeError(f"Falta el argumento obligatorio <{param_map['kwargs_name']}>")
+            raise TypeError(f"required argument missing <{param_map['kwargs_name']}>")
         argument_value = (
             kwargs[param_map["kwargs_name"]] if param_map["kwargs_name"] in kwargs else param_map["default"]
         )
         if argument_value in undefined_values:
             continue
 
         model_dump_mode = param_map.get("model_dump_mode", None)
@@ -79,25 +79,24 @@
     path_params = BRACKET_REGEX.findall(path)
 
     query_params_mapping: list[dict] = []
     path_params_mapping: list[dict] = []
     body_mapping: Optional[dict] = None
 
     for param_name, parameter in ((k, v) for k, v in parameters.items() if k not in ["self", "args", "kwargs"]):
+        attrs = get_args(parameter.annotation)
         param_map = {
             "api_name": (
                 parameter.default.alias
                 if isinstance(parameter.default, FieldInfo) and parameter.default.alias is not None
                 else param_name
             ),
             "kwargs_name": param_name,
-            "class": (
-                parameter.annotation if inspect.isclass(parameter.annotation) else get_args(parameter.annotation)[0]
-            ),
-            "wrap": (None if inspect.isclass(parameter.annotation) else parameter.annotation),
+            "class": (attrs[0] if attrs else parameter.annotation),
+            "wrap": (parameter.annotation if attrs else None),
         }
 
         # Default values
         if isinstance(parameter.default, FieldInfo) and parameter.default.default is not PydanticUndefined:
             param_map["default"] = parameter.default.default
         elif not isinstance(parameter.default, FieldInfo) and parameter.default != parameter.empty:
             param_map["default"] = parameter.default
@@ -121,22 +120,22 @@
 
         if location == Location.QUERY:
             query_params_mapping.append(param_map)
         elif location == Location.PATH:
             path_params_mapping.append(param_map)
         elif location == Location.BODY:
             if body_mapping:
-                raise ValueError("Too many body params")
+                raise ValueError("too many body params")
             body_mapping = param_map
         else:
-            raise ValueError("Invalid location")
+            raise ValueError("invalid location")
 
     missing_path_params = set(path_params) - {p["api_name"] for p in path_params_mapping}
     if missing_path_params:
-        raise LimaException(f"Falta definir el/los parametros de path: <{','.join(missing_path_params)}>")
+        raise LimaException(f"path parameters need to be defined: <{','.join(missing_path_params)}>")
 
     return query_params_mapping, path_params_mapping, body_mapping
 
 
 def get_body(body_mapping: Optional[dict], kwargs: dict):
     if body_mapping:
         if issubclass(body_mapping["class"], BaseModel):
```

### Comparing `lima_api-0.0.1/src/lima_api.egg-info/PKG-INFO` & `lima_api-0.0.2/src/lima_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lima-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lima-API is sync and async library that allows implements Rest APIs libs with python typing.
 Author-email: Cesar Gonzalez <cgonzalez@paradigmadigital.com>, Victor Torre <vatorre@paradigmadigital.com>
 License: MIT License
         
         Copyright (c) 2023 Paradigma Digital S.L.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lima_api-0.0.1/src/lima_api.egg-info/SOURCES.txt` & `lima_api-0.0.2/src/lima_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 .github/workflows/publish_package.yml
 src/lima_api/__init__.py
 src/lima_api/config.py
 src/lima_api/core.py
 src/lima_api/exceptions.py
 src/lima_api/parameters.py
 src/lima_api/utils.py
+tests/client.py
 tests/test_api.py
```

