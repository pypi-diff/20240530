# Comparing `tmp/near_lake_framework-0.1.0.tar.gz` & `tmp/near_lake_framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "near_lake_framework-0.1.0.tar", last modified: Wed May 29 14:51:40 2024, max compression
+gzip compressed data, was "near_lake_framework-0.1.1.tar", last modified: Thu May 30 15:50:44 2024, max compression
```

## Comparing `near_lake_framework-0.1.0.tar` & `near_lake_framework-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:51:40.577566 near_lake_framework-0.1.0/
--rw-r--r--   0 frolik     (501) staff       (20)     9722 2023-10-15 22:01:13.000000 near_lake_framework-0.1.0/LICENSE-APACHE
--rw-r--r--   0 frolik     (501) staff       (20)     5092 2024-05-29 14:51:40.577494 near_lake_framework-0.1.0/PKG-INFO
--rw-r--r--   0 frolik     (501) staff       (20)     4283 2024-05-29 14:09:55.000000 near_lake_framework-0.1.0/README.md
--rw-r--r--   0 frolik     (501) staff       (20)      110 2024-05-29 14:51:40.577820 near_lake_framework-0.1.0/setup.cfg
--rw-r--r--   0 frolik     (501) staff       (20)     1167 2024-05-29 14:50:49.000000 near_lake_framework-0.1.0/setup.py
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:51:40.574939 near_lake_framework-0.1.0/src/
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:51:40.576321 near_lake_framework-0.1.0/src/near_lake_framework/
--rw-r--r--   0 frolik     (501) staff       (20)     5134 2024-05-29 14:26:30.000000 near_lake_framework-0.1.0/src/near_lake_framework/__init__.py
--rw-r--r--   0 frolik     (501) staff       (20)     4967 2024-05-29 14:10:02.000000 near_lake_framework-0.1.0/src/near_lake_framework/near_primitives.py
--rw-r--r--   0 frolik     (501) staff       (20)        0 2024-04-25 16:39:35.000000 near_lake_framework-0.1.0/src/near_lake_framework/py.typed
--rw-r--r--   0 frolik     (501) staff       (20)     2865 2024-05-29 14:21:47.000000 near_lake_framework-0.1.0/src/near_lake_framework/s3_fetchers.py
--rw-r--r--   0 frolik     (501) staff       (20)      992 2024-05-29 14:09:55.000000 near_lake_framework-0.1.0/src/near_lake_framework/utils.py
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:51:40.577251 near_lake_framework-0.1.0/src/near_lake_framework.egg-info/
--rw-r--r--   0 frolik     (501) staff       (20)     5092 2024-05-29 14:51:40.000000 near_lake_framework-0.1.0/src/near_lake_framework.egg-info/PKG-INFO
--rw-r--r--   0 frolik     (501) staff       (20)      461 2024-05-29 14:51:40.000000 near_lake_framework-0.1.0/src/near_lake_framework.egg-info/SOURCES.txt
--rw-r--r--   0 frolik     (501) staff       (20)        1 2024-05-29 14:51:40.000000 near_lake_framework-0.1.0/src/near_lake_framework.egg-info/dependency_links.txt
--rw-r--r--   0 frolik     (501) staff       (20)       92 2024-05-29 14:51:40.000000 near_lake_framework-0.1.0/src/near_lake_framework.egg-info/requires.txt
--rw-r--r--   0 frolik     (501) staff       (20)       20 2024-05-29 14:51:40.000000 near_lake_framework-0.1.0/src/near_lake_framework.egg-info/top_level.txt
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-30 15:50:44.021339 near_lake_framework-0.1.1/
+-rw-r--r--   0 frolik     (501) staff       (20)     9722 2023-10-15 22:01:13.000000 near_lake_framework-0.1.1/LICENSE-APACHE
+-rw-r--r--   0 frolik     (501) staff       (20)     5092 2024-05-30 15:50:44.021272 near_lake_framework-0.1.1/PKG-INFO
+-rw-r--r--   0 frolik     (501) staff       (20)     4283 2024-05-29 14:09:55.000000 near_lake_framework-0.1.1/README.md
+-rw-r--r--   0 frolik     (501) staff       (20)      110 2024-05-30 15:50:44.021555 near_lake_framework-0.1.1/setup.cfg
+-rw-r--r--   0 frolik     (501) staff       (20)     1167 2024-05-30 15:50:17.000000 near_lake_framework-0.1.1/setup.py
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-30 15:50:44.018878 near_lake_framework-0.1.1/src/
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-30 15:50:44.020194 near_lake_framework-0.1.1/src/near_lake_framework/
+-rw-r--r--   0 frolik     (501) staff       (20)     5134 2024-05-29 14:26:30.000000 near_lake_framework-0.1.1/src/near_lake_framework/__init__.py
+-rw-r--r--   0 frolik     (501) staff       (20)     4967 2024-05-29 14:10:02.000000 near_lake_framework-0.1.1/src/near_lake_framework/near_primitives.py
+-rw-r--r--   0 frolik     (501) staff       (20)        0 2024-04-25 16:39:35.000000 near_lake_framework-0.1.1/src/near_lake_framework/py.typed
+-rw-r--r--   0 frolik     (501) staff       (20)     2863 2024-05-30 15:50:06.000000 near_lake_framework-0.1.1/src/near_lake_framework/s3_fetchers.py
+-rw-r--r--   0 frolik     (501) staff       (20)      992 2024-05-29 14:09:55.000000 near_lake_framework-0.1.1/src/near_lake_framework/utils.py
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-30 15:50:44.021045 near_lake_framework-0.1.1/src/near_lake_framework.egg-info/
+-rw-r--r--   0 frolik     (501) staff       (20)     5092 2024-05-30 15:50:44.000000 near_lake_framework-0.1.1/src/near_lake_framework.egg-info/PKG-INFO
+-rw-r--r--   0 frolik     (501) staff       (20)      461 2024-05-30 15:50:44.000000 near_lake_framework-0.1.1/src/near_lake_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 frolik     (501) staff       (20)        1 2024-05-30 15:50:44.000000 near_lake_framework-0.1.1/src/near_lake_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 frolik     (501) staff       (20)       92 2024-05-30 15:50:44.000000 near_lake_framework-0.1.1/src/near_lake_framework.egg-info/requires.txt
+-rw-r--r--   0 frolik     (501) staff       (20)       20 2024-05-30 15:50:44.000000 near_lake_framework-0.1.1/src/near_lake_framework.egg-info/top_level.txt
```

### Comparing `near_lake_framework-0.1.0/LICENSE-APACHE` & `near_lake_framework-0.1.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `near_lake_framework-0.1.0/PKG-INFO` & `near_lake_framework-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: near-lake-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Library to connect to the NEAR Lake S3 and stream the data
 Home-page: https://github.com/frolvanya/near-lake-framework-py
 Author: Ivan Frolov
 Author-email: frolvanya@gmail.com
 Project-URL: Bug Tracker, https://github.com/frolvanya/near-lake-framework-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `near_lake_framework-0.1.0/README.md` & `near_lake_framework-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `near_lake_framework-0.1.0/setup.py` & `near_lake_framework-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="near-lake-framework",
-    version="0.1.0",
+    version="0.1.1",
     author="Ivan Frolov",
     author_email="frolvanya@gmail.com",
     description="Python Library to connect to the NEAR Lake S3 and stream the data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/frolvanya/near-lake-framework-py",
     project_urls={
```

### Comparing `near_lake_framework-0.1.0/src/near_lake_framework/__init__.py` & `near_lake_framework-0.1.1/src/near_lake_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `near_lake_framework-0.1.0/src/near_lake_framework/near_primitives.py` & `near_lake_framework-0.1.1/src/near_lake_framework/near_primitives.py`

 * *Files identical despite different names*

### Comparing `near_lake_framework-0.1.0/src/near_lake_framework/s3_fetchers.py` & `near_lake_framework-0.1.1/src/near_lake_framework/s3_fetchers.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
             async with response["Body"] as stream:
                 body = await stream.read()
 
             return near_primitives.IndexerShard.from_json(body)
         except ClientError as e:
             if e.response["Error"]["Code"] == "NoSuchKey":
-                logging.warning("Failed to fetch shard %s - doesn't exist", shard_key)
+                logging.debug("Failed to fetch shard %s - doesn't exist", shard_key)
             else:
                 traceback.print_exc()
         except EndpointConnectionError as e:
             logging.error(
                 "EndpointConnectionError while fetching shard %s: %s", shard_key, e
             )
             traceback.print_exc()
```

### Comparing `near_lake_framework-0.1.0/src/near_lake_framework/utils.py` & `near_lake_framework-0.1.1/src/near_lake_framework/utils.py`

 * *Files identical despite different names*

### Comparing `near_lake_framework-0.1.0/src/near_lake_framework.egg-info/PKG-INFO` & `near_lake_framework-0.1.1/src/near_lake_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: near-lake-framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Library to connect to the NEAR Lake S3 and stream the data
 Home-page: https://github.com/frolvanya/near-lake-framework-py
 Author: Ivan Frolov
 Author-email: frolvanya@gmail.com
 Project-URL: Bug Tracker, https://github.com/frolvanya/near-lake-framework-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

