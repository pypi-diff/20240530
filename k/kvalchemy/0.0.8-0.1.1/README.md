# Comparing `tmp/kvalchemy-0.0.8.tar.gz` & `tmp/kvalchemy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvalchemy-0.0.8.tar", last modified: Sat May 25 23:51:49 2024, max compression
+gzip compressed data, was "kvalchemy-0.1.1.tar", last modified: Thu May 30 01:30:19 2024, max compression
```

## Comparing `kvalchemy-0.0.8.tar` & `kvalchemy-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.859967 kvalchemy-0.0.8/kvalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/kvalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.764027 kvalchemy-0.1.1/kvalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/kvalchemy/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/kvalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 01:30:19.000000 kvalchemy-0.1.1/kvalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 01:30:19.768027 kvalchemy-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-30 01:30:09.000000 kvalchemy-0.1.1/tests/test_time.py
```

### Comparing `kvalchemy-0.0.8/LICENSE.md` & `kvalchemy-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.8/PKG-INFO` & `kvalchemy-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.8
+Version: 0.1.1
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -66,10 +66,21 @@
 
 On Python 3.8 or later:
 
 ```
 pip install kvalchemy
 ```
 
+## Versioning
+
+```
+Note that the database format is stable across the same patch version.
+
+For example: Version 0.0.1 will be fully compatible with all releases in the 0.0.X family.
+Though Version 0.1.0 may not be directly compatible without a manual data migration.
+
+Make sure to pin the version family you want: kvalachemy<X.(Y+1).0
+```
+
 ## More Documentation
 
 For more documentation visit: https://csm10495.github.io/kvalchemy
```

### Comparing `kvalchemy-0.0.8/kvalchemy/client.py` & `kvalchemy-0.1.1/kvalchemy/client.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.8/kvalchemy/models.py` & `kvalchemy-0.1.1/kvalchemy/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Home to models for KVAlchemy.
 """
 from datetime import datetime
 
 from sqlalchemy import Column, ColumnElement, UniqueConstraint, or_
+from sqlalchemy.dialects.mysql import LONGBLOB
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
-from sqlalchemy.types import PickleType, Unicode
+from sqlalchemy.types import LargeBinary, PickleType, Unicode
 
 from kvalchemy.time import db_now
 
 KEY_MAX_LENGTH = 256
 TAG_MAX_LENGTH = 256
 
 
@@ -22,15 +23,17 @@
 
 
 class ValueMixIn:
     """
     A mixin used to correspond with an object with a value attribute
     """
 
-    value = Column("value", PickleType)
+    value = Column(
+        "value", PickleType(impl=LargeBinary().with_variant(LONGBLOB, "mysql"))
+    )
 
     def __init__(self, value):
         self.value = value
 
 
 class KVStore(Base, ValueMixIn):
     """
```

### Comparing `kvalchemy-0.0.8/kvalchemy/proxy.py` & `kvalchemy-0.1.1/kvalchemy/proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.8/kvalchemy/time.py` & `kvalchemy-0.1.1/kvalchemy/time.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.8/kvalchemy.egg-info/PKG-INFO` & `kvalchemy-0.1.1/kvalchemy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.8
+Version: 0.1.1
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -66,10 +66,21 @@
 
 On Python 3.8 or later:
 
 ```
 pip install kvalchemy
 ```
 
+## Versioning
+
+```
+Note that the database format is stable across the same patch version.
+
+For example: Version 0.0.1 will be fully compatible with all releases in the 0.0.X family.
+Though Version 0.1.0 may not be directly compatible without a manual data migration.
+
+Make sure to pin the version family you want: kvalachemy<X.(Y+1).0
+```
+
 ## More Documentation
 
 For more documentation visit: https://csm10495.github.io/kvalchemy
```

### Comparing `kvalchemy-0.0.8/pyproject.toml` & `kvalchemy-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.8/tests/test_client.py` & `kvalchemy-0.1.1/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,7 +350,20 @@
         return counter < 4
 
     @kvalchemy.memoize(skip_saving_to_cache_if=skip_saving_to_cache_if)
     def y():
         return uuid4()
 
     assert len({y() for _ in range(10)}) == 4
+
+
+@pytest.mark.parametrize(
+    "value",
+    [
+        [1] * 1000,
+        [None] * 60000,
+        list(range(10)) * 100000,
+    ],
+)
+def test_big_value(kvalchemy, value):
+    kvalchemy.set("key", value)
+    assert kvalchemy.get("key") == value
```

### Comparing `kvalchemy-0.0.8/tests/test_proxy.py` & `kvalchemy-0.1.1/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.8/tests/test_time.py` & `kvalchemy-0.1.1/tests/test_time.py`

 * *Files identical despite different names*

