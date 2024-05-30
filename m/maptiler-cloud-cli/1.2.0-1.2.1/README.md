# Comparing `tmp/maptiler_cloud_cli-1.2.0.tar.gz` & `tmp/maptiler_cloud_cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maptiler_cloud_cli-1.2.0.tar", max compression
+gzip compressed data, was "maptiler_cloud_cli-1.2.1.tar", max compression
```

## Comparing `maptiler_cloud_cli-1.2.0.tar` & `maptiler_cloud_cli-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2434 2023-08-23 13:56:40.543541 maptiler_cloud_cli-1.2.0/README.md
--rw-r--r--   0        0        0      693 2023-08-23 13:57:29.187910 maptiler_cloud_cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-08-21 09:41:05.423447 maptiler_cloud_cli-1.2.0/src/maptiler/cloud_cli/__init__.py
--rw-r--r--   0        0        0       42 2023-08-21 09:41:05.423447 maptiler_cloud_cli-1.2.0/src/maptiler/cloud_cli/__main__.py
--rw-r--r--   0        0        0     9874 2023-08-23 13:56:40.543541 maptiler_cloud_cli-1.2.0/src/maptiler/cloud_cli/base.py
--rw-r--r--   0        0        0     3237 1970-01-01 00:00:00.000000 maptiler_cloud_cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2434 2023-11-06 10:00:42.958026 maptiler_cloud_cli-1.2.1/README.md
+-rw-r--r--   0        0        0      693 2024-05-30 11:43:52.006300 maptiler_cloud_cli-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2021-11-15 07:52:04.479481 maptiler_cloud_cli-1.2.1/src/maptiler/cloud_cli/__init__.py
+-rw-r--r--   0        0        0       42 2021-11-15 07:52:04.479583 maptiler_cloud_cli-1.2.1/src/maptiler/cloud_cli/__main__.py
+-rw-r--r--   0        0        0    10081 2024-05-30 11:42:59.225369 maptiler_cloud_cli-1.2.1/src/maptiler/cloud_cli/base.py
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 maptiler_cloud_cli-1.2.1/PKG-INFO
```

### Comparing `maptiler_cloud_cli-1.2.0/README.md` & `maptiler_cloud_cli-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `maptiler_cloud_cli-1.2.0/pyproject.toml` & `maptiler_cloud_cli-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maptiler-cloud-cli"
-version = "1.2.0"
+version = "1.2.1"
 description = "CLI utility for MapTiler Cloud"
 authors = ["MapTiler <info@maptiler.com>"]
 packages = [{ include = "maptiler", from = "src" }]
 license = "MIT"
 repository = "https://github.com/maptiler/maptiler-cloud-cli"
 documentation = "https://docs.maptiler.com/cloud/admin-api/"
 readme = "README.md"
```

### Comparing `maptiler_cloud_cli-1.2.0/src/maptiler/cloud_cli/base.py` & `maptiler_cloud_cli-1.2.1/src/maptiler/cloud_cli/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 class S3UploadResult:
     parts: list[S3UploadResultPart]
 
 
 @dataclass
 class IngestResponse:
     id: UUID
-    document_id: UUID
+    document_id: Optional[UUID]
     state: str
     upload: Union[S3Upload, GoogleDriveUpload, None]
     errors: list[Error]
 
 
 class ClientError(Exception):
     status_code: int
@@ -113,17 +113,21 @@
             raise RuntimeError("Unknown upload type", data["upload"]["type"])
 
         if data.get("errors"):
             errors = [Error(item["message"]) for item in data["errors"]]
         else:
             errors = []
 
+        document_id = data.get("document_id")
+        if document_id is not None:
+            document_id = UUID(document_id)
+        
         return IngestResponse(
             id=UUID(data["id"]),
-            document_id=UUID(data["document_id"]),
+            document_id=document_id,
             state=data["state"],
             upload=upload,
             errors=errors,
         )
 
     def create_ingest(
         self, filename: str, size: int, document_id: Optional[UUID]
@@ -153,34 +157,34 @@
         )
         self.check(response)
         return self.ingest_response(response.json())
 
     def process_ingest(
         self, ingest_id: UUID, upload_result: Optional[S3UploadResult]
     ) -> IngestResponse:
+        url = urljoin(self.base_url, f"/v1/tiles/ingest/{ingest_id}/process")
         if upload_result is None:
-            json = None
+            response = self.session.post(url)
         else:
-            json = {
-                "upload_result": {
-                    "type": "s3_multipart",
-                    "parts": [
-                        {
-                            "part_id": item.part_id,
-                            "etag": item.etag,
-                        }
-                        for item in upload_result.parts
-                    ],
-                }
-            }
+            response = self.session.post(
+                url,
+                json={
+                    "upload_result": {
+                        "type": "s3_multipart",
+                        "parts": [
+                            {
+                                "part_id": item.part_id,
+                                "etag": item.etag,
+                            }
+                            for item in upload_result.parts
+                        ],
+                    }
+                },
+            )
 
-        response = self.session.post(
-            urljoin(self.base_url, f"/v1/tiles/ingest/{ingest_id}/process"),
-            json=json,
-        )
         self.check(response)
         return self.ingest_response(response.json())
 
 
 @click.group()
 @click.option("--token", type=str, envvar="MAPTILER_TOKEN", required=True)
 @click.option("--base-url", type=str, hidden=True)
```

### Comparing `maptiler_cloud_cli-1.2.0/PKG-INFO` & `maptiler_cloud_cli-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: maptiler-cloud-cli
-Version: 1.2.0
+Version: 1.2.1
 Summary: CLI utility for MapTiler Cloud
 Home-page: https://github.com/maptiler/maptiler-cloud-cli
 License: MIT
 Author: MapTiler
 Author-email: info@maptiler.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Project-URL: Documentation, https://docs.maptiler.com/cloud/admin-api/
 Project-URL: Repository, https://github.com/maptiler/maptiler-cloud-cli
 Description-Content-Type: text/markdown
 
 # MapTiler Cloud CLI
```

