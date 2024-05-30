# Comparing `tmp/palje-2.1.0-py3-none-any.whl.zip` & `tmp/palje-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,20 @@
-Zip file size: 24548 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      131 b- defN 24-Apr-12 06:36 palje/__init__.py
--rw-rw-rw-  2.0 fat    10422 b- defN 24-May-10 07:11 palje/__main__.py
--rw-rw-rw-  2.0 fat     7152 b- defN 24-May-06 13:39 palje/confluence_rest.py
--rw-rw-rw-  2.0 fat    10947 b- defN 24-Apr-16 13:53 palje/mssql_database.py
--rw-rw-rw-  2.0 fat     4256 b- defN 24-May-06 13:39 palje/storage_format.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-May-10 09:03 palje/version.py
--rw-rw-rw-  2.0 fat    10126 b- defN 24-Apr-12 06:36 palje/queries/database_queries.ini
--rw-rw-rw-  2.0 fat    11556 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    23307 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       46 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1024 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/RECORD
-13 files, 79492 bytes uncompressed, 22856 bytes compressed:  71.2%
+Zip file size: 74636 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat      131 b- defN 24-May-30 08:08 palje/__init__.py
+-rw-rw-rw-  2.0 fat    14940 b- defN 24-May-30 08:08 palje/__main__.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 24-May-30 08:08 palje/confluence_rest.py
+-rw-rw-rw-  2.0 fat    11904 b- defN 24-May-30 08:08 palje/mssql_database.py
+-rw-rw-rw-  2.0 fat     4256 b- defN 24-May-30 08:08 palje/storage_format.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-30 08:10 palje/version.py
+-rw-rw-rw-  2.0 fat    12420 b- defN 24-May-30 08:08 palje/gui/gui.py
+-rw-rw-rw-  2.0 fat    40429 b- defN 24-May-30 08:08 palje/gui/palje.png
+-rw-rw-rw-  2.0 fat     6130 b- defN 24-May-30 08:08 palje/gui/components/confluence_connection_widget.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 24-May-30 08:08 palje/gui/components/db_browser_widget.py
+-rw-rw-rw-  2.0 fat    14894 b- defN 24-May-30 08:08 palje/gui/components/db_server_widget.py
+-rw-rw-rw-  2.0 fat    11676 b- defN 24-May-30 08:08 palje/queries/database_queries.ini
+-rw-rw-rw-  2.0 fat    11556 b- defN 24-May-30 08:10 palje-2.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    23793 b- defN 24-May-30 08:10 palje-2.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-30 08:10 palje-2.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       77 b- defN 24-May-30 08:10 palje-2.2.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-30 08:10 palje-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1480 b- defN 24-May-30 08:10 palje-2.2.0.dist-info/RECORD
+18 files, 167112 bytes uncompressed, 72228 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -12,29 +12,44 @@
 
 Filename: palje/storage_format.py
 Comment: 
 
 Filename: palje/version.py
 Comment: 
 
+Filename: palje/gui/gui.py
+Comment: 
+
+Filename: palje/gui/palje.png
+Comment: 
+
+Filename: palje/gui/components/confluence_connection_widget.py
+Comment: 
+
+Filename: palje/gui/components/db_browser_widget.py
+Comment: 
+
+Filename: palje/gui/components/db_server_widget.py
+Comment: 
+
 Filename: palje/queries/database_queries.ini
 Comment: 
 
-Filename: palje-2.1.0.dist-info/LICENSE
+Filename: palje-2.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: palje-2.1.0.dist-info/METADATA
+Filename: palje-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: palje-2.1.0.dist-info/WHEEL
+Filename: palje-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: palje-2.1.0.dist-info/entry_points.txt
+Filename: palje-2.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: palje-2.1.0.dist-info/top_level.txt
+Filename: palje-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: palje-2.1.0.dist-info/RECORD
+Filename: palje-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## palje/__main__.py

```diff
@@ -1,248 +1,418 @@
 # Palje - Document MSSQL databases to Confluence wiki
 #
 # Copyright 2021 ALM Partners Oy
 # SPDX-License-Identifier: Apache-2.0
 
+import getpass
 import sys
 from argparse import ArgumentParser
 
 from palje import storage_format
-from palje.confluence_rest import ConfluenceREST
+from palje.confluence_rest import ConfluenceREST, ConfluenceRESTError
 from palje.mssql_database import MSSQLDatabase, DATABASE_OBJECT_TYPES
 
+# TODO: move palje core functions into their own file and leave only CLI related stuff here
+# TODO: setup and use logging instead of print
+
+def _ask_db_credentials(
+    server: str, database: str, authentication: str
+) -> tuple[str, str]:
+    """Ask the user for database credentials"""
+    if authentication == "Windows":
+        return ("", "")
+    uid = input(f"Username for {server}.{database}: ")
+    if authentication == "AAD":
+        pwd = ""
+    else:
+        pwd = getpass.getpass(f"Password for user {uid}: ")
+    return (uid, pwd)
+
+def _ask_confluence_credentials(space_key: str) -> tuple[str, str]:
+    """Ask the user for Confluence credentials"""
+    uid = input(f"Confluence user for space {space_key}: ")
+    password = getpass.getpass(f"Atlassian API token for user {uid}: ")
+    return (uid, password)
+
 
 def main(argv: list[str] | None = None):
-    global WIKI, DB, SPACE, space_id
     # TODO: possibility to read params from config?
-    (confluence_url, SPACE, parent_page, server, database,
-        schema_filter, database_filter, driver, authentication) = parse_arguments(argv)
+    (
+        confluence_url,
+        space_key,
+        parent_page,
+        server,
+        database,
+        schema_filter,
+        database_filter,
+        driver,
+        authentication,
+    ) = parse_arguments(argv)
     # ============ DATABASE CONNECTION ============
-    DB = MSSQLDatabase(server, database, driver, authentication)
-    DB.connect()
+    if authentication == "Windows":
+        database_client = MSSQLDatabase(
+            server=server,
+            database=database,
+            driver=driver,
+            authentication=authentication,
+        )
+    else:
+        uid, pwd = _ask_db_credentials(
+            server=server, database=database, authentication=authentication
+        )
+        database_client = MSSQLDatabase(
+            server=server,
+            database=database,
+            driver=driver,
+            authentication=authentication,
+            username=uid,
+            password=pwd,
+        )
+
+    database_client.connect()
+
+    available_databases = database_client.get_databases()
+    if database_client.database not in available_databases:
+        # This happens if the database name has different case than in sys.databases
+        # Find the assumed correct name and show error message to the user
+        print(f"Database '{database_client.database}' was not found on the server. Did you mean '{[db for db in available_databases if db.lower() == database_client.database.lower()][0]}'?")
+        quit()
+
     # =========== CONFLUENCE CONNECTION ===========
-    WIKI = ConfluenceREST(confluence_url)
-    WIKI.verify_credentials()
-    space_id = WIKI.get_space_id(SPACE)
+    confluence_client = ConfluenceREST(confluence_url)
+    confluence_client.user_id, confluence_client.api_token = _ask_confluence_credentials(space_key)
+    # TODO: is this test needed here? In practice, the followin get_space_id does the same.
+    try:
+        confluence_client.test_confluence_access(
+            confluence_user_id=confluence_client.user_id,
+            confluence_api_token=confluence_client.api_token,
+            space_key=space_key
+        )
+    except ConfluenceRESTError as err:
+        print(
+            f"Can't access {space_key} with given credentials."
+            + f" Check your username, password and Confluence URL."
+        )
+        quit()
+
+    space_id = confluence_client.get_space_id(space_key)
     if not space_id:
-        print(f'Failed to retrieve the id of space {SPACE}. Aborting.')
+        print(f"Failed to retrieve the id of space {space_key}. Aborting.")
         quit()
+
     # ============ SCHEMAS TO DOCUMENT ============
-    schemas = collect_schemas_to_document(schema_filter)
+    schemas = collect_schemas_to_document(database_client, schema_filter)
     # ==== DATABASES WHERE TO SEEK DEPENDENCIES ===
-    dep_databases = collect_databases_to_query_dependencies(database_filter)
+
+    dep_databases = collect_databases_to_query_dependencies(
+        database_client, database_filter, available_databases
+    )
     print("--------------------------")
-    print(f"Object dependencies are queried from the following databases: " +
-          f"{', '.join(dep_databases)}")
+    print(
+        f"Object dependencies are queried from the following databases: "
+        + f"{', '.join(dep_databases)}"
+    )
     print("--------------------------")
     # ================= ROOT PAGE =================
-    root_page_id = create_or_update_root_page(space_id, parent_page)
+    root_page_id = create_or_update_root_page(
+        database_client, confluence_client, space_id, parent_page
+    )
     # ================ OTHER PAGES ================
+    create_or_update_subpages(
+        database_client,
+        confluence_client,
+        space_id,
+        schemas,
+        dep_databases,
+        root_page_id,
+    )
+
+
+def create_or_update_subpages(
+    database_client, confluence_client, space_id, schemas, dep_databases, root_page_id
+):
     for schema in schemas:
-        schema_page_id = create_and_update_schema_page(root_page_id, schema)
-        objects = collect_objects_to_document(schema)
+        schema_page_id = create_and_update_schema_page(
+            database_client, confluence_client, space_id, root_page_id, schema
+        )
+        objects = collect_objects_to_document(database_client, schema)
         for object_type in objects:
             type_page_id = create_and_update_object_type_page(
-                schema_page_id, schema, object_type)
+                database_client,
+                confluence_client,
+                space_id,
+                schema_page_id,
+                schema,
+                object_type,
+            )
             for object_name in objects[object_type]:
                 create_and_update_object_page(
-                    type_page_id, schema, object_type, object_name, dep_databases)
+                    database_client,
+                    confluence_client,
+                    space_id,
+                    type_page_id,
+                    schema,
+                    object_type,
+                    object_name,
+                    dep_databases,
+                )
 
 
 def parse_arguments(args):
     parser = ArgumentParser(
-        description='A tool for creating hierarchical documentation of SQL Server databases to Confluence wiki.')
-    parser.add_argument('confluence-url',
-                        help='URL to Confluence REST content. In Confluence Cloud, this is something like https://yourconfluence.atlassian.net/wiki/rest/api/content.')
-    parser.add_argument('space',
-                        help='Space key of the Confluence space, in which the documentation is created.')
-    parser.add_argument('--parent-page',
-                        help='Name or title of the Confluence page, under which the documentation is created. If page is not given, the documentation will be created to top level (under pages).')
-    parser.add_argument('server',
-                        help='Host name of the SQL Server. Include port with comma.')
-    parser.add_argument('database',
-                        help='Name of the database that is documented.')
-    parser.add_argument('--schemas', nargs='+',
-                        help='Names of the schemas that are documented. If not given, all schemas will be documented.')
-    parser.add_argument('--dependent', nargs='+',
-                        help='Names of the databases, where object dependencies are sought. If not given, dependencies are sought only in documented database.')
-    parser.add_argument('--db-driver', default="ODBC Driver 17 for SQL Server",
-                        help='Name of the database driver.')
-    parser.add_argument('--authentication', default="SQL",
-                        help='Authentication method to database. If not provided, SQL authentication is used. Other options are "Windows" (Windwos authentication will be used) \
-                             and "AAD" (Azure Active Directory login will be prompted) ')
+        description="A tool for creating hierarchical documentation of SQL Server databases to Confluence wiki."
+    )
+    parser.add_argument(
+        "confluence-url",
+        help='URL to Confluence REST content. In Confluence Cloud, this is something like https://<your-org>.atlassian.net/.',
+    )
+    parser.add_argument(
+        "space",
+        help="Space key of the Confluence space, in which the documentation is created.",
+    )
+    parser.add_argument(
+        "--parent-page",
+        help="Name or title of the Confluence page, under which the documentation is created. If page is not given, the documentation will be created to top level (under pages).",
+    )
+    parser.add_argument(
+        "server", help="Host name of the SQL Server. Include port with comma."
+    )
+    parser.add_argument("database", help="Name of the database that is documented.")
+    parser.add_argument(
+        "--schemas",
+        nargs="+",
+        help="Names of the schemas that are documented. If not given, all schemas will be documented.",
+    )
+    parser.add_argument(
+        "--dependent",
+        nargs="+",
+        help="Names of the databases, where object dependencies are sought. If not given, dependencies are sought only in documented database.",
+    )
+    parser.add_argument(
+        "--db-driver",
+        default="ODBC Driver 17 for SQL Server",
+        help="Name of the database driver.",
+    )
+    parser.add_argument(
+        "--authentication",
+        default="SQL",
+        help='Authentication method to database. If not provided, SQL authentication is used. Other options are "Windows" (Windwos authentication will be used) \
+                             and "AAD" (Azure Active Directory login will be prompted) ',
+    )
     args = vars(parser.parse_args(args))
     return (
-        args.get('confluence-url'),
-        args.get('space'),
-        args.get('parent_page'),
-        args.get('server'),
-        args.get('database'),
-        args.get('schemas'),
-        args.get('dependent'),
-        args.get('db_driver', 'ODBC Driver 17 for SQL Server'),
-        args.get('authentication', 'SQL')
+        args.get("confluence-url"),
+        args.get("space"),
+        args.get("parent_page"),
+        args.get("server"),
+        args.get("database"),
+        args.get("schemas"),
+        args.get("dependent"),
+        args.get("db_driver", "ODBC Driver 17 for SQL Server"),
+        args.get("authentication", "SQL"),
     )
 
 
-def collect_schemas_to_document(schema_filter):
+def collect_schemas_to_document(database_client: MSSQLDatabase, schema_filter):
     """If documented schemas not given,
     document all schemas.
     """
-    all_schemas = DB.get_schemas()
+    all_schemas = database_client.get_schemas()
     if schema_filter:
         schemas = [s for s in schema_filter if s in all_schemas]
         schemas = list(set(schemas))
     else:
         schemas = list(set(all_schemas))  # unique database schemas
     return schemas
 
 
-def collect_databases_to_query_dependencies(database_filter):
+def collect_databases_to_query_dependencies(
+    database_client: MSSQLDatabase, database_filter, available_databases
+):
     """If dependent databases not given,
     track dependencies only inside documented database.
     """
     if database_filter:
-        server_databases = DB.get_databases()
-        database_filter.append(DB.database)  # add current database to filter
-        dep_databases = [d for d in database_filter if d in server_databases]
+        database_filter.append(
+            database_client.database
+        )  # add current database to filter
+        dep_databases = [d for d in database_filter if d in available_databases]
         return list(set(dep_databases))
     else:
-        return [DB.database]
+        return [database_client.database]
 
 
-def collect_objects_to_document(schema):
+def collect_objects_to_document(database_client: MSSQLDatabase, schema):
     """Create dict of form
     {
         'Tables': ['table_1', 'table_2'],
         'Views': ['view_1', 'view_5'],
         ...
     }
     """
     objects = {}
-    db_objects = DB.get_objects(schema)
+    db_objects = database_client.get_objects(schema)
     for o in db_objects:
-        o_type = DATABASE_OBJECT_TYPES[o['type']]
+        o_type = DATABASE_OBJECT_TYPES[o["type"]]
         try:
-            objects[o_type].append(o['name'])
+            objects[o_type].append(o["name"])
         except:
             objects[o_type] = []
-            objects[o_type].append(o['name'])
+            objects[o_type].append(o["name"])
     return objects
 
 
-def create_or_update_root_page(space_id, page_name=None):
+def create_or_update_root_page(
+    database_client: MSSQLDatabase,
+    confluence_client: ConfluenceREST,
+    space_id,
+    page_name=None,
+):
     """Create or update the root page of the documentation.
 
     If a page name is given, that will be used as the name of the root
     page. If no name is given, the default name 'DATABASE: <name-of-db>'
     is used.
 
     If a page already exists with the page name it and it's children
     will be updated, otherwise new pages will be created.
     """
-    default_page_name = 'DATABASE: ' + DB.database
+    default_page_name = "DATABASE: " + database_client.database
     page_content = storage_format.objects_list()
     page_id = None
 
     if not page_name:
         page_name = default_page_name
 
-    page_id = WIKI.get_page_id(space_id, page_name)
+    page_id = confluence_client.get_page_id(space_id, page_name)
 
     if page_id:
-        WIKI.update_page(page_id, page_name, page_content)
+        confluence_client.update_page(page_id, page_name, page_content)
     else:
-        page_id = WIKI.new_page(space_id, page_name, page_content)
+        page_id = confluence_client.new_page(space_id, page_name, page_content)
     return page_id
 
 
-def create_and_update_schema_page(root_page_id, schema):
+def create_and_update_schema_page(
+    database_client: MSSQLDatabase,
+    confluence_client: ConfluenceREST,
+    space_id: str,
+    root_page_id,
+    schema,
+):
     """First, get schema description.
     Second, check that schema page exists.
     If page exists, update it.
     Else, create schema page under root page.
     """
-    schema_page_name = DB.database + '.' + schema
-    description = DB.get_schema_description(schema)
-    schema_page_content = storage_format.description_header(description) + \
-        storage_format.objects_list()
+    schema_page_name = database_client.database + "." + schema
+    description = database_client.get_schema_description(schema)
+    schema_page_content = (
+        storage_format.description_header(description) + storage_format.objects_list()
+    )
 
-    schema_page_id = WIKI.get_page_id(space_id, schema_page_name)
+    schema_page_id = confluence_client.get_page_id(space_id, schema_page_name)
     if schema_page_id:
-        WIKI.update_page(schema_page_id, schema_page_name, schema_page_content)
+        confluence_client.update_page(
+            schema_page_id, schema_page_name, schema_page_content
+        )
     else:
-        schema_page_id = WIKI.new_page(
-            space_id, schema_page_name, schema_page_content, root_page_id)
+        schema_page_id = confluence_client.new_page(
+            space_id, schema_page_name, schema_page_content, root_page_id
+        )
 
     return schema_page_id
 
 
-def create_and_update_object_type_page(schema_page_id, schema, object_type):
+def create_and_update_object_type_page(
+    database_client: MSSQLDatabase,
+    confluence_client: ConfluenceREST,
+    space_id: str,
+    schema_page_id,
+    schema,
+    object_type,
+):
     """First, check that object type page exists.
     If page exists, update it.
     Else, create object type page under schema page.
     """
-    type_page_name = object_type + ' ' + DB.database + '.' + schema
+    type_page_name = object_type + " " + database_client.database + "." + schema
     type_page_content = storage_format.objects_list()
 
-    type_page_id = WIKI.get_page_id(space_id, type_page_name)
+    type_page_id = confluence_client.get_page_id(space_id, type_page_name)
     if type_page_id:
-        WIKI.update_page(type_page_id, type_page_name, type_page_content)
+        confluence_client.update_page(type_page_id, type_page_name, type_page_content)
     else:
-        type_page_id = WIKI.new_page(
-            space_id, type_page_name, type_page_content, schema_page_id)
+        type_page_id = confluence_client.new_page(
+            space_id, type_page_name, type_page_content, schema_page_id
+        )
     return type_page_id
 
 
 def create_and_update_object_page(
-        type_page_id, schema, object_type, object_name, dep_databases):
+    database_client: MSSQLDatabase,
+    confluence_client: ConfluenceREST,
+    space_id: str,
+    type_page_id,
+    schema,
+    object_type,
+    object_name,
+    dep_databases,
+):
     """First, create object page content.
     Second, check that object page exist.
     If page exists, update it.
     Else, create object page under object type page.
     """
-    object_page_title = DB.database + '.' + schema + '.' + object_name
+    object_page_title = database_client.database + "." + schema + "." + object_name
     object_page_content = create_object_page_content(
-        schema, object_type, object_name, dep_databases)
+        database_client, schema, object_type, object_name, dep_databases
+    )
 
-    object_page_id = WIKI.get_page_id(space_id, object_page_title)
+    object_page_id = confluence_client.get_page_id(space_id, object_page_title)
     if object_page_id:
-        WIKI.update_page(object_page_id, object_page_title,
-                         object_page_content, parent_id=type_page_id)
+        confluence_client.update_page(
+            object_page_id,
+            object_page_title,
+            object_page_content,
+            parent_id=type_page_id,
+        )
     else:
-        WIKI.new_page(space_id, object_page_title,
-                      object_page_content, parent_id=type_page_id)
+        confluence_client.new_page(
+            space_id, object_page_title, object_page_content, parent_id=type_page_id
+        )
 
 
-def create_object_page_content(schema, object_type, object_name, dep_databases):
+def create_object_page_content(
+    database_client: MSSQLDatabase, schema, object_type, object_name, dep_databases
+):
     """Object page consists of
     - Header with object description
     - For tables and views, HTML table listing
         - columns
         - their data types
         - extended properties
     - For tables and views, HTML table listing indexes
     - For procedures and functions, HTML table listing routine parameters
     - HTML table listing object dependencies in dep_databases
     """
-    description = DB.get_object_description(schema, object_name)
+    description = database_client.get_object_description(schema, object_name)
     object_page_content = storage_format.description_header(description)
-    if object_type in ['Tables', 'Views']:
-        object_columns = DB.get_object_columns(
-            schema, object_type, object_name)
+    if object_type in ["Tables", "Views"]:
+        object_columns = database_client.get_object_columns(
+            schema, object_type, object_name
+        )
         object_page_content += storage_format.column_table(object_columns)
-        object_indexes = DB.get_object_indexes(schema, object_name)
+        object_indexes = database_client.get_object_indexes(schema, object_name)
         object_page_content += storage_format.index_table(object_indexes)
-    elif object_type in ['Procedures', 'Functions']:
-        object_parameters = DB.get_object_parameters(schema, object_name)
-        object_page_content += storage_format.parameter_table(
-            object_parameters)
-    object_dependencies = DB.get_object_dependencies(
-        schema, object_name, dep_databases)
-    object_page_content += storage_format.dependencies_table(
-        object_dependencies)
+    elif object_type in ["Procedures", "Functions"]:
+        object_parameters = database_client.get_object_parameters(schema, object_name)
+        object_page_content += storage_format.parameter_table(object_parameters)
+    object_dependencies = database_client.get_object_dependencies(
+        schema, object_name, dep_databases
+    )
+    object_page_content += storage_format.dependencies_table(object_dependencies)
     return object_page_content
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

## palje/confluence_rest.py

```diff
@@ -1,23 +1,40 @@
 # Palje - Document MSSQL databases to Confluence wiki
 #
 # Copyright 2021 ALM Partners Oy
 # SPDX-License-Identifier: Apache-2.0
 
-import getpass
 import json
 from urllib.parse import urljoin
 
-from requests import get, post, put
+import requests
+from requests.auth import HTTPBasicAuth
 from requests.exceptions import HTTPError
 
+
+class ConfluenceRESTError(Exception):
+    """Generic Confluence related exception"""
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
+class ConfluenceRESTAuthError(ConfluenceRESTError):
+    """Generic Confluence related exception"""
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
+
 HEADERS = {"Content-type": "application/json"}
 
+# TODO: wrap exceptions into ConfluenceRESTErrors (and subclasses) to avoid requests imports in the main code
+# TODO: use logging instead of print
+
 class ConfluenceREST:
-    '''Class for confluence REST API tools.
+    """Class for confluence REST API tools.
 
     Arguments
     ---------
     atlassian_url
         URL to Atlassian root page. The form is
         https://<yourconfluence>.atlassian.net/.
 
@@ -26,131 +43,152 @@
     name
         Network location part from atlassian_url.
         Empty if not present.
     headers
         HTTP header to a request.
     auth
         Authentication tuple to a request.
-    '''
+    """
+
+    _confluence_user_id: str
+    _confluence_api_token: str
 
-    def __init__(self, atlassian_url):
-        self.wiki_root_url = urljoin(atlassian_url, 'wiki/')
+    def __init__(self, atlassian_url: str):
+        # TODO: take creds as params
+        self.wiki_root_url = urljoin(atlassian_url, "wiki/")
         self.name = atlassian_url
         self.headers = HEADERS
-        self.auth = ''
-
-    def verify_credentials(self):
-        '''Ask for credentials and check that they work.
+        self._confluence_user_id = ""
+        self._confluence_api_token = ""
 
-        Ask the user for a username and API token for Confluence. Verify
-        that the credentials work by sending a request to the wiki's
-        root url. Quit palje if the login fails.
-        '''
-        uid = input(f"Confluence user for {self.name}: ")
-        password = getpass.getpass(f"Atlassian API token for user {uid}: ")
-        self.auth = (uid, password)
+    def test_confluence_access(
+        self, confluence_user_id: str, confluence_api_token: str, space_key: str
+    ) -> bool:
+        """Test if the Confluence space is accessible with given crendentials."""
+
+        # TODO: test with set credentials instead of params
+        url = urljoin(self.wiki_root_url, "api/v2/spaces")
+        auth = HTTPBasicAuth(username=confluence_user_id, password=confluence_api_token)
+        headers = {"Accept": "application/json"}
         try:
-            response = get(self.wiki_root_url, auth=self.auth)
+            response = requests.request(
+                "GET", url, params={"keys": [space_key]}, headers=headers, auth=auth
+            )
             response.raise_for_status()
+            if len(response.json()["results"]) == 0:
+                raise ConfluenceRESTAuthError("No accessible space was found with the given key.")
             return True
-        except Exception as err:
-            print(err)
-            print(f'Failed to login into Confluence {self.name}.' +
-                  f' Check your username, password and Confluence URL.')
-            quit()
+        except HTTPError as err:
+            raise ConfluenceRESTError(str(err)) from err
+
+    @property
+    def auth(self) -> tuple[str, str]:
+        return (self._confluence_user_id, self._confluence_api_token)
+
+    @auth.setter
+    def auth(self, values: tuple[str, str]):
+        self._confluence_user_id = values[0]
+        self._confluence_api_token = values[1]
+
+    @property
+    def user_id(self) -> str:
+        return self._confluence_user_id
+
+    @user_id.setter
+    def user_id(self, value):
+        self._confluence_user_id = value
+
+    @property
+    def api_token(self) -> str:
+        return self._confluence_api_token
+
+    @api_token.setter
+    def api_token(self, value):
+        self._confluence_api_token = value
+
 
     def get_space_id(self, space_key):
-        '''Return the id of the space or None.
+        """Return the id of the space or None.
 
         Arguments
         ---------
         space_key
             The key of the space.
-        '''
-        url = urljoin(self.wiki_root_url, 'api/v2/spaces')
-        response = get(
-            url,
-            params={'keys': [space_key]},
-            auth=self.auth)
+        """
+        url = urljoin(self.wiki_root_url, "api/v2/spaces")
+        response = requests.get(url, params={"keys": [space_key]}, auth=self.auth)
         response.raise_for_status()
-        if results := response.json()['results']:
-            return results[0]['id']
+        if results := response.json()["results"]:
+            return results[0]["id"]
         return None
 
     def get_page_id(self, space_id, page_title):
-        '''Return the id of the page or None if no page is found.
+        """Return the id of the page or None if no page is found.
 
         Page titles are unique inside a space.
 
         Arguments
         ---------
         space_id
             The id of the space the page is in.
         page_title
             The title of the page.
-        '''
-        url = urljoin(self.wiki_root_url, 'api/v2/pages')
-        response = get(
-            url,
-            params={
-                'title': page_title,
-                'space-id': [space_id]},
-            auth=self.auth)
+        """
+        url = urljoin(self.wiki_root_url, "api/v2/pages")
+        response = requests.get(
+            url, params={"title": page_title, "space-id": [space_id]}, auth=self.auth
+        )
         try:
             response.raise_for_status()
-            if results := response.json()['results']:
-                return results[0]['id']
+            if results := response.json()["results"]:
+                return results[0]["id"]
             return None
         except HTTPError as err:
-            print(f'Failed to retrieve the id of the page {page_title}.')
-            print(f'Response: {err.response.text}')
+            print(f"Failed to retrieve the id of the page {page_title}.")
+            print(f"Response: {err.response.text}")
             return None
 
     def new_page(self, space_id, page_title, page_content, parent_id=None):
-        '''Create a new page.
+        """Create a new page.
 
         Arguments
         ---------
         space_id
             The id of the space where the page will be created.
         page_title
             The title of the page.
         page_content
             The content of the page. Can be either simple HTML or
             Confluence Storage Format.
         parent_id
             The id number of the page whose child the page should be.
             If this is None, the page is created into the root of the
             space.
-        '''
+        """
         url = urljoin(self.wiki_root_url, "api/v2/pages")
         data = {
             "title": page_title,
             "spaceId": space_id,
-            "body": {
-                "representation": "storage",
-                "value": page_content}
+            "body": {"representation": "storage", "value": page_content},
         }
         if parent_id:
             data["parentId"] = parent_id
-        response = post(
-            url,
-            data=json.dumps(data),
-            headers=self.headers,
-            auth=self.auth)
+        response = requests.post(
+            url, data=json.dumps(data), headers=self.headers, auth=self.auth
+        )
         try:
             response.raise_for_status()
-            print(f'Page {page_title} created.')
-            return response.json()['id']
+            print(f"Page {page_title} created.")
+            return response.json()["id"]
         except HTTPError as err:
-            print(f'Failed to create page {page_title}.')
-            print(f'Response: {err.response.text}')
+            print(f"Failed to create page {page_title}.")
+            print(f"Response: {err.response.text}")
 
     def update_page(self, page_id, page_title, page_content, parent_id=None):
-        '''Update the title, content and/or parent of a page.
+        """Update the title, content and/or parent of a page.
 
         Notice that this overwrites the previous contents of the page!
 
         Arguments
         ---------
         page_id
             The id number of the page.
@@ -158,59 +196,56 @@
             The new title of the page. If the title isn't changed, the
             old title has to be given.
         page_content
             The content of the page. Can be either simple HTML or
             Confluence Storage Format.
         parent-id
             The new parent of page.
-        '''
+        """
         new_page_status = "current"
         content_representation_type = "storage"
         page_url = urljoin(self.wiki_root_url, f"api/v2/pages/{page_id}/")
 
         # get current version number
-        versions_url = urljoin(page_url, 'versions')
-        response = get(
-            versions_url,
-            params={'limit': 1, "sort": "-modified-date"},
-            auth=self.auth)
-        
+        versions_url = urljoin(page_url, "versions")
+        response = requests.get(
+            versions_url, params={"limit": 1, "sort": "-modified-date"}, auth=self.auth
+        )
+
         try:
             response.raise_for_status()
-            if results := response.json()['results']:
-                current_version = results[0]['number']
+            if results := response.json()["results"]:
+                current_version = results[0]["number"]
                 new_version = current_version + 1
             else:
-                print(f'Failed to retrieve the version number of page {page_title}.')
+                print(f"Failed to retrieve the version number of page {page_title}.")
                 print(f"Cannot update page {page_title}.")
                 return
         except HTTPError as err:
-            print(f'Failed to retrieve the version number of page {page_title}.')
-            print(f'Response: {err.response.text}')
+            print(f"Failed to retrieve the version number of page {page_title}.")
+            print(f"Response: {err.response.text}")
             return
 
         # NEW CONTENT
         new_data = {
             "id": page_id,
             "status": new_page_status,
             "title": page_title,
             "body": {
                 "representation": content_representation_type,
-                "value": page_content
+                "value": page_content,
             },
-            "version": {"number": new_version}
+            "version": {"number": new_version},
         }
         if parent_id:
             new_data["parent_id"] = parent_id
 
         # UPDATE
-        response = put(
-            page_url,
-            data=json.dumps(new_data),
-            headers=self.headers,
-            auth=self.auth)
+        response = requests.put(
+            page_url, data=json.dumps(new_data), headers=self.headers, auth=self.auth
+        )
         try:
             response.raise_for_status()
-            print(f'Page {page_title} updated.')
+            print(f"Page {page_title} updated.")
         except HTTPError as err:
-            print(f'Failed to update page {page_title}.')
-            print(f'Response: {err.response.text}')
+            print(f"Failed to update page {page_title}.")
+            print(f"Response: {err.response.text}")
```

## palje/mssql_database.py

```diff
@@ -1,14 +1,13 @@
 # Palje - Document MSSQL databases to Confluence wiki
 #
 # Copyright 2021 ALM Partners Oy
 # SPDX-License-Identifier: Apache-2.0
 
 """Module for querying data from MSSQL database."""
-import getpass
 import struct
 import pyodbc
 import importlib
 from os import path
 from configparser import ConfigParser
 
 
@@ -17,68 +16,93 @@
     'BASE TABLE': 'Tables',
     'VIEW': 'Views',
     'PROCEDURE': 'Procedures',
     'FUNCTION': 'Functions'
 }
 SQL_COPT_SS_ACCESS_TOKEN = 1256  # This connection option is defined by microsoft in msodbcsql.h
 
+# TODO: exception handling (wrap into custom exceptions)
+# TODO: use logging instead of print
 
 class MSSQLDatabase():
-    def __init__(self, server, database, driver, authentication):
+    def __init__(self, server, database, driver, authentication, port: int = 1433, username: str | None = None, password: str | None = None):
         self.server = server
         self.database = database
         self.driver = driver
         self.authentication = authentication
         self.connection = None
         self.queries = self._read_queries_from_ini()
+        self.username = username
+        self.password = password
+        self.port = port
+
+    @staticmethod
+    def available_db_drivers() -> list[str]:
+        """Return a list of available SQL Server drivers available to pyodbc."""
+        all_drivers = pyodbc.drivers()
+        applicable_drivers = list(filter(lambda driver_name: 'SQL Server' in driver_name, all_drivers))
+        applicable_drivers.sort()
+        return applicable_drivers
 
     @staticmethod
     def _read_queries_from_ini():
         current_dir = path.dirname(path.abspath(__file__))
         config_file = path.join(current_dir, QUERY_FILE)
         config = ConfigParser()
         config.read(config_file)
         return config['Queries']
 
+    def close(self):
+        try:
+            self.connection.close()
+        except:
+            print(
+                'Failed to close the database connection. Most likely because the connection is already closed.')
+
     def connect(self):
-        connection_str = self._ask_credentials()
         try:
             if self.authentication.lower() == "azureidentity":
                 self.connection = pyodbc.connect(
-                    connection_str,
+                    self.connection_string,
                     attrs_before={SQL_COPT_SS_ACCESS_TOKEN: self.get_az_token()}
                 )
             else:
-                self.connection = pyodbc.connect(connection_str)
+                self.connection = pyodbc.connect(self.connection_string)
         except:
             print(
                 f'Failed to connect to {self.server}.{self.database}. Check your server details, username and password.')
             raise
 
-    def close(self):
+    def change_current_db(self, db_name: str):
+        if self.connection is None:
+            self.connect()
+        cursor = self.connection.cursor()
         try:
-            self.connection.close()
-        except:
-            print(
-                'Failed to close the database connection. Most likely because the connection is already closed.')
-
-    def _ask_credentials(self):
-        conn_str = f'DRIVER={{{self.driver}}};SERVER={self.server};DATABASE={self.database}'
+            # TODO: sanitize db_name? 
+            # Apparently default sanitization (?, db_name) is not supported for this kind of query.
+            cursor.execute(f"USE {db_name}")
+            self.database = db_name
+        except pyodbc.Error as ex:
+            print(f'Failed to change database to {db_name}')
+            raise ex
+
+    @property
+    def connection_string(self) -> str:
+        conn_str = f'DRIVER={{{self.driver}}};SERVER={self.server}'
+        if self.port:
+            conn_str = f'{conn_str},{self.port}'
+        if self.database:
+            conn_str = f'{conn_str};DATABASE={self.database}'
         if self.authentication == 'SQL':
-            uid = input(
-                f'User for {self.server}.{self.database}. If you wish to use Windows Authentication, hit enter: ')
-            if uid:
-                pwd = getpass.getpass(f'Password for user {uid}: ')
-                conn_str = f'{conn_str};UID={uid};PWD={pwd}'
-            else: 
-                conn_str = f'{conn_str};Trusted_Connection=yes;'
+            conn_str = f'{conn_str};UID={self.username};PWD={self.password}'
         elif self.authentication == 'Windows':
             conn_str = f'{conn_str};Trusted_Connection=yes;'
         elif self.authentication == 'AAD':
             conn_str = f'{conn_str};Authentication=ActiveDirectoryInteractive;'
+
         return conn_str
 
     def get_az_token(self):
         identity = importlib.import_module('.identity', 'azure')
         credential = identity.DefaultAzureCredential(exclude_interactive_browser_credential=False)
         token_bytes = credential.get_token("https://database.windows.net/.default").token.encode("UTF-16-LE")
         token_struct = struct.pack(f'<I{len(token_bytes)}s', len(token_bytes), token_bytes)
```

## palje/version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '2.1.0'
-__version_tuple__ = version_tuple = (2, 1, 0)
+__version__ = version = '2.2.0'
+__version_tuple__ = version_tuple = (2, 2, 0)
```

## palje/queries/database_queries.ini

```diff
@@ -151,47 +151,79 @@
                  JOIN sys.indexes ind
                  	ON ind.object_id = OBJECT_ID('' + tbl.TABLE_SCHEMA + '.' + tbl.TABLE_NAME)
                  	AND ind.is_primary_key = 0	-- do not include primary keys
                  WHERE ind.type <> 0
 					 AND tbl.TABLE_SCHEMA = ?
                      AND tbl.TABLE_NAME = ?
 
-index_columns = SELECT
-                	col.COLUMN_NAME	AS [column_name],
-                	CASE
+index_columns = SELECT col.name AS [column_name],
+                    CASE
                         WHEN indc.is_descending_key = 0 THEN '(ascending)'
                         ELSE '(descending)'
                     END		AS [column_sort_order]
-                FROM INFORMATION_SCHEMA.COLUMNS col
-                JOIN sys.indexes ind
-                	ON ind.object_id = OBJECT_ID('' + col.TABLE_SCHEMA + '.' + col.TABLE_NAME)
-                JOIN sys.index_columns indc
-                	ON ind.index_id = indc.index_id
-                		AND ind.object_id = indc.object_id
-                		AND indc.column_id = col.ORDINAL_POSITION
-                WHERE col.TABLE_SCHEMA = ?
-                    AND col.TABLE_NAME = ?
-                	AND ind.name = ?
+                FROM sys.indexes ind
+                    JOIN sys.index_columns indc
+                        ON ind.index_id = indc.index_id
+                        AND ind.object_id = indc.object_id
+                    JOIN sys.columns col 
+                        ON indc.object_id = col.object_id 
+                        AND indc.column_id = col.column_id 
+                    JOIN sys.tables t 
+                        ON ind.object_id = t.object_id 
+                    JOIN sys.schemas s
+                        ON t.schema_id = s.schema_id
+                WHERE s.name = ?
+                    AND t.name = ?
+                    AND ind.name = ?
                 ORDER BY indc.key_ordinal ASC
 
-object_dependencies = SELECT
+object_dependencies =   SET NOCOUNT ON
+                        -- Variables
+                        DECLARE @komp TABLE(nimi varchar(255), database_name varchar(255), schema_name varchar(255), object_name varchar(255))
+                        DECLARE @dep TABLE(referenced_database_name varchar(255), referenced_schema_name varchar(255), referenced_entity_name varchar(255))
+                        DECLARE @target TABLE(nimi varchar(255), database_name varchar(255), schema_name varchar(255), object_name varchar(255))
+                        DECLARE @links TABLE(source varchar(255), target varchar(255))
+
+                        -- Insert target data to @komp
+                        INSERT INTO @komp (nimi, database_name, schema_name, object_name)
+                        SELECT 
+                            s.name + '.' + o.name as nimi,
+                            '{0}' as database_name,
+                            s.name as schema_name,
+                            o.name as object_name
+                        FROM [{0}].sys.objects o
+                        JOIN [{0}].sys.schemas s 
+                            ON o.schema_id = s.schema_id
+                        WHERE is_ms_shipped = 0 AND o.type in ('U','V','P','FN','IF','TF','PC','TR')
+
+                        -- Loop through targets in @komp
+                        WHILE EXISTS (SELECT 1 FROM @komp)
+                        BEGIN
+
+                            DELETE FROM @target
+
+                            INSERT INTO @target
+                            SELECT TOP(1) nimi, database_name, schema_name, object_name
+                            FROM @komp
+
+                            DELETE FROM @komp
+                            WHERE nimi = (SELECT nimi from @target)
+
+                            BEGIN TRY
+                                INSERT INTO @links
+                                SELECT
+                                    ISNULL(dep.referenced_database_name, '{0}') + '.' + ISNULL(dep.referenced_schema_name, 'dbo') + '.' + referenced_entity_name as [source]
+                                    ,komp.database_name + '.' + komp.schema_name + '.' + komp.object_name as [target]
+                                FROM @target komp
+                                CROSS APPLY [{0}].sys.dm_sql_referenced_entities (komp.nimi, 'OBJECT') dep
+                                WHERE referenced_minor_name IS NULL
+                            END TRY
+                            BEGIN CATCH
+                            END CATCH
+
+                        END
+
+                        SELECT
                         source,
                         target
-                      FROM (
-                          SELECT
-                                ISNULL(dep.referenced_database_name, '{0}') + '.' + ISNULL(dep.referenced_schema_name, 'dbo') + '.' + referenced_entity_name as [source]
-                                ,komp.database_name + '.' + komp.schema_name + '.' + komp.object_name as [target]
-                          FROM (
-                              SELECT 
-                          	      s.name + '.' + o.name as nimi,
-                          	      '{0}' as database_name,
-                          	      s.name as schema_name,
-                          	      o.name as object_name
-                              FROM [{0}].sys.objects o
-                              JOIN [{0}].sys.schemas s 
-                          	      ON o.schema_id = s.schema_id
-                              WHERE is_ms_shipped = 0 AND o.type in ('U','V','P','FN','IF','TF','PC','TR')
-                              ) as komp
-                          CROSS APPLY [{0}].sys.dm_sql_referenced_entities (komp.nimi, 'OBJECT') dep
-                          WHERE dep.referenced_minor_name is null
-                      ) links
-                      WHERE links.target = ? OR links.source = ?
+                        FROM @links
+                        WHERE target = ? OR source = ?
```

## Comparing `palje-2.1.0.dist-info/LICENSE` & `palje-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `palje-2.1.0.dist-info/METADATA` & `palje-2.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palje
-Version: 2.1.0
+Version: 2.2.0
 Summary: A tool for creating hierarchical documentation of SQL Server databases to Confluence wiki.
 Author: ALM Partners Oy
 Maintainer: ALM Partners Oy
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,15 +214,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azure-identity ~=1.14
 Requires-Dist: sqlalchemy[mssql] ~=2.0.29
-Requires-Dist: requests ~=2.31.0
+Requires-Dist: requests ~=2.32
 Provides-Extra: msibuild
 Requires-Dist: cx-freeze ~=7.0.0 ; extra == 'msibuild'
 Provides-Extra: test
 Requires-Dist: tox ~=4.15 ; extra == 'test'
 
 Palje
 ====================
@@ -250,14 +250,16 @@
 ```
 cd .\palje
 pip install [-e] .
 ```
 
 # Usage
 
+Palje can be used either from the command line (CLI) or from the graphical user interface (GUI).
+
 ## Prerequisites
 
 - Read access to the MSSQL database you wish to document
     - Data is read from documented database, information schema and system views
     - You can use either SQL authentication or Windows authentication (if available)
 
 - Write access to Confluence space on which you wish to create the documentation pages
@@ -274,14 +276,28 @@
 - Palje has been tested on multiple SQL Server versions, including [SQL Server images](https://hub.docker.com/_/microsoft-mssql-server)
 - Palje has been tested on cloud instances, such as Azure SQL Database
     - Palje supports Azure Active Directory authentication with argument --authentication "AAD"
 - Palje has been tested to work with Confluence Cloud
     - There is a possibility that Palje works with Confluence Server since the Server REST API is similar to Cloud REST API
     - Notice that the authentication works differently in Confluence Server
 
+## Graphical user-interface
+
+Notice that GUI may be lacking some of the more advanced features that are available via CLI.
+
+![Page hierarchy in Confluence](./images/palje_gui.PNG?raw=true)
+
+Launch Palje GUI from a shell with command:
+
+```
+palje-gui
+```
+
+See the CLI documentation below for information on various parameters - it all applies to GUI, too.
+
 ## CLI and arguments
 
 See online help for up-to-date documentation for available options.
 ```
 palje -h
 ```
 
@@ -306,15 +322,17 @@
 | schemas | No | Names of the schemas that are documented | list of str | If schemas not given, all schemas will be documented |
 | dependent | No | Names of the databases, where object dependencies are sought | list of str | If databases not given, dependencies are sought only in documented database |
 | db-driver | No | Name of the database driver | str | "ODBC Driver 17 for SQL Server" |
 | authentication | No | Authentication method to use. Options are "SQL", "Windows", "AAD" and "AzureIdentity". | str | "SQL"
  
 
 ## Usage example
-### Command
+
+
+### Command-line interface
 ```
 # Run via a configured script endpoint ("palje.exe")
 palje "https://<your-org>.atlassian.net/" TEST "localhost,1433" MY_DB --schemas dbo store --dependent MY_OTHER_DB --authentication "SQL"
 
 # Optionally you also run palje as a Python library module
 python -m palje "https://<your-org>.atlassian.net/" TEST "localhost,1433" MY_DB --schemas dbo store --dependent MY_OTHER_DB --authentication "SQL"
```

