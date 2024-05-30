# Comparing `tmp/keyring_proxy-0.1.5.tar.gz` & `tmp/keyring_proxy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy-0.1.5.tar", last modified: Thu May 30 10:23:49 2024, max compression
+gzip compressed data, was "keyring_proxy-0.1.6.tar", last modified: Thu May 30 10:33:40 2024, max compression
```

## Comparing `keyring_proxy-0.1.5.tar` & `keyring_proxy-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.5/README.md
--rw-r--r--   0        0        0      724 2024-05-30 10:23:49.269167 keyring_proxy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.5/src/keyring_proxy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.5/src/keyring_proxy/py.typed
--rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.5/src/keyring_proxy/transport.py
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.6/README.md
+-rw-r--r--   0        0        0      724 2024-05-30 10:33:40.945790 keyring_proxy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.6/src/keyring_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.6/src/keyring_proxy/py.typed
+-rw-r--r--   0        0        0     3367 2024-05-30 10:31:30.067152 keyring_proxy-0.1.6/src/keyring_proxy/socketproxy.py
+-rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.6/src/keyring_proxy/transport.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.6/PKG-INFO
```

### Comparing `keyring_proxy-0.1.5/pyproject.toml` & `keyring_proxy-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyring-proxy"
-version = "0.1.5"
+version = "0.1.6"
 description = "Proxy Base for pypi keyring"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
     "keyring>=25.2.1",
 ]
```

### Comparing `keyring_proxy-0.1.5/src/keyring_proxy/transport.py` & `keyring_proxy-0.1.6/src/keyring_proxy/transport.py`

 * *Files identical despite different names*

