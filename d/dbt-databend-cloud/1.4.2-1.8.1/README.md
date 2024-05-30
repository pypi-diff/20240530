# Comparing `tmp/dbt_databend_cloud-1.4.2-py3-none-any.whl.zip` & `tmp/dbt_databend_cloud-1.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 22821 bytes, number of entries: 25
+Zip file size: 22736 bytes, number of entries: 25
 -rw-r--r--  2.0 unx      545 b- defN 23-Feb-12 13:44 dbt/adapters/databend/__init__.py
--rw-r--r--  2.0 unx       18 b- defN 23-Jul-27 03:22 dbt/adapters/databend/__version__.py
--rw-r--r--  2.0 unx     1607 b- defN 23-Feb-12 13:44 dbt/adapters/databend/column.py
--rw-r--r--  2.0 unx     7531 b- defN 23-Jul-27 03:22 dbt/adapters/databend/connections.py
--rw-r--r--  2.0 unx    11224 b- defN 23-Jul-27 03:22 dbt/adapters/databend/impl.py
--rw-r--r--  2.0 unx     2885 b- defN 23-Jul-27 03:22 dbt/adapters/databend/relation.py
+-rw-r--r--  2.0 unx       18 b- defN 24-May-30 09:17 dbt/adapters/databend/__version__.py
+-rw-r--r--  2.0 unx     1787 b- defN 24-May-30 09:17 dbt/adapters/databend/column.py
+-rw-r--r--  2.0 unx     8081 b- defN 24-May-30 09:17 dbt/adapters/databend/connections.py
+-rw-r--r--  2.0 unx     9979 b- defN 24-May-30 09:17 dbt/adapters/databend/impl.py
+-rw-r--r--  2.0 unx     2929 b- defN 24-May-30 09:17 dbt/adapters/databend/relation.py
 -rw-r--r--  2.0 unx       52 b- defN 23-Feb-12 13:44 dbt/include/databend/__init__.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Jul-27 03:22 dbt/include/databend/dbt_project.yml
 -rw-r--r--  2.0 unx      185 b- defN 23-Jul-18 07:59 dbt/include/databend/profile_template.yml
--rw-r--r--  2.0 unx     5771 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/adapters.sql
+-rw-r--r--  2.0 unx     5808 b- defN 24-May-30 09:17 dbt/include/databend/macros/adapters.sql
 -rw-r--r--  2.0 unx      796 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/catalog.sql
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/incremental.sql
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/snapshot.sql
 -rw-r--r--  2.0 unx      285 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/utils.sql
 -rw-r--r--  2.0 unx     1095 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/adapters/apply_grants.sql
--rw-r--r--  2.0 unx      826 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/adapters/relation.sql
+-rw-r--r--  2.0 unx      734 b- defN 24-May-30 09:17 dbt/include/databend/macros/adapters/relation.sql
 -rw-r--r--  2.0 unx     6216 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/materializations/incremental.sql
 -rw-r--r--  2.0 unx     1111 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/materializations/seed.sql
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/materializations/snapshot.sql
--rw-r--r--  2.0 unx     2987 b- defN 23-Jul-27 03:22 dbt/include/databend/macros/materializations/table.sql
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      907 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2393 b- defN 23-Jul-27 03:25 dbt_databend_cloud-1.4.2.dist-info/RECORD
-25 files, 57964 bytes uncompressed, 18807 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-21 09:06 dbt/include/databend/macros/materializations/snapshot.sql
+-rw-r--r--  2.0 unx     2999 b- defN 24-May-30 09:17 dbt/include/databend/macros/materializations/table.sql
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-30 09:26 dbt_databend_cloud-1.8.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      918 b- defN 24-May-30 09:26 dbt_databend_cloud-1.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 09:26 dbt_databend_cloud-1.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-May-30 09:26 dbt_databend_cloud-1.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2392 b- defN 24-May-30 09:26 dbt_databend_cloud-1.8.1.dist-info/RECORD
+25 files, 57460 bytes uncompressed, 18722 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: dbt/include/databend/macros/materializations/snapshot.sql
 Comment: 
 
 Filename: dbt/include/databend/macros/materializations/table.sql
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.2.dist-info/LICENSE
+Filename: dbt_databend_cloud-1.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.2.dist-info/METADATA
+Filename: dbt_databend_cloud-1.8.1.dist-info/METADATA
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.2.dist-info/WHEEL
+Filename: dbt_databend_cloud-1.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.2.dist-info/top_level.txt
+Filename: dbt_databend_cloud-1.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dbt_databend_cloud-1.4.2.dist-info/RECORD
+Filename: dbt_databend_cloud-1.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dbt/adapters/databend/__version__.py

```diff
@@ -1 +1 @@
-version = "1.4.2"
+version = "1.8.1"
```

## dbt/adapters/databend/column.py

```diff
@@ -1,44 +1,50 @@
 from dataclasses import dataclass
 from typing import TypeVar, Optional, Dict, Any
 
-import dbt.exceptions
 from dbt.adapters.base.column import Column
+from dbt_common.exceptions import DbtRuntimeError
 
 Self = TypeVar("Self", bound="DatabendColumn")
 
 
 @dataclass
 class DatabendColumn(Column):
     @property
     def quoted(self) -> str:
         return '"{}"'.format(self.column)
 
     def is_string(self) -> bool:
+        if self.dtype is None:
+            return False
         return self.dtype.lower() in [
             "string",
             "varchar",
         ]
 
     def is_integer(self) -> bool:
+        if self.dtype is None:
+            return False
         return self.dtype.lower().startswith("int") or self.dtype.lower() in (
             "tinyint",
             "smallint",
             "bigint",
         )
 
     def is_numeric(self) -> bool:
         return False
 
     def is_float(self) -> bool:
+        if self.dtype is None:
+            return False
         return self.dtype.lower() in ("float", "double")
 
     def string_size(self) -> int:
         if not self.is_string():
-            raise dbt.exceptions.RuntimeException(
+            raise DbtRuntimeError(
                 "Called string_size() on non-string field!"
             )
 
         if self.char_size is None:
             return 256
         else:
             return int(self.char_size)
```

## dbt/adapters/databend/connections.py

```diff
@@ -1,22 +1,29 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 
 import agate
-import dbt.exceptions  # noqa
-from dbt.adapters.base import Credentials
+import dbt_common.exceptions  # noqa
 
+from dbt.adapters.exceptions.connection import FailedToConnectError
+from dbt.adapters.contracts.connection import AdapterResponse, Connection, Credentials
+from dbt_common.clients.agate_helper import empty_table
 from dbt.adapters.sql import SQLConnectionManager as connection_cls
-from dbt.contracts.connection import AdapterResponse
-from dbt.events import AdapterLogger
+from dbt.adapters.events.logging import AdapterLogger  # type: ignore
+from dbt_common.events.functions import warn_or_error
+from dbt.adapters.events.types import AdapterEventWarning
+from dbt_common.ui import line_wrap_message, warning_tag
+from dbt_common.clients.agate_helper import empty_table
 from typing import Optional, Tuple, List, Any
 from databend_sqlalchemy import connector
 
-from dbt.exceptions import (
-    Exception,
+from dbt_common.exceptions import (
+    DbtInternalError,
+    DbtRuntimeError,
+    DbtConfigError,
 )
 
 logger = AdapterLogger("databend")
 
 
 @dataclass
 class DatabendAdapterResponse(AdapterResponse):
@@ -58,15 +65,15 @@
             data["database"] = None
         return data
 
     def __post_init__(self):
         # databend classifies database and schema as the same thing
         self.database = None
         if self.database is not None and self.database != self.schema:
-            raise dbt.exceptions.Exception(
+            raise DbtRuntimeError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
                 f"On Databend, database must be omitted or have the same value as"
                 f" schema."
             )
 
     @property
@@ -85,14 +92,19 @@
     def _connection_keys(self):
         """
         List of keys to display in the `dbt debug` output.
         """
         return ("host", "port", "database", "schema", "user")
 
 
+@dataclass
+class DatabendAdapterResponse(AdapterResponse):
+    query_id: str = ""
+
+
 class DatabendConnectionManager(connection_cls):
     TYPE = "databend"
 
     @contextmanager
     def exception_handler(self, sql: str):
         """
         Returns a context manager, that will handle exceptions raised
@@ -101,15 +113,15 @@
         try:
             yield
 
         except Exception as e:
             logger.debug("Error running SQL: {}".format(sql))
             logger.debug("Rolling back transaction.")
             self.rollback_if_open()
-            raise dbt.exceptions.Exception(str(e))
+            raise DbtRuntimeError(str(e))
 
     # except for DML statements where explicitly defined
     def add_begin_query(self, *args, **kwargs):
         pass
 
     def add_commit_query(self, *args, **kwargs):
         pass
@@ -132,20 +144,14 @@
         if connection.state == "open":
             logger.debug("Connection is already open, skipping open.")
             return connection
 
         credentials = connection.credentials
 
         try:
-            # handle = mysql.connector.connect(
-            #     # host=credentials.host,
-            #     # port=credentials.port,
-            #     # user=credentials.username,
-            #     # password=credentials.password,
-            # )
             if credentials.secure is None:
                 credentials.secure = True
 
             if credentials.secure:
                 handle = connector.connect(
                     f"https://{credentials.username}:{credentials.password}@{credentials.host}:{credentials.port}/{credentials.schema}?secure=true "
                 )
@@ -154,35 +160,38 @@
                     f"http://{credentials.username}:{credentials.password}@{credentials.host}:{credentials.port}/{credentials.schema}?secure=false "
                 )
 
         except Exception as e:
             logger.debug("Error opening connection: {}".format(e))
             connection.handle = None
             connection.state = "fail"
-            raise dbt.exceptions.FailedToConnectException(str(e))
+            raise FailedToConnectError(str(e))
         connection.state = "open"
         connection.handle = handle
         return connection
 
     @classmethod
-    def get_response(cls, _):
-        return "OK"
+    def get_response(cls, cursor):
+        return DatabendAdapterResponse(
+            _message="{} {}".format("adapter response", cursor.rowcount),
+            rows_affected=cursor.rowcount,
+        )
 
     def execute(
-            self, sql: str, auto_begin: bool = False, fetch: bool = False
+            self, sql: str, auto_begin: bool = False, fetch: bool = False, limit: Optional[int] = None
     ) -> Tuple[AdapterResponse, agate.Table]:
         # don't apply the query comment here
         # it will be applied after ';' queries are split
         _, cursor = self.add_query(sql, auto_begin)
         response = self.get_response(cursor)
         # table: rows, column_names=None, column_types=None, row_names=None
         if fetch:
-            table = self.get_result_from_cursor(cursor)
+            table = self.get_result_from_cursor(cursor, limit)
         else:
-            table = dbt.clients.agate_helper.empty_table()
+            table = dbt_common.clients.agate_helper.empty_table()
         return response, table
 
     def add_query(self, sql, auto_begin=False, bindings=None, abridge_sql_log=False):
         connection, cursor = super().add_query(
             sql, auto_begin, bindings=bindings, abridge_sql_log=abridge_sql_log
         )
 
@@ -227,17 +236,20 @@
 
     @classmethod
     def process_results(cls, column_names, rows):
 
         return [dict(zip(column_names, row)) for row in rows]
 
     @classmethod
-    def get_result_from_cursor(cls, cursor: Any) -> agate.Table:
+    def get_result_from_cursor(cls, cursor: Any, limit: Optional[int]) -> agate.Table:
         data: List[Any] = []
         column_names: List[str] = []
 
         if cursor.description is not None:
             column_names = [col[0] for col in cursor.description]
-            rows = cursor.fetchall()
+            if limit:
+                rows = cursor.fetchmany(limit)
+            else:
+                rows = cursor.fetchall()
             data = cls.process_results(column_names, rows)
 
-        return dbt.clients.agate_helper.table_from_data_flat(data, column_names)
+        return dbt_common.clients.agate_helper.table_from_data_flat(data, column_names)
```

## dbt/adapters/databend/impl.py

```diff
@@ -1,22 +1,24 @@
 from concurrent.futures import Future
 from dataclasses import dataclass
-from typing import Callable, List, Optional, Set, Union
+from typing import Callable, List, Optional, Set, Union, FrozenSet, Tuple
 
 import agate
-import dbt.exceptions
 from dbt.adapters.base import AdapterConfig, available
 from dbt.adapters.base.impl import catch_as_completed
 from dbt.adapters.base.relation import InformationSchema
 from dbt.adapters.sql import SQLAdapter
-from dbt.clients.agate_helper import table_from_rows
-from dbt.contracts.graph.manifest import Manifest
-from dbt.contracts.relation import RelationType
-from dbt.events import AdapterLogger
-from dbt.utils import executor
+
+from dbt_common.clients.agate_helper import table_from_rows
+from dbt.adapters.events.logging import AdapterLogger
+from dbt.adapters.contracts.relation import RelationType
+from dbt_common.contracts.constraints import ConstraintType
+from dbt_common.exceptions import CompilationError, DbtDatabaseError, DbtRuntimeError, DbtInternalError
+from dbt_common.utils import filter_null_values
+from dbt_common.utils import executor
 
 import csv
 import io
 from dbt.adapters.databend.column import DatabendColumn
 from dbt.adapters.databend.connections import DatabendConnectionManager
 from dbt.adapters.databend.relation import DatabendRelation
 
@@ -25,34 +27,21 @@
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
 
 logger = AdapterLogger("databend")
 
 
 def _expect_row_value(key: str, row: agate.Row):
     if key not in row.keys():
-        raise dbt.exceptions.InternalException(
+        raise DbtInternalError(
             f"Got a row without '{key}' column, columns: {row.keys()}"
         )
 
     return row[key]
 
 
-def _catalog_filter_schemas(manifest: Manifest) -> Callable[[agate.Row], bool]:
-    schemas = frozenset((None, s.lower()) for d, s in manifest.get_used_schemas())
-
-    def test(row: agate.Row) -> bool:
-        table_database = _expect_row_value("table_database", row)
-        table_schema = _expect_row_value("table_schema", row)
-        if table_schema is None:
-            return False
-        return (table_database, table_schema.lower()) in schemas
-
-    return test
-
-
 @dataclass
 class DatabendConfig(AdapterConfig):
     cluster_by: Optional[Union[List[str], str]] = None
 
 
 class DatabendAdapter(SQLAdapter):
     Relation = DatabendRelation
@@ -95,15 +84,15 @@
 
     @classmethod
     def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "date"
 
     @classmethod
     def convert_time_type(cls, agate_table: agate.Table, col_idx: int) -> str:
-        raise dbt.exceptions.DbtRuntimeError(
+        raise DbtRuntimeError(
             "`convert_time_type` is not implemented for this adapter!"
         )
 
     def quote(self, identifier):
         return "{}".format(identifier)
 
     def check_schema_exists(self, database, schema):
@@ -111,57 +100,52 @@
             LIST_SCHEMAS_MACRO_NAME, kwargs={"database": database}
         )
 
         exists = True if schema in [row[0] for row in results] else False
         return exists
 
     def list_relations_without_caching(
-        self, schema_relation: DatabendRelation
+            self, schema_relation: DatabendRelation
     ) -> List[DatabendRelation]:
         kwargs = {"schema_relation": schema_relation}
         results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
 
         relations = []
         for row in results:
             if len(row) != 4:
-                raise dbt.exceptions.DbtRuntimeError(
+                raise DbtRuntimeError(
                     f"Invalid value from 'show table extended ...', "
                     f"got {len(row)} values, expected 4"
                 )
             _database, name, schema, type_info = row
             rel_type = RelationType.View if "view" in type_info else RelationType.Table
-            relation = self.Relation.create(
-                database=None,
-                schema=schema,
-                identifier=name,
-                type=rel_type,
-            )
+            relation = self.Relation.create(database=None, schema=schema, identifier=name, rt=rel_type)
             relations.append(relation)
 
         return relations
 
     @classmethod
     def _catalog_filter_table(
-        cls, table: agate.Table, manifest: Manifest
+            cls, table: agate.Table, used_schemas: FrozenSet[Tuple[str, str]]
     ) -> agate.Table:
         table = table_from_rows(
             table.rows,
             table.column_names,
             text_only_columns=["table_schema", "table_name"],
         )
-        return table.where(_catalog_filter_schemas(manifest))
+        return super()._catalog_filter_table(table, used_schemas)
 
     def get_relation(self, database: Optional[str], schema: str, identifier: str):
         # if not self.Relation.include_policy.database:
         #     database = None
 
         return super().get_relation(database, schema, identifier)
 
     def parse_show_columns(
-        self, _relation: DatabendRelation, raw_rows: List[agate.Row]
+            self, _relation: DatabendRelation, raw_rows: List[agate.Row]
     ) -> List[DatabendColumn]:
         rows = [
             dict(zip(row._keys, row._values))  # pylint: disable=protected-access
             for row in raw_rows
         ]
 
         return [
@@ -169,66 +153,41 @@
                 column=column["name"],
                 dtype=column["type"],
             )
             for column in rows
         ]
 
     def get_columns_in_relation(
-        self, relation: DatabendRelation
+            self, relation: DatabendRelation
     ) -> List[DatabendColumn]:
         rows: List[agate.Row] = super().get_columns_in_relation(relation)
 
         return self.parse_show_columns(relation, rows)
 
-    def get_catalog(self, manifest):
-        schema_map = self._get_catalog_schemas(manifest)
-        if len(schema_map) > 1:
-            dbt.exceptions.DbtRuntimeError(
-                f"Expected only one database in get_catalog, found "
-                f"{list(schema_map)}"
-            )
-
-        with executor(self.config) as tpe:
-            futures: List[Future[agate.Table]] = []
-            for info, schemas in schema_map.items():
-                for schema in schemas:
-                    futures.append(
-                        tpe.submit_connected(
-                            self,
-                            schema,
-                            self._get_one_catalog,
-                            info,
-                            [schema],
-                            manifest,
-                        )
-                    )
-            catalogs, exceptions = catch_as_completed(futures)
-        return catalogs, exceptions
-
     def _get_one_catalog(
-        self,
-        information_schema: InformationSchema,
-        schemas: Set[str],
-        manifest: Manifest,
+            self,
+            information_schema: InformationSchema,
+            schemas: Set[str],
+            used_schemas: FrozenSet[Tuple[str, str]],
     ) -> agate.Table:
         if len(schemas) != 1:
-            dbt.exceptions.DbtRuntimeError(
+            DbtRuntimeError(
                 f"Expected only one schema in databend _get_one_catalog, found {schemas}"
             )
 
-        return super()._get_one_catalog(information_schema, schemas, manifest)
+        return super()._get_one_catalog(information_schema, schemas, used_schemas)
 
     def update_column_sql(
-        self,
-        dst_name: str,
-        dst_column: str,
-        clause: str,
-        where_clause: Optional[str] = None,
+            self,
+            dst_name: str,
+            dst_column: str,
+            clause: str,
+            where_clause: Optional[str] = None,
     ) -> str:
-        raise dbt.exceptions.DbtInternalError(
+        raise DbtInternalError(
             "`update_column_sql` is not implemented for this adapter!"
         )
 
     def run_sql_for_tests(self, sql, fetch, conn):
         cursor = conn.handle.cursor()
         try:
             cursor.execute(sql)
@@ -245,19 +204,19 @@
             logger.error(sql)
             logger.error(exc)
             raise exc
         finally:
             conn.transaction_open = False
 
     def get_rows_different_sql(
-        self,
-        relation_a: DatabendRelation,
-        relation_b: DatabendRelation,
-        column_names: Optional[List[str]] = None,
-        except_operator: str = "EXCEPT",
+            self,
+            relation_a: DatabendRelation,
+            relation_b: DatabendRelation,
+            column_names: Optional[List[str]] = None,
+            except_operator: str = "EXCEPT",
     ) -> str:
         names: List[str]
         if column_names is None:
             columns = self.get_columns_in_relation(relation_a)
             names = sorted((self.quote(c.name) for c in columns))
         else:
             names = sorted((self.quote(n) for n in column_names))
@@ -335,8 +294,8 @@
 
     @property
     def default_python_submission_method(self):
         raise NotImplementedError("default_python_submission_method is not specified")
 
     @property
     def python_submission_helpers(self):
-        raise NotImplementedError("python_submission_helpers is not specified")
+        raise NotImplementedError("python_submission_helpers is not specified")
```

## dbt/adapters/databend/relation.py

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass, field
 from typing import Optional, TypeVar, Any, Type, Dict, Union, Iterator, Tuple, Set
-import dbt.exceptions
+
+from dbt_common.exceptions import CompilationError, DbtDatabaseError, DbtRuntimeError, DbtInternalError
 from dbt.adapters.base.relation import BaseRelation, Policy
-from dbt.contracts.relation import (
+from dbt.adapters.contracts.relation import (
     Path,
     RelationType,
 )
 
 
 @dataclass
 class DatabendQuotePolicy(Policy):
@@ -31,46 +32,46 @@
     include_policy: DatabendIncludePolicy = field(
         default_factory=lambda: DatabendIncludePolicy()
     )
     quote_character: str = ""
 
     def __post_init__(self):
         if self.database != self.schema and self.database:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtDatabaseError(
                 f"    schema: {self.schema} \n"
                 f"    database: {self.database} \n"
                 f"On Databend, database must be omitted or have the same value as"
                 f" schema."
             )
 
     @classmethod
     def create(
             cls: Type[Self],
             database: Optional[str] = None,
             schema: Optional[str] = None,
             identifier: Optional[str] = None,
-            type: Optional[RelationType] = None,
+            rt: Optional[RelationType] = None,
             **kwargs,
     ) -> Self:
         database = None
         kwargs.update(
             {
                 "path": {
                     "database": database,
                     "schema": schema,
                     "identifier": identifier,
                 },
-                "type": type,
+                "type": rt,
             }
         )
         return cls.from_dict(kwargs)
 
     def render(self):
         if self.include_policy.database and self.include_policy.schema:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 "Got a databend relation with schema and database set to "
                 "include, but only one can be set"
             )
         return super().render()
 
     @classmethod
     def get_path(
@@ -86,11 +87,11 @@
     def matches(
             self,
             database: Optional[str] = None,
             schema: Optional[str] = None,
             identifier: Optional[str] = None,
     ):
         if database:
-            raise dbt.exceptions.DbtRuntimeError(
+            raise DbtRuntimeError(
                 f"Passed unexpected schema value {schema} to Relation.matches"
             )
         return self.schema == schema and self.identifier == identifier
```

## dbt/include/databend/macros/adapters.sql

```diff
@@ -89,15 +89,15 @@
 {% macro databend__rename_relation(from_relation, to_relation) -%}
 '''Renames a relation in the database.'''
 /*
   1. Search for a specific relation name
   2. alter table by targeting specific name and passing in new name
 */
   {% call statement('drop_relation') %}
-    drop table if exists {{ to_relation }}
+    drop {{ to_relation.type }} if exists {{ to_relation }}
   {% endcall %}
   {% call statement('rename_relation') %}
     rename table {{ from_relation }} to {{ to_relation }}
   {% endcall %}
 {% endmacro %}
 
 {% macro databend__truncate_relation(relation) -%}
@@ -129,28 +129,28 @@
 
 {% macro databend__create_table_as(temporary, relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
 
   {{ sql_header if sql_header is not none }}
 
   {% if temporary -%}
-    create transient table {{ relation.name }} if not exist
+    create or replace transient table {{ relation.name }}
   {%- else %}
-    create table {{ relation.include(database=False) }}
+    create or replace table {{ relation.include(database=False) }}
     {{ cluster_by_clause(label="cluster by") }}
   {%- endif %}
   as {{ sql }}
 {%- endmacro %}
 
 {% macro databend__create_view_as(relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
 
   {{ sql_header if sql_header is not none }}
 
-  create view {{ relation.include(database=False) }}
+  create or replace view {{ relation.include(database=False) }}
   as {{ sql }}
 {%- endmacro %}
 
 {% macro databend__get_columns_in_query(select_sql) %}
   {% call statement('get_columns_in_query', fetch_result=True, auto_begin=False) -%}
     select * from (
         {{ select_sql }}
```

## dbt/include/databend/macros/adapters/relation.sql

```diff
@@ -1,20 +1,18 @@
 {% macro databend__get_or_create_relation(database, schema, identifier, type) %}
   {%- set target_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) %}
   {% if target_relation %}
     {% do return([true, target_relation]) %}
   {% endif %}
 
-  {%- set can_exchange = adapter.can_exchange(schema, type) %}
   {%- set new_relation = api.Relation.create(
-      database=None,
+      database=database,
       schema=schema,
       identifier=identifier,
-      type=type,
-      can_exchange=can_exchange
+      type=type
   ) -%}
   {% do return([false, new_relation]) %}
 {% endmacro %}
 
 {% macro databend__get_database(database) %}
     {% call statement('get_database', fetch_result=True) %}
 select name
```

## dbt/include/databend/macros/materializations/table.sql

```diff
@@ -6,18 +6,18 @@
   {%- set preexisting_backup_relation = none -%}
   {%- set preexisting_intermediate_relation = none -%}
 
   {% if existing_relation is not none %}
     {%- set backup_relation_type = existing_relation.type -%}
     {%- set backup_relation = make_backup_relation(target_relation, backup_relation_type) -%}
     {%- set preexisting_backup_relation = load_cached_relation(backup_relation) -%}
-    {% if not existing_relation.can_exchange %}
-      {%- set intermediate_relation =  make_intermediate_relation(target_relation) -%}
-      {%- set preexisting_intermediate_relation = load_cached_relation(intermediate_relation) -%}
-    {% endif %}
+--     {% if not existing_relation.can_exchange %}
+--       {%- set intermediate_relation =  make_intermediate_relation(target_relation) -%}
+--       {%- set preexisting_intermediate_relation = load_cached_relation(intermediate_relation) -%}
+--     {% endif %}
   {% endif %}
 
   {% set grant_config = config.get('grants') %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
   -- drop the temp relations if they exist already in the database
```

## Comparing `dbt_databend_cloud-1.4.2.dist-info/LICENSE` & `dbt_databend_cloud-1.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dbt_databend_cloud-1.4.2.dist-info/METADATA` & `dbt_databend_cloud-1.8.1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-databend-cloud
-Version: 1.4.2
+Version: 1.8.1
 Summary: The Databend adapter plugin for dbt
 Home-page: https://github.com/databendcloud/dbt-databend.git
 Author: Databend Cloud Team
 Author-email: zhangzhihan@datafuselabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: dbt-core (~=1.5.0)
-Requires-Dist: databend-py (~=0.4.6)
-Requires-Dist: databend-sqlalchemy (~=0.2.4)
+Requires-Dist: dbt-common <2.0,>=1.0.4
+Requires-Dist: dbt-adapters <2.0,>=1.1.1
+Requires-Dist: dbt-core >=1.8.0
+Requires-Dist: agate
+Requires-Dist: databend-sqlalchemy ~=0.3.2
 
 The Databend adapter plugin for dbt
```

## Comparing `dbt_databend_cloud-1.4.2.dist-info/RECORD` & `dbt_databend_cloud-1.8.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 dbt/adapters/databend/__init__.py,sha256=SvHY_N6iQvLzzJNhLWeWP9su1lEfVliXN4NzmFQgzwA,545
-dbt/adapters/databend/__version__.py,sha256=-uWtlLHp1EDR3r-3CaOSpIVyxZIvXb0psDESjAXS1pU,18
-dbt/adapters/databend/column.py,sha256=l0FNfQwJP1kuRtU7OebBH9mhI9LF3sJHN9Kyo76_RGk,1607
-dbt/adapters/databend/connections.py,sha256=MG-3o57ixIZT_bZVUIbZXBIBTxu5kB1lmHJ0ciJOv6c,7531
-dbt/adapters/databend/impl.py,sha256=5c8jYUC5PHuAmB3fG82DSRzFBZl459iiB_nPYx7cg4s,11224
-dbt/adapters/databend/relation.py,sha256=4i9bj3JxYNxaYSeeXFqNa7e8hu0_0AfRrg0nbBOsMmI,2885
+dbt/adapters/databend/__version__.py,sha256=426OzYvRixOakC4L5bESfXkzEDB-ZhhgWtVpaiidIwQ,18
+dbt/adapters/databend/column.py,sha256=fFwh7RKrOfjo_kJw2lH9cNsJJroQtFV4B7f-5N6kLW4,1787
+dbt/adapters/databend/connections.py,sha256=XFQlEOb3_Y12Hw_szvZMQvbEPgA6cN9UMmuMGJDOvWA,8081
+dbt/adapters/databend/impl.py,sha256=b9wXWgzxjG6P-KWXWWJUjU2w3lwYXav_D5OW355q1aM,9979
+dbt/adapters/databend/relation.py,sha256=QgkjAf97VB40QZpBfKOHF6hykdgu561ZzDvTbRXGDag,2929
 dbt/include/databend/__init__.py,sha256=vBGWeG-dHHkimfnX8axBJ4IgAowFw8xADmo6Auzn2xc,52
 dbt/include/databend/dbt_project.yml,sha256=a5ToAC1KwPft8Ch76mfow1MQHwjH1F3JBhDn1skZI0s,77
 dbt/include/databend/profile_template.yml,sha256=_Q0973TJHhTwumKY63JaGVmBrCNkDrWTUk7QNSDiu_0,185
-dbt/include/databend/macros/adapters.sql,sha256=B9hwx8O9B8KpDFTC7ltQ3IGirTm9g7NMcwklPfjKUjk,5771
+dbt/include/databend/macros/adapters.sql,sha256=zfzEfGFP4RDRM6sQfkCs66SzT2bLMxjXbjX1xGDaESg,5808
 dbt/include/databend/macros/catalog.sql,sha256=vcEQgzo9t6JSd3hLMb4MWgjsp87D4UjXa967r63l1FA,796
 dbt/include/databend/macros/incremental.sql,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dbt/include/databend/macros/snapshot.sql,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dbt/include/databend/macros/utils.sql,sha256=RIu7q-44BE2gU10miSNJr11A9X_D9KfNI-HvE7lEa1c,285
 dbt/include/databend/macros/adapters/apply_grants.sql,sha256=49GisxjcJIl70uqPZbye67mEDPH4bszihC4vpoZoQz4,1095
-dbt/include/databend/macros/adapters/relation.sql,sha256=3o8jhfi49A-6bDMP4KxcapTkS7uZ6qnwMDPgoe9Nye4,826
+dbt/include/databend/macros/adapters/relation.sql,sha256=wQ5OlZ02VqpifyF-BtmmKk5NGodq_mg_X2ZtuRG9B-A,734
 dbt/include/databend/macros/materializations/incremental.sql,sha256=-vtmnUcb1s3fAde4HPq5z5iWwTyuhRDfzonXlvtnahk,6216
 dbt/include/databend/macros/materializations/seed.sql,sha256=f8_gtCILvU5nSsp3WgMccVvDvGB4whpntB17-_rTgOE,1111
 dbt/include/databend/macros/materializations/snapshot.sql,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dbt/include/databend/macros/materializations/table.sql,sha256=EHkzF_zAoWeUzAdY0ERFr0_THSuIkxrZ7NcIafW8g8w,2987
-dbt_databend_cloud-1.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-dbt_databend_cloud-1.4.2.dist-info/METADATA,sha256=WoVumJAufFLaknTe9drXxDy6HH88zDdCiJdOm8uODiE,907
-dbt_databend_cloud-1.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dbt_databend_cloud-1.4.2.dist-info/top_level.txt,sha256=B2YH4he17ajilEWOGCKHbRcEJlCuZKwCcgFcLPntLsE,4
-dbt_databend_cloud-1.4.2.dist-info/RECORD,,
+dbt/include/databend/macros/materializations/table.sql,sha256=-61PfdISsL2kjVRKuBwO6f83KXr8JXWMXtwG_x9ssi0,2999
+dbt_databend_cloud-1.8.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+dbt_databend_cloud-1.8.1.dist-info/METADATA,sha256=nQr_MOxhGahWjvhz2yuOC5FuGwMBsTkA_Csu4BLXYhE,918
+dbt_databend_cloud-1.8.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dbt_databend_cloud-1.8.1.dist-info/top_level.txt,sha256=B2YH4he17ajilEWOGCKHbRcEJlCuZKwCcgFcLPntLsE,4
+dbt_databend_cloud-1.8.1.dist-info/RECORD,,
```

