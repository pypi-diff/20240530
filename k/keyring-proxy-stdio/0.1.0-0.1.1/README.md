# Comparing `tmp/keyring_proxy_stdio-0.1.0.tar.gz` & `tmp/keyring_proxy_stdio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy_stdio-0.1.0.tar", last modified: Thu May 30 10:49:27 2024, max compression
+gzip compressed data, was "keyring_proxy_stdio-0.1.1.tar", last modified: Thu May 30 10:52:44 2024, max compression
```

## Comparing `keyring_proxy_stdio-0.1.0.tar` & `keyring_proxy_stdio-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.0/README.md
--rw-r--r--   0        0        0      854 2024-05-30 10:49:27.951641 keyring_proxy_stdio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.0/src/keyring_proxy_stdio/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 keyring_proxy_stdio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.1/README.md
+-rw-r--r--   0        0        0      854 2024-05-30 10:52:44.898929 keyring_proxy_stdio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.1/src/keyring_proxy_stdio/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 keyring_proxy_stdio-0.1.1/PKG-INFO
```

### Comparing `keyring_proxy_stdio-0.1.0/pyproject.toml` & `keyring_proxy_stdio-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "keyring-proxy-stdio"
-version = "0.1.0"
+version = "0.1.1"
 description = "Default template for PDM package"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
-    "keyring-proxy>=0.1.6",
+    "keyring-proxy>=0.1.7",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

