# Comparing `tmp/keyring_proxy-0.1.7.tar.gz` & `tmp/keyring_proxy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy-0.1.7.tar", last modified: Thu May 30 10:50:04 2024, max compression
+gzip compressed data, was "keyring_proxy-0.1.8.tar", last modified: Thu May 30 11:17:53 2024, max compression
```

## Comparing `keyring_proxy-0.1.7.tar` & `keyring_proxy-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.7/README.md
--rw-r--r--   0        0        0      724 2024-05-30 10:50:04.850276 keyring_proxy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.7/src/keyring_proxy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.7/src/keyring_proxy/py.typed
--rw-r--r--   0        0        0     3367 2024-05-30 10:31:30.067152 keyring_proxy-0.1.7/src/keyring_proxy/socketproxy.py
--rw-r--r--   0        0        0     1451 2024-05-30 10:45:52.132822 keyring_proxy-0.1.7/src/keyring_proxy/stdioproxy.py
--rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.7/src/keyring_proxy/transport.py
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.8/README.md
+-rw-r--r--   0        0        0      724 2024-05-30 11:17:53.345317 keyring_proxy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.8/src/keyring_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.8/src/keyring_proxy/py.typed
+-rw-r--r--   0        0        0     3001 2024-05-30 11:17:22.076918 keyring_proxy-0.1.8/src/keyring_proxy/socketproxy.py
+-rw-r--r--   0        0        0     1079 2024-05-30 11:15:51.832801 keyring_proxy-0.1.8/src/keyring_proxy/stdioproxy.py
+-rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.8/src/keyring_proxy/transport.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.8/PKG-INFO
```

### Comparing `keyring_proxy-0.1.7/pyproject.toml` & `keyring_proxy-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyring-proxy"
-version = "0.1.7"
+version = "0.1.8"
 description = "Proxy Base for pypi keyring"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
     "keyring>=25.2.1",
 ]
```

### Comparing `keyring_proxy-0.1.7/src/keyring_proxy/socketproxy.py` & `keyring_proxy-0.1.8/src/keyring_proxy/socketproxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 import dataclasses
 import logging
 import os
 import pathlib
 import socket
 from typing import override
 
-import jaraco.classes.properties as properties  # type: ignore
-from keyring_proxy.transport import ProxyBackend, ReqPacket, RespPacket, TransportClient, TransportServer
+from keyring_proxy.transport import ReqPacket, RespPacket, TransportClient, TransportServer
 
-PRIORITY = 7.8
 DEFAULT_SOCKET_PATH = "/tmp/keyring-proxy.sock"
 
 logger = logging.getLogger(__name__)
 
 
 def _get_socket() -> socket.socket:
     if os.name == "nt":
@@ -77,27 +75,14 @@
             return _recv_packet(sock)
 
     @classmethod
     def from_path(cls, sock: str):
         return cls(pathlib.Path(sock))
 
 
-class SocketProxyBackend(ProxyBackend):
-
-    socket: str = DEFAULT_SOCKET_PATH
-
-    @override
-    def _get_transport(self) -> TransportClient:
-        return SocketClient.from_path(self.socket)
-
-    @properties.classproperty
-    def priority(cls):
-        return PRIORITY
-
-
 @dataclasses.dataclass
 class SocketServer(TransportServer):
 
     socket_path: pathlib.Path = pathlib.Path(DEFAULT_SOCKET_PATH)
 
     def serve(self):
         with _listening_socket(self.socket_path) as sock:
```

### Comparing `keyring_proxy-0.1.7/src/keyring_proxy/transport.py` & `keyring_proxy-0.1.8/src/keyring_proxy/transport.py`

 * *Files identical despite different names*

