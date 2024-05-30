# Comparing `tmp/cmdbapi-1.0.1.tar.gz` & `tmp/cmdbapi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmdbapi-1.0.1.tar", last modified: Thu May 30 07:55:16 2024, max compression
+gzip compressed data, was "dist/cmdbapi-1.0.2.tar", last modified: Thu May 30 08:26:07 2024, max compression
```

## Comparing `cmdbapi-1.0.1.tar` & `cmdbapi-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 lpa       (1002) lpa       (1002)        0 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/
--rw-r--r--   0 lpa       (1002) lpa       (1002)      851 2024-05-30 07:54:17.000000 cmdbapi-1.0.1/setup.py
-drwxrwxr-x   0 lpa       (1002) lpa       (1002)        0 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/cmdbapi.egg-info/
--rw-rw-r--   0 lpa       (1002) lpa       (1002)       17 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/cmdbapi.egg-info/requires.txt
--rw-rw-r--   0 lpa       (1002) lpa       (1002)        8 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/cmdbapi.egg-info/top_level.txt
--rw-rw-r--   0 lpa       (1002) lpa       (1002)     4068 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/cmdbapi.egg-info/PKG-INFO
--rw-rw-r--   0 lpa       (1002) lpa       (1002)        1 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/cmdbapi.egg-info/dependency_links.txt
--rw-rw-r--   0 lpa       (1002) lpa       (1002)      241 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/cmdbapi.egg-info/SOURCES.txt
--rw-r--r--   0 lpa       (1002) lpa       (1002)       34 2024-05-30 05:16:34.000000 cmdbapi-1.0.1/MANIFEST.in
--rw-rw-r--   0 lpa       (1002) lpa       (1002)     4068 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/PKG-INFO
--rw-r--r--   0 lpa       (1002) lpa       (1002)       38 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/setup.cfg
-drwxrwxr-x   0 lpa       (1002) lpa       (1002)        0 2024-05-30 07:55:16.000000 cmdbapi-1.0.1/cmdbapi/
--rw-r--r--   0 lpa       (1002) lpa       (1002)        0 2024-05-30 05:14:59.000000 cmdbapi-1.0.1/cmdbapi/__init__.py
--rw-rw-r--   0 lpa       (1002) lpa       (1002)     4372 2024-05-30 06:48:01.000000 cmdbapi-1.0.1/cmdbapi/cmdbapi.py
--rw-rw-r--   0 lpa       (1002) lpa       (1002)     1073 2023-04-19 08:30:31.000000 cmdbapi-1.0.1/LICENSE
--rw-r--r--   0 lpa       (1002) lpa       (1002)     2925 2024-05-30 07:21:08.000000 cmdbapi-1.0.1/README.md
+drwxrwxr-x   0 lpa       (1002) lpa       (1002)        0 2024-05-30 08:26:07.000000 cmdbapi-1.0.2/
+-rw-r--r--   0 lpa       (1002) lpa       (1002)      851 2024-05-30 08:25:55.000000 cmdbapi-1.0.2/setup.py
+drwxrwxr-x   0 lpa       (1002) lpa       (1002)        0 2024-05-30 08:26:07.000000 cmdbapi-1.0.2/cmdbapi.egg-info/
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)       17 2024-05-30 08:26:06.000000 cmdbapi-1.0.2/cmdbapi.egg-info/requires.txt
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)        8 2024-05-30 08:26:06.000000 cmdbapi-1.0.2/cmdbapi.egg-info/top_level.txt
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)     4068 2024-05-30 08:26:06.000000 cmdbapi-1.0.2/cmdbapi.egg-info/PKG-INFO
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)        1 2024-05-30 08:26:06.000000 cmdbapi-1.0.2/cmdbapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)      241 2024-05-30 08:26:06.000000 cmdbapi-1.0.2/cmdbapi.egg-info/SOURCES.txt
+-rw-r--r--   0 lpa       (1002) lpa       (1002)       34 2024-05-30 05:16:34.000000 cmdbapi-1.0.2/MANIFEST.in
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)     4068 2024-05-30 08:26:07.000000 cmdbapi-1.0.2/PKG-INFO
+-rw-r--r--   0 lpa       (1002) lpa       (1002)       38 2024-05-30 08:26:07.000000 cmdbapi-1.0.2/setup.cfg
+drwxrwxr-x   0 lpa       (1002) lpa       (1002)        0 2024-05-30 08:26:07.000000 cmdbapi-1.0.2/cmdbapi/
+-rw-r--r--   0 lpa       (1002) lpa       (1002)       28 2024-05-30 08:25:47.000000 cmdbapi-1.0.2/cmdbapi/__init__.py
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)     4372 2024-05-30 06:48:01.000000 cmdbapi-1.0.2/cmdbapi/cmdbapi.py
+-rw-rw-r--   0 lpa       (1002) lpa       (1002)     1073 2023-04-19 08:30:31.000000 cmdbapi-1.0.2/LICENSE
+-rw-r--r--   0 lpa       (1002) lpa       (1002)     2925 2024-05-30 07:21:08.000000 cmdbapi-1.0.2/README.md
```

### Comparing `cmdbapi-1.0.1/setup.py` & `cmdbapi-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cmdbapi",  
-    version="1.0.1",
+    version="1.0.2",
     author="Pavlo Lashkevych",
     author_email="laspavel@gmail.com",
     description="A short library for working CMDB API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/laspavel/cmdbapi",
     packages=find_packages(),
```

### Comparing `cmdbapi-1.0.1/cmdbapi.egg-info/PKG-INFO` & `cmdbapi-1.0.2/cmdbapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdbapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: A short library for working CMDB API
 Home-page: https://github.com/laspavel/cmdbapi
 Author: Pavlo Lashkevych
 Author-email: laspavel@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/laspavel/cmdbapi/blob/master/README.md
 Description: s# CMDBAPI
```

### Comparing `cmdbapi-1.0.1/PKG-INFO` & `cmdbapi-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdbapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: A short library for working CMDB API
 Home-page: https://github.com/laspavel/cmdbapi
 Author: Pavlo Lashkevych
 Author-email: laspavel@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/laspavel/cmdbapi/blob/master/README.md
 Description: s# CMDBAPI
```

### Comparing `cmdbapi-1.0.1/cmdbapi/cmdbapi.py` & `cmdbapi-1.0.2/cmdbapi/cmdbapi.py`

 * *Files identical despite different names*

### Comparing `cmdbapi-1.0.1/LICENSE` & `cmdbapi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdbapi-1.0.1/README.md` & `cmdbapi-1.0.2/README.md`

 * *Files identical despite different names*

