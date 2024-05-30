# Comparing `tmp/mssql_dataframe-3.1.1.tar.gz` & `tmp/mssql_dataframe-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mssql_dataframe-3.1.1.tar", last modified: Mon Feb 12 20:28:36 2024, max compression
+gzip compressed data, was "mssql_dataframe-3.2.0.tar", last modified: Thu May 30 12:48:17 2024, max compression
```

## Comparing `mssql_dataframe-3.1.1.tar` & `mssql_dataframe-3.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 20:28:36.608158 mssql_dataframe-3.1.1/
--rw-rw-rw-   0        0        0     1086 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/LICENSE
--rw-rw-rw-   0        0        0       42 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6494 2024-02-12 20:28:36.608158 mssql_dataframe-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5812 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/README.md
--rw-rw-rw-   0        0        0        5 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/VERSION
-drwxrwxrwx   0        0        0        0 2024-02-12 20:28:36.592533 mssql_dataframe-3.1.1/mssql_dataframe/
--rw-rw-rw-   0        0        0      398 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/__equality__.py
--rw-rw-rw-   0        0        0      327 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/__init__.py
--rw-rw-rw-   0        0        0     3322 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/connect.py
-drwxrwxrwx   0        0        0        0 2024-02-12 20:28:36.592533 mssql_dataframe-3.1.1/mssql_dataframe/core/
--rw-rw-rw-   0        0        0       28 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/__init__.py
--rw-rw-rw-   0        0        0    35559 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/conversion.py
--rw-rw-rw-   0        0        0     5566 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/conversion_rules.py
--rw-rw-rw-   0        0        0     8254 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/create.py
--rw-rw-rw-   0        0        0     1620 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/custom_errors.py
--rw-rw-rw-   0        0        0     5937 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/dynamic.py
--rw-rw-rw-   0        0        0     8192 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/modify.py
--rw-rw-rw-   0        0        0     5760 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/read.py
-drwxrwxrwx   0        0        0        0 2024-02-12 20:28:36.608158 mssql_dataframe-3.1.1/mssql_dataframe/core/write/
--rw-rw-rw-   0        0        0       56 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/write/__init__.py
--rw-rw-rw-   0        0        0     1498 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/write/_exceptions.py
--rw-rw-rw-   0        0        0    10594 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/write/insert.py
--rw-rw-rw-   0        0        0    11001 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/write/merge.py
--rw-rw-rw-   0        0        0     6570 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/write/update.py
--rw-rw-rw-   0        0        0     1074 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/core/write/write.py
--rw-rw-rw-   0        0        0     4621 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/mssql_dataframe/package.py
-drwxrwxrwx   0        0        0        0 2024-02-12 20:28:36.608158 mssql_dataframe-3.1.1/mssql_dataframe.egg-info/
--rw-rw-rw-   0        0        0     6494 2024-02-12 20:28:36.000000 mssql_dataframe-3.1.1/mssql_dataframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      867 2024-02-12 20:28:36.000000 mssql_dataframe-3.1.1/mssql_dataframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-12 20:28:36.000000 mssql_dataframe-3.1.1/mssql_dataframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-02-12 20:28:36.000000 mssql_dataframe-3.1.1/mssql_dataframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-02-12 20:28:36.000000 mssql_dataframe-3.1.1/mssql_dataframe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      163 2024-02-12 20:25:31.000000 mssql_dataframe-3.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1006 2024-02-12 20:28:36.608158 mssql_dataframe-3.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 12:48:17.374648 mssql_dataframe-3.2.0/
+-rw-rw-rw-   0        0        0     1086 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6494 2024-05-30 12:48:17.374648 mssql_dataframe-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5812 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-30 12:48:17.374648 mssql_dataframe-3.2.0/mssql_dataframe/
+-rw-rw-rw-   0        0        0      398 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/__equality__.py
+-rw-rw-rw-   0        0        0      327 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/__init__.py
+-rw-rw-rw-   0        0        0     3322 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/connect.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:48:17.374648 mssql_dataframe-3.2.0/mssql_dataframe/core/
+-rw-rw-rw-   0        0        0       28 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/__init__.py
+-rw-rw-rw-   0        0        0    35778 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/conversion.py
+-rw-rw-rw-   0        0        0     5566 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/conversion_rules.py
+-rw-rw-rw-   0        0        0     8461 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/create.py
+-rw-rw-rw-   0        0        0     1620 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/custom_errors.py
+-rw-rw-rw-   0        0        0     5937 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/dynamic.py
+-rw-rw-rw-   0        0        0     8413 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/modify.py
+-rw-rw-rw-   0        0        0     5760 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/read.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:48:17.374648 mssql_dataframe-3.2.0/mssql_dataframe/core/write/
+-rw-rw-rw-   0        0        0       56 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/write/__init__.py
+-rw-rw-rw-   0        0        0     1498 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/write/_exceptions.py
+-rw-rw-rw-   0        0        0    10698 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/write/insert.py
+-rw-rw-rw-   0        0        0    11232 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/write/merge.py
+-rw-rw-rw-   0        0        0     6808 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/write/update.py
+-rw-rw-rw-   0        0        0     1074 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/core/write/write.py
+-rw-rw-rw-   0        0        0     4621 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/mssql_dataframe/package.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:48:17.374648 mssql_dataframe-3.2.0/mssql_dataframe.egg-info/
+-rw-rw-rw-   0        0        0     6494 2024-05-30 12:48:17.000000 mssql_dataframe-3.2.0/mssql_dataframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      867 2024-05-30 12:48:17.000000 mssql_dataframe-3.2.0/mssql_dataframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:48:17.000000 mssql_dataframe-3.2.0/mssql_dataframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-30 12:48:17.000000 mssql_dataframe-3.2.0/mssql_dataframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-30 12:48:17.000000 mssql_dataframe-3.2.0/mssql_dataframe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      163 2024-05-30 12:45:52.000000 mssql_dataframe-3.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1006 2024-05-30 12:48:17.374648 mssql_dataframe-3.2.0/setup.cfg
```

### Comparing `mssql_dataframe-3.1.1/LICENSE` & `mssql_dataframe-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/PKG-INFO` & `mssql_dataframe-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mssql_dataframe
-Version: 3.1.1
+Version: 3.2.0
 Summary: Update, Upsert, and Merge from Python dataframes to SQL Server and Azure SQL database.
 Home-page: https://github.com/jwcook23/mssql_dataframe
 Author: Jason Cook
 Author-email: jasoncook1989@gmail.com
 Project-URL: Bug Tracker, https://github.com/jwcook23/mssql_dataframe/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `mssql_dataframe-3.1.1/README.md` & `mssql_dataframe-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/connect.py` & `mssql_dataframe-3.2.0/mssql_dataframe/connect.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/conversion.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,28 @@
 
 # TODO: remove future opt-in
 pd.set_option("future.no_silent_downcasting", True)
 
 logger = logging.getLogger(__name__)
 
 
+def _get_schema_name(table_name):
+
+    # add cataglog for temporary tables
+    try:
+        schema_name, table_name = table_name.split(".")
+    except ValueError as err:
+        if err.args[0].startswith("not enough values to unpack"):
+            schema_name = "dbo"
+        else:  # pragma: no cover
+            raise
+
+    return schema_name, table_name
+
+
 def get_schema(
     connection: pyodbc.connect,
     table_name: str,
     dataframe: pd.DataFrame = None,
     additional_columns: List[str] = None,
 ) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Get schema of an SQL table and the defined conversion rules between data types.
@@ -43,22 +57,17 @@
     Returns
     -------
     schema (pandas.DataFrame) : table column specifications and conversion rules
     dataframe (pandas.DataFrame) : dataframe with contents converted to conform to SQL data type
     """
     cursor = connection.cursor()
 
+    schema_name, table_name = _get_schema_name(table_name)
+
     # add cataglog for temporary tables
-    try:
-        schema_name, table_name = table_name.split(".")
-    except ValueError as err:
-        if err.args[0].startswith("not enough values to unpack"):
-            schema_name = None
-        else:  # pragma: no cover
-            raise
     if table_name.startswith("#"):
         catalog = "tempdb"
     else:
         catalog = None
 
     # get schema
     schema = []
@@ -110,15 +119,17 @@
         "string"
     )
     schema["decimal_digits"] = schema["decimal_digits"].fillna(0).astype("int64")
     schema["is_nullable"] = schema["is_nullable"] == "YES"
     schema["ss_is_identity"] = schema["ss_is_identity"] == 1
 
     # add primary key info
-    pk = cursor.primaryKeys(table=table_name, catalog=catalog).fetchall()
+    pk = cursor.primaryKeys(
+        table=table_name, catalog=catalog, schema=schema_name
+    ).fetchall()
     pk = pd.DataFrame([list(x) for x in pk], columns=[x[0] for x in cursor.description])
     pk = pk.rename(columns={"key_seq": "pk_seq"})
     schema = schema.merge(
         pk[["column_name", "pk_seq", "pk_name"]],
         left_on="column_name",
         right_on="column_name",
         how="left",
```

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/conversion_rules.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/conversion_rules.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/create.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Methods for creating SQL tables both explicitly and implicitly."""
 
 from typing import List, Dict
 import logging
 
 import pyodbc
 
-from mssql_dataframe.core import dynamic
+from mssql_dataframe.core import dynamic, conversion
 
 logger = logging.getLogger(__name__)
 
 
 class create:
     """Class for creating SQL tables both explicitly and implicitly."""
 
@@ -60,15 +60,15 @@
         Table with an SQL identity primary key.
 
         >>> create.table(table_name='##ExampleCreateIdentityPKTable', columns={"A": "VARCHAR(100)", "B": "INT"}, not_nullable="B", sql_primary_key=True)
         """
         statement = """
         DECLARE @SQLStatement AS NVARCHAR(MAX);
         {declare}
-        SET @SQLStatement = N'CREATE TABLE {table} ('+
+        SET @SQLStatement = N'CREATE TABLE {schema}.{table} ('+
         {syntax}
         {pk}
         +');'
         EXEC sp_executesql
         @SQLStatement,
         N'{parameters}',
         {values};
@@ -81,14 +81,16 @@
             )
         if isinstance(not_nullable, str):
             not_nullable = [not_nullable]
         if isinstance(primary_key_column, str):
             primary_key_column = [primary_key_column]
 
         # parse inputs
+        schema_name, table_name = conversion._get_schema_name(table_name)
+        schema_name = dynamic.escape(self._connection.cursor(), schema_name)
         table_name = dynamic.escape(self._connection.cursor(), table_name)
         column_names = list(columns.keys())
         alias_names = [str(x) for x in list(range(0, len(column_names)))]
         size, dtypes_sql = dynamic.column_spec(columns.values())
         size_vars = [
             alias_names[idx] if x is not None else None for idx, x in enumerate(size)
         ]
@@ -192,14 +194,15 @@
         if primary_key_column is not None:
             values += ", " + ", ".join(
                 ["@PK_" + x + "" + "=@PK_" + x + "" for x in alias_pk]
             )
 
         # join components into final synax
         statement = statement.format(
+            schema=schema_name,
             table=table_name,
             declare=declare,
             syntax=syntax,
             pk=pk,
             parameters=parameters,
             values=values,
         )
```

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/custom_errors.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/custom_errors.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/dynamic.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/dynamic.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/modify.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/modify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Methods for modifying SQL columns or primary keys."""
 
 from typing import Literal, List
 import pyodbc
 
-from mssql_dataframe.core import dynamic
+from mssql_dataframe.core import dynamic, conversion
 
 
 class modify:
     """Class for modifying SQL columns or primary keys."""
 
     def __init__(self, connection: pyodbc.connect):
         """Class for modifying SQL table columns.
@@ -56,30 +56,33 @@
         >>> modify.column('##ExampleModifyTableColumn', modify='alter', column_name='B', data_type='tinyint', is_nullable=False)
 
         Drop a column.
         >>> modify.column('##ExampleModifyTableColumn', modify='drop', column_name='B')
         """
         statement = """
             DECLARE @SQLStatement AS NVARCHAR(MAX);
+            DECLARE @SchemaName SYSNAME = ?;
             DECLARE @TableName SYSNAME = ?;
             DECLARE @ColumnName SYSNAME = ?;
             {declare_type}
             {declare_size}
 
             SET @SQLStatement =
-                N'ALTER TABLE '+QUOTENAME(@TableName)+
+                N'ALTER TABLE '+QUOTENAME(@SchemaName)+'.'+QUOTENAME(@TableName)+
                 {syntax} +QUOTENAME(@ColumnName) {type_column} {size_column} {null_column}+';'
 
             EXEC sp_executesql
                 @SQLStatement,
-                N'@TableName SYSNAME, @ColumnName SYSNAME {parameter_type} {parameter_size}',
-                @TableName=@TableName, @ColumnName=@ColumnName {value_type} {value_size};
+                N'@SchemaName SYSNAME, @TableName SYSNAME, @ColumnName SYSNAME {parameter_type} {parameter_size}',
+                @SchemaName=@SchemaName, @TableName=@TableName, @ColumnName=@ColumnName {value_type} {value_size};
         """
 
-        args = [table_name, column_name]
+        schema_name, table_name = conversion._get_schema_name(table_name)
+
+        args = [schema_name, table_name, column_name]
         if modify == "drop":
             syntax = "'DROP COLUMN'"
             declare_type = ""
             declare_size = ""
             type_column = ""
             size_column = ""
             null_column = ""
```

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/read.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/read.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/write/_exceptions.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/write/_exceptions.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/write/insert.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/write/insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,17 @@
         if missing:
             raise custom_errors.DataframeColumnDoesNotExist(
                 "match_columns not found in dataframe", missing
             )
 
         # insert data into source temporary table
         uid = "".join(random.choices(string.ascii_lowercase, k=4))  # nosec B311
+
+        schema_name, table_name = conversion._get_schema_name(table_name)
+
         temp_name = f"##__source_{table_name}_{uid}"
         columns = list(dataframe.columns)
         if any(dataframe.index.names):
             columns = list(dataframe.index.names) + columns
 
         dtypes = self._column_spec(schema, columns)
 
@@ -261,8 +264,8 @@
         # reset match columns that were part of the primary key in the source table
         # dataframe needs returned in the event values were adjusted but indicies/columns should be the same
         names = schema.loc[dataframe.index.names, "pk_seq"]
         extra = names[names.isna()].index.tolist()
         if any(extra):
             dataframe = dataframe.reset_index(level=extra)
 
-        return schema, dataframe, match_columns, temp_name
+        return schema, dataframe, match_columns, temp_name, schema_name, table_name
```

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/write/merge.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/write/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,38 +96,41 @@
             include_metadata_timestamps = self.include_metadata_timestamps
 
         # get target table schema, while checking for errors and adjusting data for inserting
         if include_metadata_timestamps:
             additional_columns = ["_time_update", "_time_insert"]
         else:
             additional_columns = None
-        schema, dataframe, match_columns, temp_name = self._source_table(
-            table_name, dataframe, cursor, match_columns, additional_columns
+        schema, dataframe, match_columns, temp_name, schema_name, table_name = (
+            self._source_table(
+                table_name, dataframe, cursor, match_columns, additional_columns
+            )
         )
 
         # develop basic merge syntax
         statement = """
             DECLARE @SQLStatement AS NVARCHAR(MAX);
+            DECLARE @SchemaName SYSNAME = ?;
             DECLARE @TableName SYSNAME = ?;
             DECLARE @TableTemp SYSNAME = ?;
             {declare}
 
             SET @SQLStatement =
-            N' MERGE '+QUOTENAME(@TableName)+' AS _target '
-            +' USING '+QUOTENAME(@TableTemp)+' AS _source '
+            N' MERGE '+QUOTENAME(@SchemaName)+'.'+QUOTENAME(@TableName)+' AS _target '
+            +' USING '+QUOTENAME(@SchemaName)+'.'+QUOTENAME(@TableTemp)+' AS _source '
             +' ON ('+{match_syntax}+') '
             +' WHEN MATCHED THEN UPDATE SET '+{update_syntax}
             +' WHEN NOT MATCHED THEN INSERT ('+{insert_syntax}+')'
             +' VALUES ('+{insert_values}+')'
             +{delete_syntax}+';'
 
             EXEC sp_executesql
                 @SQLStatement,
-                N'@TableName SYSNAME, @TableTemp SYSNAME, {parameters}',
-                @TableName=@TableName, @TableTemp=@TableTemp, {values};
+                N'@SchemaName SYSNAME, @TableName SYSNAME, @TableTemp SYSNAME, {parameters}',
+                @SchemaName=@SchemaName, @TableName=@TableName, @TableTemp=@TableTemp, {values};
         """
 
         # if matched, update all columns in dataframe besides match_columns
         update_columns = list(dataframe.columns[~dataframe.columns.isin(match_columns)])
 
         # if not matched, insert all columns in dataframe
         if any(dataframe.index.names):
@@ -218,22 +221,22 @@
             parameters=parameters,
             values=values,
         )
 
         # perform merge
         if delete_requires is None:
             args = (
-                [table_name, temp_name]
+                [schema_name, table_name, temp_name]
                 + match_columns
                 + update_columns
                 + insert_columns
             )
         else:
             args = (
-                [table_name, temp_name]
+                [schema_name, table_name, temp_name]
                 + match_columns
                 + update_columns
                 + insert_columns
                 + delete_requires
             )
 
         # execute statement to perform update in target table using source
```

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/write/update.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/write/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,44 +72,47 @@
             include_metadata_timestamps = self.include_metadata_timestamps
 
         # get target table schema, while checking for errors and adjusting data for inserting
         if include_metadata_timestamps:
             additional_columns = ["_time_update"]
         else:
             additional_columns = None
-        schema, dataframe, match_columns, temp_name = self._source_table(
-            table_name,
-            dataframe,
-            cursor,
-            match_columns,
-            additional_columns,
-            updating_table=True,
+        schema, dataframe, match_columns, temp_name, schema_name, table_name = (
+            self._source_table(
+                table_name,
+                dataframe,
+                cursor,
+                match_columns,
+                additional_columns,
+                updating_table=True,
+            )
         )
 
         # develop basic update syntax
         statement = """
             DECLARE @SQLStatement AS NVARCHAR(MAX);
+            DECLARE @SchemaName SYSNAME = ?;
             DECLARE @TableName SYSNAME = ?;
             DECLARE @TableTemp SYSNAME = ?;
             {declare}
 
             SET @SQLStatement =
                 N'UPDATE '+
-                    QUOTENAME(@TableName)+
+                    QUOTENAME(@SchemaName)+'.'+QUOTENAME(@TableName)+
                 ' SET '+
                     {update_syntax}+
                 ' FROM '+
-                    QUOTENAME(@TableName)+' AS _target '+
+                    QUOTENAME(@SchemaName)+'.'+QUOTENAME(@TableName)+' AS _target '+
                 ' INNER JOIN '+
                     QUOTENAME(@TableTemp)+' AS _source '+
                     'ON '+{match_syntax}+';'
             EXEC sp_executesql
                 @SQLStatement,
-                N'@TableName SYSNAME, @TableTemp SYSNAME, {parameters}',
-                @TableName=@TableName, @TableTemp=@TableTemp, {values};
+                N'@SchemaName SYSNAME, @TableName SYSNAME, @TableTemp SYSNAME, {parameters}',
+                @SchemaName=@SchemaName, @TableName=@TableName, @TableTemp=@TableTemp, {values};
         """
 
         # update all columns in dataframe besides match columns
         update_columns = list(dataframe.columns[~dataframe.columns.isin(match_columns)])
 
         # alias columns to prevent direct input into SQL string
         alias_match = [str(x) for x in list(range(0, len(match_columns)))]
@@ -148,15 +151,15 @@
             match_syntax=match_syntax,
             update_syntax=update_syntax,
             parameters=parameters,
             values=values,
         )
 
         # perform update
-        args = [table_name, temp_name] + match_columns + update_columns
+        args = [schema_name, table_name, temp_name] + match_columns + update_columns
 
         # execute statement to perform update in target table using source
         cursor.execute(statement, args)
         temp_name = dynamic.escape(cursor, temp_name)
         cursor.execute("DROP TABLE " + temp_name)
         cursor.commit()
```

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/core/write/write.py` & `mssql_dataframe-3.2.0/mssql_dataframe/core/write/write.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe/package.py` & `mssql_dataframe-3.2.0/mssql_dataframe/package.py`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe.egg-info/PKG-INFO` & `mssql_dataframe-3.2.0/mssql_dataframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mssql_dataframe
-Version: 3.1.1
+Version: 3.2.0
 Summary: Update, Upsert, and Merge from Python dataframes to SQL Server and Azure SQL database.
 Home-page: https://github.com/jwcook23/mssql_dataframe
 Author: Jason Cook
 Author-email: jasoncook1989@gmail.com
 Project-URL: Bug Tracker, https://github.com/jwcook23/mssql_dataframe/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `mssql_dataframe-3.1.1/mssql_dataframe.egg-info/SOURCES.txt` & `mssql_dataframe-3.2.0/mssql_dataframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mssql_dataframe-3.1.1/setup.cfg` & `mssql_dataframe-3.2.0/setup.cfg`

 * *Files identical despite different names*

