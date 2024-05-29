# Comparing `tmp/inngest-0.3.8.tar.gz` & `tmp/inngest-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inngest-0.3.8.tar", last modified: Sun Apr  7 14:47:09 2024, max compression
+gzip compressed data, was "inngest-0.3.9.tar", last modified: Fri Apr 19 13:23:33 2024, max compression
```

## Comparing `inngest-0.3.8.tar` & `inngest-0.3.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.904055 inngest-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 14:46:48.000000 inngest-0.3.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-07 14:47:09.904055 inngest-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-07 14:46:48.000000 inngest-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.892055 inngest-0.3.8/inngest/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/client_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/client_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/comm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/const_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/env_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/event_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/event_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/function_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/function_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest/_internal/middleware_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/net_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest/_internal/step_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/step_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/step_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/django.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-07 14:46:48.000000 inngest-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:47:09.904055 inngest-0.3.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.300301 inngest-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 13:23:12.000000 inngest-0.3.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-19 13:23:33.300301 inngest-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-19 13:23:12.000000 inngest-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.292301 inngest-0.3.9/inngest/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.296301 inngest-0.3.9/inngest/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/client_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/client_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/comm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/const_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/env_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/event_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/event_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/function_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/function_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.296301 inngest-0.3.9/inngest/_internal/middleware_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/net_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.296301 inngest-0.3.9/inngest/_internal/step_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/step_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/step_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.300301 inngest-0.3.9/inngest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-19 13:23:12.000000 inngest-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:23:33.300301 inngest-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.300301 inngest-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_types.py
```

### Comparing `inngest-0.3.8/LICENSE.md` & `inngest-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/PKG-INFO` & `inngest-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inngest
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python SDK for Inngest
 Project-URL: Homepage, https://github.com/inngest/inngest-py
 Project-URL: Bug Tracker, https://github.com/inngest/inngest-py/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inngest Version: 0.3.8 Summary: Python SDK for
+Metadata-Version: 2.1 Name: inngest Version: 0.3.9 Summary: Python SDK for
 Inngest Project-URL: Homepage, https://github.com/inngest/inngest-py Project-
 URL: Bug Tracker, https://github.com/inngest/inngest-py/issues Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: Django Classifier:
 Framework :: FastAPI Classifier: Framework :: Flask Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `inngest-0.3.8/README.md` & `inngest-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/__init__.py` & `inngest-0.3.9/inngest/__init__.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/client_lib.py` & `inngest-0.3.9/inngest/_internal/client_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,18 @@
     def event_key(self) -> typing.Optional[str]:
         return self._event_key
 
     @property
     def signing_key(self) -> typing.Optional[str]:
         return self._signing_key
 
+    @property
+    def signing_key_fallback(self) -> typing.Optional[str]:
+        return self._signing_key_fallback
+
     def __init__(
         self,
         *,
         api_base_url: typing.Optional[str] = None,
         app_id: str,
         env: typing.Optional[str] = None,
         event_api_base_url: typing.Optional[str] = None,
@@ -104,14 +108,22 @@
         self.middleware = middleware or []
         self._event_key = event_key or os.getenv(const.EnvKey.EVENT_KEY.value)
 
         self._signing_key = signing_key or os.getenv(
             const.EnvKey.SIGNING_KEY.value
         )
 
+        self._signing_key_fallback = signing_key or os.getenv(
+            const.EnvKey.SIGNING_KEY_FALLBACK.value
+        )
+
+        self._signing_key_fallback = os.getenv(
+            const.EnvKey.SIGNING_KEY_FALLBACK.value
+        )
+
         self._env = env or env_lib.get_environment_name()
         if (
             self._env is None
             and self._signing_key is not None
             and "branch" in self._signing_key
         ):
             self.logger.warning(
@@ -158,15 +170,14 @@
         # do that.
         server_kind = None
 
         headers = net.create_headers(
             env=self._env,
             framework=framework,
             server_kind=server_kind,
-            signing_key=None,
         )
 
         body = []
         for event in events:
             d = event.to_dict()
             if isinstance(d, Exception):
                 return d
@@ -287,40 +298,55 @@
         return decorator
 
     async def _get(self, url: str) -> httpx.Response:
         """
         Perform an asynchronous HTTP GET request. Handles authn
         """
 
+        req = httpx.Client().build_request(
+            "GET",
+            url,
+            headers=net.create_headers(
+                env=self._env,
+                framework=None,
+                server_kind=None,
+            ),
+        )
+
         async with httpx.AsyncClient() as client:
-            return await client.get(
-                url,
-                headers=net.create_headers(
-                    env=self._env,
-                    framework=None,
-                    server_kind=None,
-                    signing_key=self._signing_key,
-                ),
+            return await net.fetch_with_auth_fallback(
+                client,
+                req,
+                signing_key=self._signing_key,
+                signing_key_fallback=self._signing_key_fallback,
             )
 
     def _get_sync(self, url: str) -> httpx.Response:
         """
         Perform a synchronous HTTP GET request. Handles authn
         """
 
-        return httpx.get(
+        req = httpx.Client().build_request(
+            "GET",
             url,
             headers=net.create_headers(
                 env=self._env,
                 framework=None,
                 server_kind=None,
-                signing_key=self._signing_key,
             ),
         )
 
+        with httpx.Client() as client:
+            return net.fetch_with_auth_fallback_sync(
+                client,
+                req,
+                signing_key=self._signing_key,
+                signing_key_fallback=self._signing_key_fallback,
+            )
+
     async def _get_batch(self, run_id: str) -> list[event_lib.Event]:
         """
         Fetch a batch of events from the API
         """
 
         url = urllib.parse.urljoin(
             self._api_origin,
```

### Comparing `inngest-0.3.8/inngest/_internal/client_lib_test.py` & `inngest-0.3.9/inngest/_internal/client_lib_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/comm.py` & `inngest-0.3.9/inngest/_internal/comm.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,23 +143,23 @@
 class CommHandler:
     _base_url: str
     _client: client_lib.Inngest
     _fns: dict[str, function.Function]
     _framework: const.Framework
     _mode: const.ServerKind
     _signing_key: typing.Optional[str]
+    _signing_key_fallback: typing.Optional[str]
 
     def __init__(
         self,
         *,
         api_base_url: typing.Optional[str] = None,
         client: client_lib.Inngest,
         framework: const.Framework,
         functions: list[function.Function],
-        signing_key: typing.Optional[str] = None,
     ) -> None:
         self._client = client
 
         self._mode = client._mode
 
         api_base_url = api_base_url or os.getenv(
             const.EnvKey.API_BASE_URL.value
@@ -174,22 +174,25 @@
             self._api_origin = net.parse_url(api_base_url)
         except Exception as err:
             raise errors.URLInvalidError() from err
 
         self._fns = {fn.get_id(): fn for fn in functions}
         self._framework = framework
 
+        signing_key = client.signing_key
         if signing_key is None:
             if self._client.is_production:
                 signing_key = os.getenv(const.EnvKey.SIGNING_KEY.value)
                 if signing_key is None:
                     self._client.logger.error("missing signing key")
                     raise errors.SigningKeyMissingError()
         self._signing_key = signing_key
 
+        self._signing_key_fallback = client.signing_key_fallback
+
     def _build_registration_request(
         self,
         *,
         app_url: str,
         server_kind: typing.Optional[const.ServerKind],
         sync_id: typing.Optional[str],
     ) -> types.MaybeError[httpx.Request]:
@@ -214,15 +217,14 @@
         if isinstance(body, Exception):
             return body
 
         headers = net.create_headers(
             env=self._client.env,
             framework=self._framework,
             server_kind=server_kind,
-            signing_key=self._signing_key,
         )
 
         params = {}
         if sync_id is not None:
             params[const.QueryParamKey.SYNC_ID.value] = sync_id
 
         return httpx.Client().build_request(
@@ -248,15 +250,18 @@
             target_step_id = None
         else:
             target_step_id = target_hashed_id
 
         middleware = middleware_lib.MiddlewareManager.from_client(self._client)
 
         # Validate the request signature.
-        err = req_sig.validate(self._signing_key)
+        err = req_sig.validate(
+            signing_key=self._signing_key,
+            signing_key_fallback=self._signing_key_fallback,
+        )
         if isinstance(err, Exception):
             return await self._respond(middleware, err)
 
         # Get the function we should call.
         fn = self._get_function(fn_id)
         if isinstance(fn, Exception):
             return await self._respond(middleware, fn)
@@ -314,15 +319,18 @@
             target_step_id = None
         else:
             target_step_id = target_hashed_id
 
         middleware = middleware_lib.MiddlewareManager.from_client(self._client)
 
         # Validate the request signature.
-        err = req_sig.validate(self._signing_key)
+        err = req_sig.validate(
+            signing_key=self._signing_key,
+            signing_key_fallback=self._signing_key_fallback,
+        )
         if isinstance(err, Exception):
             return self._respond_sync(middleware, err)
 
         # Get the function we should call.
         fn = self._get_function(fn_id)
         if isinstance(fn, Exception):
             return self._respond_sync(middleware, fn)
@@ -400,45 +408,75 @@
                 configs.append(config.on_failure)
 
         if len(configs) == 0:
             return errors.FunctionConfigInvalidError("no functions found")
         return configs
 
     def inspect(
-        self, server_kind: typing.Optional[const.ServerKind]
+        self,
+        server_kind: typing.Optional[const.ServerKind],
+        req_sig: net.RequestSignature,
     ) -> CommResponse:
         """Handle Dev Server's auto-discovery."""
 
         if server_kind is not None and server_kind != self._mode:
             # Tell Dev Server to leave the app alone since it's in production
             # mode.
             return CommResponse(
                 body={},
                 headers={},
                 status_code=403,
             )
 
-        body = _Inspection(
-            function_count=len(self._fns),
-            has_event_key=self._client.event_key is not None,
-            has_signing_key=self._signing_key is not None,
-            mode=self._mode,
-        ).to_dict()
+        # Validate the request signature.
+        err = req_sig.validate(
+            signing_key=self._signing_key,
+            signing_key_fallback=self._signing_key_fallback,
+        )
+        if isinstance(err, Exception):
+            body = _InsecureInspection(
+                function_count=len(self._fns),
+                has_event_key=self._client.event_key is not None,
+                has_signing_key=self._signing_key is not None,
+                mode=self._mode,
+            )
+        else:
+            signing_key_hash = (
+                transforms.hash_signing_key(self._signing_key)
+                if self._signing_key
+                else None
+            )
+
+            signing_key_fallback_hash = (
+                transforms.hash_signing_key(self._signing_key_fallback)
+                if self._signing_key_fallback
+                else None
+            )
+
+            body = _SecureInspection(
+                function_count=len(self._fns),
+                has_event_key=self._client.event_key is not None,
+                has_signing_key=self._signing_key is not None,
+                mode=self._mode,
+                signing_key_fallback_hash=signing_key_fallback_hash,
+                signing_key_hash=signing_key_hash,
+            )
+
+        body_json = body.to_dict()
         if isinstance(body, Exception):
-            body = {
+            body_json = {
                 "error": "failed to serialize inspection data",
             }
 
         return CommResponse(
-            body=body,
+            body=body_json,
             headers=net.create_headers(
                 env=self._client.env,
                 framework=self._framework,
                 server_kind=server_kind,
-                signing_key=None,
             ),
             status_code=200,
         )
 
     def _parse_registration_response(
         self,
         server_res: httpx.Response,
@@ -461,15 +499,14 @@
         if server_res.status_code < 400:
             return CommResponse(
                 body=server_res_body,
                 headers=net.create_headers(
                     env=self._client.env,
                     framework=self._framework,
                     server_kind=server_kind,
-                    signing_key=None,
                 ),
                 status_code=http.HTTPStatus.OK,
             )
 
         msg = server_res_body.get("error")
         if not isinstance(msg, str):
             msg = "registration failed"
@@ -485,56 +522,70 @@
         *,
         app_url: str,
         server_kind: typing.Optional[const.ServerKind],
         sync_id: typing.Optional[str] = None,
     ) -> CommResponse:
         """Handle a registration call."""
 
-        res = self._validate_registration(server_kind)
-        if res is not None:
-            return res
+        comm_res = self._validate_registration(server_kind)
+        if comm_res is not None:
+            return comm_res
+
+        req = self._build_registration_request(
+            app_url=app_url,
+            server_kind=server_kind,
+            sync_id=sync_id,
+        )
+        if isinstance(req, Exception):
+            return CommResponse.from_error(self._client.logger, req)
 
         async with httpx.AsyncClient() as client:
-            req = self._build_registration_request(
-                app_url=app_url,
-                server_kind=server_kind,
-                sync_id=sync_id,
+            res = await net.fetch_with_auth_fallback(
+                client,
+                req,
+                signing_key=self._signing_key,
+                signing_key_fallback=self._signing_key_fallback,
             )
-            if isinstance(req, Exception):
-                return CommResponse.from_error(self._client.logger, req)
 
             return self._parse_registration_response(
-                await client.send(req),
+                res,
                 server_kind,
             )
 
     def register_sync(
         self,
         *,
         app_url: str,
         server_kind: typing.Optional[const.ServerKind],
         sync_id: typing.Optional[str],
     ) -> CommResponse:
         """Handle a registration call."""
 
-        res = self._validate_registration(server_kind)
-        if res is not None:
-            return res
+        comm_res = self._validate_registration(server_kind)
+        if comm_res is not None:
+            return comm_res
+
+        req = self._build_registration_request(
+            app_url=app_url,
+            server_kind=server_kind,
+            sync_id=sync_id,
+        )
+        if isinstance(req, Exception):
+            return CommResponse.from_error(self._client.logger, req)
 
         with httpx.Client() as client:
-            req = self._build_registration_request(
-                app_url=app_url,
-                server_kind=server_kind,
-                sync_id=sync_id,
+            res = net.fetch_with_auth_fallback_sync(
+                client,
+                req,
+                signing_key=self._signing_key,
+                signing_key_fallback=self._signing_key_fallback,
             )
-            if isinstance(req, Exception):
-                return CommResponse.from_error(self._client.logger, req)
 
             return self._parse_registration_response(
-                client.send(req),
+                res,
                 server_kind,
             )
 
     async def _respond(
         self,
         middleware: middleware_lib.MiddlewareManager,
         value: typing.Union[execution.CallResult, Exception],
@@ -579,12 +630,17 @@
                 msg,
                 http.HTTPStatus.BAD_REQUEST,
             )
 
         return None
 
 
-class _Inspection(types.BaseModel):
+class _InsecureInspection(types.BaseModel):
     function_count: int
     has_event_key: bool
     has_signing_key: bool
     mode: const.ServerKind
+
+
+class _SecureInspection(_InsecureInspection):
+    signing_key_fallback_hash: typing.Optional[str]
+    signing_key_hash: typing.Optional[str]
```

### Comparing `inngest-0.3.8/inngest/_internal/comm_test.py` & `inngest-0.3.9/inngest/_internal/comm_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/const.py` & `inngest-0.3.9/inngest/_internal/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 
 DEFAULT_API_ORIGIN: typing.Final = "https://api.inngest.com/"
 DEFAULT_EVENT_ORIGIN: typing.Final = "https://inn.gs/"
 DEV_SERVER_ORIGIN: typing.Final = "http://127.0.0.1:8288/"
 LANGUAGE: typing.Final = "py"
 ROOT_STEP_ID: typing.Final = "step"
-VERSION: typing.Final = "0.3.8"
+VERSION: typing.Final = "0.3.9"
 
 
 class EnvKey(enum.Enum):
     API_BASE_URL = "INNGEST_API_BASE_URL"
     DEV = "INNGEST_DEV"
     EVENT_API_BASE_URL = "INNGEST_EVENT_API_BASE_URL"
     EVENT_KEY = "INNGEST_EVENT_KEY"
@@ -23,14 +23,15 @@
     # Render deployment's git branch
     # https://render.com/docs/environment-variables#all-services
     RENDER_GIT_BRANCH = "RENDER_GIT_BRANCH"
 
     SERVE_ORIGIN = "INNGEST_SERVE_ORIGIN"
     SERVE_PATH = "INNGEST_SERVE_PATH"
     SIGNING_KEY = "INNGEST_SIGNING_KEY"
+    SIGNING_KEY_FALLBACK = "INNGEST_SIGNING_KEY_FALLBACK"
 
     # Vercel deployment's git branch
     # https://vercel.com/docs/concepts/projects/environment-variables/system-environment-variables#system-environment-variables
     VERCEL_GIT_BRANCH = "VERCEL_GIT_COMMIT_REF"
 
 
 class ErrorCode(enum.Enum):
```

### Comparing `inngest-0.3.8/inngest/_internal/env_lib.py` & `inngest-0.3.9/inngest/_internal/env_lib.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/errors.py` & `inngest-0.3.9/inngest/_internal/errors.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/event_lib_test.py` & `inngest-0.3.9/inngest/_internal/event_lib_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/execution.py` & `inngest-0.3.9/inngest/_internal/execution.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/function.py` & `inngest-0.3.9/inngest/_internal/function.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/function_config.py` & `inngest-0.3.9/inngest/_internal/function_config.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/function_config_test.py` & `inngest-0.3.9/inngest/_internal/function_config_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/log.py` & `inngest-0.3.9/inngest/_internal/log.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/middleware_lib/log.py` & `inngest-0.3.9/inngest/_internal/middleware_lib/log.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/middleware_lib/manager.py` & `inngest-0.3.9/inngest/_internal/middleware_lib/manager.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/middleware_lib/middleware.py` & `inngest-0.3.9/inngest/_internal/middleware_lib/middleware.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/net.py` & `inngest-0.3.9/inngest/_internal/net.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import hashlib
 import hmac
+import http
 import os
 import typing
 import urllib.parse
 
+import httpx
+
 from . import const, errors, transforms, types
 
 Method = typing.Literal["GET", "POST"]
 
 
 def create_headers(
     *,
     env: typing.Optional[str],
     framework: typing.Optional[const.Framework],
     server_kind: typing.Optional[const.ServerKind],
-    signing_key: typing.Optional[str],
 ) -> dict[str, str]:
     """
     Create standard headers that should exist on every possible outgoing
     request.
     """
 
     headers = {
@@ -29,18 +31,14 @@
 
     if env is not None:
         headers[const.HeaderKey.ENV.value] = env
     if framework is not None:
         headers[const.HeaderKey.FRAMEWORK.value] = framework.value
     if server_kind is not None:
         headers[const.HeaderKey.EXPECTED_SERVER_KIND.value] = server_kind.value
-    if signing_key is not None:
-        headers[
-            const.HeaderKey.AUTHORIZATION.value
-        ] = f"Bearer {transforms.hash_signing_key(signing_key)}"
 
     return headers
 
 
 def create_serve_url(
     *,
     request_url: str,
@@ -81,14 +79,78 @@
         new_path = serve_path
 
     return urllib.parse.urlunparse(
         (new_scheme, new_netloc, new_path, "", "", "")
     )
 
 
+async def fetch_with_auth_fallback(
+    client: httpx.AsyncClient,
+    request: httpx.Request,
+    *,
+    signing_key: typing.Optional[str],
+    signing_key_fallback: typing.Optional[str],
+) -> httpx.Response:
+    """
+    Send an HTTP request with the given signing key. If the response is a 401 or
+    403, then try again with the fallback signing key
+    """
+
+    if signing_key is not None:
+        request.headers[
+            const.HeaderKey.AUTHORIZATION.value
+        ] = f"Bearer {transforms.hash_signing_key(signing_key)}"
+
+    res = await client.send(request)
+    if (
+        res.status_code
+        in (http.HTTPStatus.FORBIDDEN, http.HTTPStatus.UNAUTHORIZED)
+        and signing_key_fallback is not None
+    ):
+        # Try again with the signing key fallback
+        request.headers[
+            const.HeaderKey.AUTHORIZATION.value
+        ] = f"Bearer {transforms.hash_signing_key(signing_key_fallback)}"
+        res = await client.send(request)
+
+    return res
+
+
+def fetch_with_auth_fallback_sync(
+    client: httpx.Client,
+    request: httpx.Request,
+    *,
+    signing_key: typing.Optional[str],
+    signing_key_fallback: typing.Optional[str],
+) -> httpx.Response:
+    """
+    Send an HTTP request with the given signing key. If the response is a 401 or
+    403, then try again with the fallback signing key
+    """
+
+    if signing_key is not None:
+        request.headers[
+            const.HeaderKey.AUTHORIZATION.value
+        ] = f"Bearer {transforms.hash_signing_key(signing_key)}"
+
+    res = client.send(request)
+    if (
+        res.status_code
+        in (http.HTTPStatus.FORBIDDEN, http.HTTPStatus.UNAUTHORIZED)
+        and signing_key_fallback is not None
+    ):
+        # Try again with the signing key fallback
+        request.headers[
+            const.HeaderKey.AUTHORIZATION.value
+        ] = f"Bearer {transforms.hash_signing_key(signing_key_fallback)}"
+        res = client.send(request)
+
+    return res
+
+
 def normalize_headers(headers: dict[str, str]) -> dict[str, str]:
     """
     Ensure that known headers are in the correct casing.
     """
 
     new_headers = {}
 
@@ -128,16 +190,17 @@
         if sig_header is not None:
             parsed = urllib.parse.parse_qs(sig_header)
             if "t" in parsed:
                 self._timestamp = int(parsed["t"][0])
             if "s" in parsed:
                 self._signature = parsed["s"][0]
 
-    def validate(
-        self, signing_key: typing.Optional[str]
+    def _validate(
+        self,
+        signing_key: typing.Optional[str],
     ) -> types.MaybeError[None]:
         if self._mode == const.ServerKind.DEV_SERVER:
             return None
 
         if signing_key is None:
             return errors.SigningKeyMissingError(
                 "cannot validate signature in production mode without a signing key"
@@ -154,7 +217,32 @@
             hashlib.sha256,
         )
         mac.update(str(self._timestamp).encode("utf-8"))
         if not hmac.compare_digest(self._signature, mac.hexdigest()):
             return errors.SigVerificationFailedError()
 
         return None
+
+    def validate(
+        self,
+        *,
+        signing_key: typing.Optional[str],
+        signing_key_fallback: typing.Optional[str],
+    ) -> types.MaybeError[None]:
+        """
+        Validate the request signature. Falls back to the fallback signing key if
+        signature validation fails with the primary signing key.
+
+        Args:
+        ----
+            signing_key: The primary signing key.
+            signing_key_fallback: The fallback signing key.
+        """
+
+        err = self._validate(signing_key)
+        if err is not None and signing_key_fallback is not None:
+            # If the signature validation failed but there's a "fallback"
+            # signing key, attempt to validate the signature with the fallback
+            # key
+            err = self._validate(signing_key_fallback)
+
+        return err
```

### Comparing `inngest-0.3.8/inngest/_internal/step_lib/base.py` & `inngest-0.3.9/inngest/_internal/step_lib/base.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/step_lib/step_async.py` & `inngest-0.3.9/inngest/_internal/step_lib/step_async.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/step_lib/step_sync.py` & `inngest-0.3.9/inngest/_internal/step_lib/step_sync.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/transforms.py` & `inngest-0.3.9/inngest/_internal/transforms.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/transforms_test.py` & `inngest-0.3.9/inngest/_internal/transforms_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/_internal/types.py` & `inngest-0.3.9/inngest/_internal/types.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/inngest/django.py` & `inngest-0.3.9/inngest/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     """
 
     handler = comm.CommHandler(
         api_base_url=client.api_origin,
         client=client,
         framework=FRAMEWORK,
         functions=functions,
-        signing_key=client.signing_key,
     )
 
     if async_mode:
         return _create_handler_async(
             client,
             handler,
             serve_origin=serve_origin,
@@ -83,18 +82,24 @@
         headers = net.normalize_headers(dict(request.headers.items()))
 
         server_kind = transforms.get_server_kind(headers)
         if isinstance(server_kind, Exception):
             client.logger.error(server_kind)
             server_kind = None
 
+        req_sig = net.RequestSignature(
+            body=request.body,
+            headers=headers,
+            mode=client._mode,
+        )
+
         if request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind),
+                handler.inspect(server_kind, req_sig),
                 server_kind,
             )
 
         if request.method == "POST":
             fn_id = request.GET.get(const.QueryParamKey.FUNCTION_ID.value)
             if fn_id is None:
                 raise errors.QueryParamMissingError(
@@ -116,19 +121,15 @@
                 )
 
             return _to_response(
                 client,
                 handler.call_function_sync(
                     call=call,
                     fn_id=fn_id,
-                    req_sig=net.RequestSignature(
-                        body=request.body,
-                        headers=headers,
-                        mode=client._mode,
-                    ),
+                    req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if request.method == "PUT":
             sync_id = request.GET.get(const.QueryParamKey.SYNC_ID.value)
@@ -171,18 +172,24 @@
         headers = net.normalize_headers(dict(request.headers.items()))
 
         server_kind = transforms.get_server_kind(headers)
         if isinstance(server_kind, Exception):
             client.logger.error(server_kind)
             server_kind = None
 
+        req_sig = net.RequestSignature(
+            body=request.body,
+            headers=headers,
+            mode=client._mode,
+        )
+
         if request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind),
+                handler.inspect(server_kind, req_sig),
                 server_kind,
             )
 
         if request.method == "POST":
             fn_id = request.GET.get(const.QueryParamKey.FUNCTION_ID.value)
             if fn_id is None:
                 raise errors.QueryParamMissingError(
@@ -204,19 +211,15 @@
                 )
 
             return _to_response(
                 client,
                 await handler.call_function(
                     call=call,
                     fn_id=fn_id,
-                    req_sig=net.RequestSignature(
-                        body=request.body,
-                        headers=headers,
-                        mode=client._mode,
-                    ),
+                    req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if request.method == "PUT":
             sync_id = request.GET.get(const.QueryParamKey.SYNC_ID.value)
@@ -260,12 +263,11 @@
         body.encode("utf-8"),
         headers={
             **comm_res.headers,
             **net.create_headers(
                 env=client.env,
                 framework=FRAMEWORK,
                 server_kind=server_kind,
-                signing_key=None,
             ),
         },
         status=comm_res.status_code,
     )
```

### Comparing `inngest-0.3.8/inngest/fast_api.py` & `inngest-0.3.9/inngest/fast_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,31 +40,38 @@
     """
 
     handler = comm.CommHandler(
         api_base_url=client.api_origin,
         client=client,
         framework=FRAMEWORK,
         functions=functions,
-        signing_key=client.signing_key,
     )
 
     @app.get("/api/inngest")
     async def get_api_inngest(
         request: fastapi.Request,
     ) -> fastapi.Response:
+        body = await request.body()
         headers = net.normalize_headers(dict(request.headers.items()))
 
         server_kind = transforms.get_server_kind(headers)
         if isinstance(server_kind, Exception):
             client.logger.error(server_kind)
             server_kind = None
 
         return _to_response(
             client,
-            handler.inspect(server_kind),
+            handler.inspect(
+                server_kind,
+                net.RequestSignature(
+                    body=body,
+                    headers=headers,
+                    mode=client._mode,
+                ),
+            ),
             server_kind,
         )
 
     @app.post("/api/inngest")
     async def post_inngest_api(
         fnId: str,  # noqa: N803
         stepId: str,  # noqa: N803
@@ -143,12 +150,11 @@
         content=body.encode("utf-8"),
         headers={
             **comm_res.headers,
             **net.create_headers(
                 env=client.env,
                 framework=FRAMEWORK,
                 server_kind=server_kind,
-                signing_key=None,
             ),
         },
         status_code=comm_res.status_code,
     )
```

### Comparing `inngest-0.3.8/inngest/flask.py` & `inngest-0.3.9/inngest/flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     """
 
     handler = comm.CommHandler(
         api_base_url=client.api_origin,
         client=client,
         framework=FRAMEWORK,
         functions=functions,
-        signing_key=client.signing_key,
     )
 
     async_mode = any(
         function.is_handler_async or function.is_on_failure_handler_async
         for function in functions
     )
     if async_mode:
@@ -83,18 +82,24 @@
         headers = net.normalize_headers(dict(flask.request.headers.items()))
 
         server_kind = transforms.get_server_kind(headers)
         if isinstance(server_kind, Exception):
             client.logger.error(server_kind)
             server_kind = None
 
+        req_sig = net.RequestSignature(
+            body=flask.request.data,
+            headers=headers,
+            mode=client._mode,
+        )
+
         if flask.request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind),
+                handler.inspect(server_kind, req_sig),
                 server_kind,
             )
 
         if flask.request.method == "POST":
             fn_id = flask.request.args.get(
                 const.QueryParamKey.FUNCTION_ID.value
             )
@@ -118,19 +123,15 @@
                 )
 
             return _to_response(
                 client,
                 await handler.call_function(
                     call=call,
                     fn_id=fn_id,
-                    req_sig=net.RequestSignature(
-                        body=flask.request.data,
-                        headers=headers,
-                        mode=client._mode,
-                    ),
+                    req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if flask.request.method == "PUT":
             return _to_response(
@@ -163,18 +164,24 @@
         headers = net.normalize_headers(dict(flask.request.headers.items()))
 
         server_kind = transforms.get_server_kind(headers)
         if isinstance(server_kind, Exception):
             client.logger.error(server_kind)
             server_kind = None
 
+        req_sig = net.RequestSignature(
+            body=flask.request.data,
+            headers=headers,
+            mode=client._mode,
+        )
+
         if flask.request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind),
+                handler.inspect(server_kind, req_sig),
                 server_kind,
             )
 
         if flask.request.method == "POST":
             fn_id = flask.request.args.get(
                 const.QueryParamKey.FUNCTION_ID.value
             )
@@ -198,19 +205,15 @@
                 )
 
             return _to_response(
                 client,
                 handler.call_function_sync(
                     call=call,
                     fn_id=fn_id,
-                    req_sig=net.RequestSignature(
-                        body=flask.request.data,
-                        headers=headers,
-                        mode=client._mode,
-                    ),
+                    req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if flask.request.method == "PUT":
             sync_id = flask.request.args.get(const.QueryParamKey.SYNC_ID.value)
@@ -246,13 +249,12 @@
     return flask.Response(
         headers={
             **comm_res.headers,
             **net.create_headers(
                 env=client.env,
                 framework=FRAMEWORK,
                 server_kind=server_kind,
-                signing_key=None,
             ),
         },
         response=body.encode("utf-8"),
         status=comm_res.status_code,
     )
```

### Comparing `inngest-0.3.8/inngest/tornado.py` & `inngest-0.3.9/inngest/tornado.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         serve_path: Path to serve the functions from.
     """
     handler = comm.CommHandler(
         api_base_url=client.api_origin,
         client=client,
         framework=FRAMEWORK,
         functions=functions,
-        signing_key=client.signing_key,
     )
 
     class InngestHandler(tornado.web.RequestHandler):
         def data_received(
             self, chunk: bytes
         ) -> typing.Optional[typing.Awaitable[None]]:
             return None
@@ -57,15 +56,21 @@
             headers = net.normalize_headers(dict(self.request.headers.items()))
 
             server_kind = transforms.get_server_kind(headers)
             if isinstance(server_kind, Exception):
                 client.logger.error(server_kind)
                 server_kind = None
 
-            comm_res = handler.inspect(server_kind)
+            req_sig = net.RequestSignature(
+                body=self.request.body,
+                headers=headers,
+                mode=client._mode,
+            )
+
+            comm_res = handler.inspect(server_kind, req_sig)
 
             self._write_comm_response(comm_res, server_kind)
 
         def post(self) -> None:
             fn_id: typing.Optional[str]
             raw_fn_id = self.request.query_arguments.get(
                 const.QueryParamKey.FUNCTION_ID.value
@@ -89,29 +94,31 @@
             headers = net.normalize_headers(dict(self.request.headers.items()))
 
             server_kind = transforms.get_server_kind(headers)
             if isinstance(server_kind, Exception):
                 client.logger.error(server_kind)
                 server_kind = None
 
+            req_sig = net.RequestSignature(
+                body=self.request.body,
+                headers=headers,
+                mode=client._mode,
+            )
+
             call = execution.Call.from_raw(json.loads(self.request.body))
             if isinstance(call, Exception):
                 return self._write_comm_response(
                     comm.CommResponse.from_error(client.logger, call),
                     server_kind,
                 )
 
             comm_res = handler.call_function_sync(
                 call=call,
                 fn_id=fn_id,
-                req_sig=net.RequestSignature(
-                    body=self.request.body,
-                    headers=headers,
-                    mode=client._mode,
-                ),
+                req_sig=req_sig,
                 target_hashed_id=step_id,
             )
 
             self._write_comm_response(comm_res, server_kind)
 
         def put(self) -> None:
             headers = net.normalize_headers(dict(self.request.headers.items()))
@@ -154,14 +161,13 @@
 
             for k, v in comm_res.headers.items():
                 self.add_header(k, v)
             for k, v in net.create_headers(
                 env=client.env,
                 framework=FRAMEWORK,
                 server_kind=server_kind,
-                signing_key=None,
             ).items():
                 self.add_header(k, v)
 
             self.set_status(comm_res.status_code)
 
     app.add_handlers(r".*", [("/api/inngest", InngestHandler)])
```

### Comparing `inngest-0.3.8/inngest.egg-info/PKG-INFO` & `inngest-0.3.9/inngest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inngest
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python SDK for Inngest
 Project-URL: Homepage, https://github.com/inngest/inngest-py
 Project-URL: Bug Tracker, https://github.com/inngest/inngest-py/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inngest Version: 0.3.8 Summary: Python SDK for
+Metadata-Version: 2.1 Name: inngest Version: 0.3.9 Summary: Python SDK for
 Inngest Project-URL: Homepage, https://github.com/inngest/inngest-py Project-
 URL: Bug Tracker, https://github.com/inngest/inngest-py/issues Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: Django Classifier:
 Framework :: FastAPI Classifier: Framework :: Flask Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `inngest-0.3.8/inngest.egg-info/SOURCES.txt` & `inngest-0.3.9/inngest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/pyproject.toml` & `inngest-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "inngest"
-version = "0.3.8"
+version = "0.3.9"
 description = "Python SDK for Inngest"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Django",
     "Framework :: FastAPI",
     "Framework :: Flask",
```

### Comparing `inngest-0.3.8/tests/test_client.py` & `inngest-0.3.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/tests/test_django.py` & `inngest-0.3.9/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/tests/test_fast_api.py` & `inngest-0.3.9/tests/test_flask.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import dataclasses
 import json
 import typing
 import unittest
 
-import fastapi
-import fastapi.testclient
+import flask
+import flask.logging
+import flask.testing
+import pytest
 
 import inngest
-import inngest.fast_api
-from inngest._internal import const
+import inngest.flask
+from inngest._internal import const, errors
 
 from . import base, cases, dev_server, http_proxy, net
 
-_framework = "fast_api"
+_framework = "flask"
 _dev_server_origin = f"http://{net.HOST}:{dev_server.PORT}"
 
 _client = inngest.Inngest(
     api_base_url=_dev_server_origin,
     app_id=_framework,
     event_api_base_url=_dev_server_origin,
     is_production=False,
 )
 
-_cases = cases.create_async_cases(_client, _framework)
+_cases = cases.create_sync_cases(_client, _framework)
 _fns: list[inngest.Function] = []
 for case in _cases:
     if isinstance(case.fn, list):
         _fns.extend(case.fn)
     else:
         _fns.append(case.fn)
 
 
-class TestFastAPI(unittest.TestCase):
-    app: fastapi.FastAPI
+class TestFunctions(unittest.TestCase):
+    app: flask.testing.FlaskClient
     client: inngest.Inngest
     dev_server_port: int
-    fast_api_client: fastapi.testclient.TestClient
     proxy: http_proxy.Proxy
 
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
-        cls.app = fastapi.FastAPI()
+        app = flask.Flask(__name__)
         cls.client = _client
 
-        inngest.fast_api.serve(
-            cls.app,
+        inngest.flask.serve(
+            app,
             cls.client,
             _fns,
         )
-        cls.fast_api_client = fastapi.testclient.TestClient(cls.app)
+        cls.app = app.test_client()
         cls.proxy = http_proxy.Proxy(cls.on_proxy_request).start()
         base.register(cls.proxy.port)
 
     @classmethod
     def tearDownClass(cls) -> None:
         super().tearDownClass()
         cls.proxy.stop()
@@ -63,44 +64,55 @@
         cls,
         *,
         body: typing.Optional[bytes],
         headers: dict[str, list[str]],
         method: str,
         path: str,
     ) -> http_proxy.Response:
-        if body is None or len(body) == 0:
-            body = json.dumps({}).encode("utf-8")
-
-        new_headers = {key: value[0] for key, value in headers.items()}
-
-        if method == "POST":
-            res = cls.fast_api_client.post(
-                path,
-                content=body,
-                headers=new_headers,
-            )
-        elif method == "PUT":
-            res = cls.fast_api_client.put(
-                path,
-                content=body,
-                headers=new_headers,
-            )
-        else:
-            raise Exception(f"unsupported method: {method}")
+        res = cls.app.open(
+            method=method,
+            path=path,
+            headers=headers,
+            data=body,
+        )
 
         return http_proxy.Response(
-            body=res.content,
+            body=res.data,
             headers=dict(res.headers),
             status_code=res.status_code,
         )
 
 
 for case in _cases:
     test_name = f"test_{case.name}"
-    setattr(TestFastAPI, test_name, case.run_test)
+    setattr(TestFunctions, test_name, case.run_test)
+
+
+class TestServe(unittest.TestCase):
+    def test_cloud_mode_without_signing_key(self) -> None:
+        """
+        When in Cloud mode but no signing key, raise an error.
+
+        This test isn't needed for every framework since it's testing logic in
+        CommHandler
+        """
+
+        app = flask.Flask(__name__)
+        client = inngest.Inngest(app_id="client")
+
+        @client.create_function(
+            fn_id="fn",
+            trigger=inngest.TriggerEvent(event="event"),
+        )
+        def fn(ctx: inngest.Context, step: inngest.StepSync) -> None:
+            pass
+
+        with pytest.raises(Exception) as err:
+            inngest.flask.serve(app, client, [fn])
+        assert isinstance(err.value, errors.SigningKeyMissingError)
 
 
 class TestRegistration(unittest.TestCase):
     def test_sync_with_server_kind_mismatch(self) -> None:
         """Ensure that Dev Server cannot initiate a registration request when in
         production mode.
         """
@@ -111,39 +123,37 @@
         )
 
         @client.create_function(
             fn_id="foo",
             retries=0,
             trigger=inngest.TriggerEvent(event="app/foo"),
         )
-        async def fn(
+        def fn(
             ctx: inngest.Context,
-            step: inngest.Step,
+            step: inngest.StepSync,
         ) -> None:
             pass
 
-        app = fastapi.FastAPI()
-        inngest.fast_api.serve(
+        app = flask.Flask(__name__)
+        inngest.flask.serve(
             app,
             client,
             [fn],
         )
-        fast_api_client = fastapi.testclient.TestClient(app)
-        res = fast_api_client.put(
+        flask_client = app.test_client()
+        res = flask_client.put(
             "/api/inngest",
             headers={
                 const.HeaderKey.SERVER_KIND.value.lower(): const.ServerKind.DEV_SERVER.value,
             },
         )
         assert res.status_code == 400
-        body: object = res.json()
-        assert (
-            isinstance(body, dict)
-            and body["code"] == const.ErrorCode.SERVER_KIND_MISMATCH.value
-        )
+        body: object = res.json
+        assert isinstance(body, dict)
+        assert body["code"] == const.ErrorCode.SERVER_KIND_MISMATCH.value
 
     def test_sync_to_cloud_branch_env(self) -> None:
         """
         Test that the SDK correctly syncs itself with Cloud when using a branch
         environment.
 
         We need to use a mock Cloud since the Dev Server doesn't have a mode
@@ -175,40 +185,82 @@
         mock_cloud = http_proxy.Proxy(on_request).start()
         self.addCleanup(mock_cloud.stop)
 
         client = inngest.Inngest(
             api_base_url=f"http://localhost:{mock_cloud.port}",
             app_id="my-app",
             env="my-env",
-            signing_key="signkey-prod-0486c9",
+            signing_key="signkey-branch-123abc",
         )
 
         @client.create_function(
             fn_id="foo",
             retries=0,
             trigger=inngest.TriggerEvent(event="app/foo"),
         )
         def fn(
             ctx: inngest.Context,
             step: inngest.StepSync,
         ) -> None:
             pass
 
-        app = fastapi.FastAPI()
-        inngest.fast_api.serve(
+        app = flask.Flask(__name__)
+        inngest.flask.serve(
             app,
             client,
             [fn],
         )
-        fast_api_client = fastapi.testclient.TestClient(app)
-        res = fast_api_client.put("/api/inngest")
+        flask_client = app.test_client()
+        res = flask_client.put("/api/inngest")
         assert res.status_code == 200
         assert state.headers.get("Authorization") is not None
         assert state.headers.get("X-Inngest-Env") == ["my-env"]
-        assert state.headers.get("X-Inngest-Framework") == ["fast_api"]
+        assert state.headers.get("X-Inngest-Framework") == ["flask"]
         assert state.headers.get("X-Inngest-SDK") == [
             f"inngest-py:v{const.VERSION}"
         ]
 
 
+class TestIntrospection(base.BaseTestIntrospection):
+    def _serve(self, client: inngest.Inngest) -> flask.testing.FlaskClient:
+        app = flask.Flask(__name__)
+        inngest.flask.serve(
+            app,
+            client,
+            self.create_functions(client),
+        )
+        return app.test_client()
+
+    def test_insecure(self) -> None:
+        flask_client = self._serve(
+            inngest.Inngest(
+                app_id="test",
+                event_key="test",
+                signing_key=self.signing_key,
+            )
+        )
+        res = flask_client.get("/api/inngest")
+        assert res.status_code == 200
+        assert res.json == self.expected_insecure_body
+
+    def test_secure(self) -> None:
+        self.set_signing_key_fallback_env_var()
+
+        flask_client = self._serve(
+            inngest.Inngest(
+                app_id="test",
+                event_key="test",
+                signing_key=self.signing_key,
+            )
+        )
+        res = flask_client.get(
+            "/api/inngest",
+            headers={
+                const.HeaderKey.SIGNATURE.value: self.create_signature(),
+            },
+        )
+        assert res.status_code == 200
+        assert res.json == self.expected_secure_body
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `inngest-0.3.8/tests/test_flask.py` & `inngest-0.3.9/tests/test_fast_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 import dataclasses
 import json
 import typing
 import unittest
 
-import flask
-import flask.logging
-import flask.testing
-import pytest
+import fastapi
+import fastapi.testclient
 
 import inngest
-import inngest.flask
-from inngest._internal import const, errors
+import inngest.fast_api
+from inngest._internal import const
 
 from . import base, cases, dev_server, http_proxy, net
 
-_framework = "flask"
+_framework = "fast_api"
 _dev_server_origin = f"http://{net.HOST}:{dev_server.PORT}"
 
 _client = inngest.Inngest(
     api_base_url=_dev_server_origin,
     app_id=_framework,
     event_api_base_url=_dev_server_origin,
     is_production=False,
 )
 
-_cases = cases.create_sync_cases(_client, _framework)
+_cases = cases.create_async_cases(_client, _framework)
 _fns: list[inngest.Function] = []
 for case in _cases:
     if isinstance(case.fn, list):
         _fns.extend(case.fn)
     else:
         _fns.append(case.fn)
 
 
-class TestFunctions(unittest.TestCase):
-    app: flask.testing.FlaskClient
+class TestFastAPI(unittest.TestCase):
+    app: fastapi.FastAPI
     client: inngest.Inngest
     dev_server_port: int
+    fast_api_client: fastapi.testclient.TestClient
     proxy: http_proxy.Proxy
 
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
-        app = flask.Flask(__name__)
+        cls.app = fastapi.FastAPI()
         cls.client = _client
 
-        inngest.flask.serve(
-            app,
+        inngest.fast_api.serve(
+            cls.app,
             cls.client,
             _fns,
         )
-        cls.app = app.test_client()
+        cls.fast_api_client = fastapi.testclient.TestClient(cls.app)
         cls.proxy = http_proxy.Proxy(cls.on_proxy_request).start()
         base.register(cls.proxy.port)
 
     @classmethod
     def tearDownClass(cls) -> None:
         super().tearDownClass()
         cls.proxy.stop()
@@ -64,55 +63,44 @@
         cls,
         *,
         body: typing.Optional[bytes],
         headers: dict[str, list[str]],
         method: str,
         path: str,
     ) -> http_proxy.Response:
-        res = cls.app.open(
-            method=method,
-            path=path,
-            headers=headers,
-            data=body,
-        )
+        if body is None or len(body) == 0:
+            body = json.dumps({}).encode("utf-8")
+
+        new_headers = {key: value[0] for key, value in headers.items()}
+
+        if method == "POST":
+            res = cls.fast_api_client.post(
+                path,
+                content=body,
+                headers=new_headers,
+            )
+        elif method == "PUT":
+            res = cls.fast_api_client.put(
+                path,
+                content=body,
+                headers=new_headers,
+            )
+        else:
+            raise Exception(f"unsupported method: {method}")
 
         return http_proxy.Response(
-            body=res.data,
+            body=res.content,
             headers=dict(res.headers),
             status_code=res.status_code,
         )
 
 
 for case in _cases:
     test_name = f"test_{case.name}"
-    setattr(TestFunctions, test_name, case.run_test)
-
-
-class TestServe(unittest.TestCase):
-    def test_cloud_mode_without_signing_key(self) -> None:
-        """
-        When in Cloud mode but no signing key, raise an error.
-
-        This test isn't needed for every framework since it's testing logic in
-        CommHandler
-        """
-
-        app = flask.Flask(__name__)
-        client = inngest.Inngest(app_id="client")
-
-        @client.create_function(
-            fn_id="fn",
-            trigger=inngest.TriggerEvent(event="event"),
-        )
-        def fn(ctx: inngest.Context, step: inngest.StepSync) -> None:
-            pass
-
-        with pytest.raises(Exception) as err:
-            inngest.flask.serve(app, client, [fn])
-        assert isinstance(err.value, errors.SigningKeyMissingError)
+    setattr(TestFastAPI, test_name, case.run_test)
 
 
 class TestRegistration(unittest.TestCase):
     def test_sync_with_server_kind_mismatch(self) -> None:
         """Ensure that Dev Server cannot initiate a registration request when in
         production mode.
         """
@@ -123,37 +111,39 @@
         )
 
         @client.create_function(
             fn_id="foo",
             retries=0,
             trigger=inngest.TriggerEvent(event="app/foo"),
         )
-        def fn(
+        async def fn(
             ctx: inngest.Context,
-            step: inngest.StepSync,
+            step: inngest.Step,
         ) -> None:
             pass
 
-        app = flask.Flask(__name__)
-        inngest.flask.serve(
+        app = fastapi.FastAPI()
+        inngest.fast_api.serve(
             app,
             client,
             [fn],
         )
-        flask_client = app.test_client()
-        res = flask_client.put(
+        fast_api_client = fastapi.testclient.TestClient(app)
+        res = fast_api_client.put(
             "/api/inngest",
             headers={
                 const.HeaderKey.SERVER_KIND.value.lower(): const.ServerKind.DEV_SERVER.value,
             },
         )
         assert res.status_code == 400
-        body: object = res.json
-        assert isinstance(body, dict)
-        assert body["code"] == const.ErrorCode.SERVER_KIND_MISMATCH.value
+        body: object = res.json()
+        assert (
+            isinstance(body, dict)
+            and body["code"] == const.ErrorCode.SERVER_KIND_MISMATCH.value
+        )
 
     def test_sync_to_cloud_branch_env(self) -> None:
         """
         Test that the SDK correctly syncs itself with Cloud when using a branch
         environment.
 
         We need to use a mock Cloud since the Dev Server doesn't have a mode
@@ -185,40 +175,82 @@
         mock_cloud = http_proxy.Proxy(on_request).start()
         self.addCleanup(mock_cloud.stop)
 
         client = inngest.Inngest(
             api_base_url=f"http://localhost:{mock_cloud.port}",
             app_id="my-app",
             env="my-env",
-            signing_key="signkey-branch-123abc",
+            signing_key="signkey-prod-0486c9",
         )
 
         @client.create_function(
             fn_id="foo",
             retries=0,
             trigger=inngest.TriggerEvent(event="app/foo"),
         )
         def fn(
             ctx: inngest.Context,
             step: inngest.StepSync,
         ) -> None:
             pass
 
-        app = flask.Flask(__name__)
-        inngest.flask.serve(
+        app = fastapi.FastAPI()
+        inngest.fast_api.serve(
             app,
             client,
             [fn],
         )
-        flask_client = app.test_client()
-        res = flask_client.put("/api/inngest")
+        fast_api_client = fastapi.testclient.TestClient(app)
+        res = fast_api_client.put("/api/inngest")
         assert res.status_code == 200
         assert state.headers.get("Authorization") is not None
         assert state.headers.get("X-Inngest-Env") == ["my-env"]
-        assert state.headers.get("X-Inngest-Framework") == ["flask"]
+        assert state.headers.get("X-Inngest-Framework") == ["fast_api"]
         assert state.headers.get("X-Inngest-SDK") == [
             f"inngest-py:v{const.VERSION}"
         ]
 
 
+class TestIntrospection(base.BaseTestIntrospection):
+    def _serve(self, client: inngest.Inngest) -> fastapi.testclient.TestClient:
+        app = fastapi.FastAPI()
+        inngest.fast_api.serve(
+            app,
+            client,
+            self.create_functions(client),
+        )
+        return fastapi.testclient.TestClient(app)
+
+    def test_insecure(self) -> None:
+        fast_api_client = self._serve(
+            inngest.Inngest(
+                app_id="test",
+                event_key="test",
+                signing_key=self.signing_key,
+            )
+        )
+        res = fast_api_client.get("/api/inngest")
+        assert res.status_code == 200
+        assert res.json() == self.expected_insecure_body
+
+    def test_secure(self) -> None:
+        self.set_signing_key_fallback_env_var()
+
+        fast_api_client = self._serve(
+            inngest.Inngest(
+                app_id="test",
+                event_key="test",
+                signing_key=self.signing_key,
+            )
+        )
+        res = fast_api_client.get(
+            "/api/inngest",
+            headers={
+                const.HeaderKey.SIGNATURE.value: self.create_signature(),
+            },
+        )
+        assert res.status_code == 200
+        assert res.json() == self.expected_secure_body
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `inngest-0.3.8/tests/test_tornado.py` & `inngest-0.3.9/tests/test_tornado.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.8/tests/test_types.py` & `inngest-0.3.9/tests/test_types.py`

 * *Files identical despite different names*

