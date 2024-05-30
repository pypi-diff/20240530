# Comparing `tmp/pyplate_hte-0.4.2.tar.gz` & `tmp/pyplate_hte-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplate_hte-0.4.2.tar", last modified: Thu May 30 19:01:35 2024, max compression
+gzip compressed data, was "pyplate_hte-0.4.3.tar", last modified: Thu May 30 19:08:00 2024, max compression
```

## Comparing `pyplate_hte-0.4.2.tar` & `pyplate_hte-0.4.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.338218 pyplate_hte-0.4.2/
--rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-01-28 17:38:34.000000 pyplate_hte-0.4.2/LICENSE.txt
--rw-r--r--   0 marvinj    (502) staff       (20)    15695 2024-05-30 19:01:35.336542 pyplate_hte-0.4.2/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)     2944 2024-04-15 03:08:55.000000 pyplate_hte-0.4.2/README.md
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.247036 pyplate_hte-0.4.2/pyplate/
--rw-r--r--   0 marvinj    (502) staff       (20)     2301 2024-05-30 18:57:49.000000 pyplate_hte-0.4.2/pyplate/__init__.py
--rw-r--r--   0 marvinj    (502) staff       (20)    12580 2024-05-30 18:53:20.000000 pyplate_hte-0.4.2/pyplate/experiment_design.py
--rw-r--r--   0 marvinj    (502) staff       (20)   131169 2024-05-30 18:53:20.000000 pyplate_hte-0.4.2/pyplate/pyplate.py
--rw-r--r--   0 marvinj    (502) staff       (20)      940 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/pyplate/pyplate.yaml
--rw-r--r--   0 marvinj    (502) staff       (20)    14330 2024-05-30 18:53:20.000000 pyplate_hte-0.4.2/pyplate/slicer.py
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.333878 pyplate_hte-0.4.2/pyplate_hte.egg-info/
--rw-r--r--   0 marvinj    (502) staff       (20)    15695 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)      739 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/SOURCES.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/dependency_links.txt
--rw-r--r--   0 marvinj    (502) staff       (20)       20 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/requires.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-05-30 19:01:35.000000 pyplate_hte-0.4.2/pyplate_hte.egg-info/top_level.txt
--rw-r--r--   0 marvinj    (502) staff       (20)      689 2024-05-30 18:41:13.000000 pyplate_hte-0.4.2/pyproject.toml
--rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-05-30 19:01:35.338421 pyplate_hte-0.4.2/setup.cfg
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:01:35.293187 pyplate_hte-0.4.2/tests/
--rw-r--r--   0 marvinj    (502) staff       (20)    15601 2024-05-16 22:26:42.000000 pyplate_hte-0.4.2/tests/test_Container.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5325 2024-04-15 02:14:28.000000 pyplate_hte-0.4.2/tests/test_Plate.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6607 2024-04-19 03:26:45.000000 pyplate_hte-0.4.2/tests/test_Recipe.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-03-13 22:47:19.000000 pyplate_hte-0.4.2/tests/test_Slicer.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3869 2024-04-15 03:08:55.000000 pyplate_hte-0.4.2/tests/test_Substance.py
--rw-r--r--   0 marvinj    (502) staff       (20)     2877 2024-04-15 03:08:55.000000 pyplate_hte-0.4.2/tests/test_convert.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3738 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_create_solution.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1352 2024-04-15 02:14:28.000000 pyplate_hte-0.4.2/tests/test_dilute.py
--rw-r--r--   0 marvinj    (502) staff       (20)      939 2024-04-04 18:26:24.000000 pyplate_hte-0.4.2/tests/test_eugene.py
--rw-r--r--   0 marvinj    (502) staff       (20)     4235 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_get_substance_used2.py
--rw-r--r--   0 marvinj    (502) staff       (20)     2268 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_recipe_amount_remaining.py
--rw-r--r--   0 marvinj    (502) staff       (20)    12757 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_recipe_get_container_flows.py
--rw-r--r--   0 marvinj    (502) staff       (20)    27431 2024-05-06 17:36:49.000000 pyplate_hte-0.4.2/tests/test_recipe_get_substance_used.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5796 2024-04-15 02:14:28.000000 pyplate_hte-0.4.2/tests/test_transfers.py
--rw-r--r--   0 marvinj    (502) staff       (20)      501 2024-05-16 22:26:42.000000 pyplate_hte-0.4.2/tests/test_volume_used_Plate_transfer.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:08:00.326707 pyplate_hte-0.4.3/
+-rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-01-28 17:38:34.000000 pyplate_hte-0.4.3/LICENSE.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)    15719 2024-05-30 19:08:00.325137 pyplate_hte-0.4.3/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)     2944 2024-04-15 03:08:55.000000 pyplate_hte-0.4.3/README.md
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:08:00.291033 pyplate_hte-0.4.3/pyplate/
+-rw-r--r--   0 marvinj    (502) staff       (20)     2301 2024-05-30 18:57:49.000000 pyplate_hte-0.4.3/pyplate/__init__.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    12580 2024-05-30 18:53:20.000000 pyplate_hte-0.4.3/pyplate/experiment_design.py
+-rw-r--r--   0 marvinj    (502) staff       (20)   131169 2024-05-30 18:53:20.000000 pyplate_hte-0.4.3/pyplate/pyplate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      940 2024-05-06 17:36:49.000000 pyplate_hte-0.4.3/pyplate/pyplate.yaml
+-rw-r--r--   0 marvinj    (502) staff       (20)    14330 2024-05-30 18:53:20.000000 pyplate_hte-0.4.3/pyplate/slicer.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:08:00.323386 pyplate_hte-0.4.3/pyplate_hte.egg-info/
+-rw-r--r--   0 marvinj    (502) staff       (20)    15719 2024-05-30 19:08:00.000000 pyplate_hte-0.4.3/pyplate_hte.egg-info/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)      739 2024-05-30 19:08:00.000000 pyplate_hte-0.4.3/pyplate_hte.egg-info/SOURCES.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-05-30 19:08:00.000000 pyplate_hte-0.4.3/pyplate_hte.egg-info/dependency_links.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)       29 2024-05-30 19:08:00.000000 pyplate_hte-0.4.3/pyplate_hte.egg-info/requires.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-05-30 19:08:00.000000 pyplate_hte-0.4.3/pyplate_hte.egg-info/top_level.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)      706 2024-05-30 19:07:21.000000 pyplate_hte-0.4.3/pyproject.toml
+-rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-05-30 19:08:00.326970 pyplate_hte-0.4.3/setup.cfg
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-05-30 19:08:00.321151 pyplate_hte-0.4.3/tests/
+-rw-r--r--   0 marvinj    (502) staff       (20)    15601 2024-05-16 22:26:42.000000 pyplate_hte-0.4.3/tests/test_Container.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5325 2024-04-15 02:14:28.000000 pyplate_hte-0.4.3/tests/test_Plate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6607 2024-04-19 03:26:45.000000 pyplate_hte-0.4.3/tests/test_Recipe.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-03-13 22:47:19.000000 pyplate_hte-0.4.3/tests/test_Slicer.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3869 2024-04-15 03:08:55.000000 pyplate_hte-0.4.3/tests/test_Substance.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     2877 2024-04-15 03:08:55.000000 pyplate_hte-0.4.3/tests/test_convert.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3738 2024-05-06 17:36:49.000000 pyplate_hte-0.4.3/tests/test_create_solution.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1352 2024-04-15 02:14:28.000000 pyplate_hte-0.4.3/tests/test_dilute.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      939 2024-04-04 18:26:24.000000 pyplate_hte-0.4.3/tests/test_eugene.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     4235 2024-05-06 17:36:49.000000 pyplate_hte-0.4.3/tests/test_get_substance_used2.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     2268 2024-05-06 17:36:49.000000 pyplate_hte-0.4.3/tests/test_recipe_amount_remaining.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    12757 2024-05-06 17:36:49.000000 pyplate_hte-0.4.3/tests/test_recipe_get_container_flows.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    27431 2024-05-06 17:36:49.000000 pyplate_hte-0.4.3/tests/test_recipe_get_substance_used.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5796 2024-04-15 02:14:28.000000 pyplate_hte-0.4.3/tests/test_transfers.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      501 2024-05-16 22:26:42.000000 pyplate_hte-0.4.3/tests/test_volume_used_Plate_transfer.py
```

### Comparing `pyplate_hte-0.4.2/LICENSE.txt` & `pyplate_hte-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/PKG-INFO` & `pyplate_hte-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -198,14 +198,15 @@
 Project-URL: Repository, https://github.com/ekwan/PyPlate
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyyaml
+Requires-Dist: tabulate
 
 # PyPlate
 
 [![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 [![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
```

### Comparing `pyplate_hte-0.4.2/README.md` & `pyplate_hte-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/pyplate/__init__.py` & `pyplate_hte-0.4.3/pyplate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/pyplate/experiment_design.py` & `pyplate_hte-0.4.3/pyplate/experiment_design.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/pyplate/pyplate.py` & `pyplate_hte-0.4.3/pyplate/pyplate.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/pyplate/pyplate.yaml` & `pyplate_hte-0.4.3/pyplate/pyplate.yaml`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/pyplate/slicer.py` & `pyplate_hte-0.4.3/pyplate/slicer.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/pyplate_hte.egg-info/PKG-INFO` & `pyplate_hte-0.4.3/pyplate_hte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -198,14 +198,15 @@
 Project-URL: Repository, https://github.com/ekwan/PyPlate
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyyaml
+Requires-Dist: tabulate
 
 # PyPlate
 
 [![PyPI](https://img.shields.io/pypi/v/pyplate-hte)](https://pypi.org/project/pyplate-hte)
 [![Documentation Status](https://readthedocs.org/projects/pyplate-hte/badge/?version=latest)](https://pyplate-hte.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyplate-hte)](https://pypi.org/project/pyplate-hte)
```

### Comparing `pyplate_hte-0.4.2/pyplate_hte.egg-info/SOURCES.txt` & `pyplate_hte-0.4.3/pyplate_hte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/pyproject.toml` & `pyplate_hte-0.4.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires      = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplate-hte"
-version = "0.4.2"
+version = "0.4.3"
 description = "A Python tool for designing chemistry experiments in plate format"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Eugene Kwan and James Marvin"},
     {email = "ekwan16@gmail.com"}
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
 ]
 dependencies = [
     "numpy",
     "pandas",
-    "pyyaml"
+    "pyyaml",
+    "tabulate",
 ]
 
 
 [tool.setuptools]
 packages = ["pyplate"]
 
 [project.urls]
```

### Comparing `pyplate_hte-0.4.2/tests/test_Container.py` & `pyplate_hte-0.4.3/tests/test_Container.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_Plate.py` & `pyplate_hte-0.4.3/tests/test_Plate.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_Recipe.py` & `pyplate_hte-0.4.3/tests/test_Recipe.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_Slicer.py` & `pyplate_hte-0.4.3/tests/test_Slicer.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_Substance.py` & `pyplate_hte-0.4.3/tests/test_Substance.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_convert.py` & `pyplate_hte-0.4.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_create_solution.py` & `pyplate_hte-0.4.3/tests/test_create_solution.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_dilute.py` & `pyplate_hte-0.4.3/tests/test_dilute.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_eugene.py` & `pyplate_hte-0.4.3/tests/test_eugene.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_get_substance_used2.py` & `pyplate_hte-0.4.3/tests/test_get_substance_used2.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_recipe_amount_remaining.py` & `pyplate_hte-0.4.3/tests/test_recipe_amount_remaining.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_recipe_get_container_flows.py` & `pyplate_hte-0.4.3/tests/test_recipe_get_container_flows.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_recipe_get_substance_used.py` & `pyplate_hte-0.4.3/tests/test_recipe_get_substance_used.py`

 * *Files identical despite different names*

### Comparing `pyplate_hte-0.4.2/tests/test_transfers.py` & `pyplate_hte-0.4.3/tests/test_transfers.py`

 * *Files identical despite different names*

