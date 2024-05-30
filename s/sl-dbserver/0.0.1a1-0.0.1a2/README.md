# Comparing `tmp/sl-dbserver-0.0.1a1.tar.gz` & `tmp/sl_dbserver-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sl-dbserver-0.0.1a1.tar", last modified: Thu Feb  9 15:36:18 2023, max compression
+gzip compressed data, was "sl_dbserver-0.0.1a2.tar", last modified: Thu May 30 01:15:58 2024, max compression
```

## Comparing `sl-dbserver-0.0.1a1.tar` & `sl_dbserver-0.0.1a2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1058 2023-02-06 15:15:22.000000 sl-dbserver-0.0.1a1/LICENSE.md
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1740 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/PKG-INFO
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1286 2023-02-08 07:36:00.000000 sl-dbserver-0.0.1a1/README.md
--rw-r--r--   0 cogs      (1000) cogs      (1001)       38 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/setup.cfg
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1656 2023-02-09 15:26:48.000000 sl-dbserver-0.0.1a1/setup.py
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/sl/
--rw-r--r--   0 cogs      (1000) cogs      (1001)      132 2023-02-06 15:15:22.000000 sl-dbserver-0.0.1a1/src/sl/__init__.py
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/sl/dbserver/
--rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-06 15:15:22.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/__init__.py
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/
--rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/__init__.py
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/db/
--rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/db/__init__.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1212 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/db/models.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1974 2023-02-09 15:26:04.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/fixtures.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     2411 2023-02-09 15:26:04.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/_test_app.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)      371 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/_test_db.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1944 2023-02-09 15:26:04.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/app.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)       36 2023-02-08 07:36:00.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/cli.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)      215 2023-02-09 15:26:04.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/conftest.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     2558 2023-02-09 15:26:04.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/db.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     6092 2023-02-09 15:26:04.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/types.py
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/sl/dbserver/util/
--rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/__init__.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)      592 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/_test_file.py
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/
--rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/__init__.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1436 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/_test_url.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     2907 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/conn.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)      760 2023-02-09 03:45:55.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/schema.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     2663 2023-02-09 15:26:04.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/seed.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     3525 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/serialize.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     2505 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/url.py
--rw-r--r--   0 cogs      (1000) cogs      (1001)     3274 2023-02-08 02:08:58.000000 sl-dbserver-0.0.1a1/src/sl/dbserver/util/file.py
-drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2023-02-09 15:36:18.246681 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1740 2023-02-09 15:36:18.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/PKG-INFO
--rw-r--r--   0 cogs      (1000) cogs      (1001)     1064 2023-02-09 15:36:18.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/SOURCES.txt
--rw-r--r--   0 cogs      (1000) cogs      (1001)        1 2023-02-09 15:36:18.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/dependency_links.txt
--rw-r--r--   0 cogs      (1000) cogs      (1001)       61 2023-02-09 15:36:18.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/entry_points.txt
--rw-r--r--   0 cogs      (1000) cogs      (1001)        3 2023-02-09 15:36:18.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/namespace_packages.txt
--rw-r--r--   0 cogs      (1000) cogs      (1001)        1 2023-02-05 01:08:04.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/not-zip-safe
--rw-r--r--   0 cogs      (1000) cogs      (1001)      270 2023-02-09 15:36:18.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/requires.txt
--rw-r--r--   0 cogs      (1000) cogs      (1001)        3 2023-02-09 15:36:18.000000 sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/top_level.txt
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     1058 2023-02-06 15:15:22.000000 sl_dbserver-0.0.1a2/LICENSE.md
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     2418 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/PKG-INFO
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     1286 2023-02-08 07:36:00.000000 sl_dbserver-0.0.1a2/README.md
+-rw-r--r--   0 cogs      (1000) cogs      (1001)       38 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/setup.cfg
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     1656 2024-05-30 01:04:02.000000 sl_dbserver-0.0.1a2/setup.py
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.351261 sl_dbserver-0.0.1a2/src/
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/src/sl/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)      132 2023-02-06 15:15:22.000000 sl_dbserver-0.0.1a2/src/sl/__init__.py
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/src/sl/dbserver/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-06 15:15:22.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/__init__.py
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/__init__.py
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/db/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/db/__init__.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     1212 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/db/models.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     2064 2023-02-28 03:45:55.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/fixtures.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     3640 2023-02-28 03:45:55.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/_test_app.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)      371 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/_test_db.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     1856 2024-05-26 00:27:00.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/app.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)       36 2023-02-08 07:36:00.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/cli.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)      241 2023-02-28 03:45:55.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/conftest.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     2794 2023-02-28 03:45:55.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/db.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     6111 2023-02-28 03:45:55.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/types.py
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/src/sl/dbserver/util/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/__init__.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)      592 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/_test_file.py
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        0 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/__init__.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     1760 2024-05-30 00:55:09.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/_test_url.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     2907 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/conn.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)      947 2023-02-28 03:45:55.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/schema.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     2663 2023-02-09 15:26:04.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/seed.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     3525 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/serialize.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     2505 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/url.py
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     3274 2023-02-08 02:08:58.000000 sl_dbserver-0.0.1a2/src/sl/dbserver/util/file.py
+drwxr-xr-x   0 cogs      (1000) cogs      (1001)        0 2024-05-30 01:15:58.354594 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     2418 2024-05-30 01:15:58.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/PKG-INFO
+-rw-r--r--   0 cogs      (1000) cogs      (1001)     1064 2024-05-30 01:15:58.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/SOURCES.txt
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        1 2024-05-30 01:15:58.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/dependency_links.txt
+-rw-r--r--   0 cogs      (1000) cogs      (1001)       61 2024-05-30 01:15:58.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/entry_points.txt
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        3 2024-05-30 01:15:58.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/namespace_packages.txt
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        1 2023-02-05 01:08:04.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/not-zip-safe
+-rw-r--r--   0 cogs      (1000) cogs      (1001)      270 2024-05-30 01:15:58.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/requires.txt
+-rw-r--r--   0 cogs      (1000) cogs      (1001)        3 2024-05-30 01:15:58.000000 sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/top_level.txt
```

### Comparing `sl-dbserver-0.0.1a1/LICENSE.md` & `sl_dbserver-0.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/PKG-INFO` & `sl_dbserver-0.0.1a2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sl-dbserver
-Version: 0.0.1a1
-Summary: Springless Database Server
-Home-page: https://github.com/Springless/sl-dbserver
-Author: cogs
-Author-email: cogs@springless.com
-License: MIT
-Keywords: sl springless database server testing postgresql
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development :: Testing
-Provides-Extra: dev
-License-File: LICENSE.md
-
 # Springless DB Server (sl-dbserver)
 
 This is a simple Python server for the purpose of spinning up and destroying full copies of a
 database on demand. An example use-case is running integration tests with a local postgres
 instance in a docker container. Each test can create its own isolated database, run its
 tests, and then destroy the created database instance when done.
```

### Comparing `sl-dbserver-0.0.1a1/setup.py` & `sl_dbserver-0.0.1a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "alembic               >= 1",
     "build",
     "twine",
 ]
 
 setup(
     name="sl-dbserver",
-    version="0.0.1a1",
+    version="0.0.1a2",
     license="MIT",
     description="Springless Database Server",
     long_description=README,
     author="cogs",
     author_email="cogs@springless.com",
     url="https://github.com/Springless/sl-dbserver",
     packages=find_packages("src"),
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/db/models.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/db/models.py`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/__test__/fixtures.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/__test__/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,44 +25,46 @@
 
 @_pytest.fixture(scope="function")
 def sldb_test_schema_module() -> str:
     return "sl.dbserver.__test__.db.models:metadata"
 
 
 @_pytest.fixture(scope="function")
+def sldb_test_schema_def(sldb_test_schema_module) -> _types.SchemaDef:
+    return _types.SchemaDef(type="sqlalchemy", value=sldb_test_schema_module)
+
+
+@_pytest.fixture(scope="function")
 def sldb_test_seed_data() -> _t.List[_types.SeedData]:
     return [
         _types.SeedData(type="module", value="sl.dbserver.__test__:seeds/test01.json")
     ]
 
 
 @_pytest.fixture(scope="function")
 def sldb_test_reset_seq() -> bool:
     return True
 
 
 @_pytest.fixture(scope="function")
 def sldb_url(
     sldb_test_url,
-    sldb_test_schema_module,
+    sldb_test_schema_def,
     request,
     sldb_test_seed_data,
     sldb_test_reset_seq,
 ):
     """Creates, yields, and cleans up a testing database"""
     test_name = request.node.name
     response = _app.create_db(
         _types.CreateDbArgs(
             url=sldb_test_url,
             append_name=test_name,
             with_timestamp=True,
-            schema=_types.SchemaDef(
-                type="sqlalchemy",
-                value=sldb_test_schema_module,
-            ),
+            schema=sldb_test_schema_def,
             seeds=sldb_test_seed_data,
             reset_seq=sldb_test_reset_seq,
         )
     )
     yield response.url
     _app.drop_db(_types.DropDbArgs(drop_id=response.drop_id))
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/_test_app.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/_test_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sqlalchemy_utils as _su
 import sqlalchemy as _sa
 import sqlalchemy.engine as _sae
 import pytest as _pytest
 from . import app as _app
 from . import types as _types
 from .__test__.db import models as _m
+from .util import file as _file
 
 _TC = _ut.TestCase()
 
 
 def test_create_drop_test_db(sldb_test_url, sldb_test_schema_module):
     response = _app.create_db(
         _types.CreateDbArgs(
@@ -74,8 +75,44 @@
         all_users = sldb_conn.execute(_sa.select(_m.User)).all()
         _TC.assertEqual(
             all_users,
             [
                 (1, "user1", "user1@email.com"),
                 (2, "user2", "user2@email.com"),
             ],
+        )
+
+
+class TestSqlSchema:
+    @_pytest.fixture(scope="function")
+    def sldb_test_schema_def(self) -> _types.SchemaDef:
+        path_to_schema = _file.module_path("sl.dbserver.__test__:schema.sql")
+        return _types.SchemaDef(type="file", value=path_to_schema)
+
+    def test_load_sql_schema(self, sldb_conn):
+        all_users = sldb_conn.execute(_sa.select(_m.User)).all()
+        _TC.assertEqual(
+            all_users,
+            [
+                (1, "user1", "user1@email.com"),
+                (2, "user2", "user2@email.com"),
+            ],
+        )
+
+
+class TestRawSqlSchema:
+    @_pytest.fixture(scope="function")
+    def sldb_test_schema_def(self) -> _types.SchemaDef:
+        path_to_schema = _file.module_path("sl.dbserver.__test__:schema.sql")
+        with open(path_to_schema, "r") as f:
+            raw_sql = f.read()
+        return _types.SchemaDef(type="raw_sql", value=raw_sql)
+
+    def test_load_sql_schema(self, sldb_conn):
+        all_users = sldb_conn.execute(_sa.select(_m.User)).all()
+        _TC.assertEqual(
+            all_users,
+            [
+                (1, "user1", "user1@email.com"),
+                (2, "user2", "user2@email.com"),
+            ],
         )
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/app.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import fastapi as _fapi
 import datetime as _dt
-import sqlalchemy as _sa
-import sqlalchemy.engine as _sae
 from .util.db import (
     url as _dbu_url,
     conn as _dbu_conn,
 )
-from .util import file as _fu
 from . import (
     types as _types,
     db as _db,
 )
 
 
 def create_db(args: _types.CreateDbArgs = _fapi.Body()) -> _types.CreatedDb:
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/db.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
 
 def create_schema(url: _sae.URL | str, schema: _types.SchemaDef):
     """Uses the schema definition to create the schema inside the passed database url"""
     match schema.type:
         case "sqlalchemy":
             _dbu_schema.load_sqlalchemy_schema(url, schema.value)
+        case "file":
+            with open(schema.value, "r") as f:
+                fdata = f.read()
+            _dbu_schema.load_sql_schema(url, fdata)
+        case "raw_sql":
+            _dbu_schema.load_sql_schema(url, schema.value)
 
 
 def _seed_data_from_file(fname: str) -> _types.SeedData:
     fext = _pl.Path(fname).suffix.lower()
     match fext:
         case ".json":
             ftype = "json"
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/types.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 - `raw_sql` - Raw SQL passed in through the value which will create the schema.
 """
 
 
 class SchemaDef(_pyd.BaseModel):
     """Define how to load the schema"""
 
-    type: _t.Literal["sqlalchemy"] = _pyd.Field(
+    type: _t.Literal["sqlalchemy", "file", "raw_sql"] = _pyd.Field(
         title="Type", description=_schemadef_type_desc
     )
     value: str = _pyd.Field(
         title="Value",
         description=(
             "Value that corresponds to the type. See the type field for more information."
         ),
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/_test_file.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/_test_file.py`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/_test_url.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/_test_url.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,24 @@
         at_timestamp=_use_timestamp,
     )
     _TC.assertEqual(
         created_name,
         "20220423140534_my_database_my_appended_and_very_long_tes5119",
     )
 
+def test_make_db_name_long_2():
+    created_name = _dbu.make_db_name(
+        "my_database",
+        append="My appended and very long test name string thing",
+        at_timestamp=_use_timestamp,
+    )
+    _TC.assertEqual(
+        created_name,
+        "20220423140534_my_database_my_appended_and_very_long_tesbf3f",
+    )
 
 def test_make_db_name_no_timestamp():
     created_name = _dbu.make_db_name(
         "my_database",
         append="My appended string",
     )
     _TC.assertEqual(
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/conn.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/conn.py`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/schema.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,21 @@
         raise _types.ApiError(
             message=f"Not a valid sqlalchemy metadata object: {value}"
         ).to_httperr()
     engine = _sae.create_engine(url)
     metadata.create_all(engine)
 
 
+def load_sql_schema(url: _sae.URL | str, value: str):
+    engine = _sae.create_engine(url)
+    with engine.connect() as conn:
+        with conn.begin():
+            conn.execute(value)
+
+
 def metadata_from_str(metadata_str: str) -> _sa.MetaData:
     metadata = _fu.import_from_str(metadata_str)
     if not isinstance(metadata, _sa.MetaData):
         raise _types.ApiError(
             message=f"Not a valid metadata module: {metadata_str}"
         ).to_httperr()
     return metadata
```

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/seed.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/seed.py`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/serialize.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/serialize.py`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/db/url.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/db/url.py`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/src/sl/dbserver/util/file.py` & `sl_dbserver-0.0.1a2/src/sl/dbserver/util/file.py`

 * *Files identical despite different names*

### Comparing `sl-dbserver-0.0.1a1/src/sl_dbserver.egg-info/SOURCES.txt` & `sl_dbserver-0.0.1a2/src/sl_dbserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

