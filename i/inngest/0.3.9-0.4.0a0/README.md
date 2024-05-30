# Comparing `tmp/inngest-0.3.9.tar.gz` & `tmp/inngest-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inngest-0.3.9.tar", last modified: Fri Apr 19 13:23:33 2024, max compression
+gzip compressed data, was "inngest-0.4.0a0.tar", last modified: Wed May 29 23:52:11 2024, max compression
```

## Comparing `inngest-0.3.9.tar` & `inngest-0.4.0a0.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.300301 inngest-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 13:23:12.000000 inngest-0.3.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-19 13:23:33.300301 inngest-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-19 13:23:12.000000 inngest-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.292301 inngest-0.3.9/inngest/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.296301 inngest-0.3.9/inngest/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/client_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/client_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20519 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/comm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/const_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/env_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/event_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/event_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/function_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/function_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.296301 inngest-0.3.9/inngest/_internal/middleware_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/middleware_lib/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/net.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/net_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.296301 inngest-0.3.9/inngest/_internal/step_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/step_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/step_lib/step_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/django.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-19 13:23:12.000000 inngest-0.3.9/inngest/tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.300301 inngest-0.3.9/inngest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 13:23:33.000000 inngest-0.3.9/inngest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-19 13:23:12.000000 inngest-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:23:33.300301 inngest-0.3.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:23:33.300301 inngest-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 13:23:12.000000 inngest-0.3.9/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.733080 inngest-0.4.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 23:51:38.000000 inngest-0.4.0a0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-29 23:52:11.733080 inngest-0.4.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-29 23:51:38.000000 inngest-0.4.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.725080 inngest-0.4.0a0/inngest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.729080 inngest-0.4.0a0/inngest/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/async_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.729080 inngest-0.4.0a0/inngest/_internal/client_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/client_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/client_lib/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/client_lib/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/client_lib/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23094 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/comm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/const_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/env_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/event_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/event_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16995 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/function_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/function_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.729080 inngest-0.4.0a0/inngest/_internal/middleware_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/middleware_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/middleware_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11093 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/middleware_lib/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/middleware_lib/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13199 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/net_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.733080 inngest-0.4.0a0/inngest/_internal/step_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/step_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/step_lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/step_lib/step_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13683 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/step_lib/step_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/digital_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/django.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.733080 inngest-0.4.0a0/inngest/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/experimental/digital_ocean_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/experimental/encryption_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/experimental/sentry_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-29 23:51:38.000000 inngest-0.4.0a0/inngest/tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.733080 inngest-0.4.0a0/inngest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-29 23:52:11.000000 inngest-0.4.0a0/inngest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-29 23:52:11.000000 inngest-0.4.0a0/inngest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:52:11.000000 inngest-0.4.0a0/inngest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-29 23:52:11.000000 inngest-0.4.0a0/inngest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 23:52:11.000000 inngest-0.4.0a0/inngest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-29 23:51:38.000000 inngest-0.4.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 23:52:11.733080 inngest-0.4.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:52:11.733080 inngest-0.4.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-29 23:51:38.000000 inngest-0.4.0a0/tests/test_types.py
```

### Comparing `inngest-0.3.9/LICENSE.md` & `inngest-0.4.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inngest-0.3.9/PKG-INFO` & `inngest-0.4.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: inngest
-Version: 0.3.9
+Version: 0.4.0a0
 Summary: Python SDK for Inngest
 Project-URL: Homepage, https://github.com/inngest/inngest-py
 Project-URL: Bug Tracker, https://github.com/inngest/inngest-py/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,21 +19,24 @@
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: pydantic>=2.1.1
 Requires-Dist: typing-extensions>=4.8.0
 Provides-Extra: extra
 Requires-Dist: Django==4.2; extra == "extra"
 Requires-Dist: Flask==2.3.0; extra == "extra"
 Requires-Dist: build==1.0.3; extra == "extra"
+Requires-Dist: cryptography==42.0.5; extra == "extra"
 Requires-Dist: django-types==0.19.1; extra == "extra"
 Requires-Dist: fastapi==0.100.0; extra == "extra"
 Requires-Dist: mypy==1.8.0; extra == "extra"
+Requires-Dist: pynacl==1.5.0; extra == "extra"
 Requires-Dist: pytest==7.4.2; extra == "extra"
 Requires-Dist: pytest-django==4.7.0; extra == "extra"
 Requires-Dist: pytest-xdist[psutil]==3.3.1; extra == "extra"
 Requires-Dist: ruff==0.1.9; extra == "extra"
+Requires-Dist: sentry-sdk==2.1.1; extra == "extra"
 Requires-Dist: toml==0.10.2; extra == "extra"
 Requires-Dist: tornado==6.3; extra == "extra"
 Requires-Dist: types-toml==0.10.8.7; extra == "extra"
 Requires-Dist: types-tornado==5.1.1; extra == "extra"
 Requires-Dist: uvicorn==0.23.2; extra == "extra"
 
 <div align="center">
@@ -57,18 +60,17 @@
   </p>
 </div>
 
 <hr />
 
 # Inngest Python SDK
 
-> 🚧 Currently in beta! Users have deployed our Python SDK in their production environments but it isn't as battle-tested as our TypeScript SDK.
-
 We currently support the following frameworks (but adding a new framework is easy!):
 
+- DigitalOcean Functions
 - Django (`>=4.2`)
 - FastAPI (`>=0.100.0`)
 - Flask (`>=2.3.0`)
 - Tornado (`>=6.3`)
 
 Python 3.9 is the minimum version we support.
 
@@ -181,15 +183,15 @@
     def _fetch_ship(url: str) -> dict:
         res = requests.get(url)
         return res.json()
 
     ship_names = []
     for ship_url in person["starships"]:
         # step.run works in loops!
-        ship = step.run("fetch_ship", lambda: _fetch_ship(ship_url))
+        ship = step.run("fetch_ship", _fetch_ship, ship_url)
 
         ship_names.append(ship["name"])
 
     return {
         "person_name": person["name"],
         "ship_names": ship_names,
     }
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1 Name: inngest Version: 0.3.9 Summary: Python SDK for
+Metadata-Version: 2.1 Name: inngest Version: 0.4.0a0 Summary: Python SDK for
 Inngest Project-URL: Homepage, https://github.com/inngest/inngest-py Project-
 URL: Bug Tracker, https://github.com/inngest/inngest-py/issues Classifier:
-Development Status :: 4 - Beta Classifier: Framework :: Django Classifier:
-Framework :: FastAPI Classifier: Framework :: Flask Classifier: Intended
-Audience :: Developers Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Development Status :: 5 - Production/Stable Classifier: Framework :: Django
+Classifier: Framework :: FastAPI Classifier: Framework :: Flask Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python ::
+3.9 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: httpx>=0.24.0 Requires-Dist: pydantic>=2.1.1
 Requires-Dist: typing-extensions>=4.8.0 Provides-Extra: extra Requires-Dist:
 Django==4.2; extra == "extra" Requires-Dist: Flask==2.3.0; extra == "extra"
-Requires-Dist: build==1.0.3; extra == "extra" Requires-Dist: django-
-types==0.19.1; extra == "extra" Requires-Dist: fastapi==0.100.0; extra ==
-"extra" Requires-Dist: mypy==1.8.0; extra == "extra" Requires-Dist:
-pytest==7.4.2; extra == "extra" Requires-Dist: pytest-django==4.7.0; extra ==
-"extra" Requires-Dist: pytest-xdist[psutil]==3.3.1; extra == "extra" Requires-
-Dist: ruff==0.1.9; extra == "extra" Requires-Dist: toml==0.10.2; extra ==
+Requires-Dist: build==1.0.3; extra == "extra" Requires-Dist:
+cryptography==42.0.5; extra == "extra" Requires-Dist: django-types==0.19.1;
+extra == "extra" Requires-Dist: fastapi==0.100.0; extra == "extra" Requires-
+Dist: mypy==1.8.0; extra == "extra" Requires-Dist: pynacl==1.5.0; extra ==
+"extra" Requires-Dist: pytest==7.4.2; extra == "extra" Requires-Dist: pytest-
+django==4.7.0; extra == "extra" Requires-Dist: pytest-xdist[psutil]==3.3.1;
+extra == "extra" Requires-Dist: ruff==0.1.9; extra == "extra" Requires-Dist:
+sentry-sdk==2.1.1; extra == "extra" Requires-Dist: toml==0.10.2; extra ==
 "extra" Requires-Dist: tornado==6.3; extra == "extra" Requires-Dist: types-
 toml==0.10.8.7; extra == "extra" Requires-Dist: types-tornado==5.1.1; extra ==
 "extra" Requires-Dist: uvicorn==0.23.2; extra == "extra"
 
 _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_3_0_6_1_7_7_/_1_9_1_5_8_0_7_1_7_-_1_f_5_6_3_f_4_c_-_3_1_e_3_-_4_a_a_0_-
                             _8_4_8_c_-_5_d_d_c_9_7_8_0_8_a_9_a_._p_n_g_]
 
@@ -28,31 +30,29 @@
               Read the _d_o_c_u_m_e_n_t_a_t_i_o_n and get started in minutes.
  [![pypi](https://img.shields.io/pypi/v/inngest.svg)](https://pypi.python.org/
 pypi/inngest) ![versions](https://img.shields.io/pypi/pyversions/inngest.svg)
  [![discord](https://img.shields.io/discord/842170679536517141?label=discord)]
  (https://www.inngest.com/discord) [![twitter](https://img.shields.io/twitter/
           follow/inngest?style=social)](https://twitter.com/inngest)
 ===============================================================================
-# Inngest Python SDK > ð§ Currently in beta! Users have deployed our Python
-SDK in their production environments but it isn't as battle-tested as our
-TypeScript SDK. We currently support the following frameworks (but adding a new
-framework is easy!): - Django (`>=4.2`) - FastAPI (`>=0.100.0`) - Flask
-(`>=2.3.0`) - Tornado (`>=6.3`) Python 3.9 is the minimum version we support.
-## Getting started Install `inngest` in your project: ```sh pip install inngest
-``` Write a basic function and serve it (see the [basic](#basic-no-steps)
-example for guidance). Start the Dev Server (the local version of our cloud
-platform): ```sh npx inngest-cli@latest dev ``` Browse to http://127.0.0.1:8288
-and you should see your app! Visit our docs to read more about the [Dev Server]
-(https://www.inngest.com/docs/local-development). ## Examples > ð¡ You can
-mix `async` and non-`async` functions in the same app! - [Basic](#basic-no-
-steps) - [Step run](#step-run) - [Async function](#async-function) ### Basic
-(no steps) This is a minimal example of an Inngest function. It's missing some
-of our features but it's a good starting point. ```py import flask import
-inngest.flask import requests inngest_client = inngest.Inngest
-( app_id="flask_example", is_production=False, )
+# Inngest Python SDK We currently support the following frameworks (but adding
+a new framework is easy!): - DigitalOcean Functions - Django (`>=4.2`) -
+FastAPI (`>=0.100.0`) - Flask (`>=2.3.0`) - Tornado (`>=6.3`) Python 3.9 is the
+minimum version we support. ## Getting started Install `inngest` in your
+project: ```sh pip install inngest ``` Write a basic function and serve it (see
+the [basic](#basic-no-steps) example for guidance). Start the Dev Server (the
+local version of our cloud platform): ```sh npx inngest-cli@latest dev ```
+Browse to http://127.0.0.1:8288 and you should see your app! Visit our docs to
+read more about the [Dev Server](https://www.inngest.com/docs/local-
+development). ## Examples > ð¡ You can mix `async` and non-`async` functions
+in the same app! - [Basic](#basic-no-steps) - [Step run](#step-run) - [Async
+function](#async-function) ### Basic (no steps) This is a minimal example of an
+Inngest function. It's missing some of our features but it's a good starting
+point. ```py import flask import inngest.flask import requests inngest_client =
+inngest.Inngest( app_id="flask_example", is_production=False, )
 @inngest_client.create_function( fn_id="find_person",
 trigger=inngest.TriggerEvent(event="app/person.find"), ) def fetch_person( ctx:
 inngest.Context, step: inngest.StepSync, ) -> dict: person_id = ctx.event.data
 ["person_id"] res = requests.get(f"https://swapi.dev/api/people/{person_id}")
 return res.json() app = flask.Flask(__name__) # Register functions with the
 Inngest server inngest.flask.serve( app, inngest_client, [fetch_person], )
 app.run(port=8000) ``` Send the following event in the Dev Server UI and the
@@ -64,16 +64,16 @@
 trigger=inngest.TriggerEvent(event="app/ships.find"), ) def fetch_ships( ctx:
 inngest.Context, step: inngest.StepSync, ) -> dict: """ Find all the ships a
 person has. """ person_id = ctx.event.data["person_id"] def _fetch_person() -
 > dict: res = requests.get(f"https://swapi.dev/api/people/{person_id}") return
 res.json() # Wrap the function with step.run to enable retries person =
 step.run("fetch_person", _fetch_person) def _fetch_ship(url: str) -> dict: res
 = requests.get(url) return res.json() ship_names = [] for ship_url in person
-["starships"]: # step.run works in loops! ship = step.run("fetch_ship", lambda:
-_fetch_ship(ship_url)) ship_names.append(ship["name"]) return { "person_name":
+["starships"]: # step.run works in loops! ship = step.run("fetch_ship",
+_fetch_ship, ship_url) ship_names.append(ship["name"]) return { "person_name":
 person["name"], "ship_names": ship_names, } ``` Send the following event in the
 Dev Server UI and the `fetch_person` function will run: ```json { "name": "app/
 ships.find", "data": { "person_id": 1 } } ``` ### Async function ```py
 @inngest_client.create_function( fn_id="find_person",
 trigger=inngest.TriggerEvent(event="app/person.find"), ) async def fetch_person
 ( ctx: inngest.Context, step: inngest.Step, ) -> dict: person_id =
 ctx.event.data["person_id"] async with httpx.AsyncClient() as client: res =
```

### Comparing `inngest-0.3.9/README.md` & `inngest-0.4.0a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,17 @@
   </p>
 </div>
 
 <hr />
 
 # Inngest Python SDK
 
-> 🚧 Currently in beta! Users have deployed our Python SDK in their production environments but it isn't as battle-tested as our TypeScript SDK.
-
 We currently support the following frameworks (but adding a new framework is easy!):
 
+- DigitalOcean Functions
 - Django (`>=4.2`)
 - FastAPI (`>=0.100.0`)
 - Flask (`>=2.3.0`)
 - Tornado (`>=6.3`)
 
 Python 3.9 is the minimum version we support.
 
@@ -143,15 +142,15 @@
     def _fetch_ship(url: str) -> dict:
         res = requests.get(url)
         return res.json()
 
     ship_names = []
     for ship_url in person["starships"]:
         # step.run works in loops!
-        ship = step.run("fetch_ship", lambda: _fetch_ship(ship_url))
+        ship = step.run("fetch_ship", _fetch_ship, ship_url)
 
         ship_names.append(ship["name"])
 
     return {
         "person_name": person["name"],
         "ship_names": ship_names,
     }
```

#### html2text {}

```diff
@@ -7,31 +7,29 @@
               Read the _d_o_c_u_m_e_n_t_a_t_i_o_n and get started in minutes.
  [![pypi](https://img.shields.io/pypi/v/inngest.svg)](https://pypi.python.org/
 pypi/inngest) ![versions](https://img.shields.io/pypi/pyversions/inngest.svg)
  [![discord](https://img.shields.io/discord/842170679536517141?label=discord)]
  (https://www.inngest.com/discord) [![twitter](https://img.shields.io/twitter/
           follow/inngest?style=social)](https://twitter.com/inngest)
 ===============================================================================
-# Inngest Python SDK > ð§ Currently in beta! Users have deployed our Python
-SDK in their production environments but it isn't as battle-tested as our
-TypeScript SDK. We currently support the following frameworks (but adding a new
-framework is easy!): - Django (`>=4.2`) - FastAPI (`>=0.100.0`) - Flask
-(`>=2.3.0`) - Tornado (`>=6.3`) Python 3.9 is the minimum version we support.
-## Getting started Install `inngest` in your project: ```sh pip install inngest
-``` Write a basic function and serve it (see the [basic](#basic-no-steps)
-example for guidance). Start the Dev Server (the local version of our cloud
-platform): ```sh npx inngest-cli@latest dev ``` Browse to http://127.0.0.1:8288
-and you should see your app! Visit our docs to read more about the [Dev Server]
-(https://www.inngest.com/docs/local-development). ## Examples > ð¡ You can
-mix `async` and non-`async` functions in the same app! - [Basic](#basic-no-
-steps) - [Step run](#step-run) - [Async function](#async-function) ### Basic
-(no steps) This is a minimal example of an Inngest function. It's missing some
-of our features but it's a good starting point. ```py import flask import
-inngest.flask import requests inngest_client = inngest.Inngest
-( app_id="flask_example", is_production=False, )
+# Inngest Python SDK We currently support the following frameworks (but adding
+a new framework is easy!): - DigitalOcean Functions - Django (`>=4.2`) -
+FastAPI (`>=0.100.0`) - Flask (`>=2.3.0`) - Tornado (`>=6.3`) Python 3.9 is the
+minimum version we support. ## Getting started Install `inngest` in your
+project: ```sh pip install inngest ``` Write a basic function and serve it (see
+the [basic](#basic-no-steps) example for guidance). Start the Dev Server (the
+local version of our cloud platform): ```sh npx inngest-cli@latest dev ```
+Browse to http://127.0.0.1:8288 and you should see your app! Visit our docs to
+read more about the [Dev Server](https://www.inngest.com/docs/local-
+development). ## Examples > ð¡ You can mix `async` and non-`async` functions
+in the same app! - [Basic](#basic-no-steps) - [Step run](#step-run) - [Async
+function](#async-function) ### Basic (no steps) This is a minimal example of an
+Inngest function. It's missing some of our features but it's a good starting
+point. ```py import flask import inngest.flask import requests inngest_client =
+inngest.Inngest( app_id="flask_example", is_production=False, )
 @inngest_client.create_function( fn_id="find_person",
 trigger=inngest.TriggerEvent(event="app/person.find"), ) def fetch_person( ctx:
 inngest.Context, step: inngest.StepSync, ) -> dict: person_id = ctx.event.data
 ["person_id"] res = requests.get(f"https://swapi.dev/api/people/{person_id}")
 return res.json() app = flask.Flask(__name__) # Register functions with the
 Inngest server inngest.flask.serve( app, inngest_client, [fetch_person], )
 app.run(port=8000) ``` Send the following event in the Dev Server UI and the
@@ -43,16 +41,16 @@
 trigger=inngest.TriggerEvent(event="app/ships.find"), ) def fetch_ships( ctx:
 inngest.Context, step: inngest.StepSync, ) -> dict: """ Find all the ships a
 person has. """ person_id = ctx.event.data["person_id"] def _fetch_person() -
 > dict: res = requests.get(f"https://swapi.dev/api/people/{person_id}") return
 res.json() # Wrap the function with step.run to enable retries person =
 step.run("fetch_person", _fetch_person) def _fetch_ship(url: str) -> dict: res
 = requests.get(url) return res.json() ship_names = [] for ship_url in person
-["starships"]: # step.run works in loops! ship = step.run("fetch_ship", lambda:
-_fetch_ship(ship_url)) ship_names.append(ship["name"]) return { "person_name":
+["starships"]: # step.run works in loops! ship = step.run("fetch_ship",
+_fetch_ship, ship_url) ship_names.append(ship["name"]) return { "person_name":
 person["name"], "ship_names": ship_names, } ``` Send the following event in the
 Dev Server UI and the `fetch_person` function will run: ```json { "name": "app/
 ships.find", "data": { "person_id": 1 } } ``` ### Async function ```py
 @inngest_client.create_function( fn_id="find_person",
 trigger=inngest.TriggerEvent(event="app/person.find"), ) async def fetch_person
 ( ctx: inngest.Context, step: inngest.Step, ) -> dict: person_id =
 ctx.event.data["person_id"] async with httpx.AsyncClient() as client: res =
```

### Comparing `inngest-0.3.9/inngest/_internal/client_lib.py` & `inngest-0.4.0a0/inngest/_internal/client_lib/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,41 +4,34 @@
 import os
 import time
 import typing
 import urllib.parse
 
 import httpx
 
-from . import (
+from inngest._internal import (
     const,
     env_lib,
     errors,
     event_lib,
     function,
     function_config,
+    middleware_lib,
     net,
     types,
 )
 
-if typing.TYPE_CHECKING:
-    from . import middleware_lib
-
+from . import models
 
 # Dummy value
 _DEV_SERVER_EVENT_KEY = "NO_EVENT_KEY_SET"
 
 
 class Inngest:
-    middleware: list[
-        type[
-            typing.Union[
-                middleware_lib.Middleware, middleware_lib.MiddlewareSync
-            ]
-        ]
-    ]
+    middleware: list[middleware_lib.UninitializedMiddleware]
 
     @property
     def api_origin(self) -> str:
         return self._api_origin
 
     @property
     def env(self) -> typing.Optional[str]:
@@ -67,21 +60,15 @@
         app_id: str,
         env: typing.Optional[str] = None,
         event_api_base_url: typing.Optional[str] = None,
         event_key: typing.Optional[str] = None,
         is_production: typing.Optional[bool] = None,
         logger: typing.Optional[types.Logger] = None,
         middleware: typing.Optional[
-            list[
-                type[
-                    typing.Union[
-                        middleware_lib.Middleware, middleware_lib.MiddlewareSync
-                    ]
-                ]
-            ]
+            list[middleware_lib.UninitializedMiddleware]
         ] = None,
         signing_key: typing.Optional[str] = None,
     ) -> None:
         """
         Args:
         ----
             api_base_url: Origin for the Inngest REST API.
@@ -144,14 +131,17 @@
         if event_origin is None:
             if self._mode == const.ServerKind.DEV_SERVER:
                 event_origin = const.DEV_SERVER_ORIGIN
             else:
                 event_origin = const.DEFAULT_EVENT_ORIGIN
         self._event_api_origin = event_origin
 
+        self._http_client = net.ThreadAwareAsyncHTTPClient().initialize()
+        self._http_client_sync = httpx.Client()
+
     def _build_send_request(
         self,
         events: list[event_lib.Event],
     ) -> types.MaybeError[httpx.Request]:
         event_key: str
         if self._event_key is not None:
             event_key = self._event_key
@@ -184,48 +174,38 @@
 
             if d.get("id") == "":
                 del d["id"]
             if d.get("ts") == 0:
                 d["ts"] = int(time.time() * 1000)
             body.append(d)
 
-        return httpx.Client().build_request(
+        return self._http_client_sync.build_request(
             "POST",
             url,
             headers=headers,
             json=body,
             timeout=30,
         )
 
     def add_middleware(
         self,
-        middleware: type[
-            typing.Union[
-                middleware_lib.Middleware, middleware_lib.MiddlewareSync
-            ]
-        ],
+        middleware: middleware_lib.UninitializedMiddleware,
     ) -> None:
         self.middleware = [*self.middleware, middleware]
 
     def create_function(
         self,
         *,
         batch_events: typing.Optional[function_config.Batch] = None,
         cancel: typing.Optional[list[function_config.Cancel]] = None,
         concurrency: typing.Optional[list[function_config.Concurrency]] = None,
         debounce: typing.Optional[function_config.Debounce] = None,
         fn_id: str,
         middleware: typing.Optional[
-            list[
-                type[
-                    typing.Union[
-                        middleware_lib.Middleware, middleware_lib.MiddlewareSync
-                    ]
-                ]
-            ]
+            list[middleware_lib.UninitializedMiddleware]
         ] = None,
         name: typing.Optional[str] = None,
         on_failure: typing.Union[
             function.FunctionHandlerAsync, function.FunctionHandlerSync, None
         ] = None,
         rate_limit: typing.Optional[function_config.RateLimit] = None,
         retries: typing.Optional[int] = None,
@@ -298,54 +278,53 @@
         return decorator
 
     async def _get(self, url: str) -> httpx.Response:
         """
         Perform an asynchronous HTTP GET request. Handles authn
         """
 
-        req = httpx.Client().build_request(
+        req = self._http_client_sync.build_request(
             "GET",
             url,
             headers=net.create_headers(
                 env=self._env,
                 framework=None,
                 server_kind=None,
             ),
         )
 
-        async with httpx.AsyncClient() as client:
-            return await net.fetch_with_auth_fallback(
-                client,
-                req,
-                signing_key=self._signing_key,
-                signing_key_fallback=self._signing_key_fallback,
-            )
+        return await net.fetch_with_auth_fallback(
+            self._http_client,
+            self._http_client_sync,
+            req,
+            signing_key=self._signing_key,
+            signing_key_fallback=self._signing_key_fallback,
+        )
 
     def _get_sync(self, url: str) -> httpx.Response:
         """
         Perform a synchronous HTTP GET request. Handles authn
         """
 
-        req = httpx.Client().build_request(
+        req = self._http_client_sync.build_request(
             "GET",
             url,
             headers=net.create_headers(
                 env=self._env,
                 framework=None,
                 server_kind=None,
             ),
         )
 
-        with httpx.Client() as client:
-            return net.fetch_with_auth_fallback_sync(
-                client,
-                req,
-                signing_key=self._signing_key,
-                signing_key_fallback=self._signing_key_fallback,
-            )
+        return net.fetch_with_auth_fallback_sync(
+            self._http_client_sync,
+            req,
+            signing_key=self._signing_key,
+            signing_key_fallback=self._signing_key_fallback,
+        )
 
     async def _get_batch(self, run_id: str) -> list[event_lib.Event]:
         """
         Fetch a batch of events from the API
         """
 
         url = urllib.parse.urljoin(
@@ -408,66 +387,113 @@
             raise errors.BodyInvalidError("step data is not an object")
 
         return data
 
     async def send(
         self,
         events: typing.Union[event_lib.Event, list[event_lib.Event]],
+        *,
+        skip_middleware: bool = False,
     ) -> list[str]:
         """
         Send one or more events. This method is asynchronous.
 
         Args:
         ----
             events: An event or list of events to send.
+            skip_middleware: Whether to skip middleware.
         """
 
         if not isinstance(events, list):
             events = [events]
 
-        async with httpx.AsyncClient() as client:
-            req = self._build_send_request(events)
-            if isinstance(req, Exception):
-                raise req
-            return _extract_ids((await client.send(req)).json())
+        middleware = None
+        if not skip_middleware:
+            middleware = middleware_lib.MiddlewareManager.from_client(
+                self,
+                raw_request=None,
+            )
+            await middleware.before_send_events(events)
+
+        req = self._build_send_request(events)
+        if isinstance(req, Exception):
+            raise req
+
+        result = models.SendEventsResult.from_raw(
+            (
+                await net.fetch_with_thready_safety(
+                    self._http_client,
+                    self._http_client_sync,
+                    req,
+                )
+            ).json()
+        )
+        if isinstance(result, Exception):
+            raise result
+
+        if middleware is not None:
+            err = await middleware.after_send_events(result)
+            if isinstance(err, Exception):
+                raise err
+
+        if result.error is not None:
+            raise errors.SendEventsError(result.error, result.ids)
+
+        return result.ids
 
     def send_sync(
         self,
         events: typing.Union[event_lib.Event, list[event_lib.Event]],
+        *,
+        skip_middleware: bool = False,
     ) -> list[str]:
         """
         Send one or more events. This method is synchronous.
 
         Args:
         ----
             events: An event or list of events to send.
+            skip_middleware: Whether to skip middleware.
         """
 
         if not isinstance(events, list):
             events = [events]
 
-        with httpx.Client() as client:
-            req = self._build_send_request(events)
-            if isinstance(req, Exception):
-                raise req
-            return _extract_ids((client.send(req)).json())
+        middleware = None
+        if not skip_middleware:
+            middleware = middleware_lib.MiddlewareManager.from_client(
+                self,
+                raw_request=None,
+            )
+            err = middleware.before_send_events_sync(events)
+            if isinstance(err, Exception):
+                raise err
 
-    def set_logger(self, logger: types.Logger) -> None:
-        self.logger = logger
+        req = self._build_send_request(events)
+        if isinstance(req, Exception):
+            raise req
+
+        result = models.SendEventsResult.from_raw(
+            (self._http_client_sync.send(req)).json(),
+        )
+        if isinstance(result, Exception):
+            raise result
 
+        if middleware is not None:
+            err = middleware.after_send_events_sync(result)
+            if isinstance(err, Exception):
+                raise err
 
-def _extract_ids(body: object) -> list[str]:
-    if not isinstance(body, dict) or "ids" not in body:
-        raise errors.BodyInvalidError("unexpected response when sending events")
-
-    ids = body["ids"]
-    if not isinstance(ids, list):
-        raise errors.BodyInvalidError("unexpected response when sending events")
+        if result.error is not None:
+            raise errors.SendEventsError(result.error, result.ids)
 
-    return ids
+        return result.ids
+
+    def set_logger(self, logger: types.Logger) -> None:
+        self.logger = logger
 
 
 def _get_mode(
     logger: types.Logger,
     is_production: typing.Optional[bool],
 ) -> const.ServerKind:
     if is_production is not None:
```

### Comparing `inngest-0.3.9/inngest/_internal/client_lib_test.py` & `inngest-0.4.0a0/inngest/_internal/client_lib/client_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import unittest
 
 import pytest
 
-from . import client_lib, const, errors, event_lib
+from inngest._internal import client_lib, const, errors, event_lib
 
 
 class Test(unittest.TestCase):
     def test_dev_env_var(self) -> None:
         """
         No error is raised when the INNGEST_DEV environment variable is set.
         This env var is a fallback for the is_production param.
```

### Comparing `inngest-0.3.9/inngest/_internal/comm.py` & `inngest-0.4.0a0/inngest/_internal/comm.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,89 @@
     errors,
     execution,
     function,
     function_config,
     middleware_lib,
     net,
     registration,
+    step_lib,
     transforms,
     types,
 )
 
 
+class _ErrorData(types.BaseModel):
+    code: const.ErrorCode
+    message: str
+    name: str
+    stack: typing.Optional[str]
+
+    @classmethod
+    def from_error(cls, err: Exception) -> _ErrorData:
+        if isinstance(err, errors.Error):
+            code = err.code
+            message = err.message
+            name = err.name
+            stack = err.stack
+        else:
+            code = const.ErrorCode.UNKNOWN
+            message = str(err)
+            name = type(err).__name__
+            stack = transforms.get_traceback(err)
+
+        return cls(
+            code=code,
+            message=message,
+            name=name,
+            stack=stack,
+        )
+
+
+def _prep_call_result(
+    call_res: execution.CallResult,
+) -> types.MaybeError[object]:
+    """
+    Convert a CallResult to the shape the Inngest Server expects. For step-level
+    results this is a dict and for function-level results this is the output or
+    error.
+    """
+
+    if call_res.step is not None:
+        d = call_res.step.to_dict()
+        if isinstance(d, Exception):
+            # Unreachable
+            return d
+    else:
+        d = {}
+
+    if call_res.error is not None:
+        e = _ErrorData.from_error(call_res.error).to_dict()
+        if isinstance(e, Exception):
+            return e
+        d["error"] = e
+
+    if call_res.output is not types.empty_sentinel:
+        err = transforms.dump_json(call_res.output)
+        if isinstance(err, Exception):
+            msg = "returned unserializable data"
+            if call_res.step is not None:
+                msg = f'"{call_res.step.display_name}" {msg}'
+
+            return errors.OutputUnserializableError(msg)
+
+        d["data"] = call_res.output
+
+    is_function_level = call_res.step is None
+    if is_function_level:
+        # Don't nest function-level results
+        return d.get("error") or d.get("data")
+
+    return d
+
+
 class CommResponse:
     def __init__(
         self,
         *,
         body: object = None,
         headers: typing.Optional[dict[str, str]] = None,
         status_code: int = http.HTTPStatus.OK.value,
@@ -41,67 +111,51 @@
         logger: types.Logger,
         call_res: execution.CallResult,
     ) -> CommResponse:
         headers = {
             const.HeaderKey.SERVER_TIMING.value: "handler",
         }
 
-        if execution.is_step_call_responses(call_res):
-            out: list[dict[str, object]] = []
-            for item in call_res:
-                d = item.to_dict()
+        if call_res.multi:
+            multi_body: list[object] = []
+            for item in call_res.multi:
+                d = _prep_call_result(item)
                 if isinstance(d, Exception):
-                    return cls.from_error(
-                        logger,
-                        errors.OutputUnserializableError(
-                            f'"{item.display_name}" returned unserializable data'
-                        ),
-                    )
-
-                # Unnest data and error fields to work with the StepRun opcode.
-                # They should probably be unnested lower in the code, but this
-                # is a quick fix that doesn't break middleware contracts
-                nested_data = d.get("data")
-                if isinstance(nested_data, dict):
-                    d["data"] = nested_data.get("data")
-                    d["error"] = nested_data.get("error")
+                    return cls.from_error(logger, d)
+                multi_body.append(d)
 
-                out.append(d)
+                if item.error is not None:
+                    if errors.is_retriable(item.error) is False:
+                        headers[const.HeaderKey.NO_RETRY.value] = "true"
 
             return cls(
-                body=transforms.prep_body(out),
+                body=multi_body,
                 headers=headers,
                 status_code=http.HTTPStatus.PARTIAL_CONTENT.value,
             )
 
-        if isinstance(call_res, execution.CallError):
-            logger.error(call_res.stack)
-
-            d = call_res.to_dict()
-            if isinstance(d, Exception):
-                return cls.from_error(logger, d)
+        body = _prep_call_result(call_res)
+        status_code = http.HTTPStatus.OK.value
+        if isinstance(body, Exception):
+            return cls.from_error(logger, body)
 
-            if call_res.is_retriable is False:
+        if call_res.error is not None:
+            status_code = http.HTTPStatus.INTERNAL_SERVER_ERROR.value
+            if errors.is_retriable(call_res.error) is False:
                 headers[const.HeaderKey.NO_RETRY.value] = "true"
 
-            return cls(
-                body=transforms.prep_body(d),
-                headers=headers,
-                status_code=http.HTTPStatus.INTERNAL_SERVER_ERROR.value,
-            )
+            if isinstance(call_res.error, errors.RetryAfterError):
+                headers[
+                    const.HeaderKey.RETRY_AFTER.value
+                ] = transforms.to_iso_utc(call_res.error.retry_after)
 
-        if isinstance(call_res, execution.FunctionCallResponse):
-            return cls(
-                body=call_res.data,
-                headers=headers,
-            )
-
-        return cls.from_error(
-            logger,
-            errors.UnknownError("unknown call result"),
+        return cls(
+            body=body,
+            headers=headers,
+            status_code=status_code,
         )
 
     @classmethod
     def from_error(
         cls,
         logger: types.Logger,
         err: Exception,
@@ -109,15 +163,16 @@
     ) -> CommResponse:
         code: typing.Optional[str] = None
         if isinstance(err, errors.Error):
             code = err.code.value
         else:
             code = const.ErrorCode.UNKNOWN.value
 
-        logger.error(f"{code}: {err!s}")
+        if errors.is_quiet(err) is False:
+            logger.error(f"{code}: {err!s}")
 
         return cls(
             body={
                 "code": code,
                 "message": str(err),
                 "name": type(err).__name__,
             },
@@ -223,158 +278,162 @@
             server_kind=server_kind,
         )
 
         params = {}
         if sync_id is not None:
             params[const.QueryParamKey.SYNC_ID.value] = sync_id
 
-        return httpx.Client().build_request(
+        return self._client._http_client_sync.build_request(
             "POST",
             registration_url,
             headers=headers,
-            json=transforms.prep_body(body),
+            json=transforms.deep_strip_none(body),
             params=params,
             timeout=30,
         )
 
     async def call_function(
         self,
         *,
         call: execution.Call,
         fn_id: str,
+        raw_request: object,
         req_sig: net.RequestSignature,
         target_hashed_id: str,
     ) -> CommResponse:
         """Handle a function call from the Executor."""
 
         if target_hashed_id == execution.UNSPECIFIED_STEP_ID:
             target_step_id = None
         else:
             target_step_id = target_hashed_id
 
-        middleware = middleware_lib.MiddlewareManager.from_client(self._client)
+        middleware = middleware_lib.MiddlewareManager.from_client(
+            self._client,
+            raw_request,
+        )
 
         # Validate the request signature.
         err = req_sig.validate(
             signing_key=self._signing_key,
             signing_key_fallback=self._signing_key_fallback,
         )
         if isinstance(err, Exception):
-            return await self._respond(middleware, err)
+            return await self._respond(err)
 
         # Get the function we should call.
         fn = self._get_function(fn_id)
         if isinstance(fn, Exception):
-            return await self._respond(middleware, fn)
+            return await self._respond(fn)
 
         events = call.events
         steps = call.steps
         if call.use_api:
             # Putting the batch and memoized steps in the request would make it
             # to big, so the Executor is telling the SDK to fetch them from the
             # API
 
             try:
                 events, steps = await asyncio.gather(
                     self._client._get_batch(call.ctx.run_id),
                     self._client._get_steps(call.ctx.run_id),
                 )
             except Exception as err:
-                return await self._respond(middleware, err)
+                return await self._respond(err)
         if events is None:
             # Should be unreachable. The Executor should always either send the
             # batch or tell the SDK to fetch the batch
 
-            return await self._respond(
-                middleware, Exception("events not in request")
-            )
+            return await self._respond(Exception("events not in request"))
 
         call_res = await fn.call(
             self._client,
             function.Context(
                 attempt=call.ctx.attempt,
                 event=call.event,
                 events=events,
                 logger=self._client.logger,
                 run_id=call.ctx.run_id,
             ),
             fn_id,
             middleware,
-            steps,
+            step_lib.StepMemos.from_raw(steps),
             target_step_id,
         )
 
-        return await self._respond(middleware, call_res)
+        return await self._respond(call_res)
 
     def call_function_sync(
         self,
         *,
         call: execution.Call,
         fn_id: str,
+        raw_request: object,
         req_sig: net.RequestSignature,
         target_hashed_id: str,
     ) -> CommResponse:
         """Handle a function call from the Executor."""
 
         if target_hashed_id == execution.UNSPECIFIED_STEP_ID:
             target_step_id = None
         else:
             target_step_id = target_hashed_id
 
-        middleware = middleware_lib.MiddlewareManager.from_client(self._client)
+        middleware = middleware_lib.MiddlewareManager.from_client(
+            self._client,
+            raw_request,
+        )
 
         # Validate the request signature.
         err = req_sig.validate(
             signing_key=self._signing_key,
             signing_key_fallback=self._signing_key_fallback,
         )
         if isinstance(err, Exception):
-            return self._respond_sync(middleware, err)
+            return self._respond_sync(err)
 
         # Get the function we should call.
         fn = self._get_function(fn_id)
         if isinstance(fn, Exception):
-            return self._respond_sync(middleware, fn)
+            return self._respond_sync(fn)
 
         events = call.events
         steps = call.steps
         if call.use_api:
             # Putting the batch and memoized steps in the request would make it
             # to big, so the Executor is telling the SDK to fetch them from the
             # API
 
             try:
                 events = self._client._get_batch_sync(call.ctx.run_id)
                 steps = self._client._get_steps_sync(call.ctx.run_id)
             except Exception as err:
-                return self._respond_sync(middleware, err)
+                return self._respond_sync(err)
         if events is None:
             # Should be unreachable. The Executor should always either send the
             # batch or tell the SDK to fetch the batch
 
-            return self._respond_sync(
-                middleware, Exception("events not in request")
-            )
+            return self._respond_sync(Exception("events not in request"))
 
         call_res = fn.call_sync(
             self._client,
             function.Context(
                 attempt=call.ctx.attempt,
                 event=call.event,
                 events=events,
                 logger=self._client.logger,
                 run_id=call.ctx.run_id,
             ),
             fn_id,
             middleware,
-            steps,
+            step_lib.StepMemos.from_raw(steps),
             target_step_id,
         )
 
-        return self._respond_sync(middleware, call_res)
+        return self._respond_sync(call_res)
 
     def _get_function(self, fn_id: str) -> types.MaybeError[function.Function]:
         # Look for the function ID in the list of user functions, but also
         # look for it in the list of on_failure functions.
         for _fn in self._fns.values():
             if _fn.get_id() == fn_id:
                 return _fn
@@ -409,16 +468,19 @@
 
         if len(configs) == 0:
             return errors.FunctionConfigInvalidError("no functions found")
         return configs
 
     def inspect(
         self,
-        server_kind: typing.Optional[const.ServerKind],
+        *,
         req_sig: net.RequestSignature,
+        serve_origin: typing.Optional[str],
+        serve_path: typing.Optional[str],
+        server_kind: typing.Optional[const.ServerKind],
     ) -> CommResponse:
         """Handle Dev Server's auto-discovery."""
 
         if server_kind is not None and server_kind != self._mode:
             # Tell Dev Server to leave the app alone since it's in production
             # mode.
             return CommResponse(
@@ -428,39 +490,63 @@
             )
 
         # Validate the request signature.
         err = req_sig.validate(
             signing_key=self._signing_key,
             signing_key_fallback=self._signing_key_fallback,
         )
-        if isinstance(err, Exception):
-            body = _InsecureInspection(
+        if self._client._mode != const.ServerKind.CLOUD or isinstance(
+            err, Exception
+        ):
+            authentication_succeeded = None
+            if isinstance(err, Exception):
+                authentication_succeeded = False
+
+            body = _UnauthenticatedIntrospection(
+                authentication_succeeded=authentication_succeeded,
                 function_count=len(self._fns),
                 has_event_key=self._client.event_key is not None,
                 has_signing_key=self._signing_key is not None,
+                has_signing_key_fallback=self._signing_key_fallback is not None,
                 mode=self._mode,
             )
         else:
+            event_key_hash = (
+                transforms.hash_event_key(self._client.event_key)
+                if self._client.event_key
+                else None
+            )
+
             signing_key_hash = (
                 transforms.hash_signing_key(self._signing_key)
                 if self._signing_key
                 else None
             )
 
             signing_key_fallback_hash = (
                 transforms.hash_signing_key(self._signing_key_fallback)
                 if self._signing_key_fallback
                 else None
             )
 
-            body = _SecureInspection(
+            body = _AuthenticatedIntrospection(
+                api_origin=self._client.api_origin,
+                app_id=self._client.app_id,
+                authentication_succeeded=True,
+                env=self._client.env,
+                event_api_origin=self._client.event_api_origin,
+                event_key_hash=event_key_hash,
+                framework=self._framework.value,
                 function_count=len(self._fns),
                 has_event_key=self._client.event_key is not None,
                 has_signing_key=self._signing_key is not None,
+                has_signing_key_fallback=self._signing_key_fallback is not None,
                 mode=self._mode,
+                serve_origin=serve_origin,
+                serve_path=serve_path,
                 signing_key_fallback_hash=signing_key_fallback_hash,
                 signing_key_hash=signing_key_hash,
             )
 
         body_json = body.to_dict()
         if isinstance(body, Exception):
             body_json = {
@@ -518,15 +604,15 @@
         return comm_res
 
     async def register(
         self,
         *,
         app_url: str,
         server_kind: typing.Optional[const.ServerKind],
-        sync_id: typing.Optional[str] = None,
+        sync_id: typing.Optional[str],
     ) -> CommResponse:
         """Handle a registration call."""
 
         comm_res = self._validate_registration(server_kind)
         if comm_res is not None:
             return comm_res
 
@@ -534,26 +620,26 @@
             app_url=app_url,
             server_kind=server_kind,
             sync_id=sync_id,
         )
         if isinstance(req, Exception):
             return CommResponse.from_error(self._client.logger, req)
 
-        async with httpx.AsyncClient() as client:
-            res = await net.fetch_with_auth_fallback(
-                client,
-                req,
-                signing_key=self._signing_key,
-                signing_key_fallback=self._signing_key_fallback,
-            )
+        res = await net.fetch_with_auth_fallback(
+            self._client._http_client,
+            self._client._http_client_sync,
+            req,
+            signing_key=self._signing_key,
+            signing_key_fallback=self._signing_key_fallback,
+        )
 
-            return self._parse_registration_response(
-                res,
-                server_kind,
-            )
+        return self._parse_registration_response(
+            res,
+            server_kind,
+        )
 
     def register_sync(
         self,
         *,
         app_url: str,
         server_kind: typing.Optional[const.ServerKind],
         sync_id: typing.Optional[str],
@@ -568,50 +654,39 @@
             app_url=app_url,
             server_kind=server_kind,
             sync_id=sync_id,
         )
         if isinstance(req, Exception):
             return CommResponse.from_error(self._client.logger, req)
 
-        with httpx.Client() as client:
-            res = net.fetch_with_auth_fallback_sync(
-                client,
-                req,
-                signing_key=self._signing_key,
-                signing_key_fallback=self._signing_key_fallback,
-            )
+        res = net.fetch_with_auth_fallback_sync(
+            self._client._http_client_sync,
+            req,
+            signing_key=self._signing_key,
+            signing_key_fallback=self._signing_key_fallback,
+        )
 
-            return self._parse_registration_response(
-                res,
-                server_kind,
-            )
+        return self._parse_registration_response(
+            res,
+            server_kind,
+        )
 
     async def _respond(
         self,
-        middleware: middleware_lib.MiddlewareManager,
         value: typing.Union[execution.CallResult, Exception],
     ) -> CommResponse:
-        err = await middleware.before_response()
-        if isinstance(err, Exception):
-            return CommResponse.from_error(self._client.logger, err)
-
         if isinstance(value, Exception):
             return CommResponse.from_error(self._client.logger, value)
 
         return CommResponse.from_call_result(self._client.logger, value)
 
     def _respond_sync(
         self,
-        middleware: middleware_lib.MiddlewareManager,
         value: typing.Union[execution.CallResult, Exception],
     ) -> CommResponse:
-        err = middleware.before_response_sync()
-        if isinstance(err, Exception):
-            return CommResponse.from_error(self._client.logger, err)
-
         if isinstance(value, Exception):
             return CommResponse.from_error(self._client.logger, value)
 
         return CommResponse.from_call_result(self._client.logger, value)
 
     def _validate_registration(
         self,
@@ -630,17 +705,32 @@
                 msg,
                 http.HTTPStatus.BAD_REQUEST,
             )
 
         return None
 
 
-class _InsecureInspection(types.BaseModel):
+class _UnauthenticatedIntrospection(types.BaseModel):
+    schema_version: str = "2024-05-24"
+
+    authentication_succeeded: typing.Optional[bool]
     function_count: int
     has_event_key: bool
     has_signing_key: bool
+    has_signing_key_fallback: bool
     mode: const.ServerKind
 
 
-class _SecureInspection(_InsecureInspection):
+class _AuthenticatedIntrospection(_UnauthenticatedIntrospection):
+    api_origin: str
+    app_id: str
+    authentication_succeeded: bool = True
+    env: typing.Optional[str]
+    event_api_origin: str
+    event_key_hash: typing.Optional[str]
+    framework: str
+    sdk_language: str = const.LANGUAGE
+    sdk_version: str = const.VERSION
+    serve_origin: typing.Optional[str]
+    serve_path: typing.Optional[str]
     signing_key_fallback_hash: typing.Optional[str]
     signing_key_hash: typing.Optional[str]
```

### Comparing `inngest-0.3.9/inngest/_internal/comm_test.py` & `inngest-0.4.0a0/inngest/_internal/comm_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.9/inngest/_internal/const.py` & `inngest-0.4.0a0/inngest/_internal/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 
 DEFAULT_API_ORIGIN: typing.Final = "https://api.inngest.com/"
 DEFAULT_EVENT_ORIGIN: typing.Final = "https://inn.gs/"
 DEV_SERVER_ORIGIN: typing.Final = "http://127.0.0.1:8288/"
 LANGUAGE: typing.Final = "py"
 ROOT_STEP_ID: typing.Final = "step"
-VERSION: typing.Final = "0.3.9"
+VERSION: typing.Final = "0.4.0a0"
 
 
 class EnvKey(enum.Enum):
     API_BASE_URL = "INNGEST_API_BASE_URL"
     DEV = "INNGEST_DEV"
     EVENT_API_BASE_URL = "INNGEST_EVENT_API_BASE_URL"
     EVENT_KEY = "INNGEST_EVENT_KEY"
@@ -41,37 +41,40 @@
     FUNCTION_CONFIG_INVALID = "function_config_invalid"
     FUNCTION_NOT_FOUND = "function_not_found"
     HEADER_MISSING = "header_missing"
     NON_RETRIABLE_ERROR = "non_retriable_error"
     OUTPUT_UNSERIALIZABLE = "output_unserializable"
     QUERY_PARAM_MISSING = "query_param_missing"
     REGISTRATION_FAILED = "registration_failed"
+    RETRY_AFTER_ERROR = "retry_after_error"
     SERVER_KIND_MISMATCH = "server_kind_mismatch"
     SIGNING_KEY_UNSPECIFIED = "signing_key_unspecified"
     SIG_VERIFICATION_FAILED = "sig_verification_failed"
     STEP_ERRORED = "step_errored"
     STEP_UNEXPECTED = "step_unexpected"
     UNKNOWN = "unknown"
     URL_INVALID = "url_invalid"
 
 
 class Framework(enum.Enum):
+    DIGITAL_OCEAN = "digitalocean"
     DJANGO = "django"
     FAST_API = "fast_api"
     FLASK = "flask"
     TORNADO = "tornado"
 
 
 class HeaderKey(enum.Enum):
     AUTHORIZATION = "Authorization"
     CONTENT_TYPE = "Content-Type"
     ENV = "X-Inngest-Env"
     EXPECTED_SERVER_KIND = "X-Inngest-Expected-Server-Kind"
     FRAMEWORK = "X-Inngest-Framework"
     NO_RETRY = "X-Inngest-No-Retry"
+    RETRY_AFTER = "Retry-After"
     SDK = "X-Inngest-SDK"
     SERVER_KIND = "X-Inngest-Server-Kind"
     SERVER_TIMING = "Server-Timing"
     SIGNATURE = "X-Inngest-Signature"
     USER_AGENT = "User-Agent"
```

### Comparing `inngest-0.3.9/inngest/_internal/env_lib.py` & `inngest-0.4.0a0/inngest/_internal/env_lib.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.9/inngest/_internal/errors.py` & `inngest-0.4.0a0/inngest/_internal/errors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import datetime
 import typing
 
 import pydantic
 
 from . import const, transforms
 
 
@@ -126,18 +127,63 @@
 
     code = const.ErrorCode.NON_RETRIABLE_ERROR
     is_retriable = False
 
     def __init__(
         self,
         message: typing.Optional[str] = None,
-        cause: typing.Optional[typing.Mapping[str, object]] = None,
+        quiet: bool = False,
     ) -> None:
         super().__init__(message)
-        self.cause = cause
+        self.quiet = quiet
+
+
+class RetryAfterError(Error):
+    code = const.ErrorCode.RETRY_AFTER_ERROR
+
+    def __init__(
+        self,
+        message: typing.Optional[str],
+        retry_after: typing.Union[int, datetime.timedelta, datetime.datetime],
+        quiet: bool = False,
+    ) -> None:
+        """
+        Raise this error to retry at a specific time.
+
+        Args:
+        ----
+            message: Error message
+            retry_after: Time to retry after in milliseconds, timedelta, or datetime
+            quiet: Whether to supress logging
+        """
+
+        super().__init__(message)
+
+        if isinstance(retry_after, int):
+            retry_after = datetime.datetime.now() + datetime.timedelta(
+                milliseconds=retry_after
+            )
+        elif isinstance(retry_after, datetime.timedelta):
+            retry_after = datetime.datetime.now() + retry_after
+
+        self.retry_after: datetime.datetime = retry_after
+        self.quiet: bool = quiet
+
+
+class SendEventsError(Error):
+    def __init__(self, message: str, ids: list[str]) -> None:
+        """
+        Args:
+        ----
+            message: Error message
+            ids: List of event IDs that successfully sent
+        """
+
+        super().__init__(message)
+        self.ids = ids
 
 
 class StepError(Error):
     """
     Wraps a userland error. This is necessary because the Executor sends
     memoized error data which can't be deserialized into the original error
     class.
@@ -186,7 +232,24 @@
             stack: Userland error's stack trace
         """
 
         super().__init__(message)
         self._message = message
         self._name = name
         self._stack = stack
+
+
+def is_retriable(err: Exception) -> bool:
+    if isinstance(err, Error):
+        return err.is_retriable
+    return True
+
+
+def is_quiet(err: Exception) -> bool:
+    if isinstance(err, _Quietable):
+        return err.quiet
+    return False
+
+
+@typing.runtime_checkable
+class _Quietable(typing.Protocol):
+    quiet: bool
```

### Comparing `inngest-0.3.9/inngest/_internal/event_lib_test.py` & `inngest-0.4.0a0/inngest/_internal/event_lib_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.9/inngest/_internal/execution.py` & `inngest-0.4.0a0/inngest/_internal/execution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
+import dataclasses
 import enum
 import typing
 
 import pydantic
 import typing_extensions
 
-from . import const, errors, event_lib, transforms, types
+from . import event_lib, transforms, types
 
 
 class Call(types.BaseModel):
     ctx: CallContext
     event: event_lib.Event
     events: typing.Optional[list[event_lib.Event]] = None
     steps: dict[str, object]
@@ -23,80 +24,35 @@
     stack: CallStack
 
 
 class CallStack(types.BaseModel):
     stack: list[str]
 
 
-class CallError(types.BaseModel):
-    """
-    When an error that occurred during a call. Used for both function- and step-level
-    errors.
-    """
-
-    code: const.ErrorCode
-    is_retriable: bool
-    message: str
-    name: str
-    original_error: object = pydantic.Field(exclude=True)
-    stack: typing.Optional[str]
-    step_id: typing.Optional[str]
-
-    @classmethod
-    def from_error(
-        cls,
-        err: Exception,
-        step_id: typing.Optional[str] = None,
-    ) -> CallError:
-        code = const.ErrorCode.UNKNOWN
-        if isinstance(err, errors.Error):
-            code = err.code
-            is_retriable = err.is_retriable
-            message = err.message
-            name = err.name
-            stack = err.stack
-        else:
-            is_retriable = True
-            message = str(err)
-            name = type(err).__name__
-            stack = transforms.get_traceback(err)
-
-        return cls(
-            code=code,
-            is_retriable=is_retriable,
-            message=message,
-            name=name,
-            original_error=err,
-            stack=stack,
-            step_id=step_id,
-        )
-
-
-class FunctionCallResponse(types.BaseModel):
-    """When a function successfully returns."""
-
-    data: object
-
-
-class StepResponse(types.BaseModel):
-    data: typing.Optional[Output] = None
+class StepInfo(types.BaseModel):
     display_name: str = pydantic.Field(..., serialization_alias="displayName")
     id: str
 
     # Deprecated
     name: typing.Optional[str] = None
 
     op: Opcode
     opts: typing.Optional[dict[str, object]] = None
 
 
+class StepResponse(types.BaseModel):
+    output: object = None
+    original_error: object = pydantic.Field(default=None, exclude=True)
+    step: StepInfo
+
+
 class MemoizedError(types.BaseModel):
     message: str
     name: str
-    stack: typing.Optional[str]
+    stack: typing.Optional[str] = None
 
     @classmethod
     def from_error(cls, err: Exception) -> MemoizedError:
         return cls(
             message=str(err),
             name=type(err).__name__,
             stack=transforms.get_traceback(err),
@@ -105,31 +61,72 @@
 
 class Output(types.BaseModel):
     # Fail validation if any extra fields exist, because this will prevent
     # accidentally assuming user data is nested data
     model_config = pydantic.ConfigDict(extra="forbid")
 
     data: object = None
-
-    # TODO: Change the type to MemoizedError. But that requires a breaking
-    # change, so do it in version 0.4
-    error: typing.Optional[dict[str, object]] = None
+    error: typing.Optional[MemoizedError] = None
 
 
 def is_step_call_responses(
     value: object,
 ) -> typing_extensions.TypeGuard[list[StepResponse]]:
     if not isinstance(value, list):
         return False
     return all(isinstance(item, StepResponse) for item in value)
 
 
-CallResult: typing_extensions.TypeAlias = typing.Union[
-    list[StepResponse], FunctionCallResponse, CallError
-]
+@dataclasses.dataclass
+class CallResult:
+    error: typing.Optional[Exception] = None
+
+    # Multiple results from a single call (only used for steps). This will only
+    # be longer than 1 for parallel steps. Otherwise, it will be 1 long for
+    # sequential steps
+    multi: typing.Optional[list[CallResult]] = None
+
+    # Need a sentinel value to differentiate between None and unset
+    output: object = types.empty_sentinel
+
+    # Step metadata (e.g. user-specified ID)
+    step: typing.Optional[StepInfo] = None
+
+    @property
+    def is_empty(self) -> bool:
+        return all(
+            [
+                self.error is None,
+                self.multi is None,
+                self.output is types.empty_sentinel,
+                self.step is None,
+            ]
+        )
+
+    @classmethod
+    def from_responses(
+        cls,
+        responses: list[StepResponse],
+    ) -> CallResult:
+        multi = []
+
+        for response in responses:
+            error = None
+            if isinstance(response.original_error, Exception):
+                error = response.original_error
+
+            multi.append(
+                cls(
+                    error=error,
+                    output=response.output,
+                    step=response.step,
+                )
+            )
+
+        return cls(multi=multi)
 
 
 class Opcode(enum.Enum):
     INVOKE = "InvokeFunction"
     PLANNED = "StepPlanned"
     SLEEP = "Sleep"
     STEP_RUN = "StepRun"
```

### Comparing `inngest-0.3.9/inngest/_internal/function.py` & `inngest-0.4.0a0/inngest/_internal/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,14 +125,22 @@
         on_failure handler.
         """
         if self._opts.on_failure is None:
             return None
         return _is_function_handler_async(self._opts.on_failure)
 
     @property
+    def local_id(self) -> str:
+        return self._opts.local_id
+
+    @property
+    def name(self) -> str:
+        return self._opts.name
+
+    @property
     def on_failure_fn_id(self) -> typing.Optional[str]:
         return self._on_failure_fn_id
 
     def __init__(
         self,
         opts: FunctionOpts,
         trigger: typing.Union[
@@ -142,266 +150,278 @@
                 typing.Union[
                     function_config.TriggerCron, function_config.TriggerEvent
                 ]
             ],
         ],
         handler: typing.Union[FunctionHandlerAsync, FunctionHandlerSync],
         middleware: typing.Optional[
-            list[
-                type[
-                    typing.Union[
-                        middleware_lib.Middleware, middleware_lib.MiddlewareSync
-                    ]
-                ]
-            ]
+            list[middleware_lib.UninitializedMiddleware]
         ] = None,
     ) -> None:
         self._handler = handler
         self._middleware = middleware or []
         self._opts = opts
         self._triggers = trigger if isinstance(trigger, list) else [trigger]
 
         if opts.on_failure is not None:
             self._on_failure_fn_id = f"{opts.fully_qualified_id}-failure"
 
-    async def call(  # noqa: C901
+    async def call(
         self,
         client: client_lib.Inngest,
         ctx: Context,
         fn_id: str,
         middleware: middleware_lib.MiddlewareManager,
-        steps: dict[str, object],
+        steps: step_lib.StepMemos,
         target_hashed_id: typing.Optional[str],
     ) -> execution.CallResult:
         middleware = middleware_lib.MiddlewareManager.from_manager(middleware)
         for m in self._middleware:
             middleware.add(m)
 
-        memos = step_lib.StepMemos.from_raw(steps)
+        # Move business logic to a private method to make it simpler to run the
+        # transform_output hook on every call result code path
+        call_res = await self._call(
+            client,
+            ctx,
+            fn_id,
+            middleware,
+            steps,
+            target_hashed_id,
+        )
+
+        err = await middleware.transform_output(call_res)
+        if isinstance(err, Exception):
+            return execution.CallResult(err)
+
+        err = await middleware.before_response()
+        if isinstance(err, Exception):
+            return execution.CallResult(err)
 
+        return call_res
+
+    async def _call(
+        self,
+        client: client_lib.Inngest,
+        ctx: Context,
+        fn_id: str,
+        middleware: middleware_lib.MiddlewareManager,
+        steps: step_lib.StepMemos,
+        target_hashed_id: typing.Optional[str],
+    ) -> execution.CallResult:
         # Give middleware the opportunity to change some of params passed to the
         # user's handler.
-        new_ctx = await middleware.transform_input(ctx)
-        if isinstance(new_ctx, Exception):
-            return execution.CallError.from_error(new_ctx)
-        ctx = new_ctx
+        middleware_err = await middleware.transform_input(ctx, self, steps)
+        if isinstance(middleware_err, Exception):
+            return execution.CallResult(middleware_err)
 
         # No memoized data means we're calling the function for the first time.
-        if memos.size == 0:
+        if steps.size == 0:
             err = await middleware.before_execution()
             if isinstance(err, Exception):
-                return execution.CallError.from_error(err)
+                return execution.CallResult(err)
 
         try:
             handler: typing.Union[FunctionHandlerAsync, FunctionHandlerSync]
             if self.id == fn_id:
                 handler = self._handler
             elif self.on_failure_fn_id == fn_id:
                 if self._opts.on_failure is None:
-                    return execution.CallError.from_error(
+                    return execution.CallResult(
                         errors.FunctionNotFoundError("on_failure not defined")
                     )
                 handler = self._opts.on_failure
             else:
-                return execution.CallError.from_error(
+                return execution.CallResult(
                     errors.FunctionNotFoundError("function ID mismatch")
                 )
 
             output: object
 
             try:
                 # # Determine whether the handler is async (i.e. if we need to await
                 # # it). Sync functions are OK in async contexts, so it's OK if the
                 # # handler is sync.
                 if _is_function_handler_async(handler):
                     output = await handler(
                         ctx=ctx,
                         step=step_lib.Step(
                             client,
-                            memos,
+                            steps,
                             middleware,
                             step_lib.StepIDCounter(),
                             target_hashed_id,
                         ),
                     )
                 elif _is_function_handler_sync(handler):
                     output = handler(
                         ctx=ctx,
                         step=step_lib.StepSync(
                             client,
-                            memos,
+                            steps,
                             middleware,
                             step_lib.StepIDCounter(),
                             target_hashed_id,
                         ),
                     )
                 else:
                     # Should be unreachable but Python's custom type guards don't
                     # support negative checks :(
-                    return execution.CallError.from_error(
+                    return execution.CallResult(
                         errors.UnknownError(
                             "unable to determine function handler type"
                         )
                     )
             except Exception as user_err:
                 transforms.remove_first_traceback_frame(user_err)
                 raise _UserError(user_err)
 
             err = await middleware.after_execution()
             if isinstance(err, Exception):
-                return execution.CallError.from_error(err)
-
-            output = await middleware.transform_output(
-                # Function output isn't wrapped in an Output object, so we need
-                # to wrap it to make it compatible with middleware.
-                execution.Output(data=output)
-            )
-            if isinstance(output, Exception):
-                return execution.CallError.from_error(output)
+                return execution.CallResult(err)
 
-            if output is None:
-                return execution.FunctionCallResponse(data=None)
-            return execution.FunctionCallResponse(data=output.data)
+            return execution.CallResult(output=output)
         except step_lib.ResponseInterrupt as interrupt:
             err = await middleware.after_execution()
             if isinstance(err, Exception):
-                return execution.CallError.from_error(err)
+                return execution.CallResult(err)
 
-            # TODO: How should transform_output work with multiple responses?
-            if len(interrupt.responses) == 1:
-                output = await middleware.transform_output(
-                    interrupt.responses[0].data
-                )
-                if isinstance(output, Exception):
-                    return execution.CallError.from_error(output)
-                interrupt.responses[0].data = output
-
-            return interrupt.responses
+            return execution.CallResult.from_responses(interrupt.responses)
         except _UserError as err:
-            return execution.CallError.from_error(err.err)
+            return execution.CallResult(err.err)
         except step_lib.SkipInterrupt as err:
             # This should only happen in a non-deterministic scenario, where
             # step targeting is enabled and an unexpected step is encountered.
             # We don't currently have a way to recover from this scenario.
 
-            return execution.CallError.from_error(
+            return execution.CallResult(
                 errors.StepUnexpectedError(
                     f'found step "{err.step_id}" when targeting a different step'
                 )
             )
         except Exception as err:
-            return execution.CallError.from_error(err)
+            return execution.CallResult(err)
 
-    def call_sync(  # noqa: C901
+    def call_sync(
         self,
         client: client_lib.Inngest,
         ctx: Context,
         fn_id: str,
         middleware: middleware_lib.MiddlewareManager,
-        steps: dict[str, object],
+        steps: step_lib.StepMemos,
         target_hashed_id: typing.Optional[str],
     ) -> execution.CallResult:
         middleware = middleware_lib.MiddlewareManager.from_manager(middleware)
         for m in self._middleware:
             middleware.add(m)
 
-        memos = step_lib.StepMemos.from_raw(steps)
+        # Move business logic to a private method to make it simpler to run the
+        # transform_output hook on every call result code path
+        call_res = self._call_sync(
+            client,
+            ctx,
+            fn_id,
+            middleware,
+            steps,
+            target_hashed_id,
+        )
+
+        err = middleware.transform_output_sync(call_res)
+        if isinstance(err, Exception):
+            return execution.CallResult(err)
+
+        err = middleware.before_response_sync()
+        if isinstance(err, Exception):
+            return execution.CallResult(err)
 
+        return call_res
+
+    def _call_sync(
+        self,
+        client: client_lib.Inngest,
+        ctx: Context,
+        fn_id: str,
+        middleware: middleware_lib.MiddlewareManager,
+        steps: step_lib.StepMemos,
+        target_hashed_id: typing.Optional[str],
+    ) -> execution.CallResult:
         # Give middleware the opportunity to change some of params passed to the
         # user's handler.
-        new_ctx = middleware.transform_input_sync(ctx)
-        if isinstance(new_ctx, Exception):
-            return execution.CallError.from_error(new_ctx)
-        ctx = new_ctx
+        middleware_err = middleware.transform_input_sync(ctx, self, steps)
+        if isinstance(middleware_err, Exception):
+            return execution.CallResult(middleware_err)
 
         # No memoized data means we're calling the function for the first time.
-        if memos.size == 0:
-            middleware.before_execution_sync()
+        if steps.size == 0:
+            err = middleware.before_execution_sync()
+            if isinstance(err, Exception):
+                return execution.CallResult(err)
 
         try:
             handler: typing.Union[FunctionHandlerAsync, FunctionHandlerSync]
             if self.id == fn_id:
                 handler = self._handler
             elif self.on_failure_fn_id == fn_id:
                 if self._opts.on_failure is None:
-                    return execution.CallError.from_error(
+                    return execution.CallResult(
                         errors.FunctionNotFoundError("on_failure not defined")
                     )
                 handler = self._opts.on_failure
             else:
-                return execution.CallError.from_error(
+                return execution.CallResult(
                     errors.FunctionNotFoundError("function ID mismatch")
                 )
 
             if _is_function_handler_sync(handler):
                 try:
                     output: object = handler(
                         ctx=ctx,
                         step=step_lib.StepSync(
                             client,
-                            memos,
+                            steps,
                             middleware,
                             step_lib.StepIDCounter(),
                             target_hashed_id,
                         ),
                     )
                 except Exception as user_err:
                     transforms.remove_first_traceback_frame(user_err)
                     raise _UserError(user_err)
             else:
-                return execution.CallError.from_error(
+                return execution.CallResult(
                     errors.AsyncUnsupportedError(
                         "encountered async function in non-async context"
                     )
                 )
 
             err = middleware.after_execution_sync()
             if isinstance(err, Exception):
-                return execution.CallError.from_error(err)
+                return execution.CallResult(err)
 
-            output = middleware.transform_output_sync(
-                # Function output isn't wrapped in an Output object, so we need
-                # to wrap it to make it compatible with middleware.
-                execution.Output(data=output)
-            )
-            if isinstance(output, Exception):
-                return execution.CallError.from_error(output)
-
-            if output is None:
-                return execution.FunctionCallResponse(data=None)
-            return execution.FunctionCallResponse(data=output.data)
+            return execution.CallResult(output=output)
         except step_lib.ResponseInterrupt as interrupt:
             err = middleware.after_execution_sync()
             if isinstance(err, Exception):
-                return execution.CallError.from_error(err)
-
-            # TODO: How should transform_output work with multiple responses?
-            if len(interrupt.responses) == 1:
-                output = middleware.transform_output_sync(
-                    interrupt.responses[0].data
-                )
-                if isinstance(output, Exception):
-                    return execution.CallError.from_error(output)
-                interrupt.responses[0].data = output
+                return execution.CallResult(err)
 
-            return interrupt.responses
+            return execution.CallResult.from_responses(interrupt.responses)
         except _UserError as err:
-            return execution.CallError.from_error(err.err)
+            return execution.CallResult(err.err)
         except step_lib.SkipInterrupt as err:
             # This should only happen in a non-deterministic scenario, where
             # step targeting is enabled and an unexpected step is encountered.
             # We don't currently have a way to recover from this scenario.
 
-            return execution.CallError.from_error(
+            return execution.CallResult(
                 errors.StepUnexpectedError(
                     f'found step "{err.step_id}" when targeting a different step'
                 )
             )
         except Exception as err:
-            return execution.CallError.from_error(err)
+            return execution.CallResult(err)
 
     def get_config(self, app_url: str) -> _Config:
         fn_id = self._opts.fully_qualified_id
         name = self._opts.name
 
         if self._opts.retries is not None:
             retries = function_config.Retries(attempts=self._opts.retries)
```

### Comparing `inngest-0.3.9/inngest/_internal/function_config.py` & `inngest-0.4.0a0/inngest/_internal/function_config.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.9/inngest/_internal/function_config_test.py` & `inngest-0.4.0a0/inngest/_internal/function_config_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.9/inngest/_internal/log.py` & `inngest-0.4.0a0/inngest/_internal/middleware_lib/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from __future__ import annotations
 
-from . import client_lib, function, middleware_lib, types
+from inngest._internal import client_lib, function, step_lib, types
 
+from .middleware import MiddlewareSync
 
-class LoggerProxy:
-    """
-    Wraps a logger, allowing us to disable logging when we want to. This is
-    important because we may call a function multiple times and we don't want
-    duplicate logs.
-    """
 
+class LoggerProxy:
     _proxied_methods = (
         "critical",
         "debug",
         "error",
         "exception",
         "fatal",
         "info",
@@ -33,23 +29,23 @@
 
         return getattr(self.logger, name)
 
     def enable(self) -> None:
         self._is_enabled = True
 
 
-class LoggerMiddleware(middleware_lib.MiddlewareSync):
-    def __init__(self, client: client_lib.Inngest) -> None:
-        super().__init__(client)
+class LoggerMiddleware(MiddlewareSync):
+    def __init__(self, client: client_lib.Inngest, raw_request: object) -> None:
+        super().__init__(client, raw_request)
         self.logger = LoggerProxy(client.logger)
 
     def before_execution(self) -> None:
-        # Enable logging because we've encountered new code.
         self.logger.enable()
 
     def transform_input(
         self,
         ctx: function.Context,
-    ) -> function.Context:
+        function: function.Function,
+        steps: step_lib.StepMemos,
+    ) -> None:
         self.logger.logger = ctx.logger
         ctx.logger = self.logger  # type: ignore
-        return ctx
```

### Comparing `inngest-0.3.9/inngest/_internal/net.py` & `inngest-0.4.0a0/inngest/_internal/net.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,41 @@
+from __future__ import annotations
+
 import hashlib
 import hmac
 import http
 import os
+import threading
 import typing
 import urllib.parse
 
 import httpx
 
-from . import const, errors, transforms, types
+from . import async_lib, const, errors, transforms, types
+
+
+class ThreadAwareAsyncHTTPClient(httpx.AsyncClient):
+    """
+    Thin wrapper around httpx.AsyncClient. It keeps track of the thread it was
+    created in, which is critical since asyncio is not thread safe: calling an
+    async method in a different thread will raise an exception
+    """
 
-Method = typing.Literal["GET", "POST"]
+    _creation_thread_id: typing.Optional[int] = None
+
+    def is_same_thread(self) -> bool:
+        if self._creation_thread_id is None:
+            raise Exception("did not initialize ThreadAwareAsyncHTTPClient")
+
+        current_thread_id = threading.get_ident()
+        return self._creation_thread_id == current_thread_id
+
+    def initialize(self) -> ThreadAwareAsyncHTTPClient:
+        self._creation_thread_id = threading.get_ident()
+        return self
 
 
 def create_headers(
     *,
     env: typing.Optional[str],
     framework: typing.Optional[const.Framework],
     server_kind: typing.Optional[const.ServerKind],
@@ -80,15 +102,16 @@
 
     return urllib.parse.urlunparse(
         (new_scheme, new_netloc, new_path, "", "", "")
     )
 
 
 async def fetch_with_auth_fallback(
-    client: httpx.AsyncClient,
+    client: ThreadAwareAsyncHTTPClient,
+    client_sync: httpx.Client,
     request: httpx.Request,
     *,
     signing_key: typing.Optional[str],
     signing_key_fallback: typing.Optional[str],
 ) -> httpx.Response:
     """
     Send an HTTP request with the given signing key. If the response is a 401 or
@@ -96,25 +119,34 @@
     """
 
     if signing_key is not None:
         request.headers[
             const.HeaderKey.AUTHORIZATION.value
         ] = f"Bearer {transforms.hash_signing_key(signing_key)}"
 
-    res = await client.send(request)
+    res = await fetch_with_thready_safety(
+        client,
+        client_sync,
+        request,
+    )
     if (
         res.status_code
         in (http.HTTPStatus.FORBIDDEN, http.HTTPStatus.UNAUTHORIZED)
         and signing_key_fallback is not None
     ):
         # Try again with the signing key fallback
         request.headers[
             const.HeaderKey.AUTHORIZATION.value
         ] = f"Bearer {transforms.hash_signing_key(signing_key_fallback)}"
-        res = await client.send(request)
+
+        res = await fetch_with_thready_safety(
+            client,
+            client_sync,
+            request,
+        )
 
     return res
 
 
 def fetch_with_auth_fallback_sync(
     client: httpx.Client,
     request: httpx.Request,
@@ -169,14 +201,40 @@
 
     if parsed.scheme == "":
         parsed._replace(scheme="https")
 
     return parsed.geturl()
 
 
+async def fetch_with_thready_safety(
+    client: ThreadAwareAsyncHTTPClient,
+    client_sync: httpx.Client,
+    request: httpx.Request,
+) -> httpx.Response:
+    """
+    Safely handles the situation where the async HTTP client is called in a
+    different thread.
+    """
+
+    if client.is_same_thread() is True:
+        # Python freaks out if you call httpx.AsyncClient's methods in multiple
+        # threads. So we'll only use it if we're in the same thread as its first
+        # method call
+        return await client.send(request)
+
+    loop = async_lib.get_event_loop()
+    if loop is None:
+        return client_sync.send(request)
+
+    return await loop.run_in_executor(
+        None,
+        lambda: client_sync.send(request),
+    )
+
+
 class RequestSignature:
     _signature: typing.Optional[str] = None
     _timestamp: typing.Optional[int] = None
 
     def __init__(
         self,
         body: bytes,
```

### Comparing `inngest-0.3.9/inngest/_internal/net_test.py` & `inngest-0.4.0a0/inngest/_internal/net_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,15 +237,18 @@
 
             if actual_token != expected_token:
                 return httpx.Response(401, content=b"", request=request)
 
             return httpx.Response(200, content=b"", request=request)
 
         res = await net.fetch_with_auth_fallback(
-            httpx.AsyncClient(transport=self._create_async_transport(handler)),
+            net.ThreadAwareAsyncHTTPClient(
+                transport=self._create_async_transport(handler)
+            ).initialize(),
+            httpx.Client(transport=self._create_transport(handler)),
             self._req,
             signing_key=_signing_key,
             signing_key_fallback=_signing_key_fallback,
         )
         assert res.status_code == 200
         assert req_count == 1
         req_count = 0
@@ -279,15 +282,18 @@
 
             if actual_token != expected_token:
                 return httpx.Response(401, content=b"", request=request)
 
             return httpx.Response(200, content=b"", request=request)
 
         res = await net.fetch_with_auth_fallback(
-            httpx.AsyncClient(transport=self._create_async_transport(handler)),
+            net.ThreadAwareAsyncHTTPClient(
+                transport=self._create_async_transport(handler)
+            ).initialize(),
+            httpx.Client(transport=self._create_transport(handler)),
             self._req,
             signing_key=_signing_key,
             signing_key_fallback=_signing_key_fallback,
         )
         assert res.status_code == 200
         assert req_count == 2
         req_count = 0
@@ -321,15 +327,18 @@
 
             if actual_token != expected_token:
                 return httpx.Response(401, content=b"", request=request)
 
             return httpx.Response(200, content=b"", request=request)
 
         res = await net.fetch_with_auth_fallback(
-            httpx.AsyncClient(transport=self._create_async_transport(handler)),
+            net.ThreadAwareAsyncHTTPClient(
+                transport=self._create_async_transport(handler)
+            ).initialize(),
+            httpx.Client(transport=self._create_transport(handler)),
             self._req,
             signing_key="signkey-prod-aaaaaa",
             signing_key_fallback="signkey-prod-bbbbbb",
         )
         assert res.status_code == 401
         assert req_count == 2
         req_count = 0
@@ -358,15 +367,18 @@
             actual_token = request.headers.get("Authorization")
             if actual_token is not None:
                 return httpx.Response(500, content=b"", request=request)
 
             return httpx.Response(200, content=b"", request=request)
 
         res = await net.fetch_with_auth_fallback(
-            httpx.AsyncClient(transport=self._create_async_transport(handler)),
+            net.ThreadAwareAsyncHTTPClient(
+                transport=self._create_async_transport(handler)
+            ).initialize(),
+            httpx.Client(transport=self._create_transport(handler)),
             self._req,
             signing_key=None,
             signing_key_fallback=None,
         )
         assert res.status_code == 200
         assert req_count == 1
         req_count = 0
```

### Comparing `inngest-0.3.9/inngest/_internal/step_lib/base.py` & `inngest-0.4.0a0/inngest/_internal/step_lib/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     @property
     def size(self) -> int:
         return len(self._memos)
 
     def __init__(self, memos: dict[str, execution.Output]) -> None:
         self._memos = memos
 
+    def values(self) -> typing.Iterator[execution.Output]:
+        return iter(self._memos.values())
+
     def pop(
         self, hashed_id: str
     ) -> typing.Union[execution.Output, types.EmptySentinel]:
         if hashed_id in self._memos:
             memo = self._memos[hashed_id]
 
             # Remove memo
@@ -81,24 +84,20 @@
 
         # If there are no more memos then all future code is new.
         if self._memos.size == 0:
             await self._middleware.before_execution()
 
         if not isinstance(memo, types.EmptySentinel):
             if memo.error is not None:
-                error = execution.MemoizedError.from_raw(memo.error)
-                if isinstance(error, Exception):
-                    raise error
-
                 # If there's a memoized error then raise an error, since the
                 # step exhausted its retries
                 raise errors.StepError(
-                    message=error.message,
-                    name=error.name,
-                    stack=error.stack,
+                    message=memo.error.message,
+                    name=memo.error.name,
+                    stack=memo.error.stack,
                 )
 
         return memo
 
     def _get_memo_sync(
         self,
         hashed_id: str,
@@ -107,24 +106,20 @@
 
         # If there are no more memos then all future code is new.
         if self._memos.size == 0:
             self._middleware.before_execution_sync()
 
         if not isinstance(memo, types.EmptySentinel):
             if memo.error is not None:
-                error = execution.MemoizedError.from_raw(memo.error)
-                if isinstance(error, Exception):
-                    raise error
-
                 # If there's a memoized error then raise an error, since the
                 # step exhausted its retries
                 raise errors.StepError(
-                    message=error.message,
-                    name=error.name,
-                    stack=error.stack,
+                    message=memo.error.message,
+                    name=memo.error.name,
+                    stack=memo.error.stack,
                 )
 
         return memo
 
     def _handle_skip(
         self,
         parsed_step_id: _ParsedStepID,
@@ -200,23 +195,18 @@
 
 
 class SkipInterrupt(BaseException):
     def __init__(self, step_id: str) -> None:
         self.step_id = step_id
 
 
-@dataclasses.dataclass
-class FunctionID:
-    app_id: str
-    function_id: str
-
-
 class InvokeOpts(types.BaseModel):
     function_id: str
     payload: InvokeOptsPayload
+    timeout: typing.Optional[str]
 
 
 class InvokeOptsPayload(types.BaseModel):
     data: object
     user: object
     v: typing.Optional[str]
```

### Comparing `inngest-0.3.9/inngest/_internal/step_lib/step_async.py` & `inngest-0.4.0a0/inngest/_internal/step_lib/step_sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 import datetime
 import typing
 
+import typing_extensions
+
 from inngest._internal import errors, event_lib, execution, transforms, types
+from inngest._internal.client_lib import models as client_models
 
 from . import base
 
 # Avoid circular import at runtime
 if typing.TYPE_CHECKING:
     from inngest._internal.function import Function
 else:
     Function = object
 
 
-class Step(base.StepBase):
-    async def invoke(
+class StepSync(base.StepBase):
+    def invoke(
         self,
         step_id: str,
         *,
         function: Function,
         data: typing.Optional[types.JSON] = None,
+        timeout: typing.Union[int, datetime.timedelta],
         user: typing.Optional[types.JSON] = None,
         v: typing.Optional[str] = None,
     ) -> object:
         """
         Invoke an Inngest function with data. Returns the result of the returned
         value of the function or `None` if the function does not return a value.
 
         If a function isn't found or otherwise errors, the step will fail and
         raise a `NonRetriableError`.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
 
             function: The function object to invoke.
-            data: Will become `event.data` in the invoked function. Must be JSON
-                serializable.
-            user: Will become `event.user` in the invoked function. Must be JSON
-                serializable.
+            data: Will become `event.data` in the invoked function. Must be JSON serializable.
+            timeout: The maximum number of milliseconds to wait for the function to complete.
+            user: Will become `event.user` in the invoked function. Must be JSON serializable.
             v: Will become `event.v` in the invoked function.
         """
 
-        return await self.invoke_by_id(
+        return self.invoke_by_id(
             step_id,
             app_id=self._client.app_id,
             function_id=function._opts.local_id,
             data=data,
+            timeout=timeout,
             user=user,
             v=v,
         )
 
-    async def invoke_by_id(
+    def invoke_by_id(
         self,
         step_id: str,
         *,
         app_id: typing.Optional[str] = None,
         function_id: str,
         data: typing.Optional[types.JSON] = None,
+        timeout: typing.Union[int, datetime.timedelta],
         user: typing.Optional[types.JSON] = None,
         v: typing.Optional[str] = None,
     ) -> object:
         """
         Invoke an Inngest function with data. Returns the result of the returned
         value of the function or `None` if the function does not return a value.
 
@@ -70,300 +73,314 @@
         app.
 
         If a function isn't found or otherwise errors, the step will fail and
         raise a `NonRetriableError`.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
 
-            app_id: The app ID of the function to invoke. Not necessary if this
-                function and the invoked function are in the same app.
+            app_id: The app ID of the function to invoke. Not necessary if this function and the invoked function are in the same app.
             function_id: The ID of the function to invoke.
-            data: Will become `event.data` in the invoked function. Must be JSON
-                serializable.
-            user: Will become `event.user` in the invoked function. Must be JSON
-                serializable.
+            data: Will become `event.data` in the invoked function. Must be JSON serializable.
+            timeout: The maximum number of milliseconds to wait for the function to complete.
+            user: Will become `event.user` in the invoked function. Must be JSON serializable.
             v: Will become `event.v` in the invoked function.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = await self._get_memo(parsed_step_id.hashed)
+        memo = self._get_memo_sync(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             return memo.data
 
         self._handle_skip(parsed_step_id)
 
-        err = await self._middleware.before_execution()
+        err = self._middleware.before_execution_sync()
         if isinstance(err, Exception):
             raise err
 
+        timeout_str = transforms.to_duration_str(timeout)
+        if isinstance(timeout_str, Exception):
+            raise timeout_str
+
         opts = base.InvokeOpts(
             function_id=f"{app_id}-{function_id}",
             payload=base.InvokeOptsPayload(
                 data=data,
                 user=user,
                 v=v,
             ),
+            timeout=timeout_str,
         ).to_dict()
         if isinstance(opts, Exception):
             raise opts
 
         raise base.ResponseInterrupt(
             execution.StepResponse(
-                display_name=parsed_step_id.user_facing,
-                id=parsed_step_id.hashed,
-                name=parsed_step_id.user_facing,
-                op=execution.Opcode.INVOKE,
-                opts=opts,
+                step=execution.StepInfo(
+                    display_name=parsed_step_id.user_facing,
+                    id=parsed_step_id.hashed,
+                    name=parsed_step_id.user_facing,
+                    op=execution.Opcode.INVOKE,
+                    opts=opts,
+                )
             )
         )
 
-    async def parallel(
+    def parallel(
         self,
-        callables: tuple[typing.Callable[[], typing.Awaitable[types.T]], ...],
+        callables: tuple[typing.Callable[[], types.T], ...],
     ) -> tuple[types.T, ...]:
         """
         Run multiple steps in parallel.
 
         Args:
         ----
-            callables: An arbitrary number of step callbacks to run. These are
-                callables that contain the step (e.g. `lambda: step.run("my_step", my_step_fn)`.
+            callables: An arbitrary number of step callbacks to run. These are callables that contain the step (e.g. `lambda: step.run("my_step", my_step_fn)`.
         """
 
         self._inside_parallel = True
 
         outputs = tuple[types.T]()
         responses: list[execution.StepResponse] = []
         for cb in callables:
             try:
-                output = await cb()
+                output = cb()
                 outputs = (*outputs, output)
             except base.ResponseInterrupt as interrupt:
                 responses = [*responses, *interrupt.responses]
             except base.SkipInterrupt:
                 pass
 
         if len(responses) > 0:
             raise base.ResponseInterrupt(responses)
 
         self._inside_parallel = False
         return outputs
 
-    @typing.overload
-    async def run(
-        self,
-        step_id: str,
-        handler: typing.Callable[[], typing.Awaitable[types.JSONT]],
-    ) -> types.JSONT:
-        ...
-
-    @typing.overload
-    async def run(
-        self,
-        step_id: str,
-        handler: typing.Callable[[], types.JSONT],
-    ) -> types.JSONT:
-        ...
-
-    async def run(
+    def run(
         self,
         step_id: str,
-        handler: typing.Union[
-            typing.Callable[[], typing.Awaitable[types.JSONT]],
-            typing.Callable[[], types.JSONT],
+        handler: typing.Callable[
+            [typing_extensions.Unpack[types.TTuple]],
+            types.JSONT,
         ],
+        *handler_args: typing_extensions.Unpack[types.TTuple],
     ) -> types.JSONT:
         """
         Run logic that should be retried on error and memoized after success.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             handler: The logic to run.
+            *handler_args: Arguments to pass to the handler.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = await self._get_memo(parsed_step_id.hashed)
+        memo = self._get_memo_sync(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             return memo.data  # type: ignore
 
         self._handle_skip(parsed_step_id)
 
         is_targeting_enabled = self._target_hashed_id is not None
         if self._inside_parallel and not is_targeting_enabled:
             # Plan this step because we're in parallel mode.
             raise base.ResponseInterrupt(
                 execution.StepResponse(
-                    display_name=parsed_step_id.user_facing,
-                    id=parsed_step_id.hashed,
-                    name=parsed_step_id.user_facing,
-                    op=execution.Opcode.PLANNED,
+                    step=execution.StepInfo(
+                        display_name=parsed_step_id.user_facing,
+                        id=parsed_step_id.hashed,
+                        name=parsed_step_id.user_facing,
+                        op=execution.Opcode.PLANNED,
+                    )
                 )
             )
 
-        err = await self._middleware.before_execution()
+        err = self._middleware.before_execution_sync()
         if isinstance(err, Exception):
             raise err
 
         try:
-            output = await transforms.maybe_await(handler())
+            output = handler(*handler_args)
 
             raise base.ResponseInterrupt(
                 execution.StepResponse(
-                    data=execution.Output(data=output),
-                    display_name=parsed_step_id.user_facing,
-                    id=parsed_step_id.hashed,
-                    name=parsed_step_id.user_facing,
-                    op=execution.Opcode.STEP_RUN,
+                    output=output,
+                    step=execution.StepInfo(
+                        display_name=parsed_step_id.user_facing,
+                        id=parsed_step_id.hashed,
+                        name=parsed_step_id.user_facing,
+                        op=execution.Opcode.STEP_RUN,
+                    ),
                 )
             )
-        except errors.NonRetriableError as err:
-            # NonRetriableErrors should bubble up to the function level
+        except (errors.NonRetriableError, errors.RetryAfterError) as err:
+            # Bubble up these error types to the function level
             raise err
         except Exception as err:
             transforms.remove_first_traceback_frame(err)
 
-            error_dict = execution.MemoizedError.from_error(err).to_dict()
-            if isinstance(error_dict, Exception):
-                raise error_dict
-
             raise base.ResponseInterrupt(
                 execution.StepResponse(
-                    data=execution.Output(error=error_dict),
-                    display_name=parsed_step_id.user_facing,
-                    id=parsed_step_id.hashed,
-                    op=execution.Opcode.STEP_ERROR,
+                    original_error=err,
+                    step=execution.StepInfo(
+                        display_name=parsed_step_id.user_facing,
+                        id=parsed_step_id.hashed,
+                        op=execution.Opcode.STEP_ERROR,
+                    ),
                 )
             )
 
-    async def send_event(
+    def send_event(
         self,
         step_id: str,
         events: typing.Union[event_lib.Event, list[event_lib.Event]],
     ) -> list[str]:
         """
         Send an event or list of events.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             events: An event or list of events to send.
         """
 
-        async def fn() -> list[str]:
-            return await self._client.send(events)
+        def fn() -> list[str]:
+            if isinstance(events, list):
+                _events = events
+            else:
+                _events = [events]
+
+            middleware_err = self._middleware.before_send_events_sync(_events)
+            if isinstance(middleware_err, Exception):
+                raise middleware_err
+
+            try:
+                result = client_models.SendEventsResult(
+                    ids=self._client.send_sync(
+                        events,
+                        # Skip middleware since we're already running it above. Without
+                        # this, we'll double-call middleware hooks
+                        skip_middleware=True,
+                    )
+                )
+            except errors.SendEventsError as err:
+                result = client_models.SendEventsResult(
+                    error=str(err),
+                    ids=err.ids,
+                )
+                raise err
+            finally:
+                middleware_err = self._middleware.after_send_events_sync(result)
+                if isinstance(middleware_err, Exception):
+                    raise middleware_err
 
-        return await self.run(step_id, fn)
+            return result.ids
 
-    async def sleep(
+        return self.run(step_id, fn)
+
+    def sleep(
         self,
         step_id: str,
         duration: typing.Union[int, datetime.timedelta],
     ) -> None:
         """
         Sleep for a duration.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             duration: The number of milliseconds to sleep.
         """
         if isinstance(duration, int):
             until = datetime.datetime.now() + datetime.timedelta(
                 milliseconds=duration
             )
         else:
             until = datetime.datetime.now() + duration
 
-        return await self.sleep_until(step_id, until)
+        return self.sleep_until(step_id, until)
 
-    async def sleep_until(
+    def sleep_until(
         self,
         step_id: str,
         until: datetime.datetime,
     ) -> None:
         """
         Sleep until a specific time.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             until: The time to sleep until.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = await self._get_memo(parsed_step_id.hashed)
+        memo = self._get_memo_sync(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             return memo.data  # type: ignore
 
         self._handle_skip(parsed_step_id)
 
-        err = await self._middleware.before_execution()
+        err = self._middleware.before_execution_sync()
         if isinstance(err, Exception):
             raise err
 
         raise base.ResponseInterrupt(
             execution.StepResponse(
-                display_name=parsed_step_id.user_facing,
-                id=parsed_step_id.hashed,
-                name=transforms.to_iso_utc(until),
-                op=execution.Opcode.SLEEP,
+                step=execution.StepInfo(
+                    display_name=parsed_step_id.user_facing,
+                    id=parsed_step_id.hashed,
+                    name=transforms.to_iso_utc(until),
+                    op=execution.Opcode.SLEEP,
+                )
             )
         )
 
-    async def wait_for_event(
+    def wait_for_event(
         self,
         step_id: str,
         *,
         event: str,
         if_exp: typing.Optional[str] = None,
         timeout: typing.Union[int, datetime.timedelta],
     ) -> typing.Optional[event_lib.Event]:
         """
         Wait for an event to be sent.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             event: Event name.
             if_exp: An expression to filter events.
             timeout: The maximum number of milliseconds to wait for the event.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = await self._get_memo(parsed_step_id.hashed)
+        memo = self._get_memo_sync(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             if memo.data is None:
                 # Timeout
                 return None
 
             # Fulfilled by an event
-            return event_lib.Event.model_validate(memo.data)
+            event_obj = event_lib.Event.from_raw(memo.data)
+            if isinstance(event_obj, Exception):
+                raise errors.UnknownError("invalid event shape") from event_obj
+            return event_obj
 
         self._handle_skip(parsed_step_id)
 
-        err = await self._middleware.before_execution()
+        err = self._middleware.before_execution_sync()
         if isinstance(err, Exception):
             raise err
 
         timeout_str = transforms.to_duration_str(timeout)
         if isinstance(timeout_str, Exception):
             raise timeout_str
 
@@ -372,14 +389,16 @@
             timeout=timeout_str,
         ).to_dict()
         if isinstance(opts, Exception):
             raise opts
 
         raise base.ResponseInterrupt(
             execution.StepResponse(
-                id=parsed_step_id.hashed,
-                display_name=parsed_step_id.user_facing,
-                name=event,
-                op=execution.Opcode.WAIT_FOR_EVENT,
-                opts=opts,
+                step=execution.StepInfo(
+                    display_name=parsed_step_id.user_facing,
+                    id=parsed_step_id.hashed,
+                    name=event,
+                    op=execution.Opcode.WAIT_FOR_EVENT,
+                    opts=opts,
+                )
             )
         )
```

### Comparing `inngest-0.3.9/inngest/_internal/step_lib/step_sync.py` & `inngest-0.4.0a0/inngest/_internal/step_lib/step_async.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,71 @@
 import datetime
 import typing
 
+import typing_extensions
+
 from inngest._internal import errors, event_lib, execution, transforms, types
+from inngest._internal.client_lib import models as client_models
 
 from . import base
 
 # Avoid circular import at runtime
 if typing.TYPE_CHECKING:
     from inngest._internal.function import Function
 else:
     Function = object
 
 
-class StepSync(base.StepBase):
-    def invoke(
+class Step(base.StepBase):
+    async def invoke(
         self,
         step_id: str,
         *,
         function: Function,
         data: typing.Optional[types.JSON] = None,
+        timeout: typing.Union[int, datetime.timedelta],
         user: typing.Optional[types.JSON] = None,
         v: typing.Optional[str] = None,
     ) -> object:
         """
         Invoke an Inngest function with data. Returns the result of the returned
         value of the function or `None` if the function does not return a value.
 
         If a function isn't found or otherwise errors, the step will fail and
         raise a `NonRetriableError`.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
 
             function: The function object to invoke.
-            data: Will become `event.data` in the invoked function. Must be JSON
-                serializable.
-            user: Will become `event.user` in the invoked function. Must be JSON
-                serializable.
+            data: Will become `event.data` in the invoked function. Must be JSON serializable.
+            timeout: The maximum number of milliseconds to wait for the function to complete.
+            user: Will become `event.user` in the invoked function. Must be JSON serializable.
             v: Will become `event.v` in the invoked function.
         """
 
-        return self.invoke_by_id(
+        return await self.invoke_by_id(
             step_id,
             app_id=self._client.app_id,
             function_id=function._opts.local_id,
             data=data,
+            timeout=timeout,
             user=user,
             v=v,
         )
 
-    def invoke_by_id(
+    async def invoke_by_id(
         self,
         step_id: str,
         *,
         app_id: typing.Optional[str] = None,
         function_id: str,
         data: typing.Optional[types.JSON] = None,
+        timeout: typing.Union[int, datetime.timedelta],
         user: typing.Optional[types.JSON] = None,
         v: typing.Optional[str] = None,
     ) -> object:
         """
         Invoke an Inngest function with data. Returns the result of the returned
         value of the function or `None` if the function does not return a value.
 
@@ -70,284 +73,343 @@
         app.
 
         If a function isn't found or otherwise errors, the step will fail and
         raise a `NonRetriableError`.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
 
-            app_id: The app ID of the function to invoke. Not necessary if this
-                function and the invoked function are in the same app.
+            app_id: The app ID of the function to invoke. Not necessary if this function and the invoked function are in the same app.
             function_id: The ID of the function to invoke.
-            data: Will become `event.data` in the invoked function. Must be JSON
-                serializable.
-            user: Will become `event.user` in the invoked function. Must be JSON
-                serializable.
+            data: Will become `event.data` in the invoked function. Must be JSON serializable.
+            timeout: The maximum number of milliseconds to wait for the function to complete.
+            user: Will become `event.user` in the invoked function. Must be JSON serializable.
             v: Will become `event.v` in the invoked function.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = self._get_memo_sync(parsed_step_id.hashed)
+        memo = await self._get_memo(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             return memo.data
 
         self._handle_skip(parsed_step_id)
 
-        err = self._middleware.before_execution_sync()
+        err = await self._middleware.before_execution()
         if isinstance(err, Exception):
             raise err
 
+        timeout_str = transforms.to_duration_str(timeout)
+        if isinstance(timeout_str, Exception):
+            raise timeout_str
+
         opts = base.InvokeOpts(
             function_id=f"{app_id}-{function_id}",
             payload=base.InvokeOptsPayload(
                 data=data,
                 user=user,
                 v=v,
             ),
+            timeout=timeout_str,
         ).to_dict()
         if isinstance(opts, Exception):
             raise opts
 
         raise base.ResponseInterrupt(
             execution.StepResponse(
-                display_name=parsed_step_id.user_facing,
-                id=parsed_step_id.hashed,
-                name=parsed_step_id.user_facing,
-                op=execution.Opcode.INVOKE,
-                opts=opts,
+                step=execution.StepInfo(
+                    display_name=parsed_step_id.user_facing,
+                    id=parsed_step_id.hashed,
+                    name=parsed_step_id.user_facing,
+                    op=execution.Opcode.INVOKE,
+                    opts=opts,
+                )
             )
         )
 
-    def parallel(
+    async def parallel(
         self,
-        callables: tuple[typing.Callable[[], types.T], ...],
+        callables: tuple[typing.Callable[[], typing.Awaitable[types.T]], ...],
     ) -> tuple[types.T, ...]:
         """
         Run multiple steps in parallel.
 
         Args:
         ----
-            callables: An arbitrary number of step callbacks to run. These are
-                callables that contain the step (e.g. `lambda: step.run("my_step", my_step_fn)`.
+            callables: An arbitrary number of step callbacks to run. These are callables that contain the step (e.g. `lambda: step.run("my_step", my_step_fn)`.
         """
 
         self._inside_parallel = True
 
         outputs = tuple[types.T]()
         responses: list[execution.StepResponse] = []
         for cb in callables:
             try:
-                output = cb()
+                output = await cb()
                 outputs = (*outputs, output)
             except base.ResponseInterrupt as interrupt:
                 responses = [*responses, *interrupt.responses]
             except base.SkipInterrupt:
                 pass
 
         if len(responses) > 0:
             raise base.ResponseInterrupt(responses)
 
         self._inside_parallel = False
         return outputs
 
-    def run(
+    @typing.overload
+    async def run(
+        self,
+        step_id: str,
+        handler: typing.Callable[
+            [typing_extensions.Unpack[types.TTuple]],
+            typing.Awaitable[types.JSONT],
+        ],
+        *handler_args: typing_extensions.Unpack[types.TTuple],
+    ) -> types.JSONT:
+        ...
+
+    @typing.overload
+    async def run(
         self,
         step_id: str,
-        handler: typing.Callable[[], types.JSONT],
+        handler: typing.Callable[
+            [typing_extensions.Unpack[types.TTuple]], types.JSONT
+        ],
+        *handler_args: typing_extensions.Unpack[types.TTuple],
+    ) -> types.JSONT:
+        ...
+
+    async def run(
+        self,
+        step_id: str,
+        handler: typing.Union[
+            typing.Callable[
+                [typing_extensions.Unpack[types.TTuple]],
+                typing.Awaitable[types.JSONT],
+            ],
+            typing.Callable[
+                [typing_extensions.Unpack[types.TTuple]], types.JSONT
+            ],
+        ],
+        *handler_args: typing_extensions.Unpack[types.TTuple],
     ) -> types.JSONT:
         """
         Run logic that should be retried on error and memoized after success.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             handler: The logic to run.
+            *handler_args: Arguments to pass to the handler.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = self._get_memo_sync(parsed_step_id.hashed)
+        memo = await self._get_memo(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             return memo.data  # type: ignore
 
         self._handle_skip(parsed_step_id)
 
         is_targeting_enabled = self._target_hashed_id is not None
         if self._inside_parallel and not is_targeting_enabled:
             # Plan this step because we're in parallel mode.
             raise base.ResponseInterrupt(
                 execution.StepResponse(
-                    display_name=parsed_step_id.user_facing,
-                    id=parsed_step_id.hashed,
-                    name=parsed_step_id.user_facing,
-                    op=execution.Opcode.PLANNED,
+                    step=execution.StepInfo(
+                        display_name=parsed_step_id.user_facing,
+                        id=parsed_step_id.hashed,
+                        name=parsed_step_id.user_facing,
+                        op=execution.Opcode.PLANNED,
+                    )
                 )
             )
 
-        err = self._middleware.before_execution_sync()
+        err = await self._middleware.before_execution()
         if isinstance(err, Exception):
             raise err
 
         try:
-            output = handler()
+            output = await transforms.maybe_await(handler(*handler_args))
 
             raise base.ResponseInterrupt(
                 execution.StepResponse(
-                    data=execution.Output(data=output),
-                    display_name=parsed_step_id.user_facing,
-                    id=parsed_step_id.hashed,
-                    name=parsed_step_id.user_facing,
-                    op=execution.Opcode.STEP_RUN,
+                    output=output,
+                    step=execution.StepInfo(
+                        display_name=parsed_step_id.user_facing,
+                        id=parsed_step_id.hashed,
+                        name=parsed_step_id.user_facing,
+                        op=execution.Opcode.STEP_RUN,
+                    ),
                 )
             )
-        except errors.NonRetriableError as err:
-            # NonRetriableErrors should bubble up to the function level
+        except (errors.NonRetriableError, errors.RetryAfterError) as err:
+            # Bubble up these error types to the function level
             raise err
         except Exception as err:
             transforms.remove_first_traceback_frame(err)
 
-            error_dict = execution.MemoizedError.from_error(err).to_dict()
-            if isinstance(error_dict, Exception):
-                raise error_dict
-
             raise base.ResponseInterrupt(
                 execution.StepResponse(
-                    display_name=parsed_step_id.user_facing,
-                    data=execution.Output(error=error_dict),
-                    id=parsed_step_id.hashed,
-                    op=execution.Opcode.STEP_ERROR,
+                    original_error=err,
+                    step=execution.StepInfo(
+                        display_name=parsed_step_id.user_facing,
+                        id=parsed_step_id.hashed,
+                        op=execution.Opcode.STEP_ERROR,
+                    ),
                 )
             )
 
-    def send_event(
+    async def send_event(
         self,
         step_id: str,
         events: typing.Union[event_lib.Event, list[event_lib.Event]],
     ) -> list[str]:
         """
         Send an event or list of events.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             events: An event or list of events to send.
         """
 
-        def fn() -> list[str]:
-            return self._client.send_sync(events)
+        async def fn() -> list[str]:
+            if isinstance(events, list):
+                _events = events
+            else:
+                _events = [events]
+
+            middleware_err = await self._middleware.before_send_events(_events)
+            if isinstance(middleware_err, Exception):
+                raise middleware_err
+
+            try:
+                result = client_models.SendEventsResult(
+                    ids=(
+                        await self._client.send(
+                            events,
+                            # Skip middleware since we're already running it above. Without
+                            # this, we'll double-call middleware hooks
+                            skip_middleware=True,
+                        )
+                    )
+                )
+            except errors.SendEventsError as err:
+                result = client_models.SendEventsResult(
+                    error=str(err),
+                    ids=err.ids,
+                )
+                raise err
+            finally:
+                middleware_err = await self._middleware.after_send_events(
+                    result
+                )
+                if isinstance(middleware_err, Exception):
+                    raise middleware_err
+
+            return result.ids
 
-        return self.run(step_id, fn)
+        return await self.run(step_id, fn)
 
-    def sleep(
+    async def sleep(
         self,
         step_id: str,
         duration: typing.Union[int, datetime.timedelta],
     ) -> None:
         """
         Sleep for a duration.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             duration: The number of milliseconds to sleep.
         """
         if isinstance(duration, int):
             until = datetime.datetime.now() + datetime.timedelta(
                 milliseconds=duration
             )
         else:
             until = datetime.datetime.now() + duration
 
-        return self.sleep_until(step_id, until)
+        return await self.sleep_until(step_id, until)
 
-    def sleep_until(
+    async def sleep_until(
         self,
         step_id: str,
         until: datetime.datetime,
     ) -> None:
         """
         Sleep until a specific time.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             until: The time to sleep until.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = self._get_memo_sync(parsed_step_id.hashed)
+        memo = await self._get_memo(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             return memo.data  # type: ignore
 
         self._handle_skip(parsed_step_id)
 
-        err = self._middleware.before_execution_sync()
+        err = await self._middleware.before_execution()
         if isinstance(err, Exception):
             raise err
 
         raise base.ResponseInterrupt(
             execution.StepResponse(
-                display_name=parsed_step_id.user_facing,
-                id=parsed_step_id.hashed,
-                name=transforms.to_iso_utc(until),
-                op=execution.Opcode.SLEEP,
+                step=execution.StepInfo(
+                    display_name=parsed_step_id.user_facing,
+                    id=parsed_step_id.hashed,
+                    name=transforms.to_iso_utc(until),
+                    op=execution.Opcode.SLEEP,
+                )
             )
         )
 
-    def wait_for_event(
+    async def wait_for_event(
         self,
         step_id: str,
         *,
         event: str,
         if_exp: typing.Optional[str] = None,
         timeout: typing.Union[int, datetime.timedelta],
     ) -> typing.Optional[event_lib.Event]:
         """
         Wait for an event to be sent.
 
         Args:
         ----
-            step_id: Durable step ID. Should usually be unique within a
-                function, but it's OK to reuse as long as your function is
-                deterministic.
+            step_id: Durable step ID. Should usually be unique within a function, but it's OK to reuse as long as your function is deterministic.
             event: Event name.
             if_exp: An expression to filter events.
             timeout: The maximum number of milliseconds to wait for the event.
         """
 
         parsed_step_id = self._parse_step_id(step_id)
 
-        memo = self._get_memo_sync(parsed_step_id.hashed)
+        memo = await self._get_memo(parsed_step_id.hashed)
         if not isinstance(memo, types.EmptySentinel):
             if memo.data is None:
                 # Timeout
                 return None
 
             # Fulfilled by an event
-            event_obj = event_lib.Event.from_raw(memo.data)
-            if isinstance(event_obj, Exception):
-                raise errors.UnknownError("invalid event shape") from event_obj
-            return event_obj
+            return event_lib.Event.model_validate(memo.data)
 
         self._handle_skip(parsed_step_id)
 
-        err = self._middleware.before_execution_sync()
+        err = await self._middleware.before_execution()
         if isinstance(err, Exception):
             raise err
 
         timeout_str = transforms.to_duration_str(timeout)
         if isinstance(timeout_str, Exception):
             raise timeout_str
 
@@ -356,14 +418,16 @@
             timeout=timeout_str,
         ).to_dict()
         if isinstance(opts, Exception):
             raise opts
 
         raise base.ResponseInterrupt(
             execution.StepResponse(
-                display_name=parsed_step_id.user_facing,
-                id=parsed_step_id.hashed,
-                name=event,
-                op=execution.Opcode.WAIT_FOR_EVENT,
-                opts=opts,
+                step=execution.StepInfo(
+                    id=parsed_step_id.hashed,
+                    display_name=parsed_step_id.user_facing,
+                    name=event,
+                    op=execution.Opcode.WAIT_FOR_EVENT,
+                    opts=opts,
+                )
             )
         )
```

### Comparing `inngest-0.3.9/inngest/_internal/transforms.py` & `inngest-0.4.0a0/inngest/_internal/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 def get_traceback(err: Exception) -> str:
     return "".join(
         traceback.format_exception(type(err), err, err.__traceback__)
     )
 
 
+def hash_event_key(key: str) -> str:
+    return hashlib.sha256(key.encode("utf-8")).hexdigest()
+
+
 def hash_signing_key(key: str) -> str:
     return hashlib.sha256(
         bytearray.fromhex(remove_signing_key_prefix(key))
     ).hexdigest()
 
 
 def hash_step_id(step_id: str) -> str:
@@ -37,25 +41,23 @@
     prefix = ""
     if prefix_match:
         prefix = prefix_match.group(0)
 
     return key[len(prefix) :]
 
 
-def prep_body(obj: types.T) -> types.T:
+def deep_strip_none(obj: types.T) -> types.T:
     """
-    Prep body before sending to the Inngest server. This function will:
-    - Remove items whose value is None.
-    - Convert keys to camelCase.
+    Recursively remove items whose value is None.
     """
 
     if isinstance(obj, dict):
-        return {k: prep_body(v) for k, v in obj.items() if v is not None}  # type: ignore
+        return {k: deep_strip_none(v) for k, v in obj.items() if v is not None}  # type: ignore
     if isinstance(obj, list):
-        return [prep_body(v) for v in obj if v is not None]  # type: ignore
+        return [deep_strip_none(v) for v in obj if v is not None]  # type: ignore
     return obj
 
 
 class _Duration:
     @classmethod
     def second(cls, count: int = 1) -> int:
         return count * 1000
@@ -96,23 +98,42 @@
         return f"{ms // _Duration.hour()}h"
     if ms < _Duration.week():
         return f"{ms // _Duration.day()}d"
 
     return f"{ms // _Duration.week()}w"
 
 
+def to_maybe_duration_str(
+    ms: typing.Union[int, datetime.timedelta, None],
+) -> typing.Union[types.MaybeError[str], None]:
+    if ms is None:
+        return None
+    return to_duration_str(ms)
+
+
 def to_iso_utc(value: datetime.datetime) -> str:
     return (
         value.astimezone(datetime.timezone.utc).strftime(
             "%Y-%m-%dT%H:%M:%S.%f"
         )[:-3]
         + "Z"
     )
 
 
+def _to_int(value: typing.Any) -> types.MaybeError[int]:
+    try:
+        return int(value)
+    except Exception as err:
+        return ValueError(f"invalid integer: {err}")
+
+
+def get_major_version(version: str) -> types.MaybeError[int]:
+    return _to_int(version.split(".")[0])
+
+
 def get_server_kind(
     headers: dict[str, str],
 ) -> typing.Union[const.ServerKind, None, Exception]:
     value = headers.get(const.HeaderKey.SERVER_KIND.value, None)
     if value is None:
         return None
```

### Comparing `inngest-0.3.9/inngest/_internal/transforms_test.py` & `inngest-0.4.0a0/inngest/_internal/transforms_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.9/inngest/_internal/types.py` & `inngest-0.4.0a0/inngest/_internal/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 if typing.TYPE_CHECKING:
     # https://github.com/python/typeshed/issues/7855
     Logger = typing.Union[logging.Logger, logging.LoggerAdapter[logging.Logger]]
 else:
     Logger = object
 
 T = typing.TypeVar("T")
+TTuple = typing_extensions.TypeVarTuple("TTuple")
 
 
 class EmptySentinel:
     pass
 
 
 empty_sentinel = EmptySentinel()
```

### Comparing `inngest-0.3.9/inngest/django.py` & `inngest-0.4.0a0/inngest/django.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,38 +25,42 @@
 FRAMEWORK = const.Framework.DJANGO
 
 
 def serve(
     client: client_lib.Inngest,
     functions: list[function.Function],
     *,
-    async_mode: bool = False,
     serve_origin: typing.Optional[str] = None,
     serve_path: typing.Optional[str] = None,
 ) -> django.urls.URLPattern:
     """
     Serve Inngest functions in a Django app.
 
     Args:
     ----
         client: Inngest client.
         functions: List of functions to serve.
 
-        async_mode: Whether to serve functions asynchronously.
+        async_mode: [DEPRECATED] Whether to serve functions asynchronously.
         serve_origin: Origin to serve Inngest from.
         serve_path: Path to serve Inngest from.
     """
 
     handler = comm.CommHandler(
         api_base_url=client.api_origin,
         client=client,
         framework=FRAMEWORK,
         functions=functions,
     )
 
+    async_mode = any(
+        function.is_handler_async or function.is_on_failure_handler_async
+        for function in functions
+    )
+
     if async_mode:
         return _create_handler_async(
             client,
             handler,
             serve_origin=serve_origin,
             serve_path=serve_path,
         )
@@ -91,15 +95,20 @@
             headers=headers,
             mode=client._mode,
         )
 
         if request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind, req_sig),
+                handler.inspect(
+                    serve_origin=serve_origin,
+                    serve_path=serve_path,
+                    server_kind=server_kind,
+                    req_sig=req_sig,
+                ),
                 server_kind,
             )
 
         if request.method == "POST":
             fn_id = request.GET.get(const.QueryParamKey.FUNCTION_ID.value)
             if fn_id is None:
                 raise errors.QueryParamMissingError(
@@ -121,14 +130,15 @@
                 )
 
             return _to_response(
                 client,
                 handler.call_function_sync(
                     call=call,
                     fn_id=fn_id,
+                    raw_request=request,
                     req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if request.method == "PUT":
@@ -162,14 +172,24 @@
 def _create_handler_async(
     client: client_lib.Inngest,
     handler: comm.CommHandler,
     *,
     serve_origin: typing.Optional[str],
     serve_path: typing.Optional[str],
 ) -> django.urls.URLPattern:
+    major_version = transforms.get_major_version(django.get_version())
+    if isinstance(major_version, Exception):
+        client.logger.error(major_version)
+    else:
+        if major_version < 5:
+            # Django 5 introduced async support for csrf_exempt
+            raise Exception(
+                "Django version 5 or higher is required for async mode"
+            )
+
     async def inngest_api(
         request: django.http.HttpRequest,
     ) -> django.http.HttpResponse:
         headers = net.normalize_headers(dict(request.headers.items()))
 
         server_kind = transforms.get_server_kind(headers)
         if isinstance(server_kind, Exception):
@@ -181,15 +201,20 @@
             headers=headers,
             mode=client._mode,
         )
 
         if request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind, req_sig),
+                handler.inspect(
+                    serve_origin=serve_origin,
+                    serve_path=serve_path,
+                    server_kind=server_kind,
+                    req_sig=req_sig,
+                ),
                 server_kind,
             )
 
         if request.method == "POST":
             fn_id = request.GET.get(const.QueryParamKey.FUNCTION_ID.value)
             if fn_id is None:
                 raise errors.QueryParamMissingError(
@@ -211,14 +236,15 @@
                 )
 
             return _to_response(
                 client,
                 await handler.call_function(
                     call=call,
                     fn_id=fn_id,
+                    raw_request=request,
                     req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if request.method == "PUT":
```

### Comparing `inngest-0.3.9/inngest/fast_api.py` & `inngest-0.4.0a0/inngest/fast_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,18 @@
         if isinstance(server_kind, Exception):
             client.logger.error(server_kind)
             server_kind = None
 
         return _to_response(
             client,
             handler.inspect(
-                server_kind,
-                net.RequestSignature(
+                serve_origin=serve_origin,
+                serve_path=serve_path,
+                server_kind=server_kind,
+                req_sig=net.RequestSignature(
                     body=body,
                     headers=headers,
                     mode=client._mode,
                 ),
             ),
             server_kind,
         )
@@ -94,14 +96,15 @@
             )
 
         return _to_response(
             client,
             await handler.call_function(
                 call=call,
                 fn_id=fnId,
+                raw_request=request,
                 req_sig=net.RequestSignature(
                     body=body,
                     headers=headers,
                     mode=client._mode,
                 ),
                 target_hashed_id=stepId,
             ),
```

### Comparing `inngest-0.3.9/inngest/flask.py` & `inngest-0.4.0a0/inngest/flask.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,20 @@
             headers=headers,
             mode=client._mode,
         )
 
         if flask.request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind, req_sig),
+                handler.inspect(
+                    serve_origin=serve_origin,
+                    serve_path=serve_path,
+                    server_kind=server_kind,
+                    req_sig=req_sig,
+                ),
                 server_kind,
             )
 
         if flask.request.method == "POST":
             fn_id = flask.request.args.get(
                 const.QueryParamKey.FUNCTION_ID.value
             )
@@ -123,30 +128,34 @@
                 )
 
             return _to_response(
                 client,
                 await handler.call_function(
                     call=call,
                     fn_id=fn_id,
+                    raw_request=flask.request,
                     req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if flask.request.method == "PUT":
+            sync_id = flask.request.args.get(const.QueryParamKey.SYNC_ID.value)
+
             return _to_response(
                 client,
                 await handler.register(
                     app_url=net.create_serve_url(
                         request_url=flask.request.url,
                         serve_origin=serve_origin,
                         serve_path=serve_path,
                     ),
                     server_kind=server_kind,
+                    sync_id=sync_id,
                 ),
                 server_kind,
             )
 
         # Should be unreachable
         return ""
 
@@ -173,15 +182,20 @@
             headers=headers,
             mode=client._mode,
         )
 
         if flask.request.method == "GET":
             return _to_response(
                 client,
-                handler.inspect(server_kind, req_sig),
+                handler.inspect(
+                    serve_origin=serve_origin,
+                    serve_path=serve_path,
+                    server_kind=server_kind,
+                    req_sig=req_sig,
+                ),
                 server_kind,
             )
 
         if flask.request.method == "POST":
             fn_id = flask.request.args.get(
                 const.QueryParamKey.FUNCTION_ID.value
             )
@@ -205,14 +219,15 @@
                 )
 
             return _to_response(
                 client,
                 handler.call_function_sync(
                     call=call,
                     fn_id=fn_id,
+                    raw_request=flask.request,
                     req_sig=req_sig,
                     target_hashed_id=step_id,
                 ),
                 server_kind,
             )
 
         if flask.request.method == "PUT":
```

### Comparing `inngest-0.3.9/inngest/tornado.py` & `inngest-0.4.0a0/inngest/tornado.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,20 @@
 
             req_sig = net.RequestSignature(
                 body=self.request.body,
                 headers=headers,
                 mode=client._mode,
             )
 
-            comm_res = handler.inspect(server_kind, req_sig)
+            comm_res = handler.inspect(
+                serve_origin=serve_origin,
+                serve_path=serve_path,
+                server_kind=server_kind,
+                req_sig=req_sig,
+            )
 
             self._write_comm_response(comm_res, server_kind)
 
         def post(self) -> None:
             fn_id: typing.Optional[str]
             raw_fn_id = self.request.query_arguments.get(
                 const.QueryParamKey.FUNCTION_ID.value
@@ -110,14 +115,15 @@
                     comm.CommResponse.from_error(client.logger, call),
                     server_kind,
                 )
 
             comm_res = handler.call_function_sync(
                 call=call,
                 fn_id=fn_id,
+                raw_request=self.request,
                 req_sig=req_sig,
                 target_hashed_id=step_id,
             )
 
             self._write_comm_response(comm_res, server_kind)
 
         def put(self) -> None:
```

### Comparing `inngest-0.3.9/inngest.egg-info/PKG-INFO` & `inngest-0.4.0a0/inngest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: inngest
-Version: 0.3.9
+Version: 0.4.0a0
 Summary: Python SDK for Inngest
 Project-URL: Homepage, https://github.com/inngest/inngest-py
 Project-URL: Bug Tracker, https://github.com/inngest/inngest-py/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,21 +19,24 @@
 Requires-Dist: httpx>=0.24.0
 Requires-Dist: pydantic>=2.1.1
 Requires-Dist: typing-extensions>=4.8.0
 Provides-Extra: extra
 Requires-Dist: Django==4.2; extra == "extra"
 Requires-Dist: Flask==2.3.0; extra == "extra"
 Requires-Dist: build==1.0.3; extra == "extra"
+Requires-Dist: cryptography==42.0.5; extra == "extra"
 Requires-Dist: django-types==0.19.1; extra == "extra"
 Requires-Dist: fastapi==0.100.0; extra == "extra"
 Requires-Dist: mypy==1.8.0; extra == "extra"
+Requires-Dist: pynacl==1.5.0; extra == "extra"
 Requires-Dist: pytest==7.4.2; extra == "extra"
 Requires-Dist: pytest-django==4.7.0; extra == "extra"
 Requires-Dist: pytest-xdist[psutil]==3.3.1; extra == "extra"
 Requires-Dist: ruff==0.1.9; extra == "extra"
+Requires-Dist: sentry-sdk==2.1.1; extra == "extra"
 Requires-Dist: toml==0.10.2; extra == "extra"
 Requires-Dist: tornado==6.3; extra == "extra"
 Requires-Dist: types-toml==0.10.8.7; extra == "extra"
 Requires-Dist: types-tornado==5.1.1; extra == "extra"
 Requires-Dist: uvicorn==0.23.2; extra == "extra"
 
 <div align="center">
@@ -57,18 +60,17 @@
   </p>
 </div>
 
 <hr />
 
 # Inngest Python SDK
 
-> 🚧 Currently in beta! Users have deployed our Python SDK in their production environments but it isn't as battle-tested as our TypeScript SDK.
-
 We currently support the following frameworks (but adding a new framework is easy!):
 
+- DigitalOcean Functions
 - Django (`>=4.2`)
 - FastAPI (`>=0.100.0`)
 - Flask (`>=2.3.0`)
 - Tornado (`>=6.3`)
 
 Python 3.9 is the minimum version we support.
 
@@ -181,15 +183,15 @@
     def _fetch_ship(url: str) -> dict:
         res = requests.get(url)
         return res.json()
 
     ship_names = []
     for ship_url in person["starships"]:
         # step.run works in loops!
-        ship = step.run("fetch_ship", lambda: _fetch_ship(ship_url))
+        ship = step.run("fetch_ship", _fetch_ship, ship_url)
 
         ship_names.append(ship["name"])
 
     return {
         "person_name": person["name"],
         "ship_names": ship_names,
     }
```

#### html2text {}

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1 Name: inngest Version: 0.3.9 Summary: Python SDK for
+Metadata-Version: 2.1 Name: inngest Version: 0.4.0a0 Summary: Python SDK for
 Inngest Project-URL: Homepage, https://github.com/inngest/inngest-py Project-
 URL: Bug Tracker, https://github.com/inngest/inngest-py/issues Classifier:
-Development Status :: 4 - Beta Classifier: Framework :: Django Classifier:
-Framework :: FastAPI Classifier: Framework :: Flask Classifier: Intended
-Audience :: Developers Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Development Status :: 5 - Production/Stable Classifier: Framework :: Django
+Classifier: Framework :: FastAPI Classifier: Framework :: Flask Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python ::
+3.9 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: httpx>=0.24.0 Requires-Dist: pydantic>=2.1.1
 Requires-Dist: typing-extensions>=4.8.0 Provides-Extra: extra Requires-Dist:
 Django==4.2; extra == "extra" Requires-Dist: Flask==2.3.0; extra == "extra"
-Requires-Dist: build==1.0.3; extra == "extra" Requires-Dist: django-
-types==0.19.1; extra == "extra" Requires-Dist: fastapi==0.100.0; extra ==
-"extra" Requires-Dist: mypy==1.8.0; extra == "extra" Requires-Dist:
-pytest==7.4.2; extra == "extra" Requires-Dist: pytest-django==4.7.0; extra ==
-"extra" Requires-Dist: pytest-xdist[psutil]==3.3.1; extra == "extra" Requires-
-Dist: ruff==0.1.9; extra == "extra" Requires-Dist: toml==0.10.2; extra ==
+Requires-Dist: build==1.0.3; extra == "extra" Requires-Dist:
+cryptography==42.0.5; extra == "extra" Requires-Dist: django-types==0.19.1;
+extra == "extra" Requires-Dist: fastapi==0.100.0; extra == "extra" Requires-
+Dist: mypy==1.8.0; extra == "extra" Requires-Dist: pynacl==1.5.0; extra ==
+"extra" Requires-Dist: pytest==7.4.2; extra == "extra" Requires-Dist: pytest-
+django==4.7.0; extra == "extra" Requires-Dist: pytest-xdist[psutil]==3.3.1;
+extra == "extra" Requires-Dist: ruff==0.1.9; extra == "extra" Requires-Dist:
+sentry-sdk==2.1.1; extra == "extra" Requires-Dist: toml==0.10.2; extra ==
 "extra" Requires-Dist: tornado==6.3; extra == "extra" Requires-Dist: types-
 toml==0.10.8.7; extra == "extra" Requires-Dist: types-tornado==5.1.1; extra ==
 "extra" Requires-Dist: uvicorn==0.23.2; extra == "extra"
 
 _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_3_0_6_1_7_7_/_1_9_1_5_8_0_7_1_7_-_1_f_5_6_3_f_4_c_-_3_1_e_3_-_4_a_a_0_-
                             _8_4_8_c_-_5_d_d_c_9_7_8_0_8_a_9_a_._p_n_g_]
 
@@ -28,31 +30,29 @@
               Read the _d_o_c_u_m_e_n_t_a_t_i_o_n and get started in minutes.
  [![pypi](https://img.shields.io/pypi/v/inngest.svg)](https://pypi.python.org/
 pypi/inngest) ![versions](https://img.shields.io/pypi/pyversions/inngest.svg)
  [![discord](https://img.shields.io/discord/842170679536517141?label=discord)]
  (https://www.inngest.com/discord) [![twitter](https://img.shields.io/twitter/
           follow/inngest?style=social)](https://twitter.com/inngest)
 ===============================================================================
-# Inngest Python SDK > ð§ Currently in beta! Users have deployed our Python
-SDK in their production environments but it isn't as battle-tested as our
-TypeScript SDK. We currently support the following frameworks (but adding a new
-framework is easy!): - Django (`>=4.2`) - FastAPI (`>=0.100.0`) - Flask
-(`>=2.3.0`) - Tornado (`>=6.3`) Python 3.9 is the minimum version we support.
-## Getting started Install `inngest` in your project: ```sh pip install inngest
-``` Write a basic function and serve it (see the [basic](#basic-no-steps)
-example for guidance). Start the Dev Server (the local version of our cloud
-platform): ```sh npx inngest-cli@latest dev ``` Browse to http://127.0.0.1:8288
-and you should see your app! Visit our docs to read more about the [Dev Server]
-(https://www.inngest.com/docs/local-development). ## Examples > ð¡ You can
-mix `async` and non-`async` functions in the same app! - [Basic](#basic-no-
-steps) - [Step run](#step-run) - [Async function](#async-function) ### Basic
-(no steps) This is a minimal example of an Inngest function. It's missing some
-of our features but it's a good starting point. ```py import flask import
-inngest.flask import requests inngest_client = inngest.Inngest
-( app_id="flask_example", is_production=False, )
+# Inngest Python SDK We currently support the following frameworks (but adding
+a new framework is easy!): - DigitalOcean Functions - Django (`>=4.2`) -
+FastAPI (`>=0.100.0`) - Flask (`>=2.3.0`) - Tornado (`>=6.3`) Python 3.9 is the
+minimum version we support. ## Getting started Install `inngest` in your
+project: ```sh pip install inngest ``` Write a basic function and serve it (see
+the [basic](#basic-no-steps) example for guidance). Start the Dev Server (the
+local version of our cloud platform): ```sh npx inngest-cli@latest dev ```
+Browse to http://127.0.0.1:8288 and you should see your app! Visit our docs to
+read more about the [Dev Server](https://www.inngest.com/docs/local-
+development). ## Examples > ð¡ You can mix `async` and non-`async` functions
+in the same app! - [Basic](#basic-no-steps) - [Step run](#step-run) - [Async
+function](#async-function) ### Basic (no steps) This is a minimal example of an
+Inngest function. It's missing some of our features but it's a good starting
+point. ```py import flask import inngest.flask import requests inngest_client =
+inngest.Inngest( app_id="flask_example", is_production=False, )
 @inngest_client.create_function( fn_id="find_person",
 trigger=inngest.TriggerEvent(event="app/person.find"), ) def fetch_person( ctx:
 inngest.Context, step: inngest.StepSync, ) -> dict: person_id = ctx.event.data
 ["person_id"] res = requests.get(f"https://swapi.dev/api/people/{person_id}")
 return res.json() app = flask.Flask(__name__) # Register functions with the
 Inngest server inngest.flask.serve( app, inngest_client, [fetch_person], )
 app.run(port=8000) ``` Send the following event in the Dev Server UI and the
@@ -64,16 +64,16 @@
 trigger=inngest.TriggerEvent(event="app/ships.find"), ) def fetch_ships( ctx:
 inngest.Context, step: inngest.StepSync, ) -> dict: """ Find all the ships a
 person has. """ person_id = ctx.event.data["person_id"] def _fetch_person() -
 > dict: res = requests.get(f"https://swapi.dev/api/people/{person_id}") return
 res.json() # Wrap the function with step.run to enable retries person =
 step.run("fetch_person", _fetch_person) def _fetch_ship(url: str) -> dict: res
 = requests.get(url) return res.json() ship_names = [] for ship_url in person
-["starships"]: # step.run works in loops! ship = step.run("fetch_ship", lambda:
-_fetch_ship(ship_url)) ship_names.append(ship["name"]) return { "person_name":
+["starships"]: # step.run works in loops! ship = step.run("fetch_ship",
+_fetch_ship, ship_url) ship_names.append(ship["name"]) return { "person_name":
 person["name"], "ship_names": ship_names, } ``` Send the following event in the
 Dev Server UI and the `fetch_person` function will run: ```json { "name": "app/
 ships.find", "data": { "person_id": 1 } } ``` ### Async function ```py
 @inngest_client.create_function( fn_id="find_person",
 trigger=inngest.TriggerEvent(event="app/person.find"), ) async def fetch_person
 ( ctx: inngest.Context, step: inngest.Step, ) -> dict: person_id =
 ctx.event.data["person_id"] async with httpx.AsyncClient() as client: res =
```

### Comparing `inngest-0.3.9/inngest.egg-info/SOURCES.txt` & `inngest-0.4.0a0/inngest.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 LICENSE.md
 README.md
 pyproject.toml
 inngest/__init__.py
+inngest/digital_ocean.py
 inngest/django.py
-inngest/experimental.py
 inngest/fast_api.py
 inngest/flask.py
 inngest/py.typed
 inngest/tornado.py
 inngest.egg-info/PKG-INFO
 inngest.egg-info/SOURCES.txt
 inngest.egg-info/dependency_links.txt
 inngest.egg-info/requires.txt
 inngest.egg-info/top_level.txt
 inngest/_internal/__init__.py
-inngest/_internal/client_lib.py
-inngest/_internal/client_lib_test.py
+inngest/_internal/async_lib.py
 inngest/_internal/comm.py
 inngest/_internal/comm_test.py
 inngest/_internal/const.py
 inngest/_internal/const_test.py
 inngest/_internal/env_lib.py
 inngest/_internal/errors.py
 inngest/_internal/event_lib.py
@@ -31,21 +30,24 @@
 inngest/_internal/log.py
 inngest/_internal/net.py
 inngest/_internal/net_test.py
 inngest/_internal/registration.py
 inngest/_internal/transforms.py
 inngest/_internal/transforms_test.py
 inngest/_internal/types.py
+inngest/_internal/client_lib/__init__.py
+inngest/_internal/client_lib/client.py
+inngest/_internal/client_lib/client_test.py
+inngest/_internal/client_lib/models.py
 inngest/_internal/middleware_lib/__init__.py
 inngest/_internal/middleware_lib/log.py
 inngest/_internal/middleware_lib/manager.py
 inngest/_internal/middleware_lib/middleware.py
 inngest/_internal/step_lib/__init__.py
 inngest/_internal/step_lib/base.py
 inngest/_internal/step_lib/step_async.py
 inngest/_internal/step_lib/step_sync.py
-tests/test_client.py
-tests/test_django.py
-tests/test_fast_api.py
-tests/test_flask.py
-tests/test_tornado.py
+inngest/experimental/__init__.py
+inngest/experimental/digital_ocean_simulator.py
+inngest/experimental/encryption_middleware.py
+inngest/experimental/sentry_middleware.py
 tests/test_types.py
```

### Comparing `inngest-0.3.9/pyproject.toml` & `inngest-0.4.0a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "inngest"
-version = "0.3.9"
+version = "0.4.0a0"
 description = "Python SDK for Inngest"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: Django",
     "Framework :: FastAPI",
     "Framework :: Flask",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -19,21 +19,24 @@
 dependencies = ["httpx>=0.24.0", "pydantic>=2.1.1", "typing-extensions>=4.8.0"]
 
 [project.optional-dependencies]
 extra = [
     "Django==4.2",
     "Flask==2.3.0",
     "build==1.0.3",
+    "cryptography==42.0.5",
     "django-types==0.19.1",
     "fastapi==0.100.0",
     "mypy==1.8.0",
+    "pynacl==1.5.0",
     "pytest==7.4.2",
     "pytest-django==4.7.0",
     "pytest-xdist[psutil]==3.3.1",
     "ruff==0.1.9",
+    "sentry-sdk==2.1.1",
     "toml==0.10.2",
     "tornado==6.3",
     "types-toml==0.10.8.7",
     "types-tornado==5.1.1",
     "uvicorn==0.23.2",
 ]
 
@@ -98,19 +101,20 @@
     'D415',
 
     # Can't use the "|" operator for unions until we drop support for Python 3.9
     'UP007',
 ]
 
 line-length = 80
-mccabe = { max-complexity = 16 }
+mccabe = { max-complexity = 21 }
 
 [tool.ruff.extend-per-file-ignores]
 "examples/**/*.py" = ['D', 'T20']
 "inngest/**/*_test.py" = ['C901', 'D', 'N', 'S', 'T20']
+"inngest/experimental/**/*.py" = ['D102', 'D417']
 "tests/**/*.py" = ['C901', 'D', 'N', 'S', 'T20']
 
 [tool.ruff.lint]
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 
 [tool.setuptools.package-data]
```

