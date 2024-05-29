# Comparing `tmp/qualipy-1.1.0.tar.gz` & `tmp/qualipy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualipy-1.1.0.tar", last modified: Thu Apr 11 00:23:58 2024, max compression
+gzip compressed data, was "qualipy-1.1.1.tar", last modified: Wed May 29 23:12:58 2024, max compression
```

## Comparing `qualipy-1.1.0.tar` & `qualipy-1.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/
--rw-r--r--   0 kali      (1000) kali      (1000)     1070 2024-01-13 00:11:01.000000 qualipy-1.1.0/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     2867 2024-04-11 00:23:58.994543 qualipy-1.1.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      792 2024-04-10 04:14:30.000000 qualipy-1.1.0/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)     2209 2024-04-11 00:23:52.000000 qualipy-1.1.0/readme.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-04-11 00:23:58.994543 qualipy-1.1.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      344 2024-01-13 00:11:01.000000 qualipy-1.1.0/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.990543 qualipy-1.1.0/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.990543 qualipy-1.1.0/src/qualipy/
--rw-r--r--   0 kali      (1000) kali      (1000)       44 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3552 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/__main__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/authentication/
--rw-r--r--   0 kali      (1000) kali      (1000)       62 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/authentication/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      942 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/authentication/authenticator.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1809 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/authentication/keyring_authenticator.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/config/
--rw-r--r--   0 kali      (1000) kali      (1000)     2172 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/config/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5509 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/config/app_config.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/data_management/
--rw-r--r--   0 kali      (1000) kali      (1000)      159 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5444 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/csv_data_loader.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1506 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/data_loader.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6811 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/data_manager.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3026 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/excel_data_loader.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1980 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/json_data_loader.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2604 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/xml_data_loader.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1812 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/yaml_data_loader.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/exceptions/
--rw-r--r--   0 kali      (1000) kali      (1000)     1537 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/exceptions/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/
--rw-r--r--   0 kali      (1000) kali      (1000)       86 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)    12900 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1874 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/proj_mgmt_plugin.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/test_plugins/
--rw-r--r--   0 kali      (1000) kali      (1000)      121 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/test_plugins/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      752 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/test_plugins/behave_plugin.py
--rw-r--r--   0 kali      (1000) kali      (1000)      783 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/test_plugins/test_plugin.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2867 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1148 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       31 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/top_level.txt
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/tests/
--rw-r--r--   0 kali      (1000) kali      (1000)      121 2024-04-10 03:56:13.000000 qualipy-1.1.0/tests/test_main.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.309896 qualipy-1.1.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1070 2024-01-13 00:11:01.000000 qualipy-1.1.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     2910 2024-05-29 23:12:58.309896 qualipy-1.1.1/PKG-INFO
+-rw-rw-r--   0 kali      (1000) kali      (1000)      872 2024-05-29 23:02:57.000000 qualipy-1.1.1/pyproject.toml
+-rw-rw-r--   0 kali      (1000) kali      (1000)     2164 2024-05-29 23:12:55.000000 qualipy-1.1.1/readme.md
+-rw-rw-r--   0 kali      (1000) kali      (1000)       38 2024-05-29 23:12:58.309896 qualipy-1.1.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      344 2024-01-13 00:11:01.000000 qualipy-1.1.1/setup.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.301896 qualipy-1.1.1/src/
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.305896 qualipy-1.1.1/src/qualipy/
+-rw-r--r--   0 kali      (1000) kali      (1000)       44 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3552 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/__main__.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.305896 qualipy-1.1.1/src/qualipy/authentication/
+-rw-r--r--   0 kali      (1000) kali      (1000)       62 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/authentication/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      942 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/authentication/authenticator.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1809 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/authentication/keyring_authenticator.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.305896 qualipy-1.1.1/src/qualipy/config/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2172 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/config/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5509 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/config/app_config.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.309896 qualipy-1.1.1/src/qualipy/data_management/
+-rw-r--r--   0 kali      (1000) kali      (1000)      159 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5444 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/csv_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1506 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6811 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/data_manager.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3026 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/excel_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1980 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/json_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2604 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/xml_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1812 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/data_management/yaml_data_loader.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.309896 qualipy-1.1.1/src/qualipy/exceptions/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1537 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/exceptions/__init__.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.309896 qualipy-1.1.1/src/qualipy/proj_mgmt_plugins/
+-rw-r--r--   0 kali      (1000) kali      (1000)       86 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/proj_mgmt_plugins/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    12900 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1874 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/proj_mgmt_plugins/proj_mgmt_plugin.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.309896 qualipy-1.1.1/src/qualipy/test_plugins/
+-rw-r--r--   0 kali      (1000) kali      (1000)      121 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/test_plugins/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      752 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/test_plugins/behave_plugin.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      783 2024-04-10 03:56:13.000000 qualipy-1.1.1/src/qualipy/test_plugins/test_plugin.py
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.309896 qualipy-1.1.1/src/qualipy.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2910 2024-05-29 23:12:58.000000 qualipy-1.1.1/src/qualipy.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1148 2024-05-29 23:12:58.000000 qualipy-1.1.1/src/qualipy.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-29 23:12:58.000000 qualipy-1.1.1/src/qualipy.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       31 2024-05-29 23:12:58.000000 qualipy-1.1.1/src/qualipy.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2024-05-29 23:12:58.000000 qualipy-1.1.1/src/qualipy.egg-info/top_level.txt
+drwxrwxr-x   0 kali      (1000) kali      (1000)        0 2024-05-29 23:12:58.309896 qualipy-1.1.1/tests/
+-rw-r--r--   0 kali      (1000) kali      (1000)      121 2024-04-10 03:56:13.000000 qualipy-1.1.1/tests/test_main.py
```

### Comparing `qualipy-1.1.0/LICENSE` & `qualipy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/PKG-INFO` & `qualipy-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: qualipy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automated test process framework
 Author-email: Charles Morris <cmorris616@gmail.com>
 Project-URL: Homepage, https://github.com/cmorris616/qualipy
 Project-URL: Bug Tracker, https://github.com/cmorris616/qualipy/issues
+Project-URL: Documentation, https://cmorris-qualipy.readthedocs.io/en/latest/index.html
 Keywords: test,testing,project management,jira,framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,15 +22,14 @@
 QualiPy is a framework for assisting with the automated testing process.  Qualipy is not meant to replace pytest, behave, or other testing frameworks.  Instead, it is meant to augment the process to provider further automation.  It can be configured based on the needs of the project and the availablility of other technologies.
 
 QualiPy features include:
 - Exporting feature files from JIRA for progression and regression testing
 - Uploading test results to JIRA
 - Support for custom project management, authentication, and testing plugins
 - Moving user stories based on the outcome of the tests
-- Moving user stories based on test results]
 - Loading test data to be used during the testing process
 - Data management across steps and scenarios
 
 ## Test Plugins
 QualiPy is built to use multiple testing frameworks via plugins.  Currently, QualiPy supports the behave framework out of the box for business-driven development.
 
 ## Project Management Plugins
```

### Comparing `qualipy-1.1.0/pyproject.toml` & `qualipy-1.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qualipy"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Charles Morris", email="cmorris616@gmail.com" },
 ]
 description = "Automated test process framework"
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,10 +23,11 @@
   "requests",
   "PyYAML"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/cmorris616/qualipy"
 "Bug Tracker" = "https://github.com/cmorris616/qualipy/issues"
+"Documentation" = "https://cmorris-qualipy.readthedocs.io/en/latest/index.html"
 
 # [tool.setuptools.packages.find]
 # exclude = ["docs*", "tests*"]
```

### Comparing `qualipy-1.1.0/readme.md` & `qualipy-1.1.1/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 QualiPy is a framework for assisting with the automated testing process.  Qualipy is not meant to replace pytest, behave, or other testing frameworks.  Instead, it is meant to augment the process to provider further automation.  It can be configured based on the needs of the project and the availablility of other technologies.
 
 QualiPy features include:
 - Exporting feature files from JIRA for progression and regression testing
 - Uploading test results to JIRA
 - Support for custom project management, authentication, and testing plugins
 - Moving user stories based on the outcome of the tests
-- Moving user stories based on test results]
 - Loading test data to be used during the testing process
 - Data management across steps and scenarios
 
 ## Test Plugins
 QualiPy is built to use multiple testing frameworks via plugins.  Currently, QualiPy supports the behave framework out of the box for business-driven development.
 
 ## Project Management Plugins
```

### Comparing `qualipy-1.1.0/src/qualipy/__main__.py` & `qualipy-1.1.1/src/qualipy/__main__.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/authentication/authenticator.py` & `qualipy-1.1.1/src/qualipy/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/authentication/keyring_authenticator.py` & `qualipy-1.1.1/src/qualipy/authentication/keyring_authenticator.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/config/__init__.py` & `qualipy-1.1.1/src/qualipy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/config/app_config.py` & `qualipy-1.1.1/src/qualipy/config/app_config.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/data_management/csv_data_loader.py` & `qualipy-1.1.1/src/qualipy/data_management/csv_data_loader.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/data_management/data_loader.py` & `qualipy-1.1.1/src/qualipy/data_management/data_loader.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/data_management/data_manager.py` & `qualipy-1.1.1/src/qualipy/data_management/data_manager.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/data_management/excel_data_loader.py` & `qualipy-1.1.1/src/qualipy/data_management/excel_data_loader.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/data_management/json_data_loader.py` & `qualipy-1.1.1/src/qualipy/data_management/json_data_loader.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/data_management/xml_data_loader.py` & `qualipy-1.1.1/src/qualipy/data_management/xml_data_loader.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/data_management/yaml_data_loader.py` & `qualipy-1.1.1/src/qualipy/data_management/yaml_data_loader.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/exceptions/__init__.py` & `qualipy-1.1.1/src/qualipy/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py` & `qualipy-1.1.1/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/proj_mgmt_plugin.py` & `qualipy-1.1.1/src/qualipy/proj_mgmt_plugins/proj_mgmt_plugin.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/test_plugins/behave_plugin.py` & `qualipy-1.1.1/src/qualipy/test_plugins/behave_plugin.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy/test_plugins/test_plugin.py` & `qualipy-1.1.1/src/qualipy/test_plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `qualipy-1.1.0/src/qualipy.egg-info/PKG-INFO` & `qualipy-1.1.1/src/qualipy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: qualipy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Automated test process framework
 Author-email: Charles Morris <cmorris616@gmail.com>
 Project-URL: Homepage, https://github.com/cmorris616/qualipy
 Project-URL: Bug Tracker, https://github.com/cmorris616/qualipy/issues
+Project-URL: Documentation, https://cmorris-qualipy.readthedocs.io/en/latest/index.html
 Keywords: test,testing,project management,jira,framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -21,15 +22,14 @@
 QualiPy is a framework for assisting with the automated testing process.  Qualipy is not meant to replace pytest, behave, or other testing frameworks.  Instead, it is meant to augment the process to provider further automation.  It can be configured based on the needs of the project and the availablility of other technologies.
 
 QualiPy features include:
 - Exporting feature files from JIRA for progression and regression testing
 - Uploading test results to JIRA
 - Support for custom project management, authentication, and testing plugins
 - Moving user stories based on the outcome of the tests
-- Moving user stories based on test results]
 - Loading test data to be used during the testing process
 - Data management across steps and scenarios
 
 ## Test Plugins
 QualiPy is built to use multiple testing frameworks via plugins.  Currently, QualiPy supports the behave framework out of the box for business-driven development.
 
 ## Project Management Plugins
```

### Comparing `qualipy-1.1.0/src/qualipy.egg-info/SOURCES.txt` & `qualipy-1.1.1/src/qualipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

