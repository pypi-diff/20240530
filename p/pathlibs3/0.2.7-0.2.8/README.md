# Comparing `tmp/pathlibs3-0.2.7.tar.gz` & `tmp/pathlibs3-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.7.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.8.tar", max compression
```

## Comparing `pathlibs3-0.2.7.tar` & `pathlibs3-0.2.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1652 2024-05-30 09:52:58.162711 pathlibs3-0.2.7/README.md
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.7/pathlibs3/__init__.py
--rw-r--r--   0        0        0     4636 2024-05-16 16:55:44.797522 pathlibs3-0.2.7/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      654 2024-05-30 09:53:04.286602 pathlibs3-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 pathlibs3-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1690 2024-05-30 12:32:17.840094 pathlibs3-0.2.8/README.md
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.8/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     4661 2024-05-30 12:56:04.042825 pathlibs3-0.2.8/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      654 2024-05-30 12:52:09.792720 pathlibs3-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 pathlibs3-0.2.8/PKG-INFO
```

### Comparing `pathlibs3-0.2.7/README.md` & `pathlibs3-0.2.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pip install pathlibs3
 ```
 
 # Usage
 
 ## Create a PathlibS3 Object
 ```python
-
+from pathlibs3.pathlibs3 import S3Path
 # Create a pathlibs3
 
 client = boto3.client("s3", region_name="us-east-1")
 bucket = "test-bucket"
 
 # Create an object to s3://test-bucket/myfolder/random_file.txt
 s3_path_to_myfolder = S3Path(client, bucket, "myfolder/")
```

### Comparing `pathlibs3-0.2.7/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.8/pathlibs3/pathlibs3.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     def name(self):
         return Path(self.path).name
 
     def __truediv__(self, other: str) -> "S3Path":
         return S3Path(
             client=self.client,
             bucket=self.bucket,
-            path=str(Path(self.path) / other),
+            path=f"{self.path}/{other}".replace("//", "/").lstrip("/"),
         )
 
     @classmethod
     def _copy_from_s3_to_s3(cls, source: "S3Path", destination: "S3Path"):
         client = source.client
         copy_source = {"Bucket": source.bucket, "Key": source.path}
         client.copy(copy_source, destination.bucket, destination.path)
```

### Comparing `pathlibs3-0.2.7/pyproject.toml` & `pathlibs3-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pathlibs3"
-version = "0.2.7"
+version = "0.2.8"
 description = "S3 navigation using object, inspired by pathlib.Path"
 authors = ["thibault.blanc"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 boto3 = "*"
```

### Comparing `pathlibs3-0.2.7/PKG-INFO` & `pathlibs3-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathlibs3
-Version: 0.2.7
+Version: 0.2.8
 Summary: S3 navigation using object, inspired by pathlib.Path
 Author: thibault.blanc
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
@@ -21,15 +21,15 @@
 pip install pathlibs3
 ```
 
 # Usage
 
 ## Create a PathlibS3 Object
 ```python
-
+from pathlibs3.pathlibs3 import S3Path
 # Create a pathlibs3
 
 client = boto3.client("s3", region_name="us-east-1")
 bucket = "test-bucket"
 
 # Create an object to s3://test-bucket/myfolder/random_file.txt
 s3_path_to_myfolder = S3Path(client, bucket, "myfolder/")
```

