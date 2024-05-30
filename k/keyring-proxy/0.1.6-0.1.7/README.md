# Comparing `tmp/keyring_proxy-0.1.6.tar.gz` & `tmp/keyring_proxy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy-0.1.6.tar", last modified: Thu May 30 10:33:40 2024, max compression
+gzip compressed data, was "keyring_proxy-0.1.7.tar", last modified: Thu May 30 10:50:04 2024, max compression
```

## Comparing `keyring_proxy-0.1.6.tar` & `keyring_proxy-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.6/README.md
--rw-r--r--   0        0        0      724 2024-05-30 10:33:40.945790 keyring_proxy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.6/src/keyring_proxy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.6/src/keyring_proxy/py.typed
--rw-r--r--   0        0        0     3367 2024-05-30 10:31:30.067152 keyring_proxy-0.1.6/src/keyring_proxy/socketproxy.py
--rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.6/src/keyring_proxy/transport.py
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.7/README.md
+-rw-r--r--   0        0        0      724 2024-05-30 10:50:04.850276 keyring_proxy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.7/src/keyring_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.7/src/keyring_proxy/py.typed
+-rw-r--r--   0        0        0     3367 2024-05-30 10:31:30.067152 keyring_proxy-0.1.7/src/keyring_proxy/socketproxy.py
+-rw-r--r--   0        0        0     1451 2024-05-30 10:45:52.132822 keyring_proxy-0.1.7/src/keyring_proxy/stdioproxy.py
+-rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.7/src/keyring_proxy/transport.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.7/PKG-INFO
```

### Comparing `keyring_proxy-0.1.6/pyproject.toml` & `keyring_proxy-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyring-proxy"
-version = "0.1.6"
+version = "0.1.7"
 description = "Proxy Base for pypi keyring"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
     "keyring>=25.2.1",
 ]
```

### Comparing `keyring_proxy-0.1.6/src/keyring_proxy/socketproxy.py` & `keyring_proxy-0.1.7/src/keyring_proxy/socketproxy.py`

 * *Files identical despite different names*

### Comparing `keyring_proxy-0.1.6/src/keyring_proxy/transport.py` & `keyring_proxy-0.1.7/src/keyring_proxy/transport.py`

 * *Files identical despite different names*

