# Comparing `tmp/rov_db_access-1.0.6.tar.gz` & `tmp/rov_db_access-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-1.0.6.tar", max compression
+gzip compressed data, was "rov_db_access-1.0.7.tar", max compression
```

## Comparing `rov_db_access-1.0.6.tar` & `rov_db_access-1.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2024-01-29 18:44:26.776172 rov_db_access-1.0.6/README.md
--rw-r--r--   0        0        0      561 2024-05-29 15:21:47.087624 rov_db_access-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 20:01:43.946199 rov_db_access-1.0.6/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.475751 rov_db_access-1.0.6/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2332 2024-05-20 20:01:43.946696 rov_db_access-1.0.6/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     1195 2024-05-20 13:50:20.917781 rov_db_access-1.0.6/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.917823 rov_db_access-1.0.6/rov_db_access/config/__init__.py
--rw-r--r--   0        0        0     2069 2024-05-15 15:24:19.907085 rov_db_access-1.0.6/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0      983 2024-05-20 20:01:43.947272 rov_db_access-1.0.6/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.918355 rov_db_access-1.0.6/rov_db_access/geodata/__init__.py
--rw-r--r--   0        0        0     1966 2024-05-20 13:50:20.918452 rov_db_access-1.0.6/rov_db_access/geodata/models.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476424 rov_db_access-1.0.6/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     8313 2024-05-28 22:12:46.563385 rov_db_access-1.0.6/rov_db_access/gis/models.py
--rw-r--r--   0        0        0       78 2024-05-20 13:50:20.918762 rov_db_access-1.0.6/rov_db_access/gis/test.py
--rw-r--r--   0        0        0    36021 2024-05-29 15:21:38.081120 rov_db_access-1.0.6/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919463 rov_db_access-1.0.6/rov_db_access/ine/__init__.py
--rw-r--r--   0        0        0      850 2024-05-20 13:50:20.919583 rov_db_access-1.0.6/rov_db_access/ine/models.py
--rw-r--r--   0        0        0     2298 2024-05-20 13:50:20.919670 rov_db_access-1.0.6/rov_db_access/ine/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919752 rov_db_access-1.0.6/rov_db_access/label_studio/__init__.py
--rw-r--r--   0        0        0     9115 2024-05-20 13:50:20.919967 rov_db_access-1.0.6/rov_db_access/label_studio/models.py
--rw-r--r--   0        0        0     7153 2024-05-20 13:50:20.920121 rov_db_access-1.0.6/rov_db_access/label_studio/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920191 rov_db_access-1.0.6/rov_db_access/landing/__init__.py
--rw-r--r--   0        0        0     2124 2024-05-20 13:50:20.920282 rov_db_access-1.0.6/rov_db_access/landing/models.py
--rw-r--r--   0        0        0     5890 2024-05-20 13:50:20.920415 rov_db_access-1.0.6/rov_db_access/landing/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920480 rov_db_access-1.0.6/rov_db_access/risks/__init__.py
--rw-r--r--   0        0        0     1176 2024-05-20 13:50:20.920564 rov_db_access-1.0.6/rov_db_access/risks/models.py
--rw-r--r--   0        0        0     6554 2024-05-27 19:05:01.933210 rov_db_access-1.0.6/rov_db_access/risks/worker.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476890 rov_db_access-1.0.6/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      412 2024-05-08 18:50:41.477041 rov_db_access-1.0.6/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     5878 2024-05-20 13:50:20.921035 rov_db_access-1.0.6/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.921067 rov_db_access-1.0.6/rov_db_access/utils/__init__.py
--rw-r--r--   0        0        0     5317 2024-05-20 20:01:43.948847 rov_db_access-1.0.6/rov_db_access/utils/geoserver_utils.py
--rw-r--r--   0        0        0     2078 2024-05-20 20:01:43.949178 rov_db_access-1.0.6/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1120 2024-05-20 13:50:20.921348 rov_db_access-1.0.6/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-29 18:44:26.776172 rov_db_access-1.0.7/README.md
+-rw-r--r--   0        0        0      561 2024-05-29 18:51:42.240872 rov_db_access-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 20:01:43.946199 rov_db_access-1.0.7/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.475751 rov_db_access-1.0.7/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2332 2024-05-20 20:01:43.946696 rov_db_access-1.0.7/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     1195 2024-05-20 13:50:20.917781 rov_db_access-1.0.7/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.917823 rov_db_access-1.0.7/rov_db_access/config/__init__.py
+-rw-r--r--   0        0        0     2069 2024-05-15 15:24:19.907085 rov_db_access-1.0.7/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0      983 2024-05-20 20:01:43.947272 rov_db_access-1.0.7/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.918355 rov_db_access-1.0.7/rov_db_access/geodata/__init__.py
+-rw-r--r--   0        0        0     1966 2024-05-20 13:50:20.918452 rov_db_access-1.0.7/rov_db_access/geodata/models.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476424 rov_db_access-1.0.7/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     8313 2024-05-28 22:12:46.563385 rov_db_access-1.0.7/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0       78 2024-05-20 13:50:20.918762 rov_db_access-1.0.7/rov_db_access/gis/test.py
+-rw-r--r--   0        0        0    36047 2024-05-29 19:41:43.231752 rov_db_access-1.0.7/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919463 rov_db_access-1.0.7/rov_db_access/ine/__init__.py
+-rw-r--r--   0        0        0      850 2024-05-20 13:50:20.919583 rov_db_access-1.0.7/rov_db_access/ine/models.py
+-rw-r--r--   0        0        0     2298 2024-05-20 13:50:20.919670 rov_db_access-1.0.7/rov_db_access/ine/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919752 rov_db_access-1.0.7/rov_db_access/label_studio/__init__.py
+-rw-r--r--   0        0        0     9115 2024-05-20 13:50:20.919967 rov_db_access-1.0.7/rov_db_access/label_studio/models.py
+-rw-r--r--   0        0        0     7153 2024-05-20 13:50:20.920121 rov_db_access-1.0.7/rov_db_access/label_studio/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920191 rov_db_access-1.0.7/rov_db_access/landing/__init__.py
+-rw-r--r--   0        0        0     2124 2024-05-20 13:50:20.920282 rov_db_access-1.0.7/rov_db_access/landing/models.py
+-rw-r--r--   0        0        0     5890 2024-05-20 13:50:20.920415 rov_db_access-1.0.7/rov_db_access/landing/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920480 rov_db_access-1.0.7/rov_db_access/risks/__init__.py
+-rw-r--r--   0        0        0     1176 2024-05-20 13:50:20.920564 rov_db_access-1.0.7/rov_db_access/risks/models.py
+-rw-r--r--   0        0        0     6554 2024-05-27 19:05:01.933210 rov_db_access-1.0.7/rov_db_access/risks/worker.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476890 rov_db_access-1.0.7/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-08 18:50:41.477041 rov_db_access-1.0.7/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     5878 2024-05-20 13:50:20.921035 rov_db_access-1.0.7/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0        0 2024-05-20 13:50:20.921067 rov_db_access-1.0.7/rov_db_access/utils/__init__.py
+-rw-r--r--   0        0        0     5317 2024-05-20 20:01:43.948847 rov_db_access-1.0.7/rov_db_access/utils/geoserver_utils.py
+-rw-r--r--   0        0        0     2078 2024-05-20 20:01:43.949178 rov_db_access-1.0.7/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1120 2024-05-20 13:50:20.921348 rov_db_access-1.0.7/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.7/PKG-INFO
```

### Comparing `rov_db_access-1.0.6/pyproject.toml` & `rov_db_access-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rov-db-access"
-version = "1.0.6"
+version = "1.0.7"
 description = ""
 authors = ["Pablo Cano <pablo.cano@rovisen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 geoalchemy2 = "^0.14.2"
```

### Comparing `rov_db_access-1.0.6/rov_db_access/authentication/models.py` & `rov_db_access-1.0.7/rov_db_access/authentication/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/authentication/worker.py` & `rov_db_access-1.0.7/rov_db_access/authentication/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/config/db_utils.py` & `rov_db_access-1.0.7/rov_db_access/config/db_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/config/settings.py` & `rov_db_access-1.0.7/rov_db_access/config/settings.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/geodata/models.py` & `rov_db_access-1.0.7/rov_db_access/geodata/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/gis/models.py` & `rov_db_access-1.0.7/rov_db_access/gis/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/gis/worker.py` & `rov_db_access-1.0.7/rov_db_access/gis/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,14 @@
                 return None
             else:
                 process_type = process_to_copy.type
                 new_name = "Copy of " + process_to_copy.name
                 model_id: int = process_to_copy.inference_model_id
                 area: float = process_to_copy.area
                 cost_estimated: float = process_to_copy.cost_estimated
-                data: dict = process_to_copy.data
                 geom: str = wkbelement_to_wkt(process_to_copy.geom)
                 mask = wkbelement_to_wkt(process_to_copy.mask)
                 print(f'Process with id: {process_to_copy.id} found! type: {process_type}')
 
                 if process_type == 'on demand':
                     process = Process(
                         name=new_name,
@@ -171,45 +170,48 @@
                         organization_id=process_to_copy.organization_id,
                         geom=geom,
                         mask=mask,
                         user_id=user.id
                     )
                     session.add(process)
 
-                    for run in process.runs:
+                    for run in process_to_copy.runs:
+                        print("BORRAR: run to copy: ", run)
                         new_output = RunData(
                             status="waiting",
                             type=run.output.type,
                             user_id=user.id,
                             organization_id=process_to_copy.organization_id,
                         )
                         new_run = Run(
+                            status='queued',
+                            runtime=run.runtime,
+                            engine=run.engine,
+                            cost=run.cost,
                             input=run.input,
                             output=new_output,
                             inference_model_id=run.inference_model_id,
-                            process=process,
+                            process=process
                         )
 
                         session.add(new_output)
                         session.add(new_run)
-
                     try:
                         session.commit()
                         return True
                     except Exception as error:
                         print("ERROR Create process. An exception occurred during DB insertion:", error)
                         return False
-                    
                 elif process_type == 'tasking':
                     data: CreateTaskingDict = {
                         "name": new_name,
                         "inference_model_id": model_id,
                         "area": area,
                         "cost_estimated": cost_estimated,
-                        "tasking_config": data,
+                        "tasking_config": {},  # TODO: esto hay que hacerlo bien
                         "geom": geom,
                         "mask": mask
                     }
                     return self.create_tasking(data, user)
                 else:
                     return False
 
@@ -403,17 +405,17 @@
 
     def get_inference_models(self):
         with Session(self.engine) as session:
             query = (
                 select(InferenceModel)
                 .order_by(InferenceModel.id)
             )
-            models = session.scalars(query)
-            if models is None:
-                return {}
+            models = session.scalars(query).all()
+            if models is None or len(models) == 0:
+                return []
             result = []
             for model in models:
                 result.append({
                     "id": model.id,
                     "name": model.name,
                     "title": model.title,
                     "description": model.description,
@@ -518,15 +520,14 @@
                     "status": process.status,
                     "type": process.type,
                     "created_at": process.created_at,
                     "finished_at": process.finished_at,
                     "runtime": process.runtime,
                     "area": process.area,
                     "cost_estimated": process.cost_estimated,
-                    "user": process.user.username,
                     "inference_model_id": process.inference_model_id,
                     "geom": geom,
                     "mask": mask,
                 }
 
     def load_processes_by_org(self, org_id: int):
         with Session(self.engine) as session:
@@ -554,15 +555,14 @@
                     "status": process.status,
                     "type": process.type,
                     "created_at": process.created_at,
                     "finished_at": process.finished_at,
                     "runtime": process.runtime,
                     "area": process.area,
                     "cost_estimated": process.cost_estimated,
-                    "user": process.user.username,
                     "inference_model_id": process.inference_model_id,
                     "geom": geom,
                     "mask": mask,
                 })
             return result
 
     def load_results_by_run_id(self, id: str):
@@ -754,39 +754,36 @@
                 session.commit()
                 return True
 
     def get_raster_img_url(self, id: str, user: User):
         with Session(self.engine) as session:
             raster = session.get(ResultsRaster, id)
             if raster is None:
-                print(f'No raster result with id ${id} found!')
+                print(f'No raster result with id: {id} found!')
                 return None
             else:
                 print(f'Raster result with id: {id} found!')
                 return raster.url
 
-    def get_run_data_preview(self, id: str, user: User):
+    def get_run_data_data(self, id: str, user: User):
         with Session(self.engine) as session:
             run_data = session.get(RunData, id)
             if run_data is None:
                 print(f'No run_data with id ${id} found!')
                 return None
             else:
                 print(f'Run_data with id: {id} found!')
                 data = run_data.data
                 if run_data.organization_id != user.organization_id:
                     print(f'No permission allowed for this user!')
                     return None
                 if data is None:
-                    print(f'No preview for run_data id ${id} found!')
+                    print(f'No data for run_data id ${id} found!')
                     return None
-                return {
-                    "bbox": data["bbox"],
-                    "preview": data["preview"]
-                }
+                return data
 
     def edit_process_name(self, id: str, name: str, user: User):
         with Session(self.engine) as session:
             query = (
                 select(Process)
                 .where(
                     and_(
```

### Comparing `rov_db_access-1.0.6/rov_db_access/ine/models.py` & `rov_db_access-1.0.7/rov_db_access/ine/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/ine/worker.py` & `rov_db_access-1.0.7/rov_db_access/ine/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/label_studio/models.py` & `rov_db_access-1.0.7/rov_db_access/label_studio/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/label_studio/worker.py` & `rov_db_access-1.0.7/rov_db_access/label_studio/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/landing/models.py` & `rov_db_access-1.0.7/rov_db_access/landing/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/landing/worker.py` & `rov_db_access-1.0.7/rov_db_access/landing/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/risks/models.py` & `rov_db_access-1.0.7/rov_db_access/risks/models.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/risks/worker.py` & `rov_db_access-1.0.7/rov_db_access/risks/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/sentinel/worker.py` & `rov_db_access-1.0.7/rov_db_access/sentinel/worker.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/utils/geoserver_utils.py` & `rov_db_access-1.0.7/rov_db_access/utils/geoserver_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/utils/s3_utils.py` & `rov_db_access-1.0.7/rov_db_access/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/rov_db_access/utils/utils.py` & `rov_db_access-1.0.7/rov_db_access/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rov_db_access-1.0.6/PKG-INFO` & `rov_db_access-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 1.0.6
+Version: 1.0.7
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

