# Comparing `tmp/keyring_proxy-0.1.4.tar.gz` & `tmp/keyring_proxy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy-0.1.4.tar", last modified: Wed May 29 14:37:59 2024, max compression
+gzip compressed data, was "keyring_proxy-0.1.5.tar", last modified: Thu May 30 10:23:49 2024, max compression
```

## Comparing `keyring_proxy-0.1.4.tar` & `keyring_proxy-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.4/README.md
--rw-r--r--   0        0        0      724 2024-05-29 14:37:59.680513 keyring_proxy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.4/src/keyring_proxy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.4/src/keyring_proxy/py.typed
--rw-r--r--   0        0        0     6872 2024-05-29 14:03:20.644194 keyring_proxy-0.1.4/src/keyring_proxy/transport.py
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.5/README.md
+-rw-r--r--   0        0        0      724 2024-05-30 10:23:49.269167 keyring_proxy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.5/src/keyring_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.5/src/keyring_proxy/py.typed
+-rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.5/src/keyring_proxy/transport.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.5/PKG-INFO
```

### Comparing `keyring_proxy-0.1.4/pyproject.toml` & `keyring_proxy-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyring-proxy"
-version = "0.1.4"
+version = "0.1.5"
 description = "Proxy Base for pypi keyring"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
     "keyring>=25.2.1",
 ]
```

### Comparing `keyring_proxy-0.1.4/src/keyring_proxy/transport.py` & `keyring_proxy-0.1.5/src/keyring_proxy/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # mypy: disable-error-code="return-value, valid-type"
 
 import abc
 import dataclasses
 import json
+import logging
 import typing
 from types import UnionType
 from typing import Any, ClassVar, Self, Type, TypeVar, Union, get_args, get_origin, overload
 
 import keyring.backend
 import keyring.credentials
 
@@ -196,14 +197,22 @@
         resp_data = self._communicate(req_data)
         resp_cls = req.get_reponse_cls()
         return unpack_response(resp_cls, resp_data)
 
 
 class ProxyBackend(keyring.backend.KeyringBackend):
 
+    logfile: str = "keyring-proxy.log"
+    log: bool = False
+
+    def __init__(self):
+        super().__init__()
+        if self.log:
+            logging.basicConfig(level=logging.DEBUG, filename=self.logfile)
+
     @property
     def _transport(self):
         return self._get_transport()
 
     @abc.abstractmethod
     def _get_transport(self) -> TransportClient:
         pass
```

