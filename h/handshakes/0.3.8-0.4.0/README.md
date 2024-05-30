# Comparing `tmp/handshakes-0.3.8.tar.gz` & `tmp/handshakes-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handshakes-0.3.8.tar", max compression
+gzip compressed data, was "handshakes-0.4.0.tar", max compression
```

## Comparing `handshakes-0.3.8.tar` & `handshakes-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      749 2024-05-21 06:44:30.233990 handshakes-0.3.8/README.md
--rw-r--r--   0        0        0      448 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/.version
--rw-r--r--   0        0        0       22 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/CommandLine/__init__.py
--rw-r--r--   0        0        0     8485 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/CommandLine/_init.py
--rw-r--r--   0        0        0     4326 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/CommandLine/center.py
--rw-r--r--   0        0        0       15 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/__init__.py
--rw-r--r--   0        0        0     3107 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/lifecycle.py
--rw-r--r--   0        0        0     4234 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/migrator.py
--rw-r--r--   0        0        0      570 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/__init__.py
--rw-r--r--   0        0        0      939 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/attachmentBase.py
--rw-r--r--   0        0        0     2034 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/config_base.py
--rw-r--r--   0        0        0     1618 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/dynamic_base.py
--rw-r--r--   0        0        0     1010 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/enums.py
--rw-r--r--   0        0        0     5833 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/result_base.py
--rw-r--r--   0        0        0     1167 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/static_base.py
--rw-r--r--   0        0        0     2102 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/models/types.py
--rw-r--r--   0        0        0       50 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/sanic_free_shared.py
--rw-r--r--   0        0        0      221 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/bump-v5.sql
--rw-r--r--   0        0        0      369 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/bump-v6.sql
--rw-r--r--   0        0        0      407 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/revert-v4.sql
--rw-r--r--   0        0        0       99 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/revert-v6.sql
--rw-r--r--   0        0        0      452 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/scripts/revert-v7.sql
--rw-r--r--   0        0        0      753 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/DBService/shared.py
--rw-r--r--   0        0        0        0 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/__init__.py
--rw-r--r--   0        0        0     7967 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/coreEndpoints.py
--rw-r--r--   0        0        0     1434 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/utils.py
--rw-r--r--   0        0        0     1956 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/blueprints/writeServices.py
--rw-r--r--   0        0        0      431 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/center.py
--rw-r--r--   0        0        0     1055 2024-05-21 06:44:30.249990 handshakes-0.3.8/handshake/services/Endpoints/core.py
--rw-r--r--   0        0        0      278 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/Endpoints/errorHandling.py
--rw-r--r--   0        0        0      954 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/Endpoints/internalEndpoints.py
--rw-r--r--   0        0        0      128 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/Endpoints/static_server.py
--rw-r--r--   0        0        0     2587 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/README.md
--rw-r--r--   0        0        0        0 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/__init__.py
--rw-r--r--   0        0        0     9654 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/completeTestRun.py
--rw-r--r--   0        0        0      875 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/constants.py
--rw-r--r--   0        0        0     4562 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/handlePending.py
--rw-r--r--   0        0        0     1635 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/handleTestResults.py
--rw-r--r--   0        0        0     8216 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/modifySuites.py
--rw-r--r--   0        0        0     1867 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/pruneTasks.py
--rw-r--r--   0        0        0      666 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/refer_types.py
--rw-r--r--   0        0        0     1653 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/register.py
--rw-r--r--   0        0        0    19555 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/SchedularService/start.py
--rw-r--r--   0        0        0        0 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/__init__.py
--rw-r--r--   0        0        0      193 2024-05-21 06:44:30.253990 handshakes-0.3.8/handshake/services/starter.py
--rw-r--r--   0        0        0     1576 2024-05-21 06:44:30.253990 handshakes-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 handshakes-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      749 2024-05-30 18:59:15.797668 handshakes-0.4.0/README.md
+-rw-r--r--   0        0        0      448 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/.version
+-rw-r--r--   0        0        0       22 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/CommandLine/__init__.py
+-rw-r--r--   0        0        0     8551 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/CommandLine/_init.py
+-rw-r--r--   0        0        0     4447 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/CommandLine/center.py
+-rw-r--r--   0        0        0       34 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/__init__.py
+-rw-r--r--   0        0        0     3107 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/lifecycle.py
+-rw-r--r--   0        0        0     6103 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/migrator.py
+-rw-r--r--   0        0        0      604 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/__init__.py
+-rw-r--r--   0        0        0      939 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/attachmentBase.py
+-rw-r--r--   0        0        0     2793 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/config_base.py
+-rw-r--r--   0        0        0     1618 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/dynamic_base.py
+-rw-r--r--   0        0        0     1211 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/enums.py
+-rw-r--r--   0        0        0     5833 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/result_base.py
+-rw-r--r--   0        0        0     1167 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/static_base.py
+-rw-r--r--   0        0        0     2102 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/models/types.py
+-rw-r--r--   0        0        0       50 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/sanic_free_shared.py
+-rw-r--r--   0        0        0      221 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/scripts/bump-v5.sql
+-rw-r--r--   0        0        0      369 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/scripts/bump-v6.sql
+-rw-r--r--   0        0        0       99 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/scripts/revert-v6.sql
+-rw-r--r--   0        0        0      452 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/scripts/revert-v7.sql
+-rw-r--r--   0        0        0      753 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/DBService/shared.py
+-rw-r--r--   0        0        0        0 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/Endpoints/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/Endpoints/blueprints/__init__.py
+-rw-r--r--   0        0        0     9848 2024-05-30 18:59:15.813668 handshakes-0.4.0/handshake/services/Endpoints/blueprints/coreEndpoints.py
+-rw-r--r--   0        0        0     1434 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/blueprints/utils.py
+-rw-r--r--   0        0        0     2233 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/blueprints/writeServices.py
+-rw-r--r--   0        0        0      431 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/center.py
+-rw-r--r--   0        0        0      692 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/core.py
+-rw-r--r--   0        0        0      246 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/define_api.py
+-rw-r--r--   0        0        0      278 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/errorHandling.py
+-rw-r--r--   0        0        0      954 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/internalEndpoints.py
+-rw-r--r--   0        0        0      128 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/Endpoints/static_server.py
+-rw-r--r--   0        0        0     2587 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/__init__.py
+-rw-r--r--   0        0        0     9654 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/completeTestRun.py
+-rw-r--r--   0        0        0      875 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/constants.py
+-rw-r--r--   0        0        0     4562 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/handlePending.py
+-rw-r--r--   0        0        0     1635 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/handleTestResults.py
+-rw-r--r--   0        0        0     8216 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/modifySuites.py
+-rw-r--r--   0        0        0     1867 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/pruneTasks.py
+-rw-r--r--   0        0        0      666 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/refer_types.py
+-rw-r--r--   0        0        0     1653 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/register.py
+-rw-r--r--   0        0        0    19555 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/SchedularService/start.py
+-rw-r--r--   0        0        0        0 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-30 18:59:15.817668 handshakes-0.4.0/handshake/services/starter.py
+-rw-r--r--   0        0        0     1544 2024-05-30 18:59:15.817668 handshakes-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 handshakes-0.4.0/PKG-INFO
```

### Comparing `handshakes-0.3.8/README.md` & `handshakes-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/CommandLine/_init.py` & `handshakes-0.4.0/handshake/services/CommandLine/_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,20 @@
     secho,
     version_option,
     pass_context,
     Context,
     Path as C_Path,
 )
 from handshake import __version__
-from handshake.services.DBService.migrator import check_version, migration, DB_VERSION
+from handshake.services.DBService.migrator import (
+    check_version,
+    migration,
+    DB_VERSION,
+    MigrationTrigger,
+)
 from handshake.services.SchedularService.start import Scheduler
 from handshake.services.SchedularService.handleTestResults import (
     setConfig,
 )
 from loguru import logger
 import json
 from handshake.services.DBService.lifecycle import config_file, close_connection
@@ -75,15 +80,15 @@
         )
     return True
 
 
 @general_requirement
 @handle_cli.command()
 def db_version(collection_path):
-    return check_version(db_path(collection_path))
+    return check_version(path=db_path(collection_path))
 
 
 @handle_cli.command(
     short_help="checks the version of the sqlite3 installed in your system"
 )
 def check_sqlite():
     assert int(sqlite_version_info[0]) >= 3, "Required version is >= 3."
@@ -96,15 +101,15 @@
 @general_requirement
 @handle_cli.command(
     short_help="Migrates the database to the latest version as per the handshake executable.",
     help="it's a command to execute the required migration scripts, note; this command would be executed "
     "automatically whenever we run patch or run-app command",
 )
 def migrate(collection_path: str):
-    return migration(db_path(collection_path))
+    return migration(db_path(collection_path), MigrationTrigger.CLI)
 
 
 @handle_cli.command(
     short_help="Processes the collected results and even could export the test results",
     help="runs an async loop, schedules some tasks to patch some your test results "
     "so you can see it in the way we need. you can pass the output directory to generate the report",
 )
```

### Comparing `handshakes-0.3.8/handshake/services/CommandLine/center.py` & `handshakes-0.4.0/handshake/services/CommandLine/center.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from handshake.services.CommandLine._init import (
     handle_cli,
     general_but_optional_requirement,
-    version_option,
     observed_version,
     break_if_mismatch,
 )
 from handshake.services.Endpoints.center import service_provider
 from handshake.services.DBService.lifecycle import (
     init_tortoise_orm,
     close_connection,
@@ -118,36 +117,44 @@
 @handle_cli.command(
     help="serves the generated reports. simply serves the static files generated in your directory mentioned "
     "in static_path",
     short_help="serves generated report",
 )
 @argument("STATIC_PATH", nargs=1, required=False, type=Path(exists=True, dir_okay=True))
 @option(
+    "-h",
+    "--host",
+    default="localhost",
+    show_default=True,
+    help="Host for the reports to be displayed at",
+    type=str,
+)
+@option(
     "-p",
     "--port",
     default=8000,
     show_default=True,
-    help="Port for the service to connect to",
+    help="At this port you reports would be displayed",
     type=int,
 )
 def display(
-    version: Union[bool, str] = False,
     static_path: Union[str, P_Path] = "TestReports",
     port: int = 8000,
+    host: str = "localhost",
 ):
     if static_path:
         static_path = P_Path(static_path)
 
         if not static_path.exists():
             raise NotADirectoryError(f"{static_path} does not exist")
 
     loader = AppLoader(factory=partial(feed_static_provider, static_path))
     _app = loader.load()
     _app.prepare(
-        host="127.0.0.1",
+        host=host,
         port=port,
         access_log=False,
         motd_display=dict(version=__version__),
     )
     Sanic.serve(primary=_app, app_loader=loader)
```

### Comparing `handshakes-0.3.8/handshake/services/DBService/lifecycle.py` & `handshakes-0.4.0/handshake/services/DBService/lifecycle.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/DBService/models/attachmentBase.py` & `handshakes-0.4.0/handshake/services/DBService/models/attachmentBase.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/DBService/models/config_base.py` & `handshakes-0.4.0/handshake/services/DBService/models/config_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-from handshake.services.DBService.models.enums import ConfigKeys
+from handshake.services.DBService.models.enums import (
+    ConfigKeys,
+    MigrationStatus,
+    MigrationTrigger,
+)
 from tortoise.fields import IntField
 from handshake.services.DBService.models.result_base import RunBase
 from tortoise.models import Model
 from tortoise.fields import (
     CharEnumField,
     ForeignKeyField,
     ForeignKeyRelation,
     TextField,
     UUIDField,
     BooleanField,
     JSONField,
+    DatetimeField,
 )
 
 
 class ConfigBase(Model):
     key = CharEnumField(
         ConfigKeys, pk=True, null=False, description="Type of job we would like to run"
     )
@@ -56,7 +61,32 @@
         description="if > 0 then it means that run would stop if it finds this number of test cases failed",
     )
     tags = JSONField(
         default=[],
         null=False,
         description="comma separated list of tags (used by framework) to filter the spec files",
     )
+
+
+class MigrationBase(Model):
+    modified = DatetimeField(auto_now=True)  # use modified timestamp
+    fromVersion = IntField(
+        null=False,
+        default=0,
+        description="migrated from",
+    )
+    toVersion = IntField(
+        null=False,
+        default=0,
+        description="migrated to",
+    )
+    status = CharEnumField(
+        MigrationStatus,
+        description="status of the migration",
+        default=MigrationStatus.PENDING,
+    )
+    trigger = CharEnumField(
+        MigrationTrigger,
+        description="status of the migration",
+        default=MigrationTrigger.AUTOMATIC,
+    )
+    error = TextField(null=True, default="", description="Error if any")
```

### Comparing `handshakes-0.3.8/handshake/services/DBService/models/dynamic_base.py` & `handshakes-0.4.0/handshake/services/DBService/models/dynamic_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/DBService/models/enums.py` & `handshakes-0.4.0/handshake/services/DBService/models/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 from enum import StrEnum
+from typing import Tuple
 
 
-class Status(StrEnum):
+class MigrationStatus(StrEnum):
     PASSED = "PASSED"
-    SKIPPED = "SKIPPED"
+    PENDING = "PENDING"
     FAILED = "FAILED"
+
+
+class MigrationTrigger(StrEnum):
+    AUTOMATIC = "AUTO"
+    CLI = "CLI"
+
+
+class Status(StrEnum):
+    PASSED = "PASSED"
     PENDING = "PENDING"
+    FAILED = "FAILED"
+    SKIPPED = "SKIPPED"
     YET_TO_CALCULATE = (
         "YET_TO_CALC"  # needs to be updated by our server to either passed or failed
     )
     # yet_to_calc is mostly seen for the suite
     RETRIED = "RETRIED"
```

### Comparing `handshakes-0.3.8/handshake/services/DBService/models/result_base.py` & `handshakes-0.4.0/handshake/services/DBService/models/result_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/DBService/models/static_base.py` & `handshakes-0.4.0/handshake/services/DBService/models/static_base.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/DBService/models/types.py` & `handshakes-0.4.0/handshake/services/DBService/models/types.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/DBService/shared.py` & `handshakes-0.4.0/handshake/services/DBService/shared.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/Endpoints/blueprints/coreEndpoints.py` & `handshakes-0.4.0/handshake/services/Endpoints/blueprints/coreEndpoints.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,21 +14,26 @@
     attachWarn,
     extractPydanticErrors,
 )
 from handshake.services.DBService.models.static_base import (
     AttachmentBase,
     AttachmentType,
 )
+from handshake.services.Endpoints.define_api import definition
 from handshake.services.DBService.models.config_base import TestConfigBase
 from handshake.services.DBService.models.attachmentBase import AssertBase
-from handshake.services.DBService.models.enums import Status, SuiteType
+from handshake.services.DBService.models.enums import (
+    Status,
+    SuiteType,
+)
 from handshake.services.DBService.models.static_base import StaticBase
 from sanic.blueprints import Blueprint
 from sanic.response import JSONResponse, text, HTTPResponse
 from loguru import logger
+from typing import List
 from sanic.request import Request
 from handshake.services.DBService.shared import get_test_id
 from handshake.services.SchedularService.register import register_patch_suite
 from pydantic import ValidationError
 from dotenv import load_dotenv
 from handshake.services.DBService.lifecycle import attachment_folder, db_path
 
@@ -45,14 +50,20 @@
 
     payload = extractPayload(request, response)
     await attachError(payload, request.url)
     return JSONResponse(body=payload, status=response.status)
 
 
 @service.put("/registerSession")
+@definition(
+    summary="Registers a Session",
+    description="Registers a session with state datetime on the currently running Test Run.",
+    tag="register",
+    body={"application/json": RegisterSession.model_json_schema()},
+)
 async def register_session(request: Request) -> HTTPResponse:
     try:
         session = RegisterSession.model_validate(request.json)
         session_record = await SessionBase.create(
             **session.model_dump(), test_id=get_test_id()
         )
         await session_record.save()
@@ -60,23 +71,36 @@
         logger.error("Failed to create a session due to exception: {}", str(error))
         return text(str(error), status=404)
 
     return text(str(session_record.sessionID), status=201)
 
 
 @service.put("/registerSuite")
+@definition(
+    summary="Registers a Suite under a session",
+    description="Registers a suite/test with provided meta details of suite/test and session id",
+    tag="register",
+    body={"application/json": RegisterSuite},
+)
 async def register_suite(request: Request) -> HTTPResponse:
     suite = RegisterSuite.model_validate(request.json)
     suite_record = await SuiteBase.create(**suite.model_dump())
     await suite_record.save()
 
     return text(str(suite_record.suiteID), status=201)
 
 
 @service.put("/updateSuite", error_format="json")
+@definition(
+    summary="Updates the suite past the test suite's execution",
+    description="Once the Test suite/test gets executed, through this endpoint "
+    "we would updates its status and timings on the registered suite/test",
+    tag="update",
+    body={"application/json": MarkSuite.model_json_schema()},
+)
 async def updateSuite(request: Request) -> HTTPResponse:
     suite = MarkSuite.model_validate(request.json)
 
     suite_record = await SuiteBase.filter(suiteID=suite.suiteID).first()
     if not suite_record:
         logger.error("Was not able to found {} suite", str(suite.suiteID))
         return text(f"Suite {suite.suiteID} was not found", status=404)
@@ -99,27 +123,41 @@
 
     return text(
         f"Suite: {suite_record.title} - {suite_record.suiteID} was updated", status=201
     )
 
 
 @service.put("/updateSession", error_format="json")
+@definition(
+    summary="Updates the session past the test session's execution",
+    description="Once the Test session gets executed, through this endpoint "
+    "we would updates its status and timings on the registered session",
+    tag="update",
+    body={"application/json": MarkSession.model_json_schema()},
+)
 async def update_session(request: Request) -> HTTPResponse:
     session = MarkSession.model_validate(request.json)
     test_session = await SessionBase.filter(sessionID=session.sessionID).first()
     if not test_session:
         logger.error("Expected {} session was not found", str(session.sessionID))
         return text(f"Session {session.sessionID} was not found", status=404)
 
     await test_session.update_from_dict(session.model_dump())
     await test_session.save()
     return text(f"{session.sessionID} was updated", status=201)
 
 
 @service.put("/addAttachmentsForEntities")
+@definition(
+    summary="adds multiple attachments to the specified entities",
+    description="provide the list of attachments (assertion/link/description) as mentioned in the body, "
+    "and attachments would be inserted in their respective tables",
+    tag="add",
+    body={"application/json": List[AddAttachmentForEntity]},
+)
 async def addAttachmentForEntity(request: Request) -> HTTPResponse:
     attachments = []
     note = []
     assertions = []
 
     for _ in request.json:
         try:
@@ -196,14 +234,20 @@
     await test.save()
     await config.save()
 
     return text("provided config was saved successfully.", status=200)
 
 
 @service.put("/registerAWrittenAttachment", error_format="json")
+@definition(
+    summary="Attach an Images to the specified entity",
+    description="Writes an attachment inside of our Attachments folder, and attaches it with the specified entity",
+    tag="add",
+    body={"application/json": WrittenAttachmentForEntity},
+)
 async def saveImage(request: Request) -> HTTPResponse:
     attachment = WrittenAttachmentForEntity.model_validate(request.json)
     record = await StaticBase.create(
         entity_id=attachment.entityID,
         description=attachment.description,
         type=attachment.type,
     )
@@ -212,9 +256,15 @@
         dict(
             attachmentValue=dict(value=file_name, title=attachment.title),
         )
     )
     await record.save()
     # we can save the file in this request itself, but no. we let the framework's custom reporter cook.
     return text(
-        str(attachment_folder(db_path()) / get_test_id() / file_name), status=201
+        str(
+            attachment_folder(db_path())
+            / get_test_id()
+            / str(attachment.entityID)
+            / file_name
+        ),
+        status=201,
     )
```

### Comparing `handshakes-0.3.8/handshake/services/Endpoints/blueprints/utils.py` & `handshakes-0.4.0/handshake/services/Endpoints/blueprints/utils.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/Endpoints/blueprints/writeServices.py` & `handshakes-0.4.0/handshake/services/Endpoints/blueprints/writeServices.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,32 +8,37 @@
 )
 from handshake.services.DBService.shared import root_dir
 from handshake.services.DBService.models.static_base import (
     StaticBase,
 )
 from handshake.services.SchedularService.constants import writtenAttachmentFolderName
 from handshake.services.Endpoints.blueprints.utils import extractPayload, attachWarn
+from handshake.services.Endpoints.define_api import definition
 
 writeServices = Blueprint("WriteService", url_prefix="/write")
 
 
 @writeServices.on_response
 async def handle_response(request: Request, response: JSONResponse):
     if 200 <= response.status < 300:
         return response
 
     payload = extractPayload(request, response)
     await attachWarn(payload, request.url)
     return JSONResponse(body=payload, status=response.status)
 
 
-# NOTE: depreciated
-
-
 @writeServices.put("/addAttachmentForEntity", error_format="json")
+@definition(
+    summary="adds an image to the specified entity",
+    description="saves an image and then attaches it to a specified entity",
+    tag="add",
+    deprecated=True,
+    body={"application/json": AddAttachmentForEntity},
+)
 async def saveImage(request: Request) -> HTTPResponse:
     attachment = AddAttachmentForEntity.model_validate(request.json)
 
     record = await StaticBase.create(
         entity_id=attachment.entityID,
         description=attachment.description,
         type=attachment.type,
```

### Comparing `handshakes-0.3.8/handshake/services/Endpoints/internalEndpoints.py` & `handshakes-0.4.0/handshake/services/Endpoints/internalEndpoints.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/README.md` & `handshakes-0.4.0/handshake/services/SchedularService/README.md`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/completeTestRun.py` & `handshakes-0.4.0/handshake/services/SchedularService/completeTestRun.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/constants.py` & `handshakes-0.4.0/handshake/services/SchedularService/constants.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/handlePending.py` & `handshakes-0.4.0/handshake/services/SchedularService/handlePending.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/handleTestResults.py` & `handshakes-0.4.0/handshake/services/SchedularService/handleTestResults.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/modifySuites.py` & `handshakes-0.4.0/handshake/services/SchedularService/modifySuites.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/pruneTasks.py` & `handshakes-0.4.0/handshake/services/SchedularService/pruneTasks.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/refer_types.py` & `handshakes-0.4.0/handshake/services/SchedularService/refer_types.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/register.py` & `handshakes-0.4.0/handshake/services/SchedularService/register.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/handshake/services/SchedularService/start.py` & `handshakes-0.4.0/handshake/services/SchedularService/start.py`

 * *Files identical despite different names*

### Comparing `handshakes-0.3.8/pyproject.toml` & `handshakes-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "handshakes"
-version = "0.3.8"
+version = "0.4.0"
 description = "A service that's keen to process your test results"
 authors = ["Rahul <saihanumarahul66@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "handshake"}]
 maintainers = [
     "Rahul <saihanumarahul66@gmail.com>"
@@ -24,25 +24,25 @@
 pydantic = "^2.4.2"
 sanic = "^23.6.0"
 tortoise-orm = "^0.20.0"
 click = "^8.1.7"
 loguru = "^0.7.2"
 httpx = "^0.26.0"
 python-dotenv = "^1.0.1"
-sentry-sdk = {extras = ["sanic"], version = "^1.40.4"}
 setuptools = "^69.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 pytest-asyncio = "^0.21.1"
 sanic-testing = "^23.6.0"
 psutil = "^5.9.5"
 black = ">=23.9.1,<25.0.0"
 virtualenv = "^20.25.1"
 requests = "^2.31.0"
+sanic-ext = "^23.12.0"
 
 [tool.poetry.extras]
 excel-export = ["openpyxl"]
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `handshakes-0.3.8/PKG-INFO` & `handshakes-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handshakes
-Version: 0.3.8
+Version: 0.4.0
 Summary: A service that's keen to process your test results
 License: MIT
 Author: Rahul
 Author-email: saihanumarahul66@gmail.com
 Maintainer: Rahul
 Maintainer-email: saihanumarahul66@gmail.com
 Requires-Python: >=3.11,<3.13
@@ -19,15 +19,14 @@
 Provides-Extra: excel-export
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: sanic (>=23.6.0,<24.0.0)
-Requires-Dist: sentry-sdk[sanic] (>=1.40.4,<2.0.0)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0)
 Requires-Dist: tortoise-orm (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Handshake 🫱🏾‍🫲🏼
 _A Modern Test Reporter_
```

