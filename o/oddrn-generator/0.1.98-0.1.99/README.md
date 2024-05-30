# Comparing `tmp/oddrn_generator-0.1.98.tar.gz` & `tmp/oddrn_generator-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oddrn_generator-0.1.98.tar", max compression
+gzip compressed data, was "oddrn_generator-0.1.99.tar", max compression
```

## Comparing `oddrn_generator-0.1.98.tar` & `oddrn_generator-0.1.99.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11356 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/LICENSE
--rw-r--r--   0        0        0     6337 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/README.md
--rw-r--r--   0        0        0     2990 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/oddrn_generator/__init__.py
--rw-r--r--   0        0        0      158 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/oddrn_generator/exceptions.py
--rw-r--r--   0        0        0    13584 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/oddrn_generator/generators.py
--rw-r--r--   0        0        0    27218 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/oddrn_generator/path_models.py
--rw-r--r--   0        0        0     4382 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/oddrn_generator/server_models.py
--rw-r--r--   0        0        0      287 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/oddrn_generator/utils/__init__.py
--rw-r--r--   0        0        0     7327 2023-10-27 13:16:54.027227 oddrn_generator-0.1.98/oddrn_generator/utils/external_generators.py
--rw-r--r--   0        0        0      734 2023-10-27 13:17:24.655700 oddrn_generator-0.1.98/pyproject.toml
--rw-r--r--   0        0        0     7363 1970-01-01 00:00:00.000000 oddrn_generator-0.1.98/setup.py
--rw-r--r--   0        0        0     7089 1970-01-01 00:00:00.000000 oddrn_generator-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/LICENSE
+-rw-r--r--   0        0        0     6643 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/README.md
+-rw-r--r--   0        0        0     2990 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/oddrn_generator/__init__.py
+-rw-r--r--   0        0        0      158 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/oddrn_generator/exceptions.py
+-rw-r--r--   0        0        0    13584 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/oddrn_generator/generators.py
+-rw-r--r--   0        0        0    27333 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/oddrn_generator/path_models.py
+-rw-r--r--   0        0        0     4382 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/oddrn_generator/server_models.py
+-rw-r--r--   0        0        0      287 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/oddrn_generator/utils/__init__.py
+-rw-r--r--   0        0        0     7327 2024-01-24 11:33:01.825895 oddrn_generator-0.1.99/oddrn_generator/utils/external_generators.py
+-rw-r--r--   0        0        0      734 2024-01-24 11:33:29.129371 oddrn_generator-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0     7674 1970-01-01 00:00:00.000000 oddrn_generator-0.1.99/setup.py
+-rw-r--r--   0        0        0     7395 1970-01-01 00:00:00.000000 oddrn_generator-0.1.99/PKG-INFO
```

### Comparing `oddrn_generator-0.1.98/LICENSE` & `oddrn_generator-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.98/README.md` & `oddrn_generator-0.1.99/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,36 +90,39 @@
     host_settings='my.host.com:5432',
     schemas='schema_name', databases='database_name', tables='table_name'
 )
 
 oddrn_gen.base_oddrn
 # //postgresql/host/my.host.com:5432
 oddrn_gen.available_paths
-# ('schemas', 'databases', 'tables', 'columns')
+# ('databases', 'schemas', 'tables', 'views', 'tables_columns', 'views_columns', 'relationships')
 
 oddrn_gen.get_data_source_oddrn()
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
+# //postgresql/host/my.host.com:5432/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("schemas")
-# //postgresql/host/my.host.com:5432/schemas/schema_name
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name
 
 oddrn_gen.get_oddrn_by_path("databases")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
+# //postgresql/host/my.host.com:5432/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("tables")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/table_name
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/table_name
 
 # you can set or change path:
-oddrn_gen.set_oddrn_paths(tables='another_table_name', columns='new_column_name')
-oddrn_gen.get_oddrn_by_path("columns")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/new_column_name
+oddrn_gen.set_oddrn_paths(tables="another_table_name", tables_columns="new_column_name")
+oddrn_gen.get_oddrn_by_path("tables_columns")
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/columns/new_column_name
+
+oddrn_gen.set_oddrn_paths(relationships="references_table_2_with_constraint_fk")
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/relationships/references_table_2_with_constraint_fk
 
 # you can get path wih new values:
-oddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name
+oddrn_gen.get_oddrn_by_path("tables_columns", new_value="another_new_column_name")
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/columns/another_new_column_name
 
 
 # glue
 from oddrn_generator import GlueGenerator
 
 oddrn_gen = GlueGenerator(
     cloud_settings={'account': 'acc_id', 'region': 'reg_id'},
@@ -156,17 +159,17 @@
 
 ```python
 from oddrn_generator import PostgresqlGenerator
 
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432',
     schemas='schema_name', databases='database_name',
-    columns='column_without_table'
+    tables_columns='column_without_table'
 )
-# WrongPathOrderException: 'columns' can not be without 'tables' attribute
+# WrongPathOrderException: 'tables_columns' can not be without 'tables' attribute
 ```
 
 * EmptyPathValueException - raises when trying to get a path that is not set up
 
 ```python
 from oddrn_generator import PostgresqlGenerator
 
@@ -197,9 +200,9 @@
 #Install dependencies
 poetry install
 
 #Activate shell
 poetry shell
 
 # Run tests
-python run pytest
+pytest tests/
 ```
```

### Comparing `oddrn_generator-0.1.98/oddrn_generator/__init__.py` & `oddrn_generator-0.1.99/oddrn_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.98/oddrn_generator/generators.py` & `oddrn_generator-0.1.99/oddrn_generator/generators.py`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.98/oddrn_generator/path_models.py` & `oddrn_generator-0.1.99/oddrn_generator/path_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,25 @@
 class PostgresqlPathsModel(BasePathsModel):
     databases: str
     schemas: Optional[str]
     tables: Optional[str]
     views: Optional[str]
     tables_columns: Optional[str] = Field(alias="columns")
     views_columns: Optional[str] = Field(alias="columns")
+    relationships: Optional[str]
 
     class Config:
         dependencies_map = {
             "databases": ("databases",),
             "schemas": ("databases", "schemas"),
             "tables": ("databases", "schemas", "tables"),
             "views": ("databases", "schemas", "views"),
             "tables_columns": ("databases", "schemas", "tables", "tables_columns"),
             "views_columns": ("databases", "schemas", "views", "views_columns"),
+            "relationships": ("databases", "schemas", "tables", "relationships"),
         }
         data_source_path = "databases"
 
 
 class MysqlPathsModel(BasePathsModel):
     databases: str
     tables: Optional[str]
```

### Comparing `oddrn_generator-0.1.98/oddrn_generator/server_models.py` & `oddrn_generator-0.1.99/oddrn_generator/server_models.py`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.98/oddrn_generator/utils/external_generators.py` & `oddrn_generator-0.1.99/oddrn_generator/utils/external_generators.py`

 * *Files identical despite different names*

### Comparing `oddrn_generator-0.1.98/pyproject.toml` & `oddrn_generator-0.1.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oddrn-generator"
-version = "0.1.98"
+version = "0.1.99"
 description = "Open Data Discovery Resource Name Generator"
 authors = ["Open Data Discovery <pypi@opendatadiscovery.org>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/opendatadiscovery/oddrn-generator"
 repository = "https://github.com/opendatadiscovery/oddrn-generator"
 keywords = ["oddrn", "opendatadiscovery"]
```

### Comparing `oddrn_generator-0.1.98/setup.py` & `oddrn_generator-0.1.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.9.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'oddrn-generator',
-    'version': '0.1.98',
+    'version': '0.1.99',
     'description': 'Open Data Discovery Resource Name Generator',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)\n\n# Open Data Discovery Resource Name Generator\n\nHelps generate oddrn for data sources.\n\n* [Requirements](#requirements)\n* [Installation](#installation)\n* [Available generators](#available-generators)\n* [Generator properties](#generator-properties)\n* [Generator methods](#generator-methods)\n* [Generator properties](#generator-properties)\n* [Example usage](#example-usage)\n* [Exceptions](#example-usage)\n* [Development](#development)\n\n## Requirements\n\n* __Python >= 3.7__\n\n## Installation\n\n```bash\npoetry add oddrn-generator\n# or\npip install oddrn-generator\n```\n\n## Usage and configuration\n\n### Available generators\n| DataSource   | Generator class name  |\n|--------------|-----------------------|\n| cassandra    | CassandraGenerator    |\n| postgresql   | PostgresqlGenerator   |\n| mysql        | MysqlGenerator        |\n| glue         | GlueGenerator         |\n| s3           | S3Generator           |\n| kafka        | KafkaGenerator        |\n| kafkaconnect | KafkaConnectGenerator |\n| snowflake    | SnowflakeGenerator    |\n| airflow      | AirflowGenerator      |\n| hive         | HiveGenerator         |\n| dynamodb     | DynamodbGenerator     |\n| odbc         | OdbcGenerator         |\n| mssql        | MssqlGenerator        |\n| oracle       | OracleGenerator       |\n| redshift     | RedshiftGenerator     |\n| clickhouse   | ClickHouseGenerator   |\n| athena       | AthenaGenerator       |\n| quicksight   | QuicksightGenerator   |\n| dbt          | DbtGenerator          |\n| prefect      | PrefectGenerator      |\n| tableau      | TableauGenerator      |\n| neo4j        | Neo4jGenerator        |\n| mongodb      | MongoGenerator        |\n| vertica      | VerticaGenerator      |\n| CubeJs       | CubeJsGenerator       |\n| superset     | SupersetGenerator     |\n| Presto       | PrestoGenerator       |\n| Trino        | TrinoGenerator        |\n| dms          | DmsGenerator          |\n| powerbi      | PowerBiGenerator      |\n\n### Generator properties\n\n* base_oddrn - Get base oddrn (without path)\n* available_paths - Get all available path of generator\n\n### Generator methods\n\n* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using \'\n  new_value\' param\n* set_oddrn_paths(**kwargs) - Set or update values of oddrn path\n* get_data_source_oddrn() - Get data source oddrn\n\n### Generator parameters:\n\n* host_settings: str - optional. Hostname configuration\n* cloud_settings: dict - optional. Cloud configuration\n* **kwargs - path\'s name and values\n\n### Example usage\n\n```python\n# postgresql\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\', tables=\'table_name\'\n)\n\noddrn_gen.base_oddrn\n# //postgresql/host/my.host.com:5432\noddrn_gen.available_paths\n# (\'schemas\', \'databases\', \'tables\', \'columns\')\n\noddrn_gen.get_data_source_oddrn()\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("schemas")\n# //postgresql/host/my.host.com:5432/schemas/schema_name\n\noddrn_gen.get_oddrn_by_path("databases")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/table_name\n\n# you can set or change path:\noddrn_gen.set_oddrn_paths(tables=\'another_table_name\', columns=\'new_column_name\')\noddrn_gen.get_oddrn_by_path("columns")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/new_column_name\n\n# you can get path wih new values:\noddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")\n# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name\n\n\n# glue\nfrom oddrn_generator import GlueGenerator\n\noddrn_gen = GlueGenerator(\n    cloud_settings={\'account\': \'acc_id\', \'region\': \'reg_id\'},\n    databases=\'database_name\', tables=\'table_name\', columns=\'column_name\',\n    jobs=\'job_name\', runs=\'run_name\', owners=\'owner_name\'\n)\n\noddrn_gen.available_paths\n# (\'databases\', \'tables\', \'columns\', \'owners\', \'jobs\', \'runs\')\n\noddrn_gen.get_oddrn_by_path("databases")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name\'\n\noddrn_gen.get_oddrn_by_path("columns")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name/columns/column_name\n\noddrn_gen.get_oddrn_by_path("jobs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name\n\noddrn_gen.get_oddrn_by_path("runs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name/runs/run_name\n\noddrn_gen.get_oddrn_by_path("owners")\n# //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name\n\n```\n\n### Exceptions\n\n* WrongPathOrderException - raises when trying set path that depends on another path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\',\n    columns=\'column_without_table\'\n)\n# WrongPathOrderException: \'columns\' can not be without \'tables\' attribute\n```\n\n* EmptyPathValueException - raises when trying to get a path that is not set up\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("tables")\n\n# EmptyPathValueException: Path \'tables\' is not set up\n```\n\n* PathDoestExistException - raises when trying to get not existing oddrn path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("jobs")\n\n# PathDoestExistException: Path \'jobs\' doesn\'t exist in generator\n```\n\n## Development\n\n```bash\n#Install dependencies\npoetry install\n\n#Activate shell\npoetry shell\n\n# Run tests\npython run pytest\n```\n',
+    'long_description': '[![PyPI version](https://badge.fury.io/py/oddrn-generator.svg)](https://badge.fury.io/py/oddrn-generator)\n\n# Open Data Discovery Resource Name Generator\n\nHelps generate oddrn for data sources.\n\n* [Requirements](#requirements)\n* [Installation](#installation)\n* [Available generators](#available-generators)\n* [Generator properties](#generator-properties)\n* [Generator methods](#generator-methods)\n* [Generator properties](#generator-properties)\n* [Example usage](#example-usage)\n* [Exceptions](#example-usage)\n* [Development](#development)\n\n## Requirements\n\n* __Python >= 3.7__\n\n## Installation\n\n```bash\npoetry add oddrn-generator\n# or\npip install oddrn-generator\n```\n\n## Usage and configuration\n\n### Available generators\n| DataSource   | Generator class name  |\n|--------------|-----------------------|\n| cassandra    | CassandraGenerator    |\n| postgresql   | PostgresqlGenerator   |\n| mysql        | MysqlGenerator        |\n| glue         | GlueGenerator         |\n| s3           | S3Generator           |\n| kafka        | KafkaGenerator        |\n| kafkaconnect | KafkaConnectGenerator |\n| snowflake    | SnowflakeGenerator    |\n| airflow      | AirflowGenerator      |\n| hive         | HiveGenerator         |\n| dynamodb     | DynamodbGenerator     |\n| odbc         | OdbcGenerator         |\n| mssql        | MssqlGenerator        |\n| oracle       | OracleGenerator       |\n| redshift     | RedshiftGenerator     |\n| clickhouse   | ClickHouseGenerator   |\n| athena       | AthenaGenerator       |\n| quicksight   | QuicksightGenerator   |\n| dbt          | DbtGenerator          |\n| prefect      | PrefectGenerator      |\n| tableau      | TableauGenerator      |\n| neo4j        | Neo4jGenerator        |\n| mongodb      | MongoGenerator        |\n| vertica      | VerticaGenerator      |\n| CubeJs       | CubeJsGenerator       |\n| superset     | SupersetGenerator     |\n| Presto       | PrestoGenerator       |\n| Trino        | TrinoGenerator        |\n| dms          | DmsGenerator          |\n| powerbi      | PowerBiGenerator      |\n\n### Generator properties\n\n* base_oddrn - Get base oddrn (without path)\n* available_paths - Get all available path of generator\n\n### Generator methods\n\n* get_oddrn_by_path(path_name, new_value=None) - Get oddrn string by path. You also can set value for this path using \'\n  new_value\' param\n* set_oddrn_paths(**kwargs) - Set or update values of oddrn path\n* get_data_source_oddrn() - Get data source oddrn\n\n### Generator parameters:\n\n* host_settings: str - optional. Hostname configuration\n* cloud_settings: dict - optional. Cloud configuration\n* **kwargs - path\'s name and values\n\n### Example usage\n\n```python\n# postgresql\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\', tables=\'table_name\'\n)\n\noddrn_gen.base_oddrn\n# //postgresql/host/my.host.com:5432\noddrn_gen.available_paths\n# (\'databases\', \'schemas\', \'tables\', \'views\', \'tables_columns\', \'views_columns\', \'relationships\')\n\noddrn_gen.get_data_source_oddrn()\n# //postgresql/host/my.host.com:5432/databases/database_name\n\noddrn_gen.get_oddrn_by_path("schemas")\n# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name\n\noddrn_gen.get_oddrn_by_path("databases")\n# //postgresql/host/my.host.com:5432/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/table_name\n\n# you can set or change path:\noddrn_gen.set_oddrn_paths(tables="another_table_name", tables_columns="new_column_name")\noddrn_gen.get_oddrn_by_path("tables_columns")\n# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/columns/new_column_name\n\noddrn_gen.set_oddrn_paths(relationships="references_table_2_with_constraint_fk")\n# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/relationships/references_table_2_with_constraint_fk\n\n# you can get path wih new values:\noddrn_gen.get_oddrn_by_path("tables_columns", new_value="another_new_column_name")\n# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/columns/another_new_column_name\n\n\n# glue\nfrom oddrn_generator import GlueGenerator\n\noddrn_gen = GlueGenerator(\n    cloud_settings={\'account\': \'acc_id\', \'region\': \'reg_id\'},\n    databases=\'database_name\', tables=\'table_name\', columns=\'column_name\',\n    jobs=\'job_name\', runs=\'run_name\', owners=\'owner_name\'\n)\n\noddrn_gen.available_paths\n# (\'databases\', \'tables\', \'columns\', \'owners\', \'jobs\', \'runs\')\n\noddrn_gen.get_oddrn_by_path("databases")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name\n\noddrn_gen.get_oddrn_by_path("tables")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name\'\n\noddrn_gen.get_oddrn_by_path("columns")\n# //glue/cloud/aws/account/acc_id/region/reg_id/databases/database_name/tables/table_name/columns/column_name\n\noddrn_gen.get_oddrn_by_path("jobs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name\n\noddrn_gen.get_oddrn_by_path("runs")\n# //glue/cloud/aws/account/acc_id/region/reg_id/jobs/job_name/runs/run_name\n\noddrn_gen.get_oddrn_by_path("owners")\n# //glue/cloud/aws/account/acc_id/region/reg_id/owners/owner_name\n\n```\n\n### Exceptions\n\n* WrongPathOrderException - raises when trying set path that depends on another path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\',\n    schemas=\'schema_name\', databases=\'database_name\',\n    tables_columns=\'column_without_table\'\n)\n# WrongPathOrderException: \'tables_columns\' can not be without \'tables\' attribute\n```\n\n* EmptyPathValueException - raises when trying to get a path that is not set up\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("tables")\n\n# EmptyPathValueException: Path \'tables\' is not set up\n```\n\n* PathDoestExistException - raises when trying to get not existing oddrn path\n\n```python\nfrom oddrn_generator import PostgresqlGenerator\n\noddrn_gen = PostgresqlGenerator(\n    host_settings=\'my.host.com:5432\', schemas=\'schema_name\', databases=\'database_name\',\n)\noddrn_gen.get_oddrn_by_path("jobs")\n\n# PathDoestExistException: Path \'jobs\' doesn\'t exist in generator\n```\n\n## Development\n\n```bash\n#Install dependencies\npoetry install\n\n#Activate shell\npoetry shell\n\n# Run tests\npytest tests/\n```\n',
     'author': 'Open Data Discovery',
     'author_email': 'pypi@opendatadiscovery.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/opendatadiscovery/oddrn-generator',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `oddrn_generator-0.1.98/PKG-INFO` & `oddrn_generator-0.1.99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oddrn-generator
-Version: 0.1.98
+Version: 0.1.99
 Summary: Open Data Discovery Resource Name Generator
 Home-page: https://github.com/opendatadiscovery/oddrn-generator
 License: Apache-2.0
 Keywords: oddrn,opendatadiscovery
 Author: Open Data Discovery
 Author-email: pypi@opendatadiscovery.org
 Requires-Python: >=3.9,<4.0
@@ -109,36 +109,39 @@
     host_settings='my.host.com:5432',
     schemas='schema_name', databases='database_name', tables='table_name'
 )
 
 oddrn_gen.base_oddrn
 # //postgresql/host/my.host.com:5432
 oddrn_gen.available_paths
-# ('schemas', 'databases', 'tables', 'columns')
+# ('databases', 'schemas', 'tables', 'views', 'tables_columns', 'views_columns', 'relationships')
 
 oddrn_gen.get_data_source_oddrn()
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
+# //postgresql/host/my.host.com:5432/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("schemas")
-# //postgresql/host/my.host.com:5432/schemas/schema_name
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name
 
 oddrn_gen.get_oddrn_by_path("databases")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name
+# //postgresql/host/my.host.com:5432/databases/database_name
 
 oddrn_gen.get_oddrn_by_path("tables")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/table_name
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/table_name
 
 # you can set or change path:
-oddrn_gen.set_oddrn_paths(tables='another_table_name', columns='new_column_name')
-oddrn_gen.get_oddrn_by_path("columns")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/new_column_name
+oddrn_gen.set_oddrn_paths(tables="another_table_name", tables_columns="new_column_name")
+oddrn_gen.get_oddrn_by_path("tables_columns")
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/columns/new_column_name
+
+oddrn_gen.set_oddrn_paths(relationships="references_table_2_with_constraint_fk")
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/relationships/references_table_2_with_constraint_fk
 
 # you can get path wih new values:
-oddrn_gen.get_oddrn_by_path("columns", new_value="another_new_column_name")
-# //postgresql/host/my.host.com:5432/schemas/schema_name/databases/database_name/tables/another_table_name/columns/another_new_column_name
+oddrn_gen.get_oddrn_by_path("tables_columns", new_value="another_new_column_name")
+# //postgresql/host/my.host.com:5432/databases/database_name/schemas/schema_name/tables/another_table_name/columns/another_new_column_name
 
 
 # glue
 from oddrn_generator import GlueGenerator
 
 oddrn_gen = GlueGenerator(
     cloud_settings={'account': 'acc_id', 'region': 'reg_id'},
@@ -175,17 +178,17 @@
 
 ```python
 from oddrn_generator import PostgresqlGenerator
 
 oddrn_gen = PostgresqlGenerator(
     host_settings='my.host.com:5432',
     schemas='schema_name', databases='database_name',
-    columns='column_without_table'
+    tables_columns='column_without_table'
 )
-# WrongPathOrderException: 'columns' can not be without 'tables' attribute
+# WrongPathOrderException: 'tables_columns' can not be without 'tables' attribute
 ```
 
 * EmptyPathValueException - raises when trying to get a path that is not set up
 
 ```python
 from oddrn_generator import PostgresqlGenerator
 
@@ -216,10 +219,10 @@
 #Install dependencies
 poetry install
 
 #Activate shell
 poetry shell
 
 # Run tests
-python run pytest
+pytest tests/
 ```
```

