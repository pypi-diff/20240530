# Comparing `tmp/e1608-0.1.2.tar.gz` & `tmp/e1608-0.1.3.tar.gz`

## Comparing `e1608-0.1.2.tar` & `e1608-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 e1608-0.1.2/Mapper.py
--rw-r--r--   0        0        0    17071 2020-02-02 00:00:00.000000 e1608-0.1.2/MCCDAQ/E1608.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 e1608-0.1.2/MCCDAQ/__init__.py
--rw-r--r--   0        0        0  7899900 2020-02-02 00:00:00.000000 e1608-0.1.2/data_files/data_2024-04-23_13-14-06.csv
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 e1608-0.1.2/LICENSE
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 e1608-0.1.2/README.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 e1608-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 e1608-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 e1608-0.1.3/Mapper.py
+-rw-r--r--   0        0        0    17071 2020-02-02 00:00:00.000000 e1608-0.1.3/E1608/E1608.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 e1608-0.1.3/E1608/__init__.py
+-rw-r--r--   0        0        0  7899900 2020-02-02 00:00:00.000000 e1608-0.1.3/data_files/data_2024-04-23_13-14-06.csv
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 e1608-0.1.3/LICENSE
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 e1608-0.1.3/README.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 e1608-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 e1608-0.1.3/PKG-INFO
```

### Comparing `e1608-0.1.2/Mapper.py` & `e1608-0.1.3/Mapper.py`

 * *Files identical despite different names*

### Comparing `e1608-0.1.2/MCCDAQ/E1608.py` & `e1608-0.1.3/E1608/E1608.py`

 * *Files identical despite different names*

### Comparing `e1608-0.1.2/data_files/data_2024-04-23_13-14-06.csv` & `e1608-0.1.3/data_files/data_2024-04-23_13-14-06.csv`

 * *Files identical despite different names*

### Comparing `e1608-0.1.2/LICENSE` & `e1608-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `e1608-0.1.2/pyproject.toml` & `e1608-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "E1608"
-version = '0.1.2'
+version = '0.1.3'
 authors  = [{name="Maedeh Lavvaf", email="mdhlvf@gmail.com" }]
 description = "Python API for E1608 devices used by the TUCAN collaboration."
 readme = "README.md"
 classifiers = [
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
```

### Comparing `e1608-0.1.2/PKG-INFO` & `e1608-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: E1608
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python API for E1608 devices used by the TUCAN collaboration.
 Project-URL: Homepage, https://github.com/mlavvaf/MCCDAQ
 Project-URL: Bug Tracker, https://github.com/mlavvaf/MCCDAQ/issues
 Author-email: Maedeh Lavvaf <mdhlvf@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 mlavvaf
@@ -37,9 +37,9 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 # MCCDAQ data acquisition
 
-<img src="https://img.shields.io/pypi/v/DataAcquisition?style=flat-square"/> <img src="https://img.shields.io/pypi/format/MCCDAQ?style=flat-square"/> <img src="https://img.shields.io/github/languages/top/mlavvaf/MCCDAQ?style=flat-square"/>
-<img src="https://img.shields.io/github/languages/code-size/mlavvaf/MCCDAQ?style=flat-square"/> <img src="https://img.shields.io/pypi/l/MCCDAQ?style=flat-square"/> <img src="https://img.shields.io/github/last-commit/mlavvaf/MCCDAQ?style=flat-square"/>
+<img src="https://img.shields.io/pypi/v/E1608?style=flat-square"/> <img src="https://img.shields.io/pypi/format/E1608?style=flat-square"/> <img src="https://img.shields.io/github/languages/top/mlavvaf/MCCDAQ?style=flat-square"/>
+<img src="https://img.shields.io/github/languages/code-size/mlavvaf/MCCDAQ?style=flat-square"/> <img src="https://img.shields.io/pypi/l/E1608?style=flat-square"/> <img src="https://img.shields.io/github/last-commit/mlavvaf/MCCDAQ?style=flat-square"/>
```

