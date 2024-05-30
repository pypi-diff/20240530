# Comparing `tmp/rtorrent_rpc-0.6.5.tar.gz` & `tmp/rtorrent_rpc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.6.5.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.7.0.tar", max compression
```

## Comparing `rtorrent_rpc-0.6.5.tar` & `rtorrent_rpc-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/LICENSE
--rw-r--r--   0        0        0     2550 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     1669 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/readme.md
--rw-r--r--   0        0        0    29843 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2458 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/rtorrent_rpc/_jsonrpc/__init__.py
--rw-r--r--   0        0        0     3050 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/rtorrent_rpc/_jsonrpc/transport.py
--rw-r--r--   0        0        0     1235 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/rtorrent_rpc/_scgi.py
--rw-r--r--   0        0        0      803 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/rtorrent_rpc/_transport.py
--rw-r--r--   0        0        0     3920 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-05-17 02:46:29.591142 rtorrent_rpc-0.6.5/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 rtorrent_rpc-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2639 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1832 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/readme.md
+-rw-r--r--   0        0        0    29843 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2458 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/rtorrent_rpc/_jsonrpc/__init__.py
+-rw-r--r--   0        0        0     3446 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/rtorrent_rpc/_jsonrpc/transport.py
+-rw-r--r--   0        0        0     1235 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/rtorrent_rpc/_scgi.py
+-rw-r--r--   0        0        0      803 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/rtorrent_rpc/_transport.py
+-rw-r--r--   0        0        0     3932 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-05-30 18:34:12.322617 rtorrent_rpc-0.7.0/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 rtorrent_rpc-0.7.0/PKG-INFO
```

### Comparing `rtorrent_rpc-0.6.5/LICENSE` & `rtorrent_rpc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.5/pyproject.toml` & `rtorrent_rpc-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.6.5"
+version = "0.7.0"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -20,16 +20,17 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # dependencies
 typing-extensions = ">=4.7.1"
 bencode2 = ">=0.0.6,<1"
-urllib3 = "^2.2.1"
+urllib3 = { version = "^2.2.1", extras = ['secure'] }
 orjson = { version = '>3.0.0,<4', optional = true }
+certifi = { version = '>=2024.2.2', optional = true }
 
 [tool.poetry.extras]
 orjson = ['orjson']
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "^2024.0.0", python = "^3.9" }
```

### Comparing `rtorrent_rpc-0.6.5/readme.md` & `rtorrent_rpc-0.7.0/readme.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![Documentation Status](https://readthedocs.org/projects/rtorrent-rpc/badge/)](https://rtorrent-rpc.readthedocs.io/)
 
 `rtorrent-rpc` is a python wrapper on top of rtorrent XML RPC protocol,
-hosted on GitHub at [github.com/trim21/rtorrent-rpc](https://github.com/trim21/rtorrent-rpc)
+hosted on GitHub
+at [github.com/trim21/rtorrent-rpc](https://github.com/trim21/rtorrent-rpc)
 
 Document is hosted at https://rtorrent-rpc.readthedocs.io/ by readthedocs.
 
 ## Introduction
 
 ```console
 pip install rtorrent-rpc
 ```
 
-if you prefer [orjson](https://github.com/ijl/orjson) as jsonlib:
+supported extras:
+
+- `orjson`: use [orjson](https://github.com/ijl/orjson) as jsonlib
 
 ```console
 pip install 'rtorrent-rpc[orjson]'
 ```
 
 ## Contributing
 
@@ -30,23 +33,28 @@
 ```python
 from rtorrent_rpc import RTorrent
 
 client = RTorrent(address='scgi://127.0.0.1:5000')
 unix_client = RTorrent(address='scgi:///home/ubuntu/.local/share/rtorrent.sock')
 ```
 
+tls cert validation is enabled when you are using `https` protocol, set environment
+variable `PY_RTORRENT_RPC_DISABLE_TLS_CERT=1` to disable.
+
 ## Known Problem
 
-rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250), for example, emoji.
+rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250),
+for example, emoji.
 
 If torrent name of file name contains any emoji,
 you can't retrieve correct torrent name or file name through xmlrpc.
 
 Please consider use a rtorrent distro with json-rpc support,
-for example: [jesec/rtorrent](https://github.com/jesec/rtorrent), which support utf8 correctly.
+for example: [jesec/rtorrent](https://github.com/jesec/rtorrent), which support utf8
+correctly.
 
 If your rtorrent distro support jsonrpc,
 you can use send json-rpc request with `RTorrent(...).jsonrpc.call(...)`.
 
 ## License
 
 `rtorrent-rpc` is licensed under the MIT license.
```

### Comparing `rtorrent_rpc-0.6.5/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.7.0/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.5/rtorrent_rpc/_jsonrpc/__init__.py` & `rtorrent_rpc-0.7.0/rtorrent_rpc/_jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.5/rtorrent_rpc/_jsonrpc/transport.py` & `rtorrent_rpc-0.7.0/rtorrent_rpc/_jsonrpc/transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from __future__ import annotations
 
+import os
 import socket
+import ssl
 from typing import Protocol
 from urllib.parse import urlparse
 
+import certifi
 from urllib3 import HTTPConnectionPool, HTTPSConnectionPool
 
 from rtorrent_rpc import _scgi as scgi
 
+_VALIDATE_ENV_KEY = "PY_RTORRENT_RPC_DISABLE_TLS_CERT"
+
 
 class BadStatusError(Exception):
     status: int
     body: bytes
 
     def __init__(self, status: int, body: bytes):
         super().__init__(f"unexpected response status code {status}")
@@ -84,15 +89,23 @@
         self.host = u.hostname
         self.port = u.port
         self.u = u
 
         if self.u.scheme == "http":
             self._pool = HTTPConnectionPool(self.host, self.port)
         elif self.u.scheme == "https":
-            self._pool = HTTPSConnectionPool(self.host, self.port)
+            if os.environ.get(_VALIDATE_ENV_KEY) == "1":
+                self._pool = HTTPSConnectionPool(self.host, self.port)
+            else:
+                self._pool = HTTPSConnectionPool(
+                    self.host,
+                    self.port,
+                    ca_certs=certifi.where(),
+                    cert_reqs=ssl.CERT_REQUIRED,
+                )
 
     def request(self, body: bytes, content_type: str | None = None) -> bytes:
         headers = {}
         if content_type:
             headers["content-type"] = content_type
 
         with self._pool.urlopen(
```

### Comparing `rtorrent_rpc-0.6.5/rtorrent_rpc/_scgi.py` & `rtorrent_rpc-0.7.0/rtorrent_rpc/_scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.5/rtorrent_rpc/_transport.py` & `rtorrent_rpc-0.7.0/rtorrent_rpc/_transport.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.6.5/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.7.0/rtorrent_rpc/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """ruTorrent compatibility method to parse ``d.custom2`` as torrent comment"""
     if s.startswith("VRS24mrker"):
         return unquote(__remove_prefix(s, "VRS24mrker"))
     return s
 
 
 def get_torrent_info_hash(content: bytes) -> str:
-    """get torrent info_hash in low case string"""
+    """generate torrent info_hash v1 in low case hex string"""
     data = bencode2.bdecode(content)
     return hashlib.sha1(bencode2.bencode(data[b"info"])).hexdigest()
 
 
 class LibTorrentFilePriority(enum.IntEnum):
     OFF = 0
     NORMAL = 1
```

### Comparing `rtorrent_rpc-0.6.5/PKG-INFO` & `rtorrent_rpc-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.6.5
+Version: 0.7.0
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.8,<4.0
@@ -16,38 +16,42 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: orjson
 Requires-Dist: bencode2 (>=0.0.6,<1)
+Requires-Dist: certifi (>=2024.2.2)
 Requires-Dist: orjson (>3.0.0,<4) ; extra == "orjson"
 Requires-Dist: typing-extensions (>=4.7.1)
-Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
+Requires-Dist: urllib3[secure] (>=2.2.1,<3.0.0)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
 [![Documentation Status](https://readthedocs.org/projects/rtorrent-rpc/badge/)](https://rtorrent-rpc.readthedocs.io/)
 
 `rtorrent-rpc` is a python wrapper on top of rtorrent XML RPC protocol,
-hosted on GitHub at [github.com/trim21/rtorrent-rpc](https://github.com/trim21/rtorrent-rpc)
+hosted on GitHub
+at [github.com/trim21/rtorrent-rpc](https://github.com/trim21/rtorrent-rpc)
 
 Document is hosted at https://rtorrent-rpc.readthedocs.io/ by readthedocs.
 
 ## Introduction
 
 ```console
 pip install rtorrent-rpc
 ```
 
-if you prefer [orjson](https://github.com/ijl/orjson) as jsonlib:
+supported extras:
+
+- `orjson`: use [orjson](https://github.com/ijl/orjson) as jsonlib
 
 ```console
 pip install 'rtorrent-rpc[orjson]'
 ```
 
 ## Contributing
 
@@ -58,23 +62,28 @@
 ```python
 from rtorrent_rpc import RTorrent
 
 client = RTorrent(address='scgi://127.0.0.1:5000')
 unix_client = RTorrent(address='scgi:///home/ubuntu/.local/share/rtorrent.sock')
 ```
 
+tls cert validation is enabled when you are using `https` protocol, set environment
+variable `PY_RTORRENT_RPC_DISABLE_TLS_CERT=1` to disable.
+
 ## Known Problem
 
-rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250), for example, emoji.
+rTorrent's [xmlrpc do not support all utf8 characters](https://github.com/rakshasa/rtorrent/issues/1250),
+for example, emoji.
 
 If torrent name of file name contains any emoji,
 you can't retrieve correct torrent name or file name through xmlrpc.
 
 Please consider use a rtorrent distro with json-rpc support,
-for example: [jesec/rtorrent](https://github.com/jesec/rtorrent), which support utf8 correctly.
+for example: [jesec/rtorrent](https://github.com/jesec/rtorrent), which support utf8
+correctly.
 
 If your rtorrent distro support jsonrpc,
 you can use send json-rpc request with `RTorrent(...).jsonrpc.call(...)`.
 
 ## License
 
 `rtorrent-rpc` is licensed under the MIT license.
```

