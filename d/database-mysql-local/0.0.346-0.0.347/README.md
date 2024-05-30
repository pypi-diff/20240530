# Comparing `tmp/database_mysql_local-0.0.346.tar.gz` & `tmp/database_mysql_local-0.0.347.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.346.tar", last modified: Thu May 30 08:04:57 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.347.tar", last modified: Thu May 30 15:07:50 2024, max compression
```

## Comparing `database_mysql_local-0.0.346.tar` & `database_mysql_local-0.0.347.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:57.437696 database_mysql_local-0.0.346/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 08:04:57.437696 database_mysql_local-0.0.346/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:57.433696 database_mysql_local-0.0.346/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:57.437696 database_mysql_local-0.0.346/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    58562 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31606 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   252237 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   668288 2024-05-30 08:04:25.000000 database_mysql_local-0.0.346/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:04:57.437696 database_mysql_local-0.0.346/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 08:04:57.000000 database_mysql_local-0.0.346/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 08:04:57.000000 database_mysql_local-0.0.346/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:04:57.000000 database_mysql_local-0.0.346/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 08:04:57.000000 database_mysql_local-0.0.346/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 08:04:57.000000 database_mysql_local-0.0.346/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 08:04:10.000000 database_mysql_local-0.0.346/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:04:57.437696 database_mysql_local-0.0.346/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 08:04:02.000000 database_mysql_local-0.0.346/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.442032 database_mysql_local-0.0.347/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59334 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253151 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   668288 2024-05-30 15:07:14.000000 database_mysql_local-0.0.347/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 15:06:56.000000 database_mysql_local-0.0.347/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/setup.py
```

### Comparing `database_mysql_local-0.0.346/PKG-INFO` & `database_mysql_local-0.0.347/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.346
+Version: 0.0.347
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.346/README.md` & `database_mysql_local-0.0.347/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.347/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.347/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.347/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.347/database_mysql_local/src/generate_table_columns.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os
 
 from database_mysql_local.connector import Connector
 
 # TODO improve Sql2Code. We prefer only Sql2Code to generate those structures.
 
 connection = Connector.connect(schema_name="test")
 try:
```

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.347/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .table_definition import table_definition
 from .utils import (detect_if_is_test_data, generate_column_name,
                     generate_table_name, generate_view_name,
                     get_entity_type_by_table_name, get_where_params,
                     process_insert_data_dict, process_update_data_dict, process_upsert_data_dict,
                     replace_view_with_table, validate_none_select_table_name,
                     validate_select_table_name, validate_single_clause_value,
-                    where_skip_null_values, insert_is_undelete,
+                    where_skip_null_values, insert_is_undelete, is_column_in_table,
                     is_end_timestamp_in_table, get_table_columns, group_list_by_columns)
 
 printed_dep_warning = []
 
 
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
@@ -323,16 +323,16 @@
             f"WHERE {duplicate_column_name} = %s LIMIT 1;"
         )
         self.connection.commit()
         self.cursor.execute(select_query, (duplicate_value,))
         existing_duplicate_id = (self.cursor.fetchone() or [None])[0]
         return existing_duplicate_id
 
-    def undelete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None, column_name: str = None,
-                                     column_value: Any = None) -> None:
+    def undelete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
+                                     column_name: str = None, column_value: Any = None) -> None:
         """Undeletes a row by setting the end_timestamp to NULL."""
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
         self._validate_args(args=locals())
         self.update_by_column_and_value(
             schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=column_value,
@@ -473,19 +473,26 @@
         where = self.__where_security(where=where, view_name=view_table_name)
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
 
         if self.is_test_data:
+            # TODO: auto detect with entity table (save in memory first)
+            # once done, we prefer not to send it as parameter, to allow changing the name later without changing the code.
+            # In the future we will change to default_view_with_test_data that does not show deleted data, so that
+            # we can select-delete-select in a similar way and verify the deletion.
+            # Will we ever have a case where there will be a view with no assosiated table that we will need to see deleted data in there? It appears no.
             if self.default_view_with_deleted_and_test_data:
                 view_table_name = self.default_view_with_deleted_and_test_data
             else:
                 view_table_name = replace_view_with_table(view_table_name=view_table_name,
                                                           select_clause_value=select_clause_value)
+        elif is_column_in_table(table_name=view_table_name, column_name="is_test_data") and "is_test_data" not in where:
+            where += " AND is_test_data <> 1"  # hide test data from real users.
 
         if where and "end_timestamp" not in where and is_end_timestamp_in_table(view_table_name):
             where += " AND end_timestamp IS NULL "  # not deleted
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
```

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.347/database_mysql_local/src/generic_crud_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from .table_definition import table_definition
 from .utils import generate_column_name, generate_view_name, is_column_in_table
 
 IS_MAIN_COLUMN_NAME = "is_main"
 
 
 # TODO If I understand, there are two things:
-# is_main in data_ml_dict
-# table_definition_table.is_main_column
-# I'm not sure we need additional parameter.
+#   - is_main in data_ml_dict
+#   - table_definition_table.is_main_column
+#   I'm not sure we need additional parameter.
 class GenericCRUDML(GenericCRUD, metaclass=MetaLogger, object=LOGGER_CRUD_ML_CODE_OBJECT):
     """A class that provides generic CRUD functionality for tables with multi-language support."""
 
     # TODO: allow overiding all default values in all methods
     # TODO Shall we add same_entity method as parameter?
     def __init__(self, default_schema_name: str,
                  default_table_name: str = None, default_view_table_name: str = None,
@@ -61,14 +61,15 @@
         if ids:
             result = f" IN ({','.join([str(_id[f'{entity_name}_id']) for _id in ids])})"
         else:
             result = " = TRUE"
 
         return result
 
+    # TODO: should we rename all those methode similar to CRUD? (select, etc.)
     def add_value(self, *, schema_name: str = None, data_dict: dict = None, data_ml_dict: dict = None,
                   data_json: dict = None, data_ml_json: dict = None, column_name: str = None,
                   table_id: int = None, lang_code: LangCode = None,
                   is_main: bool or None = False, table_name: str = None,
                   ml_table_name: str = None) -> Optional[tuple]:
         schema_name = schema_name or self.default_schema_name
         data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
```

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.347/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/point.py` & `database_mysql_local-0.0.347/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.347/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.347/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.347/database_mysql_local/src/table_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,37 @@
 table_columns = {
+    "action_general_view": (
+        "action_id",
+        "name",
+        "description",
+        "is_queue_action",
+        "is_smartlink_action",
+        "package_name",
+        "function_name",
+        "function_module",
+        "folder_name",
+        "filename",
+        "source_system_id",
+        "destination_system_id",
+        "destination_subsystem_id",
+        "expiration_unit",
+        "expiration_value",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "action_stars"
+    ),
     "action_table": (
         "action_id",
         "name",
         "description",
         "is_queue_action",
         "is_smartlink_action",
         "package_name",
@@ -6795,40 +6824,15 @@
         "organization_ml_id",
         "number",
         "identifier",
         "organization_id",
         "lang_code",
         "is_main",
         "title",
-        "is_name_approved",
-        "description",
-        "is_description_approved",
-        "is_test_data",
-        "start_timestamp",
-        "end_timestamp",
-        "created_timestamp",
-        "created_user_id",
-        "created_real_user_id",
-        "created_effective_user_id",
-        "created_effective_profile_id",
-        "updated_timestamp",
-        "updated_user_id",
-        "updated_real_user_id",
-        "updated_effective_user_id",
-        "updated_effective_profile_id"
-    ),
-    "organization_ml_view": (
-        "organization_ml_id",
-        "number",
-        "identifier",
-        "organization_id",
-        "lang_code",
-        "is_main",
-        "title",
-        "is_name_approved",
+        "is_title_approved",
         "description",
         "is_description_approved",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
@@ -8588,14 +8592,34 @@
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id"
     ),
+    "reaction_type_ml_general_view": (
+        "reaction_id",
+        "name",
+        "number",
+        "value",
+        "text",
+        "image",
+        "reaction_type_id",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "lang_code",
+        "title",
+        "reaction_type_ml.is_test_data",
+        "reaction_type_ml.end_timestamp"
+    ),
     "reaction_type_ml_table": (
         "reaction_type_ml_id",
         "reaction_type_id",
         "lang_code",
         "title",
         "description",
         "start_timestamp",
@@ -8608,19 +8632,31 @@
     ),
     "reaction_type_ml_view": (
         "reaction_type_id",
         "name",
         "lang_code",
         "title"
     ),
+    "reaction_type_ml_with_deleted_and_test_data_view": (
+        "reaction_type_id",
+        "name",
+        "is_test_data",
+        "end_timestamp",
+        "lang_code",
+        "title",
+        "reaction_type_ml.is_test_data",
+        "reaction_type_ml.end_timestamp"
+    ),
     "reaction_type_table": (
         "reaction_type_id",
-        "name"
+        "name",
+        "is_test_data",
+        "end_timestamp"
     ),
-    "reaction_view": (
+    "reaction_type_view": (
         "reaction_id",
         "name",
         "number",
         "value",
         "text",
         "image",
         "reaction_type_id",
```

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.347/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.347/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.347/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.347/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.346
+Version: 0.0.347
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.346/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.347/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/pyproject.toml` & `database_mysql_local-0.0.347/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.346/setup.py` & `database_mysql_local-0.0.347/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.346',
+    version='0.0.347',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

