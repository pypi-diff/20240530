# Comparing `tmp/rivian_python_client-1.1.2.tar.gz` & `tmp/rivian_python_client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian_python_client-1.1.2.tar", max compression
+gzip compressed data, was "rivian_python_client-1.1.3.tar", max compression
```

## Comparing `rivian_python_client-1.1.2.tar` & `rivian_python_client-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      325 2024-02-03 21:59:30.260252 rivian_python_client-1.1.2/README.md
--rw-r--r--   0        0        0      989 2024-02-03 21:59:42.512338 rivian_python_client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      155 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/__init__.py
--rw-r--r--   0        0        0     5785 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/ble.py
--rw-r--r--   0        0        0     6177 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/const.py
--rw-r--r--   0        0        0      969 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/py.typed
--rw-r--r--   0        0        0    28086 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/rivian.py
--rw-r--r--   0        0        0     3636 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/schemas/charging.graphql
--rw-r--r--   0        0        0    12887 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/schemas/gateway.graphql
--rw-r--r--   0        0        0     4290 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/schemas/orders.graphql
--rw-r--r--   0        0        0     3298 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/utils.py
--rw-r--r--   0        0        0     7509 2024-02-03 21:59:30.264252 rivian_python_client-1.1.2/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 rivian_python_client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      325 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/README.md
+-rw-r--r--   0        0        0     1019 2024-05-29 22:30:58.722718 rivian_python_client-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/__init__.py
+-rw-r--r--   0        0        0     5785 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/ble.py
+-rw-r--r--   0        0        0     6177 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/const.py
+-rw-r--r--   0        0        0      969 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/py.typed
+-rw-r--r--   0        0        0    28086 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/rivian.py
+-rw-r--r--   0        0        0     3636 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/schemas/charging.graphql
+-rw-r--r--   0        0        0    17112 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/schemas/gateway.graphql
+-rw-r--r--   0        0        0     4290 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/schemas/orders.graphql
+-rw-r--r--   0        0        0     3298 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/utils.py
+-rw-r--r--   0        0        0     7509 2024-05-29 22:30:47.006645 rivian_python_client-1.1.3/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 rivian_python_client-1.1.3/PKG-INFO
```

### Comparing `rivian_python_client-1.1.2/pyproject.toml` & `rivian_python_client-1.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "1.1.2"
+version = "1.1.3"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.13"
+python = ">=3.9,<3.13"
 aiohttp = ">=3.0.0"
-cryptography = ">=41.0.1, <43.0"
+cryptography = ">=41.0.1,<43.0"
 backports-strenum = { version = "^1.2.4", python = "<3.11" }
-bleak = { version = "^0.21", optional = true }
+bleak = { version = ">=0.21,<1.0.0", optional = true }
 dbus-fast = {version = "^2.11.0", optional = true, platform = "linux"}
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.1.2"
+pytest = ">=7.1.2,<9.0.0"
 pytest-asyncio = ">=0.18.3,<0.24.0"
 python-dotenv = ">=0.20,<1.1"
-aresponses = "^2.1.5"
-mypy = "^1.7.0"
+aresponses = ">=2.1.5,<4.0.0"
+mypy = ">=1.7.0,<2.0.0"
 
 [tool.poetry.extras]
 ble = ["bleak", "dbus-fast"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `rivian_python_client-1.1.2/src/rivian/ble.py` & `rivian_python_client-1.1.3/src/rivian/ble.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/src/rivian/const.py` & `rivian_python_client-1.1.3/src/rivian/const.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/src/rivian/exceptions.py` & `rivian_python_client-1.1.3/src/rivian/exceptions.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/src/rivian/rivian.py` & `rivian_python_client-1.1.3/src/rivian/rivian.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/src/rivian/schemas/charging.graphql` & `rivian_python_client-1.1.3/src/rivian/schemas/charging.graphql`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/src/rivian/schemas/orders.graphql` & `rivian_python_client-1.1.3/src/rivian/schemas/orders.graphql`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/src/rivian/utils.py` & `rivian_python_client-1.1.3/src/rivian/utils.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/src/rivian/ws_monitor.py` & `rivian_python_client-1.1.3/src/rivian/ws_monitor.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-1.1.2/PKG-INFO` & `rivian_python_client-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: ble
 Requires-Dist: aiohttp (>=3.0.0)
 Requires-Dist: backports-strenum (>=1.2.4,<2.0.0) ; python_version < "3.11"
-Requires-Dist: bleak (>=0.21,<0.22) ; extra == "ble"
+Requires-Dist: bleak (>=0.21,<1.0.0) ; extra == "ble"
 Requires-Dist: cryptography (>=41.0.1,<43.0)
 Requires-Dist: dbus-fast (>=2.11.0,<3.0.0) ; (sys_platform == "linux") and (extra == "ble")
 Description-Content-Type: text/markdown
 
 # Python: Rivian API Client
 
 Currently a Work In Progress
```

