# Comparing `tmp/datagovindia-1.0.0.tar.gz` & `tmp/datagovindia-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagovindia-1.0.0.tar", last modified: Sun Oct  1 07:53:19 2023, max compression
+gzip compressed data, was "datagovindia-1.0.1.tar", last modified: Thu May 30 13:07:45 2024, max compression
```

## Comparing `datagovindia-1.0.0.tar` & `datagovindia-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2023-10-01 07:53:19.732791 datagovindia-1.0.0/
--rw-r--r--   0 adityachhabra   (501) staff       (20)     1106 2023-09-30 12:10:22.000000 datagovindia-1.0.0/LICENSE
--rw-r--r--   0 adityachhabra   (501) staff       (20)    17446 2023-10-01 07:53:19.732524 datagovindia-1.0.0/PKG-INFO
--rw-r--r--   0 adityachhabra   (501) staff       (20)    14538 2023-10-01 07:44:30.000000 datagovindia-1.0.0/README.md
--rw-r--r--   0 adityachhabra   (501) staff       (20)     1913 2023-10-01 07:46:58.000000 datagovindia-1.0.0/pyproject.toml
--rw-r--r--   0 adityachhabra   (501) staff       (20)       38 2023-10-01 07:53:19.732839 datagovindia-1.0.0/setup.cfg
-drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2023-10-01 07:53:19.730232 datagovindia-1.0.0/src/
-drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2023-10-01 07:53:19.731247 datagovindia-1.0.0/src/datagovindia/
--rw-------   0 adityachhabra   (501) staff       (20)    22436 2023-09-30 21:05:13.000000 datagovindia-1.0.0/src/datagovindia/__init__.py
--rw-r--r--   0 adityachhabra   (501) staff       (20)    12150 2023-10-01 07:47:41.000000 datagovindia-1.0.0/src/datagovindia/cli.py
-drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2023-10-01 07:53:19.732244 datagovindia-1.0.0/src/datagovindia.egg-info/
--rw-r--r--   0 adityachhabra   (501) staff       (20)    17446 2023-10-01 07:53:19.000000 datagovindia-1.0.0/src/datagovindia.egg-info/PKG-INFO
--rw-r--r--   0 adityachhabra   (501) staff       (20)      327 2023-10-01 07:53:19.000000 datagovindia-1.0.0/src/datagovindia.egg-info/SOURCES.txt
--rw-r--r--   0 adityachhabra   (501) staff       (20)        1 2023-10-01 07:53:19.000000 datagovindia-1.0.0/src/datagovindia.egg-info/dependency_links.txt
--rw-r--r--   0 adityachhabra   (501) staff       (20)       54 2023-10-01 07:53:19.000000 datagovindia-1.0.0/src/datagovindia.egg-info/entry_points.txt
--rw-r--r--   0 adityachhabra   (501) staff       (20)       73 2023-10-01 07:53:19.000000 datagovindia-1.0.0/src/datagovindia.egg-info/requires.txt
--rw-r--r--   0 adityachhabra   (501) staff       (20)       13 2023-10-01 07:53:19.000000 datagovindia-1.0.0/src/datagovindia.egg-info/top_level.txt
+drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2024-05-30 13:07:45.148368 datagovindia-1.0.1/
+-rw-r--r--   0 adityachhabra   (501) staff       (20)     1106 2024-05-30 12:02:42.000000 datagovindia-1.0.1/LICENSE
+-rw-r--r--   0 adityachhabra   (501) staff       (20)    17403 2024-05-30 13:07:45.148001 datagovindia-1.0.1/PKG-INFO
+-rw-r--r--   0 adityachhabra   (501) staff       (20)    14538 2024-05-30 12:02:42.000000 datagovindia-1.0.1/README.md
+-rw-r--r--   0 adityachhabra   (501) staff       (20)     1859 2024-05-30 12:25:27.000000 datagovindia-1.0.1/pyproject.toml
+-rw-r--r--   0 adityachhabra   (501) staff       (20)       38 2024-05-30 13:07:45.148412 datagovindia-1.0.1/setup.cfg
+drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2024-05-30 13:07:45.142815 datagovindia-1.0.1/src/
+drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2024-05-30 13:07:45.146132 datagovindia-1.0.1/src/datagovindia/
+-rw-r--r--   0 adityachhabra   (501) staff       (20)    24395 2024-05-30 12:58:02.000000 datagovindia-1.0.1/src/datagovindia/__init__.py
+-rw-r--r--   0 adityachhabra   (501) staff       (20)    12348 2024-05-30 13:03:21.000000 datagovindia-1.0.1/src/datagovindia/cli.py
+drwxr-xr-x   0 adityachhabra   (501) staff       (20)        0 2024-05-30 13:07:45.147698 datagovindia-1.0.1/src/datagovindia.egg-info/
+-rw-r--r--   0 adityachhabra   (501) staff       (20)    17403 2024-05-30 13:07:45.000000 datagovindia-1.0.1/src/datagovindia.egg-info/PKG-INFO
+-rw-r--r--   0 adityachhabra   (501) staff       (20)      327 2024-05-30 13:07:45.000000 datagovindia-1.0.1/src/datagovindia.egg-info/SOURCES.txt
+-rw-r--r--   0 adityachhabra   (501) staff       (20)        1 2024-05-30 13:07:45.000000 datagovindia-1.0.1/src/datagovindia.egg-info/dependency_links.txt
+-rw-r--r--   0 adityachhabra   (501) staff       (20)       54 2024-05-30 13:07:45.000000 datagovindia-1.0.1/src/datagovindia.egg-info/entry_points.txt
+-rw-r--r--   0 adityachhabra   (501) staff       (20)       45 2024-05-30 13:07:45.000000 datagovindia-1.0.1/src/datagovindia.egg-info/requires.txt
+-rw-r--r--   0 adityachhabra   (501) staff       (20)       13 2024-05-30 13:07:45.000000 datagovindia-1.0.1/src/datagovindia.egg-info/top_level.txt
```

### Comparing `datagovindia-1.0.0/LICENSE` & `datagovindia-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datagovindia-1.0.0/PKG-INFO` & `datagovindia-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagovindia
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API wrapper for Government of India Open Government Data (OGD) platform data.gov.in
 Author: Abhishek Arora
 Author-email: Aditya Karan Chhabra <aditya0chhabra@gmail.com>, Arijit Basu <hi@arijitbasu.in>
 Maintainer-email: Aditya Karan Chhabra <aditya0chhabra@gmail.com>, Arijit Basu <hi@arijitbasu.in>
 License: MIT License
         
         Copyright (c) 2023 Aditya Karan Chhabra, Abhishek Arora, Arijit Basu
@@ -45,18 +45,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.0.0
-Requires-Dist: pandas>=1.2.0
-Requires-Dist: python-dateutil>=2.8.0
-Requires-Dist: requests>=2.25.0
-Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: python-dateutil
 
 <div align="center">
 
 # datagovindia
 
 [![MIT license](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/addypy/datagovindia/blob/master/LICENSE) ![PyPI - Version](https://img.shields.io/pypi/v/datagovindia?color=green) [![Downloads](https://static.pepy.tech/personalized-badge/datagovindia?period=total&units=international_system&left_color=gray&left_text=Downloads)](https://pepy.tech/project/datagovindia)
```

### Comparing `datagovindia-1.0.0/README.md` & `datagovindia-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `datagovindia-1.0.0/pyproject.toml` & `datagovindia-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 [tool.setuptools]
 packages = ["datagovindia"]
 package-dir = {"" = "src"}
 
 [project]
 name = "datagovindia"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python API wrapper for Government of India Open Government Data (OGD) platform data.gov.in"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Aditya Karan Chhabra", email = "aditya0chhabra@gmail.com" },
     { name = "Arijit Basu", email = "hi@arijitbasu.in" },
     { name = "Abhishek Arora" }
 ]
 maintainers = [
     { name = "Aditya Karan Chhabra", email = "aditya0chhabra@gmail.com" },
     { name = "Arijit Basu", email = "hi@arijitbasu.in" }
 ]
 
-keywords = ["data.gov.in","indian-government-data","open-data-india","public-datasets","indian-datasets","government-api","india-statistics","ogd-platform"]
+keywords = ["data.gov.in", "indian-government-data", "open-data-india", "public-datasets", "indian-datasets", "government-api", "india-statistics", "ogd-platform"]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Topic :: Database",
     "Intended Audience :: Education",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Information Technology",
@@ -39,20 +39,19 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Natural Language :: English",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "click >=8.0.0",
-    "pandas >=1.2.0",
-    "python-dateutil >=2.8.0",
-    "requests >=2.25.0",
-    "numpy"
+    "click>=8.0.0",
+    "requests",
+    "pandas",
+    "python-dateutil"
 ]
 
 [project.urls]
-homepage   = "https://pypi.org/project/datagovindia/"
+homepage = "https://pypi.org/project/datagovindia/"
 repository = "https://github.com/addypy/datagovindia/"
 
-[project.entry-points.console_scripts]
-datagovindia = "datagovindia.cli:cli"
+[project.scripts]
+datagovindia = "datagovindia.cli:cli"
```

### Comparing `datagovindia-1.0.0/src/datagovindia/__init__.py` & `datagovindia-1.0.1/src/datagovindia/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,42 @@
 import time
 import requests
 import sqlite3
 import pandas as pd
 import multiprocessing as mp
 from typing import List, Dict
 from urllib.parse import urlencode
+from requests.adapters import HTTPAdapter
+from urllib3.util.retry import Retry
 from datetime import datetime
 from dateutil.parser import parse as dateutil_parse
+from collections.abc import Iterable
+from urllib.parse import urlencode
+import logging
 
+# Configure logging
+logging.basicConfig(level=logging.ERROR, format='%(asctime)s - %(levelname)s - %(message)s')
+logger = logging.getLogger(__name__)
+
+__version__ = "0.1.0"
+
+def flatten(lst):
+    """Flatten a nested list"""
+    for item in lst:
+        if isinstance(item, Iterable) and not isinstance(item, str):
+            yield from flatten(item)
+        else:
+            yield item
 def construct_url(params: dict) -> str:
     """
     Construct URL with query parameters.
     """
-    return "https://api.data.gov.in/lists" + "?" + "&".join([f"{k}={v}" for k, v in params.items()])
+    base_url = "https://api.data.gov.in/lists"
+    query_string = urlencode(params)
+    return f"{base_url}?{query_string}"
 
 def remove_special_chars(s: str) -> str:
     """
     Remove special characters from string.
     """
     return re.sub("[^a-zA-Z0-9\.]", "", s).strip().lower() # type: ignore
 
@@ -92,18 +112,18 @@
 def compile_record_info(record: dict) -> dict:
     """Compile record info into a dictionary"""
     return {
         "resource_id": record.get("index_name"),
         "title": record.get("title"),
         "description": record.get("desc"),
         "org_type": record.get("org_type"),
-        "fields": " | ".join([f.get("id", "") for f in record.get("field", [])]),
-        "orgs": " | ".join(record.get("org", [])),
+        "fields": " | ".join(str(f.get("id", "")) for f in record.get("field", [])),
+        "orgs": " | ".join(str(item) for item in flatten(record.get("org", []))),
         "source": record.get("source"),
-        "sectors": " | ".join(record.get("sector", [])),
+        "sectors": " | ".join(str(item) for item in record.get("sector", [])),
         "date_created": format_date(record.get("created_date")),
         "date_updated": format_date(record.get("updated_date")),
     }
 
 def get_total_available_resources() -> int:
     """
     Retrieve total number of available records.
@@ -129,26 +149,46 @@
         "filters[active]": 1,
         "sort[updated]": "desc",
         "format": "json",
         "offset": start,
         "limit": end - start,
     }
     api_url = construct_url(params)
-    resp = requests.get(api_url, timeout=(5, 10))
-    return [compile_record_info(record) for record in resp.json()["records"]]
 
+    session = requests.Session()
+    retry_strategy = Retry(
+        total=5,
+        backoff_factor=2,
+        status_forcelist=[429, 500, 502, 503, 504],
+        allowed_methods=["GET"]
+    )
+    adapter = HTTPAdapter(max_retries=retry_strategy)
+    session.mount("https://", adapter)
+    session.mount("http://", adapter)
+
+    try:
+        resp = session.get(api_url, timeout=(30, 60))
+        resp.raise_for_status()
+        logger.info(f"Successfully fetched data for range ({start}-{end}")
+        return [compile_record_info(record) for record in resp.json().get("records", [])]
+    except requests.exceptions.RequestException as e:
+        logger.error(f"Request failed for range ({start}-{end}): {e}")
+        return []
+    
 def fetch_metadata_records(
-    api_key:str, start: int = 0, end: int = 1000000, batch_size: int = 100, njobs: int = None
+    api_key: str, start: int = 0, end: int = 1000000, batch_size: int = 100, njobs: int = None
 ) -> list:
     """Retrieve records using multiple threads."""
     with mp.Pool(njobs) as pool:
         data = pool.starmap(
             _fetch_metadata, [(api_key, i, min(end, i + batch_size)) for i in range(start, end, batch_size)]
         )
-    return [item for sublist in data for item in sublist]
+    # Filter out None results
+    data = [item for sublist in data if sublist is not None for item in sublist]
+    return data
 
 def get_api_info(url) -> dict:
     """Get json data from url"""
     response = requests.get(url, timeout=(5, 10)).json()
     skip_keys = [
         "message",
         "version",
@@ -284,14 +324,15 @@
         if db_path:
             self.db_path = db_path
         else:
             self.db_path = os.environ.get(
                 "DATAGOVINDIA_DB_PATH", os.path.join(os.path.expanduser("~"), "datagovindia.db")
             )
         self.connect(verify=False)
+        
 
     def validate_api_key(self):
         if not self.api_key:
             raise ValueError("API key not found. Please set it as an environment variable `DATAGOVINDIA_API_KEY` or pass it as an argument while initializing the DataGovIndia object.")
 
     def connect(self, verify:bool=False):
         """Connect to datagovindia.db sqlite database"""
@@ -561,21 +602,35 @@
 
     def upsert_records(self, table_name, data_dicts):
         """Insert or replace records in database"""
         self.connect(verify=True)
         placeholders = ", ".join(["?"] * len(data_dicts[0]))
         columns = ", ".join(data_dicts[0].keys())
         sql = f"""INSERT OR REPLACE INTO {table_name} 
-                  ({columns}) 
-                  VALUES ({placeholders})"""
-        self.cursor.executemany(sql, [tuple(data_dict.values()) for data_dict in data_dicts])
+                ({columns}) 
+                VALUES ({placeholders})"""
+        
+        # Convert all values to supported types and log them
+        def convert_value(value):
+            if isinstance(value, (str, int, float, type(None))):
+                return value
+            return str(value)  # Convert unsupported types to strings
+        
+        data_values = []
+        for data_dict in data_dicts:
+            converted_values = tuple(convert_value(v) for v in data_dict.values())
+            logger.debug(f"Inserting values: {converted_values}")
+            data_values.append(converted_values)
+        
+        self.cursor.executemany(sql, data_values)
         self.conn.commit()
         self.close()
+        
 
-    def sync_metadata(self, batch_size=2500, njobs=None):
+    def sync_metadata(self, batch_size=1000, njobs=None): # Reducing batch_size to 1000 to avoid timeout errors
         """Updates metadata in datagovindia.db sqlite database
 
         Parameters
         ----------
 
         batch_size: int (optional)
             Number of records to be fetched in a single request. Defaults to 2500.
@@ -588,30 +643,30 @@
 
         start_time = time.time()
 
         _num_available = get_total_available_resources()
         _num_updated = 0
 
         self.create_tables()
-        njobs = mp.cpu_count() if njobs is None else njobs
+        njobs  = mp.cpu_count() if njobs is None else njobs
         _batch = njobs * batch_size
 
         display_progress_bar(_num_updated, _num_available)
 
         for start in range(0, _num_available, _batch):
-            end = min(_num_available, start + _batch)
+            end     = min(_num_available, start + _batch)
             records = fetch_metadata_records(
                 self.api_key, start=start, end=end, batch_size=batch_size, njobs=njobs
             )
             self.upsert_records("resources", records)
             _num_updated += len(records)
 
             # Calculate ETA
-            elapsed_time = time.time() - start_time
-            avg_time     = elapsed_time / _num_updated
+            elapsed_time   = time.time() - start_time
+            avg_time       = elapsed_time / _num_updated
             _num_remaining = (_num_available - _num_updated) 
             eta = avg_time * _num_remaining
             display_progress_bar(_num_updated, _num_available, eta=format_seconds(eta))
 
         total_time = time.time() - start_time
-        print(f"\nFinished updating {_num_updated} records in {round(total_time)} seconds.")
+        logger.info(f"\nTotal time taken: {format_seconds(total_time)} to update {_num_updated} resources.")
         self._save_update_info(_num_updated)
```

### Comparing `datagovindia-1.0.0/src/datagovindia/cli.py` & `datagovindia-1.0.1/src/datagovindia/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 
         `get-resource-info`: Fetches info for a given resource ID from the OGD platform and displays it in the terminal.
         
         `get-data`: Fetches data for a given resource ID from the OGD platform and saves it to a specified file.
 
     """    
 
+@cli.command(name="version")
+def version():
+    """Displays the version of the DataGovIndia API wrapper."""
+    from datagovindia import __version__
+
+    click.echo(f"datagovindia v{__version__}")
+
 ################## sync-metadata ##################
 @cli.command(name="sync-metadata")
 @click.option(
     "--api-key",
     default=None,
     type=str,
     help=(
@@ -169,22 +176,22 @@
 
         - `asc`: `Sort the results in ascending order. If not provided, defaults to ascending.`
     """
     datagovin = DataGovIndia(api_key=api_key, db_path=db_path)
     click.echo(f"Searching for '{query}' in fields {fields}...")
     search_df = datagovin.search(query, search_fields=fields, sort_by=sort_by, ascending=asc)
 
-    if output:
-        save_dataframe(search_df, output)
-        click.echo(f"{len(search_df)} results saved to '{output}'.")
-
     if preview:
         click.echo(search_df.head(limit))
         click.echo(f"{len(search_df)} results found.")
 
+    if output:
+        save_dataframe(search_df, output)
+        click.echo(f"{len(search_df)} results saved to '{output}'.")
+
     else:
         click.echo(f"{len(search_df)} results found.")
 
 ################## resource-info ##################
 @cli.command(name="get-resource-info")
 @click.argument("resource_id", required=True, type=str)
 @click.option(
```

### Comparing `datagovindia-1.0.0/src/datagovindia.egg-info/PKG-INFO` & `datagovindia-1.0.1/src/datagovindia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagovindia
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API wrapper for Government of India Open Government Data (OGD) platform data.gov.in
 Author: Abhishek Arora
 Author-email: Aditya Karan Chhabra <aditya0chhabra@gmail.com>, Arijit Basu <hi@arijitbasu.in>
 Maintainer-email: Aditya Karan Chhabra <aditya0chhabra@gmail.com>, Arijit Basu <hi@arijitbasu.in>
 License: MIT License
         
         Copyright (c) 2023 Aditya Karan Chhabra, Abhishek Arora, Arijit Basu
@@ -45,18 +45,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.0.0
-Requires-Dist: pandas>=1.2.0
-Requires-Dist: python-dateutil>=2.8.0
-Requires-Dist: requests>=2.25.0
-Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: python-dateutil
 
 <div align="center">
 
 # datagovindia
 
 [![MIT license](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/addypy/datagovindia/blob/master/LICENSE) ![PyPI - Version](https://img.shields.io/pypi/v/datagovindia?color=green) [![Downloads](https://static.pepy.tech/personalized-badge/datagovindia?period=total&units=international_system&left_color=gray&left_text=Downloads)](https://pepy.tech/project/datagovindia)
```

