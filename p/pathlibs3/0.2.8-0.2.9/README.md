# Comparing `tmp/pathlibs3-0.2.8.tar.gz` & `tmp/pathlibs3-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.8.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.9.tar", max compression
```

## Comparing `pathlibs3-0.2.8.tar` & `pathlibs3-0.2.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1690 2024-05-30 12:32:17.840094 pathlibs3-0.2.8/README.md
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.8/pathlibs3/__init__.py
--rw-r--r--   0        0        0     4661 2024-05-30 12:56:04.042825 pathlibs3-0.2.8/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      654 2024-05-30 12:52:09.792720 pathlibs3-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 pathlibs3-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1881 2024-05-30 13:05:28.909683 pathlibs3-0.2.9/README.md
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.9/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     4661 2024-05-30 12:56:04.042825 pathlibs3-0.2.9/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      710 2024-05-30 16:41:15.213353 pathlibs3-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 pathlibs3-0.2.9/PKG-INFO
```

### Comparing `pathlibs3-0.2.8/README.md` & `pathlibs3-0.2.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -71,12 +71,14 @@
 # Create another pathlibs3 object
 s3_path_to_anotherfolder = S3Path(client, bucket, "anotherfolder/")
 
 # Will download the s3 folder localy
 S3Path.copy(s3_path_to_myfolder, s3_path_to_anotherfolder)
 ```
 
+## How pathlibS3 distinguish file from folder
 
+> :warning: PathlibS3 will distinguish folder from file using this simple rule: if a path end with "/" then it is a folder, if not it is a file.
 
 # run test
 
 run test with `poetry run python -m pytest`
```

### Comparing `pathlibs3-0.2.8/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.9/pathlibs3/pathlibs3.py`

 * *Files identical despite different names*

### Comparing `pathlibs3-0.2.8/pyproject.toml` & `pathlibs3-0.2.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "pathlibs3"
-version = "0.2.8"
+version = "0.2.9"
 description = "S3 navigation using object, inspired by pathlib.Path"
 authors = ["thibault.blanc"]
 readme = "README.md"
+homepage = "https://github.com/thibaultbl/s3_navigator"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 boto3 = "*"
 urllib3 = "*"
 
 Sphinx = { version = "4.2.0", optional = true }
```

