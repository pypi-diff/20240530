# Comparing `tmp/listless-0.1.6.tar.gz` & `tmp/listless-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "listless-0.1.6.tar", max compression
+gzip compressed data, was "listless-0.2.0.tar", max compression
```

## Comparing `listless-0.1.6.tar` & `listless-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1056 2022-02-11 23:27:58.165586 listless-0.1.6/LICENSE
--rw-r--r--   0        0        0      286 2023-08-14 21:42:09.540925 listless-0.1.6/listless/__about__.py
--rw-r--r--   0        0        0    20471 2023-08-14 21:42:28.301352 listless-0.1.6/listless/__init__.py
--rw-r--r--   0        0        0      385 2023-07-17 16:25:25.268807 listless-0.1.6/listless/__main__.py
--rw-r--r--   0        0        0      355 2023-04-28 16:52:22.392699 listless-0.1.6/listless/_meta.py
--rw-r--r--   0        0        0        0 2022-02-01 20:37:20.181695 listless-0.1.6/listless/py.typed
--rw-r--r--   0        0        0     2154 2023-08-14 21:41:55.218594 listless-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      816 2022-06-02 17:33:59.763392 listless-0.1.6/README.md
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 listless-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-02-22 14:17:28.891830 listless-0.2.0/LICENSE
+-rw-r--r--   0        0        0      816 2024-02-22 14:17:28.891830 listless-0.2.0/README.md
+-rw-r--r--   0        0        0      322 2024-02-22 14:17:28.891830 listless-0.2.0/listless/__about__.py
+-rw-r--r--   0        0        0    20715 2024-05-30 16:42:58.242846 listless-0.2.0/listless/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-03 17:50:22.123908 listless-0.2.0/listless/__main__.py
+-rw-r--r--   0        0        0      392 2024-03-21 23:48:47.629525 listless-0.2.0/listless/_meta.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:17:28.891830 listless-0.2.0/listless/py.typed
+-rw-r--r--   0        0        0     2155 2024-05-24 19:36:21.469830 listless-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 listless-0.2.0/PKG-INFO
```

### Comparing `listless-0.1.6/LICENSE` & `listless-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `listless-0.1.6/listless/__init__.py` & `listless-0.2.0/listless/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -*- coding: utf-8 -*-
 # pyright: reportInvalidTypeVarUse=false
 """Listless = generators, iterators, and async iterators, Oh My!"""
+
+from __future__ import annotations
+
 import asyncio
 
 from collections import deque
 from functools import reduce
 from itertools import chain, count, islice, tee, zip_longest
 from operator import iconcat, mul
 from typing import (
     Any,
     AsyncIterable,
     AsyncIterator,
     Callable,
+    Collection,
     Deque,
     Iterable,
     Iterator,
     List,
     Optional,
     Sequence,
     Set,
@@ -250,45 +254,46 @@
 
     if isinstance(seq, str):
         return False
     try:
         len(seq)
     except TypeError:
         return False
-    if is_subscriptable(seq):
-        return True
-    return False
+    return is_subscriptable(seq)
 
 
 def chunkseq(it: Sequence[_T], n: int) -> Iterable[Sequence[_T]]:
     """Yield chunks of size n from a Sequence"""
     return (it[i : i + n] for i in range(0, len(it), n))
 
 
 def chunkstr(string: str, n: int) -> Iterable[str]:
     """Yield chunks of size n from a string"""
     return (string[i : i + n] for i in range(0, len(string), n))
 
 
 @overload
-def chunks(it: str, chunk_size: int) -> Iterable[str]:
-    ...
+def chunks(it: str, chunk_size: int) -> Iterable[str]: ...
+
+
+@overload
+def chunks(it: List[_T], chunk_size: int) -> Iterable[List[_T]]: ...
 
 
 @overload
-def chunks(it: List[_T], chunk_size: int) -> Iterable[List[_T]]:
-    ...
+def chunks(it: Sequence[_T], chunk_size: int) -> Iterable[Sequence[_T]]: ...
 
 
 @overload
-def chunks(it: Sequence[_T], chunk_size: int) -> Iterable[Sequence[_T]]:
-    ...
+def chunks(it: Collection[_T], chunk_size: int) -> Iterable[Collection[_T]]: ...
 
 
-def chunks(it: Sequence[_T], chunk_size: int) -> Iterable[Union[Sequence[_T], str]]:
+def chunks(
+    it: Union[Sequence[_T], Collection[_T]], chunk_size: int
+) -> Iterable[Union[Sequence[_T], Collection[_T], str]]:
     """Yield chunks of something slice-able with length <= chunk_size
 
     Args:
         it (Iterable[Any]): Iterable to chunk
         chunk_size (int): Size of the chunks
 
     Returns:
@@ -310,25 +315,27 @@
         >>> list(chunks((el for el in range(10)), 4))
         [(0, 1, 2, 3), (4, 5, 6, 7), (8, 9)]
 
     """
     if isinstance(it, str):
         yield from chunkstr(it, chunk_size)
     elif isinstance(it, (list, tuple)) or is_sequence(it):
-        yield from chunkseq(it, chunk_size)
+        yield from chunkseq(cast(Sequence[_T], it), chunk_size)
     else:
         while True:
             _chunk = tuple(islice(it, chunk_size))
             if not _chunk:
                 break
             yield _chunk
 
 
-def chunk(it: Sequence[_T], n: int) -> Iterable[Sequence[_T]]:
-    """Yield chunks of size n from a Sequence
+def chunk(
+    it: Union[Sequence[_T], Collection[_T]], n: int
+) -> Iterable[Union[Sequence[_T], Collection[_T], str]]:
+    """Yield chunks of size n from an iterable/sequence/collection
 
     Examples:
         >>> list(chunk([1, 2, 3, 4, 5, 6], 3))
         [[1, 2, 3], [4, 5, 6]]
 
     """
     return chunks(it, n)
@@ -516,15 +523,15 @@
     )
 
 
 def flatten_strings(
     *args: Union[
         _T,
         Iterable[_T],
-    ]
+    ],
 ) -> Iterable[str]:
     """Flatten possibly nested iterables of sequences to a list of strings
 
     Examples:
         >>> from listless import flatten_strings
         >>> list(flatten_strings("cmd", ["uno", "dos", "tres"]))
         ['cmd', 'uno', 'dos', 'tres']
```

### Comparing `listless-0.1.6/pyproject.toml` & `listless-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [tool.poetry]
 name = "listless"
-version = "0.1.6"
+version = "0.2.0"
 description = "generator utils; aka listless"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/listless"
 readme = 'README.md'
 packages = [
   { include = "listless", from = "." },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Typing :: Typed",
 ]
 keywords = [
   "generators",
   "itertools",
   "dgpy",
   "typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4.0"
+pytest = "^8.2.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `listless-0.1.6/README.md` & `listless-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `listless-0.1.6/PKG-INFO` & `listless-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: listless
-Version: 0.1.6
+Version: 0.2.0
 Summary: generator utils; aka listless
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/listless
 License: MIT
 Keywords: generators,itertools,dgpy,typed
 Author: jesse
 Author-email: jesse@dgi.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/dynamic-graphics-inc/dgpy-libs">
 <img align="right" src="https://github.com/dynamic-graphics-inc/dgpy-libs/blob/main/docs/images/dgpy_banner.svg?raw=true" alt="drawing" height="120" width="300"/>
 </a>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: listless Version: 0.1.6 Summary: generator utils;
+Metadata-Version: 2.1 Name: listless Version: 0.2.0 Summary: generator utils;
 aka listless Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/
 main/libs/listless License: MIT Keywords: generators,itertools,dgpy,typed
-Author: jesse Author-email: jesse@dgi.com Requires-Python: >=3.7,<4.0
+Author: jesse Author-email: jesse@dgi.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Typing :: Typed Project-URL:
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Typing :: Typed Project-URL:
 Repository, https://github.com/dynamic-graphics-inc/dgpy-libs Description-
 Content-Type: text/markdown _[_d_r_a_w_i_n_g_]# listless [![Wheel](https://
 img.shields.io/pypi/wheel/listless.svg)](https://img.shields.io/pypi/wheel/
 listless.svg) [![Version](https://img.shields.io/pypi/v/listless.svg)](https://
 img.shields.io/pypi/v/listless.svg) [![py_versions](https://img.shields.io/
 pypi/pyversions/listless.svg)](https://img.shields.io/pypi/pyversions/
 listless.svg) [![Code style: black](https://img.shields.io/badge/code%20style-
```

