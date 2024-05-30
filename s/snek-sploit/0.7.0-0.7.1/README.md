# Comparing `tmp/snek_sploit-0.7.0.tar.gz` & `tmp/snek_sploit-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek_sploit-0.7.0.tar", max compression
+gzip compressed data, was "snek_sploit-0.7.1.tar", max compression
```

## Comparing `snek_sploit-0.7.0.tar` & `snek_sploit-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1069 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/LICENSE
--rw-r--r--   0        0        0     1539 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/README.md
--rw-r--r--   0        0        0      686 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1393 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/__init__.py
--rw-r--r--   0        0        0     4696 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/context.py
--rw-r--r--   0        0        0     3004 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/metasploit.py
--rw-r--r--   0        0        0        0 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/__init__.py
--rw-r--r--   0        0        0     3086 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/auth.py
--rw-r--r--   0        0        0    10952 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/consoles.py
--rw-r--r--   0        0        0     7892 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/core.py
--rw-r--r--   0        0        0    12331 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/db.py
--rw-r--r--   0        0        0      728 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/health.py
--rw-r--r--   0        0        0     2676 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/jobs.py
--rw-r--r--   0        0        0    19865 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/modules.py
--rw-r--r--   0        0        0     1629 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/plugins.py
--rw-r--r--   0        0        0    24454 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/lib/rpc/sessions.py
--rw-r--r--   0        0        0        0 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/__init__.py
--rw-r--r--   0        0        0     1887 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/constants.py
--rw-r--r--   0        0        0      448 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/enums.py
--rw-r--r--   0        0        0      276 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/exceptions.py
--rw-r--r--   0        0        0      713 2024-05-20 10:59:51.205724 snek_sploit-0.7.0/snek_sploit/util/retry.py
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 snek_sploit-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1539 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/README.md
+-rw-r--r--   0        0        0      686 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1393 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/__init__.py
+-rw-r--r--   0        0        0     4699 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/context.py
+-rw-r--r--   0        0        0     3004 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/metasploit.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/auth.py
+-rw-r--r--   0        0        0    10952 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/consoles.py
+-rw-r--r--   0        0        0     7892 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/core.py
+-rw-r--r--   0        0        0    12331 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/db.py
+-rw-r--r--   0        0        0      728 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/health.py
+-rw-r--r--   0        0        0     2676 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/jobs.py
+-rw-r--r--   0        0        0    19865 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/modules.py
+-rw-r--r--   0        0        0     1629 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/plugins.py
+-rw-r--r--   0        0        0    24454 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/lib/rpc/sessions.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/constants.py
+-rw-r--r--   0        0        0      448 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/enums.py
+-rw-r--r--   0        0        0      276 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/exceptions.py
+-rw-r--r--   0        0        0      955 2024-05-30 14:25:07.114011 snek_sploit-0.7.1/snek_sploit/util/retry.py
+-rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 snek_sploit-0.7.1/PKG-INFO
```

### Comparing `snek_sploit-0.7.0/LICENSE` & `snek_sploit-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/README.md` & `snek_sploit-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/pyproject.toml` & `snek_sploit-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snek-sploit"
-version = "0.7.0"
+version = "0.7.1"
 description = "Python RPC client for Metasploit Framework"
 authors = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
 maintainers = [
     "Jiří Rája <jiri.raja@gmail.com>"
 ]
```

### Comparing `snek_sploit-0.7.0/snek_sploit/__init__.py` & `snek_sploit-0.7.1/snek_sploit/__init__.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/context.py` & `snek_sploit-0.7.1/snek_sploit/lib/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         arguments = [self.token] if use_token else []
 
         if call_arguments is not None:
             arguments += call_arguments
 
         return arguments
 
-    @retry(tries=3, on_errors=(requests.RequestException,))
+    @retry(attempts=3, on_errors=(requests.RequestException,))
     def call(
         self, endpoint: str, arguments: list = None, use_token: bool = True, timeout: Union[float, tuple] = None
     ) -> RPCResponse:
         """
         Create a call to an endpoint.
         :param endpoint: Endpoint name
         :param arguments: Arguments that will be processed and passed to the endpoint
```

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/metasploit.py` & `snek_sploit-0.7.1/snek_sploit/lib/metasploit.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/auth.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/consoles.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/consoles.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/core.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/core.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/db.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/db.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/health.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/health.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/jobs.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/jobs.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/modules.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/plugins.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/plugins.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/lib/rpc/sessions.py` & `snek_sploit-0.7.1/snek_sploit/lib/rpc/sessions.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/util/constants.py` & `snek_sploit-0.7.1/snek_sploit/util/constants.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.7.0/snek_sploit/util/retry.py` & `snek_sploit-0.7.1/snek_sploit/util/retry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from functools import wraps, partial
+import time
 
 
-def retry(func=None, *, tries: int = 1, on_errors: tuple = None):
+def retry(func=None, *, attempts: int = 1, on_errors: tuple = None, wait_on_error: bool = True):
     """
     Retry a function if an error occurs.
     :param func: Original function
-    :param tries: Number of times to retry
+    :param attempts: Number of times to retry
     :param on_errors: On what errors to retry
+    :param wait_on_error: Whether to wait when an error occurs or not
     :return: Wrapper
     """
     if func is None:
-        return partial(retry, tries=tries, on_errors=on_errors)
+        return partial(retry, attempts=attempts, on_errors=on_errors, wait_on_error=wait_on_error)
 
     if not on_errors:
         on_errors = (Exception,)
 
     @wraps(func)
     def wrapper(*args, **kwargs):
-        for i in range(tries + 1):
+        for i in range(attempts):
             try:
                 return func(*args, **kwargs)
             except on_errors as ex:
-                if i == tries:
+                if i + 1 == attempts:
                     raise ex
+                if wait_on_error:
+                    time.sleep(min(i + 1 * 3, 30))
 
     return wrapper
```

### Comparing `snek_sploit-0.7.0/PKG-INFO` & `snek_sploit-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek-sploit
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python RPC client for Metasploit Framework
 Home-page: https://github.com/SadParad1se/snek-sploit
 License: MIT
 Keywords: metasploit,msf,rpc,client
 Author: Jiří Rája
 Author-email: jiri.raja@gmail.com
 Maintainer: Jiří Rája
```

