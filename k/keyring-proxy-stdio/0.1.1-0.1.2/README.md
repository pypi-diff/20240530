# Comparing `tmp/keyring_proxy_stdio-0.1.1.tar.gz` & `tmp/keyring_proxy_stdio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy_stdio-0.1.1.tar", last modified: Thu May 30 10:52:44 2024, max compression
+gzip compressed data, was "keyring_proxy_stdio-0.1.2.tar", last modified: Thu May 30 11:19:21 2024, max compression
```

## Comparing `keyring_proxy_stdio-0.1.1.tar` & `keyring_proxy_stdio-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.1/README.md
--rw-r--r--   0        0        0      854 2024-05-30 10:52:44.898929 keyring_proxy_stdio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.1/src/keyring_proxy_stdio/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 keyring_proxy_stdio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.2/README.md
+-rw-r--r--   0        0        0      854 2024-05-30 11:19:21.002845 keyring_proxy_stdio-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      484 2024-05-30 11:15:44.762803 keyring_proxy_stdio-0.1.2/src/keyring_proxy_stdio/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 keyring_proxy_stdio-0.1.2/PKG-INFO
```

### Comparing `keyring_proxy_stdio-0.1.1/pyproject.toml` & `keyring_proxy_stdio-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "keyring-proxy-stdio"
-version = "0.1.1"
+version = "0.1.2"
 description = "Default template for PDM package"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
-    "keyring-proxy>=0.1.7",
+    "keyring-proxy>=0.1.8",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/KalleDK/py-keyring-proxy-stdio"
 
 [project.entry-points."keyring.backends"]
-StdioProxyBackend = "keyring_proxy.stdioproxy:StdioProxyBackend"
+StdioProxyBackend = "keyring_proxy_stdioproxy:StdioProxyBackend"
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 tools = [
     "ruff>=0.4.6",
```

