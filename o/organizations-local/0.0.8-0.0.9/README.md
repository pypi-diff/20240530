# Comparing `tmp/organizations-local-0.0.8.tar.gz` & `tmp/organizations-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organizations-local-0.0.8.tar", last modified: Tue Feb 27 18:43:51 2024, max compression
+gzip compressed data, was "organizations-local-0.0.9.tar", last modified: Fri Mar  1 08:06:18 2024, max compression
```

## Comparing `organizations-local-0.0.8.tar` & `organizations-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:43:51.822103 organizations-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-27 18:43:51.822103 organizations-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-27 18:43:02.000000 organizations-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:43:51.818103 organizations-local-0.0.8/organizations_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:43:51.818103 organizations-local-0.0.8/organizations_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 18:43:02.000000 organizations-local-0.0.8/organizations_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-27 18:43:02.000000 organizations-local-0.0.8/organizations_local/src/organizations_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-02-27 18:43:02.000000 organizations-local-0.0.8/organizations_local/src/organizations_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 18:43:51.822103 organizations-local-0.0.8/organizations_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-27 18:43:51.000000 organizations-local-0.0.8/organizations_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-27 18:43:51.000000 organizations-local-0.0.8/organizations_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 18:43:51.000000 organizations-local-0.0.8/organizations_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-27 18:43:51.000000 organizations-local-0.0.8/organizations_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-27 18:43:51.000000 organizations-local-0.0.8/organizations_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-27 18:43:02.000000 organizations-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 18:43:51.822103 organizations-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-27 18:43:02.000000 organizations-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 08:06:18.225581 organizations-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-01 08:06:18.225581 organizations-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-01 08:05:50.000000 organizations-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 08:06:18.221580 organizations-local-0.0.9/organizations_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 08:06:18.225581 organizations-local-0.0.9/organizations_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 08:05:50.000000 organizations-local-0.0.9/organizations_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-01 08:05:50.000000 organizations-local-0.0.9/organizations_local/src/organizations_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-03-01 08:05:50.000000 organizations-local-0.0.9/organizations_local/src/organizations_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 08:06:18.225581 organizations-local-0.0.9/organizations_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-01 08:06:18.000000 organizations-local-0.0.9/organizations_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-01 08:06:18.000000 organizations-local-0.0.9/organizations_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 08:06:18.000000 organizations-local-0.0.9/organizations_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-01 08:06:18.000000 organizations-local-0.0.9/organizations_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-01 08:06:18.000000 organizations-local-0.0.9/organizations_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-01 08:05:50.000000 organizations-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 08:06:18.225581 organizations-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-01 08:05:50.000000 organizations-local-0.0.9/setup.py
```

### Comparing `organizations-local-0.0.8/PKG-INFO` & `organizations-local-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organizations-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles organizations-local Python
 Home-page: https://github.com/circles-zone/organization-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organizations-local-0.0.8/organizations_local/src/organizations_constants.py` & `organizations-local-0.0.9/organizations_local/src/organizations_constants.py`

 * *Files identical despite different names*

### Comparing `organizations-local-0.0.8/organizations_local.egg-info/PKG-INFO` & `organizations-local-0.0.9/organizations_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organizations-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles organizations-local Python
 Home-page: https://github.com/circles-zone/organization-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `organizations-local-0.0.8/setup.py` & `organizations-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "organizations-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/organizations-local/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/organizations-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles organizations-local Python",
     long_description="PyPI Package for Circles organizations-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/organization-local-python-package",
     packages=[package_dir],
```

