# Comparing `tmp/pysquril-0.7.0.tar.gz` & `tmp/pysquril-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysquril-0.7.0.tar", max compression
+gzip compressed data, was "pysquril-1.0.0.tar", max compression
```

## Comparing `pysquril-0.7.0.tar` & `pysquril-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3262 2024-05-27 10:01:31.474077 pysquril-0.7.0/README.md
--rw-r--r--   0        0        0      539 2024-05-27 10:01:31.474077 pysquril-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/__init__.py
--rw-r--r--   0        0        0    38193 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/backends.py
--rw-r--r--   0        0        0      412 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/exc.py
--rw-r--r--   0        0        0    25460 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/generator.py
--rw-r--r--   0        0        0     2423 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/interactive.py
--rw-r--r--   0        0        0    15251 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/parser.py
--rw-r--r--   0        0        0     2629 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/test_data.py
--rw-r--r--   0        0        0    35659 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/tests.py
--rw-r--r--   0        0        0      406 2024-05-27 10:01:31.474077 pysquril-0.7.0/pysquril/utils.py
--rw-r--r--   0        0        0     3999 1970-01-01 00:00:00.000000 pysquril-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3262 2024-05-30 10:11:31.686270 pysquril-1.0.0/README.md
+-rw-r--r--   0        0        0      539 2024-05-30 10:11:31.686270 pysquril-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/__init__.py
+-rw-r--r--   0        0        0    38205 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/backends.py
+-rw-r--r--   0        0        0      412 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/exc.py
+-rw-r--r--   0        0        0    25460 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/generator.py
+-rw-r--r--   0        0        0     2423 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/interactive.py
+-rw-r--r--   0        0        0    15251 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/parser.py
+-rw-r--r--   0        0        0     2629 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/test_data.py
+-rw-r--r--   0        0        0    35858 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/tests.py
+-rw-r--r--   0        0        0      406 2024-05-30 10:11:31.686270 pysquril-1.0.0/pysquril/utils.py
+-rw-r--r--   0        0        0     3999 1970-01-01 00:00:00.000000 pysquril-1.0.0/PKG-INFO
```

### Comparing `pysquril-0.7.0/README.md` & `pysquril-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pysquril-0.7.0/pyproject.toml` & `pysquril-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysquril"
-version = "0.7.0"
+version = "1.0.0"
 description = "Python implementation of structured URI query language"
 readme = "README.md"
 repository = "https://github.com/unioslo/pysquril"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
     "Eirik Haatveit <haatveit@uio.no>",
 ]
```

### Comparing `pysquril-0.7.0/pysquril/backends.py` & `pysquril-1.0.0/pysquril/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,15 +511,15 @@
         neccesary = table_name.endswith(AUDIT_SEPARATOR + AUDIT_SUFFIX)
         if not neccesary:
             return neccesary and sufficient
         try:
             dummy_event = AuditTransaction("").event_read(query="")
             result = list(
                 self._yield_results(
-                    f"select data from {table_name} limit 1"
+                    f"select data from {self._fqtn(table_name)} limit 1"
                 )
             )[0]
             sufficient = (
                 uuid.UUID(result.get("transaction_id"))
                 and uuid.UUID(result.get("event_id"))
                 and result.get("event") in ["update", "delete", "read", "create"]
                 and result.get("timestamp") is not None
```

### Comparing `pysquril-0.7.0/pysquril/generator.py` & `pysquril-1.0.0/pysquril/generator.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.7.0/pysquril/interactive.py` & `pysquril-1.0.0/pysquril/interactive.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.7.0/pysquril/parser.py` & `pysquril-1.0.0/pysquril/parser.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.7.0/pysquril/test_data.py` & `pysquril-1.0.0/pysquril/test_data.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.7.0/pysquril/tests.py` & `pysquril-1.0.0/pysquril/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,20 @@
     WhereClause,
     GroupByTerm,
     GroupByClause,
     AlterClause,
     UriQuery,
 )
 from pysquril.test_data import dataset
-from pysquril.utils import audit_table
+from pysquril.utils import audit_table, AUDIT_SEPARATOR, AUDIT_SUFFIX
 
 
 TEST_REQUESTOR = "p11-treq"
 TEST_REQUESTOR_NAME = "Test Requestor"
+AUDIT_END = f"{AUDIT_SEPARATOR}{AUDIT_SUFFIX}"
 
 class TestParser(object):
 
     def test_select(self) -> None:
         c = SelectClause("x[*|a,b],y.z")
         assert len(c.split_clause()) == 2
 
@@ -221,15 +222,15 @@
         try:
             db.table_delete('silly_table', '')
             db.table_delete(audit_table('silly_table'), '')
         except Exception as e:
             pass
 
         # test '*' without any tables
-        out = list(db.table_select('*', 'select=count(1)', exclude_endswith = ['_audit', '_metadata']))
+        out = list(db.table_select('*', 'select=count(1)', exclude_endswith = [AUDIT_END, '_metadata']))
         assert list(out) == []
 
         # create tables
         db.table_insert('test_table', data)
         db.table_insert('another_table', data)
 
         # SELECT
@@ -320,43 +321,43 @@
         out = run_select_query('select=max(q.r[0|s])')
         assert out == [[77]]
 
         if verbose:
             print('\n===> BROADCASTING\n')
 
         # broadcasting aggregations
-        out = list(db.table_select('*', 'select=count(1)', exclude_endswith = ['_audit', '_metadata']))
+        out = list(db.table_select('*', 'select=count(1)', exclude_endswith = [AUDIT_END, '_metadata']))
         assert out == [{'another_table': [5]}, {'test_table': [5]}]
 
         # fuzzy matching
-        out = list(db.table_select('another*', 'select=count(1)', exclude_endswith = ['_audit', '_metadata']))
+        out = list(db.table_select('another*', 'select=count(1)', exclude_endswith = [AUDIT_END, '_metadata']))
         assert out == [{'another_table': [5]}]
 
-        out = list(db.table_select('*_table', 'select=count(1)', exclude_endswith = ['_audit', '_metadata']))
+        out = list(db.table_select('*_table', 'select=count(1)', exclude_endswith = [AUDIT_END, '_metadata']))
         assert out == [{'another_table': [5]}, {'test_table': [5]}]
 
         # broadcasting queries without aggregation
-        out = list(db.table_select('*', 'select=x', exclude_endswith = ['_audit', '_metadata']))
+        out = list(db.table_select('*', 'select=x', exclude_endswith = [AUDIT_END, '_metadata']))
         assert out is not None
         assert len(out) == 2
         assert len(out[0].get("another_table")) == 5
         assert len(out[1].get("test_table")) == 5
 
-        out = list(db.table_select('*', 'select=x,y&where=z=not.is.null', exclude_endswith = ['_audit', '_metadata']))
+        out = list(db.table_select('*', 'select=x,y&where=z=not.is.null', exclude_endswith = [AUDIT_END, '_metadata']))
         assert out is not None
         assert len(out) == 2
         assert len(out[0].get("another_table")) == 4
         assert len(out[1].get("test_table")) == 4
 
         # table lists
         out = list(
             db.table_select(
                 'another_table,test_table',
                 'select=x,y&where=z=not.is.null',
-                exclude_endswith = ['_audit', '_metadata']
+                exclude_endswith = [AUDIT_END, '_metadata']
             )
         )
         assert out is not None
         assert len(out) == 2
         assert len(out[0].get("another_table")) == 4
         assert len(out[1].get("test_table")) == 4
 
@@ -794,17 +795,17 @@
         self.backend.table_insert(table_name=not_backup_table, data={"breathe-out": "short", "id": 1})
         self.backend.table_delete(table_name=not_backup_table, uri_query="")
 
         # now adjust the audit timestamps to fall outside the retention period
         target = (datetime.datetime.now() - timedelta(days=2)).isoformat()
         if isinstance(self.backend, SqliteBackend):
             new = json.dumps({"timestamp": target})
-            update_query = f"update {audit_table(not_backup_table)} set data = json_patch(data, '{new}')"
+            update_query = f"update {self.backend._fqtn(audit_table(not_backup_table))} set data = json_patch(data, '{new}')"
         elif isinstance(self.backend, PostgresBackend):
-            update_query = f"update {audit_table(not_backup_table)} set data = jsonb_set(data, '{{timestamp}}', '\"{target}\"')"
+            update_query = f"update {self.backend._fqtn(audit_table(not_backup_table))} set data = jsonb_set(data, '{{timestamp}}', '\"{target}\"')"
         with self.session_func(self.engine) as session:
             session.execute(update_query)
 
         # should not be able to view audit or restore data
         audit = list(self.backend.table_select(table_name=audit_table(not_backup_table), uri_query=""))
         self.assertEqual(len(audit), 0)
         result = self.backend.table_restore(
@@ -845,14 +846,15 @@
         audit = list(
             self.backend.table_select(
                 table_name=audit_table(verbose_table),
                 uri_query="",
             )
         )
         self.assertEqual(len(audit), 2)
+        self.backend.table_delete(table_name=verbose_table, uri_query="")
         self.backend.table_delete(table_name=audit_table(verbose_table), uri_query="")
 
     def test_all_view(self) -> bool:
         tenant1 = "p11"
         tenant2 = "p12"
         tenant3 = "p13"
         table_name = "A"
```

### Comparing `pysquril-0.7.0/PKG-INFO` & `pysquril-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysquril
-Version: 0.7.0
+Version: 1.0.0
 Summary: Python implementation of structured URI query language
 Home-page: https://github.com/unioslo/pysquril
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

