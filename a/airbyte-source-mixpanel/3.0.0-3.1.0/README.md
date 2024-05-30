# Comparing `tmp/airbyte_source_mixpanel-3.0.0.tar.gz` & `tmp/airbyte_source_mixpanel-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_mixpanel-3.0.0.tar", max compression
+gzip compressed data, was "airbyte_source_mixpanel-3.1.0.tar", max compression
```

## Comparing `airbyte_source_mixpanel-3.0.0.tar` & `airbyte_source_mixpanel-3.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4547 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/README.md
--rw-r--r--   0        0        0      753 2024-05-23 13:11:25.666516 airbyte_source_mixpanel-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1138 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/__init__.py
--rw-r--r--   0        0        0    13953 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/components.py
--rw-r--r--   0        0        0     3363 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/config_migrations.py
--rw-r--r--   0        0        0    12373 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/manifest.yaml
--rw-r--r--   0        0        0     1505 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/property_transformation.py
--rw-r--r--   0        0        0      350 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/run.py
--rw-r--r--   0        0        0     1208 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/annotations.json
--rw-r--r--   0        0        0     2050 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/cohort_members.json
--rw-r--r--   0        0        0     1249 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/cohorts.json
--rw-r--r--   0        0        0     1796 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/engage.json
--rw-r--r--   0        0        0     9765 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/export.json
--rw-r--r--   0        0        0      204 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/funnel_ids.json
--rw-r--r--   0        0        0     5384 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/funnels.json
--rw-r--r--   0        0        0      843 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/revenue.json
--rw-r--r--   0        0        0     5269 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/source.py
--rw-r--r--   0        0        0     5361 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/spec.json
--rw-r--r--   0        0        0      298 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/streams/__init__.py
--rw-r--r--   0        0        0     9965 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/streams/base.py
--rw-r--r--   0        0        0     1511 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/streams/engage.py
--rw-r--r--   0        0        0     8023 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/streams/export.py
--rw-r--r--   0        0        0      992 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/testing.py
--rw-r--r--   0        0        0     1965 2024-05-23 12:04:03.000000 airbyte_source_mixpanel-3.0.0/source_mixpanel/utils.py
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 airbyte_source_mixpanel-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4547 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/README.md
+-rw-r--r--   0        0        0      753 2024-05-30 08:44:20.972485 airbyte_source_mixpanel-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1138 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/__init__.py
+-rw-r--r--   0        0        0    13953 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/components.py
+-rw-r--r--   0        0        0     3363 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/config_migrations.py
+-rw-r--r--   0        0        0    12373 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/manifest.yaml
+-rw-r--r--   0        0        0     1505 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/property_transformation.py
+-rw-r--r--   0        0        0      350 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/run.py
+-rw-r--r--   0        0        0     1208 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/annotations.json
+-rw-r--r--   0        0        0     2050 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/cohort_members.json
+-rw-r--r--   0        0        0     1249 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/cohorts.json
+-rw-r--r--   0        0        0     1796 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/engage.json
+-rw-r--r--   0        0        0     9765 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/export.json
+-rw-r--r--   0        0        0      204 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/funnel_ids.json
+-rw-r--r--   0        0        0     5384 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/funnels.json
+-rw-r--r--   0        0        0      843 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/revenue.json
+-rw-r--r--   0        0        0     5269 2024-05-30 08:39:41.570374 airbyte_source_mixpanel-3.1.0/source_mixpanel/source.py
+-rw-r--r--   0        0        0     5371 2024-05-30 08:39:41.574374 airbyte_source_mixpanel-3.1.0/source_mixpanel/spec.json
+-rw-r--r--   0        0        0      298 2024-05-30 08:39:41.574374 airbyte_source_mixpanel-3.1.0/source_mixpanel/streams/__init__.py
+-rw-r--r--   0        0        0     9965 2024-05-30 08:39:41.574374 airbyte_source_mixpanel-3.1.0/source_mixpanel/streams/base.py
+-rw-r--r--   0        0        0     1511 2024-05-30 08:39:41.574374 airbyte_source_mixpanel-3.1.0/source_mixpanel/streams/engage.py
+-rw-r--r--   0        0        0     8023 2024-05-30 08:39:41.574374 airbyte_source_mixpanel-3.1.0/source_mixpanel/streams/export.py
+-rw-r--r--   0        0        0      992 2024-05-30 08:39:41.574374 airbyte_source_mixpanel-3.1.0/source_mixpanel/testing.py
+-rw-r--r--   0        0        0     1965 2024-05-30 08:39:41.574374 airbyte_source_mixpanel-3.1.0/source_mixpanel/utils.py
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 airbyte_source_mixpanel-3.1.0/PKG-INFO
```

### Comparing `airbyte_source_mixpanel-3.0.0/README.md` & `airbyte_source_mixpanel-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/pyproject.toml` & `airbyte_source_mixpanel-3.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.0.0"
+version = "3.1.0"
 name = "airbyte-source-mixpanel"
 description = "Source implementation for Mixpanel."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/__init__.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/components.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/config_migrations.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/manifest.yaml` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/property_transformation.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/property_transformation.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/annotations.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/annotations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/cohort_members.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/cohort_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/cohorts.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/cohorts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/engage.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/engage.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/export.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/export.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/funnels.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/funnels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/schemas/revenue.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/schemas/revenue.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/source.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/spec.json` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/spec.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997767857142857%*

 * *Differences: {"'connectionSpecification'": "{'properties': {'start_date': {'format': 'date-time'}, 'end_date': "*

 * *                              "{'format': 'date-time'}}}"}*

```diff
@@ -82,15 +82,15 @@
                 "type": "integer"
             },
             "end_date": {
                 "description": "The date in the format YYYY-MM-DD. Any data after this date will not be replicated. Left empty to always sync to most recent date",
                 "examples": [
                     "2021-11-16"
                 ],
-                "format": "date",
+                "format": "date-time",
                 "order": 6,
                 "pattern": "^$|^[0-9]{4}-[0-9]{2}-[0-9]{2}(T[0-9]{2}:[0-9]{2}:[0-9]{2}Z)?$",
                 "title": "End Date",
                 "type": "string"
             },
             "project_timezone": {
                 "default": "US/Pacific",
@@ -122,15 +122,15 @@
                 "type": "boolean"
             },
             "start_date": {
                 "description": "The date in the format YYYY-MM-DD. Any data before this date will not be replicated. If this option is not set, the connector will replicate data from up to one year ago by default.",
                 "examples": [
                     "2021-11-16"
                 ],
-                "format": "date",
+                "format": "date-time",
                 "order": 5,
                 "pattern": "^$|^[0-9]{4}-[0-9]{2}-[0-9]{2}(T[0-9]{2}:[0-9]{2}:[0-9]{2}Z)?$",
                 "title": "Start Date",
                 "type": "string"
             }
         },
         "required": [
```

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/streams/base.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/streams/base.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/streams/engage.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/streams/engage.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/streams/export.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/streams/export.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/testing.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/testing.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/source_mixpanel/utils.py` & `airbyte_source_mixpanel-3.1.0/source_mixpanel/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_mixpanel-3.0.0/PKG-INFO` & `airbyte_source_mixpanel-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-mixpanel
-Version: 3.0.0
+Version: 3.1.0
 Summary: Source implementation for Mixpanel.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

