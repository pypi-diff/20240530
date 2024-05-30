# Comparing `tmp/fast_verify-0.1.0.tar.gz` & `tmp/fast_verify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_verify-0.1.0.tar", max compression
+gzip compressed data, was "fast_verify-0.1.1.tar", max compression
```

## Comparing `fast_verify-0.1.0.tar` & `fast_verify-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      358 2024-05-11 16:42:30.241779 fast_verify-0.1.0/README.md
--rw-r--r--   0        0        0     3668 2024-05-11 16:49:29.224901 fast_verify-0.1.0/fast_verify/__init__.py
--rw-r--r--   0        0        0      350 2024-05-11 16:35:49.876203 fast_verify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 fast_verify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-18 10:53:44.388801 fast_verify-0.1.1/LICENSE
+-rw-r--r--   0        0        0      358 2024-05-11 16:42:30.241779 fast_verify-0.1.1/README.md
+-rw-r--r--   0        0        0     3658 2024-05-30 11:39:40.859416 fast_verify-0.1.1/fast_verify/__init__.py
+-rw-r--r--   0        0        0      350 2024-05-30 11:39:46.281884 fast_verify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 fast_verify-0.1.1/PKG-INFO
```

### Comparing `fast_verify-0.1.0/fast_verify/__init__.py` & `fast_verify-0.1.1/fast_verify/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 from functools import cache, cached_property
-from typing import ClassVar, Protocol, override, runtime_checkable
+from typing import ClassVar, Protocol, runtime_checkable
 from hmac import compare_digest, HMAC
 from hashlib import pbkdf2_hmac
 
 
 class InvalidSignature(Exception): ...
```

### Comparing `fast_verify-0.1.0/PKG-INFO` & `fast_verify-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-verify
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Chongchen Chen
 Author-email: chenkovsky@qq.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

