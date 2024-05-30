# Comparing `tmp/keyring_proxy-0.1.3.tar.gz` & `tmp/keyring_proxy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy-0.1.3.tar", last modified: Wed May 29 14:35:53 2024, max compression
+gzip compressed data, was "keyring_proxy-0.1.4.tar", last modified: Wed May 29 14:37:59 2024, max compression
```

## Comparing `keyring_proxy-0.1.3.tar` & `keyring_proxy-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.3/README.md
--rw-r--r--   0        0        0      724 2024-05-29 14:35:53.680591 keyring_proxy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.3/src/keyring_proxy/__init__.py
--rw-r--r--   0        0        0     6872 2024-05-29 14:03:20.644194 keyring_proxy-0.1.3/src/keyring_proxy/transport.py
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.4/README.md
+-rw-r--r--   0        0        0      724 2024-05-29 14:37:59.680513 keyring_proxy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.4/src/keyring_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.4/src/keyring_proxy/py.typed
+-rw-r--r--   0        0        0     6872 2024-05-29 14:03:20.644194 keyring_proxy-0.1.4/src/keyring_proxy/transport.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.4/PKG-INFO
```

### Comparing `keyring_proxy-0.1.3/pyproject.toml` & `keyring_proxy-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyring-proxy"
-version = "0.1.3"
+version = "0.1.4"
 description = "Proxy Base for pypi keyring"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
     "keyring>=25.2.1",
 ]
```

### Comparing `keyring_proxy-0.1.3/src/keyring_proxy/transport.py` & `keyring_proxy-0.1.4/src/keyring_proxy/transport.py`

 * *Files identical despite different names*

