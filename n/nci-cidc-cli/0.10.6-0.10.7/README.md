# Comparing `tmp/nci_cidc_cli-0.10.6.tar.gz` & `tmp/nci_cidc_cli-0.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-d4ce5x3g/nci_cidc_cli-0.10.6.tar", last modified: Fri Jul 21 00:47:56 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-asjb759c/nci_cidc_cli-0.10.7.tar", last modified: Thu May 30 13:20:35 2024, max compression
```

## Comparing `nci_cidc_cli-0.10.6.tar` & `nci_cidc_cli-0.10.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/consent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/nci_cidc_cli/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:56.000000 nci_cidc_cli-0.10.6/tests/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/dbedit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/dbedit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/dbedit/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/dbedit/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 00:47:43.000000 nci_cidc_cli-0.10.6/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/consent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34527 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/nci_cidc_cli/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:35.000000 nci_cidc_cli-0.10.7/tests/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/dbedit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/dbedit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18466 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/dbedit/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57256 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/dbedit/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13366 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-30 13:20:27.000000 nci_cidc_cli-0.10.7/tests/util.py
```

### Comparing `nci_cidc_cli-0.10.6/LICENSE` & `nci_cidc_cli-0.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/PKG-INFO` & `nci_cidc_cli-0.10.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_cli
-Version: 0.10.6
+Version: 0.10.7
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.6/README.md` & `nci_cidc_cli-0.10.7/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/api.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/auth.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/cache.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/cli.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/config.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/config.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/consent.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/consent.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/cli.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/core.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/list.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/dbedit/remove.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/dbedit/remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/gcloud.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/gcloud.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli/upload.py` & `nci_cidc_cli-0.10.7/nci_cidc_cli/upload.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/PKG-INFO` & `nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-cli
-Version: 0.10.6
+Version: 0.10.7
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.6/nci_cidc_cli.egg-info/SOURCES.txt` & `nci_cidc_cli-0.10.7/nci_cidc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/setup.py` & `nci_cidc_cli-0.10.7/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/dbedit/constants.py` & `nci_cidc_cli-0.10.7/tests/dbedit/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/dbedit/test_core.py` & `nci_cidc_cli-0.10.7/tests/dbedit/test_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/dbedit/test_list.py` & `nci_cidc_cli-0.10.7/tests/dbedit/test_list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/dbedit/test_remove.py` & `nci_cidc_cli-0.10.7/tests/dbedit/test_remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/test_api.py` & `nci_cidc_cli-0.10.7/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/test_auth.py` & `nci_cidc_cli-0.10.7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/test_cache.py` & `nci_cidc_cli-0.10.7/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/test_cli.py` & `nci_cidc_cli-0.10.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/test_upload.py` & `nci_cidc_cli-0.10.7/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.6/tests/util.py` & `nci_cidc_cli-0.10.7/tests/util.py`

 * *Files identical despite different names*

