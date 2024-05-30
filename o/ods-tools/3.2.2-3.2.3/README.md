# Comparing `tmp/ods_tools-3.2.2.tar.gz` & `tmp/ods_tools-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ods_tools-3.2.2.tar", last modified: Wed Mar 27 11:04:31 2024, max compression
+gzip compressed data, was "ods_tools-3.2.3.tar", last modified: Mon Apr 29 10:57:48 2024, max compression
```

## Comparing `ods_tools-3.2.2.tar` & `ods_tools-3.2.3.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.587478 ods_tools-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-03-27 11:04:31.587478 ods_tools-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-03-27 11:04:13.000000 ods_tools-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.579478 ods_tools-3.2.2/ods_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.583478 ods_tools-3.2.2/ods_tools/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.583478 ods_tools-3.2.2/ods_tools/odtf/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.583478 ods_tools-3.2.2/ods_tools/odtf/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/connector/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.583478 ods_tools-3.2.2/ods_tools/odtf/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.583478 ods_tools-3.2.2/ods_tools/odtf/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/files/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/files/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.583478 ods_tools-3.2.2/ods_tools/odtf/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/mapping/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/mapping/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17980 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/mapping/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/notset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.587478 ods_tools-3.2.2/ods_tools/odtf/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/runner/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.587478 ods_tools-3.2.2/ods_tools/odtf/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/transformers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/transformers/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)    19470 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/transformers/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/validator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/odtf/validator_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.587478 ods_tools-3.2.2/ods_tools/oed/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/forex.py
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/oed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/setting_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    23012 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/source.py
--rw-r--r--   0 runner    (1001) docker     (127)    17182 2024-03-27 11:04:13.000000 ods_tools-3.2.2/ods_tools/oed/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 11:04:31.583478 ods_tools-3.2.2/ods_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-03-27 11:04:31.000000 ods_tools-3.2.2/ods_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-27 11:04:31.000000 ods_tools-3.2.2/ods_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 11:04:31.000000 ods_tools-3.2.2/ods_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-27 11:04:31.000000 ods_tools-3.2.2/ods_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-27 11:04:31.000000 ods_tools-3.2.2/ods_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 11:04:31.000000 ods_tools-3.2.2/ods_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 11:04:31.587478 ods_tools-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-27 11:04:13.000000 ods_tools-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.179804 ods_tools-3.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-29 10:57:48.179804 ods_tools-3.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-29 10:57:34.000000 ods_tools-3.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.171804 ods_tools-3.2.3/ods_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.175804 ods_tools-3.2.3/ods_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.175804 ods_tools-3.2.3/ods_tools/odtf/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.175804 ods_tools-3.2.3/ods_tools/odtf/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/connector/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.175804 ods_tools-3.2.3/ods_tools/odtf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.175804 ods_tools-3.2.3/ods_tools/odtf/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/files/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/files/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.175804 ods_tools-3.2.3/ods_tools/odtf/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9263 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/mapping/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/mapping/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17980 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/mapping/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/notset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.175804 ods_tools-3.2.3/ods_tools/odtf/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/runner/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.179804 ods_tools-3.2.3/ods_tools/odtf/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/transformers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/transformers/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/transformers/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/transformers/transform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/validator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/odtf/validator_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.179804 ods_tools-3.2.3/ods_tools/oed/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/forex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/oed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/setting_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23012 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17182 2024-04-29 10:57:34.000000 ods_tools-3.2.3/ods_tools/oed/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:57:48.171804 ods_tools-3.2.3/ods_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-29 10:57:48.000000 ods_tools-3.2.3/ods_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-29 10:57:48.000000 ods_tools-3.2.3/ods_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:57:48.000000 ods_tools-3.2.3/ods_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 10:57:48.000000 ods_tools-3.2.3/ods_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-29 10:57:48.000000 ods_tools-3.2.3/ods_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 10:57:48.000000 ods_tools-3.2.3/ods_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:57:48.179804 ods_tools-3.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-29 10:57:34.000000 ods_tools-3.2.3/setup.py
```

### Comparing `ods_tools-3.2.2/PKG-INFO` & `ods_tools-3.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods_tools
-Version: 3.2.2
+Version: 3.2.3
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.2.2/README.md` & `ods_tools-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/main.py` & `ods_tools-3.2.3/ods_tools/main.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/config.py` & `ods_tools-3.2.3/ods_tools/odtf/config.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/connector/base.py` & `ods_tools-3.2.3/ods_tools/odtf/connector/base.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/connector/csv.py` & `ods_tools-3.2.3/ods_tools/odtf/connector/csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,28 +66,31 @@
             "minimal": csv.QUOTE_MINIMAL,
             "none": csv.QUOTE_NONE,
             "nonnumeric": csv.QUOTE_NONNUMERIC,
         }.get(options.get("quoting", "nonnumeric"))
 
     def _data_serializer(self, row):
         return {
-            k: v if v is not None and not isinstance(v, NotSetType) else ""
+            k: f'"{v}"'.strip() if isinstance(v, str) and any(d in v for d in [',', ';', '\t', '\n', '"']) else (
+                v if v is not None and not isinstance(v, NotSetType) else "")
             for k, v in row.items()
         }
 
     def load(self, data: Iterable[Dict[str, Any]]):
         try:
             data = iter(data)
             first_row = next(data)
         except StopIteration:
             return
 
         with open(self.file_path, "w", newline="") as f:
             writer = csv.DictWriter(
-                f, fieldnames=list(first_row.keys()), quoting=self.quoting
+                f,
+                fieldnames=list(first_row.keys()),
+                quoting=self.quoting
             )
 
             if self.write_header:
                 writer.writeheader()
 
             writer.writerow(self._data_serializer(first_row))
             writer.writerows(map(self._data_serializer, data))
```

### Comparing `ods_tools-3.2.2/ods_tools/odtf/controller.py` & `ods_tools-3.2.3/ods_tools/odtf/controller.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/data/__init__.py` & `ods_tools-3.2.3/ods_tools/odtf/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/files/csv.py` & `ods_tools-3.2.3/ods_tools/odtf/files/csv.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/files/yaml.py` & `ods_tools-3.2.3/ods_tools/odtf/files/yaml.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/log.py` & `ods_tools-3.2.3/ods_tools/odtf/log.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/mapping/base.py` & `ods_tools-3.2.3/ods_tools/odtf/mapping/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Optional,
     Reversible,
     Set,
     Union,
 )
 
 import networkx as nx
-from lark import Tree
+from lark import Tree, Token
 
 from ..config import TransformationConfig
 from .errors import NoConversionPathError
 from ..transformers.transform import parse
 
 
 logger = logging.getLogger(__name__)
@@ -230,27 +230,69 @@
         return list(
             map(
                 lambda in_out: self.mapping_graph[in_out[0]][in_out[1]],
                 zip(self.path[:-1], self.path[1:]),
             )
         )
 
-    def get_transformations(self) -> List[DirectionalMapping]:
+    @staticmethod
+    def has_missing_columns(node: Union[Tree, Token, int, None], missing_columns: List[str]) -> bool:
+        """
+        Recursively checks if a node in the transformation tree contains any missing columns.
+
+        Args:
+            node (Union[Tree, Token, int, None]): The node to check for missing columns.
+            missing_columns (List[str]): A list of missing column names.
+
+        Returns:
+            bool: True if the node contains any missing columns, False otherwise.
+        """
+        if node is None or isinstance(node, int):
+            return False
+        if isinstance(node, Token):
+            return node.type == 'IDENT' and node.value in missing_columns
+        if node.data == 'lookup' and BaseMapping.has_missing_columns(node.children[0], missing_columns):
+            return True
+        return any(BaseMapping.has_missing_columns(child, missing_columns) for child in node.children)
+
+    def get_transformations(self, available_columns: List[str]) -> List[DirectionalMapping]:
         """
         Gets a column transformations and full transformation set for the
-        provided input and output paths.
+        provided input and output paths, filtered based on the available columns.
 
-        :return: The mappings along the conversion path.
+        :param available_columns: List of available columns in the input data
+        :return: The filtered mappings along the conversion path.
         """
         path = self.path
         logger.info(
             f"Path found {' -> '.join(f'{n.name} v{n.version}' for n in path)}"
         )
-        # parse the trees of the path so that is doesnt need
-        # to be done for every row
         transformations = [edge["transform"] for edge in self.path_edges]
+
+        missing_columns = list(set(transformations[0].types.keys()) - set(available_columns))
+
+        doable_transformations = []
         for mapping in transformations:
-            for transform in mapping.transformation_set.values():
-                for case in transform:
-                    case.parse()
+            doable_transformation_set = {}
+            for col, transform_list in mapping.transformation_set.items():
+                valid_transforms = []
+                for transform in transform_list:
+                    transform.parse()
+                    if ((transform.transformation_tree is None or
+                        not self.has_missing_columns(transform.transformation_tree, missing_columns)) and
+                        (transform.when_tree is None or
+                         not self.has_missing_columns(transform.when_tree, missing_columns))):
+                        valid_transforms.append(transform)
+                if valid_transforms:
+                    doable_transformation_set[col] = valid_transforms
+            if doable_transformation_set:
+                doable_transformations.append(
+                    DirectionalMapping(
+                        input_format=mapping.input_format,
+                        output_format=mapping.output_format,
+                        transformation_set=doable_transformation_set,
+                        types=mapping.types,
+                        null_values=mapping.null_values,
+                    )
+                )
 
-        return transformations
+        return doable_transformations
```

### Comparing `ods_tools-3.2.2/ods_tools/odtf/mapping/errors.py` & `ods_tools-3.2.3/ods_tools/odtf/mapping/errors.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/mapping/file.py` & `ods_tools-3.2.3/ods_tools/odtf/mapping/file.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/runner/base.py` & `ods_tools-3.2.3/ods_tools/odtf/runner/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     AsyncIterable,
     Callable,
     Dict,
     Iterable,
     List,
     TypedDict,
     Union,
-    Set
 )
 
 from ..config import TransformationConfig
 from ..connector.base import BaseConnector
 from ..mapping.base import (
     BaseMapping,
     ColumnConversions,
@@ -167,44 +166,39 @@
         else:
             return NotSet
 
     def apply_column_transformation(
         self,
         row: RowType,
         entry_list: List[TransformationEntry],
-        missing_columns: Set[str] = None,
     ):
         """
         Applies all the transformations for a single output column
 
         :param row: The current input row
         :param entry_list: A list of all the transformations to apply to
             generate the output series
 
         :return: The transformation result
         """
-        if entry_list[0].transformation in missing_columns:
-            return NotSet
-        else:
-            result = reduce(
-                lambda current_column_value, entry: self.combine_column(
-                    row,
-                    current_column_value,
-                    entry,
-                ),
-                entry_list,
-                NotSet,
-            )
-            return result
+        result = reduce(
+            lambda current_column_value, entry: self.combine_column(
+                row,
+                current_column_value,
+                entry,
+            ),
+            entry_list,
+            NotSet,
+        )
+        return result
 
     def apply_transformation_set(
         self,
         row: RowType,
         transformations: DirectionalMapping,
-        missing_columns: Set[str] = None,
     ) -> RowType:
         """
         Applies all the transformations to produce the output row
 
         :param row: The current input row
         :param transformations: The full set of column conversions and
             transformation sets to apply to the ``row`` row.
@@ -217,15 +211,15 @@
 
         return reduce(
             lambda target, col_transforms: self.assign(
                 row,
                 target,
                 **{
                     col_transforms[0]: self.apply_column_transformation(
-                        coerced_row, col_transforms[1], missing_columns=missing_columns
+                        coerced_row, col_transforms[1]
                     )
                 },
             ),
             transformations.transformation_set.items(),
             NotSet,
         )
```

### Comparing `ods_tools-3.2.2/ods_tools/odtf/runner/pandas.py` & `ods_tools-3.2.3/ods_tools/odtf/runner/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 
 import pandas as pd
 from numpy import nan
 
 from ..connector.base import BaseConnector
 from ..mapping.base import (
     BaseMapping,
-    DirectionalMapping,
     ColumnConversions,
     TransformationEntry
 )
 from ..transformers import run
 from ..transformers.transform import (
     GroupWrapper,
     RowType,
     TransformerMapping,
     default_match,
-    default_search,
-    transform_loc_perils
+    default_search
 )
+from ..transformers.transform_utils import replace_multiple
 from ..notset import NotSet, NotSetType
 from ..validator_pandas import PandasValidator
 from .base import BaseRunner
 #
 # Group Wrappers
 #
 if tuple(map(int, pd.__version__.split('.'))) >= (2, 1, 9):
@@ -382,15 +381,15 @@
             "not_in": not_in_transformer,
             "any": lambda r, values: PandasAnyWrapper(values),
             "all": lambda r, values: PandasAllWrapper(values),
             "str_replace": StrReplace(self.series_type),
             "str_match": StrMatch(self.series_type),
             "str_search": StrSearch(self.series_type),
             "str_join": StrJoin(self.series_type),
-            "transform_loc_perils": transform_loc_perils,
+            "replace_multiple": replace_multiple,
         }
 
         # process the when clause to get a filter series
         filter_series = run(
             input_df, entry.when_tree or entry.when, transformer_mapping
         )
 
@@ -419,42 +418,31 @@
             return result
         else:
             return self.create_series(input_df.index, result)
 
     def transform(
         self, extractor: BaseConnector, mapping: BaseMapping
     ) -> Iterable[Dict[str, Any]]:
-        transformations = mapping.get_transformations()
+        available_columns = set(pd.read_csv(extractor.file_path, nrows=1).columns)
+        transformations = mapping.get_transformations(available_columns=available_columns)
 
         validator = PandasValidator(search_paths=([os.path.dirname(self.config.path)] if self.config.path else []))
 
         logger.info(f"Running transformation set {transformations[0].input_format} -> {transformations[-1].output_format}")
         total_rows = 0
         runner_config = self.config.config.get('runner', None)
-        batch_size = runner_config.get('batch_size', 10000)
+        batch_size = runner_config.get('batch_size', 50000)
 
         for batch in pd.read_csv(extractor.file_path, chunksize=batch_size, low_memory=False):
-            # Check if all the columns necessary for the transformations are present. If not, drop the transformations we can't run
-            missing_columns = set(transformations[0].types.keys()) - set(batch.columns)
-            updated_transformations = [
-                DirectionalMapping(
-                    input_format=t.input_format,
-                    output_format=t.output_format,
-                    transformation_set={k: v for k, v in t.transformation_set.items() if k not in missing_columns},
-                    types=t.types,
-                    null_values=t.null_values,
-                )
-                for t in transformations
-            ]
 
-            validator.run(self.coerce_row_types(batch, updated_transformations[0].types),
+            validator.run(self.coerce_row_types(batch, transformations[0].types),
                           mapping.input_format.name, mapping.input_format.version, mapping.file_type)
 
             transformed = batch
-            for transformation in updated_transformations:
-                transformed = self.apply_transformation_set(transformed, transformation, missing_columns)
+            for transformation in transformations:
+                transformed = self.apply_transformation_set(transformed, transformation)
 
             validator.run(transformed, mapping.output_format.name, mapping.output_format.version, mapping.file_type)
             total_rows += len(batch)
             logger.info(f"Processed {len(batch)} rows in the current batch (total: {total_rows})")
 
             yield from (r.to_dict() for idx, r in transformed.iterrows())
```

### Comparing `ods_tools-3.2.2/ods_tools/odtf/transformers/grammar.py` & `ods_tools-3.2.3/ods_tools/odtf/transformers/grammar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from lark import lark
 
-
 _grammar = r"""
 ?start: expression
 
 ?expression: product
            | comparison
            | "not" comparison -> logical_not
            | expression "or" comparison -> logical_or
@@ -45,25 +44,26 @@
 array: "[" [expression ("," expression)*] "]"
 
 ?lookup: "lookup(" string ")" -> lookup
        | IDENT -> lookup
 
 ?string_manip: "join(" string [("," expression)*] ")" -> str_join
              | "replace(" expression [("," pattern "," expression)+] ")" -> str_replace
-             | "transform_loc_perils(" expression [("," STRING)*] ")" -> transform_loc_perils
+             | "replace_multiple(" expression "," string "," string ("," string "," string)* ")" -> replace_multiple
              | "match(" expression "," pattern ")" -> str_match
              | "search(" expression "," pattern ")" -> str_search
 
 ?pattern: string
         | regex
 
 ?regex: "re" string -> regex
       | "ire" string -> iregex
 
 ?string: "'" STRING "'" -> string
+       | "'''" STRING "'''" -> string
        | "''"  -> string
 
 IDENT: /[a-zA-Z][a-zA-Z0-9_]*/
 STRING: /((`['`])|([^']))+/
 BOOL: /True|False/
 NULL: /Null/
```

### Comparing `ods_tools-3.2.2/ods_tools/odtf/transformers/transform.py` & `ods_tools-3.2.3/ods_tools/odtf/transformers/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 import re
 from functools import partial
 from operator import add, mul, sub
 from operator import truediv as div
 from typing import Any, Callable, Iterable, List, Pattern, TypedDict, Union
 
 from lark import Transformer as _LarkTransformer
 from lark import Tree
 from lark import exceptions as lark_exceptions
 from lark import v_args
+from ..transformers.transform_utils import replace_multiple
 
 from .errors import UnexpectedCharacters
 from .grammar import parser
 
 
 RowType = Any
+logger = logging.getLogger(__name__)
 
 
 class TransformerMapping(TypedDict, total=False):
     lookup: Callable[[RowType, str], Any]
 
     # math operators
     add: Callable[[RowType, Any, Any], Any]
@@ -371,36 +374,14 @@
     :param elements: The elements to join
 
     :return: The joined string
     """
     return str(join).join(map(str, elements))
 
 
-def transform_loc_perils(row: RowType, target, *pattern_repl):
-    if isinstance(target, str):
-        perils = [p.strip() for p in target.split(',')]
-        transformed_perils = []
-
-        # Convert the pattern_repl tuple to a list of pairs
-        pattern_repl_list = list(zip(pattern_repl[::2], pattern_repl[1::2]))
-
-        for peril in perils:
-            for pattern, repl in pattern_repl_list:
-                if peril == pattern.strip("'"):
-                    transformed_perils.append(repl.strip("'"))
-                    break
-            else:
-                transformed_perils.append(peril)
-
-        # Join the transformed perils using a comma and space
-        return ', '.join(transformed_perils)
-    else:
-        return target
-
-
 @v_args(inline=True)
 class BaseTreeTransformer(_LarkTransformer):
     """
     Abstract implementation of the Tree transformer class
     """
 
     lookup: Callable[[RowType, str], Any]
@@ -421,14 +402,15 @@
     logical_and: Callable[[RowType, Any, Any], Any]
     any: Callable[[RowType, List[Any]], GroupWrapper]
     all: Callable[[RowType, List[Any]], GroupWrapper]
     str_join: Callable[..., Any]
     str_replace: Callable[[RowType, Any, Pattern, Any], Any]
     str_match: Callable[[RowType, Any, Pattern, Any], Any]
     str_search: Callable[[RowType, Any, Pattern, Any], Any]
+    replace_multiple: Callable[..., Any]
 
     array = v_args(inline=False)(list)
     string_escape_re = re.compile(r"`([`'])")
 
     def string(self, value=""):
         """
         Parses a string from the transformer language and performs any
@@ -525,15 +507,15 @@
         "logical_not": lambda r, v: not v,
         "any": lambda r, v: AnyWrapper(v),
         "all": lambda r, v: AllWrapper(v),
         "str_join": default_join,
         "str_replace": default_replace,
         "str_match": default_match,
         "str_search": default_search,
-        "transform_loc_perils": transform_loc_perils,
+        "replace_multiple": replace_multiple,
         **(transformer_mapping or {}),
     }
 
     def mapped_function(name, *args, **kwargs):
         return transformer_mapping[name](row, *args, **kwargs)
 
     @v_args(inline=True)
@@ -556,15 +538,15 @@
         logical_and = partial(mapped_function, "logical_and")
         any = partial(mapped_function, "any")
         all = partial(mapped_function, "all")
         str_join = partial(mapped_function, "str_join")
         str_replace = partial(mapped_function, "str_replace")
         str_match = partial(mapped_function, "str_match")
         str_search = partial(mapped_function, "str_search")
-
+        replace_multiple = partial(mapped_function, "replace_multiple")
     return TreeTransformer
 
 
 def parse(expression: Union[str, Tree]) -> Tree:
     """
     Parse an expression from the transformation language
```

### Comparing `ods_tools-3.2.2/ods_tools/odtf/validator_base.py` & `ods_tools-3.2.3/ods_tools/odtf/validator_base.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/odtf/validator_pandas.py` & `ods_tools-3.2.3/ods_tools/odtf/validator_pandas.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/oed/__init__.py` & `ods_tools-3.2.3/ods_tools/oed/__init__.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/oed/common.py` & `ods_tools-3.2.3/ods_tools/oed/common.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/oed/exposure.py` & `ods_tools-3.2.3/ods_tools/oed/exposure.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/oed/forex.py` & `ods_tools-3.2.3/ods_tools/oed/forex.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/oed/oed_schema.py` & `ods_tools-3.2.3/ods_tools/oed/oed_schema.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/oed/setting_schema.py` & `ods_tools-3.2.3/ods_tools/oed/setting_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         schema (dict): The JSON schema being used for validation.
         settings_type (str): A string describing the type of settings being loaded.
 
     Methods:
         from_json(cls, setting_json): Creates a new instance of the `SettingSchema` class by loading a JSON file.
         compatibility(self, settings_data): Updates the loaded JSON data to account for deprecated keys.
         load(self, settings_fp): Loads the JSON data from a file path.
+        check_unique_summary_ids(self, setting_data): Ensures that the JSON data contains unique summary IDs for each runtype.
         validate(self, setting_data): Validates the loaded JSON data against the schema.
         get(self, settings_fp, key=None, validate=True): Gets a value from the loaded JSON data.
 
     """
     SCHEMA_FILE = ''
 
     def __init__(self, schema=None, json_path=None, settings_type=''):
@@ -155,14 +156,38 @@
             with filepath.open(encoding="UTF-8") as f:
                 settings_raw = json.load(f)
                 settings_data = self.compatibility(settings_raw)
         except (IOError, TypeError, ValueError):
             raise OdsException(f'Invalid {self.settings_type} file or file path: {settings_fp}')
         return settings_data
 
+    def check_unique_summary_ids(self, setting_data):
+        """
+        Ensures that the JSON data contains unique summary IDs for each
+        runtype.
+
+        Args:
+            setting_data (dict): The loaded JSON data.
+
+        Returns:
+            dict: Exception messages. Will be empty if there are no unique
+            summary IDs.
+
+        """
+        exception_msgs = {}
+        runtype_summaries = [f'{runtype}_summaries' for runtype in ['gul', 'il', 'ri']]
+        for runtype_summary in runtype_summaries:
+            summary_ids = [summary.get('id', []) for summary in setting_data.get(runtype_summary, [])]
+            duplicate_ids = set(summary_id for summary_id in summary_ids if summary_ids.count(summary_id) > 1)
+            if duplicate_ids:
+                error_msgs = [f'id {summary_id} is duplicated' for summary_id in duplicate_ids]
+                exception_msgs[runtype_summary] = error_msgs
+
+        return exception_msgs
+
     def validate(self, setting_data, raise_error=True):
         """
         Validates the loaded JSON data against the schema.
 
         Args:
             setting_data (dict): The loaded JSON data.
             raise_error (bool): raise execption on validation failuer
@@ -170,16 +195,16 @@
         Returns:
             tuple: A tuple containing a boolean indicating whether the JSON data is valid
             and a dictionary containing any validation errors.
 
         """
         validator = jsonschema.Draft4Validator(self.schema)
         validation_errors = [e for e in validator.iter_errors(setting_data)]
-        exception_msgs = {}
-        is_valid = validator.is_valid(setting_data)
+        exception_msgs = self.check_unique_summary_ids(setting_data)
+        is_valid = validator.is_valid(setting_data) and not exception_msgs
 
         if validation_errors:
             for err in validation_errors:
                 if err.path:
                     field = '-'.join([str(e) for e in err.path])
                 elif err.schema_path:
                     field = '-'.join([str(e) for e in err.schema_path])
```

### Comparing `ods_tools-3.2.2/ods_tools/oed/source.py` & `ods_tools-3.2.3/ods_tools/oed/source.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools/oed/validator.py` & `ods_tools-3.2.3/ods_tools/oed/validator.py`

 * *Files identical despite different names*

### Comparing `ods_tools-3.2.2/ods_tools.egg-info/PKG-INFO` & `ods_tools-3.2.3/ods_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ods-tools
-Version: 3.2.2
+Version: 3.2.3
 Summary: Tools to manage ODS files
 Home-page: https://github.com/OasisLMF/OpenDataStandards
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ods_tools-3.2.2/ods_tools.egg-info/SOURCES.txt` & `ods_tools-3.2.3/ods_tools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 ods_tools/odtf/runner/__init__.py
 ods_tools/odtf/runner/base.py
 ods_tools/odtf/runner/pandas.py
 ods_tools/odtf/transformers/__init__.py
 ods_tools/odtf/transformers/errors.py
 ods_tools/odtf/transformers/grammar.py
 ods_tools/odtf/transformers/transform.py
+ods_tools/odtf/transformers/transform_utils.py
 ods_tools/oed/__init__.py
 ods_tools/oed/common.py
 ods_tools/oed/exposure.py
 ods_tools/oed/forex.py
 ods_tools/oed/oed_schema.py
 ods_tools/oed/setting_schema.py
 ods_tools/oed/source.py
```

### Comparing `ods_tools-3.2.2/setup.py` & `ods_tools-3.2.3/setup.py`

 * *Files identical despite different names*

