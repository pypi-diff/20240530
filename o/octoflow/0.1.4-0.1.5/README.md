# Comparing `tmp/octoflow-0.1.4.tar.gz` & `tmp/octoflow-0.1.5.tar.gz`

## Comparing `octoflow-0.1.4.tar` & `octoflow-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/config.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/constants.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/core.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/exceptions.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/logging.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/plugin.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/typing.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/base.py
--rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/dataclass.py
--rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/dataset.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/expression.py
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/loaders.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/metadata.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/sampler.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/schema.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/data/types.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/__init__.py
--rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/artifact/__init__.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/tracking/artifact/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/cache.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/collections.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/config.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/func.py
--rw-r--r--   0        0        0    11582 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/hashing.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/objects.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/rsync.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.4/octoflow/utils/string.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.4/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.4/AUTHORS.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.4/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.4/README.md
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/config.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/constants.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/core.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/exceptions.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/logging.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/plugin.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/typing.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/base.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/dataclass.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/dataset.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/expression.py
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/loaders.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/metadata.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/sampler.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/schema.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/data/types.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/__init__.py
+-rw-r--r--   0        0        0    12381 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/artifact/__init__.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/tracking/artifact/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/cache.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/collections.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/config.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/func.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/hashing.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/objects.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/rsync.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 octoflow-0.1.5/octoflow/utils/string.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.5/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.5/AUTHORS.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.5/README.md
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.5/PKG-INFO
```

### Comparing `octoflow-0.1.4/octoflow/__init__.py` & `octoflow-0.1.5/octoflow/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 
 from octoflow import logging
 from octoflow.config import config
 from octoflow.utils.config import Config
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 __all__ = [
     "Config",
     "config",
     "logger",
     "logging",
 ]
```

### Comparing `octoflow-0.1.4/octoflow/config.py` & `octoflow-0.1.5/octoflow/config.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/core.py` & `octoflow-0.1.5/octoflow/core.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/logging.py` & `octoflow-0.1.5/octoflow/logging.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/plugin.py` & `octoflow-0.1.5/octoflow/plugin.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/__init__.py` & `octoflow-0.1.5/octoflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/base.py` & `octoflow-0.1.5/octoflow/data/base.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/dataclass.py` & `octoflow-0.1.5/octoflow/data/dataclass.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/dataset.py` & `octoflow-0.1.5/octoflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/expression.py` & `octoflow-0.1.5/octoflow/data/expression.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/loaders.py` & `octoflow-0.1.5/octoflow/data/loaders.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/metadata.py` & `octoflow-0.1.5/octoflow/data/metadata.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/sampler.py` & `octoflow-0.1.5/octoflow/data/sampler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/schema.py` & `octoflow-0.1.5/octoflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/data/types.py` & `octoflow-0.1.5/octoflow/data/types.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/tracking/models.py` & `octoflow-0.1.5/octoflow/tracking/models.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/tracking/artifact/handler.py` & `octoflow-0.1.5/octoflow/tracking/artifact/handler.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/utils/cache.py` & `octoflow-0.1.5/octoflow/utils/cache.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/utils/collections.py` & `octoflow-0.1.5/octoflow/utils/collections.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/utils/config.py` & `octoflow-0.1.5/octoflow/utils/config.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/utils/func.py` & `octoflow-0.1.5/octoflow/utils/func.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/utils/hashing.py` & `octoflow-0.1.5/octoflow/utils/hashing.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 """
 
 # Author: Gael Varoquaux <gael dot varoquaux at normalesup dot org>
 # Copyright (c) 2009 Gael Varoquaux
 # License: BSD Style, 3 clauses.
 
 import decimal
+import functools
+import inspect
 import io
 import logging
 import pickle  # noqa: S403
 import struct
 import sys
 import types
 from typing import (
     Any,
     Callable,
     Generic,
     Literal,
+    Optional,
     Type,
     TypeVar,
     overload,
     runtime_checkable,
 )
 
 import xxhash
@@ -109,21 +112,25 @@
             # them into components that make them uniquely identifiable
             if hasattr(obj, "__func__"):
                 func_name = obj.__func__.__name__
             else:
                 func_name = obj.__name__
             inst = obj.__self__
             if type(inst) is type(pickle):
-                obj = _MyHash(func_name, inst.__name__)
+                obj = _MyHash("==MethodType==", func_name, inst.__name__)
             elif inst is None:
                 # type(None) or type(module) do not pickle
-                obj = _MyHash(func_name, inst)
+                obj = _MyHash("==MethodType==", func_name, inst)
             else:
                 cls = obj.__self__.__class__
-                obj = _MyHash(func_name, inst, cls)
+                obj = _MyHash("==MethodType==", func_name, inst, cls)
+        if isinstance(obj, types.FunctionType):
+            pkl = pickle.dumps(obj)
+            src = inspect.getsource(obj)
+            obj = _MyHash("==FunctionType==", pkl, src)
         Pickler.save(self, obj)
 
     def memoize(self, obj):
         # We want hashing to be sensitive to value instead of reference.
         # For example we want ['aa', 'aa'] and ['aa', 'aaZ'[:2]]
         # to hash to the same value and that's why we disable memoization
         # for strings
@@ -317,14 +324,23 @@
         return getattr(self.cls, name)
 
 
 def init_based_hash(cls: Type[T]) -> Wrapped[T]:
     return Wrapped(cls)
 
 
-def hashable(func: Callable[P, T]) -> Callable[P, T]:
+def hashable(
+    func: Optional[Callable[P, T]] = None,
+    /,
+    *,
+    depends: Optional[Any] = None,
+) -> Callable[P, T]:
+    if func is None:
+        return functools.partial(hashable, depends=depends)
+
     def hash_repr() -> Any:
-        return _MyHash("==FunctionHash==", func)
+        pkl = pickle.dumps(func)
+        src = inspect.getsource(func)
+        return _MyHash("==WrappedFunction==", pkl, src, depends)
 
     func._hash_repr_ = hash_repr
-
     return func
```

### Comparing `octoflow-0.1.4/octoflow/utils/objects.py` & `octoflow-0.1.5/octoflow/utils/objects.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/utils/rsync.py` & `octoflow-0.1.5/octoflow/utils/rsync.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/octoflow/utils/string.py` & `octoflow-0.1.5/octoflow/utils/string.py`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/.gitignore` & `octoflow-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/LICENSE` & `octoflow-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/README.md` & `octoflow-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/pyproject.toml` & `octoflow-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octoflow-0.1.4/PKG-INFO` & `octoflow-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoflow
-Version: 0.1.4
+Version: 0.1.5
 Summary: Streamlining machine learning tracking for seamless experiment management.
 Project-URL: Documentation, https://github.com/ysenarath/octoflow
 Project-URL: Source, https://github.com/ysenarath/octoflow
 Author-email: Yasas Senarath <email@example.com>
 License-Expression: MIT
 License-File: AUTHORS.md
 License-File: LICENSE
```

