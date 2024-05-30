# Comparing `tmp/database_mysql_local-0.0.348.tar.gz` & `tmp/database_mysql_local-0.0.349.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.348.tar", last modified: Thu May 30 15:36:10 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.349.tar", last modified: Thu May 30 16:33:10 2024, max compression
```

## Comparing `database_mysql_local-0.0.348.tar` & `database_mysql_local-0.0.349.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.679641 database_mysql_local-0.0.348/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    58304 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   253151 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   668288 2024-05-30 15:35:35.000000 database_mysql_local-0.0.348/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 15:35:17.000000 database_mysql_local-0.0.348/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:33:10.070864 database_mysql_local-0.0.349/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 16:33:10.070864 database_mysql_local-0.0.349/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:33:10.062864 database_mysql_local-0.0.349/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:33:10.070864 database_mysql_local-0.0.349/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58241 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253151 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   668288 2024-05-30 16:32:36.000000 database_mysql_local-0.0.349/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:33:10.070864 database_mysql_local-0.0.349/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 16:33:10.000000 database_mysql_local-0.0.349/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 16:33:10.000000 database_mysql_local-0.0.349/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:33:10.000000 database_mysql_local-0.0.349/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 16:33:10.000000 database_mysql_local-0.0.349/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 16:33:10.000000 database_mysql_local-0.0.349/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 16:32:18.000000 database_mysql_local-0.0.349/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 16:33:10.070864 database_mysql_local-0.0.349/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 16:32:10.000000 database_mysql_local-0.0.349/setup.py
```

### Comparing `database_mysql_local-0.0.348/PKG-INFO` & `database_mysql_local-0.0.349/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.348
+Version: 0.0.349
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.348/README.md` & `database_mysql_local-0.0.349/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.349/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.349/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.349/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.349/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.349/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,28 +273,28 @@
 
     def __get_existing_duplicate_id_with_timestamp(
             self, schema_name: str, table_name: str, duplicate_column_name: str,
             duplicate_value: Any, column_name: str) -> int or None:
         select_query = (
             f"SELECT {column_name}, end_timestamp "
             f"FROM `{schema_name}`.`{table_name}` "
-            f"WHERE {duplicate_column_name} = %s AND end_timestamp IS NOT NULL LIMIT 1;"
+            f"WHERE {duplicate_column_name} = %s LIMIT 1;"
         )
         self.connection.commit()
         self.cursor.execute(select_query, (duplicate_value,))
         row = self.cursor.fetchone()
         if row is None:
             existing_duplicate_id = None
             return existing_duplicate_id
         else:
             existing_duplicate_id, end_timestamp = row
-        end_timestamp = end_timestamp.replace(tzinfo=timezone.utc)
-        if datetime.now(timezone.utc) > end_timestamp:
-            self.undelete_by_column_and_value(schema_name=schema_name, table_name=table_name, column_name=column_name,
-                                              column_value=existing_duplicate_id)
+        if end_timestamp and datetime.now(timezone.utc) > end_timestamp.replace(tzinfo=timezone.utc):
+            self.undelete_by_column_and_value(
+                schema_name=schema_name, table_name=table_name,
+                column_name=column_name, column_value=existing_duplicate_id)
         return existing_duplicate_id
 
     # TODO: test
     def __get_existing_duplicate_id_without_timestamp(
             self, *, schema_name: str, table_name: str, duplicate_column_name: str,
             duplicate_value: Any, column_name: str) -> int or None:
         select_query = (
```

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.349/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.349/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/point.py` & `database_mysql_local-0.0.349/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.349/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.349/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.349/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.349/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.349/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.349/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.349/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.348
+Version: 0.0.349
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.348/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.349/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/pyproject.toml` & `database_mysql_local-0.0.349/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.348/setup.py` & `database_mysql_local-0.0.349/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.348',
+    version='0.0.349',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

