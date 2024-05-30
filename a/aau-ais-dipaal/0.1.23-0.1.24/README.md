# Comparing `tmp/aau_ais_dipaal-0.1.23.tar.gz` & `tmp/aau_ais_dipaal-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_dipaal-0.1.23.tar", last modified: Thu May 16 07:03:42 2024, max compression
+gzip compressed data, was "aau_ais_dipaal-0.1.24.tar", last modified: Thu May 30 14:53:58 2024, max compression
```

## Comparing `aau_ais_dipaal-0.1.23.tar` & `aau_ais_dipaal-0.1.24.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0        0        0      130 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/README.md
--rw-r--r--   0        0        0      713 2024-05-16 07:03:42.525052 aau_ais_dipaal-0.1.23/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/__init__.py
--rw-r--r--   0        0        0      237 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/__init__.py
--rw-r--r--   0        0        0     1161 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/callsign.py
--rw-r--r--   0        0        0     1546 2024-05-16 05:24:21.673162 aau_ais_dipaal-0.1.23/src/dipaal/convert/converter.py
--rw-r--r--   0        0        0     1132 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/imo.py
--rw-r--r--   0        0        0     1142 2024-04-29 11:43:36.000000 aau_ais_dipaal-0.1.23/src/dipaal/convert/mmsi.py
--rw-r--r--   0        0        0        0 2024-05-03 12:25:02.814192 aau_ais_dipaal-0.1.23/src/dipaal/export/__init__.py
--rw-r--r--   0        0        0     8050 2024-05-03 14:00:48.480144 aau_ais_dipaal-0.1.23/src/dipaal/export/map_exporter.py
--rw-r--r--   0        0        0     6170 2024-05-16 06:59:44.399530 aau_ais_dipaal-0.1.23/src/dipaal/export/sql_map.py
--rw-r--r--   0        0        0       52 2024-05-16 05:47:45.666615 aau_ais_dipaal-0.1.23/src/dipaal/list/__init__.py
--rw-r--r--   0        0        0     1598 2024-05-16 06:07:58.761276 aau_ais_dipaal-0.1.23/src/dipaal/list/lister.py
--rw-r--r--   0        0        0       50 2024-05-16 05:38:16.272469 aau_ais_dipaal-0.1.23/src/dipaal/list/sql/enc.sql
--rw-r--r--   0        0        0        0 2024-05-16 05:27:13.493857 aau_ais_dipaal-0.1.23/src/dipaal/list/sql/ship_type.sql
--rw-r--r--   0        0        0      124 2024-05-14 11:53:55.399670 aau_ais_dipaal-0.1.23/src/dipaal/load/__init__.py
--rw-r--r--   0        0        0     4751 2024-05-14 19:29:40.057506 aau_ais_dipaal-0.1.23/src/dipaal/load/loader.py
--rw-r--r--   0        0        0     2026 2024-05-14 11:53:55.400692 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/02.load.fact_depth_50m.sql
--rw-r--r--   0        0        0     2556 2024-05-14 11:53:55.401684 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/04.update.confidence.fact_depth_50m.sql
--rw-r--r--   0        0        0     1973 2024-05-14 11:53:55.402694 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/06.load.fact_raster_confidence.sql
--rw-r--r--   0        0        0      976 2024-05-14 12:45:57.777054 aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/08.load.fact_raster_confidence_month.sql
--rw-r--r--   0        0        0     1118 2024-05-14 11:53:55.403671 aau_ais_dipaal-0.1.23/src/dipaal/settings.py
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.23/PKG-INFO
+-rw-r--r--   0        0        0      144 2024-05-22 06:37:27.033402 aau_ais_dipaal-0.1.24/README.md
+-rw-r--r--   0        0        0      713 2024-05-30 14:53:58.283578 aau_ais_dipaal-0.1.24/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 08:35:14.351270 aau_ais_dipaal-0.1.24/src/dipaal/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-22 06:45:45.843293 aau_ais_dipaal-0.1.24/src/dipaal/convert/__init__.py
+-rw-r--r--   0        0        0     1332 2024-05-22 06:46:16.541130 aau_ais_dipaal-0.1.24/src/dipaal/convert/callsign.py
+-rw-r--r--   0        0        0     1550 2024-05-27 13:47:30.020121 aau_ais_dipaal-0.1.24/src/dipaal/convert/converter.py
+-rw-r--r--   0        0        0     1473 2024-05-22 07:20:30.854697 aau_ais_dipaal-0.1.24/src/dipaal/convert/imo.py
+-rw-r--r--   0        0        0     1332 2024-05-22 07:26:16.213158 aau_ais_dipaal-0.1.24/src/dipaal/convert/mmsi.py
+-rw-r--r--   0        0        0      209 2024-05-30 07:00:40.275687 aau_ais_dipaal-0.1.24/src/dipaal/export/__init__.py
+-rw-r--r--   0        0        0     8062 2024-05-27 13:47:30.015555 aau_ais_dipaal-0.1.24/src/dipaal/export/map_exporter.py
+-rw-r--r--   0        0        0     6170 2024-05-27 13:47:30.009797 aau_ais_dipaal-0.1.24/src/dipaal/export/sql/map.py
+-rw-r--r--   0        0        0      183 2024-05-30 07:00:40.276690 aau_ais_dipaal-0.1.24/src/dipaal/extract/__init__.py
+-rw-r--r--   0        0        0     9580 2024-05-30 14:30:20.080154 aau_ais_dipaal-0.1.24/src/dipaal/extract/grid.py
+-rw-r--r--   0        0        0      252 2024-05-30 08:29:39.867519 aau_ais_dipaal-0.1.24/src/dipaal/extract/sql/__init__.py
+-rw-r--r--   0        0        0     2313 2024-05-30 12:50:27.760640 aau_ais_dipaal-0.1.24/src/dipaal/extract/sql/grid_fact_depth.py
+-rw-r--r--   0        0        0      139 2024-05-30 07:00:40.278689 aau_ais_dipaal-0.1.24/src/dipaal/list/__init__.py
+-rw-r--r--   0        0        0     1601 2024-05-30 07:00:40.279697 aau_ais_dipaal-0.1.24/src/dipaal/list/lister.py
+-rw-r--r--   0        0        0       50 2024-05-16 05:38:16.272469 aau_ais_dipaal-0.1.24/src/dipaal/list/sql/enc.sql
+-rw-r--r--   0        0        0        0 2024-05-16 05:27:13.493857 aau_ais_dipaal-0.1.24/src/dipaal/list/sql/ship_type.sql
+-rw-r--r--   0        0        0      124 2024-05-14 11:53:55.399670 aau_ais_dipaal-0.1.24/src/dipaal/load/__init__.py
+-rw-r--r--   0        0        0     7067 2024-05-27 13:47:30.036183 aau_ais_dipaal-0.1.24/src/dipaal/load/loader.py
+-rw-r--r--   0        0        0     2026 2024-05-14 11:53:55.400692 aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/02.load.fact_depth_50m.sql
+-rw-r--r--   0        0        0     2556 2024-05-14 11:53:55.401684 aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/04.update.confidence.fact_depth_50m.sql
+-rw-r--r--   0        0        0     1973 2024-05-14 11:53:55.402694 aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/06.load.fact_raster_confidence.sql
+-rw-r--r--   0        0        0      976 2024-05-14 12:45:57.777054 aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/08.load.fact_raster_confidence_month.sql
+-rw-r--r--   0        0        0     1124 2024-05-22 06:40:59.005801 aau_ais_dipaal-0.1.24/src/dipaal/settings.py
+-rw-r--r--   0        0        0      317 2024-05-30 07:00:40.280686 aau_ais_dipaal-0.1.24/tests/extract/test_cell.py
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.24/PKG-INFO
```

### Comparing `aau_ais_dipaal-0.1.23/pyproject.toml` & `aau_ais_dipaal-0.1.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aau-ais-dipaal"
-version = "0.1.23"
+version = "0.1.24"
 description = "TODO: Add a description of your project."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "aau-ais-utilities==0.1.*",
     "pydantic==2.7.*",
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/convert/callsign.py` & `aau_ais_dipaal-0.1.24/src/dipaal/convert/callsign.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from .converter import Converter
 from sqlalchemy import Engine
+
 from dipaal.settings import get_dipaal_engine
+from .converter import Converter
 
 
 class CallsignConverter(Converter):
     """Convert callsigns to other formats.
 
     This class requires a connection to a database containing the relevant data.
     """
 
     def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
+        """Construct an instance of the CallsignConverter class.
+
+        Args:
+            engine: The database engine to use. Default is the DIPAAL engine.
+        """
         super().__init__(engine)
 
     def to_mmsi(self, callsign: str) -> str:
         """Convert a callsign to an MMSI number.
 
         Args:
             callsign: The callsign to convert.
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/convert/converter.py` & `aau_ais_dipaal-0.1.24/src/dipaal/convert/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """
 
         # TODO: Change the SQL query so that it ignores non-vessels (e.g. ports, etc.).
         #  Currently, the query will return the most recent value for the given input, regardless of the type of vessel.
         #  Meaning that IMO to MMSI might have a MID in the 800 range, which are handheld radios.
         sql_statement = f"SELECT {to_format} FROM {table} WHERE {from_format} = :VALUE ORDER BY ship_id DESC LIMIT 1;"
 
-        result = self.connection.execute(
+        result = self.connection.execute_raw(
             sql=sql_statement,
             params={'VALUE': value}
         ).fetchone()
 
         if result is None:
             raise KeyError(f"No {to_format} found for {from_format} {value}.")
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/convert/imo.py` & `aau_ais_dipaal-0.1.24/src/dipaal/convert/imo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .converter import Converter
 from dipaal.settings import get_dipaal_engine
 from sqlalchemy import Engine
+from aau_ais_utilities.validate import IMOValidator
 
 
 class IMOConverter(Converter):
     """Convert IMO numbers to other formats.
 
     This class requires a connection to a database containing the relevant data.
     """
@@ -17,14 +18,18 @@
 
         Args:
             imo: The IMO number to convert.
 
         Returns:
             The MMSI number.
         """
+        validator = IMOValidator()
+
+        if not validator.validate(imo):
+            raise ValueError(validator.get_last_error()[2])
 
         return self.convert_within_table(
             from_format="imo",
             to_format="mmsi",
             table="public.dim_ship",
             value=imo)
 
@@ -33,13 +38,17 @@
 
         Args:
             imo: The IMO number to convert.
 
         Returns:
             The callsign.
         """
+        validator = IMOValidator()
+        if not validator.validate(imo):
+
+            raise ValueError("Invalid IMO number. Must be a 7-digit number.")
 
         return self.convert_within_table(
             from_format="imo",
             to_format="callsign",
             table="public.dim_ship",
-            value=imo)
+            value=imo)
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/convert/mmsi.py` & `aau_ais_dipaal-0.1.24/src/dipaal/convert/mmsi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .converter import Converter
 from dipaal.settings import get_dipaal_engine
 from sqlalchemy import Engine
-
+from aau_ais_utilities.validate import MMSIValidator
 
 class MMSIConverter(Converter):
     """Convert MMSI numbers to other formats.
 
     This class requires a connection to a database containing the relevant data.
     """
 
@@ -17,14 +17,18 @@
 
         Args:
             mmsi: The MMSI number to convert.
 
         Returns:
             The IMO number.
         """
+        validator = MMSIValidator()
+
+        if not validator.validate(mmsi):
+            raise ValueError(validator.get_last_error()[2])
 
         return self.convert_within_table(
             from_format="mmsi",
             to_format="imo",
             table="public.dim_ship",
             value=mmsi)
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/export/map_exporter.py` & `aau_ais_dipaal-0.1.24/src/dipaal/export/map_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from sqlalchemy import Engine, CursorResult
 from dipaal.settings import get_dipaal_engine
 from aau_ais_utilities.connections import PostgreSQLConnection
 from pydantic import BaseModel, field_validator
 from typing import Optional
 from jinjasql import JinjaSql
-from dipaal.export.sql_map import query_count_ship, query_count_traj, query_draught_month
+from dipaal.export.sql.map import query_count_ship, query_count_traj, query_draught_month
 
 
 class NoDataFoundError(Exception):
     """Raised when there is no data to export."""
 
     def __init__(self, message: str = "No data found for the given parameters"):
         super().__init__(message)
@@ -95,15 +95,15 @@
         SELECT COUNT(*)
         FROM public.enc
         WHERE title = {{enc}}
         """
 
         query, bind_params = self.jsql.prepare_query(initial_query, self.params)
 
-        result = self.connection.execute(
+        result = self.connection.execute_raw(
             sql=query,
             params=bind_params
         )
 
         if int(result.fetchone()[0]) == 0:
             raise ValueNotExistsError(f"ENC '{self.params['ENC']}' does not exist in the database.")
 
@@ -116,15 +116,15 @@
         SELECT COUNT(*)
         FROM public.dim_ship_type
         WHERE ship_type = {{ship_type}}
         """
 
         query, bind_params = self.jsql.prepare_query(initial_query, self.params)
 
-        result = self.connection.execute(
+        result = self.connection.execute_raw(
             sql=query,
             params=bind_params
         )
 
         if int(result.fetchone()[0]) == 0:
             raise ValueNotExistsError(f"Ship type '{self.params['ship_type']}' does not exist in the database.")
 
@@ -137,15 +137,15 @@
 
         self.validate_enc()
         self.validate_ship_type()
 
     def get_file_name(self) -> str:
         """Return the file name for the exported file."""
         file_name = (
-            f"RASTER_{self.params['raster_type']}_"
+            f"DIPAAL_{self.params['raster_type']}_"
             f"DATE_{self.params['start_date']}_{self.params['end_date']}_"
             f"RES_{self.params['resolution']}_"
             f"ENC_{self.params['enc']}_"
             f"CONF_{self.params.get('confidence', '0')}_"
             f"ST_{self.params.get('ship_type', 'all')}_"
             f"MT_{self.params.get('mobile_type', 'all')}"
         )
@@ -207,15 +207,15 @@
         """
         self.set_params(params)
 
         base_query = self.get_query()
 
         query, bind_params = self.jsql.prepare_query(base_query, params)
 
-        result = self.connection.execute(
+        result = self.connection.execute_raw(
             sql=query,
             params=bind_params
         )
 
         return result
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/export/sql_map.py` & `aau_ais_dipaal-0.1.24/src/dipaal/export/sql/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     {% if enc %}
     AND st_intersects(geom,
                   (SELECT st_transform(geom, 3034)
                    FROM public.enc
                    WHERE title = {{enc}}
                    AND country = 'Denmark'))
     {% endif %}
-    
+
     {% if ship_type %}
     AND dst.ship_type = {{ship_type}}
     {% endif %}
 
     GROUP BY cell_x, cell_y, geom, division_id
 ),
 
@@ -216,11 +216,11 @@
 
     from aau_ais_utilities.connections import PostgreSQLConnection
 
     connection = PostgreSQLConnection(engine)
 
     query, bind_params = j.prepare_query(sql, params)
 
-    result = connection.execute(sql=query, params=bind_params)
+    result = connection.execute_raw(sql=query, params=bind_params)
 
     for row in result.fetchall():
         print(row)
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/list/lister.py` & `aau_ais_dipaal-0.1.24/src/dipaal/list/lister.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 import pandas as pd
 from sqlalchemy import Engine
 
 from aau_ais_utilities.connections import PostgreSQLConnection
 from dipaal.settings import get_dipaal_engine
 
-
 class Lister:
     """Class for listing information from tables in the DIPAAL data warehouse.
 
     Each method in this class corresponds to a different table in the DIPAAL data warehouse and returns the
     information from that table as a pandas DataFrame.
     """
 
     def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
+        """Construct an instance of the Lister class.
+
+        Args:
+            engine: The database engine to use. Default is the DIPAAL engine.
+        """
         self.connection = PostgreSQLConnection(engine)
         self.sql_folder = Path(__file__).parent / 'sql'
 
     def list_enc(self) -> pd.DataFrame:
         """Return the ENC table as a pandas DataFrame.
 
         Limit the results to only include data from Denmark as they are the only relevant data for the project.
@@ -29,14 +33,7 @@
 
     def list_ship_type(self) -> pd.DataFrame:
         """Return the ship_type table as a pandas DataFrame.
 
         Note that ship types are paired with a mobile type, such that each ship type appears twice in the table.
         """
         return pd.read_sql("SELECT * FROM public.dim_ship_type", self.connection.engine)
-
-
-if __name__ == '__main__':
-    lister = Lister()
-    # All column names
-    print(lister.list_enc().columns)
-    print(lister.list_ship_type().columns)
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/load/loader.py` & `aau_ais_dipaal-0.1.24/src/dipaal/load/loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """This module contains the Loader class, which is used to load data from the DIPAAL schema into the depth schema."""
+from calendar import monthrange
 from datetime import datetime, timedelta
 from pathlib import Path
-from calendar import monthrange
+from time import sleep
 
 from sqlalchemy import Engine
 from sqlalchemy.exc import SQLAlchemyError
 
 from aau_ais_utilities.connections import PostgreSQLConnection
 from dipaal.settings import get_dipaal_admin_engine
 
 
 class Loader:
     """Base class for DIPAAL loaders."""
 
-    def __init__(self, engine: Engine = get_dipaal_admin_engine(), *, update: bool = False):
+    def __init__(self, engine: Engine = get_dipaal_admin_engine(),
+                 *, skip: bool = False, save_error: bool = False):
+        """Construct an instance of the Loader class.
+
+        Args:
+            engine: The database engine to use. Default is the DIPAAL admin engine.
+            skip: Whether to check and skip loading already loaded data. Default is False.
+            save_error: Whether to save errors to a file instead of raising them. Default is False.
+        """
         self.connection = PostgreSQLConnection(engine)
-        self.update = update
         self.sql_folder = Path(__file__).parent / 'sql'
+        self.skip = skip
+        self.save_error = save_error
 
     def load_depth(
             self,
             start_date: int,
             end_date: int,
             confidence_scores: list = [0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1]
-    ):
+    ) -> None:
         """Load data into the depth schema from the DIPAAL schema.
 
         For the method to work,
          the following tables must exist in the DIPAAL schema and be populated with appropriate data:
             - dim_ship
             - dim_date
             - dim_time
@@ -45,66 +55,104 @@
         """
         min_time = '000000'
         max_time = '235959'
 
         date_range = self._get_date_range(start_date, end_date)
 
         for day in date_range:
-            print(f'Loading data for {day} into the fact_depth_50m table...')
-            self._attempt_sql_execution(
-                sql=Path(self.sql_folder, 'dipaal_to_depth/02.load.fact_depth_50m.sql'),
-                params={'start_date': day, 'end_date': day,
-                        'start_time': min_time, 'end_time': max_time}
-            )
-
-            print(f"Updating confidence in the fact_depth_50m table for {day}...")
-            self._attempt_sql_execution(
-                sql="""CALL depth.update_confidence_depth_01(:start_date, :end_date);""",
-                params={'start_date': day, 'end_date': day}
-            )
+            skip_fact_depth_50m = False
+            skip_fact_raster_cfd = []
+
+            if self.skip:
+                print(f"Testing if some of the load processes for {day} have already been done...")
+                result = self._attempt_sql_execution(
+                    sql="""SELECT EXISTS(SELECT 1 FROM depth.fact_depth_50m WHERE date_id = :day);""",
+                    params={'day': day}
+                ).fetchone()
+
+                if result[0] is True:
+                    skip_fact_depth_50m = True
+
+                for confidence in confidence_scores:
+                    result = self._attempt_sql_execution(
+                        sql="""SELECT EXISTS(SELECT 1 FROM depth.fact_raster_cfd
+                        WHERE date_id = :day AND cfd_gte = :confidence);""",
+                        params={'day': day, 'confidence': confidence}
+                    ).fetchone()
+
+                    if result[0] is True:
+                        skip_fact_raster_cfd.append(confidence)
+
+            if not skip_fact_depth_50m:
+                print(f'Loading data for {day} into the fact_depth_50m table...')
+                self._attempt_sql_execution(
+                    sql=Path(self.sql_folder, 'dipaal_to_depth/02.load.fact_depth_50m.sql'),
+                    params={'start_date': day, 'end_date': day,
+                            'start_time': min_time, 'end_time': max_time}
+                )
+
+                print(f"Updating confidence in the fact_depth_50m table for {day}...")
+                self._attempt_sql_execution(
+                    sql="""CALL depth.update_confidence_depth_01(:start_date, :end_date);""",
+                    params={'start_date': day, 'end_date': day}
+                )
+            else:
+                print(f"Data for {day} already loaded into the fact_depth_50m table. Skipping...")
 
             for confidence in confidence_scores:
+                if confidence in skip_fact_raster_cfd:
+                    print(f"Data for {day} and confidence {confidence} already loaded into the fact_raster_cfd table. "
+                          f"Skipping...")
+                    continue
                 print(f'Loading data for {day} and confidence {confidence} into the fact_raster_cfd table...')
                 self._attempt_sql_execution(
                     sql=Path(self.sql_folder, 'dipaal_to_depth/06.load.fact_raster_confidence.sql'),
                     params={'date_key': day, 'confidence': confidence}
                 )
 
             print(f"Testing if all days in month {day[:6]} have been loaded into the fact_raster_cfd_month table...")
             days_in_month = monthrange(int(day[:4]), int(day[4:6]))[1]
             year = day[:4]
             month = day[4:6]
 
-            result = self.connection.execute(
-                sql="""SELECT count(DISTINCT date_id) FROM depth.fact_raster_cfd 
+            result = self._attempt_sql_execution(
+                sql="""SELECT count(DISTINCT date_id) FROM depth.fact_raster_cfd
                 WHERE EXTRACT(YEAR FROM to_date(date_id::text, 'YYYYMMDD')) = :year
                 AND EXTRACT(MONTH FROM to_date(date_id::text, 'YYYYMMDD')) = :month;""",
                 params={'year': year, 'month': month}
             ).fetchone()
 
             if result[0] == days_in_month:
                 print(f'Loading data for {day} into the fact_raster_cfd_month table...')
                 self._attempt_sql_execution(
                     sql=Path(self.sql_folder, 'dipaal_to_depth/08.load.fact_raster_confidence_month.sql'),
                     params={'start_date': day, 'end_date': day}
                 )
 
-    def _attempt_sql_execution(self, *, sql: str | Path, params: dict):
+    def _attempt_sql_execution(self, *, sql: str | Path, params: dict) -> None:
         """Attempt to execute SQL and raise an exception if it fails."""
-        try:
-            self.connection.execute(
-                sql=sql,
-                params=params
-            )
-        except SQLAlchemyError as e:
-            error = str(e.__dict__['orig'])
-            raise Exception(error)
+        attempt = 0
+        max_attempts = 5
+        while attempt < max_attempts:
+            try:
+                result = self.connection.execute_raw(
+                    sql=sql,
+                    params=params
+                )
+                return result
+            except SQLAlchemyError as e:
+                error = str(e.__dict__['orig'])
+                attempt += 1
+                print(f'Attempt {attempt} failed. Trying again in 5 seconds...')
+                sleep(5)
+            if attempt == max_attempts:
+                raise Exception(error)
 
     @staticmethod
-    def _get_date_range(start_date, end_date):
+    def _get_date_range(start_date: int, end_date: int) -> list:
         """Get a range of dates."""
         date_range = []
         current_date = datetime.strptime(str(start_date), '%Y%m%d')
         while current_date <= datetime.strptime(str(end_date), '%Y%m%d'):
             date_range.append(current_date.strftime('%Y%m%d'))
             current_date += timedelta(days=1)
         return date_range
```

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/02.load.fact_depth_50m.sql` & `aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/02.load.fact_depth_50m.sql`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/04.update.confidence.fact_depth_50m.sql` & `aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/04.update.confidence.fact_depth_50m.sql`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/06.load.fact_raster_confidence.sql` & `aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/06.load.fact_raster_confidence.sql`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/load/sql/dipaal_to_depth/08.load.fact_raster_confidence_month.sql` & `aau_ais_dipaal-0.1.24/src/dipaal/load/sql/dipaal_to_depth/08.load.fact_raster_confidence_month.sql`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.23/src/dipaal/settings.py` & `aau_ais_dipaal-0.1.24/src/dipaal/settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 from sqlalchemy import Engine, create_engine
 
 from aau_ais_utilities.connections import EngineSettings
 
 
 class DIPAALEngineSettings(EngineSettings):
     """Settings for the DIPAAL data warehouse."""
+
     model_config = SettingsConfigDict(env_prefix='DIPAAL_')
 
 
 @lru_cache
 def get_dipaal_engine() -> Engine:
     """Create an Engine object for the DIPAAL data warehouse, with read-only access."""
     return create_engine(DIPAALEngineSettings().url)
 
 
 class DIPAALAdminEngineSettings(EngineSettings):
     """Settings for the DIPAAL data warehouse, with administrative access."""
+
     model_config = SettingsConfigDict(env_prefix='DIPAAL_ADMIN_')
 
+
 @lru_cache
 def get_dipaal_admin_engine() -> Engine:
     """Create an Engine object for the DIPAAL data warehouse, with administrative access.
 
     This engine should be used with caution, as it allows for administrative operations on the DIPAAL data warehouse.
     """
     return create_engine(DIPAALAdminEngineSettings().url)
```

### Comparing `aau_ais_dipaal-0.1.23/PKG-INFO` & `aau_ais_dipaal-0.1.24/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: aau-ais-dipaal
-Version: 0.1.23
+Version: 0.1.24
 Summary: TODO: Add a description of your project.
 Author-Email: Mikael Vind Mikkelsen <mvmi@cs.aau.dk>
 License: MIT
 Requires-Python: ==3.12.*
 Requires-Dist: aau-ais-utilities==0.1.*
 Requires-Dist: pydantic==2.7.*
 Requires-Dist: pydantic-settings==2.2.*
 Requires-Dist: jinjasql==0.1.*
 Requires-Dist: jinja2==3.0.*
 Requires-Dist: pandas==2.2.*
 Description-Content-Type: text/markdown
 
-# Convert Package
+# DIPAAL Package
+This package 
 
 ## Overview
 
+
 ## Usage
 
 ## Dependencies
 
 ## License
 This project is licensed under the terms of the MIT license.
```

