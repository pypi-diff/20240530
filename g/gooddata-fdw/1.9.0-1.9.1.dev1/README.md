# Comparing `tmp/gooddata-fdw-1.9.0.tar.gz` & `tmp/gooddata-fdw-1.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-fdw-1.9.0.tar", last modified: Thu Nov 16 13:25:00 2023, max compression
+gzip compressed data, was "gooddata-fdw-1.9.1.dev1.tar", last modified: Thu Dec 14 13:21:11 2023, max compression
```

## Comparing `gooddata-fdw-1.9.0.tar` & `gooddata-fdw-1.9.1.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.256908 gooddata-fdw-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    39598 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-11-16 13:25:00.256908 gooddata-fdw-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.252908 gooddata-fdw-1.9.0/gooddata_fdw/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/column_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/column_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/fdw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/import_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/pg_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/gooddata_fdw/result_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 13:25:00.256908 gooddata-fdw-1.9.0/gooddata_fdw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-11-16 13:25:00.000000 gooddata-fdw-1.9.0/gooddata_fdw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-11-16 13:25:00.000000 gooddata-fdw-1.9.0/gooddata_fdw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 13:25:00.000000 gooddata-fdw-1.9.0/gooddata_fdw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-16 13:25:00.000000 gooddata-fdw-1.9.0/gooddata_fdw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-16 13:25:00.000000 gooddata-fdw-1.9.0/gooddata_fdw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-16 13:25:00.256908 gooddata-fdw-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2023-11-16 13:24:42.000000 gooddata-fdw-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:11.709154 gooddata-fdw-1.9.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    39598 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2023-12-14 13:21:11.709154 gooddata-fdw-1.9.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:11.705154 gooddata-fdw-1.9.1.dev1/gooddata_fdw/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/column_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/column_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/fdw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/import_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/pg_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-12-14 13:20:48.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw/result_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 13:21:11.709154 gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2023-12-14 13:21:11.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2023-12-14 13:21:11.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 13:21:11.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-14 13:21:11.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-14 13:21:11.000000 gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 13:21:11.709154 gooddata-fdw-1.9.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-12-14 13:21:04.000000 gooddata-fdw-1.9.1.dev1/setup.py
```

### Comparing `gooddata-fdw-1.9.0/LICENSE.txt` & `gooddata-fdw-1.9.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/PKG-INFO` & `gooddata-fdw-1.9.1.dev1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-fdw
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: GoodData Cloud Foreign Data Wrapper For PostgreSQL
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.9.0
+Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.9.1.dev1
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,fdw,postgresql,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-sdk~=1.9.0
+Requires-Dist: gooddata-sdk~=1.9.1.dev1
 
 # GoodData Foreign Data Wrapper
 
 This project delivers PostgreSQL foreign data wrapper extension built on top of [multicorn](https://multicorn.org/).
 The extension makes [GoodData](https://www.gooddata.com/docs/cloud/) insights, computations and ad-hoc report data available in PostgreSQL as tables.
 It can be selected like any other table using SQL language.
```

### Comparing `gooddata-fdw-1.9.0/README.md` & `gooddata-fdw-1.9.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/column_utils.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/column_utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/column_validation.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/column_validation.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/environment.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/environment.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/executor.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/executor.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/fdw.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/fdw.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/filter.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/import_workspace.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/import_workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/naming.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/naming.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/options.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/options.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/pg_logging.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/pg_logging.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw/result_reader.py` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw/result_reader.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw.egg-info/PKG-INFO` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-fdw
-Version: 1.9.0
+Version: 1.9.1.dev1
 Summary: GoodData Cloud Foreign Data Wrapper For PostgreSQL
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.9.0
+Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.9.1.dev1
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,fdw,postgresql,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: gooddata-sdk~=1.9.0
+Requires-Dist: gooddata-sdk~=1.9.1.dev1
 
 # GoodData Foreign Data Wrapper
 
 This project delivers PostgreSQL foreign data wrapper extension built on top of [multicorn](https://multicorn.org/).
 The extension makes [GoodData](https://www.gooddata.com/docs/cloud/) insights, computations and ad-hoc report data available in PostgreSQL as tables.
 It can be selected like any other table using SQL language.
```

### Comparing `gooddata-fdw-1.9.0/gooddata_fdw.egg-info/SOURCES.txt` & `gooddata-fdw-1.9.1.dev1/gooddata_fdw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.9.0/setup.py` & `gooddata-fdw-1.9.1.dev1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.9.0",
+    "gooddata-sdk~=1.9.1.dev1",
     #    "multicorn>=1.4.0",
 ]
 
 setup(
     name="gooddata-fdw",
     description="GoodData Cloud Foreign Data Wrapper For PostgreSQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.9.0",
+    version="1.9.1.dev1",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.8.0",
     project_urls={
-        "Documentation": "https://gooddata-fdw.readthedocs.io/en/v1.9.0",
+        "Documentation": "https://gooddata-fdw.readthedocs.io/en/v1.9.1.dev1",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
```

