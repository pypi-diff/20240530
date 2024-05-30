# Comparing `tmp/lsst_felis-27.2024.2100.tar.gz` & `tmp/lsst_felis-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_felis-27.2024.2100.tar", last modified: Thu May 23 10:08:06 2024, max compression
+gzip compressed data, was "lsst_felis-27.2024.2200.tar", last modified: Thu May 30 09:55:46 2024, max compression
```

## Comparing `lsst_felis-27.2024.2100.tar` & `lsst_felis-27.2024.2200.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:06.269515 lsst_felis-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-23 10:08:06.269515 lsst_felis-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:06.261515 lsst_felis-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:06.265515 lsst_felis-27.2024.2100/python/felis/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    21351 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:06.265515 lsst_felis-27.2024.2100/python/felis/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/db/_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/db/sqltypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/python/felis/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:08:06.000000 lsst_felis-27.2024.2100/python/felis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:06.269515 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-23 10:08:06.000000 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-23 10:08:06.000000 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:08:06.000000 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 10:08:06.000000 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 10:08:06.000000 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 10:08:06.000000 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:08:05.000000 lsst_felis-27.2024.2100/python/lsst_felis.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 10:08:06.269515 lsst_felis-27.2024.2100/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:06.269515 lsst_felis-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    22986 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/tests/test_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/tests/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/tests/test_tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-23 10:07:59.000000 lsst_felis-27.2024.2100/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:46.556455 lsst_felis-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-30 09:55:46.556455 lsst_felis-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:46.548455 lsst_felis-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:46.552455 lsst_felis-27.2024.2200/python/felis/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21351 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:46.552455 lsst_felis-27.2024.2200/python/felis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/db/_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/db/sqltypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/python/felis/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/felis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:46.556455 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:55:46.000000 lsst_felis-27.2024.2200/python/lsst_felis.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 09:55:46.556455 lsst_felis-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:55:46.556455 lsst_felis-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22986 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/tests/test_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/tests/test_tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-30 09:55:40.000000 lsst_felis-27.2024.2200/tests/test_validation.py
```

### Comparing `lsst_felis-27.2024.2100/LICENSE` & `lsst_felis-27.2024.2200/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/PKG-INFO` & `lsst_felis-27.2024.2200/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://felis.lsst.io
 Project-URL: Source, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lsst_felis-27.2024.2100/README.rst` & `lsst_felis-27.2024.2200/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/pyproject.toml` & `lsst_felis-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/__init__.py` & `lsst_felis-27.2024.2200/python/felis/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/cli.py` & `lsst_felis-27.2024.2200/python/felis/cli.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/datamodel.py` & `lsst_felis-27.2024.2200/python/felis/datamodel.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/db/_variants.py` & `lsst_felis-27.2024.2200/python/felis/db/_variants.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/db/sqltypes.py` & `lsst_felis-27.2024.2200/python/felis/db/sqltypes.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/metadata.py` & `lsst_felis-27.2024.2200/python/felis/metadata.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/tap.py` & `lsst_felis-27.2024.2200/python/felis/tap.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/types.py` & `lsst_felis-27.2024.2200/python/felis/types.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/felis/validation.py` & `lsst_felis-27.2024.2200/python/felis/validation.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/python/lsst_felis.egg-info/PKG-INFO` & `lsst_felis-27.2024.2200/python/lsst_felis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://felis.lsst.io
 Project-URL: Source, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lsst_felis-27.2024.2100/python/lsst_felis.egg-info/SOURCES.txt` & `lsst_felis-27.2024.2200/python/lsst_felis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/tests/test_cli.py` & `lsst_felis-27.2024.2200/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/tests/test_datamodel.py` & `lsst_felis-27.2024.2200/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/tests/test_datatypes.py` & `lsst_felis-27.2024.2200/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/tests/test_metadata.py` & `lsst_felis-27.2024.2200/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/tests/test_tap.py` & `lsst_felis-27.2024.2200/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.2100/tests/test_validation.py` & `lsst_felis-27.2024.2200/tests/test_validation.py`

 * *Files identical despite different names*

