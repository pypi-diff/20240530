# Comparing `tmp/coderdata-0.1.8.tar.gz` & `tmp/coderdata-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderdata-0.1.8.tar", last modified: Fri Dec 29 20:01:59 2023, max compression
+gzip compressed data, was "coderdata-0.1.9.tar", last modified: Tue Jan  2 21:51:22 2024, max compression
```

## Comparing `coderdata-0.1.8.tar` & `coderdata-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.829892 coderdata-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2023-12-29 20:01:42.000000 coderdata-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2023-12-29 20:01:59.829892 coderdata-0.1.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2889 2023-12-29 20:01:42.000000 coderdata-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.825892 coderdata-0.1.8/coderdata/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.825892 coderdata-0.1.8/coderdata/builder/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.825892 coderdata-0.1.8/coderdata/download/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/download/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.829892 coderdata-0.1.8/coderdata/load/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.829892 coderdata-0.1.8/coderdata/reformat/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-29 20:01:42.000000 coderdata-0.1.8/coderdata/reformat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.825892 coderdata-0.1.8/coderdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2023-12-29 20:01:59.000000 coderdata-0.1.8/coderdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-29 20:01:59.000000 coderdata-0.1.8/coderdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 20:01:59.000000 coderdata-0.1.8/coderdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-29 20:01:59.000000 coderdata-0.1.8/coderdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-29 20:01:59.000000 coderdata-0.1.8/coderdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-29 20:01:59.000000 coderdata-0.1.8/coderdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 20:01:59.829892 coderdata-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-29 20:01:56.000000 coderdata-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:59.829892 coderdata-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_and_load_beataml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_and_load_cell_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_and_load_cptac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_and_load_hcmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_beataml_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_cell_line_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_cptac_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-29 20:01:42.000000 coderdata-0.1.8/tests/test_download_hcmi_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.643750 coderdata-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-01-02 21:51:10.000000 coderdata-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-02 21:51:22.643750 coderdata-0.1.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2889 2024-01-02 21:51:10.000000 coderdata-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.639750 coderdata-0.1.9/coderdata/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.639750 coderdata-0.1.9/coderdata/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.639750 coderdata-0.1.9/coderdata/download/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/download/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.639750 coderdata-0.1.9/coderdata/load/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/load/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.639750 coderdata-0.1.9/coderdata/reformat/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-02 21:51:10.000000 coderdata-0.1.9/coderdata/reformat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.639750 coderdata-0.1.9/coderdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-02 21:51:22.000000 coderdata-0.1.9/coderdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-01-02 21:51:22.000000 coderdata-0.1.9/coderdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 21:51:22.000000 coderdata-0.1.9/coderdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-02 21:51:22.000000 coderdata-0.1.9/coderdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-02 21:51:22.000000 coderdata-0.1.9/coderdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-02 21:51:22.000000 coderdata-0.1.9/coderdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-02 21:51:22.643750 coderdata-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-02 21:51:20.000000 coderdata-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:22.643750 coderdata-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_and_load_beataml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_and_load_cell_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_and_load_cptac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_and_load_hcmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_beataml_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_cell_line_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_cptac_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-01-02 21:51:10.000000 coderdata-0.1.9/tests/test_download_hcmi_cli.py
```

### Comparing `coderdata-0.1.8/LICENSE` & `coderdata-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/PKG-INFO` & `coderdata-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderdata
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to download, load, and process multiple benchmark multi-omic drug response datasets
 Home-page: https://github.com/PNNL-CompBio/candleDataProcessing
 Author: Jeremy Jacobson
 Author-email: jeremy.jacobson@pnnl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `coderdata-0.1.8/README.md` & `coderdata-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/coderdata/cli.py` & `coderdata-0.1.9/coderdata/cli.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/coderdata/download/downloader.py` & `coderdata-0.1.9/coderdata/download/downloader.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/coderdata/load/loader.py` & `coderdata-0.1.9/coderdata/load/loader.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/coderdata.egg-info/PKG-INFO` & `coderdata-0.1.9/coderdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coderdata
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to download, load, and process multiple benchmark multi-omic drug response datasets
 Home-page: https://github.com/PNNL-CompBio/candleDataProcessing
 Author: Jeremy Jacobson
 Author-email: jeremy.jacobson@pnnl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `coderdata-0.1.8/coderdata.egg-info/SOURCES.txt` & `coderdata-0.1.9/coderdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/setup.py` & `coderdata-0.1.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='coderdata',  
-    version='0.1.8',   
+    version='0.1.9',   
     author='Jeremy Jacobson',
     author_email='jeremy.jacobson@pnnl.gov',
     description='A package to download, load, and process multiple benchmark multi-omic drug response datasets',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/PNNL-CompBio/candleDataProcessing',
     packages = find_packages(),
```

### Comparing `coderdata-0.1.8/tests/test_download_and_load_beataml.py` & `coderdata-0.1.9/tests/test_download_and_load_beataml.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/tests/test_download_and_load_cell_line.py` & `coderdata-0.1.9/tests/test_download_and_load_cell_line.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/tests/test_download_and_load_cptac.py` & `coderdata-0.1.9/tests/test_download_and_load_cptac.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/tests/test_download_and_load_hcmi.py` & `coderdata-0.1.9/tests/test_download_and_load_hcmi.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/tests/test_download_beataml_cli.py` & `coderdata-0.1.9/tests/test_download_beataml_cli.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/tests/test_download_cell_line_cli.py` & `coderdata-0.1.9/tests/test_download_cell_line_cli.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/tests/test_download_cptac_cli.py` & `coderdata-0.1.9/tests/test_download_cptac_cli.py`

 * *Files identical despite different names*

### Comparing `coderdata-0.1.8/tests/test_download_hcmi_cli.py` & `coderdata-0.1.9/tests/test_download_hcmi_cli.py`

 * *Files identical despite different names*

