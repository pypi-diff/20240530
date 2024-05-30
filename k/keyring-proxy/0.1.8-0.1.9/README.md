# Comparing `tmp/keyring_proxy-0.1.8.tar.gz` & `tmp/keyring_proxy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy-0.1.8.tar", last modified: Thu May 30 11:17:53 2024, max compression
+gzip compressed data, was "keyring_proxy-0.1.9.tar", last modified: Thu May 30 13:18:59 2024, max compression
```

## Comparing `keyring_proxy-0.1.8.tar` & `keyring_proxy-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.8/README.md
--rw-r--r--   0        0        0      724 2024-05-30 11:17:53.345317 keyring_proxy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.8/src/keyring_proxy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.8/src/keyring_proxy/py.typed
--rw-r--r--   0        0        0     3001 2024-05-30 11:17:22.076918 keyring_proxy-0.1.8/src/keyring_proxy/socketproxy.py
--rw-r--r--   0        0        0     1079 2024-05-30 11:15:51.832801 keyring_proxy-0.1.8/src/keyring_proxy/stdioproxy.py
--rw-r--r--   0        0        0     7107 2024-05-30 10:23:20.657478 keyring_proxy-0.1.8/src/keyring_proxy/transport.py
--rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 13:29:53.354115 keyring_proxy-0.1.9/README.md
+-rw-r--r--   0        0        0      724 2024-05-30 13:18:59.572001 keyring_proxy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.9/src/keyring_proxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:37:18.859494 keyring_proxy-0.1.9/src/keyring_proxy/py.typed
+-rw-r--r--   0        0        0     3001 2024-05-30 11:17:22.076918 keyring_proxy-0.1.9/src/keyring_proxy/socketproxy.py
+-rw-r--r--   0        0        0     1079 2024-05-30 11:15:51.832801 keyring_proxy-0.1.9/src/keyring_proxy/stdioproxy.py
+-rw-r--r--   0        0        0     7084 2024-05-30 13:18:42.620301 keyring_proxy-0.1.9/src/keyring_proxy/transport.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:29:53.354115 keyring_proxy-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 keyring_proxy-0.1.9/PKG-INFO
```

### Comparing `keyring_proxy-0.1.8/pyproject.toml` & `keyring_proxy-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "keyring-proxy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Proxy Base for pypi keyring"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
     "keyring>=25.2.1",
 ]
```

### Comparing `keyring_proxy-0.1.8/src/keyring_proxy/socketproxy.py` & `keyring_proxy-0.1.9/src/keyring_proxy/socketproxy.py`

 * *Files identical despite different names*

### Comparing `keyring_proxy-0.1.8/src/keyring_proxy/stdioproxy.py` & `keyring_proxy-0.1.9/src/keyring_proxy/stdioproxy.py`

 * *Files identical despite different names*

### Comparing `keyring_proxy-0.1.8/src/keyring_proxy/transport.py` & `keyring_proxy-0.1.9/src/keyring_proxy/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
     logfile: str = "keyring-proxy.log"
     log: bool = False
 
     def __init__(self):
         super().__init__()
         if self.log:
-            logging.basicConfig(level=logging.DEBUG, filename=self.logfile)
+            logging.basicConfig(level=logging.DEBUG)
 
     @property
     def _transport(self):
         return self._get_transport()
 
     @abc.abstractmethod
     def _get_transport(self) -> TransportClient:
```

