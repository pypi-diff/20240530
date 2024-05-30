# Comparing `tmp/database_mysql_local-0.0.347.tar.gz` & `tmp/database_mysql_local-0.0.348.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.347.tar", last modified: Thu May 30 15:07:50 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.348.tar", last modified: Thu May 30 15:36:10 2024, max compression
```

## Comparing `database_mysql_local-0.0.347.tar` & `database_mysql_local-0.0.348.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.442032 database_mysql_local-0.0.347/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    59334 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   253151 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   668288 2024-05-30 15:07:14.000000 database_mysql_local-0.0.347/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:07:50.000000 database_mysql_local-0.0.347/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 15:06:56.000000 database_mysql_local-0.0.347/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:07:50.446032 database_mysql_local-0.0.347/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 15:06:47.000000 database_mysql_local-0.0.347/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.679641 database_mysql_local-0.0.348/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58304 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   253151 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   668288 2024-05-30 15:35:35.000000 database_mysql_local-0.0.348/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:36:10.000000 database_mysql_local-0.0.348/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 15:35:17.000000 database_mysql_local-0.0.348/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:36:10.687641 database_mysql_local-0.0.348/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 15:35:09.000000 database_mysql_local-0.0.348/setup.py
```

### Comparing `database_mysql_local-0.0.347/PKG-INFO` & `database_mysql_local-0.0.348/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.347
+Version: 0.0.348
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.347/README.md` & `database_mysql_local-0.0.348/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.348/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.348/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.348/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.348/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.348/database_mysql_local/src/generic_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .cursor import Cursor
 from .table_definition import table_definition
 from .utils import (detect_if_is_test_data, generate_column_name,
-                    generate_table_name, generate_view_name,
+                    generate_table_name, generate_view_name, extract_duplicated_from_error,
                     get_entity_type_by_table_name, get_where_params,
                     process_insert_data_dict, process_update_data_dict, process_upsert_data_dict,
                     replace_view_with_table, validate_none_select_table_name,
                     validate_select_table_name, validate_single_clause_value,
                     where_skip_null_values, insert_is_undelete, is_column_in_table,
                     is_end_timestamp_in_table, get_table_columns, group_list_by_columns)
 
@@ -241,38 +241,18 @@
             table_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict,
                                    ignore_duplicate=True)
 
         self.logger.debug(object=locals())
         return table_id
 
     def _get_existing_duplicate_id(self, schema_name: str, table_name: str, error: Exception) -> int or None:
-        """Error examples:
-        - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'
-        - Duplicate entry '7263200721327371865' for key 'test_mysql_table.number_UNIQUE
-        - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
-        - 1062 (23000): Duplicate entry 'tal@circlez.ai' for key 'person_table.person_table.main_email_person.unique'
-        - 1062 (23000): Duplicate entry '1-2' for key 'test_location_profile_table.idx_location_id_profile_id'
-        """
         # When inserting a deleted entity and insert_is_undelete=false, we should null all the unique fields of the deleted entity
-
-        pattern = r'Duplicate entry \'(.+?)\' for key \'(.+?)\''
-        match = re.search(pattern, str(error))
-        if not match:  # a different error
-            raise error
-        duplicate_value = match.group(1)
-        key = match.group(2)
-        if key.endswith("PRIMARY"):
-            return int(duplicate_value)
-        elif key.endswith("_UNIQUE"):
-            duplicate_column_name = key.split(".")[-1].split('_')[0]
-        elif key.count(".") > 1:
-            duplicate_column_name = key.split(".")[-2]
-        else:
-            raise Exception(f"GenericCRUD._get_existing_duplicate_id: please report the following error,"
-                            f" so we can add support to this case: insert error: {error}")
+        duplicate_value, duplicate_column_name = extract_duplicated_from_error(error)
+        if not duplicate_column_name:
+            return duplicate_value  # found the duplicated id
 
         column_name = self.get_primary_key(schema_name=schema_name, table_name=table_name)
         if not column_name:
             raise error  # Column name for constraint not found
         if is_end_timestamp_in_table(table_name=table_name) and insert_is_undelete(table_name=table_name):
             existing_duplicate_id = self.__get_existing_duplicate_id_with_timestamp(
                 schema_name=schema_name, table_name=table_name, duplicate_column_name=duplicate_column_name,
```

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.348/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.348/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/point.py` & `database_mysql_local-0.0.348/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.348/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.348/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.348/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.348/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.348/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.348/database_mysql_local/src/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import copy
 import inspect
 import os
+import re
 from functools import lru_cache
 from typing import Any, Optional
 
 from python_sdk_remote.utilities import get_environment_name
 from url_remote.environment_name_enum import EnvironmentName
 
 from .table_columns import table_columns
@@ -228,14 +229,41 @@
         if key not in grouped:
             grouped[key] = []
         for col in group_by:
             dict_row.pop(col)
         grouped[key].append(dict_row)
     return grouped
 
+def extract_duplicated_from_error(error: Exception) -> (Any, str):
+    """Error examples:
+    - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'  - in such case return the duplicated value, otherwise the column
+    - Duplicate entry '7263200721327371865' for key 'test_mysql_table.number_UNIQUE
+    - IntegrityError(1062, "1062 (23000): Duplicate entry '202-405-3018' for key 'person_table.person.main_full_number_normalized_UNIQUE'", '23000')
+    - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
+    - 1062 (23000): Duplicate entry 'tal@circlez.ai' for key 'person_table.person_table.main_email_person.unique'
+    - TODO (index can have any name): 1062 (23000): Duplicate entry '1-2' for key 'test_location_profile_table.idx_location_id_profile_id'
+    """
+    pattern = r'Duplicate entry \'(.+?)\' for key \'(.+?)\''
+    match = re.search(pattern, str(error))
+    if not match:  # a different error
+        raise error
+    duplicate_value = match.group(1)
+    key = match.group(2)
+    if key.endswith("PRIMARY"):
+        return int(duplicate_value), ""
+    elif key.endswith("_UNIQUE"):
+        # all but last
+        duplicate_column_name = "_".join(key.split(".")[-1].split('_')[:-1])
+    elif key.count(".") > 1:
+        duplicate_column_name = key.split(".")[-2]
+    else:
+        raise Exception(f"GenericCRUD._get_existing_duplicate_id: please report the following error,"
+                        f" so we can add support to this case: insert error: {error}")
+    return duplicate_value, duplicate_column_name
+
 # def get_table_columns(schema_name: str = None, table_name: str = None) -> tuple:
 #     select_query = "SELECT column_name " \
 #                    "FROM information_schema.columns " \
 #                    "WHERE TABLE_SCHEMA = %s " \
 #                    "AND TABLE_NAME = %s;"
 #     params = (schema_name, table_name)
 #
```

### Comparing `database_mysql_local-0.0.347/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.348/database_mysql_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.347
+Version: 0.0.348
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.347/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.348/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/pyproject.toml` & `database_mysql_local-0.0.348/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.347/setup.py` & `database_mysql_local-0.0.348/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.347',
+    version='0.0.348',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

