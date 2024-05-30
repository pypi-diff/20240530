# Comparing `tmp/openai_responses-0.4.1.tar.gz` & `tmp/openai_responses-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.4.1.tar", max compression
+gzip compressed data, was "openai_responses-0.5.0.tar", max compression
```

## Comparing `openai_responses-0.4.1.tar` & `openai_responses-0.5.0.tar`

### file list

```diff
@@ -1,49 +1,54 @@
--rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.4.1/LICENSE
--rw-r--r--   0        0        0     3516 2024-05-23 13:46:44.586757 openai_responses-0.4.1/README.md
--rw-r--r--   0        0        0     1477 2024-05-23 13:41:40.018962 openai_responses-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      214 2024-05-21 20:36:49.837714 openai_responses-0.4.1/src/openai_responses/__init__.py
--rw-r--r--   0        0        0      605 2024-05-21 20:36:49.838025 openai_responses-0.4.1/src/openai_responses/_api.py
--rw-r--r--   0        0        0     2447 2024-05-23 13:40:31.177359 openai_responses-0.4.1/src/openai_responses/_mock.py
--rw-r--r--   0        0        0     3863 2024-05-21 20:36:49.838619 openai_responses-0.4.1/src/openai_responses/_routes/__init__.py
--rw-r--r--   0        0        0     5240 2024-05-22 13:56:11.130530 openai_responses-0.4.1/src/openai_responses/_routes/_base.py
--rw-r--r--   0        0        0     6450 2024-05-21 20:36:49.839256 openai_responses-0.4.1/src/openai_responses/_routes/assistants.py
--rw-r--r--   0        0        0     1120 2024-05-21 13:16:58.186179 openai_responses-0.4.1/src/openai_responses/_routes/chat.py
--rw-r--r--   0        0        0     1382 2024-05-21 15:25:22.334161 openai_responses-0.4.1/src/openai_responses/_routes/embeddings.py
--rw-r--r--   0        0        0     5008 2024-05-21 20:36:49.839510 openai_responses-0.4.1/src/openai_responses/_routes/files.py
--rw-r--r--   0        0        0     8746 2024-05-21 20:36:49.839861 openai_responses-0.4.1/src/openai_responses/_routes/messages.py
--rw-r--r--   0        0        0     3780 2024-05-21 20:36:49.840137 openai_responses-0.4.1/src/openai_responses/_routes/run_steps.py
--rw-r--r--   0        0        0    11523 2024-05-21 20:36:49.840446 openai_responses-0.4.1/src/openai_responses/_routes/runs.py
--rw-r--r--   0        0        0     5369 2024-05-21 20:36:49.840740 openai_responses-0.4.1/src/openai_responses/_routes/threads.py
--rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.4.1/src/openai_responses/_types/generics.py
--rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.4.1/src/openai_responses/_types/partials/assistants.py
--rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.4.1/src/openai_responses/_types/partials/chat.py
--rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.4.1/src/openai_responses/_types/partials/embeddings.py
--rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.4.1/src/openai_responses/_types/partials/files.py
--rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.4.1/src/openai_responses/_types/partials/messages.py
--rw-r--r--   0        0        0     2993 2024-05-20 20:53:53.219560 openai_responses-0.4.1/src/openai_responses/_types/partials/run_steps.py
--rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.4.1/src/openai_responses/_types/partials/runs.py
--rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.4.1/src/openai_responses/_types/partials/threads.py
--rw-r--r--   0        0        0      304 2024-05-21 20:36:49.840984 openai_responses-0.4.1/src/openai_responses/_utils/aio.py
--rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.4.1/src/openai_responses/_utils/copy.py
--rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.4.1/src/openai_responses/_utils/faker.py
--rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.4.1/src/openai_responses/_utils/serde.py
--rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.4.1/src/openai_responses/_utils/time.py
--rw-r--r--   0        0        0       56 2024-05-21 20:36:49.841206 openai_responses-0.4.1/src/openai_responses/ext/__init__.py
--rw-r--r--   0        0        0       34 2024-05-21 20:36:49.841452 openai_responses-0.4.1/src/openai_responses/ext/httpx.py
--rw-r--r--   0        0        0       34 2024-05-21 20:36:49.841757 openai_responses-0.4.1/src/openai_responses/ext/respx.py
--rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.4.1/src/openai_responses/helpers/builders/_base.py
--rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.4.1/src/openai_responses/helpers/builders/assistants.py
--rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.4.1/src/openai_responses/helpers/builders/chat.py
--rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.4.1/src/openai_responses/helpers/builders/embeddings.py
--rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.4.1/src/openai_responses/helpers/builders/messages.py
--rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.4.1/src/openai_responses/helpers/builders/run_steps.py
--rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.4.1/src/openai_responses/helpers/builders/runs.py
--rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.4.1/src/openai_responses/helpers/builders/threads.py
--rw-r--r--   0        0        0      317 2024-05-20 16:30:34.412882 openai_responses-0.4.1/src/openai_responses/helpers/mergers/_base.py
--rw-r--r--   0        0        0      290 2024-05-20 16:30:34.413017 openai_responses-0.4.1/src/openai_responses/helpers/mergers/runs.py
--rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.4.1/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.4.1/src/openai_responses/py.typed
--rw-r--r--   0        0        0       62 2024-05-21 20:36:49.841864 openai_responses-0.4.1/src/openai_responses/stores/__init__.py
--rw-r--r--   0        0        0     6151 2024-05-21 20:36:49.841986 openai_responses-0.4.1/src/openai_responses/stores/state_store.py
--rw-r--r--   0        0        0     4855 2024-05-22 14:04:35.946588 openai_responses-0.4.1/src/openai_responses/streaming.py
--rw-r--r--   0        0        0     4607 1970-01-01 00:00:00.000000 openai_responses-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3582 2024-05-28 20:57:51.367143 openai_responses-0.5.0/README.md
+-rw-r--r--   0        0        0     1549 2024-05-28 21:01:32.303905 openai_responses-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      214 2024-05-21 20:36:49.837714 openai_responses-0.5.0/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0      605 2024-05-21 20:36:49.838025 openai_responses-0.5.0/src/openai_responses/_api.py
+-rw-r--r--   0        0        0       43 2024-05-24 14:15:43.348143 openai_responses-0.5.0/src/openai_responses/_constants/__init__.py
+-rw-r--r--   0        0        0     4480 2024-05-24 14:15:43.348330 openai_responses-0.5.0/src/openai_responses/_constants/system_models.py
+-rw-r--r--   0        0        0     2616 2024-05-28 14:27:09.182103 openai_responses-0.5.0/src/openai_responses/_mock.py
+-rw-r--r--   0        0        0     4238 2024-05-28 20:57:51.368072 openai_responses-0.5.0/src/openai_responses/_routes/__init__.py
+-rw-r--r--   0        0        0     5240 2024-05-22 13:56:11.130530 openai_responses-0.5.0/src/openai_responses/_routes/_base.py
+-rw-r--r--   0        0        0     6450 2024-05-21 20:36:49.839256 openai_responses-0.5.0/src/openai_responses/_routes/assistants.py
+-rw-r--r--   0        0        0     1120 2024-05-21 13:16:58.186179 openai_responses-0.5.0/src/openai_responses/_routes/chat.py
+-rw-r--r--   0        0        0     1382 2024-05-21 15:25:22.334161 openai_responses-0.5.0/src/openai_responses/_routes/embeddings.py
+-rw-r--r--   0        0        0     6370 2024-05-28 20:57:51.368300 openai_responses-0.5.0/src/openai_responses/_routes/files.py
+-rw-r--r--   0        0        0     8746 2024-05-21 20:36:49.839861 openai_responses-0.5.0/src/openai_responses/_routes/messages.py
+-rw-r--r--   0        0        0     1960 2024-05-24 14:15:43.348843 openai_responses-0.5.0/src/openai_responses/_routes/models.py
+-rw-r--r--   0        0        0     3780 2024-05-21 20:36:49.840137 openai_responses-0.5.0/src/openai_responses/_routes/run_steps.py
+-rw-r--r--   0        0        0    11523 2024-05-21 20:36:49.840446 openai_responses-0.5.0/src/openai_responses/_routes/runs.py
+-rw-r--r--   0        0        0     5369 2024-05-21 20:36:49.840740 openai_responses-0.5.0/src/openai_responses/_routes/threads.py
+-rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.5.0/src/openai_responses/_types/generics.py
+-rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.5.0/src/openai_responses/_types/partials/assistants.py
+-rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.5.0/src/openai_responses/_types/partials/chat.py
+-rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.5.0/src/openai_responses/_types/partials/embeddings.py
+-rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.5.0/src/openai_responses/_types/partials/files.py
+-rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.5.0/src/openai_responses/_types/partials/messages.py
+-rw-r--r--   0        0        0      354 2024-05-24 14:15:43.348974 openai_responses-0.5.0/src/openai_responses/_types/partials/models.py
+-rw-r--r--   0        0        0     2993 2024-05-20 20:53:53.219560 openai_responses-0.5.0/src/openai_responses/_types/partials/run_steps.py
+-rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.5.0/src/openai_responses/_types/partials/runs.py
+-rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.5.0/src/openai_responses/_types/partials/threads.py
+-rw-r--r--   0        0        0      304 2024-05-21 20:36:49.840984 openai_responses-0.5.0/src/openai_responses/_utils/aio.py
+-rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.5.0/src/openai_responses/_utils/copy.py
+-rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.5.0/src/openai_responses/_utils/faker.py
+-rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.5.0/src/openai_responses/_utils/serde.py
+-rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.5.0/src/openai_responses/_utils/time.py
+-rw-r--r--   0        0        0       56 2024-05-21 20:36:49.841206 openai_responses-0.5.0/src/openai_responses/ext/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-21 20:36:49.841452 openai_responses-0.5.0/src/openai_responses/ext/httpx.py
+-rw-r--r--   0        0        0       34 2024-05-21 20:36:49.841757 openai_responses-0.5.0/src/openai_responses/ext/respx.py
+-rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.5.0/src/openai_responses/helpers/builders/_base.py
+-rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.5.0/src/openai_responses/helpers/builders/assistants.py
+-rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.5.0/src/openai_responses/helpers/builders/chat.py
+-rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.5.0/src/openai_responses/helpers/builders/embeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.5.0/src/openai_responses/helpers/builders/messages.py
+-rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.5.0/src/openai_responses/helpers/builders/run_steps.py
+-rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.5.0/src/openai_responses/helpers/builders/runs.py
+-rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.5.0/src/openai_responses/helpers/builders/threads.py
+-rw-r--r--   0        0        0      317 2024-05-20 16:30:34.412882 openai_responses-0.5.0/src/openai_responses/helpers/mergers/_base.py
+-rw-r--r--   0        0        0      290 2024-05-20 16:30:34.413017 openai_responses-0.5.0/src/openai_responses/helpers/mergers/runs.py
+-rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.5.0/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.5.0/src/openai_responses/py.typed
+-rw-r--r--   0        0        0      118 2024-05-28 20:57:51.368480 openai_responses-0.5.0/src/openai_responses/stores/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-28 20:57:51.368636 openai_responses-0.5.0/src/openai_responses/stores/content_store.py
+-rw-r--r--   0        0        0     6762 2024-05-28 20:57:51.368861 openai_responses-0.5.0/src/openai_responses/stores/state_store.py
+-rw-r--r--   0        0        0     4855 2024-05-22 14:04:35.946588 openai_responses-0.5.0/src/openai_responses/streaming.py
+-rw-r--r--   0        0        0     4723 1970-01-01 00:00:00.000000 openai_responses-0.5.0/PKG-INFO
```

### Comparing `openai_responses-0.4.1/LICENSE` & `openai_responses-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/README.md` & `openai_responses-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [![sdk support](https://img.shields.io/badge/SDK_Support-v1.25+-white?logo=openai&logoColor=black&labelColor=white)](https://github.com/openai/openai-python)
 
 ## Supported Endpoints
 
 - [Chat](https://platform.openai.com/docs/api-reference/chat)
 - [Embeddings](https://platform.openai.com/docs/api-reference/embeddings)
 - [Files](https://platform.openai.com/docs/api-reference/files)
+- [Models](https://platform.openai.com/docs/api-reference/models)
 - [Assistants](https://platform.openai.com/docs/api-reference/assistants)
 - [Threads](https://platform.openai.com/docs/api-reference/threads)
 - [Messages](https://platform.openai.com/docs/api-reference/messages)
 - [Runs](https://platform.openai.com/docs/api-reference/runs)
 - [Run Steps](https://platform.openai.com/docs/api-reference/run-steps)
 
 View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/coverage).
```

### Comparing `openai_responses-0.4.1/pyproject.toml` & `openai_responses-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.4.1"
+version = "0.5.0"
 description = "🧪🤖 Pytest plugin for automatically mocking OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://mharrisb1.github.io/openai-responses-python/"
 documentation = "https://mharrisb1.github.io/openai-responses-python/"
@@ -19,28 +19,32 @@
 openai_responses = "openai_responses.plugin"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 openai = "^1.25"
 respx = "^0.20.2"
 faker-openai-api-provider = "^0.1.0"
+requests-toolbelt = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 types-decorator = "^5.1.8.20240310"
 mkdocs-material = "^9.5.18"
 tox = "^4.14.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.mypy]
+ignore_missing_imports = true
+
 [tool.pyright]
 typeCheckingMode = "strict"
 pythonVersion = "3.9"
 exclude = [".venv"]
 venvPath = "."
 venv = ".venv"
 strictListInference = true
```

### Comparing `openai_responses-0.4.1/src/openai_responses/_api.py` & `openai_responses-0.5.0/src/openai_responses/_api.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_mock.py` & `openai_responses-0.5.0/src/openai_responses/_mock.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import inspect
 from functools import wraps
 from typing import Any, Callable, Optional
 
 import respx
 
-from ._routes import BetaRoutes, ChatRoutes, EmbeddingsRoutes, FileRoutes
+from ._routes import BetaRoutes, ChatRoutes, EmbeddingsRoutes, FileRoutes, ModelRoutes
 from .stores import StateStore
 
 
 class OpenAIMock:
+    beta: BetaRoutes
+    chat: ChatRoutes
+    embeddings: EmbeddingsRoutes
+    files: FileRoutes
+    models: ModelRoutes
+
     def __init__(
         self,
         base_url: Optional[str] = None,
         state: Optional[StateStore] = None,
     ) -> None:
         self._router = respx.mock(
             assert_all_called=False,
             base_url=base_url or "https://api.openai.com/v1",
         )
         self._state = state or StateStore()
-
-        self.beta = BetaRoutes(self._router, self._state)
-        self.chat = ChatRoutes(self._router)
-        self.embeddings = EmbeddingsRoutes(self._router)
-        self.files = FileRoutes(self._router, self._state)
-
-        # NOTE: need to sort routes to avoid match conflicts
-        self._router.routes._routes.sort(key=lambda r: len(repr(r._pattern)), reverse=True)  # type: ignore
+        self._init_routes()
 
     @property
     def router(self) -> respx.MockRouter:
         """[RESPX](https://lundberg.github.io/respx) router with patched OpenAI routes"""
         return self._router
 
     @property
@@ -38,18 +37,26 @@
         """State store for API resources"""
         return self._state
 
     @state.setter
     def state(self, value: StateStore) -> None:
         assert isinstance(value, StateStore), "Object is not an instance of StateStore"
         self._state = value
+        self._init_routes()
+
+    def _init_routes(self) -> None:
+        """Called on construction and anytime that either `router` or `state` values are changed"""
         self.beta = BetaRoutes(self._router, self._state)
         self.chat = ChatRoutes(self._router)
         self.embeddings = EmbeddingsRoutes(self._router)
         self.files = FileRoutes(self._router, self._state)
+        self.models = ModelRoutes(self._router, self._state)
+
+        # NOTE: need to sort routes to avoid match conflicts
+        self._router.routes._routes.sort(key=lambda r: len(repr(r._pattern)), reverse=True)  # type: ignore
 
     def _start_mock(self):
         def wrapper(fn: Callable[..., Any]):
             is_async = inspect.iscoroutinefunction(fn)
             argspec = inspect.getfullargspec(fn)
             needs_ref = "openai_mock" in argspec.args
```

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/__init__.py` & `openai_responses-0.5.0/src/openai_responses/_routes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import respx
 
 from ..stores import StateStore
 
 from .chat import ChatCompletionsCreateRoute
 from .embeddings import EmbeddingsCreateRoute
-from .files import FileCreateRoute, FileListRoute, FileRetrieveRoute, FileDeleteRoute
+from .files import (
+    FileCreateRoute,
+    FileListRoute,
+    FileRetrieveRoute,
+    FileDeleteRoute,
+    FileRetrieveContentRoute,
+)
+from .models import ModelListRoute, ModelRetrieveRoute
 from .assistants import (
     AssistantCreateRoute,
     AssistantListRoute,
     AssistantRetrieveRoute,
     AssistantUpdateRoute,
     AssistantDeleteRoute,
 )
@@ -61,14 +68,21 @@
 
 class FileRoutes:
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         self.create = FileCreateRoute(router, state)
         self.list = FileListRoute(router, state)
         self.retrieve = FileRetrieveRoute(router, state)
         self.delete = FileDeleteRoute(router, state)
+        self.content = FileRetrieveContentRoute(router, state)
+
+
+class ModelRoutes:
+    def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
+        self.list = ModelListRoute(router, state)
+        self.retrieve = ModelRetrieveRoute(router, state)
 
 
 class BetaRoutes:
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         self.assistants = AssistantsRoutes(router, state)
         self.threads = ThreadRoutes(router, state)
```

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/_base.py` & `openai_responses-0.5.0/src/openai_responses/_routes/_base.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/assistants.py` & `openai_responses-0.5.0/src/openai_responses/_routes/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/chat.py` & `openai_responses-0.5.0/src/openai_responses/_routes/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/embeddings.py` & `openai_responses-0.5.0/src/openai_responses/_routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/files.py` & `openai_responses-0.5.0/src/openai_responses/_routes/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import re
-from typing import Any
+import sys
+from typing import Any, Optional
 from typing_extensions import override
 
 import httpx
 import respx
+from requests_toolbelt.multipart import decoder
 
 from openai.pagination import SyncPage
 from openai.types.file_object import FileObject
 from openai.types.file_deleted import FileDeleted
 
 from ._base import StatefulRoute
 
@@ -18,15 +19,14 @@
     PartialFileDeleted,
 )
 
 from .._utils.faker import faker
 from .._utils.serde import model_dict
 from .._utils.time import utcnow_unix_timestamp_s
 
-REGEXP_FILE = r'Content-Disposition: form-data;[^;]+; name="purpose"\r\n\r\n(?P<purpose_value>[^\r\n]+)|filename="(?P<filename>[^"]+)"'
 
 __all__ = ["FileCreateRoute", "FileListRoute", "FileRetrieveRoute", "FileDeleteRoute"]
 
 
 class FileCreateRoute(StatefulRoute[FileObject, PartialFileObject]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
@@ -34,47 +34,59 @@
             status_code=201,
             state=state,
         )
 
     @override
     def _handler(self, request: httpx.Request, route: respx.Route) -> httpx.Response:
         self._route = route
-        model = self._build({}, request)
+
+        filename: Optional[str] = None
+        purpose: Optional[str] = None
+        file_content: Optional[bytes] = None
+
+        multipart_data = decoder.MultipartDecoder(
+            request.content, request.headers.get("content-type")
+        )
+        for part in multipart_data.parts:  # type: ignore
+            content_disposition = part.headers.get(b"Content-Disposition", b"").decode()  # type: ignore
+            if 'name="purpose"' in content_disposition:
+                purpose = part.text  # type: ignore
+            elif 'name="file"' in content_disposition:
+                filename = (  # type: ignore
+                    part.headers.get(b"Content-Disposition", b"")  # type: ignore
+                    .decode()
+                    .split("filename=")[1]
+                    .strip('"')
+                )
+                file_content = part.content  # type: ignore
+
+        assert filename
+        assert purpose
+        assert file_content
+
+        model = FileObject(
+            id=faker.file.id(),
+            bytes=sys.getsizeof(file_content),  # type: ignore
+            created_at=utcnow_unix_timestamp_s(),
+            filename=filename,  # type: ignore
+            object="file",
+            purpose=purpose,  # type: ignore
+            status="uploaded",
+            status_details=None,
+        )
         self._state.files.put(model)
+        self._state.files.content.put(model.id, file_content)  # type: ignore
         return httpx.Response(
             status_code=self._status_code,
             json=model_dict(model),
         )
 
     @staticmethod
     def _build(partial: PartialFileObject, request: httpx.Request) -> FileObject:
-        content = request.content.decode("utf-8")
-
-        filename = ""
-        purpose = "assistants"
-
-        # FIXME: hacky
-        prog = re.compile(REGEXP_FILE)
-        matches = prog.finditer(content)
-        for match in matches:
-            if match.group("filename"):
-                filename = match.group("filename")
-            if match.group("purpose_value"):
-                purpose = match.group("purpose_value")
-
-        return FileObject(
-            id=partial.get("id", faker.file.id()),
-            bytes=partial.get("bytes", 0),
-            created_at=partial.get("created_at", utcnow_unix_timestamp_s()),
-            filename=partial.get("filename", filename),
-            object="file",
-            purpose=partial.get("purpose", purpose),  # type: ignore
-            status=partial.get("status", "uploaded"),
-            status_details=partial.get("status_details"),
-        )
+        raise NotImplementedError
 
 
 class FileListRoute(StatefulRoute[SyncPage[FileObject], PartialFileList]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.get(url__regex="/files"),
             status_code=200,
@@ -155,7 +167,37 @@
 
     @staticmethod
     def _build(
         partial: PartialFileDeleted,
         request: httpx.Request,
     ) -> FileObject:
         raise NotImplementedError
+
+
+class FileRetrieveContentRoute(StatefulRoute[FileObject, PartialFileObject]):
+    def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
+        super().__init__(
+            route=router.get(url__regex=r"/files/(?P<file_id>[a-zA-Z0-9\-]+)/content"),
+            status_code=200,
+            state=state,
+        )
+
+    @override
+    def _handler(
+        self,
+        request: httpx.Request,
+        route: respx.Route,
+        **kwargs: Any,
+    ) -> httpx.Response:
+        self._route = route
+        fil_id = kwargs["file_id"]
+        found = self._state.files.get(fil_id)
+        if not found:
+            return httpx.Response(404)
+
+        content = self._state.files.content.get(found.id)
+        assert content
+        return httpx.Response(status_code=200, content=content)
+
+    @staticmethod
+    def _build(partial: PartialFileObject, request: httpx.Request) -> FileObject:
+        raise NotImplementedError
```

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/messages.py` & `openai_responses-0.5.0/src/openai_responses/_routes/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/run_steps.py` & `openai_responses-0.5.0/src/openai_responses/_routes/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/runs.py` & `openai_responses-0.5.0/src/openai_responses/_routes/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_routes/threads.py` & `openai_responses-0.5.0/src/openai_responses/_routes/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/assistants.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/chat.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/embeddings.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/files.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/messages.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/run_steps.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/runs.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_types/partials/threads.py` & `openai_responses-0.5.0/src/openai_responses/_types/partials/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/_utils/serde.py` & `openai_responses-0.5.0/src/openai_responses/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/helpers/builders/chat.py` & `openai_responses-0.5.0/src/openai_responses/helpers/builders/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/helpers/builders/embeddings.py` & `openai_responses-0.5.0/src/openai_responses/helpers/builders/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/helpers/builders/messages.py` & `openai_responses-0.5.0/src/openai_responses/helpers/builders/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/helpers/builders/run_steps.py` & `openai_responses-0.5.0/src/openai_responses/helpers/builders/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/helpers/builders/runs.py` & `openai_responses-0.5.0/src/openai_responses/helpers/builders/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/src/openai_responses/stores/state_store.py` & `openai_responses-0.5.0/src/openai_responses/stores/state_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from typing import Any, Dict, Generic, List, Literal, Optional, TypeVar, Union
 
-from openai.types import FileObject
+from openai.types import FileObject, Model
 from openai.types.beta.assistant import Assistant
 from openai.types.beta.thread import Thread
 from openai.types.beta.threads.message import Message
 from openai.types.beta.threads.run import Run
 from openai.types.beta.threads.runs.run_step import RunStep
 
+from .content_store import ContentStore
+from .._constants import SYSTEM_MODELS
+from .._utils.serde import model_parse
 
 __all__ = ["StateStore"]
 
 M = TypeVar(
     "M",
     bound=Union[
         FileObject,
+        Model,
         Assistant,
         Thread,
         Message,
         Run,
         RunStep,
     ],
 )
 
-Resource = Union[FileObject, Assistant, Thread, Message, Run, RunStep, Any]
+Resource = Union[FileObject, Assistant, Thread, Message, Run, RunStep, Model, Any]
 
 
 class StateStore:
     def __init__(self) -> None:
         self.files = FileStore()
+        self.models = ModelStore()
         self.beta = Beta()
 
     def _blind_put(self, resource: Resource) -> None:
         if isinstance(resource, FileObject):
             self.files.put(resource)
         elif isinstance(resource, Assistant):
             self.beta.assistants.put(resource)
@@ -39,14 +44,16 @@
             self.beta.threads.put(resource)
         elif isinstance(resource, Message):
             self.beta.threads.messages.put(resource)
         elif isinstance(resource, Run):
             self.beta.threads.runs.put(resource)
         elif isinstance(resource, RunStep):
             self.beta.threads.runs.steps.put(resource)
+        elif isinstance(resource, Model):
+            self.models.put(resource)
         else:
             raise TypeError(f"Cannot put object of type {type(resource)} in store")
 
 
 class Beta:
     def __init__(self) -> None:
         self.assistants = AssistantStore()
@@ -67,16 +74,19 @@
         if self._data.get(id):
             del self._data[id]
             return True
         else:
             return False
 
 
-# TODO: add content storage
 class FileStore(BaseStore[FileObject]):
+    def __init__(self) -> None:
+        super().__init__()
+        self.content = ContentStore()
+
     def list(
         self,
         purpose: Optional[
             Literal[
                 "fine-tune",
                 "fine-tune-results",
                 "assistants",
@@ -86,14 +96,24 @@
     ) -> List[FileObject]:
         files = list(self._data.values())
         if purpose:
             files = [file for file in files if file.purpose == purpose]
         return files
 
 
+class ModelStore(BaseStore[Model]):
+    def __init__(self) -> None:
+        super().__init__()
+        for model in SYSTEM_MODELS:
+            self._data[str(model["id"])] = model_parse(Model, model)
+
+    def list(self) -> List[Model]:
+        return list(self._data.values())
+
+
 class AssistantStore(BaseStore[Assistant]):
     def list(
         self,
         limit: Optional[str] = None,
         order: Optional[str] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
```

### Comparing `openai_responses-0.4.1/src/openai_responses/streaming.py` & `openai_responses-0.5.0/src/openai_responses/streaming.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.4.1/PKG-INFO` & `openai_responses-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-responses
-Version: 0.4.1
+Version: 0.5.0
 Summary: 🧪🤖 Pytest plugin for automatically mocking OpenAI requests
 Home-page: https://mharrisb1.github.io/openai-responses-python/
 License: MIT
 Keywords: openai,pytest,testing
 Author: Michael Harris
 Author-email: mharris@definite.app
 Requires-Python: >=3.9,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Requires-Dist: faker-openai-api-provider (>=0.1.0,<0.2.0)
 Requires-Dist: openai (>=1.25,<2.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: respx (>=0.20.2,<0.21.0)
 Project-URL: Documentation, https://mharrisb1.github.io/openai-responses-python/
 Project-URL: Repository, https://github.com/mharrisb1/openai-responses-python
 Description-Content-Type: text/markdown
 
 # 🧪🤖 openai-responses
 
@@ -30,14 +31,15 @@
 [![sdk support](https://img.shields.io/badge/SDK_Support-v1.25+-white?logo=openai&logoColor=black&labelColor=white)](https://github.com/openai/openai-python)
 
 ## Supported Endpoints
 
 - [Chat](https://platform.openai.com/docs/api-reference/chat)
 - [Embeddings](https://platform.openai.com/docs/api-reference/embeddings)
 - [Files](https://platform.openai.com/docs/api-reference/files)
+- [Models](https://platform.openai.com/docs/api-reference/models)
 - [Assistants](https://platform.openai.com/docs/api-reference/assistants)
 - [Threads](https://platform.openai.com/docs/api-reference/threads)
 - [Messages](https://platform.openai.com/docs/api-reference/messages)
 - [Runs](https://platform.openai.com/docs/api-reference/runs)
 - [Run Steps](https://platform.openai.com/docs/api-reference/run-steps)
 
 View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/coverage).
```

