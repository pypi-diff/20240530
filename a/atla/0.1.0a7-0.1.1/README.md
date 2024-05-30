# Comparing `tmp/atla-0.1.0a7.tar.gz` & `tmp/atla-0.1.1.tar.gz`

## Comparing `atla-0.1.0a7.tar` & `atla-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/__init__.py
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_base_client.py
--rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_typing.py
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/lib/.keep
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/resources/__init__.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/resources/evaluate.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/types/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/types/evaluate_create_params.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 atla-0.1.0a7/src/atla/types/evaluation.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a7/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a7/LICENSE
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 atla-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_base_client.py
+-rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/lib/.keep
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/resources/__init__.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/resources/evaluate.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/types/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/types/evaluate_create_params.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 atla-0.1.1/src/atla/types/evaluation.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 atla-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10607 2020-02-02 00:00:00.000000 atla-0.1.1/PKG-INFO
```

### Comparing `atla-0.1.0a7/src/atla/__init__.py` & `atla-0.1.1/src/atla/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from . import types
 from ._types import NOT_GIVEN, NoneType, NotGiven, Transport, ProxiesTypes
 from ._utils import file_from_path
-from ._client import (
-    ENVIRONMENTS,
-    Atla,
-    Client,
-    Stream,
-    Timeout,
-    AsyncAtla,
-    Transport,
-    AsyncClient,
-    AsyncStream,
-    RequestOptions,
-)
+from ._client import Atla, Client, Stream, Timeout, AsyncAtla, Transport, AsyncClient, AsyncStream, RequestOptions
 from ._models import BaseModel
 from ._version import __title__, __version__
 from ._response import APIResponse as APIResponse, AsyncAPIResponse as AsyncAPIResponse
 from ._constants import DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES, DEFAULT_CONNECTION_LIMITS
 from ._exceptions import (
     APIError,
     AtlaError,
@@ -65,15 +54,14 @@
     "RequestOptions",
     "Client",
     "AsyncClient",
     "Stream",
     "AsyncStream",
     "Atla",
     "AsyncAtla",
-    "ENVIRONMENTS",
     "file_from_path",
     "BaseModel",
     "DEFAULT_TIMEOUT",
     "DEFAULT_MAX_RETRIES",
     "DEFAULT_CONNECTION_LIMITS",
     "DefaultHttpxClient",
     "DefaultAsyncHttpxClient",
```

### Comparing `atla-0.1.0a7/src/atla/_base_client.py` & `atla-0.1.1/src/atla/_base_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_client.py` & `atla-0.1.1/src/atla/_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import os
-from typing import Any, Dict, Union, Mapping, cast
-from typing_extensions import Self, Literal, override
+from typing import Any, Union, Mapping
+from typing_extensions import Self, override
 
 import httpx
 
 from . import resources, _exceptions
 from ._qs import Querystring
 from ._types import (
     NOT_GIVEN,
@@ -29,48 +29,39 @@
 from ._base_client import (
     DEFAULT_MAX_RETRIES,
     SyncAPIClient,
     AsyncAPIClient,
 )
 
 __all__ = [
-    "ENVIRONMENTS",
     "Timeout",
     "Transport",
     "ProxiesTypes",
     "RequestOptions",
     "resources",
     "Atla",
     "AsyncAtla",
     "Client",
     "AsyncClient",
 ]
 
-ENVIRONMENTS: Dict[str, str] = {
-    "production": "https://api.atla-ai.com",
-    "development": "https://api-dev.atla-ai.com",
-}
-
 
 class Atla(SyncAPIClient):
     evaluate: resources.EvaluateResource
     with_raw_response: AtlaWithRawResponse
     with_streaming_response: AtlaWithStreamedResponse
 
     # client options
     api_key: str
 
-    _environment: Literal["production", "development"] | NotGiven
-
     def __init__(
         self,
         *,
         api_key: str | None = None,
-        environment: Literal["production", "development"] | NotGiven = NOT_GIVEN,
-        base_url: str | httpx.URL | None | NotGiven = NOT_GIVEN,
+        base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
         # We provide a `DefaultHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
         # See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
@@ -93,39 +84,18 @@
             api_key = os.environ.get("ATLA_API_KEY")
         if api_key is None:
             raise AtlaError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the ATLA_API_KEY environment variable"
             )
         self.api_key = api_key
 
-        self._environment = environment
-
-        base_url_env = os.environ.get("ATLA_BASE_URL")
-        if is_given(base_url) and base_url is not None:
-            # cast required because mypy doesn't understand the type narrowing
-            base_url = cast("str | httpx.URL", base_url)  # pyright: ignore[reportUnnecessaryCast]
-        elif is_given(environment):
-            if base_url_env and base_url is not None:
-                raise ValueError(
-                    "Ambiguous URL; The `ATLA_BASE_URL` env var and the `environment` argument are given. If you want to use the environment, you must pass base_url=None",
-                )
-
-            try:
-                base_url = ENVIRONMENTS[environment]
-            except KeyError as exc:
-                raise ValueError(f"Unknown environment: {environment}") from exc
-        elif base_url_env is not None:
-            base_url = base_url_env
-        else:
-            self._environment = environment = "production"
-
-            try:
-                base_url = ENVIRONMENTS[environment]
-            except KeyError as exc:
-                raise ValueError(f"Unknown environment: {environment}") from exc
+        if base_url is None:
+            base_url = os.environ.get("ATLA_BASE_URL")
+        if base_url is None:
+            base_url = f"https://api.atla-ai.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
@@ -158,15 +128,14 @@
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
         api_key: str | None = None,
-        environment: Literal["production", "development"] | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.Client | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -194,15 +163,14 @@
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             api_key=api_key or self.api_key,
             base_url=base_url or self.base_url,
-            environment=environment or self._environment,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
         )
@@ -249,22 +217,19 @@
     evaluate: resources.AsyncEvaluateResource
     with_raw_response: AsyncAtlaWithRawResponse
     with_streaming_response: AsyncAtlaWithStreamedResponse
 
     # client options
     api_key: str
 
-    _environment: Literal["production", "development"] | NotGiven
-
     def __init__(
         self,
         *,
         api_key: str | None = None,
-        environment: Literal["production", "development"] | NotGiven = NOT_GIVEN,
-        base_url: str | httpx.URL | None | NotGiven = NOT_GIVEN,
+        base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
         # We provide a `DefaultAsyncHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
         # See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
@@ -287,39 +252,18 @@
             api_key = os.environ.get("ATLA_API_KEY")
         if api_key is None:
             raise AtlaError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the ATLA_API_KEY environment variable"
             )
         self.api_key = api_key
 
-        self._environment = environment
-
-        base_url_env = os.environ.get("ATLA_BASE_URL")
-        if is_given(base_url) and base_url is not None:
-            # cast required because mypy doesn't understand the type narrowing
-            base_url = cast("str | httpx.URL", base_url)  # pyright: ignore[reportUnnecessaryCast]
-        elif is_given(environment):
-            if base_url_env and base_url is not None:
-                raise ValueError(
-                    "Ambiguous URL; The `ATLA_BASE_URL` env var and the `environment` argument are given. If you want to use the environment, you must pass base_url=None",
-                )
-
-            try:
-                base_url = ENVIRONMENTS[environment]
-            except KeyError as exc:
-                raise ValueError(f"Unknown environment: {environment}") from exc
-        elif base_url_env is not None:
-            base_url = base_url_env
-        else:
-            self._environment = environment = "production"
-
-            try:
-                base_url = ENVIRONMENTS[environment]
-            except KeyError as exc:
-                raise ValueError(f"Unknown environment: {environment}") from exc
+        if base_url is None:
+            base_url = os.environ.get("ATLA_BASE_URL")
+        if base_url is None:
+            base_url = f"https://api.atla-ai.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
@@ -352,15 +296,14 @@
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
         api_key: str | None = None,
-        environment: Literal["production", "development"] | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.AsyncClient | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -388,15 +331,14 @@
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             api_key=api_key or self.api_key,
             base_url=base_url or self.base_url,
-            environment=environment or self._environment,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
         )
```

### Comparing `atla-0.1.0a7/src/atla/_compat.py` & `atla-0.1.1/src/atla/_compat.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_exceptions.py` & `atla-0.1.1/src/atla/_exceptions.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_files.py` & `atla-0.1.1/src/atla/_files.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_models.py` & `atla-0.1.1/src/atla/_models.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_qs.py` & `atla-0.1.1/src/atla/_qs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_resource.py` & `atla-0.1.1/src/atla/_resource.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_response.py` & `atla-0.1.1/src/atla/_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_streaming.py` & `atla-0.1.1/src/atla/_streaming.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_types.py` & `atla-0.1.1/src/atla/_types.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_utils/__init__.py` & `atla-0.1.1/src/atla/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_utils/_logs.py` & `atla-0.1.1/src/atla/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_utils/_proxy.py` & `atla-0.1.1/src/atla/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_utils/_sync.py` & `atla-0.1.1/src/atla/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_utils/_transform.py` & `atla-0.1.1/src/atla/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_utils/_typing.py` & `atla-0.1.1/src/atla/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/_utils/_utils.py` & `atla-0.1.1/src/atla/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/resources/__init__.py` & `atla-0.1.1/src/atla/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/resources/evaluate.py` & `atla-0.1.1/src/atla/resources/evaluate.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/types/evaluate_create_params.py` & `atla-0.1.1/src/atla/types/evaluate_create_params.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/src/atla/types/evaluation.py` & `atla-0.1.1/src/atla/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/LICENSE` & `atla-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a7/pyproject.toml` & `atla-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atla"
-version = "0.1.0-alpha.7"
+version = "0.1.1"
 description = "The official Python library for the atla API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Atla", email = "support@atla.com" },
 ]
 dependencies = [
```

### Comparing `atla-0.1.0a7/PKG-INFO` & `atla-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atla
-Version: 0.1.0a7
+Version: 0.1.1
 Summary: The official Python library for the atla API
 Project-URL: Homepage, https://github.com/atla-ai/atla-sdk-python
 Project-URL: Repository, https://github.com/atla-ai/atla-sdk-python
 Author-email: Atla <support@atla.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -38,47 +38,43 @@
 
 The Atla Python library provides convenient access to the Atla REST API from any Python 3.7+
 application. The library includes type definitions for all request params and response fields,
 and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
 
 ## Documentation
 
-The REST API documentation can be found [on docs.atla.com](https://docs.atla.com). The full API of this library can be found in [api.md](https://github.com/atla-ai/atla-sdk-python/tree/main/api.md).
+The REST API documentation can be found [on docs.atla-ai.com](https://docs.atla-ai.com). The full API of this library can be found in [api.md](https://github.com/atla-ai/atla-sdk-python/tree/main/api.md).
 
 ## Installation
 
 ```sh
-# install from the production repo
-pip install git+ssh://git@github.com/atla-ai/atla-sdk-python.git
+# install from PyPI
+pip install atla
 ```
 
-> [!NOTE]
-> Once this package is [published to PyPI](https://app.stainlessapi.com/docs/guides/publish), this will become: `pip install --pre atla`
-
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/atla-ai/atla-sdk-python/tree/main/api.md).
 
 ```python
 import os
 from atla import Atla
 
 client = Atla(
     # This is the default and can be omitted
     api_key=os.environ.get("ATLA_API_KEY"),
-    # defaults to "production".
-    environment="development",
 )
 
-score = client.evaluate.create(
-    input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
+eval = client.evaluate.create(
+    input="Is it legal to monitor employee emails under European privacy laws?",
     metrics=["precision", "recall"],
-    response="If you have any questions about my rate, please let me know.",
+    response="Monitoring employee emails is permissible under European privacy laws like GDPR, provided there's a legitimate purpose.",
+    context="European privacy laws, including GDPR, allow for the monitoring of employee emails under strict conditions. The employer must demonstrate that the monitoring is necessary for a legitimate purpose, such as protecting company assets or compliance with legal obligations. Employees must be informed about the monitoring in advance, and the privacy impact should be assessed to minimize intrusion.",
 )
-print(score.evaluations.recall.score)
+print(eval.evaluations)
 ```
 
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `ATLA_API_KEY="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
@@ -90,26 +86,25 @@
 import os
 import asyncio
 from atla import AsyncAtla
 
 client = AsyncAtla(
     # This is the default and can be omitted
     api_key=os.environ.get("ATLA_API_KEY"),
-    # defaults to "production".
-    environment="development",
 )
 
 
 async def main() -> None:
-    score = await client.evaluate.create(
-        input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
+    eval = await client.evaluate.create(
+        input="Is it legal to monitor employee emails under European privacy laws?",
         metrics=["precision", "recall"],
-        response="If you have any questions about my rate, please let me know.",
+        response="Monitoring employee emails is permissible under European privacy laws like GDPR, provided there's a legitimate purpose.",
+        context="European privacy laws, including GDPR, allow for the monitoring of employee emails under strict conditions. The employer must demonstrate that the monitoring is necessary for a legitimate purpose, such as protecting company assets or compliance with legal obligations. Employees must be informed about the monitoring in advance, and the privacy impact should be assessed to minimize intrusion.",
     )
-    print(score.evaluations.recall.score)
+    print(eval.evaluations)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -135,17 +130,18 @@
 import atla
 from atla import Atla
 
 client = Atla()
 
 try:
     client.evaluate.create(
-        input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
+        input="Is it legal to monitor employee emails under European privacy laws?",
         metrics=["precision", "recall"],
-        response="If you have any questions about my rate, please let me know.",
+        response="Monitoring employee emails is permissible under European privacy laws like GDPR, provided there's a legitimate purpose.",
+        context="European privacy laws, including GDPR, allow for the monitoring of employee emails under strict conditions. The employer must demonstrate that the monitoring is necessary for a legitimate purpose, such as protecting company assets or compliance with legal obligations. Employees must be informed about the monitoring in advance, and the privacy impact should be assessed to minimize intrusion.",
     )
 except atla.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except atla.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except atla.APIStatusError as e:
@@ -182,17 +178,18 @@
 client = Atla(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).evaluate.create(
-    input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
+    input="Is it legal to monitor employee emails under European privacy laws?",
     metrics=["precision", "recall"],
-    response="If you have any questions about my rate, please let me know.",
+    response="Monitoring employee emails is permissible under European privacy laws like GDPR, provided there's a legitimate purpose.",
+    context="European privacy laws, including GDPR, allow for the monitoring of employee emails under strict conditions. The employer must demonstrate that the monitoring is necessary for a legitimate purpose, such as protecting company assets or compliance with legal obligations. Employees must be informed about the monitoring in advance, and the privacy impact should be assessed to minimize intrusion.",
 )
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
@@ -209,17 +206,18 @@
 # More granular control:
 client = Atla(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
 client.with_options(timeout=5.0).evaluate.create(
-    input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
+    input="Is it legal to monitor employee emails under European privacy laws?",
     metrics=["precision", "recall"],
-    response="If you have any questions about my rate, please let me know.",
+    response="Monitoring employee emails is permissible under European privacy laws like GDPR, provided there's a legitimate purpose.",
+    context="European privacy laws, including GDPR, allow for the monitoring of employee emails under strict conditions. The employer must demonstrate that the monitoring is necessary for a legitimate purpose, such as protecting company assets or compliance with legal obligations. Employees must be informed about the monitoring in advance, and the privacy impact should be assessed to minimize intrusion.",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/atla-ai/atla-sdk-python/tree/main/#retries).
```

