# Comparing `tmp/globus-compute-sdk-2.8.0a0.tar.gz` & `tmp/globus-compute-sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.8.0a0.tar", last modified: Mon Nov 20 20:48:27 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.9.0.tar", last modified: Wed Dec 13 21:50:22 2023, max compression
```

## Comparing `globus-compute-sdk-2.8.0a0.tar` & `globus-compute-sdk-2.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.540834 globus-compute-sdk-2.8.0a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.8.0a0/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     2896 2023-11-20 20:48:27.540758 globus-compute-sdk-2.8.0a0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.8.0a0/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.531455 globus-compute-sdk-2.8.0a0/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.532391 globus-compute-sdk-2.8.0a0/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      408 2023-11-20 20:37:16.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2352 2023-11-20 20:37:16.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.534940 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1472 2023-09-25 16:37:20.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.535627 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)     3063 2023-08-17 23:30:28.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    26120 2023-11-15 20:50:22.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    56018 2023-11-08 18:25:44.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.537910 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      328 2023-11-01 17:16:05.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1836 2023-11-01 17:16:05.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/authorizer_login_manager.py
--rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7287 2023-06-12 17:16:14.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     3043 2023-11-09 20:18:47.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.538626 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)     2281 2023-10-05 20:40:40.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-08-17 22:25:07.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)      470 2023-08-17 23:30:28.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/utils/uuid_like.py
--rw-r--r--   0 lei        (501) staff       (20)     9824 2023-11-15 20:50:22.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.539347 globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      603 2023-08-17 23:30:28.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1098 2023-11-20 20:37:16.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     8107 2023-11-20 20:37:16.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     4868 2023-11-20 20:37:16.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)      834 2023-11-20 20:47:34.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-11-20 20:48:27.539582 globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     2896 2023-11-20 20:48:27.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1601 2023-11-20 20:48:27.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-11-20 20:48:27.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      469 2023-11-20 20:48:27.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-11-20 20:48:27.000000 globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-11-20 20:48:27.541097 globus-compute-sdk-2.8.0a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3228 2023-11-08 21:31:30.000000 globus-compute-sdk-2.8.0a0/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.677605 globus-compute-sdk-2.9.0/
+-rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 20:09:04.000000 globus-compute-sdk-2.9.0/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     2894 2023-12-13 21:50:22.677456 globus-compute-sdk-2.9.0/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      816 2023-04-17 20:09:04.000000 globus-compute-sdk-2.9.0/PyPI.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.663410 globus-compute-sdk-2.9.0/globus_compute_sdk/
+-rw-r--r--   0 chris      (501) staff       (20)      433 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.664877 globus-compute-sdk-2.9.0/globus_compute_sdk/errors/
+-rw-r--r--   0 chris      (501) staff       (20)      408 2023-11-29 16:02:16.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     3288 2023-12-13 16:13:12.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.667769 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1472 2023-11-01 18:57:58.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.668642 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      648 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 chris      (501) staff       (20)      724 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 chris      (501) staff       (20)     3063 2023-08-04 15:59:53.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 chris      (501) staff       (20)    26120 2023-11-15 19:59:40.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 chris      (501) staff       (20)     2400 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 chris      (501) staff       (20)    56435 2023-12-13 16:13:12.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.672096 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 chris      (501) staff       (20)      328 2023-11-06 17:11:40.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1836 2023-11-06 17:11:40.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/authorizer_login_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)     1787 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 chris      (501) staff       (20)      855 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 chris      (501) staff       (20)      373 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 chris      (501) staff       (20)      954 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 chris      (501) staff       (20)     7287 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 chris      (501) staff       (20)      710 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 chris      (501) staff       (20)     3043 2023-11-10 18:11:31.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 chris      (501) staff       (20)     2190 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.672986 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 chris      (501) staff       (20)     2281 2023-10-25 19:12:38.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1207 2023-04-12 14:51:48.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 chris      (501) staff       (20)      470 2023-07-24 19:26:40.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/utils/uuid_like.py
+-rw-r--r--   0 chris      (501) staff       (20)     9824 2023-11-15 19:59:40.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.675260 globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/
+-rw-r--r--   0 chris      (501) staff       (20)      603 2023-06-08 19:30:56.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1098 2023-11-29 16:02:16.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     8107 2023-11-29 16:02:16.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 chris      (501) staff       (20)     4868 2023-11-29 16:02:16.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 chris      (501) staff       (20)      832 2023-12-13 16:28:29.000000 globus-compute-sdk-2.9.0/globus_compute_sdk/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-12-13 21:50:22.675687 globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     2894 2023-12-13 21:50:22.000000 globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     1601 2023-12-13 21:50:22.000000 globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-12-13 21:50:22.000000 globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      469 2023-12-13 21:50:22.000000 globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       19 2023-12-13 21:50:22.000000 globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      282 2023-12-13 21:50:22.678025 globus-compute-sdk-2.9.0/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     3228 2023-11-10 18:11:31.000000 globus-compute-sdk-2.9.0/setup.py
```

### Comparing `globus-compute-sdk-2.8.0a0/LICENSE` & `globus-compute-sdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/PKG-INFO` & `globus-compute-sdk-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.8.0a0
+Version: 2.9.0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.8.0a0/PyPI.md` & `globus-compute-sdk-2.9.0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/errors/error_types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import re
 import textwrap
 import time
 
 
 class ComputeError(Exception):
     """Base class for all funcx exceptions"""
 
@@ -66,25 +67,49 @@
     def __str__(self) -> str:
         return (
             f"Task result of {self.result_size}B exceeded current "
             f"limit of {self.result_size_limit}B"
         )
 
 
+SERDE_TASK_EXECUTION_FAILED_HELP_MESSAGE = """
+
+This appears to be an error with serialization. If it is, using a different
+serialization strategy from globus_compute_sdk.serialize might resolve the issue. For
+example, to use globus_compute_sdk.serialize.CombinedCode:
+
+    from globus_compute_sdk import Client, Executor
+    from globus_compute_sdk.serialize import CombinedCode
+
+    gcc = Client(code_serialization_strategy=CombinedCode())
+    with Executor('<your-endpoint-id>', client=gcc) as gcx:
+        # do something with gcx
+
+For more information, see:
+    https://globus-compute.readthedocs.io/en/latest/sdk.html#specifying-a-serialization-strategy
+"""
+
+
 class TaskExecutionFailed(Exception):
     """
     Error result from the remote end, wrapped as an exception object
     """
 
+    SERDE_REGEX = re.compile("dill|pickle|serializ", re.IGNORECASE)
+
     def __init__(
         self,
         remote_data: str,
         completion_t: str | None = None,
         task_details: dict | None = None,
     ):
         self.remote_data = remote_data
         self.task_details = task_details
         # Fill in completion time if missing
         self.completion_t = completion_t or str(time.time())
 
     def __str__(self) -> str:
-        return "\n" + textwrap.indent(self.remote_data, " ")
+        remote_data = textwrap.indent(self.remote_data, " ")
+        message = "\n" + remote_data
+        if re.search(TaskExecutionFailed.SERDE_REGEX, remote_data):
+            message += SERDE_TASK_EXECUTION_FAILED_HELP_MESSAGE
+        return message
```

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/_environments.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,57 +111,66 @@
     .. _Executor: https://docs.python.org/3/library/concurrent.futures.html#executor-objects
     """  # noqa
 
     def __init__(
         self,
         endpoint_id: UUID_LIKE_T | None = None,
         container_id: UUID_LIKE_T | None = None,
-        funcx_client: Client | None = None,
+        client: Client | None = None,
         task_group_id: UUID_LIKE_T | None = None,
         user_endpoint_config: dict[str, t.Any] | None = None,
         label: str = "",
         batch_size: int = 128,
+        funcx_client: Client | None = None,
         amqp_port: int | None = None,
         **kwargs,
     ):
         """
         :param endpoint_id: id of the endpoint to which to submit tasks
         :param container_id: id of the container in which to execute tasks
-        :param funcx_client: instance of Client to be used by the
-            executor.  If not provided, the executor will instantiate one with default
-            arguments.
+        :param client: instance of Client to be used by the executor.  If not provided,
+            the executor will instantiate one with default arguments.
         :param task_group_id: The Task Group to which to associate tasks.  If not set,
             one will be instantiated.
         :param user_endpoint_config: User endpoint configuration values as described
             and allowed by endpoint administrators. Must be a JSON-serializable dict
             or None.
         :param label: a label to name the executor; mainly utilized for
             logging and advanced needs with multiple executors.
         :param batch_size: the maximum number of tasks to coalesce before
             sending upstream [min: 1, default: 128]
+        :param funcx_client: [DEPRECATED] alias for client.
         :param batch_interval: [DEPRECATED; unused] number of seconds to coalesce tasks
             before submitting upstream
         :param batch_enabled: [DEPRECATED; unused] whether to batch results
         :param amqp_port: Port to use when connecting to results queue. Note that the
             Compute web services only support 5671, 5672, and 443.
         """
         deprecated_kwargs = {"batch_interval", "batch_enabled"}
         for key in kwargs:
             if key in deprecated_kwargs:
                 warnings.warn(
-                    f"`{key}` is not utilized and will be removed in a future release",
+                    f"'{key}' is not utilized and will be removed in a future release",
                     DeprecationWarning,
                 )
                 continue
             msg = f"'{key}' is an invalid argument for {self.__class__.__name__}"
             raise TypeError(msg)
 
-        if not funcx_client:
-            funcx_client = Client()
-        self.funcx_client = funcx_client
+        if funcx_client:
+            warnings.warn(
+                "'funcx_client' is superseded by 'client'"
+                " and will be removed in a future release",
+                DeprecationWarning,
+            )
+
+        if not client:
+            client = funcx_client if funcx_client else Client()
+
+        self.client = client
 
         self.endpoint_id = endpoint_id
 
         # mypy ... sometimes you just ain't too bright
         self.container_id = container_id  # type: ignore[assignment]
 
         self._task_group_id: uuid.UUID | None = None  # help mypy out
@@ -183,15 +192,15 @@
         self._function_registry: dict[tuple[t.Callable, str | None], str] = {}
 
         self._stopped = False
         self._stopped_in_error = False
         self._shutdown_lock = threading.RLock()
         self._result_watcher: _ResultWatcher | None = None
 
-        log.debug("%s: initiated on thread: %s", self, threading.get_ident())
+        log.debug("%r: initiated on thread: %s", self, threading.get_ident())
         self._task_submitter = threading.Thread(
             target=self._task_submitter_impl, name="TaskSubmitter"
         )
         self._task_submitter.start()
         _REGISTERED_FXEXECUTORS[id(self)] = self
 
     def __repr__(self) -> str:
@@ -349,16 +358,15 @@
             ``fn`` immediately, short-circuiting the upstream registration call.
         :param func_register_kwargs: all other keyword arguments are passed to
             the ``Client.register_function()``.
         :returns: the function's ``function_id`` string, as returned by
             registration upstream
         """
         if self._stopped:
-            err_fmt = "%s is shutdown; refusing to register function"
-            raise RuntimeError(err_fmt % repr(self))
+            raise RuntimeError(f"{self!r} is shutdown; refusing to register function")
 
         fn_cache_key = self._fn_cache_key(fn)
         if fn_cache_key in self._function_registry:
             msg = f"Function already registered as function id: {function_id}"
             log.error(msg)
             self.shutdown(wait=False, cancel_futures=True)
             raise ValueError(msg)
@@ -376,15 +384,15 @@
                 "python_version": platform.python_version(),
                 "sdk_version": __version__,
             },
         }
         reg_kwargs.update(func_register_kwargs)
 
         try:
-            func_reg_id = self.funcx_client.register_function(fn, **reg_kwargs)
+            func_reg_id = self.client.register_function(fn, **reg_kwargs)
         except Exception:
             log.error(f"Unable to register function: {fn.__name__}")
             self.shutdown(wait=False, cancel_futures=True)
             raise
         self._function_registry[fn_cache_key] = func_reg_id
         log.debug("Function registered with id: %s", func_reg_id)
         return func_reg_id
@@ -414,16 +422,16 @@
         :param kwargs: keyword arguments (if any) as required to execute
             the function
         :returns: a future object that will receive a ``.task_id`` when the
             Globus Compute Web Service acknowledges receipt, and eventually will have
             a ``.result()`` when the Globus Compute web services receive and stream it.
         """
         if self._stopped:
-            err_fmt = "%s is shutdown; no new functions may be executed"
-            raise RuntimeError(err_fmt % repr(self))
+            err = f"{self!r} is shutdown; no new functions may be executed"
+            raise RuntimeError(err)
 
         fn_cache_key = self._fn_cache_key(fn)
         if fn_cache_key not in self._function_registry:
             self.register_function(fn)
 
         fn_id = self._function_registry[fn_cache_key]
         return self.submit_to_registered_function(
@@ -481,16 +489,16 @@
             the function
         :param kwargs: keyword arguments (if any) as required to execute
             the function
         :returns: a future object that (eventually) will have a ``.result()``
             when the Globus Compute web services receive and stream it.
         """
         if self._stopped:
-            err_fmt = "%s is shutdown; no new functions may be executed"
-            raise RuntimeError(err_fmt % repr(self))
+            err = f"{self!r} is shutdown; no new functions may be executed"
+            raise RuntimeError(err)
 
         if not self.endpoint_id:
             msg = (
                 "No endpoint_id set.  Did you forget to set it at construction?\n"
                 "  Hint:\n\n"
                 "    gce = Executor(endpoint_id=<ep_id>)\n"
                 "    gce.endpoint_id = <ep_id>    # alternative"
@@ -532,17 +540,24 @@
         we have decided to look at this at a future date if there is interest.
 
         .. _.map(): https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.Executor.map
         .. _Executor interface: https://docs.python.org/3/library/concurrent.futures.html#executor-objects
 
         Raises
         ------
+        RuntimeError
+          if called after shutdown, otherwise, ...
+
         NotImplementedError
-          always raised
+          ... always raised
         """  # noqa
+        if self._stopped:
+            err = f"{self!r} is shutdown; no new functions may be executed"
+            raise RuntimeError(err)
+
         raise NotImplementedError()
 
     def reload_tasks(
         self, task_group_id: UUID_LIKE_T | None = None
     ) -> t.Iterable[ComputeFuture]:
         """
         .. _reload_tasks():
@@ -575,15 +590,15 @@
             self._result_watcher.shutdown(wait=False, cancel_futures=True)
             self._result_watcher = None
 
         task_group_id = self.task_group_id  # snapshot
         assert task_group_id is not None  # mypy: we _just_ proved this
 
         # step 2: from server, acquire list of related task ids and make futures
-        r = self.funcx_client.web_client.get_taskgroup_tasks(task_group_id)
+        r = self.client.web_client.get_taskgroup_tasks(task_group_id)
         if r["taskgroup_id"] != str(task_group_id):
             msg = (
                 "Server did not respond with requested TaskGroup Tasks.  "
                 f"(Requested tasks for {task_group_id} but received "
                 f"tasks for {r['taskgroup_id']}"
             )
             raise ValueError(msg)
@@ -591,15 +606,15 @@
         # step 3: create the associated set of futures
         task_ids: list[str] = [task["id"] for task in r.get("tasks", [])]
         futures: list[ComputeFuture] = []
 
         if task_ids:
             # Complete the futures that already have results.
             pending: list[ComputeFuture] = []
-            deserialize = self.funcx_client.fx_serializer.deserialize
+            deserialize = self.client.fx_serializer.deserialize
             chunk_size = 1024
             num_chunks = len(task_ids) // chunk_size + 1
             for chunk_no, id_chunk in enumerate(
                 chunk_by(task_ids, chunk_size), start=1
             ):
                 if num_chunks > 1:
                     log.debug(
@@ -607,15 +622,15 @@
                         " (%s tasks)",
                         len(task_ids),
                         num_chunks,
                         chunk_no,
                         len(id_chunk),
                     )
 
-                res = self.funcx_client.web_client.get_batch_status(id_chunk)
+                res = self.client.web_client.get_batch_status(id_chunk)
                 for task_id, task in res.data.get("results", {}).items():
                     fut = ComputeFuture(task_id)
                     futures.append(fut)
                     completed_t = task.get("completion_t")
                     if not completed_t:
                         pending.append(fut)
                     else:
@@ -642,18 +657,18 @@
             log.warning(f"Received no tasks for Task Group ID: {task_group_id}")
 
         # step 5: the goods for the consumer
         return futures
 
     def shutdown(self, wait=True, *, cancel_futures=False):
         thread_id = threading.get_ident()
-        log.debug("%s: initiating shutdown (thread: %s)", self, thread_id)
+        log.debug("%r: initiating shutdown (thread: %s)", self, thread_id)
         if self._task_submitter.is_alive():
             log.debug(
-                "%s: %s still alive; sending poison pill",
+                "%r: %s still alive; sending poison pill",
                 self,
                 self._task_submitter.name,
             )
             self._tasks_to_send.put((None, None))
             if wait and self._task_submitter.ident != thread_id:
                 while self._task_submitter.is_alive():
                     self._task_submitter.join(0.1)
@@ -667,30 +682,30 @@
         if thread_id != self._task_submitter.ident and self._stopped_in_error:
             # In an unhappy path scenario, there's the potential for multiple
             # tracebacks, which means that the tracebacks will likely be
             # interwoven in the logs.  Attempt to make debugging easier for
             # that scenario by adding a slight delay on the *main* thread.
             time.sleep(0.1)
         _REGISTERED_FXEXECUTORS.pop(id(self), None)
-        log.debug("%s: shutdown complete (thread: %s)", self, thread_id)
+        log.debug("%r: shutdown finished (thread: %s)", self, thread_id)
 
     def _task_submitter_impl(self) -> None:
         """
         Coalesce tasks from the interthread queue (``_tasks_to_send``), up to
         ``self.batch_size``, submit them, and then send the futures to the
         ResultWatcher.
 
         The main job of this method is to loop forever, forwarding task
         requests upstream and the associated futures to the ResultWatcher.
 
         This thread stops when it receives a poison-pill of ``(None, None)``
         in the queue.  (See ``shutdown()``.)
         """
         log.debug(
-            "%s: task submission thread started (%s)", self, threading.get_ident()
+            "%r: task submission thread started (%s)", self, threading.get_ident()
         )
         to_send = self._tasks_to_send  # cache lookup
 
         # Alias types -- this awkward typing is all about the dict we use
         # internally to make sure we appropriately group tasks for upstream
         # submission.  For example, if the user submitted to two different
         # endpoints, we separate the tasks by the dictionary key.
@@ -796,40 +811,40 @@
                     task_count -= 1
                     to_send.task_done()
 
         except Exception as exc:
             self._stopped = True
             self._stopped_in_error = True
             log.debug(
-                "%s: task submission thread encountered error ([%s] %s)",
+                "%r: task submission thread encountered error ([%s] %s)",
                 self,
                 exc.__class__.__name__,
                 exc,
             )
 
             if self._shutdown_lock.acquire(blocking=False):
                 self.shutdown(wait=False, cancel_futures=True)
                 self._shutdown_lock.release()
 
-            log.debug("%s: task submission thread dies", self)
+            log.debug("%r: task submission thread dies", self)
             raise
         finally:
             if sys.exc_info() != (None, None, None):
                 time.sleep(0.1)  # give any in-flight Futures a chance to be .put() ...
             while not self._tasks_to_send.empty():
                 fut, _task = self._tasks_to_send.get()
                 if fut:
                     fut.cancel()
                     fut.set_running_or_notify_cancel()
             try:
                 while True:
                     self._tasks_to_send.task_done()
             except ValueError:
                 pass
-            log.debug("%s: task submission thread complete", self)
+            log.debug("%r: task submission thread complete", self)
 
     def _submit_tasks(
         self,
         taskgroup_uuid: uuid.UUID | None,
         endpoint_uuid: uuid.UUID,
         user_endpoint_config: dict | None,
         futs: list[ComputeFuture],
@@ -846,28 +861,28 @@
         :param futs: a list of ComputeFutures; will have their task_id attribute
             set when function completes successfully.
         :param tasks: a list of tasks to submit upstream in a batch.
         """
         if taskgroup_uuid is None and self.task_group_id:
             taskgroup_uuid = self.task_group_id
 
-        batch = self.funcx_client.create_batch(
+        batch = self.client.create_batch(
             taskgroup_uuid, user_endpoint_config, create_websocket_queue=True
         )
         submitted_futs_by_fn: t.DefaultDict[str, list[ComputeFuture]] = defaultdict(
             list
         )
         for fut, task in zip(futs, tasks):
             f_uuid_str = str(task.function_uuid)
             submitted_futs_by_fn[f_uuid_str].append(fut)
             batch.add(f_uuid_str, task.args, task.kwargs)
             log.debug("Added task to Globus Compute batch: %s", task)
 
         try:
-            batch_response = self.funcx_client.batch_run(endpoint_uuid, batch)
+            batch_response = self.client.batch_run(endpoint_uuid, batch)
         except Exception as e:
             log.exception(f"Error submitting {len(tasks)} tasks to Globus Compute")
             for fut_list in submitted_futs_by_fn.values():
                 for fut in fut_list:
                     fut.set_exception(e)
             raise
 
@@ -1159,15 +1174,15 @@
         Match the internal ``_received_results`` and ``_open_futures`` on their
         keys, and complete the associated futures.  All matching items will,
         after processing, be forgotten (i.e., ``.pop()``).
 
         This method will set the _open_futures_empty event if there are no open
         futures *at the time of processing*.
         """
-        deserialize = self.funcx_executor.funcx_client.fx_serializer.deserialize
+        deserialize = self.funcx_executor.client.fx_serializer.deserialize
         with self._new_futures_lock:
             futures_to_complete = [
                 self._open_futures.pop(tid)
                 for tid in self._open_futures.keys() & self._received_results.keys()
             ]
             if not self._open_futures:
                 self._open_futures_empty.set()
@@ -1286,15 +1301,15 @@
                     self._connection.close()
             elif self._connection.is_closed:
                 self._connection.ioloop.stop()
                 self._connection = None
 
     def _connect(self) -> pika.SelectConnection:
         with self._new_futures_lock:
-            res = self.funcx_executor.funcx_client.get_result_amqp_url()
+            res = self.funcx_executor.client.get_result_amqp_url()
             self._queue_prefix = res["queue_prefix"]
             connection_url = res["connection_url"]
 
             pika_params = pika.URLParameters(connection_url)
             if self.port is not None:
                 pika_params.port = self.port
             return pika.SelectConnection(
```

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/authorizer_login_manager.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/authorizer_login_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/utils/__init__.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/__init__.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk/version.py` & `globus-compute-sdk-2.9.0/globus_compute_sdk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.8.0a0"
+__version__ = "2.9.0"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.8.0a0
+Version: 2.9.0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.8.0a0/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.9.0/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.8.0a0/setup.py` & `globus-compute-sdk-2.9.0/setup.py`

 * *Files identical despite different names*

