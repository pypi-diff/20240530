# Comparing `tmp/rov_db_access-1.0.7.tar.gz` & `tmp/rov_db_access-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-1.0.7.tar", max compression
+gzip compressed data, was "rov_db_access-1.0.8.tar", max compression
```

## Comparing `rov_db_access-1.0.7.tar` & `rov_db_access-1.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2024-01-29 18:44:26.776172 rov_db_access-1.0.7/README.md
--rw-r--r--   0        0        0      561 2024-05-29 18:51:42.240872 rov_db_access-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 20:01:43.946199 rov_db_access-1.0.7/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.475751 rov_db_access-1.0.7/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2332 2024-05-20 20:01:43.946696 rov_db_access-1.0.7/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     1195 2024-05-20 13:50:20.917781 rov_db_access-1.0.7/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.917823 rov_db_access-1.0.7/rov_db_access/config/__init__.py
--rw-r--r--   0        0        0     2069 2024-05-15 15:24:19.907085 rov_db_access-1.0.7/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0      983 2024-05-20 20:01:43.947272 rov_db_access-1.0.7/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.918355 rov_db_access-1.0.7/rov_db_access/geodata/__init__.py
--rw-r--r--   0        0        0     1966 2024-05-20 13:50:20.918452 rov_db_access-1.0.7/rov_db_access/geodata/models.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476424 rov_db_access-1.0.7/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     8313 2024-05-28 22:12:46.563385 rov_db_access-1.0.7/rov_db_access/gis/models.py
--rw-r--r--   0        0        0       78 2024-05-20 13:50:20.918762 rov_db_access-1.0.7/rov_db_access/gis/test.py
--rw-r--r--   0        0        0    36047 2024-05-29 19:41:43.231752 rov_db_access-1.0.7/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919463 rov_db_access-1.0.7/rov_db_access/ine/__init__.py
--rw-r--r--   0        0        0      850 2024-05-20 13:50:20.919583 rov_db_access-1.0.7/rov_db_access/ine/models.py
--rw-r--r--   0        0        0     2298 2024-05-20 13:50:20.919670 rov_db_access-1.0.7/rov_db_access/ine/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919752 rov_db_access-1.0.7/rov_db_access/label_studio/__init__.py
--rw-r--r--   0        0        0     9115 2024-05-20 13:50:20.919967 rov_db_access-1.0.7/rov_db_access/label_studio/models.py
--rw-r--r--   0        0        0     7153 2024-05-20 13:50:20.920121 rov_db_access-1.0.7/rov_db_access/label_studio/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920191 rov_db_access-1.0.7/rov_db_access/landing/__init__.py
--rw-r--r--   0        0        0     2124 2024-05-20 13:50:20.920282 rov_db_access-1.0.7/rov_db_access/landing/models.py
--rw-r--r--   0        0        0     5890 2024-05-20 13:50:20.920415 rov_db_access-1.0.7/rov_db_access/landing/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920480 rov_db_access-1.0.7/rov_db_access/risks/__init__.py
--rw-r--r--   0        0        0     1176 2024-05-20 13:50:20.920564 rov_db_access-1.0.7/rov_db_access/risks/models.py
--rw-r--r--   0        0        0     6554 2024-05-27 19:05:01.933210 rov_db_access-1.0.7/rov_db_access/risks/worker.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476890 rov_db_access-1.0.7/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      412 2024-05-08 18:50:41.477041 rov_db_access-1.0.7/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     5878 2024-05-20 13:50:20.921035 rov_db_access-1.0.7/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.921067 rov_db_access-1.0.7/rov_db_access/utils/__init__.py
--rw-r--r--   0        0        0     5317 2024-05-20 20:01:43.948847 rov_db_access-1.0.7/rov_db_access/utils/geoserver_utils.py
--rw-r--r--   0        0        0     2078 2024-05-20 20:01:43.949178 rov_db_access-1.0.7/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1120 2024-05-20 13:50:20.921348 rov_db_access-1.0.7/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-29 18:44:26.776172 rov_db_access-1.0.8/README.md
+-rw-r--r--   0        0        0      561 2024-05-30 16:31:48.626463 rov_db_access-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 20:01:43.946199 rov_db_access-1.0.8/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.475751 rov_db_access-1.0.8/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2332 2024-05-20 20:01:43.946696 rov_db_access-1.0.8/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     2483 2024-05-30 16:31:48.626817 rov_db_access-1.0.8/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.917823 rov_db_access-1.0.8/rov_db_access/config/__init__.py
+-rw-r--r--   0        0        0     2069 2024-05-15 15:24:19.907085 rov_db_access-1.0.8/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0      983 2024-05-20 20:01:43.947272 rov_db_access-1.0.8/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.918355 rov_db_access-1.0.8/rov_db_access/geodata/__init__.py
+-rw-r--r--   0        0        0     1966 2024-05-20 13:50:20.918452 rov_db_access-1.0.8/rov_db_access/geodata/models.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476424 rov_db_access-1.0.8/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     8313 2024-05-28 22:12:46.563385 rov_db_access-1.0.8/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0       78 2024-05-20 13:50:20.918762 rov_db_access-1.0.8/rov_db_access/gis/test.py
+-rw-r--r--   0        0        0    36288 2024-05-30 16:31:48.627256 rov_db_access-1.0.8/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919463 rov_db_access-1.0.8/rov_db_access/ine/__init__.py
+-rw-r--r--   0        0        0      850 2024-05-20 13:50:20.919583 rov_db_access-1.0.8/rov_db_access/ine/models.py
+-rw-r--r--   0        0        0     2298 2024-05-20 13:50:20.919670 rov_db_access-1.0.8/rov_db_access/ine/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919752 rov_db_access-1.0.8/rov_db_access/label_studio/__init__.py
+-rw-r--r--   0        0        0     9115 2024-05-20 13:50:20.919967 rov_db_access-1.0.8/rov_db_access/label_studio/models.py
+-rw-r--r--   0        0        0     7153 2024-05-20 13:50:20.920121 rov_db_access-1.0.8/rov_db_access/label_studio/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920191 rov_db_access-1.0.8/rov_db_access/landing/__init__.py
+-rw-r--r--   0        0        0     2124 2024-05-20 13:50:20.920282 rov_db_access-1.0.8/rov_db_access/landing/models.py
+-rw-r--r--   0        0        0     5890 2024-05-20 13:50:20.920415 rov_db_access-1.0.8/rov_db_access/landing/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920480 rov_db_access-1.0.8/rov_db_access/risks/__init__.py
+-rw-r--r--   0        0        0     1176 2024-05-20 13:50:20.920564 rov_db_access-1.0.8/rov_db_access/risks/models.py
+-rw-r--r--   0        0        0     6554 2024-05-27 19:05:01.933210 rov_db_access-1.0.8/rov_db_access/risks/worker.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476890 rov_db_access-1.0.8/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-08 18:50:41.477041 rov_db_access-1.0.8/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     5878 2024-05-20 13:50:20.921035 rov_db_access-1.0.8/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.921067 rov_db_access-1.0.8/rov_db_access/utils/__init__.py
+-rw-r--r--   0        0        0     5317 2024-05-20 20:01:43.948847 rov_db_access-1.0.8/rov_db_access/utils/geoserver_utils.py
+-rw-r--r--   0        0        0     2078 2024-05-20 20:01:43.949178 rov_db_access-1.0.8/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1120 2024-05-20 13:50:20.921348 rov_db_access-1.0.8/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.8/PKG-INFO
```

### Comparing `rov_db_access-1.0.7/pyproject.toml` & `rov_db_access-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rov-db-access"
-version = "1.0.7"
+version = "1.0.8"
 description = ""
 authors = ["Pablo Cano <pablo.cano@rovisen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 geoalchemy2 = "^0.14.2"
```

### Comparing `rov_db_access-1.0.7/rov_db_access/authentication/models.py` & `rov_db_access-1.0.8/rov_db_access/authentication/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/config/db_utils.py` & `rov_db_access-1.0.8/rov_db_access/config/db_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/config/settings.py` & `rov_db_access-1.0.8/rov_db_access/config/settings.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/geodata/models.py` & `rov_db_access-1.0.8/rov_db_access/geodata/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/gis/models.py` & `rov_db_access-1.0.8/rov_db_access/gis/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/gis/worker.py` & `rov_db_access-1.0.8/rov_db_access/gis/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -521,14 +521,16 @@
                     "type": process.type,
                     "created_at": process.created_at,
                     "finished_at": process.finished_at,
                     "runtime": process.runtime,
                     "area": process.area,
                     "cost_estimated": process.cost_estimated,
                     "inference_model_id": process.inference_model_id,
+                    "user_id": process.user_id,
+                    "organization_id": process.organization_id,
                     "geom": geom,
                     "mask": mask,
                 }
 
     def load_processes_by_org(self, org_id: int):
         with Session(self.engine) as session:
             query = (
@@ -556,14 +558,16 @@
                     "type": process.type,
                     "created_at": process.created_at,
                     "finished_at": process.finished_at,
                     "runtime": process.runtime,
                     "area": process.area,
                     "cost_estimated": process.cost_estimated,
                     "inference_model_id": process.inference_model_id,
+                    "user_id": process.user_id,
+                    "organization_id": process.organization_id,
                     "geom": geom,
                     "mask": mask,
                 })
             return result
 
     def load_results_by_run_id(self, id: str):
         results = {
@@ -855,15 +859,15 @@
 
         assert raster_name is not None or len(file_names) != 0, 'No files to upload!'
 
         with Session(self.engine) as session:
             # actual function
             run = session.get(Run, run_id)
             if run is None:
-                print(f'No run with id ${run_id} found!')
+                print(f'No run with id {run_id} found!')
                 return False
 
             process_id = run.process_id
             org_id = run.process.organization_id
             run_id = run.id
 
             # upload files to bucket
@@ -924,13 +928,13 @@
 
     def load_run_input(self, run_id: str):
         with Session(self.engine) as session:
             query = select(Run.input).where(Run.id == run_id)
             input = session.scalar(query)
             if input is None:
                 print('Run with corrupted Input data')
+                return None
+            elif input.status == 'waiting':
+                print('Run data is not ready yet')
+                return None
             else:
-                return {
-                    "status": input.status,
-                    "data": input.data,
-                    "type": input.type,
-                }
+                return input.data
```

### Comparing `rov_db_access-1.0.7/rov_db_access/ine/models.py` & `rov_db_access-1.0.8/rov_db_access/ine/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/ine/worker.py` & `rov_db_access-1.0.8/rov_db_access/ine/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/label_studio/models.py` & `rov_db_access-1.0.8/rov_db_access/label_studio/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/label_studio/worker.py` & `rov_db_access-1.0.8/rov_db_access/label_studio/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/landing/models.py` & `rov_db_access-1.0.8/rov_db_access/landing/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/landing/worker.py` & `rov_db_access-1.0.8/rov_db_access/landing/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/risks/models.py` & `rov_db_access-1.0.8/rov_db_access/risks/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/risks/worker.py` & `rov_db_access-1.0.8/rov_db_access/risks/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/sentinel/worker.py` & `rov_db_access-1.0.8/rov_db_access/sentinel/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/utils/geoserver_utils.py` & `rov_db_access-1.0.8/rov_db_access/utils/geoserver_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/utils/s3_utils.py` & `rov_db_access-1.0.8/rov_db_access/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/rov_db_access/utils/utils.py` & `rov_db_access-1.0.8/rov_db_access/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.7/PKG-INFO` & `rov_db_access-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 1.0.7
+Version: 1.0.8
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

