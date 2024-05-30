# Comparing `tmp/dead_simple_cache-1.2.0-py3-none-any.whl.zip` & `tmp/dead_simple_cache-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7399 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     3154 b- defN 24-May-28 20:06 dead_simple_cache/__init__.py
--rw-rw-r--  2.0 unx      177 b- defN 24-May-28 19:34 dead_simple_cache/version.py
--rw-rw-r--  2.0 unx    11359 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1072 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx      703 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/RECORD
-8 files, 16576 bytes uncompressed, 6153 bytes compressed:  62.9%
+Zip file size: 7344 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     2919 b- defN 24-May-29 18:54 dead_simple_cache/__init__.py
+-rw-rw-r--  2.0 unx      177 b- defN 24-May-29 18:54 dead_simple_cache/version.py
+-rw-rw-r--  2.0 unx    11359 b- defN 24-May-29 18:56 dead_simple_cache-1.2.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1072 b- defN 24-May-29 18:56 dead_simple_cache-1.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-29 18:56 dead_simple_cache-1.2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 24-May-29 18:56 dead_simple_cache-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 24-May-29 18:56 dead_simple_cache-1.2.1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      703 b- defN 24-May-29 18:56 dead_simple_cache-1.2.1.dist-info/RECORD
+8 files, 16341 bytes uncompressed, 6098 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: dead_simple_cache/__init__.py
 Comment: 
 
 Filename: dead_simple_cache/version.py
 Comment: 
 
-Filename: dead_simple_cache-1.2.0.dist-info/LICENSE
+Filename: dead_simple_cache-1.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: dead_simple_cache-1.2.0.dist-info/METADATA
+Filename: dead_simple_cache-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: dead_simple_cache-1.2.0.dist-info/WHEEL
+Filename: dead_simple_cache-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: dead_simple_cache-1.2.0.dist-info/top_level.txt
+Filename: dead_simple_cache-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dead_simple_cache-1.2.0.dist-info/zip-safe
+Filename: dead_simple_cache-1.2.1.dist-info/zip-safe
 Comment: 
 
-Filename: dead_simple_cache-1.2.0.dist-info/RECORD
+Filename: dead_simple_cache-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dead_simple_cache/__init__.py

```diff
@@ -1,11 +1,10 @@
 import os
 from threading import Lock
 import shelve
-from bisect import insort
 import logging
 from typing import Any, Optional
 from rapidfuzz.distance import DamerauLevenshtein
 
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
@@ -16,33 +15,33 @@
 class SimpleCache:
     """Simple cache."""
 
     def __init__(self, file_path: str, fuzzy_threshold: float = 0.75):
         if not file_path:
             logger.error("error setting cache: 'path' must be set")
             raise ValueError("'path' must be set")
+
         try:
             full_path = os.path.abspath(os.path.expanduser(file_path))
             base_dir = os.path.dirname(full_path)
             os.makedirs(base_dir, exist_ok=True)
         except Exception as e:
             logger.error(f"error setting cache: {e}")
             raise ValueError(e)
+
         if full_path not in FILE_LOCKS:
             FILE_LOCKS[full_path] = Lock()
         self._lock = FILE_LOCKS[full_path]
+
         # Open database for reading and writing
         self._db = shelve.open(file_path, flag='c', protocol=None, writeback=False)
         self._threshold = fuzzy_threshold
-        with self._lock:
-            self.keys = list(sorted(self._db.keys()))
 
     def __del__(self) -> None:
         with self._lock:
-            self._db.sync()
             self._db.close()
 
     def _match(self, key: str, query: str) -> float:
         """Fuzzy matching helper method."""
         return DamerauLevenshtein.normalized_similarity(key, query) >= self._threshold
 
     def _get(self, key: str) -> dict:
@@ -51,44 +50,41 @@
             data = self._db.get(key, default=[])
         return {key: data} if data else {}
 
     def _fuzzy_get(self, query: str) -> dict:
         """Get data with fuzzy matching."""
         with self._lock:
             keys = list(
-                    filter(
-                        lambda key: self._match(key, query),
-                        self.keys
-                    )
+                filter(
+                    lambda key: self._match(key, query),
+                    sorted(self._db.keys())
                 )
+            )
             data = [self._db[key] for key in keys]
         return dict(zip(keys, data)) if keys else {}
 
     def replace(self, key: Any, data: Any) -> None:
         """Replace data."""
         key_ = str(key).lower()
         with self._lock:
             self._db[key_] = data if isinstance(data, list) else [data]
 
     def delete(self, key: Any) -> None:
         key_ = str(key).lower()
         with self._lock:
-            if key_ in self.keys:
+            if key_ in self._db:
                 del self._db[key_]
-                self.keys.remove(key_)
 
     def add(self, key: Any, data: Any) -> None:
         """Add data."""
         data_ = []
         key_ = str(key).lower()
         with self._lock:
-            if key_ in self.keys:
+            if key_ in self._db:
                 data_ = self._db[key_]
-            else:
-                insort(self.keys, key_)
             if isinstance(data, list):
                 data_.extend(data)
             else:
                 data_.append(data)
             self._db[key_] = data_
 
     def get(self, query: Any, fuzzy: bool = False) -> Optional[dict]:
```

## dead_simple_cache/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 1
 VERSION_MINOR = 2
-VERSION_BUILD = 0
+VERSION_BUILD = 1
 VERSION_ALPHA = 0
 # END_VERSION_BLOCK
```

## Comparing `dead_simple_cache-1.2.0.dist-info/LICENSE` & `dead_simple_cache-1.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dead_simple_cache-1.2.0.dist-info/METADATA` & `dead_simple_cache-1.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dead-simple-cache
-Version: 1.2.0
+Version: 1.2.1
 Summary: A dead simple caching lib
 Home-page: https://github.com/femelo/dead-simple-cache
 Author: Flávio De Melo
 Author-email: flavio.eler@gmail.com
 License: Apache 2.0
 Keywords: caching
 Description-Content-Type: text/markdown
```

## Comparing `dead_simple_cache-1.2.0.dist-info/RECORD` & `dead_simple_cache-1.2.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dead_simple_cache/__init__.py,sha256=xTr9dRhtU32HBu1jQbVtZG8AgP0VVs8M1wOPFwE2uqA,3154
-dead_simple_cache/version.py,sha256=xkoU9LVlDlOSIZ00Z6I4UlYCHlCNGapNzUksvH9hl3I,177
-dead_simple_cache-1.2.0.dist-info/LICENSE,sha256=jG2zQEdRNt88EgHUWPpXVWmOrOduUQRx7MnYV9YIPaw,11359
-dead_simple_cache-1.2.0.dist-info/METADATA,sha256=9t2Xy4CDf7K1NMGjiJVXYHtdlFpF9JeVaoNchAfLVx4,1072
-dead_simple_cache-1.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dead_simple_cache-1.2.0.dist-info/top_level.txt,sha256=rTXFTTGmSN_J-s3wSqL0KtbHyyZ2oA_-kyWEt6-e0Ss,18
-dead_simple_cache-1.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-dead_simple_cache-1.2.0.dist-info/RECORD,,
+dead_simple_cache/__init__.py,sha256=EjlfB6Sco8sph9qhGt_5yl5Wpr2_xssCRwbrniFi24c,2919
+dead_simple_cache/version.py,sha256=t4eM3GSz7xU2OQdlylcw_dUJnI5VtTFJ0NFFMQryvF8,177
+dead_simple_cache-1.2.1.dist-info/LICENSE,sha256=jG2zQEdRNt88EgHUWPpXVWmOrOduUQRx7MnYV9YIPaw,11359
+dead_simple_cache-1.2.1.dist-info/METADATA,sha256=PULIc1RqGxw2LlqUMmCmgddCOJt_xdP1BtUokctnPDI,1072
+dead_simple_cache-1.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dead_simple_cache-1.2.1.dist-info/top_level.txt,sha256=rTXFTTGmSN_J-s3wSqL0KtbHyyZ2oA_-kyWEt6-e0Ss,18
+dead_simple_cache-1.2.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+dead_simple_cache-1.2.1.dist-info/RECORD,,
```

