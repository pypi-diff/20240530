# Comparing `tmp/ioos_metrics-0.1.0a1.tar.gz` & `tmp/ioos_metrics-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ioos_metrics-0.1.0a1.tar", last modified: Thu May  9 08:01:00 2024, max compression
+gzip compressed data, was "ioos_metrics-0.2.0a0.tar", last modified: Thu May 30 14:41:22 2024, max compression
```

## Comparing `ioos_metrics-0.1.0a1.tar` & `ioos_metrics-0.2.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1070 2024-04-17 14:27:47.000000 ioos_metrics-0.1.0a1/LICENSE
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      427 2024-05-09 07:56:45.000000 ioos_metrics-0.1.0a1/MANIFEST.in
--rw-r--r--   0 filipe    (1000) filipe    (1000)     4083 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1908 2024-04-17 14:27:47.000000 ioos_metrics-0.1.0a1/README.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/ioos_metrics/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      124 2024-04-17 14:27:47.000000 ioos_metrics-0.1.0a1/ioos_metrics/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    21689 2024-05-08 18:41:21.000000 ioos_metrics-0.1.0a1/ioos_metrics/ioos_metrics.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     5037 2024-05-02 14:12:37.000000 ioos_metrics-0.1.0a1/ioos_metrics/national_platforms.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/ioos_metrics.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      133 2024-05-09 08:01:00.000000 ioos_metrics-0.1.0a1/ioos_metrics.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1313 2024-05-02 14:12:37.000000 ioos_metrics-0.1.0a1/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-05-09 08:01:00.826749 ioos_metrics-0.1.0a1/setup.cfg
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 14:41:22.840996 ioos_metrics-0.2.0a0/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1070 2024-05-09 10:35:31.000000 ioos_metrics-0.2.0a0/LICENSE
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      427 2024-05-09 10:35:31.000000 ioos_metrics-0.2.0a0/MANIFEST.in
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     4105 2024-05-30 14:41:22.840996 ioos_metrics-0.2.0a0/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1908 2024-05-09 10:35:31.000000 ioos_metrics-0.2.0a0/README.md
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 14:41:22.840996 ioos_metrics-0.2.0a0/ioos_metrics/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      124 2024-05-09 10:35:31.000000 ioos_metrics-0.2.0a0/ioos_metrics/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    24392 2024-05-30 14:40:47.000000 ioos_metrics-0.2.0a0/ioos_metrics/ioos_metrics.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     5037 2024-05-09 10:35:31.000000 ioos_metrics-0.2.0a0/ioos_metrics/national_platforms.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-30 14:41:22.840996 ioos_metrics-0.2.0a0/ioos_metrics.egg-info/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      133 2024-05-30 14:41:22.000000 ioos_metrics-0.2.0a0/ioos_metrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1325 2024-05-30 14:40:47.000000 ioos_metrics-0.2.0a0/pyproject.toml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-05-30 14:41:22.840996 ioos_metrics-0.2.0a0/setup.cfg
```

### Comparing `ioos_metrics-0.1.0a1/LICENSE` & `ioos_metrics-0.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ioos_metrics-0.1.0a1/PKG-INFO` & `ioos_metrics-0.2.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ioos_metrics
-Version: 0.1.0a1
+Version: 0.2.0a0
 Summary: Package to fetch various metrics for IOOS by the numbers
 Maintainer: Filipe Fernandes
 License: MIT License
         
         Copyright (c) 2021 Mathew Biddle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,15 @@
 Requires-Dist: gliderpy
 Requires-Dist: html5lib
 Requires-Dist: joblib
 Requires-Dist: lxml
 Requires-Dist: pandas
 Requires-Dist: pdfminer.six
 Requires-Dist: pyarrow
+Requires-Dist: pyobis
 Requires-Dist: requests
 
 # ioos_by_the_numbers
 Working on creating metrics for the [IOOS by the numbers](https://ioos.noaa.gov/about/ioos-by-the-numbers/)
 
 Requirements:
```

### Comparing `ioos_metrics-0.1.0a1/README.md` & `ioos_metrics-0.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `ioos_metrics-0.1.0a1/ioos_metrics/ioos_metrics.py` & `ioos_metrics-0.2.0a0/ioos_metrics/ioos_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import httpx
 import joblib
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from fake_useragent import UserAgent
 from gliderpy.fetchers import GliderDataFetcher
-from shapely.geometry import LineString
+from shapely.geometry import LineString, Point
 
 from ioos_metrics.national_platforms import national_platforms
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     filename="metrics.log",
     encoding="utf-8",
@@ -202,38 +202,54 @@
             "sea_name": _extra_info(info_df, attribute_name="sea_name"),
             "acknowledgment": _extra_info(
                 info_df,
                 attribute_name="acknowledgment",
             ),
         }
 
+    def _make_track_geom(df) -> "pd.DataFrame":
+        geom = Point if df.shape[0] == 1 else LineString
+
+        return geom(
+            (lon, lat)
+            for (lon, lat) in zip(
+                df["longitude (degrees_east)"],
+                df["latitude (degrees_north)"],
+                strict=False,
+            )
+        )
+
     def _computed_metadata(dataset_id) -> dict:
         """Download the minimum amount of data possible for the computed
         metadata.
 
         Note that we cannot get first and last b/c the profile_id is not a
         contiguous sequence.
         """
         glider_grab.fetcher.dataset_id = dataset_id
         glider_grab.fetcher.variables = [
             "profile_id",
             "latitude",
             "longitude",
             "time",
         ]
-        df = glider_grab.to_pandas()
+        df = glider_grab.fetcher.to_pandas(distinct=True)
+        df["time (UTC)"] = pd.to_datetime(df["time (UTC)"])
+        df = df.set_index("time (UTC)")
         df = df.sort_index()
+        track = _make_track_geom(df)
         days = df.index[-1].ceil("D") - df.index[0].floor("D")
         return {
-            "deployment_lat": df["latitude"].iloc[0],
-            "deployment_lon": df["longitude"].iloc[0],
+            "deployment_lat": df["latitude (degrees_north)"].iloc[0],
+            "deployment_lon": df["longitude (degrees_east)"].iloc[0],
             "num_profiles": len(df),
             # Profiles are not unique! Cannot use this!!
             # "num_profiles": len(set(df['profile_id']))
             "days": days,
+            "track": track,
         }
 
     glider_grab = GliderDataFetcher()
 
     df = glider_grab.query(
         min_lat=min_lat,
         max_lat=max_lat,
@@ -241,41 +257,27 @@
         max_lon=max_lon,
         min_time=min_time,
         max_time=max_time,
         delayed=False,  # We do not want delayed gliders.
     )
 
     metadata = {}
-    glider_grab.fetcher.variables = ["longitude", "latitude"]
     for _, row in list(df.iterrows()):
         dataset_id = row["Dataset ID"]
-
-        glider_grab.fetcher.dataset_id = dataset_id
-        track = glider_grab.fetcher.to_pandas(distinct=True)
-        track = LineString(
-            (lon, lat)
-            for (lon, lat) in zip(
-                track["longitude (degrees_east)"],
-                track["latitude (degrees_north)"],
-                strict=False,
-            )
-        )
-
         info_url = row["info_url"].replace("html", "csv")
         info_df = pd.read_csv(info_url)
         info = _metadata(info_df)
         try:
             info.update(_computed_metadata(dataset_id=dataset_id))
         except (httpx.HTTPError, httpx.HTTPStatusError):
             print(  # noqa: T201
                 f"Could not fetch glider {dataset_id=}. "
                 "This could be a server side error and the metrics will be incomplete!",
             )
             continue
-        info.update({"track": track})
         metadata.update({dataset_id: info})
     return pd.DataFrame(metadata).T
 
 
 def ngdac_gliders():
     """Runs _ngdac_gliders for the whole server and returns only the glider days to compare with ngdac_gliders_fast."""
     metadata = _ngdac_gliders()
@@ -551,14 +553,80 @@
     From http://hfrnet.ucsd.edu/sitediag/stationList.php
 
     """
     # This is a hardcoded number at the moment!
     return 165
 
 
+@functools.lru_cache(maxsize=128)
+def mbon_stats():
+    """Collects download statistics about MBON affiliated datasets shared with the Ocean Biodiversity
+    Information System (OBIS) and the Global Biodiversity Information Framework (GBIF). The function returns a
+    dataframe with rows corresponding to each paper citing a dataset.
+    """
+    import urllib.parse
+
+    import pyobis
+
+    # collect dataset information from OBIS
+    institution_id = 23070
+    query = pyobis.dataset.search(instituteid=institution_id)
+    df = pd.DataFrame(query.execute())
+    df_obis = pd.DataFrame.from_records(df["results"])
+    df_obis.columns = [f"obis_{col}" for col in df_obis.columns]
+
+    df_mapping = pd.DataFrame()
+    base_url = "https://api.gbif.org"
+    # iterate through each OBIS dataset to gather uuid from GBIF
+    # create a mapping table
+    for title in df_obis["obis_title"]:
+        string = title
+        query = f"{base_url}/v1/dataset/search?q={urllib.parse.quote(string)}"
+        df = pd.read_json(query, orient="index").T
+
+        # build a DataFrame with the info we need more accessible
+        df_mapping = pd.concat(
+            [
+                df_mapping,
+                pd.DataFrame(
+                    {
+                        "gbif_uuid": df["results"].to_numpy()[0][0]["key"],
+                        "title": [df["results"].to_numpy()[0][0]["title"]],
+                        "obis_id": [df_obis.loc[df_obis["obis_title"] == title, "obis_id"].to_string(index=False)],
+                        "doi": [df["results"].to_numpy()[0][0]["doi"]],
+                    },
+                ),
+            ],
+            ignore_index=True,
+        )
+
+    df_gbif = pd.DataFrame()
+    for key in df_mapping["gbif_uuid"]:
+        url = f"https://api.gbif.org/v1/literature/export?format=CSV&gbifDatasetKey={key}"
+        df2 = pd.read_csv(url)  # collect literature cited information
+        df2.columns = ["literature_" + str(col) for col in df2.columns]
+        df2["gbif_uuid"] = key
+
+        df_gbif = pd.concat([df2, df_gbif], ignore_index=True)
+
+    # merge the OBIS and GBIF data frames together
+    df_obis = df_obis.merge(df_mapping, on="obis_id")
+
+    # add gbif download stats
+
+    for key in df_obis["gbif_uuid"]:
+        url = f"https://api.gbif.org/v1/occurrence/download/statistics/export?datasetKey={key}"
+        df2 = pd.read_csv(url, sep="\t")
+        df2_group = df2.groupby("year").agg({"number_downloads": "sum"})
+
+        df_obis.loc[df_obis["gbif_uuid"] == key, "gbif_downloads"] = str(df2_group.to_dict())
+
+    return df_gbif.merge(df_obis, on="gbif_uuid")
+
+
 def update_metrics(*, debug=False):
     """Load previous metrics and update the spreadsheet."""
     df = previous_metrics()
     today = pd.Timestamp.strftime(pd.Timestamp.today(tz="UTC"), "%Y-%m-%d")
 
     new_row = {
         "date_UTC": today,
```

### Comparing `ioos_metrics-0.1.0a1/ioos_metrics/national_platforms.py` & `ioos_metrics-0.2.0a0/ioos_metrics/national_platforms.py`

 * *Files identical despite different names*

### Comparing `ioos_metrics-0.1.0a1/pyproject.toml` & `ioos_metrics-0.2.0a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   "gliderpy",
   "html5lib",
   "joblib",
   "lxml",
   "pandas",
   "pdfminer.six",
   "pyarrow",
+  "pyobis",
   "requests",
 ]
 [project.urls]
 documentation = "https://ioos.github.io/ioos_metrics"
 homepage = "https://github.com/ioos/ioos_metrics"
 repository = "https://github.com/ioos/ioos_metrics"
```

