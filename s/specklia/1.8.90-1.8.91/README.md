# Comparing `tmp/specklia-1.8.90.tar.gz` & `tmp/specklia-1.8.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.8.90.tar", last modified: Thu May 30 01:33:02 2024, max compression
+gzip compressed data, was "specklia-1.8.91.tar", last modified: Thu May 30 02:55:54 2024, max compression
```

## Comparing `specklia-1.8.90.tar` & `specklia-1.8.91.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:33:02.302788 specklia-1.8.90/
--rw-r--r--   0 root         (0) root         (0)     1061 2024-05-30 01:17:54.000000 specklia-1.8.90/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-30 01:33:02.302788 specklia-1.8.90/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1611 2024-05-30 01:17:54.000000 specklia-1.8.90/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2024-05-30 01:33:02.302788 specklia-1.8.90/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2366 2024-05-30 01:17:54.000000 specklia-1.8.90/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:33:02.302788 specklia-1.8.90/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-30 01:17:54.000000 specklia-1.8.90/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14714 2024-05-30 01:17:54.000000 specklia-1.8.90/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    40528 2024-05-30 01:17:54.000000 specklia-1.8.90/specklia/client.py
--rw-r--r--   0 root         (0) root         (0)     4074 2024-05-30 01:17:54.000000 specklia-1.8.90/specklia/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:33:02.302788 specklia-1.8.90/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-30 01:33:02.000000 specklia-1.8.90/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-30 01:33:02.000000 specklia-1.8.90/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 01:33:02.000000 specklia-1.8.90/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-30 01:33:02.000000 specklia-1.8.90/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 01:33:02.000000 specklia-1.8.90/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 01:33:02.302788 specklia-1.8.90/tests/
--rw-r--r--   0 root         (0) root         (0)    14689 2024-05-30 01:17:54.000000 specklia-1.8.90/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     2654 2024-05-30 01:17:54.000000 specklia-1.8.90/tests/test_utilities.py
--rw-r--r--   0 root         (0) root         (0)    11623 2024-05-30 01:17:54.000000 specklia-1.8.90/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:55:54.946552 specklia-1.8.91/
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-30 02:55:52.000000 specklia-1.8.91/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-30 02:55:54.946552 specklia-1.8.91/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-05-30 02:55:52.000000 specklia-1.8.91/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2024-05-30 02:55:54.946552 specklia-1.8.91/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-05-30 02:55:52.000000 specklia-1.8.91/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:55:54.946552 specklia-1.8.91/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-30 02:55:52.000000 specklia-1.8.91/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14714 2024-05-30 02:55:52.000000 specklia-1.8.91/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    40528 2024-05-30 02:55:52.000000 specklia-1.8.91/specklia/client.py
+-rw-r--r--   0 root         (0) root         (0)     4074 2024-05-30 02:55:52.000000 specklia-1.8.91/specklia/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:55:54.946552 specklia-1.8.91/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-30 02:55:54.000000 specklia-1.8.91/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-30 02:55:54.000000 specklia-1.8.91/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 02:55:54.000000 specklia-1.8.91/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-30 02:55:54.000000 specklia-1.8.91/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 02:55:54.000000 specklia-1.8.91/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 02:55:54.946552 specklia-1.8.91/tests/
+-rw-r--r--   0 root         (0) root         (0)    14689 2024-05-30 02:55:52.000000 specklia-1.8.91/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2024-05-30 02:55:52.000000 specklia-1.8.91/tests/test_utilities.py
+-rw-r--r--   0 root         (0) root         (0)    11623 2024-05-30 02:55:52.000000 specklia-1.8.91/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.8.90/LICENCE` & `specklia-1.8.91/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/PKG-INFO` & `specklia-1.8.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.8.90
+Version: 1.8.91
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/
 Project-URL: Changelog, https://specklia.earthwave.co.uk/generated_docs/change_log.html
```

### Comparing `specklia-1.8.90/README.md` & `specklia-1.8.91/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/setup.py` & `specklia-1.8.91/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/specklia/_websocket_helpers.py` & `specklia-1.8.91/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/specklia/client.py` & `specklia-1.8.91/specklia/client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/specklia/utilities.py` & `specklia-1.8.91/specklia/utilities.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/specklia.egg-info/PKG-INFO` & `specklia-1.8.91/specklia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.8.90
+Version: 1.8.91
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/
 Project-URL: Changelog, https://specklia.earthwave.co.uk/generated_docs/change_log.html
```

### Comparing `specklia-1.8.90/tests/test_client.py` & `specklia-1.8.91/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/tests/test_utilities.py` & `specklia-1.8.91/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `specklia-1.8.90/tests/test_websocket_helpers.py` & `specklia-1.8.91/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

