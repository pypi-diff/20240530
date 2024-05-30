# Comparing `tmp/autogluon-1.1.1b20240528.tar.gz` & `tmp/autogluon-1.1.1b20240529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.1.1b20240528.tar", last modified: Tue May 28 09:05:22 2024, max compression
+gzip compressed data, was "autogluon-1.1.1b20240529.tar", last modified: Wed May 29 09:05:43 2024, max compression
```

## Comparing `autogluon-1.1.1b20240528.tar` & `autogluon-1.1.1b20240529.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:05:22.190702 autogluon-1.1.1b20240528/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-28 09:05:22.190702 autogluon-1.1.1b20240528/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:05:22.190702 autogluon-1.1.1b20240528/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-28 09:03:40.000000 autogluon-1.1.1b20240528/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:05:22.190702 autogluon-1.1.1b20240528/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:05:22.190702 autogluon-1.1.1b20240528/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:05:22.190702 autogluon-1.1.1b20240528/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:03:40.000000 autogluon-1.1.1b20240528/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:05:22.190702 autogluon-1.1.1b20240528/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-28 09:05:22.000000 autogluon-1.1.1b20240528/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 09:05:22.000000 autogluon-1.1.1b20240528/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:05:22.000000 autogluon-1.1.1b20240528/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 09:05:22.000000 autogluon-1.1.1b20240528/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 09:05:22.000000 autogluon-1.1.1b20240528/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 09:05:22.000000 autogluon-1.1.1b20240528/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:05:22.000000 autogluon-1.1.1b20240528/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:05:43.741838 autogluon-1.1.1b20240529/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-29 09:05:43.741838 autogluon-1.1.1b20240529/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:05:43.741838 autogluon-1.1.1b20240529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 09:04:01.000000 autogluon-1.1.1b20240529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:05:43.737837 autogluon-1.1.1b20240529/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:05:43.737837 autogluon-1.1.1b20240529/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:05:43.737837 autogluon-1.1.1b20240529/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:04:01.000000 autogluon-1.1.1b20240529/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:05:43.737837 autogluon-1.1.1b20240529/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-29 09:05:43.000000 autogluon-1.1.1b20240529/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-29 09:05:43.000000 autogluon-1.1.1b20240529/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:05:43.000000 autogluon-1.1.1b20240529/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 09:05:43.000000 autogluon-1.1.1b20240529/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 09:05:43.000000 autogluon-1.1.1b20240529/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 09:05:43.000000 autogluon-1.1.1b20240529/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:05:43.000000 autogluon-1.1.1b20240529/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.1.1b20240528/PKG-INFO` & `autogluon-1.1.1b20240529/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240528
+Version: 1.1.1b20240529
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.1.1b20240528/setup.py` & `autogluon-1.1.1b20240529/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.1.1b20240528/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.1.1b20240529/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.1.1b20240528
+Version: 1.1.1b20240529
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

