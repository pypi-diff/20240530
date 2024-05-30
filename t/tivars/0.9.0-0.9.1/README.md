# Comparing `tmp/tivars-0.9.0.tar.gz` & `tmp/tivars-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tivars-0.9.0.tar", last modified: Mon Apr 22 20:06:03 2024, max compression
+gzip compressed data, was "tivars-0.9.1.tar", last modified: Thu May 30 21:25:56 2024, max compression
```

## Comparing `tivars-0.9.0.tar` & `tivars-0.9.1.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.342629 tivars-0.9.0/
--rw-rw-rw-   0        0        0     1093 2023-12-28 22:35:37.000000 tivars-0.9.0/LICENSE
--rw-rw-rw-   0        0        0    10710 2024-04-22 20:06:03.342629 tivars-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     8893 2024-04-22 20:05:27.000000 tivars-0.9.0/README.md
--rw-rw-rw-   0        0        0     1897 2024-04-22 20:05:27.000000 tivars-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 20:06:03.342629 tivars-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.320944 tivars-0.9.0/tivars/
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.327261 tivars-0.9.0/tivars/PIL/
--rw-rw-rw-   0        0        0      509 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/TI8caPlugin.py
--rw-rw-rw-   0        0        0      529 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/TI8ciPlugin.py
--rw-rw-rw-   0        0        0      558 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/TI8xiPlugin.py
--rw-rw-rw-   0        0        0      183 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/__init__.py
--rw-rw-rw-   0        0        0     3010 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/PIL/common.py
--rw-rw-rw-   0        0        0      309 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/__init__.py
--rw-rw-rw-   0        0        0    17327 2024-04-22 14:46:46.000000 tivars-0.9.0/tivars/data.py
--rw-rw-rw-   0        0        0     4064 2023-12-31 23:22:16.000000 tivars-0.9.0/tivars/flags.py
--rw-rw-rw-   0        0        0    25084 2024-04-22 16:40:44.000000 tivars-0.9.0/tivars/flash.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.328287 tivars-0.9.0/tivars/models/
--rw-rw-rw-   0        0        0      553 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/models/__init__.py
--rw-rw-rw-   0        0        0     7215 2024-04-22 14:46:46.000000 tivars-0.9.0/tivars/models/model.py
--rw-rw-rw-   0        0        0      523 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/models/versions.py
--rw-rw-rw-   0        0        0     5136 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/numeric.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.328287 tivars-0.9.0/tivars/tokenizer/
--rw-rw-rw-   0        0        0     2519 2024-01-03 06:10:34.000000 tivars-0.9.0/tivars/tokenizer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.329662 tivars-0.9.0/tivars/tokens/
--rw-rw-rw-   0        0        0    89045 2024-01-12 06:13:35.000000 tivars-0.9.0/tivars/tokens/73.xml
--rw-rw-rw-   0        0        0   243356 2024-01-27 18:37:59.000000 tivars-0.9.0/tivars/tokens/8X.xml
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.332665 tivars-0.9.0/tivars/tokens/scripts/
--rw-rw-rw-   0        0        0      316 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/__init__.py
--rw-rw-rw-   0        0        0      677 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/build.py
--rw-rw-rw-   0        0        0     6516 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/formats.py
--rw-rw-rw-   0        0        0    10440 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/parse.py
--rw-rw-rw-   0        0        0     7135 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/tokenide.py
--rw-rw-rw-   0        0        0     2370 2024-01-12 06:36:47.000000 tivars-0.9.0/tivars/tokens/scripts/trie.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.339090 tivars-0.9.0/tivars/types/
--rw-rw-rw-   0        0        0     1664 2023-12-31 23:01:25.000000 tivars-0.9.0/tivars/types/__init__.py
--rw-rw-rw-   0        0        0      977 2023-12-30 04:00:29.000000 tivars-0.9.0/tivars/types/appvar.py
--rw-rw-rw-   0        0        0    12017 2024-01-13 17:19:27.000000 tivars-0.9.0/tivars/types/complex.py
--rw-rw-rw-   0        0        0     1780 2024-01-13 17:15:58.000000 tivars-0.9.0/tivars/types/flash.py
--rw-rw-rw-   0        0        0    45527 2024-04-22 15:19:59.000000 tivars-0.9.0/tivars/types/gdb.py
--rw-rw-rw-   0        0        0     5188 2024-02-21 18:17:10.000000 tivars-0.9.0/tivars/types/group.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.341125 tivars-0.9.0/tivars/types/json/
--rw-rw-rw-   0        0        0     2442 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/func.default.json
--rw-rw-rw-   0        0        0     2903 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/param.default.json
--rw-rw-rw-   0        0        0     1734 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/polar.default.json
--rw-rw-rw-   0        0        0     1284 2023-12-28 22:35:37.000000 tivars-0.9.0/tivars/types/json/seq.default.json
--rw-rw-rw-   0        0        0     6347 2023-12-30 22:09:28.000000 tivars-0.9.0/tivars/types/list.py
--rw-rw-rw-   0        0        0     5857 2023-12-30 22:07:29.000000 tivars-0.9.0/tivars/types/matrix.py
--rw-rw-rw-   0        0        0    11665 2023-12-30 04:00:29.000000 tivars-0.9.0/tivars/types/picture.py
--rw-rw-rw-   0        0        0    18833 2023-12-30 04:00:29.000000 tivars-0.9.0/tivars/types/real.py
--rw-rw-rw-   0        0        0    17351 2023-12-30 04:03:46.000000 tivars-0.9.0/tivars/types/settings.py
--rw-rw-rw-   0        0        0    13624 2024-04-22 14:46:46.000000 tivars-0.9.0/tivars/types/tokenized.py
--rw-rw-rw-   0        0        0    37711 2024-04-22 20:05:27.000000 tivars-0.9.0/tivars/var.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:06:03.341125 tivars-0.9.0/tivars.egg-info/
--rw-rw-rw-   0        0        0    10710 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 20:06:03.000000 tivars-0.9.0/tivars.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.752484 tivars-0.9.1/
+-rw-rw-rw-   0        0        0     1093 2023-09-30 15:55:27.000000 tivars-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0    10710 2024-05-30 21:25:56.750483 tivars-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8893 2024-05-30 21:19:46.000000 tivars-0.9.1/README.md
+-rw-rw-rw-   0        0        0     1897 2024-05-30 21:20:04.000000 tivars-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 21:25:56.752484 tivars-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.663484 tivars-0.9.1/tivars/
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.696519 tivars-0.9.1/tivars/PIL/
+-rw-rw-rw-   0        0        0      509 2023-09-30 15:55:27.000000 tivars-0.9.1/tivars/PIL/TI8caPlugin.py
+-rw-rw-rw-   0        0        0      529 2023-09-30 15:55:27.000000 tivars-0.9.1/tivars/PIL/TI8ciPlugin.py
+-rw-rw-rw-   0        0        0      558 2023-09-30 15:55:27.000000 tivars-0.9.1/tivars/PIL/TI8xiPlugin.py
+-rw-rw-rw-   0        0        0      183 2023-09-30 15:55:27.000000 tivars-0.9.1/tivars/PIL/__init__.py
+-rw-rw-rw-   0        0        0     3010 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/PIL/common.py
+-rw-rw-rw-   0        0        0      309 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/__init__.py
+-rw-rw-rw-   0        0        0    17495 2024-05-28 06:28:34.000000 tivars-0.9.1/tivars/data.py
+-rw-rw-rw-   0        0        0     4053 2024-05-28 06:18:07.000000 tivars-0.9.1/tivars/flags.py
+-rw-rw-rw-   0        0        0    25377 2024-05-28 06:33:20.000000 tivars-0.9.1/tivars/flash.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.700524 tivars-0.9.1/tivars/models/
+-rw-rw-rw-   0        0        0      553 2023-09-30 15:55:27.000000 tivars-0.9.1/tivars/models/__init__.py
+-rw-rw-rw-   0        0        0     7215 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/models/model.py
+-rw-rw-rw-   0        0        0      523 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/models/versions.py
+-rw-rw-rw-   0        0        0     5136 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/numeric.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.707481 tivars-0.9.1/tivars/tokenizer/
+-rw-rw-rw-   0        0        0     1189 2024-05-28 19:23:59.000000 tivars-0.9.1/tivars/tokenizer/__init__.py
+-rw-rw-rw-   0        0        0     2253 2024-05-27 04:58:10.000000 tivars-0.9.1/tivars/tokenizer/decoder.py
+-rw-rw-rw-   0        0        0     3282 2024-05-29 20:12:14.000000 tivars-0.9.1/tivars/tokenizer/encoder.py
+-rw-rw-rw-   0        0        0     5125 2024-05-27 22:18:32.000000 tivars-0.9.1/tivars/tokenizer/state.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.710483 tivars-0.9.1/tivars/tokens/
+-rw-rw-rw-   0        0        0    89045 2024-05-12 17:25:40.000000 tivars-0.9.1/tivars/tokens/73.xml
+-rw-rw-rw-   0        0        0   243362 2024-05-27 03:28:39.000000 tivars-0.9.1/tivars/tokens/8X.xml
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.719483 tivars-0.9.1/tivars/tokens/scripts/
+-rw-rw-rw-   0        0        0      316 2024-05-12 17:25:40.000000 tivars-0.9.1/tivars/tokens/scripts/__init__.py
+-rw-rw-rw-   0        0        0      677 2024-05-12 17:25:40.000000 tivars-0.9.1/tivars/tokens/scripts/build.py
+-rw-rw-rw-   0        0        0     6516 2024-05-27 03:28:39.000000 tivars-0.9.1/tivars/tokens/scripts/formats.py
+-rw-rw-rw-   0        0        0    10440 2024-05-27 03:28:39.000000 tivars-0.9.1/tivars/tokens/scripts/parse.py
+-rw-rw-rw-   0        0        0     7135 2024-05-12 17:25:40.000000 tivars-0.9.1/tivars/tokens/scripts/tokenide.py
+-rw-rw-rw-   0        0        0     2370 2024-05-12 17:25:40.000000 tivars-0.9.1/tivars/tokens/scripts/trie.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.741483 tivars-0.9.1/tivars/types/
+-rw-rw-rw-   0        0        0     1664 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/types/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/types/appvar.py
+-rw-rw-rw-   0        0        0    12199 2024-05-28 06:30:17.000000 tivars-0.9.1/tivars/types/complex.py
+-rw-rw-rw-   0        0        0     1780 2024-05-12 17:25:19.000000 tivars-0.9.1/tivars/types/flash.py
+-rw-rw-rw-   0        0        0    45844 2024-05-28 06:16:04.000000 tivars-0.9.1/tivars/types/gdb.py
+-rw-rw-rw-   0        0        0     5207 2024-05-28 06:51:52.000000 tivars-0.9.1/tivars/types/group.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.746486 tivars-0.9.1/tivars/types/json/
+-rw-rw-rw-   0        0        0     2442 2023-05-11 01:28:40.000000 tivars-0.9.1/tivars/types/json/func.default.json
+-rw-rw-rw-   0        0        0     2903 2023-05-11 01:28:34.000000 tivars-0.9.1/tivars/types/json/param.default.json
+-rw-rw-rw-   0        0        0     1734 2023-05-11 01:28:45.000000 tivars-0.9.1/tivars/types/json/polar.default.json
+-rw-rw-rw-   0        0        0     1284 2023-05-11 01:28:49.000000 tivars-0.9.1/tivars/types/json/seq.default.json
+-rw-rw-rw-   0        0        0     6480 2024-05-28 06:51:52.000000 tivars-0.9.1/tivars/types/list.py
+-rw-rw-rw-   0        0        0     5922 2024-05-28 06:11:40.000000 tivars-0.9.1/tivars/types/matrix.py
+-rw-rw-rw-   0        0        0    11996 2024-05-28 06:50:08.000000 tivars-0.9.1/tivars/types/picture.py
+-rw-rw-rw-   0        0        0    18715 2024-05-28 06:16:58.000000 tivars-0.9.1/tivars/types/real.py
+-rw-rw-rw-   0        0        0    17351 2024-05-28 05:23:00.000000 tivars-0.9.1/tivars/types/settings.py
+-rw-rw-rw-   0        0        0    11829 2024-05-28 19:26:51.000000 tivars-0.9.1/tivars/types/tokenized.py
+-rw-rw-rw-   0        0        0    39023 2024-05-30 21:19:40.000000 tivars-0.9.1/tivars/var.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:25:56.748484 tivars-0.9.1/tivars.egg-info/
+-rw-rw-rw-   0        0        0    10710 2024-05-30 21:25:56.000000 tivars-0.9.1/tivars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2024-05-30 21:25:56.000000 tivars-0.9.1/tivars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 21:25:56.000000 tivars-0.9.1/tivars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-30 21:25:56.000000 tivars-0.9.1/tivars.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 21:25:56.000000 tivars-0.9.1/tivars.egg-info/top_level.txt
```

### Comparing `tivars-0.9.0/LICENSE` & `tivars-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/PKG-INFO` & `tivars-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tivars
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for interacting with TI-(e)z80 (82/83/84 series) calculator files
 License: The MIT License (MIT)
         
         Copyright (c) 2023 kg583
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -39,15 +39,15 @@
 
 `tivars_lib_py` is a Python package for interacting with TI-(e)z80 (82/83/84 series) calculator files, i.e. lists, programs, matrices, appvars, etc.
 
 Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have been made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting, dynamic typing).
 
 ## Installation
 
-The current release version is `v0.9.0`. All versions require Python 3.10+ to run.
+The current release version is `v0.9.1`. All versions require Python 3.10+ to run.
 
 ### As a Package
 
 Install the `tivars` package from PyPI using `pip`:
 ```
 pip install tivars
 ```
```

### Comparing `tivars-0.9.0/README.md` & `tivars-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 `tivars_lib_py` is a Python package for interacting with TI-(e)z80 (82/83/84 series) calculator files, i.e. lists, programs, matrices, appvars, etc.
 
 Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have been made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting, dynamic typing).
 
 ## Installation
 
-The current release version is `v0.9.0`. All versions require Python 3.10+ to run.
+The current release version is `v0.9.1`. All versions require Python 3.10+ to run.
 
 ### As a Package
 
 Install the `tivars` package from PyPI using `pip`:
 ```
 pip install tivars
 ```
```

### Comparing `tivars-0.9.0/pyproject.toml` & `tivars-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.package-data]
 "*" = ["*.default.json", "*.xml"]
 
 
 [project]
 name = "tivars"
-version = "0.9.0"
+version = "0.9.1"
 description = "A library for interacting with TI-(e)z80 (82/83/84 series) calculator files"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 
 [project.urls]
 Repository = "https://github.com/TI-Toolkit/tivars_lib_py"
```

### Comparing `tivars-0.9.0/tivars/PIL/TI8ciPlugin.py` & `tivars-0.9.1/tivars/PIL/TI8ciPlugin.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/PIL/TI8xiPlugin.py` & `tivars-0.9.1/tivars/PIL/TI8xiPlugin.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/PIL/common.py` & `tivars-0.9.1/tivars/PIL/common.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/data.py` & `tivars-0.9.1/tivars/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,17 @@
         See the `Dock` and `Loader` classes for implementation details.
 """
 
 
 import copy
 import inspect
 
+from collections.abc import Callable
 from math import ceil
-from typing import Callable, TypeVar
+from typing import TypeVar
 from warnings import warn
 
 
 _T = TypeVar('_T')
 
 
 class Converter:
@@ -114,15 +115,17 @@
         Converts ``bytes`` -> ``bytes`` and updates metadata fields
 
         :param value: The value to convert
         :param instance: The instance which contains the data section
         :return: The bytes in ``value``, unchanged
         """
 
-        instance.version = instance.get_version(value)
+        if instance is not None:
+            instance.version = instance.get_version(value)
+
         return super().set(value)
 
 
 class SizedData(Data):
     """
     No-op converter for sized data sections with associated metadata
 
@@ -132,15 +135,17 @@
             - Length
     """
 
     _T = bytes
 
     @classmethod
     def set(cls, value: _T, *, instance=None, **kwargs) -> _T:
-        instance.length = len(value)
+        if instance is not None:
+            instance.length = len(value)
+
         return super().set(value, instance=instance)
 
 
 class Boolean(Converter):
     """
     Converter for data sections best interpreted as boolean flags
 
@@ -382,15 +387,16 @@
     def __call__(self, func: Callable) -> 'Section':
         new = copy.copy(self)
         new.__doc__ = func.__doc__
 
         signature = inspect.signature(func)
         match len(signature.parameters):
             case 1: pass
-            case 2: new._set = lambda value, _set=new._set, **kwargs: _set(func(self, value), **kwargs)
+            case 2: new._set = lambda value, _set=self._set, *, instance=None, **kwargs:\
+                _set(func(instance, value), instance=instance, **kwargs)
             case _: raise TypeError("Section and View function definitions can only take 1 or 2 parameters.")
 
         return new
 
     def _get_raw(self, instance) -> bytes:
         return getattr(instance.raw, self._name, None)
```

### Comparing `tivars-0.9.0/tivars/flags.py` & `tivars-0.9.1/tivars/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
     -   `Flags`, which converts between a bitfield and a ``dict`` of bitsets.
 
         The ``dict`` representation permits the use of ``dict`` update notation to set flags with a single operation.
 """
 
 
+from collections.abc import Mapping
 from functools import total_ordering
 from math import ceil
-from typing import Mapping
 from warnings import warn
 
 from .data import *
 
 
 class Enum(Converter):
     """
@@ -76,15 +76,15 @@
     Base class for flag types
 
     Flags are bitfields in a byte that are set or cleared using dict update notation.
     """
 
     _T = 'Flags'
 
-    def __init__(self, bitsets: Mapping[int, int] | 'Flags' = None, *, width: int = 8):
+    def __init__(self, bitsets: Mapping[int, int] = None, *, width: int = 8):
         """
         Creates an empty `Flags` instance with a given initial state and width
 
         :param bitsets: The initial state of these flags
         :param width: The number of bitfields used for these flags (defaults to ``8``)
         """
 
@@ -101,15 +101,15 @@
 
     def __int__(self) -> int:
         return int(str(self), 2)
 
     def __str__(self) -> str:
         return ''.join([str(bit) for bit in self.values()][::-1])
 
-    def __contains__(self, bitsets: Mapping[int, int] | 'Flags') -> bool:
+    def __contains__(self, bitsets: Mapping[int, int]) -> bool:
         return all(self[bit] == int(bool(bitsets[bit])) for bit in bitsets)
 
     has = __contains__
 
     @classmethod
     def get(cls, data: bytes, **kwargs) -> _T:
         """
```

### Comparing `tivars-0.9.0/tivars/flash.py` & `tivars-0.9.1/tivars/flash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """
 The fundamental flash file components
 """
 
 
 from io import BytesIO
-from typing import BinaryIO, Type
+from sys import version_info
+from typing import BinaryIO
 from warnings import warn
 
 from .data import *
 from .flags import *
 from .models import *
 from .numeric import BCD
 
 
+match version_info[:2]:
+    case 3, 10:
+        Self = 'TIFlashHeader'
+
+    case _:
+        from typing import Self
+
+
 class DeviceType(Enum):
     """
     Enum of flash device types
     """
 
     TI_83P = 0x73
     TI_73 = 0x74
@@ -282,43 +291,51 @@
         return self.raw.bytes()
 
 
 class FlashData(Converter):
     """
     Converter to split flash data into blocks if stored in Intel format
 
-    If ``binary_flag == $01``, this converter manipulates ``list[TIFlashBlock]``.
-    Otherwise, this converter is a no-op on ``bytes``.
+    If ``binary_flag != $01``, this converter is a no-op on ``bytes``.
+    Otherwise, this converter manipulates ``list[TIFlashBlock]``.
     """
 
     _T = bytes | list[TIFlashBlock]
 
     @classmethod
-    def get(cls, data: bytes, *, instance=None, **kwargs) -> _T:
+    def get(cls, data: bytes, *, instance=None) -> _T:
         """
         Converts ``bytes`` -> ``bytes | list[TIFlashBlock]``
 
         :param data: The raw bytes to convert
         :param instance: The instance which contains the data section
         :return: The blocks stored in ``data``
         """
 
-        return list(map(TIFlashBlock, data.split(b'\r\n'))) if instance.binary_flag == 0x01 else data
+        if instance is None or instance.binary_flag == 0x01:
+            return list(map(TIFlashBlock, data.split(b'\r\n')))
+
+        else:
+            return data
 
     @classmethod
     def set(cls, value: _T, *, instance=None, **kwargs) -> bytes:
         """
         Converts ``bytes | list[TIFlashBlock]`` -> ``bytes``
 
         :param value: The value to convert
         :param instance: The instance which contains the data section
         :return: The concatenation of the blocks in ``value``
         """
 
-        return b'\r\n'.join(block.bytes() for block in value) if instance.binary_flag == 0x01 else value
+        if instance is None or instance.binary_flag == 0x01:
+            return b'\r\n'.join(block.bytes() for block in value)
+
+        else:
+            return value
 
 
 class TIFlashHeader(Dock):
     """
     Parser for flash headers
 
     A flash file can contain up to three headers, though usually only one.
@@ -543,15 +560,15 @@
 
         This is equal to the lower 2 bytes of the sum of all bytes in the header.
         """
 
         return self.raw.checksum
 
     @classmethod
-    def get_type(cls, type_id: int) -> Type['TIFlashHeader']:
+    def get_type(cls, type_id: int) -> type['TIFlashHeader'] | None:
         """
         Gets the subclass corresponding to a type ID if one is registered
 
         :param type_id: The type ID to search by
         :return: A subclass of `TIFlashHeader` with corresponding type ID or ``None``
         """
 
@@ -582,15 +599,15 @@
                 entry_length = 78 + data_size + 2
                 stream.seek(-len(remaining), 1)
 
         stream.seek(-78 - data_size, 1)
         return entry_length
 
     @classmethod
-    def register(cls, var_type: Type['TIFlashHeader'], override: int = None):
+    def register(cls, var_type: type['TIFlashHeader'], override: int = None):
         """
         Registers a subtype with this class for coercion
 
         :param var_type: The `TIFlashHeader` subtype to register
         :param override: A type ID to use for registry that differs from that of the var type
         """
 
@@ -735,15 +752,15 @@
         while offset:
             file.seek(self.next_header_length(file), 1)
             offset -= 1
 
         self.load_bytes(file.read(self.next_header_length(file)))
 
     @classmethod
-    def open(cls, filename: str) -> 'TIFlashHeader':
+    def open(cls, filename: str) -> Self:
         """
         Creates a new header from a file given a filename
 
         :param filename: A filename to open
         :return: The (first) header stored in the file
         """
 
@@ -761,15 +778,15 @@
                     warn(f"The selected flash file contains unexpected additional data: {remaining}.",
                          BytesWarning)
 
         return header
 
     def save(self, filename: str = None, model: TIModel = TI_84PCE):
         """
-        Saves this header given a filename and targeted model
+        Saves this header to the current directory given a filename and targeted model
 
         :param filename: A filename to save to (defaults to the header's name and extension)
         :param model: A model to target (defaults to ``TI_84PCE``)
         """
 
         with open(filename or self.filename(model), 'wb+') as file:
             file.write(self.bytes())
```

### Comparing `tivars-0.9.0/tivars/models/__init__.py` & `tivars-0.9.1/tivars/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/models/model.py` & `tivars-0.9.1/tivars/models/model.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/models/versions.py` & `tivars-0.9.1/tivars/models/versions.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/numeric.py` & `tivars-0.9.1/tivars/numeric.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/tokenizer/__init__.py` & `tivars-0.9.1/tivars/tokenizer/decoder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 """
-Tokenization utilities derived from the token sheets (see tokens directory)
+Token stream decoder
 """
 
 
-from tivars.data import String
 from tivars.models import *
 from tivars.tokens.scripts import *
 
 
 def decode(bytestream: bytes, *,
            tokens: Tokens = None, lang: str = "en",
            mode: str = "display") -> tuple[str | bytes, OsVersion]:
+    """
+    Decodes a byte stream into a string of tokens and its minimum supported OS version
+
+    Each token is represented using one of three different representations formats, dictated by ``mode``:
+        - ``display``: Represents the tokens with Unicode characters matching the calculator's display
+        - ``accessible``: Represents the tokens with ASCII-only equivalents, often requiring multi-character glyphs
+        - ``ti_ascii``: Represents the tokens with their internal font indices (returns a ``bytes`` object)
+
+    :param bytestream: The token bytes to decode
+    :param tokens: The `Tokens` object to use for decoding
+    :param lang: The language used in ``string`` (defaults to English, ``en``)
+    :param mode: The form of token representation to use for output (defaults to ``display``)
+    :return: A tuple of a string of token representations and a minimum `OsVersion`
+    """
+
     tokens = tokens or TI_84PCE.tokens
 
     out = []
     since = OsVersions.INITIAL
 
     index = 0
     curr_bytes = b''
@@ -39,47 +53,8 @@
             raise ValueError(f"unexpected null byte at position {index}")
 
         index += 1
 
     return b''.join(out) if mode == "ti_ascii" else "".join(out), since
 
 
-def encode(string: str, trie: TokenTrie) -> tuple[bytes, OsVersion]:
-    data = b''
-    since = OsVersions.INITIAL
-    index = 0
-
-    while string:
-        token, remainder = trie.get_longest_token(string)
-
-        if token is None:
-            raise ValueError(f"could not tokenize input at position {index}: '{string[:12]}'")
-
-        data += token.bits
-        since = max(token.since, since)
-
-        index += len(string) - len(remainder)
-        string = remainder
-
-    return data, since
-
-
-class TokenizedString(String):
-    """
-    Converter for data sections best interpreted as strings of tokens
-
-    Tokenization uses the TI-84+CE token sheet, which is backwards compatible for all var name tokens.
-    """
-
-    _T = str
-
-    @classmethod
-    def get(cls, data: bytes, **kwargs) -> _T:
-        return decode(data.ljust(8, b'\x00'))[0]
-
-    @classmethod
-    def set(cls, value: _T, **kwargs) -> bytes:
-        return encode(value, TI_84PCE.get_trie())[0].rstrip(b'\x00')
-
-
-__all__ = ["decode", "encode", "TokenizedString",
-           "Tokens", "OsVersion", "OsVersions"]
+__all__ = ["decode"]
```

### Comparing `tivars-0.9.0/tivars/tokens/73.xml` & `tivars-0.9.1/tivars/tokens/73.xml`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/tokens/8X.xml` & `tivars-0.9.1/tivars/tokens/8X.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -12914,2297 +12914,2298 @@
 00032710: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
 00032720: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
 00032730: 6969 3d22 3435 3738 3635 3633 3443 3639  ii="457865634C69
 00032740: 3632 3230 223e 0d0a 0909 0909 093c 6469  6220">.......<di
 00032750: 7370 6c61 793e 4578 6563 4c69 6226 2330  splay>ExecLib&#0
 00032760: 3332 3b3c 2f64 6973 706c 6179 3e0d 0a09  32;</display>...
 00032770: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-00032780: 4578 6563 4c69 623c 2f61 6363 6573 7369  ExecLib</accessi
-00032790: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
-000327a0: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-000327b0: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-000327c0: 3c74 6f6b 656e 2076 616c 7565 3d22 2431  <token value="$1
-000327d0: 3322 3e0d 0a09 0909 3c76 6572 7369 6f6e  3">.....<version
-000327e0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-000327f0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00032800: 342b 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  4+</model>......
-00032810: 093c 6f73 2d76 6572 7369 6f6e 3e32 2e33  .<os-version>2.3
-00032820: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
-00032830: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
-00032840: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
-00032850: 2220 7469 2d61 7363 6969 3d22 3639 3645  " ti-ascii="696E
-00032860: 3736 3534 3238 223e 0d0a 0909 0909 093c  765428">.......<
-00032870: 6469 7370 6c61 793e 696e 7654 283c 2f64  display>invT(</d
-00032880: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
-00032890: 6363 6573 7369 626c 653e 696e 7654 283c  ccessible>invT(<
-000328a0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-000328b0: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-000328c0: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-000328d0: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-000328e0: 616c 7565 3d22 2431 3422 3e0d 0a09 0909  alue="$14">.....
-000328f0: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00032900: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-00032910: 6465 6c3e 5449 2d38 342b 3c2f 6d6f 6465  del>TI-84+</mode
-00032920: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
-00032930: 7369 6f6e 3e32 2e33 303c 2f6f 732d 7665  sion>2.30</os-ve
-00032940: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00032950: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00032960: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00032970: 6969 3d22 4439 3132 3437 3446 3436 3244  ii="D912474F462D
-00032980: 3534 3635 3733 3734 3238 223e 0d0a 0909  5465737428">....
-00032990: 0909 093c 6469 7370 6c61 793e cf87 c2b2  ...<display>....
-000329a0: 474f 462d 5465 7374 283c 2f64 6973 706c  GOF-Test(</displ
-000329b0: 6179 3e0d 0a09 0909 0909 3c61 6363 6573  ay>.......<acces
-000329c0: 7369 626c 653e 6368 695e 3247 4f46 2d54  sible>chi^2GOF-T
-000329d0: 6573 7428 3c2f 6163 6365 7373 6962 6c65  est(</accessible
-000329e0: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
-000329f0: 3ecf 875e 3247 4f46 2d54 6573 7428 3c2f  >..^2GOF-Test(</
-00032a00: 7661 7269 616e 743e 0d0a 0909 0909 093c  variant>.......<
-00032a10: 7661 7269 616e 743e 6368 69c2 b247 4f46  variant>chi..GOF
-00032a20: 2d54 6573 7428 3c2f 7661 7269 616e 743e  -Test(</variant>
-00032a30: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
-00032a40: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
-00032a50: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
-00032a60: 656e 2076 616c 7565 3d22 2431 3522 3e0d  en value="$15">.
-00032a70: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
-00032a80: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-00032a90: 093c 6d6f 6465 6c3e 5449 2d38 342b 3c2f  .<model>TI-84+</
-00032aa0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-00032ab0: 2d76 6572 7369 6f6e 3e32 2e33 303c 2f6f  -version>2.30</o
-00032ac0: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
-00032ad0: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
-00032ae0: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
-00032af0: 2d61 7363 6969 3d22 3443 3639 3645 3532  -ascii="4C696E52
-00032b00: 3635 3637 3534 3439 3645 3734 3230 223e  656754496E7420">
-00032b10: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-00032b20: 4c69 6e52 6567 5449 6e74 2623 3033 323b  LinRegTInt&#032;
-00032b30: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-00032b40: 093c 6163 6365 7373 6962 6c65 3e4c 696e  .<accessible>Lin
-00032b50: 5265 6754 496e 7426 2330 3332 3b3c 2f61  RegTInt&#032;</a
-00032b60: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00032b70: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
-00032b80: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
-00032b90: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
-00032ba0: 7565 3d22 2431 3622 3e0d 0a09 0909 3c76  ue="$16">.....<v
-00032bb0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
-00032bc0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
-00032bd0: 6c3e 5449 2d38 342b 3c2f 6d6f 6465 6c3e  l>TI-84+</model>
-00032be0: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
-00032bf0: 6f6e 3e30 2e34 363c 2f6f 732d 7665 7273  on>0.46</os-vers
-00032c00: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
-00032c10: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
-00032c20: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-00032c30: 3d22 3444 3631 3645 3735 3631 3643 3244  ="4D616E75616C2D
-00032c40: 3436 3639 3734 3230 223e 0d0a 0909 0909  46697420">......
-00032c50: 093c 6469 7370 6c61 793e 4d61 6e75 616c  .<display>Manual
-00032c60: 2d46 6974 2623 3033 323b 3c2f 6469 7370  -Fit&#032;</disp
-00032c70: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00032c80: 7373 6962 6c65 3e4d 616e 7561 6c2d 4669  ssible>Manual-Fi
-00032c90: 7426 2330 3332 3b3c 2f61 6363 6573 7369  t&#032;</accessi
-00032ca0: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
-00032cb0: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-00032cc0: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-00032cd0: 3c74 6f6b 656e 2076 616c 7565 3d22 2431  <token value="$1
-00032ce0: 3722 3e0d 0a09 0909 3c76 6572 7369 6f6e  7">.....<version
-00032cf0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-00032d00: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00032d10: 342b 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  4+</model>......
-00032d20: 093c 6f73 2d76 6572 7369 6f6e 3e30 2e30  .<os-version>0.0
-00032d30: 313c 2f6f 732d 7665 7273 696f 6e3e 0d0a  1</os-version>..
-00032d40: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
-00032d50: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
-00032d60: 2220 7469 2d61 7363 6969 3d22 3541 3531  " ti-ascii="5A51
-00032d70: 3735 3631 3634 3732 3631 3645 3734 3331  75616472616E7431
-00032d80: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00032d90: 793e 5a51 7561 6472 616e 7431 3c2f 6469  y>ZQuadrant1</di
-00032da0: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-00032db0: 6365 7373 6962 6c65 3e5a 5175 6164 7261  cessible>ZQuadra
-00032dc0: 6e74 313c 2f61 6363 6573 7369 626c 653e  nt1</accessible>
-00032dd0: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
-00032de0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
-00032df0: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
-00032e00: 656e 2076 616c 7565 3d22 2431 3822 3e0d  en value="$18">.
-00032e10: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
-00032e20: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-00032e30: 093c 6d6f 6465 6c3e 5449 2d38 342b 3c2f  .<model>TI-84+</
-00032e40: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-00032e50: 2d76 6572 7369 6f6e 3e32 2e35 333c 2f6f  -version>2.53</o
-00032e60: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
-00032e70: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
-00032e80: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
-00032e90: 2d61 7363 6969 3d22 3541 3436 3732 3631  -ascii="5A467261
-00032ea0: 3633 3331 4636 3332 223e 0d0a 0909 0909  6331F632">......
-00032eb0: 093c 6469 7370 6c61 793e 5a46 7261 6331  .<display>ZFrac1
-00032ec0: e281 8432 3c2f 6469 7370 6c61 793e 0d0a  ...2</display>..
-00032ed0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-00032ee0: 3e5a 4672 6163 312f 323c 2f61 6363 6573  >ZFrac1/2</acces
-00032ef0: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
-00032f00: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-00032f10: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-00032f20: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-00032f30: 2431 3922 3e0d 0a09 0909 3c76 6572 7369  $19">.....<versi
-00032f40: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-00032f50: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-00032f60: 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a 0909  -84+</model>....
-00032f70: 0909 093c 6f73 2d76 6572 7369 6f6e 3e32  ...<os-version>2
-00032f80: 2e35 333c 2f6f 732d 7665 7273 696f 6e3e  .53</os-version>
-00032f90: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-00032fa0: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-00032fb0: 656e 2220 7469 2d61 7363 6969 3d22 3541  en" ti-ascii="5A
-00032fc0: 3436 3732 3631 3633 3331 4636 3333 223e  4672616331F633">
-00032fd0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-00032fe0: 5a46 7261 6331 e281 8433 3c2f 6469 7370  ZFrac1...3</disp
-00032ff0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00033000: 7373 6962 6c65 3e5a 4672 6163 312f 333c  ssible>ZFrac1/3<
-00033010: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00033020: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00033030: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-00033040: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-00033050: 616c 7565 3d22 2431 4122 3e0d 0a09 0909  alue="$1A">.....
-00033060: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00033070: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-00033080: 6465 6c3e 5449 2d38 342b 3c2f 6d6f 6465  del>TI-84+</mode
-00033090: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
-000330a0: 7369 6f6e 3e32 2e35 333c 2f6f 732d 7665  sion>2.53</os-ve
-000330b0: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-000330c0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-000330d0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-000330e0: 6969 3d22 3541 3436 3732 3631 3633 3331  ii="5A4672616331
-000330f0: 4636 3334 223e 0d0a 0909 0909 093c 6469  F634">.......<di
-00033100: 7370 6c61 793e 5a46 7261 6331 e281 8434  splay>ZFrac1...4
-00033110: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-00033120: 093c 6163 6365 7373 6962 6c65 3e5a 4672  .<accessible>ZFr
-00033130: 6163 312f 343c 2f61 6363 6573 7369 626c  ac1/4</accessibl
-00033140: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
-00033150: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
-00033160: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
-00033170: 6f6b 656e 2076 616c 7565 3d22 2431 4222  oken value="$1B"
-00033180: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
-00033190: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
-000331a0: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
-000331b0: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
-000331c0: 6f73 2d76 6572 7369 6f6e 3e32 2e35 333c  os-version>2.53<
-000331d0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-000331e0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
-000331f0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-00033200: 7469 2d61 7363 6969 3d22 3541 3436 3732  ti-ascii="5A4672
-00033210: 3631 3633 3331 4636 3335 223e 0d0a 0909  616331F635">....
-00033220: 0909 093c 6469 7370 6c61 793e 5a46 7261  ...<display>ZFra
-00033230: 6331 e281 8435 3c2f 6469 7370 6c61 793e  c1...5</display>
-00033240: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00033250: 6c65 3e5a 4672 6163 312f 353c 2f61 6363  le>ZFrac1/5</acc
-00033260: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
-00033270: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00033280: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00033290: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-000332a0: 3d22 2431 4322 3e0d 0a09 0909 3c76 6572  ="$1C">.....<ver
-000332b0: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-000332c0: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-000332d0: 5449 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a  TI-84+</model>..
-000332e0: 0909 0909 093c 6f73 2d76 6572 7369 6f6e  .....<os-version
-000332f0: 3e32 2e35 333c 2f6f 732d 7665 7273 696f  >2.53</os-versio
-00033300: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-00033310: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-00033320: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-00033330: 3541 3436 3732 3631 3633 3331 4636 3338  5A4672616331F638
-00033340: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00033350: 793e 5a46 7261 6331 e281 8438 3c2f 6469  y>ZFrac1...8</di
-00033360: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-00033370: 6365 7373 6962 6c65 3e5a 4672 6163 312f  cessible>ZFrac1/
-00033380: 383c 2f61 6363 6573 7369 626c 653e 0d0a  8</accessible>..
-00033390: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
-000333a0: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
-000333b0: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
-000333c0: 2076 616c 7565 3d22 2431 4422 3e0d 0a09   value="$1D">...
-000333d0: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
-000333e0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
-000333f0: 6d6f 6465 6c3e 5449 2d38 342b 3c2f 6d6f  model>TI-84+</mo
-00033400: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
-00033410: 6572 7369 6f6e 3e32 2e35 333c 2f6f 732d  ersion>2.53</os-
-00033420: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-00033430: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
-00033440: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00033450: 7363 6969 3d22 3541 3436 3732 3631 3633  scii="5A46726163
-00033460: 3331 4636 3331 3330 223e 0d0a 0909 0909  31F63130">......
-00033470: 093c 6469 7370 6c61 793e 5a46 7261 6331  .<display>ZFrac1
-00033480: e281 8431 303c 2f64 6973 706c 6179 3e0d  ...10</display>.
-00033490: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-000334a0: 653e 5a46 7261 6331 2f31 303c 2f61 6363  e>ZFrac1/10</acc
-000334b0: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
-000334c0: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-000334d0: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-000334e0: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-000334f0: 3d22 2431 4522 3e0d 0a09 0909 3c76 6572  ="$1E">.....<ver
-00033500: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00033510: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00033520: 5449 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a  TI-84+</model>..
-00033530: 0909 0909 093c 6f73 2d76 6572 7369 6f6e  .....<os-version
-00033540: 3e32 2e35 333c 2f6f 732d 7665 7273 696f  >2.53</os-versio
-00033550: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-00033560: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-00033570: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-00033580: 4637 223e 0d0a 0909 0909 093c 6469 7370  F7">.......<disp
-00033590: 6c61 793e 2e3c 2f64 6973 706c 6179 3e0d  lay>.</display>.
-000335a0: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-000335b0: 653e 6d61 7468 7072 696e 7462 6f78 3c2f  e>mathprintbox</
-000335c0: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
-000335d0: 0909 3c76 6172 6961 6e74 3ee2 ac9a 3c2f  ..<variant>...</
-000335e0: 7661 7269 616e 743e 0d0a 0909 0909 3c2f  variant>......</
-000335f0: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00033600: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00033610: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00033620: 3d22 2432 4522 3e0d 0a09 0909 3c76 6572  ="$2E">.....<ver
-00033630: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00033640: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00033650: 5449 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a  TI-84+</model>..
-00033660: 0909 0909 093c 6f73 2d76 6572 7369 6f6e  .....<os-version
-00033670: 3e32 2e35 333c 2f6f 732d 7665 7273 696f  >2.53</os-versio
-00033680: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-00033690: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-000336a0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-000336b0: 4636 223e 0d0a 0909 0909 093c 6469 7370  F6">.......<disp
-000336c0: 6c61 793e e281 843c 2f64 6973 706c 6179  lay>...</display
-000336d0: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
-000336e0: 626c 653e 6e2f 643c 2f61 6363 6573 7369  ble>n/d</accessi
-000336f0: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
-00033700: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-00033710: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-00033720: 3c74 6f6b 656e 2076 616c 7565 3d22 2432  <token value="$2
-00033730: 4622 3e0d 0a09 0909 3c76 6572 7369 6f6e  F">.....<version
-00033740: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-00033750: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00033760: 342b 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  4+</model>......
-00033770: 093c 6f73 2d76 6572 7369 6f6e 3e32 2e35  .<os-version>2.5
-00033780: 333c 2f6f 732d 7665 7273 696f 6e3e 0d0a  3</os-version>..
-00033790: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
-000337a0: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
-000337b0: 2220 7469 2d61 7363 6969 3d22 4635 223e  " ti-ascii="F5">
-000337c0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-000337d0: f3b8 8fb5 3c2f 6469 7370 6c61 793e 0d0a  ....</display>..
-000337e0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-000337f0: 3e55 6e2f 643c 2f61 6363 6573 7369 626c  >Un/d</accessibl
-00033800: 653e 0d0a 0909 0909 093c 7661 7269 616e  e>.......<varian
-00033810: 743e e1b5 a43c 2f76 6172 6961 6e74 3e0d  t>...</variant>.
-00033820: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
-00033830: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
-00033840: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
-00033850: 6e20 7661 6c75 653d 2224 3330 223e 0d0a  n value="$30">..
-00033860: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
-00033870: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
-00033880: 3c6d 6f64 656c 3e54 492d 3834 2b3c 2f6d  <model>TI-84+</m
-00033890: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-000338a0: 7665 7273 696f 6e3e 322e 3533 3c2f 6f73  version>2.53</os
-000338b0: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
-000338c0: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
-000338d0: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
-000338e0: 6173 6369 693d 2230 3536 4546 3636 3443  ascii="056EF664C
-000338f0: 4630 3535 3536 4546 3636 3422 3e0d 0a09  F05556EF664">...
-00033900: 0909 0909 3c64 6973 706c 6179 3ee2 96ba  ....<display>...
-00033910: 6ee2 8184 64e2 9784 e296 ba55 6ee2 8184  n...d......Un...
-00033920: 643c 2f64 6973 706c 6179 3e0d 0a09 0909  d</display>.....
-00033930: 0909 3c61 6363 6573 7369 626c 653e 2667  ..<accessible>&g
-00033940: 743b 6e2f 6426 6c74 3b26 6774 3b55 6e2f  t;n/d&lt;&gt;Un/
-00033950: 643c 2f61 6363 6573 7369 626c 653e 0d0a  d</accessible>..
-00033960: 0909 0909 093c 7661 7269 616e 743e e296  .....<variant>..
-00033970: ba6e 2f64 e297 84e2 96ba 556e 2f64 3c2f  .n/d......Un/d</
-00033980: 7661 7269 616e 743e 0d0a 0909 0909 093c  variant>.......<
-00033990: 7661 7269 616e 743e 2667 743b 6ee2 8184  variant>&gt;n...
-000339a0: 6426 6c74 3b26 6774 3b55 6ee2 8184 643c  d&lt;&gt;Un...d<
-000339b0: 2f76 6172 6961 6e74 3e0d 0a09 0909 093c  /variant>......<
-000339c0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-000339d0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-000339e0: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-000339f0: 653d 2224 3331 223e 0d0a 0909 093c 7665  e="$31">.....<ve
-00033a00: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00033a10: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00033a20: 3e54 492d 3834 2b3c 2f6d 6f64 656c 3e0d  >TI-84+</model>.
-00033a30: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-00033a40: 6e3e 322e 3533 3c2f 6f73 2d76 6572 7369  n>2.53</os-versi
-00033a50: 6f6e 3e0d 0a09 0909 093c 2f73 696e 6365  on>......</since
-00033a60: 3e0d 0a09 0909 093c 6c61 6e67 2063 6f64  >......<lang cod
-00033a70: 653d 2265 6e22 2074 692d 6173 6369 693d  e="en" ti-ascii=
-00033a80: 2230 3534 3643 4630 3534 3422 3e0d 0a09  "0546CF0544">...
-00033a90: 0909 0909 3c64 6973 706c 6179 3ee2 96ba  ....<display>...
-00033aa0: 46e2 9784 e296 ba44 3c2f 6469 7370 6c61  F......D</displa
-00033ab0: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
-00033ac0: 6962 6c65 3e26 6774 3b46 266c 743b 2667  ible>&gt;F&lt;&g
-00033ad0: 743b 443c 2f61 6363 6573 7369 626c 653e  t;D</accessible>
-00033ae0: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
-00033af0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
-00033b00: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
-00033b10: 656e 2076 616c 7565 3d22 2433 3222 3e0d  en value="$32">.
-00033b20: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
-00033b30: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-00033b40: 093c 6d6f 6465 6c3e 5449 2d38 342b 3c2f  .<model>TI-84+</
-00033b50: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-00033b60: 2d76 6572 7369 6f6e 3e32 2e35 333c 2f6f  -version>2.53</o
-00033b70: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
-00033b80: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
-00033b90: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
-00033ba0: 2d61 7363 6969 3d22 3732 3635 3644 3631  -ascii="72656D61
-00033bb0: 3639 3645 3634 3635 3732 3238 223e 0d0a  696E64657228">..
-00033bc0: 0909 0909 093c 6469 7370 6c61 793e 7265  .....<display>re
-00033bd0: 6d61 696e 6465 7228 3c2f 6469 7370 6c61  mainder(</displa
-00033be0: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
-00033bf0: 6962 6c65 3e72 656d 6169 6e64 6572 283c  ible>remainder(<
-00033c00: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00033c10: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00033c20: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-00033c30: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-00033c40: 616c 7565 3d22 2433 3322 3e0d 0a09 0909  alue="$33">.....
-00033c50: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00033c60: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-00033c70: 6465 6c3e 5449 2d38 342b 3c2f 6d6f 6465  del>TI-84+</mode
-00033c80: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
-00033c90: 7369 6f6e 3e32 2e35 333c 2f6f 732d 7665  sion>2.53</os-ve
-00033ca0: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00033cb0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00033cc0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00033cd0: 6969 3d22 4336 3238 223e 0d0a 0909 0909  ii="C628">......
-00033ce0: 093c 6469 7370 6c61 793e cea3 283c 2f64  .<display>..(</d
-00033cf0: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
-00033d00: 6363 6573 7369 626c 653e 5369 676d 6128  ccessible>Sigma(
-00033d10: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
-00033d20: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
-00033d30: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
-00033d40: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
-00033d50: 7661 6c75 653d 2224 3334 223e 0d0a 0909  value="$34">....
-00033d60: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
-00033d70: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
-00033d80: 6f64 656c 3e54 492d 3834 2b3c 2f6d 6f64  odel>TI-84+</mod
-00033d90: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
-00033da0: 7273 696f 6e3e 322e 3533 3c2f 6f73 2d76  rsion>2.53</os-v
-00033db0: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
-00033dc0: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
-00033dd0: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
-00033de0: 6369 693d 2236 4336 4636 3734 3234 3135  cii="6C6F6742415
-00033df0: 3334 3532 3822 3e0d 0a09 0909 0909 3c64  34528">.......<d
-00033e00: 6973 706c 6179 3e6c 6f67 4241 5345 283c  isplay>logBASE(<
-00033e10: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-00033e20: 3c61 6363 6573 7369 626c 653e 6c6f 6742  <accessible>logB
-00033e30: 4153 4528 3c2f 6163 6365 7373 6962 6c65  ASE(</accessible
-00033e40: 3e0d 0a09 0909 093c 2f6c 616e 673e 0d0a  >......</lang>..
-00033e50: 0909 093c 2f76 6572 7369 6f6e 3e0d 0a09  ...</version>...
-00033e60: 093c 2f74 6f6b 656e 3e0d 0a09 093c 746f  .</token>....<to
-00033e70: 6b65 6e20 7661 6c75 653d 2224 3335 223e  ken value="$35">
-00033e80: 0d0a 0909 093c 7665 7273 696f 6e3e 0d0a  .....<version>..
-00033e90: 0909 0909 3c73 696e 6365 3e0d 0a09 0909  ....<since>.....
-00033ea0: 0909 3c6d 6f64 656c 3e54 492d 3834 2b3c  ..<model>TI-84+<
-00033eb0: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
-00033ec0: 732d 7665 7273 696f 6e3e 322e 3533 3c2f  s-version>2.53</
-00033ed0: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
-00033ee0: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
-00033ef0: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
-00033f00: 692d 6173 6369 693d 2237 3236 3136 4536  i-ascii="72616E6
-00033f10: 3434 3936 4537 3434 4536 4635 3236 3537  4496E744E6F52657
-00033f20: 3032 3822 3e0d 0a09 0909 0909 3c64 6973  028">.......<dis
-00033f30: 706c 6179 3e72 616e 6449 6e74 4e6f 5265  play>randIntNoRe
-00033f40: 7028 3c2f 6469 7370 6c61 793e 0d0a 0909  p(</display>....
-00033f50: 0909 093c 6163 6365 7373 6962 6c65 3e72  ...<accessible>r
-00033f60: 616e 6449 6e74 4e6f 5265 7028 3c2f 6163  andIntNoRep(</ac
-00033f70: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
-00033f80: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-00033f90: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00033fa0: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-00033fb0: 653d 2224 3337 223e 0d0a 0909 093c 7665  e="$37">.....<ve
-00033fc0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00033fd0: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00033fe0: 3e54 492d 3834 2b3c 2f6d 6f64 656c 3e0d  >TI-84+</model>.
-00033ff0: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-00034000: 6e3e 322e 3533 3c2f 6f73 2d76 6572 7369  n>2.53</os-versi
-00034010: 6f6e 3e0d 0a09 0909 093c 2f73 696e 6365  on>......</since
-00034020: 3e0d 0a09 0909 093c 6c61 6e67 2063 6f64  >......<lang cod
-00034030: 653d 2265 6e22 2074 692d 6173 6369 693d  e="en" ti-ascii=
-00034040: 2234 4434 3135 3434 3835 3035 3234 3934  "4D4154485052494
-00034050: 4535 3422 3e0d 0a09 0909 0909 3c64 6973  E54">.......<dis
-00034060: 706c 6179 3e4d 4154 4850 5249 4e54 3c2f  play>MATHPRINT</
-00034070: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
-00034080: 6163 6365 7373 6962 6c65 3e5b 4d41 5448  accessible>[MATH
-00034090: 5052 494e 545d 3c2f 6163 6365 7373 6962  PRINT]</accessib
-000340a0: 6c65 3e0d 0a09 0909 093c 2f6c 616e 673e  le>......</lang>
-000340b0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
-000340c0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
-000340d0: 746f 6b65 6e20 7661 6c75 653d 2224 3338  token value="$38
-000340e0: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
-000340f0: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
-00034100: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
-00034110: 2b3c 2f6d 6f64 656c 3e0d 0a09 0909 0909  +</model>.......
-00034120: 3c6f 732d 7665 7273 696f 6e3e 322e 3533  <os-version>2.53
-00034130: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
-00034140: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
-00034150: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
-00034160: 2074 692d 6173 6369 693d 2234 3334 4334   ti-ascii="434C4
-00034170: 3135 3335 3334 3934 3322 3e0d 0a09 0909  153534943">.....
-00034180: 0909 3c64 6973 706c 6179 3e43 4c41 5353  ..<display>CLASS
-00034190: 4943 3c2f 6469 7370 6c61 793e 0d0a 0909  IC</display>....
-000341a0: 0909 093c 6163 6365 7373 6962 6c65 3e5b  ...<accessible>[
-000341b0: 434c 4153 5349 435d 3c2f 6163 6365 7373  CLASSIC]</access
-000341c0: 6962 6c65 3e0d 0a09 0909 093c 2f6c 616e  ible>......</lan
-000341d0: 673e 0d0a 0909 093c 2f76 6572 7369 6f6e  g>.....</version
-000341e0: 3e0d 0a09 093c 2f74 6f6b 656e 3e0d 0a09  >....</token>...
-000341f0: 093c 746f 6b65 6e20 7661 6c75 653d 2224  .<token value="$
-00034200: 3339 223e 0d0a 0909 093c 7665 7273 696f  39">.....<versio
-00034210: 6e3e 0d0a 0909 0909 3c73 696e 6365 3e0d  n>......<since>.
-00034220: 0a09 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
-00034230: 3834 2b3c 2f6d 6f64 656c 3e0d 0a09 0909  84+</model>.....
-00034240: 0909 3c6f 732d 7665 7273 696f 6e3e 322e  ..<os-version>2.
-00034250: 3533 3c2f 6f73 2d76 6572 7369 6f6e 3e0d  53</os-version>.
-00034260: 0a09 0909 093c 2f73 696e 6365 3e0d 0a09  .....</since>...
-00034270: 0909 093c 6c61 6e67 2063 6f64 653d 2265  ...<lang code="e
-00034280: 6e22 2074 692d 6173 6369 693d 2236 4546  n" ti-ascii="6EF
-00034290: 3636 3422 3e0d 0a09 0909 0909 3c64 6973  664">.......<dis
-000342a0: 706c 6179 3e6e e281 8464 3c2f 6469 7370  play>n...d</disp
-000342b0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-000342c0: 7373 6962 6c65 3e5b 6e2f 645d 3c2f 6163  ssible>[n/d]</ac
-000342d0: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
-000342e0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-000342f0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00034300: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-00034310: 653d 2224 3341 223e 0d0a 0909 093c 7665  e="$3A">.....<ve
-00034320: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00034330: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00034340: 3e54 492d 3834 2b3c 2f6d 6f64 656c 3e0d  >TI-84+</model>.
-00034350: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-00034360: 6e3e 322e 3533 3c2f 6f73 2d76 6572 7369  n>2.53</os-versi
-00034370: 6f6e 3e0d 0a09 0909 093c 2f73 696e 6365  on>......</since
-00034380: 3e0d 0a09 0909 093c 6c61 6e67 2063 6f64  >......<lang cod
-00034390: 653d 2265 6e22 2074 692d 6173 6369 693d  e="en" ti-ascii=
-000343a0: 2235 3536 4546 3636 3422 3e0d 0a09 0909  "556EF664">.....
-000343b0: 0909 3c64 6973 706c 6179 3e55 6ee2 8184  ..<display>Un...
-000343c0: 643c 2f64 6973 706c 6179 3e0d 0a09 0909  d</display>.....
-000343d0: 0909 3c61 6363 6573 7369 626c 653e 5b55  ..<accessible>[U
-000343e0: 6e2f 645d 3c2f 6163 6365 7373 6962 6c65  n/d]</accessible
-000343f0: 3e0d 0a09 0909 093c 2f6c 616e 673e 0d0a  >......</lang>..
-00034400: 0909 093c 2f76 6572 7369 6f6e 3e0d 0a09  ...</version>...
-00034410: 093c 2f74 6f6b 656e 3e0d 0a09 093c 746f  .</token>....<to
-00034420: 6b65 6e20 7661 6c75 653d 2224 3342 223e  ken value="$3B">
-00034430: 0d0a 0909 093c 7665 7273 696f 6e3e 0d0a  .....<version>..
-00034440: 0909 0909 3c73 696e 6365 3e0d 0a09 0909  ....<since>.....
-00034450: 0909 3c6d 6f64 656c 3e54 492d 3834 2b3c  ..<model>TI-84+<
-00034460: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
-00034470: 732d 7665 7273 696f 6e3e 322e 3533 3c2f  s-version>2.53</
-00034480: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
-00034490: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
-000344a0: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
-000344b0: 692d 6173 6369 693d 2234 3135 3535 3434  i-ascii="4155544
-000344c0: 4622 3e0d 0a09 0909 0909 3c64 6973 706c  F">.......<displ
-000344d0: 6179 3e41 5554 4f3c 2f64 6973 706c 6179  ay>AUTO</display
-000344e0: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
-000344f0: 626c 653e 5b41 5554 4f5d 3c2f 6163 6365  ble>[AUTO]</acce
-00034500: 7373 6962 6c65 3e0d 0a09 0909 093c 2f6c  ssible>......</l
-00034510: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
-00034520: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
-00034530: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
-00034540: 2224 3343 223e 0d0a 0909 093c 7665 7273  "$3C">.....<vers
-00034550: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
-00034560: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
-00034570: 492d 3834 2b3c 2f6d 6f64 656c 3e0d 0a09  I-84+</model>...
-00034580: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
-00034590: 322e 3533 3c2f 6f73 2d76 6572 7369 6f6e  2.53</os-version
-000345a0: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
-000345b0: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
-000345c0: 2265 6e22 2074 692d 6173 6369 693d 2234  "en" ti-ascii="4
-000345d0: 3434 3534 3322 3e0d 0a09 0909 0909 3c64  44543">.......<d
-000345e0: 6973 706c 6179 3e44 4543 3c2f 6469 7370  isplay>DEC</disp
-000345f0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00034600: 7373 6962 6c65 3e5b 4445 435d 3c2f 6163  ssible>[DEC]</ac
-00034610: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
-00034620: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-00034630: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00034640: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-00034650: 653d 2224 3344 223e 0d0a 0909 093c 7665  e="$3D">.....<ve
-00034660: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00034670: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00034680: 3e54 492d 3834 2b3c 2f6d 6f64 656c 3e0d  >TI-84+</model>.
-00034690: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-000346a0: 6e3e 322e 3533 3c2f 6f73 2d76 6572 7369  n>2.53</os-versi
-000346b0: 6f6e 3e0d 0a09 0909 093c 2f73 696e 6365  on>......</since
-000346c0: 3e0d 0a09 0909 093c 756e 7469 6c3e 0d0a  >......<until>..
-000346d0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-000346e0: 342b 4353 453c 2f6d 6f64 656c 3e0d 0a09  4+CSE</model>...
-000346f0: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
-00034700: 342e 303c 2f6f 732d 7665 7273 696f 6e3e  4.0</os-version>
-00034710: 0d0a 0909 0909 3c2f 756e 7469 6c3e 0d0a  ......</until>..
-00034720: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-00034730: 656e 2220 7469 2d61 7363 6969 3d22 3436  en" ti-ascii="46
-00034740: 3532 3431 3433 223e 0d0a 0909 0909 093c  524143">.......<
-00034750: 6469 7370 6c61 793e 4652 4143 3c2f 6469  display>FRAC</di
-00034760: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-00034770: 6365 7373 6962 6c65 3e5b 4652 4143 5d3c  cessible>[FRAC]<
-00034780: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00034790: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-000347a0: 7665 7273 696f 6e3e 0d0a 0909 093c 7665  version>.....<ve
-000347b0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-000347c0: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-000347d0: 3e54 492d 3834 2b43 5345 3c2f 6d6f 6465  >TI-84+CSE</mode
-000347e0: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
-000347f0: 7369 6f6e 3e34 2e30 3c2f 6f73 2d76 6572  sion>4.0</os-ver
-00034800: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
-00034810: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
-00034820: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
-00034830: 693d 2234 3635 3234 3134 3332 4434 3135  i="465241432D415
-00034840: 3035 3035 3234 4635 3822 3e0d 0a09 0909  050524F58">.....
-00034850: 0909 3c64 6973 706c 6179 3e46 5241 432d  ..<display>FRAC-
-00034860: 4150 5052 4f58 3c2f 6469 7370 6c61 793e  APPROX</display>
-00034870: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00034880: 6c65 3e5b 4652 4143 2d41 5050 524f 585d  le>[FRAC-APPROX]
-00034890: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
-000348a0: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
-000348b0: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
-000348c0: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
-000348d0: 7661 6c75 653d 2224 3346 223e 0d0a 0909  value="$3F">....
-000348e0: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
-000348f0: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
-00034900: 6f64 656c 3e54 492d 3834 2b3c 2f6d 6f64  odel>TI-84+</mod
-00034910: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
-00034920: 7273 696f 6e3e 322e 3535 3c2f 6f73 2d76  rsion>2.55</os-v
-00034930: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
-00034940: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
-00034950: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
-00034960: 6369 693d 2235 3335 3434 3135 3435 3734  cii="53544154574
-00034970: 3935 4134 3135 3234 3432 3034 4634 4522  95A415244204F4E"
-00034980: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
-00034990: 3e53 5441 5457 495a 4152 4420 4f4e 3c2f  >STATWIZARD ON</
-000349a0: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
-000349b0: 6163 6365 7373 6962 6c65 3e5b 5354 4154  accessible>[STAT
-000349c0: 5749 5a41 5244 204f 4e5d 3c2f 6163 6365  WIZARD ON]</acce
-000349d0: 7373 6962 6c65 3e0d 0a09 0909 093c 2f6c  ssible>......</l
-000349e0: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
-000349f0: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
-00034a00: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
-00034a10: 2224 3430 223e 0d0a 0909 093c 7665 7273  "$40">.....<vers
-00034a20: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
-00034a30: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
-00034a40: 492d 3834 2b3c 2f6d 6f64 656c 3e0d 0a09  I-84+</model>...
-00034a50: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
-00034a60: 322e 3535 3c2f 6f73 2d76 6572 7369 6f6e  2.55</os-version
-00034a70: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
-00034a80: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
-00034a90: 2265 6e22 2074 692d 6173 6369 693d 2235  "en" ti-ascii="5
-00034aa0: 3335 3434 3135 3435 3734 3935 4134 3135  354415457495A415
-00034ab0: 3234 3432 3034 4634 3634 3622 3e0d 0a09  244204F4646">...
-00034ac0: 0909 0909 3c64 6973 706c 6179 3e53 5441  ....<display>STA
-00034ad0: 5457 495a 4152 4420 4f46 463c 2f64 6973  TWIZARD OFF</dis
-00034ae0: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
-00034af0: 6573 7369 626c 653e 5b53 5441 5457 495a  essible>[STATWIZ
-00034b00: 4152 4420 4f46 465d 3c2f 6163 6365 7373  ARD OFF]</access
-00034b10: 6962 6c65 3e0d 0a09 0909 093c 2f6c 616e  ible>......</lan
-00034b20: 673e 0d0a 0909 093c 2f76 6572 7369 6f6e  g>.....</version
-00034b30: 3e0d 0a09 093c 2f74 6f6b 656e 3e0d 0a09  >....</token>...
-00034b40: 093c 746f 6b65 6e20 7661 6c75 653d 2224  .<token value="$
-00034b50: 3431 223e 0d0a 0909 093c 7665 7273 696f  41">.....<versio
-00034b60: 6e3e 0d0a 0909 0909 3c73 696e 6365 3e0d  n>......<since>.
-00034b70: 0a09 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
-00034b80: 3834 2b43 5345 3c2f 6d6f 6465 6c3e 0d0a  84+CSE</model>..
-00034b90: 0909 0909 093c 6f73 2d76 6572 7369 6f6e  .....<os-version
-00034ba0: 3e34 2e30 3c2f 6f73 2d76 6572 7369 6f6e  >4.0</os-version
-00034bb0: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
-00034bc0: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
-00034bd0: 2265 6e22 2074 692d 6173 6369 693d 2234  "en" ti-ascii="4
-00034be0: 3234 4335 3534 3522 3e0d 0a09 0909 0909  24C5545">.......
-00034bf0: 3c64 6973 706c 6179 3e42 4c55 453c 2f64  <display>BLUE</d
-00034c00: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
-00034c10: 6363 6573 7369 626c 653e 424c 5545 3c2f  ccessible>BLUE</
-00034c20: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
-00034c30: 0909 3c76 6172 6961 6e74 3e42 6c75 653c  ..<variant>Blue<
-00034c40: 2f76 6172 6961 6e74 3e0d 0a09 0909 093c  /variant>......<
-00034c50: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-00034c60: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00034c70: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-00034c80: 653d 2224 3432 223e 0d0a 0909 093c 7665  e="$42">.....<ve
-00034c90: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00034ca0: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00034cb0: 3e54 492d 3834 2b43 5345 3c2f 6d6f 6465  >TI-84+CSE</mode
-00034cc0: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
-00034cd0: 7369 6f6e 3e34 2e30 3c2f 6f73 2d76 6572  sion>4.0</os-ver
-00034ce0: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
-00034cf0: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
-00034d00: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
-00034d10: 693d 2235 3234 3534 3422 3e0d 0a09 0909  i="524544">.....
-00034d20: 0909 3c64 6973 706c 6179 3e52 4544 3c2f  ..<display>RED</
-00034d30: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
-00034d40: 6163 6365 7373 6962 6c65 3e52 4544 3c2f  accessible>RED</
-00034d50: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
-00034d60: 0909 3c76 6172 6961 6e74 3e52 6564 3c2f  ..<variant>Red</
-00034d70: 7661 7269 616e 743e 0d0a 0909 0909 3c2f  variant>......</
-00034d80: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00034d90: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00034da0: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00034db0: 3d22 2434 3322 3e0d 0a09 0909 3c76 6572  ="$43">.....<ver
-00034dc0: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00034dd0: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00034de0: 5449 2d38 342b 4353 453c 2f6d 6f64 656c  TI-84+CSE</model
-00034df0: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-00034e00: 696f 6e3e 342e 303c 2f6f 732d 7665 7273  ion>4.0</os-vers
-00034e10: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
-00034e20: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
-00034e30: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-00034e40: 3d22 3432 3443 3431 3433 3442 223e 0d0a  ="424C41434B">..
-00034e50: 0909 0909 093c 6469 7370 6c61 793e 424c  .....<display>BL
-00034e60: 4143 4b3c 2f64 6973 706c 6179 3e0d 0a09  ACK</display>...
-00034e70: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-00034e80: 424c 4143 4b3c 2f61 6363 6573 7369 626c  BLACK</accessibl
-00034e90: 653e 0d0a 0909 0909 093c 7661 7269 616e  e>.......<varian
-00034ea0: 743e 426c 6163 6b3c 2f76 6172 6961 6e74  t>Black</variant
-00034eb0: 3e0d 0a09 0909 093c 2f6c 616e 673e 0d0a  >......</lang>..
-00034ec0: 0909 093c 2f76 6572 7369 6f6e 3e0d 0a09  ...</version>...
-00034ed0: 093c 2f74 6f6b 656e 3e0d 0a09 093c 746f  .</token>....<to
-00034ee0: 6b65 6e20 7661 6c75 653d 2224 3434 223e  ken value="$44">
-00034ef0: 0d0a 0909 093c 7665 7273 696f 6e3e 0d0a  .....<version>..
-00034f00: 0909 0909 3c73 696e 6365 3e0d 0a09 0909  ....<since>.....
-00034f10: 0909 3c6d 6f64 656c 3e54 492d 3834 2b43  ..<model>TI-84+C
-00034f20: 5345 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  SE</model>......
-00034f30: 093c 6f73 2d76 6572 7369 6f6e 3e34 2e30  .<os-version>4.0
-00034f40: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
-00034f50: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
-00034f60: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
-00034f70: 2074 692d 6173 6369 693d 2234 4434 3134   ti-ascii="4D414
-00034f80: 3734 3534 4535 3434 3122 3e0d 0a09 0909  7454E5441">.....
-00034f90: 0909 3c64 6973 706c 6179 3e4d 4147 454e  ..<display>MAGEN
-00034fa0: 5441 3c2f 6469 7370 6c61 793e 0d0a 0909  TA</display>....
-00034fb0: 0909 093c 6163 6365 7373 6962 6c65 3e4d  ...<accessible>M
-00034fc0: 4147 454e 5441 3c2f 6163 6365 7373 6962  AGENTA</accessib
-00034fd0: 6c65 3e0d 0a09 0909 0909 3c76 6172 6961  le>.......<varia
-00034fe0: 6e74 3e4d 6167 656e 7461 3c2f 7661 7269  nt>Magenta</vari
-00034ff0: 616e 743e 0d0a 0909 0909 3c2f 6c61 6e67  ant>......</lang
-00035000: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-00035010: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-00035020: 3c74 6f6b 656e 2076 616c 7565 3d22 2434  <token value="$4
-00035030: 3522 3e0d 0a09 0909 3c76 6572 7369 6f6e  5">.....<version
-00035040: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-00035050: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00035060: 342b 4353 453c 2f6d 6f64 656c 3e0d 0a09  4+CSE</model>...
-00035070: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
-00035080: 342e 303c 2f6f 732d 7665 7273 696f 6e3e  4.0</os-version>
-00035090: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-000350a0: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-000350b0: 656e 2220 7469 2d61 7363 6969 3d22 3437  en" ti-ascii="47
-000350c0: 3532 3435 3435 3445 223e 0d0a 0909 0909  5245454E">......
-000350d0: 093c 6469 7370 6c61 793e 4752 4545 4e3c  .<display>GREEN<
-000350e0: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-000350f0: 3c61 6363 6573 7369 626c 653e 4752 4545  <accessible>GREE
-00035100: 4e3c 2f61 6363 6573 7369 626c 653e 0d0a  N</accessible>..
-00035110: 0909 0909 093c 7661 7269 616e 743e 4772  .....<variant>Gr
-00035120: 6565 6e3c 2f76 6172 6961 6e74 3e0d 0a09  een</variant>...
-00035130: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
-00035140: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
-00035150: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
-00035160: 7661 6c75 653d 2224 3436 223e 0d0a 0909  value="$46">....
-00035170: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
-00035180: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
-00035190: 6f64 656c 3e54 492d 3834 2b43 5345 3c2f  odel>TI-84+CSE</
-000351a0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-000351b0: 2d76 6572 7369 6f6e 3e34 2e30 3c2f 6f73  -version>4.0</os
-000351c0: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
-000351d0: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
-000351e0: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
-000351f0: 6173 6369 693d 2234 4635 3234 3134 4534  ascii="4F52414E4
-00035200: 3734 3522 3e0d 0a09 0909 0909 3c64 6973  745">.......<dis
-00035210: 706c 6179 3e4f 5241 4e47 453c 2f64 6973  play>ORANGE</dis
-00035220: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
-00035230: 6573 7369 626c 653e 4f52 414e 4745 3c2f  essible>ORANGE</
-00035240: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
-00035250: 0909 3c76 6172 6961 6e74 3e4f 7261 6e67  ..<variant>Orang
-00035260: 653c 2f76 6172 6961 6e74 3e0d 0a09 0909  e</variant>.....
-00035270: 093c 2f6c 616e 673e 0d0a 0909 093c 2f76  .</lang>.....</v
-00035280: 6572 7369 6f6e 3e0d 0a09 093c 2f74 6f6b  ersion>....</tok
-00035290: 656e 3e0d 0a09 093c 746f 6b65 6e20 7661  en>....<token va
-000352a0: 6c75 653d 2224 3437 223e 0d0a 0909 093c  lue="$47">.....<
-000352b0: 7665 7273 696f 6e3e 0d0a 0909 0909 3c73  version>......<s
-000352c0: 696e 6365 3e0d 0a09 0909 0909 3c6d 6f64  ince>.......<mod
-000352d0: 656c 3e54 492d 3834 2b43 5345 3c2f 6d6f  el>TI-84+CSE</mo
-000352e0: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
-000352f0: 6572 7369 6f6e 3e34 2e30 3c2f 6f73 2d76  ersion>4.0</os-v
-00035300: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
-00035310: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
-00035320: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
-00035330: 6369 693d 2234 3235 3234 4635 3734 4522  cii="42524F574E"
-00035340: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
-00035350: 3e42 524f 574e 3c2f 6469 7370 6c61 793e  >BROWN</display>
-00035360: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00035370: 6c65 3e42 524f 574e 3c2f 6163 6365 7373  le>BROWN</access
-00035380: 6962 6c65 3e0d 0a09 0909 0909 3c76 6172  ible>.......<var
-00035390: 6961 6e74 3e42 726f 776e 3c2f 7661 7269  iant>Brown</vari
-000353a0: 616e 743e 0d0a 0909 0909 3c2f 6c61 6e67  ant>......</lang
-000353b0: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-000353c0: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-000353d0: 3c74 6f6b 656e 2076 616c 7565 3d22 2434  <token value="$4
-000353e0: 3822 3e0d 0a09 0909 3c76 6572 7369 6f6e  8">.....<version
-000353f0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-00035400: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00035410: 342b 4353 453c 2f6d 6f64 656c 3e0d 0a09  4+CSE</model>...
-00035420: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
-00035430: 342e 303c 2f6f 732d 7665 7273 696f 6e3e  4.0</os-version>
-00035440: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-00035450: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-00035460: 656e 2220 7469 2d61 7363 6969 3d22 3445  en" ti-ascii="4E
-00035470: 3431 3536 3539 223e 0d0a 0909 0909 093c  415659">.......<
-00035480: 6469 7370 6c61 793e 4e41 5659 3c2f 6469  display>NAVY</di
-00035490: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-000354a0: 6365 7373 6962 6c65 3e4e 4156 593c 2f61  cessible>NAVY</a
-000354b0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-000354c0: 093c 7661 7269 616e 743e 4e61 7679 3c2f  .<variant>Navy</
-000354d0: 7661 7269 616e 743e 0d0a 0909 0909 3c2f  variant>......</
-000354e0: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-000354f0: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00035500: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00035510: 3d22 2434 3922 3e0d 0a09 0909 3c76 6572  ="$49">.....<ver
-00035520: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00035530: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00035540: 5449 2d38 342b 4353 453c 2f6d 6f64 656c  TI-84+CSE</model
-00035550: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-00035560: 696f 6e3e 342e 303c 2f6f 732d 7665 7273  ion>4.0</os-vers
-00035570: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
-00035580: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
-00035590: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-000355a0: 3d22 3443 3534 3432 3443 3535 3435 223e  ="4C54424C5545">
-000355b0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-000355c0: 4c54 424c 5545 3c2f 6469 7370 6c61 793e  LTBLUE</display>
-000355d0: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-000355e0: 6c65 3e4c 5442 4c55 453c 2f61 6363 6573  le>LTBLUE</acces
-000355f0: 7369 626c 653e 0d0a 0909 0909 093c 7661  sible>.......<va
-00035600: 7269 616e 743e 4c74 426c 7565 3c2f 7661  riant>LtBlue</va
-00035610: 7269 616e 743e 0d0a 0909 0909 3c2f 6c61  riant>......</la
-00035620: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-00035630: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-00035640: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-00035650: 2434 4122 3e0d 0a09 0909 3c76 6572 7369  $4A">.....<versi
-00035660: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-00035670: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-00035680: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
-00035690: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-000356a0: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
-000356b0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-000356c0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-000356d0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-000356e0: 3539 3435 3443 3443 3446 3537 223e 0d0a  59454C4C4F57">..
-000356f0: 0909 0909 093c 6469 7370 6c61 793e 5945  .....<display>YE
-00035700: 4c4c 4f57 3c2f 6469 7370 6c61 793e 0d0a  LLOW</display>..
-00035710: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-00035720: 3e59 454c 4c4f 573c 2f61 6363 6573 7369  >YELLOW</accessi
-00035730: 626c 653e 0d0a 0909 0909 093c 7661 7269  ble>.......<vari
-00035740: 616e 743e 5965 6c6c 6f77 3c2f 7661 7269  ant>Yellow</vari
-00035750: 616e 743e 0d0a 0909 0909 3c2f 6c61 6e67  ant>......</lang
-00035760: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-00035770: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-00035780: 3c74 6f6b 656e 2076 616c 7565 3d22 2434  <token value="$4
-00035790: 4222 3e0d 0a09 0909 3c76 6572 7369 6f6e  B">.....<version
-000357a0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-000357b0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-000357c0: 342b 4353 453c 2f6d 6f64 656c 3e0d 0a09  4+CSE</model>...
-000357d0: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
-000357e0: 342e 303c 2f6f 732d 7665 7273 696f 6e3e  4.0</os-version>
-000357f0: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-00035800: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-00035810: 656e 2220 7469 2d61 7363 6969 3d22 3537  en" ti-ascii="57
-00035820: 3438 3439 3534 3435 223e 0d0a 0909 0909  48495445">......
-00035830: 093c 6469 7370 6c61 793e 5748 4954 453c  .<display>WHITE<
-00035840: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-00035850: 3c61 6363 6573 7369 626c 653e 5748 4954  <accessible>WHIT
-00035860: 453c 2f61 6363 6573 7369 626c 653e 0d0a  E</accessible>..
-00035870: 0909 0909 093c 7661 7269 616e 743e 5768  .....<variant>Wh
-00035880: 6974 653c 2f76 6172 6961 6e74 3e0d 0a09  ite</variant>...
-00035890: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
-000358a0: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
-000358b0: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
-000358c0: 7661 6c75 653d 2224 3443 223e 0d0a 0909  value="$4C">....
-000358d0: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
-000358e0: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
-000358f0: 6f64 656c 3e54 492d 3834 2b43 5345 3c2f  odel>TI-84+CSE</
-00035900: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-00035910: 2d76 6572 7369 6f6e 3e34 2e30 3c2f 6f73  -version>4.0</os
-00035920: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
-00035930: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
-00035940: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
-00035950: 6173 6369 693d 2234 4335 3434 3735 3234  ascii="4C5447524
-00035960: 3135 3922 3e0d 0a09 0909 0909 3c64 6973  159">.......<dis
-00035970: 706c 6179 3e4c 5447 5241 593c 2f64 6973  play>LTGRAY</dis
-00035980: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
-00035990: 6573 7369 626c 653e 4c54 4752 4159 3c2f  essible>LTGRAY</
-000359a0: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
-000359b0: 0909 3c76 6172 6961 6e74 3e4c 7447 7261  ..<variant>LtGra
-000359c0: 793c 2f76 6172 6961 6e74 3e0d 0a09 0909  y</variant>.....
-000359d0: 0909 3c76 6172 6961 6e74 3e4c 5447 5245  ..<variant>LTGRE
-000359e0: 593c 2f76 6172 6961 6e74 3e0d 0a09 0909  Y</variant>.....
-000359f0: 0909 3c76 6172 6961 6e74 3e4c 7447 7265  ..<variant>LtGre
-00035a00: 793c 2f76 6172 6961 6e74 3e0d 0a09 0909  y</variant>.....
-00035a10: 093c 2f6c 616e 673e 0d0a 0909 093c 2f76  .</lang>.....</v
-00035a20: 6572 7369 6f6e 3e0d 0a09 093c 2f74 6f6b  ersion>....</tok
-00035a30: 656e 3e0d 0a09 093c 746f 6b65 6e20 7661  en>....<token va
-00035a40: 6c75 653d 2224 3444 223e 0d0a 0909 093c  lue="$4D">.....<
-00035a50: 7665 7273 696f 6e3e 0d0a 0909 0909 3c73  version>......<s
-00035a60: 696e 6365 3e0d 0a09 0909 0909 3c6d 6f64  ince>.......<mod
-00035a70: 656c 3e54 492d 3834 2b43 5345 3c2f 6d6f  el>TI-84+CSE</mo
-00035a80: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
-00035a90: 6572 7369 6f6e 3e34 2e30 3c2f 6f73 2d76  ersion>4.0</os-v
-00035aa0: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
-00035ab0: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
-00035ac0: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
-00035ad0: 6369 693d 2234 4434 3534 3434 3735 3234  cii="4D454447524
-00035ae0: 3135 3922 3e0d 0a09 0909 0909 3c64 6973  159">.......<dis
-00035af0: 706c 6179 3e4d 4544 4752 4159 3c2f 6469  play>MEDGRAY</di
-00035b00: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-00035b10: 6365 7373 6962 6c65 3e4d 4544 4752 4159  cessible>MEDGRAY
-00035b20: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
-00035b30: 0909 0909 3c76 6172 6961 6e74 3e4d 6564  ....<variant>Med
-00035b40: 4772 6179 3c2f 7661 7269 616e 743e 0d0a  Gray</variant>..
-00035b50: 0909 0909 093c 7661 7269 616e 743e 4d45  .....<variant>ME
-00035b60: 4447 5245 593c 2f76 6172 6961 6e74 3e0d  DGREY</variant>.
-00035b70: 0a09 0909 0909 3c76 6172 6961 6e74 3e4d  ......<variant>M
-00035b80: 6564 4772 6579 3c2f 7661 7269 616e 743e  edGrey</variant>
-00035b90: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
-00035ba0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
-00035bb0: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
-00035bc0: 656e 2076 616c 7565 3d22 2434 4522 3e0d  en value="$4E">.
-00035bd0: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
-00035be0: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-00035bf0: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
-00035c00: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
-00035c10: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
-00035c20: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-00035c30: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
-00035c40: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-00035c50: 7469 2d61 7363 6969 3d22 3437 3532 3431  ti-ascii="475241
-00035c60: 3539 223e 0d0a 0909 0909 093c 6469 7370  59">.......<disp
-00035c70: 6c61 793e 4752 4159 3c2f 6469 7370 6c61  lay>GRAY</displa
-00035c80: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
-00035c90: 6962 6c65 3e47 5241 593c 2f61 6363 6573  ible>GRAY</acces
-00035ca0: 7369 626c 653e 0d0a 0909 0909 093c 7661  sible>.......<va
-00035cb0: 7269 616e 743e 4772 6179 3c2f 7661 7269  riant>Gray</vari
-00035cc0: 616e 743e 0d0a 0909 0909 093c 7661 7269  ant>.......<vari
-00035cd0: 616e 743e 4752 4559 3c2f 7661 7269 616e  ant>GREY</varian
-00035ce0: 743e 0d0a 0909 0909 093c 7661 7269 616e  t>.......<varian
-00035cf0: 743e 4772 6579 3c2f 7661 7269 616e 743e  t>Grey</variant>
-00035d00: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
-00035d10: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
-00035d20: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
-00035d30: 656e 2076 616c 7565 3d22 2434 4622 3e0d  en value="$4F">.
-00035d40: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
-00035d50: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-00035d60: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
-00035d70: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
-00035d80: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
-00035d90: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-00035da0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
-00035db0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-00035dc0: 7469 2d61 7363 6969 3d22 3434 3431 3532  ti-ascii="444152
-00035dd0: 3442 3437 3532 3431 3539 223e 0d0a 0909  4B47524159">....
-00035de0: 0909 093c 6469 7370 6c61 793e 4441 524b  ...<display>DARK
-00035df0: 4752 4159 3c2f 6469 7370 6c61 793e 0d0a  GRAY</display>..
-00035e00: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-00035e10: 3e44 4152 4b47 5241 593c 2f61 6363 6573  >DARKGRAY</acces
-00035e20: 7369 626c 653e 0d0a 0909 0909 093c 7661  sible>.......<va
-00035e30: 7269 616e 743e 4461 726b 4772 6179 3c2f  riant>DarkGray</
-00035e40: 7661 7269 616e 743e 0d0a 0909 0909 093c  variant>.......<
-00035e50: 7661 7269 616e 743e 4441 524b 4752 4559  variant>DARKGREY
-00035e60: 3c2f 7661 7269 616e 743e 0d0a 0909 0909  </variant>......
-00035e70: 093c 7661 7269 616e 743e 4461 726b 4772  .<variant>DarkGr
-00035e80: 6579 3c2f 7661 7269 616e 743e 0d0a 0909  ey</variant>....
-00035e90: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00035ea0: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-00035eb0: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-00035ec0: 616c 7565 3d22 2435 3022 3e0d 0a09 0909  alue="$50">.....
-00035ed0: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00035ee0: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-00035ef0: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
-00035f00: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00035f10: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
-00035f20: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-00035f30: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
-00035f40: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00035f50: 7363 6969 3d22 3439 3644 3631 3637 3635  scii="496D616765
-00035f60: 3331 223e 0d0a 0909 0909 093c 6469 7370  31">.......<disp
-00035f70: 6c61 793e 496d 6167 6531 3c2f 6469 7370  lay>Image1</disp
-00035f80: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00035f90: 7373 6962 6c65 3e49 6d61 6765 313c 2f61  ssible>Image1</a
-00035fa0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00035fb0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
-00035fc0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
-00035fd0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
-00035fe0: 7565 3d22 2435 3122 3e0d 0a09 0909 3c76  ue="$51">.....<v
-00035ff0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
-00036000: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
-00036010: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
-00036020: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
-00036030: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
-00036040: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00036050: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00036060: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00036070: 6969 3d22 3439 3644 3631 3637 3635 3332  ii="496D61676532
-00036080: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00036090: 793e 496d 6167 6532 3c2f 6469 7370 6c61  y>Image2</displa
-000360a0: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
-000360b0: 6962 6c65 3e49 6d61 6765 323c 2f61 6363  ible>Image2</acc
-000360c0: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
-000360d0: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-000360e0: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-000360f0: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00036100: 3d22 2435 3222 3e0d 0a09 0909 3c76 6572  ="$52">.....<ver
-00036110: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00036120: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00036130: 5449 2d38 342b 4353 453c 2f6d 6f64 656c  TI-84+CSE</model
-00036140: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-00036150: 696f 6e3e 342e 303c 2f6f 732d 7665 7273  ion>4.0</os-vers
-00036160: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
-00036170: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
-00036180: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-00036190: 3d22 3439 3644 3631 3637 3635 3333 223e  ="496D61676533">
-000361a0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-000361b0: 496d 6167 6533 3c2f 6469 7370 6c61 793e  Image3</display>
-000361c0: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-000361d0: 6c65 3e49 6d61 6765 333c 2f61 6363 6573  le>Image3</acces
-000361e0: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
-000361f0: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-00036200: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-00036210: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-00036220: 2435 3322 3e0d 0a09 0909 3c76 6572 7369  $53">.....<versi
-00036230: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-00036240: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-00036250: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
-00036260: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-00036270: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
-00036280: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-00036290: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-000362a0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-000362b0: 3439 3644 3631 3637 3635 3334 223e 0d0a  496D61676534">..
-000362c0: 0909 0909 093c 6469 7370 6c61 793e 496d  .....<display>Im
-000362d0: 6167 6534 3c2f 6469 7370 6c61 793e 0d0a  age4</display>..
-000362e0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-000362f0: 3e49 6d61 6765 343c 2f61 6363 6573 7369  >Image4</accessi
-00036300: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
-00036310: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-00036320: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-00036330: 3c74 6f6b 656e 2076 616c 7565 3d22 2435  <token value="$5
-00036340: 3422 3e0d 0a09 0909 3c76 6572 7369 6f6e  4">.....<version
-00036350: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-00036360: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00036370: 342b 4353 453c 2f6d 6f64 656c 3e0d 0a09  4+CSE</model>...
-00036380: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
-00036390: 342e 303c 2f6f 732d 7665 7273 696f 6e3e  4.0</os-version>
-000363a0: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-000363b0: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-000363c0: 656e 2220 7469 2d61 7363 6969 3d22 3439  en" ti-ascii="49
-000363d0: 3644 3631 3637 3635 3335 223e 0d0a 0909  6D61676535">....
-000363e0: 0909 093c 6469 7370 6c61 793e 496d 6167  ...<display>Imag
-000363f0: 6535 3c2f 6469 7370 6c61 793e 0d0a 0909  e5</display>....
-00036400: 0909 093c 6163 6365 7373 6962 6c65 3e49  ...<accessible>I
-00036410: 6d61 6765 353c 2f61 6363 6573 7369 626c  mage5</accessibl
-00036420: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
-00036430: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
-00036440: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
-00036450: 6f6b 656e 2076 616c 7565 3d22 2435 3522  oken value="$55"
-00036460: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
-00036470: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
-00036480: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
-00036490: 4353 453c 2f6d 6f64 656c 3e0d 0a09 0909  CSE</model>.....
-000364a0: 0909 3c6f 732d 7665 7273 696f 6e3e 342e  ..<os-version>4.
-000364b0: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
-000364c0: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
-000364d0: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
-000364e0: 2220 7469 2d61 7363 6969 3d22 3439 3644  " ti-ascii="496D
-000364f0: 3631 3637 3635 3336 223e 0d0a 0909 0909  61676536">......
-00036500: 093c 6469 7370 6c61 793e 496d 6167 6536  .<display>Image6
-00036510: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-00036520: 093c 6163 6365 7373 6962 6c65 3e49 6d61  .<accessible>Ima
-00036530: 6765 363c 2f61 6363 6573 7369 626c 653e  ge6</accessible>
-00036540: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
-00036550: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
-00036560: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
-00036570: 656e 2076 616c 7565 3d22 2435 3622 3e0d  en value="$56">.
-00036580: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
-00036590: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-000365a0: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
-000365b0: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
-000365c0: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
-000365d0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-000365e0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
-000365f0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-00036600: 7469 2d61 7363 6969 3d22 3439 3644 3631  ti-ascii="496D61
-00036610: 3637 3635 3337 223e 0d0a 0909 0909 093c  676537">.......<
-00036620: 6469 7370 6c61 793e 496d 6167 6537 3c2f  display>Image7</
-00036630: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
-00036640: 6163 6365 7373 6962 6c65 3e49 6d61 6765  accessible>Image
-00036650: 373c 2f61 6363 6573 7369 626c 653e 0d0a  7</accessible>..
-00036660: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
-00036670: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
-00036680: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
-00036690: 2076 616c 7565 3d22 2435 3722 3e0d 0a09   value="$57">...
-000366a0: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
-000366b0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
-000366c0: 6d6f 6465 6c3e 5449 2d38 342b 4353 453c  model>TI-84+CSE<
-000366d0: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
-000366e0: 732d 7665 7273 696f 6e3e 342e 303c 2f6f  s-version>4.0</o
-000366f0: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
-00036700: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
-00036710: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
-00036720: 2d61 7363 6969 3d22 3439 3644 3631 3637  -ascii="496D6167
-00036730: 3635 3338 223e 0d0a 0909 0909 093c 6469  6538">.......<di
-00036740: 7370 6c61 793e 496d 6167 6538 3c2f 6469  splay>Image8</di
-00036750: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-00036760: 6365 7373 6962 6c65 3e49 6d61 6765 383c  cessible>Image8<
-00036770: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00036780: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00036790: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-000367a0: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-000367b0: 616c 7565 3d22 2435 3822 3e0d 0a09 0909  alue="$58">.....
-000367c0: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-000367d0: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-000367e0: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
-000367f0: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00036800: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
-00036810: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-00036820: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
-00036830: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00036840: 7363 6969 3d22 3439 3644 3631 3637 3635  scii="496D616765
-00036850: 3339 223e 0d0a 0909 0909 093c 6469 7370  39">.......<disp
-00036860: 6c61 793e 496d 6167 6539 3c2f 6469 7370  lay>Image9</disp
-00036870: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00036880: 7373 6962 6c65 3e49 6d61 6765 393c 2f61  ssible>Image9</a
-00036890: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-000368a0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
-000368b0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
-000368c0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
-000368d0: 7565 3d22 2435 3922 3e0d 0a09 0909 3c76  ue="$59">.....<v
-000368e0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
-000368f0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
-00036900: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
-00036910: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
-00036920: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
-00036930: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00036940: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00036950: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00036960: 6969 3d22 3439 3644 3631 3637 3635 3330  ii="496D61676530
-00036970: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00036980: 793e 496d 6167 6530 3c2f 6469 7370 6c61  y>Image0</displa
-00036990: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
-000369a0: 6962 6c65 3e49 6d61 6765 303c 2f61 6363  ible>Image0</acc
-000369b0: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
-000369c0: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-000369d0: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-000369e0: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-000369f0: 3d22 2435 4122 3e0d 0a09 0909 3c76 6572  ="$5A">.....<ver
-00036a00: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00036a10: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00036a20: 5449 2d38 342b 4353 453c 2f6d 6f64 656c  TI-84+CSE</model
-00036a30: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-00036a40: 696f 6e3e 342e 303c 2f6f 732d 7665 7273  ion>4.0</os-vers
-00036a50: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
-00036a60: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
-00036a70: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-00036a80: 3d22 3437 3732 3639 3634 3443 3639 3645  ="477269644C696E
-00036a90: 3635 3230 223e 0d0a 0909 0909 093c 6469  6520">.......<di
-00036aa0: 7370 6c61 793e 4772 6964 4c69 6e65 2623  splay>GridLine&#
-00036ab0: 3033 323b 3c2f 6469 7370 6c61 793e 0d0a  032;</display>..
-00036ac0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-00036ad0: 3e47 7269 644c 696e 6526 2330 3332 3b3c  >GridLine&#032;<
-00036ae0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00036af0: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00036b00: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-00036b10: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-00036b20: 616c 7565 3d22 2435 4222 3e0d 0a09 0909  alue="$5B">.....
-00036b30: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00036b40: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-00036b50: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
-00036b60: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00036b70: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
-00036b80: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-00036b90: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
-00036ba0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00036bb0: 7363 6969 3d22 3432 3631 3633 3642 3637  scii="4261636B67
-00036bc0: 3732 3646 3735 3645 3634 3446 3645 3230  726F756E644F6E20
-00036bd0: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00036be0: 793e 4261 636b 6772 6f75 6e64 4f6e 2623  y>BackgroundOn&#
-00036bf0: 3033 323b 3c2f 6469 7370 6c61 793e 0d0a  032;</display>..
-00036c00: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-00036c10: 3e42 6163 6b67 726f 756e 644f 6e26 2330  >BackgroundOn&#0
-00036c20: 3332 3b3c 2f61 6363 6573 7369 626c 653e  32;</accessible>
-00036c30: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
-00036c40: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
-00036c50: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
-00036c60: 656e 2076 616c 7565 3d22 2436 3422 3e0d  en value="$64">.
-00036c70: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
-00036c80: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-00036c90: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
-00036ca0: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
-00036cb0: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
-00036cc0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-00036cd0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
-00036ce0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-00036cf0: 7469 2d61 7363 6969 3d22 3432 3631 3633  ti-ascii="426163
-00036d00: 3642 3637 3732 3646 3735 3645 3634 3446  6B67726F756E644F
-00036d10: 3636 3636 223e 0d0a 0909 0909 093c 6469  6666">.......<di
-00036d20: 7370 6c61 793e 4261 636b 6772 6f75 6e64  splay>Background
-00036d30: 4f66 663c 2f64 6973 706c 6179 3e0d 0a09  Off</display>...
-00036d40: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-00036d50: 4261 636b 6772 6f75 6e64 4f66 663c 2f61  BackgroundOff</a
-00036d60: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00036d70: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
-00036d80: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
-00036d90: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
-00036da0: 7565 3d22 2436 3522 3e0d 0a09 0909 3c76  ue="$65">.....<v
-00036db0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
-00036dc0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
-00036dd0: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
-00036de0: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
-00036df0: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
-00036e00: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00036e10: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00036e20: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00036e30: 6969 3d22 3437 3732 3631 3730 3638 3433  ii="477261706843
-00036e40: 3646 3643 3646 3732 3238 223e 0d0a 0909  6F6C6F7228">....
-00036e50: 0909 093c 6469 7370 6c61 793e 4772 6170  ...<display>Grap
-00036e60: 6843 6f6c 6f72 283c 2f64 6973 706c 6179  hColor(</display
-00036e70: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
-00036e80: 626c 653e 4772 6170 6843 6f6c 6f72 283c  ble>GraphColor(<
-00036e90: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00036ea0: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00036eb0: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-00036ec0: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-00036ed0: 616c 7565 3d22 2436 3622 3e0d 0a09 0909  alue="$66">.....
-00036ee0: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00036ef0: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-00036f00: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
-00036f10: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00036f20: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
-00036f30: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-00036f40: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
-00036f50: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00036f60: 7363 6969 3d22 3531 3735 3639 3633 3642  scii="517569636B
-00036f70: 3530 3643 3646 3734 3236 3436 3639 3734  506C6F7426466974
-00036f80: 3244 3435 3531 223e 0d0a 0909 0909 093c  2D4551">.......<
-00036f90: 6469 7370 6c61 793e 5175 6963 6b50 6c6f  display>QuickPlo
-00036fa0: 7426 616d 703b 4669 742d 4551 3c2f 6469  t&amp;Fit-EQ</di
-00036fb0: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-00036fc0: 6365 7373 6962 6c65 3e51 7569 636b 506c  cessible>QuickPl
-00036fd0: 6f74 2661 6d70 3b46 6974 2d45 513c 2f61  ot&amp;Fit-EQ</a
-00036fe0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00036ff0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
-00037000: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
-00037010: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
-00037020: 7565 3d22 2436 3722 3e0d 0a09 0909 3c76  ue="$67">.....<v
-00037030: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
-00037040: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
-00037050: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
-00037060: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
-00037070: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
-00037080: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00037090: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-000370a0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-000370b0: 6969 3d22 3534 3635 3738 3734 3433 3646  ii="54657874436F
-000370c0: 3643 3646 3732 3238 223e 0d0a 0909 0909  6C6F7228">......
-000370d0: 093c 6469 7370 6c61 793e 5465 7874 436f  .<display>TextCo
-000370e0: 6c6f 7228 3c2f 6469 7370 6c61 793e 0d0a  lor(</display>..
-000370f0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-00037100: 3e54 6578 7443 6f6c 6f72 283c 2f61 6363  >TextColor(</acc
-00037110: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
-00037120: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00037130: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00037140: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00037150: 3d22 2436 3822 3e0d 0a09 0909 3c76 6572  ="$68">.....<ver
-00037160: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00037170: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00037180: 5449 2d38 342b 4353 453c 2f6d 6f64 656c  TI-84+CSE</model
-00037190: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-000371a0: 696f 6e3e 342e 303c 2f6f 732d 7665 7273  ion>4.0</os-vers
-000371b0: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
-000371c0: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
-000371d0: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-000371e0: 3d22 3431 3733 3644 3338 3334 3433 3530  ="41736D38344350
-000371f0: 3732 3637 3644 223e 0d0a 0909 0909 093c  72676D">.......<
-00037200: 6469 7370 6c61 793e 4173 6d38 3443 5072  display>Asm84CPr
-00037210: 676d 3c2f 6469 7370 6c61 793e 0d0a 0909  gm</display>....
-00037220: 0909 093c 6163 6365 7373 6962 6c65 3e41  ...<accessible>A
-00037230: 736d 3834 4350 7267 6d3c 2f61 6363 6573  sm84CPrgm</acces
-00037240: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
-00037250: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-00037260: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-00037270: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-00037280: 2436 4122 3e0d 0a09 0909 3c76 6572 7369  $6A">.....<versi
-00037290: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-000372a0: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-000372b0: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
-000372c0: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-000372d0: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
-000372e0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-000372f0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-00037300: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-00037310: 3434 3635 3734 3635 3633 3734 3431 3733  4465746563744173
-00037320: 3739 3644 3446 3645 223e 0d0a 0909 0909  796D4F6E">......
-00037330: 093c 6469 7370 6c61 793e 4465 7465 6374  .<display>Detect
-00037340: 4173 796d 4f6e 3c2f 6469 7370 6c61 793e  AsymOn</display>
-00037350: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00037360: 6c65 3e44 6574 6563 7441 7379 6d4f 6e3c  le>DetectAsymOn<
-00037370: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00037380: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00037390: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-000373a0: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-000373b0: 616c 7565 3d22 2436 4222 3e0d 0a09 0909  alue="$6B">.....
-000373c0: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-000373d0: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-000373e0: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
-000373f0: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00037400: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
-00037410: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-00037420: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
-00037430: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00037440: 7363 6969 3d22 3434 3635 3734 3635 3633  scii="4465746563
-00037450: 3734 3431 3733 3739 3644 3446 3636 3636  744173796D4F6666
-00037460: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00037470: 793e 4465 7465 6374 4173 796d 4f66 663c  y>DetectAsymOff<
-00037480: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-00037490: 3c61 6363 6573 7369 626c 653e 4465 7465  <accessible>Dete
-000374a0: 6374 4173 796d 4f66 663c 2f61 6363 6573  ctAsymOff</acces
-000374b0: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
-000374c0: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-000374d0: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-000374e0: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-000374f0: 2436 4322 3e0d 0a09 0909 3c76 6572 7369  $6C">.....<versi
-00037500: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-00037510: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-00037520: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
-00037530: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-00037540: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
-00037550: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-00037560: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-00037570: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-00037580: 3432 3646 3732 3634 3635 3732 3433 3646  426F72646572436F
-00037590: 3643 3646 3732 3230 223e 0d0a 0909 0909  6C6F7220">......
-000375a0: 093c 6469 7370 6c61 793e 426f 7264 6572  .<display>Border
-000375b0: 436f 6c6f 7226 2330 3332 3b3c 2f64 6973  Color&#032;</dis
-000375c0: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
-000375d0: 6573 7369 626c 653e 426f 7264 6572 436f  essible>BorderCo
-000375e0: 6c6f 7226 2330 3332 3b3c 2f61 6363 6573  lor&#032;</acces
-000375f0: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
-00037600: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-00037610: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-00037620: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-00037630: 2437 3322 3e0d 0a09 0909 3c76 6572 7369  $73">.....<versi
-00037640: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-00037650: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-00037660: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
-00037670: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-00037680: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
-00037690: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-000376a0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-000376b0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-000376c0: 4639 223e 0d0a 0909 0909 093c 6469 7370  F9">.......<disp
-000376d0: 6c61 793e 2e3c 2f64 6973 706c 6179 3e0d  lay>.</display>.
-000376e0: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-000376f0: 653e 706c 6f74 7469 6e79 646f 743c 2f61  e>plottinydot</a
-00037700: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00037710: 093c 7661 7269 616e 743e c2b7 3c2f 7661  .<variant>..</va
-00037720: 7269 616e 743e 0d0a 0909 0909 3c2f 6c61  riant>......</la
-00037730: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-00037740: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-00037750: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-00037760: 2437 3422 3e0d 0a09 0909 3c76 6572 7369  $74">.....<versi
-00037770: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-00037780: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-00037790: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
-000377a0: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-000377b0: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
-000377c0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
-000377d0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
-000377e0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-000377f0: 3534 3638 3639 3645 223e 0d0a 0909 0909  5468696E">......
-00037800: 093c 6469 7370 6c61 793e 5468 696e 3c2f  .<display>Thin</
-00037810: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
-00037820: 6163 6365 7373 6962 6c65 3e54 6869 6e3c  accessible>Thin<
-00037830: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00037840: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00037850: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-00037860: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-00037870: 616c 7565 3d22 2437 3522 3e0d 0a09 0909  alue="$75">.....
-00037880: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00037890: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-000378a0: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
-000378b0: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-000378c0: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
-000378d0: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-000378e0: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
-000378f0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00037900: 7363 6969 3d22 3434 3646 3734 3244 3534  scii="446F742D54
-00037910: 3638 3639 3645 223e 0d0a 0909 0909 093c  68696E">.......<
-00037920: 6469 7370 6c61 793e 446f 742d 5468 696e  display>Dot-Thin
-00037930: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-00037940: 093c 6163 6365 7373 6962 6c65 3e44 6f74  .<accessible>Dot
-00037950: 2d54 6869 6e3c 2f61 6363 6573 7369 626c  -Thin</accessibl
-00037960: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
-00037970: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
-00037980: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
-00037990: 6f6b 656e 2076 616c 7565 3d22 2437 3922  oken value="$79"
-000379a0: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
-000379b0: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
-000379c0: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
-000379d0: 4345 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  CE</model>......
-000379e0: 093c 6f73 2d76 6572 7369 6f6e 3e35 2e30  .<os-version>5.0
-000379f0: 2e30 3c2f 6f73 2d76 6572 7369 6f6e 3e0d  .0</os-version>.
-00037a00: 0a09 0909 093c 2f73 696e 6365 3e0d 0a09  .....</since>...
-00037a10: 0909 093c 6c61 6e67 2063 6f64 653d 2265  ...<lang code="e
-00037a20: 6e22 2074 692d 6173 6369 693d 2235 3036  n" ti-ascii="506
-00037a30: 4337 3935 3336 4436 4337 3433 3222 3e0d  C79536D6C7432">.
-00037a40: 0a09 0909 0909 3c64 6973 706c 6179 3e50  ......<display>P
-00037a50: 6c79 536d 6c74 323c 2f64 6973 706c 6179  lySmlt2</display
-00037a60: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
-00037a70: 626c 653e 506c 7953 6d6c 7432 3c2f 6163  ble>PlySmlt2</ac
-00037a80: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
-00037a90: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-00037aa0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00037ab0: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-00037ac0: 653d 2224 3741 223e 0d0a 0909 093c 7665  e="$7A">.....<ve
-00037ad0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00037ae0: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00037af0: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
-00037b00: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-00037b10: 696f 6e3e 352e 302e 303c 2f6f 732d 7665  ion>5.0.0</os-ve
-00037b20: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00037b30: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00037b40: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00037b50: 6969 3d22 3431 3733 3644 3338 3334 3433  ii="41736D383443
-00037b60: 3435 3530 3732 3637 3644 223e 0d0a 0909  455072676D">....
-00037b70: 0909 093c 6469 7370 6c61 793e 4173 6d38  ...<display>Asm8
-00037b80: 3443 4550 7267 6d3c 2f64 6973 706c 6179  4CEPrgm</display
-00037b90: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
-00037ba0: 626c 653e 4173 6d38 3443 4550 7267 6d3c  ble>Asm84CEPrgm<
-00037bb0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00037bc0: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
-00037bd0: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
-00037be0: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
-00037bf0: 616c 7565 3d22 2438 3122 3e0d 0a09 0909  alue="$81">.....
-00037c00: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
-00037c10: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
-00037c20: 6465 6c3e 5449 2d38 342b 4345 3c2f 6d6f  del>TI-84+CE</mo
-00037c30: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
-00037c40: 6572 7369 6f6e 3e35 2e31 2e30 3c2f 6f73  ersion>5.1.0</os
-00037c50: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
-00037c60: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
-00037c70: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
-00037c80: 6173 6369 693d 2235 3137 3536 3137 3237  ascii="517561727
-00037c90: 3436 3936 4336 3537 3332 3035 3336 3537  4696C65732053657
-00037ca0: 3437 3436 3936 4536 3743 4522 3e0d 0a09  474696E67CE">...
-00037cb0: 0909 0909 3c64 6973 706c 6179 3e51 7561  ....<display>Qua
-00037cc0: 7274 696c 6573 2053 6574 7469 6e67 e280  rtiles Setting..
-00037cd0: a63c 2f64 6973 706c 6179 3e0d 0a09 0909  .</display>.....
-00037ce0: 0909 3c61 6363 6573 7369 626c 653e 5175  ..<accessible>Qu
-00037cf0: 6172 7469 6c65 7320 5365 7474 696e 672e  artiles Setting.
-00037d00: 2e2e 3c2f 6163 6365 7373 6962 6c65 3e0d  ..</accessible>.
-00037d10: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
-00037d20: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
-00037d30: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
-00037d40: 6e20 7661 6c75 653d 2224 3832 223e 0d0a  n value="$82">..
-00037d50: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
-00037d60: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
-00037d70: 3c6d 6f64 656c 3e54 492d 3834 2b43 453c  <model>TI-84+CE<
-00037d80: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
-00037d90: 732d 7665 7273 696f 6e3e 352e 322e 303c  s-version>5.2.0<
-00037da0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-00037db0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
-00037dc0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-00037dd0: 7469 2d61 7363 6969 3d22 3735 3238 3031  ti-ascii="752801
-00037de0: 3244 3332 3239 223e 0d0a 0909 0909 093c  2D3229">.......<
-00037df0: 6469 7370 6c61 793e 7528 f09d 919b 2d32  display>u(....-2
-00037e00: 293c 2f64 6973 706c 6179 3e0d 0a09 0909  )</display>.....
-00037e10: 0909 3c61 6363 6573 7369 626c 653e 7528  ..<accessible>u(
-00037e20: 6e2d 3229 3c2f 6163 6365 7373 6962 6c65  n-2)</accessible
-00037e30: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
-00037e40: 3e75 28f0 9d92 8f2d 3229 3c2f 7661 7269  >u(....-2)</vari
-00037e50: 616e 743e 0d0a 0909 0909 3c2f 6c61 6e67  ant>......</lang
-00037e60: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-00037e70: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-00037e80: 3c74 6f6b 656e 2076 616c 7565 3d22 2438  <token value="$8
-00037e90: 3322 3e0d 0a09 0909 3c76 6572 7369 6f6e  3">.....<version
-00037ea0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-00037eb0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00037ec0: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
-00037ed0: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
-00037ee0: 2e32 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .2.0</os-version
-00037ef0: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
-00037f00: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
-00037f10: 2265 6e22 2074 692d 6173 6369 693d 2237  "en" ti-ascii="7
-00037f20: 3632 3830 3132 4433 3232 3922 3e0d 0a09  628012D3229">...
-00037f30: 0909 0909 3c64 6973 706c 6179 3e76 28f0  ....<display>v(.
-00037f40: 9d91 9b2d 3229 3c2f 6469 7370 6c61 793e  ...-2)</display>
-00037f50: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00037f60: 6c65 3e76 286e 2d32 293c 2f61 6363 6573  le>v(n-2)</acces
-00037f70: 7369 626c 653e 0d0a 0909 0909 093c 7661  sible>.......<va
-00037f80: 7269 616e 743e 7628 f09d 928f 2d32 293c  riant>v(....-2)<
-00037f90: 2f76 6172 6961 6e74 3e0d 0a09 0909 093c  /variant>......<
-00037fa0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-00037fb0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00037fc0: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-00037fd0: 653d 2224 3834 223e 0d0a 0909 093c 7665  e="$84">.....<ve
-00037fe0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00037ff0: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00038000: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
-00038010: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-00038020: 696f 6e3e 352e 322e 303c 2f6f 732d 7665  ion>5.2.0</os-ve
-00038030: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00038040: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00038050: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00038060: 6969 3d22 3737 3238 3031 3244 3332 3239  ii="7728012D3229
-00038070: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00038080: 793e 7728 f09d 919b 2d32 293c 2f64 6973  y>w(....-2)</dis
-00038090: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
-000380a0: 6573 7369 626c 653e 7728 6e2d 3229 3c2f  essible>w(n-2)</
-000380b0: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
-000380c0: 0909 3c76 6172 6961 6e74 3e77 28f0 9d92  ..<variant>w(...
-000380d0: 8f2d 3229 3c2f 7661 7269 616e 743e 0d0a  .-2)</variant>..
-000380e0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
-000380f0: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
-00038100: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
-00038110: 2076 616c 7565 3d22 2438 3522 3e0d 0a09   value="$85">...
-00038120: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
-00038130: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
-00038140: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
-00038150: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-00038160: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
-00038170: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
-00038180: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
-00038190: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
-000381a0: 692d 6173 6369 693d 2237 3532 3830 3132  i-ascii="7528012
-000381b0: 4433 3132 3922 3e0d 0a09 0909 0909 3c64  D3129">.......<d
-000381c0: 6973 706c 6179 3e75 28f0 9d91 9b2d 3129  isplay>u(....-1)
-000381d0: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-000381e0: 093c 6163 6365 7373 6962 6c65 3e75 286e  .<accessible>u(n
-000381f0: 2d31 293c 2f61 6363 6573 7369 626c 653e  -1)</accessible>
-00038200: 0d0a 0909 0909 093c 7661 7269 616e 743e  .......<variant>
-00038210: 7528 f09d 928f 2d31 293c 2f76 6172 6961  u(....-1)</varia
-00038220: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
-00038230: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
-00038240: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
-00038250: 746f 6b65 6e20 7661 6c75 653d 2224 3836  token value="$86
-00038260: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
-00038270: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
-00038280: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
-00038290: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
-000382a0: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
-000382b0: 322e 303c 2f6f 732d 7665 7273 696f 6e3e  2.0</os-version>
-000382c0: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-000382d0: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-000382e0: 656e 2220 7469 2d61 7363 6969 3d22 3736  en" ti-ascii="76
-000382f0: 3238 3031 3244 3331 3239 223e 0d0a 0909  28012D3129">....
-00038300: 0909 093c 6469 7370 6c61 793e 7628 f09d  ...<display>v(..
-00038310: 919b 2d31 293c 2f64 6973 706c 6179 3e0d  ..-1)</display>.
-00038320: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-00038330: 653e 7628 6e2d 3129 3c2f 6163 6365 7373  e>v(n-1)</access
-00038340: 6962 6c65 3e0d 0a09 0909 0909 3c76 6172  ible>.......<var
-00038350: 6961 6e74 3e76 28f0 9d92 8f2d 3129 3c2f  iant>v(....-1)</
-00038360: 7661 7269 616e 743e 0d0a 0909 0909 3c2f  variant>......</
-00038370: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00038380: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00038390: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-000383a0: 3d22 2438 3722 3e0d 0a09 0909 3c76 6572  ="$87">.....<ver
-000383b0: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-000383c0: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-000383d0: 5449 2d38 342b 4345 3c2f 6d6f 6465 6c3e  TI-84+CE</model>
-000383e0: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
-000383f0: 6f6e 3e35 2e32 2e30 3c2f 6f73 2d76 6572  on>5.2.0</os-ver
-00038400: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
-00038410: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
-00038420: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
-00038430: 693d 2237 3732 3830 3132 4433 3132 3922  i="7728012D3129"
-00038440: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
-00038450: 3e77 28f0 9d91 9b2d 3129 3c2f 6469 7370  >w(....-1)</disp
-00038460: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00038470: 7373 6962 6c65 3e77 286e 2d31 293c 2f61  ssible>w(n-1)</a
-00038480: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00038490: 093c 7661 7269 616e 743e 7728 f09d 928f  .<variant>w(....
-000384a0: 2d31 293c 2f76 6172 6961 6e74 3e0d 0a09  -1)</variant>...
-000384b0: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
-000384c0: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
-000384d0: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
-000384e0: 7661 6c75 653d 2224 3838 223e 0d0a 0909  value="$88">....
-000384f0: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
-00038500: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
-00038510: 6f64 656c 3e54 492d 3834 2b43 453c 2f6d  odel>TI-84+CE</m
-00038520: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00038530: 7665 7273 696f 6e3e 352e 322e 303c 2f6f  version>5.2.0</o
-00038540: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
-00038550: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
-00038560: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
-00038570: 2d61 7363 6969 3d22 3735 3238 3031 3239  -ascii="75280129
-00038580: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00038590: 793e 7528 f09d 919b 293c 2f64 6973 706c  y>u(....)</displ
-000385a0: 6179 3e0d 0a09 0909 0909 3c61 6363 6573  ay>.......<acces
-000385b0: 7369 626c 653e 7528 6e29 3c2f 6163 6365  sible>u(n)</acce
-000385c0: 7373 6962 6c65 3e0d 0a09 0909 0909 3c76  ssible>.......<v
-000385d0: 6172 6961 6e74 3e75 28f0 9d92 8f29 3c2f  ariant>u(....)</
-000385e0: 7661 7269 616e 743e 0d0a 0909 0909 3c2f  variant>......</
-000385f0: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00038600: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00038610: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00038620: 3d22 2438 3922 3e0d 0a09 0909 3c76 6572  ="$89">.....<ver
-00038630: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00038640: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00038650: 5449 2d38 342b 4345 3c2f 6d6f 6465 6c3e  TI-84+CE</model>
-00038660: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
-00038670: 6f6e 3e35 2e32 2e30 3c2f 6f73 2d76 6572  on>5.2.0</os-ver
-00038680: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
-00038690: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
-000386a0: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
-000386b0: 693d 2237 3632 3830 3132 3922 3e0d 0a09  i="76280129">...
-000386c0: 0909 0909 3c64 6973 706c 6179 3e76 28f0  ....<display>v(.
-000386d0: 9d91 9b29 3c2f 6469 7370 6c61 793e 0d0a  ...)</display>..
-000386e0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-000386f0: 3e76 286e 293c 2f61 6363 6573 7369 626c  >v(n)</accessibl
-00038700: 653e 0d0a 0909 0909 093c 7661 7269 616e  e>.......<varian
-00038710: 743e 7628 f09d 928f 293c 2f76 6172 6961  t>v(....)</varia
-00038720: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
-00038730: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
-00038740: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
-00038750: 746f 6b65 6e20 7661 6c75 653d 2224 3841  token value="$8A
-00038760: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
-00038770: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
-00038780: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
-00038790: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
-000387a0: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
-000387b0: 322e 303c 2f6f 732d 7665 7273 696f 6e3e  2.0</os-version>
-000387c0: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-000387d0: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-000387e0: 656e 2220 7469 2d61 7363 6969 3d22 3737  en" ti-ascii="77
-000387f0: 3238 3031 3239 223e 0d0a 0909 0909 093c  280129">.......<
-00038800: 6469 7370 6c61 793e 7728 f09d 919b 293c  display>w(....)<
-00038810: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-00038820: 3c61 6363 6573 7369 626c 653e 7728 6e29  <accessible>w(n)
-00038830: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
-00038840: 0909 0909 3c76 6172 6961 6e74 3e77 28f0  ....<variant>w(.
-00038850: 9d92 8f29 3c2f 7661 7269 616e 743e 0d0a  ...)</variant>..
-00038860: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
-00038870: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
-00038880: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
-00038890: 2076 616c 7565 3d22 2438 4222 3e0d 0a09   value="$8B">...
-000388a0: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
-000388b0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
-000388c0: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
-000388d0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-000388e0: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
-000388f0: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
-00038900: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
-00038910: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
-00038920: 692d 6173 6369 693d 2237 3532 3830 3132  i-ascii="7528012
-00038930: 4233 3132 3922 3e0d 0a09 0909 0909 3c64  B3129">.......<d
-00038940: 6973 706c 6179 3e75 28f0 9d91 9b2b 3129  isplay>u(....+1)
-00038950: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-00038960: 093c 6163 6365 7373 6962 6c65 3e75 286e  .<accessible>u(n
-00038970: 2b31 293c 2f61 6363 6573 7369 626c 653e  +1)</accessible>
-00038980: 0d0a 0909 0909 093c 7661 7269 616e 743e  .......<variant>
-00038990: 7528 f09d 928f 2b31 293c 2f76 6172 6961  u(....+1)</varia
-000389a0: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
-000389b0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
-000389c0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
-000389d0: 746f 6b65 6e20 7661 6c75 653d 2224 3843  token value="$8C
-000389e0: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
-000389f0: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
-00038a00: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
-00038a10: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
-00038a20: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
-00038a30: 322e 303c 2f6f 732d 7665 7273 696f 6e3e  2.0</os-version>
-00038a40: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-00038a50: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-00038a60: 656e 2220 7469 2d61 7363 6969 3d22 3736  en" ti-ascii="76
-00038a70: 3238 3031 3242 3331 3239 223e 0d0a 0909  28012B3129">....
-00038a80: 0909 093c 6469 7370 6c61 793e 7628 f09d  ...<display>v(..
-00038a90: 919b 2b31 293c 2f64 6973 706c 6179 3e0d  ..+1)</display>.
-00038aa0: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-00038ab0: 653e 7628 6e2b 3129 3c2f 6163 6365 7373  e>v(n+1)</access
-00038ac0: 6962 6c65 3e0d 0a09 0909 0909 3c76 6172  ible>.......<var
-00038ad0: 6961 6e74 3e76 28f0 9d92 8f2b 3129 3c2f  iant>v(....+1)</
-00038ae0: 7661 7269 616e 743e 0d0a 0909 0909 3c2f  variant>......</
-00038af0: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00038b00: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00038b10: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00038b20: 3d22 2438 4422 3e0d 0a09 0909 3c76 6572  ="$8D">.....<ver
-00038b30: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00038b40: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00038b50: 5449 2d38 342b 4345 3c2f 6d6f 6465 6c3e  TI-84+CE</model>
-00038b60: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
-00038b70: 6f6e 3e35 2e32 2e30 3c2f 6f73 2d76 6572  on>5.2.0</os-ver
-00038b80: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
-00038b90: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
-00038ba0: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
-00038bb0: 693d 2237 3732 3830 3132 4233 3132 3922  i="7728012B3129"
-00038bc0: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
-00038bd0: 3e77 28f0 9d91 9b2b 3129 3c2f 6469 7370  >w(....+1)</disp
-00038be0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00038bf0: 7373 6962 6c65 3e77 286e 2b31 293c 2f61  ssible>w(n+1)</a
-00038c00: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00038c10: 093c 7661 7269 616e 743e 7728 f09d 928f  .<variant>w(....
-00038c20: 2b31 293c 2f76 6172 6961 6e74 3e0d 0a09  +1)</variant>...
-00038c30: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
-00038c40: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
-00038c50: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
-00038c60: 7661 6c75 653d 2224 3845 223e 0d0a 0909  value="$8E">....
-00038c70: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
-00038c80: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
-00038c90: 6f64 656c 3e54 492d 3834 2b43 453c 2f6d  odel>TI-84+CE</m
-00038ca0: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00038cb0: 7665 7273 696f 6e3e 352e 322e 303c 2f6f  version>5.2.0</o
-00038cc0: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
-00038cd0: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c75  </since>......<u
-00038ce0: 6e74 696c 3e0d 0a09 0909 0909 3c6d 6f64  ntil>.......<mod
-00038cf0: 656c 3e54 492d 3834 2b43 453c 2f6d 6f64  el>TI-84+CE</mod
-00038d00: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
-00038d10: 7273 696f 6e3e 352e 332e 303c 2f6f 732d  rsion>5.3.0</os-
-00038d20: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
-00038d30: 756e 7469 6c3e 0d0a 0909 0909 3c6c 616e  until>......<lan
-00038d40: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-00038d50: 7363 6969 3d22 3730 3639 3635 3633 3635  scii="7069656365
-00038d60: 3537 3639 3733 3635 3238 223e 0d0a 0909  5769736528">....
-00038d70: 0909 093c 6469 7370 6c61 793e 7069 6563  ...<display>piec
-00038d80: 6557 6973 6528 3c2f 6469 7370 6c61 793e  eWise(</display>
-00038d90: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00038da0: 6c65 3e70 6965 6365 5769 7365 283c 2f61  le>pieceWise(</a
-00038db0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-00038dc0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
-00038dd0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
-00038de0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
-00038df0: 7565 3d22 2438 4622 3e0d 0a09 0909 3c76  ue="$8F">.....<v
-00038e00: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
-00038e10: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
-00038e20: 6c3e 5449 2d38 342b 4345 3c2f 6d6f 6465  l>TI-84+CE</mode
-00038e30: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
-00038e40: 7369 6f6e 3e35 2e32 2e30 3c2f 6f73 2d76  sion>5.2.0</os-v
-00038e50: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
-00038e60: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
-00038e70: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
-00038e80: 6369 693d 2235 3334 3535 3132 3830 3132  cii="53455128012
-00038e90: 3922 3e0d 0a09 0909 0909 3c64 6973 706c  9">.......<displ
-00038ea0: 6179 3e53 4551 28f0 9d91 9b29 3c2f 6469  ay>SEQ(....)</di
-00038eb0: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
-00038ec0: 6365 7373 6962 6c65 3e53 4551 286e 293c  cessible>SEQ(n)<
-00038ed0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-00038ee0: 0909 093c 7661 7269 616e 743e 5345 5128  ...<variant>SEQ(
-00038ef0: f09d 928f 293c 2f76 6172 6961 6e74 3e0d  ....)</variant>.
-00038f00: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
-00038f10: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
-00038f20: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
-00038f30: 6e20 7661 6c75 653d 2224 3930 223e 0d0a  n value="$90">..
-00038f40: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
-00038f50: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
-00038f60: 3c6d 6f64 656c 3e54 492d 3834 2b43 453c  <model>TI-84+CE<
-00038f70: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
-00038f80: 732d 7665 7273 696f 6e3e 352e 322e 303c  s-version>5.2.0<
-00038f90: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-00038fa0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
-00038fb0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-00038fc0: 7469 2d61 7363 6969 3d22 3533 3435 3531  ti-ascii="534551
-00038fd0: 3238 3031 3242 3331 3239 223e 0d0a 0909  28012B3129">....
-00038fe0: 0909 093c 6469 7370 6c61 793e 5345 5128  ...<display>SEQ(
-00038ff0: f09d 919b 2b31 293c 2f64 6973 706c 6179  ....+1)</display
-00039000: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
-00039010: 626c 653e 5345 5128 6e2b 3129 3c2f 6163  ble>SEQ(n+1)</ac
-00039020: 6365 7373 6962 6c65 3e0d 0a09 0909 0909  cessible>.......
-00039030: 3c76 6172 6961 6e74 3e53 4551 28f0 9d92  <variant>SEQ(...
-00039040: 8f2b 3129 3c2f 7661 7269 616e 743e 0d0a  .+1)</variant>..
-00039050: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
-00039060: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
-00039070: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
-00039080: 2076 616c 7565 3d22 2439 3122 3e0d 0a09   value="$91">...
-00039090: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
-000390a0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
-000390b0: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
-000390c0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-000390d0: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
-000390e0: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
-000390f0: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
-00039100: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
-00039110: 692d 6173 6369 693d 2235 3334 3535 3132  i-ascii="5345512
-00039120: 3830 3132 4233 3232 3922 3e0d 0a09 0909  8012B3229">.....
-00039130: 0909 3c64 6973 706c 6179 3e53 4551 28f0  ..<display>SEQ(.
-00039140: 9d91 9b2b 3229 3c2f 6469 7370 6c61 793e  ...+2)</display>
-00039150: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00039160: 6c65 3e53 4551 286e 2b32 293c 2f61 6363  le>SEQ(n+2)</acc
-00039170: 6573 7369 626c 653e 0d0a 0909 0909 093c  essible>.......<
-00039180: 7661 7269 616e 743e 5345 5128 f09d 928f  variant>SEQ(....
-00039190: 2b32 293c 2f76 6172 6961 6e74 3e0d 0a09  +2)</variant>...
-000391a0: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
-000391b0: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
-000391c0: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
-000391d0: 7661 6c75 653d 2224 3932 223e 0d0a 0909  value="$92">....
-000391e0: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
-000391f0: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
-00039200: 6f64 656c 3e54 492d 3834 2b43 453c 2f6d  odel>TI-84+CE</m
-00039210: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
-00039220: 7665 7273 696f 6e3e 352e 322e 303c 2f6f  version>5.2.0</o
-00039230: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
-00039240: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
-00039250: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
-00039260: 2d61 7363 6969 3d22 3443 3435 3436 3534  -ascii="4C454654
-00039270: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
-00039280: 793e 4c45 4654 3c2f 6469 7370 6c61 793e  y>LEFT</display>
-00039290: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-000392a0: 6c65 3e4c 4546 543c 2f61 6363 6573 7369  le>LEFT</accessi
-000392b0: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
-000392c0: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-000392d0: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-000392e0: 3c74 6f6b 656e 2076 616c 7565 3d22 2439  <token value="$9
-000392f0: 3322 3e0d 0a09 0909 3c76 6572 7369 6f6e  3">.....<version
-00039300: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-00039310: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-00039320: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
-00039330: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
-00039340: 2e32 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .2.0</os-version
-00039350: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
-00039360: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
-00039370: 2265 6e22 2074 692d 6173 6369 693d 2234  "en" ti-ascii="4
-00039380: 3334 3534 4535 3434 3535 3222 3e0d 0a09  3454E544552">...
-00039390: 0909 0909 3c64 6973 706c 6179 3e43 454e  ....<display>CEN
-000393a0: 5445 523c 2f64 6973 706c 6179 3e0d 0a09  TER</display>...
-000393b0: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-000393c0: 4345 4e54 4552 3c2f 6163 6365 7373 6962  CENTER</accessib
-000393d0: 6c65 3e0d 0a09 0909 093c 2f6c 616e 673e  le>......</lang>
-000393e0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
-000393f0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
-00039400: 746f 6b65 6e20 7661 6c75 653d 2224 3934  token value="$94
-00039410: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
-00039420: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
-00039430: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
-00039440: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
-00039450: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
-00039460: 322e 303c 2f6f 732d 7665 7273 696f 6e3e  2.0</os-version>
-00039470: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-00039480: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-00039490: 656e 2220 7469 2d61 7363 6969 3d22 3532  en" ti-ascii="52
-000394a0: 3439 3437 3438 3534 223e 0d0a 0909 0909  49474854">......
-000394b0: 093c 6469 7370 6c61 793e 5249 4748 543c  .<display>RIGHT<
-000394c0: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-000394d0: 3c61 6363 6573 7369 626c 653e 5249 4748  <accessible>RIGH
-000394e0: 543c 2f61 6363 6573 7369 626c 653e 0d0a  T</accessible>..
-000394f0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
-00039500: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
-00039510: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
-00039520: 2076 616c 7565 3d22 2439 3522 3e0d 0a09   value="$95">...
-00039530: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
-00039540: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
-00039550: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
-00039560: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-00039570: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
-00039580: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
-00039590: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
-000395a0: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
-000395b0: 692d 6173 6369 693d 2236 3936 4537 3634  i-ascii="696E764
-000395c0: 3236 3936 4536 4636 4432 3822 3e0d 0a09  2696E6F6D28">...
-000395d0: 0909 0909 3c64 6973 706c 6179 3e69 6e76  ....<display>inv
-000395e0: 4269 6e6f 6d28 3c2f 6469 7370 6c61 793e  Binom(</display>
-000395f0: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00039600: 6c65 3e69 6e76 4269 6e6f 6d28 3c2f 6163  le>invBinom(</ac
-00039610: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
-00039620: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-00039630: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00039640: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-00039650: 653d 2224 3936 223e 0d0a 0909 093c 7665  e="$96">.....<ve
-00039660: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-00039670: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-00039680: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
-00039690: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-000396a0: 696f 6e3e 352e 322e 303c 2f6f 732d 7665  ion>5.2.0</os-ve
-000396b0: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-000396c0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-000396d0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-000396e0: 6969 3d22 3537 3631 3639 3734 3230 223e  ii="5761697420">
-000396f0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-00039700: 5761 6974 2623 3033 323b 3c2f 6469 7370  Wait&#032;</disp
-00039710: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
-00039720: 7373 6962 6c65 3e57 6169 7426 2330 3332  ssible>Wait&#032
-00039730: 3b3c 2f61 6363 6573 7369 626c 653e 0d0a  ;</accessible>..
-00039740: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
-00039750: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
-00039760: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
-00039770: 2076 616c 7565 3d22 2439 3722 3e0d 0a09   value="$97">...
-00039780: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
-00039790: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
-000397a0: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
-000397b0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
-000397c0: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
-000397d0: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
-000397e0: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
-000397f0: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
-00039800: 692d 6173 6369 693d 2237 3436 4635 3337  i-ascii="746F537
-00039810: 3437 3236 3936 4536 3732 3822 3e0d 0a09  472696E6728">...
-00039820: 0909 0909 3c64 6973 706c 6179 3e74 6f53  ....<display>toS
-00039830: 7472 696e 6728 3c2f 6469 7370 6c61 793e  tring(</display>
-00039840: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00039850: 6c65 3e74 6f53 7472 696e 6728 3c2f 6163  le>toString(</ac
-00039860: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
-00039870: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
-00039880: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
-00039890: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
-000398a0: 653d 2224 3938 223e 0d0a 0909 093c 7665  e="$98">.....<ve
-000398b0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
-000398c0: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
-000398d0: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
-000398e0: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
-000398f0: 696f 6e3e 352e 322e 303c 2f6f 732d 7665  ion>5.2.0</os-ve
-00039900: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
-00039910: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
-00039920: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
-00039930: 6969 3d22 3635 3736 3631 3643 3238 223e  ii="6576616C28">
-00039940: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-00039950: 6576 616c 283c 2f64 6973 706c 6179 3e0d  eval(</display>.
-00039960: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-00039970: 653e 6576 616c 283c 2f61 6363 6573 7369  e>eval(</accessi
-00039980: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
-00039990: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-000399a0: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-000399b0: 3c74 6f6b 656e 2076 616c 7565 3d22 2439  <token value="$9
-000399c0: 4522 3e0d 0a09 0909 3c76 6572 7369 6f6e  E">.....<version
-000399d0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-000399e0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-000399f0: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
-00039a00: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
-00039a10: 2e33 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .3.0</os-version
-00039a20: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
-00039a30: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
-00039a40: 2265 6e22 2074 692d 6173 6369 693d 2234  "en" ti-ascii="4
-00039a50: 3537 3836 3536 3337 3537 3436 3532 3035  5786563757465205
-00039a60: 3037 3236 4636 3737 3236 3136 4422 3e0d  0726F6772616D">.
-00039a70: 0a09 0909 0909 3c64 6973 706c 6179 3e45  ......<display>E
-00039a80: 7865 6375 7465 2050 726f 6772 616d 3c2f  xecute Program</
-00039a90: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
-00039aa0: 6163 6365 7373 6962 6c65 3e45 7865 6375  accessible>Execu
-00039ab0: 7465 2050 726f 6772 616d 3c2f 6163 6365  te Program</acce
-00039ac0: 7373 6962 6c65 3e0d 0a09 0909 093c 2f6c  ssible>......</l
-00039ad0: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
-00039ae0: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
-00039af0: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
-00039b00: 2224 3946 223e 0d0a 0909 093c 7665 7273  "$9F">.....<vers
-00039b10: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
-00039b20: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
-00039b30: 492d 3834 2b43 453c 2f6d 6f64 656c 3e0d  I-84+CE</model>.
-00039b40: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-00039b50: 6e3e 352e 332e 303c 2f6f 732d 7665 7273  n>5.3.0</os-vers
-00039b60: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
-00039b70: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
-00039b80: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-00039b90: 3d22 3535 3645 3634 3646 3230 3433 3643  ="556E646F20436C
-00039ba0: 3635 3631 3732 223e 0d0a 0909 0909 093c  656172">.......<
-00039bb0: 6469 7370 6c61 793e 556e 646f 2043 6c65  display>Undo Cle
-00039bc0: 6172 3c2f 6469 7370 6c61 793e 0d0a 0909  ar</display>....
-00039bd0: 0909 093c 6163 6365 7373 6962 6c65 3e55  ...<accessible>U
-00039be0: 6e64 6f20 436c 6561 723c 2f61 6363 6573  ndo Clear</acces
-00039bf0: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
-00039c00: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
-00039c10: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
-00039c20: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-00039c30: 2441 3022 3e0d 0a09 0909 3c76 6572 7369  $A0">.....<versi
-00039c40: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
-00039c50: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
-00039c60: 2d38 342b 4345 3c2f 6d6f 6465 6c3e 0d0a  -84+CE</model>..
-00039c70: 0909 0909 093c 6f73 2d76 6572 7369 6f6e  .....<os-version
-00039c80: 3e35 2e33 2e30 3c2f 6f73 2d76 6572 7369  >5.3.0</os-versi
-00039c90: 6f6e 3e0d 0a09 0909 093c 2f73 696e 6365  on>......</since
-00039ca0: 3e0d 0a09 0909 093c 6c61 6e67 2063 6f64  >......<lang cod
-00039cb0: 653d 2265 6e22 2074 692d 6173 6369 693d  e="en" ti-ascii=
-00039cc0: 2234 3936 4537 3336 3537 3237 3432 3034  "496E73657274204
-00039cd0: 4336 3936 4536 3532 3034 3136 3236 4637  C696E652041626F7
-00039ce0: 3636 3522 3e0d 0a09 0909 0909 3c64 6973  665">.......<dis
-00039cf0: 706c 6179 3e49 6e73 6572 7420 4c69 6e65  play>Insert Line
-00039d00: 2041 626f 7665 3c2f 6469 7370 6c61 793e   Above</display>
-00039d10: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00039d20: 6c65 3e49 6e73 6572 7420 4c69 6e65 2041  le>Insert Line A
-00039d30: 626f 7665 3c2f 6163 6365 7373 6962 6c65  bove</accessible
-00039d40: 3e0d 0a09 0909 093c 2f6c 616e 673e 0d0a  >......</lang>..
-00039d50: 0909 093c 2f76 6572 7369 6f6e 3e0d 0a09  ...</version>...
-00039d60: 093c 2f74 6f6b 656e 3e0d 0a09 093c 746f  .</token>....<to
-00039d70: 6b65 6e20 7661 6c75 653d 2224 4131 223e  ken value="$A1">
-00039d80: 0d0a 0909 093c 7665 7273 696f 6e3e 0d0a  .....<version>..
-00039d90: 0909 0909 3c73 696e 6365 3e0d 0a09 0909  ....<since>.....
-00039da0: 0909 3c6d 6f64 656c 3e54 492d 3834 2b43  ..<model>TI-84+C
-00039db0: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
-00039dc0: 3c6f 732d 7665 7273 696f 6e3e 352e 332e  <os-version>5.3.
-00039dd0: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
-00039de0: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
-00039df0: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
-00039e00: 2220 7469 2d61 7363 6969 3d22 3433 3735  " ti-ascii="4375
-00039e10: 3734 3230 3443 3639 3645 3635 223e 0d0a  74204C696E65">..
-00039e20: 0909 0909 093c 6469 7370 6c61 793e 4375  .....<display>Cu
-00039e30: 7420 4c69 6e65 3c2f 6469 7370 6c61 793e  t Line</display>
-00039e40: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
-00039e50: 6c65 3e43 7574 204c 696e 653c 2f61 6363  le>Cut Line</acc
-00039e60: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
-00039e70: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
-00039e80: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
-00039e90: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
-00039ea0: 3d22 2441 3222 3e0d 0a09 0909 3c76 6572  ="$A2">.....<ver
-00039eb0: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
-00039ec0: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
-00039ed0: 5449 2d38 342b 4345 3c2f 6d6f 6465 6c3e  TI-84+CE</model>
-00039ee0: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
-00039ef0: 6f6e 3e35 2e33 2e30 3c2f 6f73 2d76 6572  on>5.3.0</os-ver
-00039f00: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
-00039f10: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
-00039f20: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
-00039f30: 693d 2234 3336 4637 3037 3932 3034 4336  i="436F7079204C6
-00039f40: 3936 4536 3522 3e0d 0a09 0909 0909 3c64  96E65">.......<d
-00039f50: 6973 706c 6179 3e43 6f70 7920 4c69 6e65  isplay>Copy Line
-00039f60: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-00039f70: 093c 6163 6365 7373 6962 6c65 3e43 6f70  .<accessible>Cop
-00039f80: 7920 4c69 6e65 3c2f 6163 6365 7373 6962  y Line</accessib
-00039f90: 6c65 3e0d 0a09 0909 093c 2f6c 616e 673e  le>......</lang>
-00039fa0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
-00039fb0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
-00039fc0: 746f 6b65 6e20 7661 6c75 653d 2224 4133  token value="$A3
-00039fd0: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
-00039fe0: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
-00039ff0: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
-0003a000: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
-0003a010: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
-0003a020: 332e 303c 2f6f 732d 7665 7273 696f 6e3e  3.0</os-version>
-0003a030: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
-0003a040: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-0003a050: 656e 2220 7469 2d61 7363 6969 3d22 3530  en" ti-ascii="50
-0003a060: 3631 3733 3734 3635 3230 3443 3639 3645  61737465204C696E
-0003a070: 3635 3230 3432 3635 3643 3646 3737 223e  652042656C6F77">
-0003a080: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
-0003a090: 5061 7374 6520 4c69 6e65 2042 656c 6f77  Paste Line Below
-0003a0a0: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-0003a0b0: 093c 6163 6365 7373 6962 6c65 3e50 6173  .<accessible>Pas
-0003a0c0: 7465 204c 696e 6520 4265 6c6f 773c 2f61  te Line Below</a
-0003a0d0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
-0003a0e0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
-0003a0f0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
-0003a100: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
-0003a110: 7565 3d22 2441 3422 3e0d 0a09 0909 3c76  ue="$A4">.....<v
-0003a120: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
-0003a130: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
-0003a140: 6c3e 5449 2d38 342b 4345 3c2f 6d6f 6465  l>TI-84+CE</mode
-0003a150: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
-0003a160: 7369 6f6e 3e35 2e33 2e30 3c2f 6f73 2d76  sion>5.3.0</os-v
-0003a170: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
-0003a180: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
-0003a190: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
-0003a1a0: 6369 693d 2234 3936 4537 3336 3537 3237  cii="496E7365727
-0003a1b0: 3432 3034 3336 4636 4436 4436 3536 4537  420436F6D6D656E7
-0003a1c0: 3432 3034 3136 3236 4637 3636 3522 3e0d  42041626F7665">.
-0003a1d0: 0a09 0909 0909 3c64 6973 706c 6179 3e49  ......<display>I
-0003a1e0: 6e73 6572 7420 436f 6d6d 656e 7420 4162  nsert Comment Ab
-0003a1f0: 6f76 653c 2f64 6973 706c 6179 3e0d 0a09  ove</display>...
-0003a200: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-0003a210: 496e 7365 7274 2043 6f6d 6d65 6e74 2041  Insert Comment A
-0003a220: 626f 7665 3c2f 6163 6365 7373 6962 6c65  bove</accessible
-0003a230: 3e0d 0a09 0909 093c 2f6c 616e 673e 0d0a  >......</lang>..
-0003a240: 0909 093c 2f76 6572 7369 6f6e 3e0d 0a09  ...</version>...
-0003a250: 093c 2f74 6f6b 656e 3e0d 0a09 093c 746f  .</token>....<to
-0003a260: 6b65 6e20 7661 6c75 653d 2224 4135 223e  ken value="$A5">
-0003a270: 0d0a 0909 093c 7665 7273 696f 6e3e 0d0a  .....<version>..
-0003a280: 0909 0909 3c73 696e 6365 3e0d 0a09 0909  ....<since>.....
-0003a290: 0909 3c6d 6f64 656c 3e54 492d 3834 2b43  ..<model>TI-84+C
-0003a2a0: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
-0003a2b0: 3c6f 732d 7665 7273 696f 6e3e 352e 332e  <os-version>5.3.
-0003a2c0: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
-0003a2d0: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
-0003a2e0: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
-0003a2f0: 2220 7469 2d61 7363 6969 3d22 3531 3735  " ti-ascii="5175
-0003a300: 3639 3734 3230 3435 3634 3639 3734 3646  697420456469746F
-0003a310: 3732 223e 0d0a 0909 0909 093c 6469 7370  72">.......<disp
-0003a320: 6c61 793e 5175 6974 2045 6469 746f 723c  lay>Quit Editor<
-0003a330: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-0003a340: 3c61 6363 6573 7369 626c 653e 5175 6974  <accessible>Quit
-0003a350: 2045 6469 746f 723c 2f61 6363 6573 7369   Editor</accessi
-0003a360: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
-0003a370: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
-0003a380: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
-0003a390: 3c74 6f6b 656e 2076 616c 7565 3d22 2441  <token value="$A
-0003a3a0: 3622 3e0d 0a09 0909 3c76 6572 7369 6f6e  6">.....<version
-0003a3b0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
-0003a3c0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
-0003a3d0: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
-0003a3e0: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
-0003a3f0: 2e33 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .3.0</os-version
-0003a400: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
-0003a410: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
-0003a420: 2265 6e22 2074 692d 6173 6369 693d 2237  "en" ti-ascii="7
-0003a430: 3036 3936 3536 3336 3537 3736 3937 3336  0696563657769736
-0003a440: 3532 3822 3e0d 0a09 0909 0909 3c64 6973  528">.......<dis
-0003a450: 706c 6179 3e70 6965 6365 7769 7365 283c  play>piecewise(<
-0003a460: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
-0003a470: 3c61 6363 6573 7369 626c 653e 7069 6563  <accessible>piec
-0003a480: 6577 6973 6528 3c2f 6163 6365 7373 6962  ewise(</accessib
-0003a490: 6c65 3e0d 0a09 0909 093c 2f6c 616e 673e  le>......</lang>
-0003a4a0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
-0003a4b0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 3c2f  ...</token>...</
-0003a4c0: 7477 6f2d 6279 7465 3e0d 0a09 3c74 6f6b  two-byte>...<tok
-0003a4d0: 656e 2076 616c 7565 3d22 2446 3022 3e0d  en value="$F0">.
-0003a4e0: 0a09 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
-0003a4f0: 093c 7369 6e63 653e 0d0a 0909 0909 3c6d  .<since>......<m
-0003a500: 6f64 656c 3e54 492d 3832 3c2f 6d6f 6465  odel>TI-82</mode
-0003a510: 6c3e 0d0a 0909 0909 3c6f 732d 7665 7273  l>......<os-vers
-0003a520: 696f 6e3e 312e 303c 2f6f 732d 7665 7273  ion>1.0</os-vers
-0003a530: 696f 6e3e 0d0a 0909 093c 2f73 696e 6365  ion>.....</since
-0003a540: 3e0d 0a09 0909 3c6c 616e 6720 636f 6465  >.....<lang code
-0003a550: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-0003a560: 3545 223e 0d0a 0909 0909 3c64 6973 706c  5E">......<displ
-0003a570: 6179 3e5e 3c2f 6469 7370 6c61 793e 0d0a  ay>^</display>..
-0003a580: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-0003a590: 5e3c 2f61 6363 6573 7369 626c 653e 0d0a  ^</accessible>..
-0003a5a0: 0909 093c 2f6c 616e 673e 0d0a 0909 3c2f  ...</lang>....</
-0003a5b0: 7665 7273 696f 6e3e 0d0a 093c 2f74 6f6b  version>...</tok
-0003a5c0: 656e 3e0d 0a09 3c74 6f6b 656e 2076 616c  en>...<token val
-0003a5d0: 7565 3d22 2446 3122 3e0d 0a09 093c 7665  ue="$F1">....<ve
-0003a5e0: 7273 696f 6e3e 0d0a 0909 093c 7369 6e63  rsion>.....<sinc
-0003a5f0: 653e 0d0a 0909 0909 3c6d 6f64 656c 3e54  e>......<model>T
-0003a600: 492d 3832 3c2f 6d6f 6465 6c3e 0d0a 0909  I-82</model>....
-0003a610: 0909 3c6f 732d 7665 7273 696f 6e3e 312e  ..<os-version>1.
-0003a620: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
-0003a630: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
-0003a640: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
-0003a650: 7469 2d61 7363 6969 3d22 4344 3130 223e  ti-ascii="CD10">
-0003a660: 0d0a 0909 0909 3c64 6973 706c 6179 3ecb  ......<display>.
-0003a670: a3e2 889a 3c2f 6469 7370 6c61 793e 0d0a  ....</display>..
-0003a680: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-0003a690: 7872 6f6f 743c 2f61 6363 6573 7369 626c  xroot</accessibl
-0003a6a0: 653e 0d0a 0909 093c 2f6c 616e 673e 0d0a  e>.....</lang>..
-0003a6b0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 093c  ..</version>...<
-0003a6c0: 2f74 6f6b 656e 3e0d 0a09 3c74 6f6b 656e  /token>...<token
-0003a6d0: 2076 616c 7565 3d22 2446 3222 3e0d 0a09   value="$F2">...
-0003a6e0: 093c 7665 7273 696f 6e3e 0d0a 0909 093c  .<version>.....<
-0003a6f0: 7369 6e63 653e 0d0a 0909 0909 3c6d 6f64  since>......<mod
-0003a700: 656c 3e54 492d 3832 3c2f 6d6f 6465 6c3e  el>TI-82</model>
-0003a710: 0d0a 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-0003a720: 6e3e 312e 303c 2f6f 732d 7665 7273 696f  n>1.0</os-versio
-0003a730: 6e3e 0d0a 0909 093c 2f73 696e 6365 3e0d  n>.....</since>.
-0003a740: 0a09 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-0003a750: 656e 2220 7469 2d61 7363 6969 3d22 3331  en" ti-ascii="31
-0003a760: 3244 3536 3631 3732 3230 3533 3734 3631  2D56617220537461
-0003a770: 3734 3733 3230 223e 0d0a 0909 0909 3c64  747320">......<d
-0003a780: 6973 706c 6179 3e31 2d56 6172 2053 7461  isplay>1-Var Sta
-0003a790: 7473 2623 3033 323b 3c2f 6469 7370 6c61  ts&#032;</displa
-0003a7a0: 793e 0d0a 0909 0909 3c61 6363 6573 7369  y>......<accessi
-0003a7b0: 626c 653e 312d 5661 7220 5374 6174 7326  ble>1-Var Stats&
-0003a7c0: 2330 3332 3b3c 2f61 6363 6573 7369 626c  #032;</accessibl
-0003a7d0: 653e 0d0a 0909 093c 2f6c 616e 673e 0d0a  e>.....</lang>..
-0003a7e0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 093c  ..</version>...<
-0003a7f0: 2f74 6f6b 656e 3e0d 0a09 3c74 6f6b 656e  /token>...<token
-0003a800: 2076 616c 7565 3d22 2446 3322 3e0d 0a09   value="$F3">...
-0003a810: 093c 7665 7273 696f 6e3e 0d0a 0909 093c  .<version>.....<
-0003a820: 7369 6e63 653e 0d0a 0909 0909 3c6d 6f64  since>......<mod
-0003a830: 656c 3e54 492d 3832 3c2f 6d6f 6465 6c3e  el>TI-82</model>
-0003a840: 0d0a 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-0003a850: 6e3e 312e 303c 2f6f 732d 7665 7273 696f  n>1.0</os-versio
-0003a860: 6e3e 0d0a 0909 093c 2f73 696e 6365 3e0d  n>.....</since>.
-0003a870: 0a09 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-0003a880: 656e 2220 7469 2d61 7363 6969 3d22 3332  en" ti-ascii="32
-0003a890: 3244 3536 3631 3732 3230 3533 3734 3631  2D56617220537461
-0003a8a0: 3734 3733 3230 223e 0d0a 0909 0909 3c64  747320">......<d
-0003a8b0: 6973 706c 6179 3e32 2d56 6172 2053 7461  isplay>2-Var Sta
-0003a8c0: 7473 2623 3033 323b 3c2f 6469 7370 6c61  ts&#032;</displa
-0003a8d0: 793e 0d0a 0909 0909 3c61 6363 6573 7369  y>......<accessi
-0003a8e0: 626c 653e 322d 5661 7220 5374 6174 7326  ble>2-Var Stats&
-0003a8f0: 2330 3332 3b3c 2f61 6363 6573 7369 626c  #032;</accessibl
-0003a900: 653e 0d0a 0909 093c 2f6c 616e 673e 0d0a  e>.....</lang>..
-0003a910: 0909 3c2f 7665 7273 696f 6e3e 0d0a 093c  ..</version>...<
-0003a920: 2f74 6f6b 656e 3e0d 0a09 3c74 6f6b 656e  /token>...<token
-0003a930: 2076 616c 7565 3d22 2446 3422 3e0d 0a09   value="$F4">...
-0003a940: 093c 7665 7273 696f 6e3e 0d0a 0909 093c  .<version>.....<
-0003a950: 7369 6e63 653e 0d0a 0909 0909 3c6d 6f64  since>......<mod
-0003a960: 656c 3e54 492d 3832 3c2f 6d6f 6465 6c3e  el>TI-82</model>
-0003a970: 0d0a 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-0003a980: 6e3e 312e 303c 2f6f 732d 7665 7273 696f  n>1.0</os-versio
-0003a990: 6e3e 0d0a 0909 093c 2f73 696e 6365 3e0d  n>.....</since>.
-0003a9a0: 0a09 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-0003a9b0: 656e 2220 7469 2d61 7363 6969 3d22 3443  en" ti-ascii="4C
-0003a9c0: 3639 3645 3532 3635 3637 3238 3631 3242  696E52656728612B
-0003a9d0: 3632 3738 3239 3230 223e 0d0a 0909 0909  62782920">......
-0003a9e0: 3c64 6973 706c 6179 3e4c 696e 5265 6728  <display>LinReg(
-0003a9f0: 612b 6278 2926 2330 3332 3b3c 2f64 6973  a+bx)&#032;</dis
-0003aa00: 706c 6179 3e0d 0a09 0909 093c 6163 6365  play>......<acce
-0003aa10: 7373 6962 6c65 3e4c 696e 5265 6728 612b  ssible>LinReg(a+
-0003aa20: 6278 2926 2330 3332 3b3c 2f61 6363 6573  bx)&#032;</acces
-0003aa30: 7369 626c 653e 0d0a 0909 093c 2f6c 616e  sible>.....</lan
-0003aa40: 673e 0d0a 0909 3c2f 7665 7273 696f 6e3e  g>....</version>
-0003aa50: 0d0a 093c 2f74 6f6b 656e 3e0d 0a09 3c74  ...</token>...<t
-0003aa60: 6f6b 656e 2076 616c 7565 3d22 2446 3522  oken value="$F5"
-0003aa70: 3e0d 0a09 093c 7665 7273 696f 6e3e 0d0a  >....<version>..
-0003aa80: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-0003aa90: 3c6d 6f64 656c 3e54 492d 3832 3c2f 6d6f  <model>TI-82</mo
-0003aaa0: 6465 6c3e 0d0a 0909 0909 3c6f 732d 7665  del>......<os-ve
-0003aab0: 7273 696f 6e3e 312e 303c 2f6f 732d 7665  rsion>1.0</os-ve
-0003aac0: 7273 696f 6e3e 0d0a 0909 093c 2f73 696e  rsion>.....</sin
-0003aad0: 6365 3e0d 0a09 0909 3c6c 616e 6720 636f  ce>.....<lang co
-0003aae0: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-0003aaf0: 3d22 3435 3738 3730 3532 3635 3637 3230  ="45787052656720
-0003ab00: 223e 0d0a 0909 0909 3c64 6973 706c 6179  ">......<display
-0003ab10: 3e45 7870 5265 6726 2330 3332 3b3c 2f64  >ExpReg&#032;</d
-0003ab20: 6973 706c 6179 3e0d 0a09 0909 093c 6163  isplay>......<ac
-0003ab30: 6365 7373 6962 6c65 3e45 7870 5265 6726  cessible>ExpReg&
-0003ab40: 2330 3332 3b3c 2f61 6363 6573 7369 626c  #032;</accessibl
-0003ab50: 653e 0d0a 0909 093c 2f6c 616e 673e 0d0a  e>.....</lang>..
-0003ab60: 0909 3c2f 7665 7273 696f 6e3e 0d0a 093c  ..</version>...<
-0003ab70: 2f74 6f6b 656e 3e0d 0a09 3c74 6f6b 656e  /token>...<token
-0003ab80: 2076 616c 7565 3d22 2446 3622 3e0d 0a09   value="$F6">...
-0003ab90: 093c 7665 7273 696f 6e3e 0d0a 0909 093c  .<version>.....<
-0003aba0: 7369 6e63 653e 0d0a 0909 0909 3c6d 6f64  since>......<mod
-0003abb0: 656c 3e54 492d 3832 3c2f 6d6f 6465 6c3e  el>TI-82</model>
-0003abc0: 0d0a 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
-0003abd0: 6e3e 312e 303c 2f6f 732d 7665 7273 696f  n>1.0</os-versio
-0003abe0: 6e3e 0d0a 0909 093c 2f73 696e 6365 3e0d  n>.....</since>.
-0003abf0: 0a09 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
-0003ac00: 656e 2220 7469 2d61 7363 6969 3d22 3443  en" ti-ascii="4C
-0003ac10: 3645 3532 3635 3637 3230 223e 0d0a 0909  6E52656720">....
-0003ac20: 0909 3c64 6973 706c 6179 3e4c 6e52 6567  ..<display>LnReg
-0003ac30: 2623 3033 323b 3c2f 6469 7370 6c61 793e  &#032;</display>
-0003ac40: 0d0a 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-0003ac50: 653e 4c6e 5265 6726 2330 3332 3b3c 2f61  e>LnReg&#032;</a
-0003ac60: 6363 6573 7369 626c 653e 0d0a 0909 093c  ccessible>.....<
-0003ac70: 2f6c 616e 673e 0d0a 0909 3c2f 7665 7273  /lang>....</vers
-0003ac80: 696f 6e3e 0d0a 093c 2f74 6f6b 656e 3e0d  ion>...</token>.
-0003ac90: 0a09 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
-0003aca0: 2446 3722 3e0d 0a09 093c 7665 7273 696f  $F7">....<versio
-0003acb0: 6e3e 0d0a 0909 093c 7369 6e63 653e 0d0a  n>.....<since>..
-0003acc0: 0909 0909 3c6d 6f64 656c 3e54 492d 3832  ....<model>TI-82
-0003acd0: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 3c6f  </model>......<o
-0003ace0: 732d 7665 7273 696f 6e3e 312e 303c 2f6f  s-version>1.0</o
-0003acf0: 732d 7665 7273 696f 6e3e 0d0a 0909 093c  s-version>.....<
-0003ad00: 2f73 696e 6365 3e0d 0a09 0909 3c6c 616e  /since>.....<lan
-0003ad10: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
-0003ad20: 7363 6969 3d22 3530 3737 3732 3532 3635  scii="5077725265
-0003ad30: 3637 3230 223e 0d0a 0909 0909 3c64 6973  6720">......<dis
-0003ad40: 706c 6179 3e50 7772 5265 6726 2330 3332  play>PwrReg&#032
-0003ad50: 3b3c 2f64 6973 706c 6179 3e0d 0a09 0909  ;</display>.....
-0003ad60: 093c 6163 6365 7373 6962 6c65 3e50 7772  .<accessible>Pwr
-0003ad70: 5265 6726 2330 3332 3b3c 2f61 6363 6573  Reg&#032;</acces
-0003ad80: 7369 626c 653e 0d0a 0909 093c 2f6c 616e  sible>.....</lan
-0003ad90: 673e 0d0a 0909 3c2f 7665 7273 696f 6e3e  g>....</version>
-0003ada0: 0d0a 093c 2f74 6f6b 656e 3e0d 0a09 3c74  ...</token>...<t
-0003adb0: 6f6b 656e 2076 616c 7565 3d22 2446 3822  oken value="$F8"
-0003adc0: 3e0d 0a09 093c 7665 7273 696f 6e3e 0d0a  >....<version>..
-0003add0: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-0003ade0: 3c6d 6f64 656c 3e54 492d 3832 3c2f 6d6f  <model>TI-82</mo
-0003adf0: 6465 6c3e 0d0a 0909 0909 3c6f 732d 7665  del>......<os-ve
-0003ae00: 7273 696f 6e3e 312e 303c 2f6f 732d 7665  rsion>1.0</os-ve
-0003ae10: 7273 696f 6e3e 0d0a 0909 093c 2f73 696e  rsion>.....</sin
-0003ae20: 6365 3e0d 0a09 0909 3c6c 616e 6720 636f  ce>.....<lang co
-0003ae30: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-0003ae40: 3d22 3444 3635 3634 3244 3444 3635 3634  ="4D65642D4D6564
-0003ae50: 3230 223e 0d0a 0909 0909 3c64 6973 706c  20">......<displ
-0003ae60: 6179 3e4d 6564 2d4d 6564 2623 3033 323b  ay>Med-Med&#032;
-0003ae70: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-0003ae80: 3c61 6363 6573 7369 626c 653e 4d65 642d  <accessible>Med-
-0003ae90: 4d65 6426 2330 3332 3b3c 2f61 6363 6573  Med&#032;</acces
-0003aea0: 7369 626c 653e 0d0a 0909 093c 2f6c 616e  sible>.....</lan
-0003aeb0: 673e 0d0a 0909 3c2f 7665 7273 696f 6e3e  g>....</version>
-0003aec0: 0d0a 093c 2f74 6f6b 656e 3e0d 0a09 3c74  ...</token>...<t
-0003aed0: 6f6b 656e 2076 616c 7565 3d22 2446 3922  oken value="$F9"
-0003aee0: 3e0d 0a09 093c 7665 7273 696f 6e3e 0d0a  >....<version>..
-0003aef0: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-0003af00: 3c6d 6f64 656c 3e54 492d 3832 3c2f 6d6f  <model>TI-82</mo
-0003af10: 6465 6c3e 0d0a 0909 0909 3c6f 732d 7665  del>......<os-ve
-0003af20: 7273 696f 6e3e 312e 303c 2f6f 732d 7665  rsion>1.0</os-ve
-0003af30: 7273 696f 6e3e 0d0a 0909 093c 2f73 696e  rsion>.....</sin
-0003af40: 6365 3e0d 0a09 0909 3c6c 616e 6720 636f  ce>.....<lang co
-0003af50: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-0003af60: 3d22 3531 3735 3631 3634 3532 3635 3637  ="51756164526567
-0003af70: 3230 223e 0d0a 0909 0909 3c64 6973 706c  20">......<displ
-0003af80: 6179 3e51 7561 6452 6567 2623 3033 323b  ay>QuadReg&#032;
-0003af90: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-0003afa0: 3c61 6363 6573 7369 626c 653e 5175 6164  <accessible>Quad
-0003afb0: 5265 6726 2330 3332 3b3c 2f61 6363 6573  Reg&#032;</acces
-0003afc0: 7369 626c 653e 0d0a 0909 093c 2f6c 616e  sible>.....</lan
-0003afd0: 673e 0d0a 0909 3c2f 7665 7273 696f 6e3e  g>....</version>
-0003afe0: 0d0a 093c 2f74 6f6b 656e 3e0d 0a09 3c74  ...</token>...<t
-0003aff0: 6f6b 656e 2076 616c 7565 3d22 2446 4122  oken value="$FA"
-0003b000: 3e0d 0a09 093c 7665 7273 696f 6e3e 0d0a  >....<version>..
-0003b010: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-0003b020: 3c6d 6f64 656c 3e54 492d 3832 3c2f 6d6f  <model>TI-82</mo
-0003b030: 6465 6c3e 0d0a 0909 0909 3c6f 732d 7665  del>......<os-ve
-0003b040: 7273 696f 6e3e 312e 303c 2f6f 732d 7665  rsion>1.0</os-ve
-0003b050: 7273 696f 6e3e 0d0a 0909 093c 2f73 696e  rsion>.....</sin
-0003b060: 6365 3e0d 0a09 0909 3c6c 616e 6720 636f  ce>.....<lang co
-0003b070: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-0003b080: 3d22 3433 3643 3732 3443 3639 3733 3734  ="436C724C697374
-0003b090: 3230 223e 0d0a 0909 0909 3c64 6973 706c  20">......<displ
-0003b0a0: 6179 3e43 6c72 4c69 7374 2623 3033 323b  ay>ClrList&#032;
-0003b0b0: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
-0003b0c0: 3c61 6363 6573 7369 626c 653e 436c 724c  <accessible>ClrL
-0003b0d0: 6973 7426 2330 3332 3b3c 2f61 6363 6573  ist&#032;</acces
-0003b0e0: 7369 626c 653e 0d0a 0909 093c 2f6c 616e  sible>.....</lan
-0003b0f0: 673e 0d0a 0909 3c2f 7665 7273 696f 6e3e  g>....</version>
-0003b100: 0d0a 093c 2f74 6f6b 656e 3e0d 0a09 3c74  ...</token>...<t
-0003b110: 6f6b 656e 2076 616c 7565 3d22 2446 4222  oken value="$FB"
-0003b120: 3e0d 0a09 093c 7665 7273 696f 6e3e 0d0a  >....<version>..
-0003b130: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-0003b140: 3c6d 6f64 656c 3e54 492d 3832 3c2f 6d6f  <model>TI-82</mo
-0003b150: 6465 6c3e 0d0a 0909 0909 3c6f 732d 7665  del>......<os-ve
-0003b160: 7273 696f 6e3e 312e 303c 2f6f 732d 7665  rsion>1.0</os-ve
-0003b170: 7273 696f 6e3e 0d0a 0909 093c 2f73 696e  rsion>.....</sin
-0003b180: 6365 3e0d 0a09 0909 3c6c 616e 6720 636f  ce>.....<lang co
-0003b190: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-0003b1a0: 3d22 3433 3643 3732 3534 3631 3632 3643  ="436C725461626C
-0003b1b0: 3635 223e 0d0a 0909 0909 3c64 6973 706c  65">......<displ
-0003b1c0: 6179 3e43 6c72 5461 626c 653c 2f64 6973  ay>ClrTable</dis
-0003b1d0: 706c 6179 3e0d 0a09 0909 093c 6163 6365  play>......<acce
-0003b1e0: 7373 6962 6c65 3e43 6c72 5461 626c 653c  ssible>ClrTable<
-0003b1f0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
-0003b200: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
-0003b210: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
-0003b220: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
-0003b230: 3d22 2446 4322 3e0d 0a09 093c 7665 7273  ="$FC">....<vers
-0003b240: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
-0003b250: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
-0003b260: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
-0003b270: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
-0003b280: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
-0003b290: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
-0003b2a0: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
-0003b2b0: 2d61 7363 6969 3d22 3438 3639 3733 3734  -ascii="48697374
-0003b2c0: 3646 3637 3732 3631 3644 223e 0d0a 0909  6F6772616D">....
-0003b2d0: 0909 3c64 6973 706c 6179 3e48 6973 746f  ..<display>Histo
-0003b2e0: 6772 616d 3c2f 6469 7370 6c61 793e 0d0a  gram</display>..
-0003b2f0: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
-0003b300: 4869 7374 6f67 7261 6d3c 2f61 6363 6573  Histogram</acces
-0003b310: 7369 626c 653e 0d0a 0909 093c 2f6c 616e  sible>.....</lan
-0003b320: 673e 0d0a 0909 3c2f 7665 7273 696f 6e3e  g>....</version>
-0003b330: 0d0a 093c 2f74 6f6b 656e 3e0d 0a09 3c74  ...</token>...<t
-0003b340: 6f6b 656e 2076 616c 7565 3d22 2446 4422  oken value="$FD"
-0003b350: 3e0d 0a09 093c 7665 7273 696f 6e3e 0d0a  >....<version>..
-0003b360: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-0003b370: 3c6d 6f64 656c 3e54 492d 3832 3c2f 6d6f  <model>TI-82</mo
-0003b380: 6465 6c3e 0d0a 0909 0909 3c6f 732d 7665  del>......<os-ve
-0003b390: 7273 696f 6e3e 312e 303c 2f6f 732d 7665  rsion>1.0</os-ve
-0003b3a0: 7273 696f 6e3e 0d0a 0909 093c 2f73 696e  rsion>.....</sin
-0003b3b0: 6365 3e0d 0a09 0909 3c6c 616e 6720 636f  ce>.....<lang co
-0003b3c0: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-0003b3d0: 3d22 3738 3739 3443 3639 3645 3635 223e  ="78794C696E65">
-0003b3e0: 0d0a 0909 0909 3c64 6973 706c 6179 3e78  ......<display>x
-0003b3f0: 794c 696e 653c 2f64 6973 706c 6179 3e0d  yLine</display>.
-0003b400: 0a09 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
-0003b410: 3e78 794c 696e 653c 2f61 6363 6573 7369  >xyLine</accessi
-0003b420: 626c 653e 0d0a 0909 093c 2f6c 616e 673e  ble>.....</lang>
-0003b430: 0d0a 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
-0003b440: 093c 2f74 6f6b 656e 3e0d 0a09 3c74 6f6b  .</token>...<tok
-0003b450: 656e 2076 616c 7565 3d22 2446 4522 3e0d  en value="$FE">.
-0003b460: 0a09 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
-0003b470: 093c 7369 6e63 653e 0d0a 0909 0909 3c6d  .<since>......<m
-0003b480: 6f64 656c 3e54 492d 3832 3c2f 6d6f 6465  odel>TI-82</mode
-0003b490: 6c3e 0d0a 0909 0909 3c6f 732d 7665 7273  l>......<os-vers
-0003b4a0: 696f 6e3e 312e 303c 2f6f 732d 7665 7273  ion>1.0</os-vers
-0003b4b0: 696f 6e3e 0d0a 0909 093c 2f73 696e 6365  ion>.....</since
-0003b4c0: 3e0d 0a09 0909 3c6c 616e 6720 636f 6465  >.....<lang code
-0003b4d0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
-0003b4e0: 3533 3633 3631 3734 3734 3635 3732 223e  53636174746572">
-0003b4f0: 0d0a 0909 0909 3c64 6973 706c 6179 3e53  ......<display>S
-0003b500: 6361 7474 6572 3c2f 6469 7370 6c61 793e  catter</display>
-0003b510: 0d0a 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
-0003b520: 653e 5363 6174 7465 723c 2f61 6363 6573  e>Scatter</acces
-0003b530: 7369 626c 653e 0d0a 0909 093c 2f6c 616e  sible>.....</lan
-0003b540: 673e 0d0a 0909 3c2f 7665 7273 696f 6e3e  g>....</version>
-0003b550: 0d0a 093c 2f74 6f6b 656e 3e0d 0a09 3c74  ...</token>...<t
-0003b560: 6f6b 656e 2076 616c 7565 3d22 2446 4622  oken value="$FF"
-0003b570: 3e0d 0a09 093c 7665 7273 696f 6e3e 0d0a  >....<version>..
-0003b580: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
-0003b590: 3c6d 6f64 656c 3e54 492d 3832 3c2f 6d6f  <model>TI-82</mo
-0003b5a0: 6465 6c3e 0d0a 0909 0909 3c6f 732d 7665  del>......<os-ve
-0003b5b0: 7273 696f 6e3e 312e 303c 2f6f 732d 7665  rsion>1.0</os-ve
-0003b5c0: 7273 696f 6e3e 0d0a 0909 093c 2f73 696e  rsion>.....</sin
-0003b5d0: 6365 3e0d 0a09 0909 3c6c 616e 6720 636f  ce>.....<lang co
-0003b5e0: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
-0003b5f0: 3d22 3443 3639 3645 3532 3635 3637 3238  ="4C696E52656728
-0003b600: 3631 3738 3242 3632 3239 3230 223e 0d0a  61782B622920">..
-0003b610: 0909 0909 3c64 6973 706c 6179 3e4c 696e  ....<display>Lin
-0003b620: 5265 6728 6178 2b62 2926 2330 3332 3b3c  Reg(ax+b)&#032;<
-0003b630: 2f64 6973 706c 6179 3e0d 0a09 0909 093c  /display>......<
-0003b640: 6163 6365 7373 6962 6c65 3e4c 696e 5265  accessible>LinRe
-0003b650: 6728 6178 2b62 2926 2330 3332 3b3c 2f61  g(ax+b)&#032;</a
-0003b660: 6363 6573 7369 626c 653e 0d0a 0909 093c  ccessible>.....<
-0003b670: 2f6c 616e 673e 0d0a 0909 3c2f 7665 7273  /lang>....</vers
-0003b680: 696f 6e3e 0d0a 093c 2f74 6f6b 656e 3e0d  ion>...</token>.
-0003b690: 0a3c 2f74 6f6b 656e 733e 0d0a            .</tokens>..
+00032780: 4578 6563 4c69 6226 2330 3332 3b3c 2f61  ExecLib&#032;</a
+00032790: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+000327a0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+000327b0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+000327c0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+000327d0: 7565 3d22 2431 3322 3e0d 0a09 0909 3c76  ue="$13">.....<v
+000327e0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+000327f0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00032800: 6c3e 5449 2d38 342b 3c2f 6d6f 6465 6c3e  l>TI-84+</model>
+00032810: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
+00032820: 6f6e 3e32 2e33 303c 2f6f 732d 7665 7273  on>2.30</os-vers
+00032830: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
+00032840: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
+00032850: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
+00032860: 3d22 3639 3645 3736 3534 3238 223e 0d0a  ="696E765428">..
+00032870: 0909 0909 093c 6469 7370 6c61 793e 696e  .....<display>in
+00032880: 7654 283c 2f64 6973 706c 6179 3e0d 0a09  vT(</display>...
+00032890: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
+000328a0: 696e 7654 283c 2f61 6363 6573 7369 626c  invT(</accessibl
+000328b0: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+000328c0: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+000328d0: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+000328e0: 6f6b 656e 2076 616c 7565 3d22 2431 3422  oken value="$14"
+000328f0: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00032900: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+00032910: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+00032920: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
+00032930: 6f73 2d76 6572 7369 6f6e 3e32 2e33 303c  os-version>2.30<
+00032940: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00032950: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00032960: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00032970: 7469 2d61 7363 6969 3d22 4439 3132 3437  ti-ascii="D91247
+00032980: 3446 3436 3244 3534 3635 3733 3734 3238  4F462D5465737428
+00032990: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+000329a0: 793e cf87 c2b2 474f 462d 5465 7374 283c  y>....GOF-Test(<
+000329b0: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
+000329c0: 3c61 6363 6573 7369 626c 653e 6368 695e  <accessible>chi^
+000329d0: 3247 4f46 2d54 6573 7428 3c2f 6163 6365  2GOF-Test(</acce
+000329e0: 7373 6962 6c65 3e0d 0a09 0909 0909 3c76  ssible>.......<v
+000329f0: 6172 6961 6e74 3ecf 875e 3247 4f46 2d54  ariant>..^2GOF-T
+00032a00: 6573 7428 3c2f 7661 7269 616e 743e 0d0a  est(</variant>..
+00032a10: 0909 0909 093c 7661 7269 616e 743e 6368  .....<variant>ch
+00032a20: 69c2 b247 4f46 2d54 6573 7428 3c2f 7661  i..GOF-Test(</va
+00032a30: 7269 616e 743e 0d0a 0909 0909 3c2f 6c61  riant>......</la
+00032a40: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
+00032a50: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
+00032a60: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+00032a70: 2431 3522 3e0d 0a09 0909 3c76 6572 7369  $15">.....<versi
+00032a80: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
+00032a90: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
+00032aa0: 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a 0909  -84+</model>....
+00032ab0: 0909 093c 6f73 2d76 6572 7369 6f6e 3e32  ...<os-version>2
+00032ac0: 2e33 303c 2f6f 732d 7665 7273 696f 6e3e  .30</os-version>
+00032ad0: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
+00032ae0: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
+00032af0: 656e 2220 7469 2d61 7363 6969 3d22 3443  en" ti-ascii="4C
+00032b00: 3639 3645 3532 3635 3637 3534 3439 3645  696E52656754496E
+00032b10: 3734 3230 223e 0d0a 0909 0909 093c 6469  7420">.......<di
+00032b20: 7370 6c61 793e 4c69 6e52 6567 5449 6e74  splay>LinRegTInt
+00032b30: 2623 3033 323b 3c2f 6469 7370 6c61 793e  &#032;</display>
+00032b40: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+00032b50: 6c65 3e4c 696e 5265 6754 496e 7426 2330  le>LinRegTInt&#0
+00032b60: 3332 3b3c 2f61 6363 6573 7369 626c 653e  32;</accessible>
+00032b70: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
+00032b80: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
+00032b90: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
+00032ba0: 656e 2076 616c 7565 3d22 2431 3622 3e0d  en value="$16">.
+00032bb0: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
+00032bc0: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
+00032bd0: 093c 6d6f 6465 6c3e 5449 2d38 342b 3c2f  .<model>TI-84+</
+00032be0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
+00032bf0: 2d76 6572 7369 6f6e 3e30 2e34 363c 2f6f  -version>0.46</o
+00032c00: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
+00032c10: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
+00032c20: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+00032c30: 2d61 7363 6969 3d22 3444 3631 3645 3735  -ascii="4D616E75
+00032c40: 3631 3643 3244 3436 3639 3734 3230 223e  616C2D46697420">
+00032c50: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00032c60: 4d61 6e75 616c 2d46 6974 2623 3033 323b  Manual-Fit&#032;
+00032c70: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00032c80: 093c 6163 6365 7373 6962 6c65 3e4d 616e  .<accessible>Man
+00032c90: 7561 6c2d 4669 7426 2330 3332 3b3c 2f61  ual-Fit&#032;</a
+00032ca0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+00032cb0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+00032cc0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+00032cd0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+00032ce0: 7565 3d22 2431 3722 3e0d 0a09 0909 3c76  ue="$17">.....<v
+00032cf0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+00032d00: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00032d10: 6c3e 5449 2d38 342b 3c2f 6d6f 6465 6c3e  l>TI-84+</model>
+00032d20: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
+00032d30: 6f6e 3e30 2e30 313c 2f6f 732d 7665 7273  on>0.01</os-vers
+00032d40: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
+00032d50: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
+00032d60: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
+00032d70: 3d22 3541 3531 3735 3631 3634 3732 3631  ="5A517561647261
+00032d80: 3645 3734 3331 223e 0d0a 0909 0909 093c  6E7431">.......<
+00032d90: 6469 7370 6c61 793e 5a51 7561 6472 616e  display>ZQuadran
+00032da0: 7431 3c2f 6469 7370 6c61 793e 0d0a 0909  t1</display>....
+00032db0: 0909 093c 6163 6365 7373 6962 6c65 3e5a  ...<accessible>Z
+00032dc0: 5175 6164 7261 6e74 313c 2f61 6363 6573  Quadrant1</acces
+00032dd0: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
+00032de0: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
+00032df0: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
+00032e00: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+00032e10: 2431 3822 3e0d 0a09 0909 3c76 6572 7369  $18">.....<versi
+00032e20: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
+00032e30: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
+00032e40: 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a 0909  -84+</model>....
+00032e50: 0909 093c 6f73 2d76 6572 7369 6f6e 3e32  ...<os-version>2
+00032e60: 2e35 333c 2f6f 732d 7665 7273 696f 6e3e  .53</os-version>
+00032e70: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
+00032e80: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
+00032e90: 656e 2220 7469 2d61 7363 6969 3d22 3541  en" ti-ascii="5A
+00032ea0: 3436 3732 3631 3633 3331 4636 3332 223e  4672616331F632">
+00032eb0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00032ec0: 5a46 7261 6331 e281 8432 3c2f 6469 7370  ZFrac1...2</disp
+00032ed0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+00032ee0: 7373 6962 6c65 3e5a 4672 6163 312f 323c  ssible>ZFrac1/2<
+00032ef0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00032f00: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+00032f10: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+00032f20: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+00032f30: 616c 7565 3d22 2431 3922 3e0d 0a09 0909  alue="$19">.....
+00032f40: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+00032f50: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+00032f60: 6465 6c3e 5449 2d38 342b 3c2f 6d6f 6465  del>TI-84+</mode
+00032f70: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
+00032f80: 7369 6f6e 3e32 2e35 333c 2f6f 732d 7665  sion>2.53</os-ve
+00032f90: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+00032fa0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+00032fb0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+00032fc0: 6969 3d22 3541 3436 3732 3631 3633 3331  ii="5A4672616331
+00032fd0: 4636 3333 223e 0d0a 0909 0909 093c 6469  F633">.......<di
+00032fe0: 7370 6c61 793e 5a46 7261 6331 e281 8433  splay>ZFrac1...3
+00032ff0: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00033000: 093c 6163 6365 7373 6962 6c65 3e5a 4672  .<accessible>ZFr
+00033010: 6163 312f 333c 2f61 6363 6573 7369 626c  ac1/3</accessibl
+00033020: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00033030: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+00033040: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+00033050: 6f6b 656e 2076 616c 7565 3d22 2431 4122  oken value="$1A"
+00033060: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00033070: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+00033080: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+00033090: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
+000330a0: 6f73 2d76 6572 7369 6f6e 3e32 2e35 333c  os-version>2.53<
+000330b0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+000330c0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+000330d0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+000330e0: 7469 2d61 7363 6969 3d22 3541 3436 3732  ti-ascii="5A4672
+000330f0: 3631 3633 3331 4636 3334 223e 0d0a 0909  616331F634">....
+00033100: 0909 093c 6469 7370 6c61 793e 5a46 7261  ...<display>ZFra
+00033110: 6331 e281 8434 3c2f 6469 7370 6c61 793e  c1...4</display>
+00033120: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+00033130: 6c65 3e5a 4672 6163 312f 343c 2f61 6363  le>ZFrac1/4</acc
+00033140: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
+00033150: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
+00033160: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
+00033170: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
+00033180: 3d22 2431 4222 3e0d 0a09 0909 3c76 6572  ="$1B">.....<ver
+00033190: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
+000331a0: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
+000331b0: 5449 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a  TI-84+</model>..
+000331c0: 0909 0909 093c 6f73 2d76 6572 7369 6f6e  .....<os-version
+000331d0: 3e32 2e35 333c 2f6f 732d 7665 7273 696f  >2.53</os-versio
+000331e0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
+000331f0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
+00033200: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+00033210: 3541 3436 3732 3631 3633 3331 4636 3335  5A4672616331F635
+00033220: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00033230: 793e 5a46 7261 6331 e281 8435 3c2f 6469  y>ZFrac1...5</di
+00033240: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00033250: 6365 7373 6962 6c65 3e5a 4672 6163 312f  cessible>ZFrac1/
+00033260: 353c 2f61 6363 6573 7369 626c 653e 0d0a  5</accessible>..
+00033270: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00033280: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00033290: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+000332a0: 2076 616c 7565 3d22 2431 4322 3e0d 0a09   value="$1C">...
+000332b0: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+000332c0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+000332d0: 6d6f 6465 6c3e 5449 2d38 342b 3c2f 6d6f  model>TI-84+</mo
+000332e0: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
+000332f0: 6572 7369 6f6e 3e32 2e35 333c 2f6f 732d  ersion>2.53</os-
+00033300: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+00033310: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+00033320: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+00033330: 7363 6969 3d22 3541 3436 3732 3631 3633  scii="5A46726163
+00033340: 3331 4636 3338 223e 0d0a 0909 0909 093c  31F638">.......<
+00033350: 6469 7370 6c61 793e 5a46 7261 6331 e281  display>ZFrac1..
+00033360: 8438 3c2f 6469 7370 6c61 793e 0d0a 0909  .8</display>....
+00033370: 0909 093c 6163 6365 7373 6962 6c65 3e5a  ...<accessible>Z
+00033380: 4672 6163 312f 383c 2f61 6363 6573 7369  Frac1/8</accessi
+00033390: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
+000333a0: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
+000333b0: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
+000333c0: 3c74 6f6b 656e 2076 616c 7565 3d22 2431  <token value="$1
+000333d0: 4422 3e0d 0a09 0909 3c76 6572 7369 6f6e  D">.....<version
+000333e0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
+000333f0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
+00033400: 342b 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  4+</model>......
+00033410: 093c 6f73 2d76 6572 7369 6f6e 3e32 2e35  .<os-version>2.5
+00033420: 333c 2f6f 732d 7665 7273 696f 6e3e 0d0a  3</os-version>..
+00033430: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
+00033440: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00033450: 2220 7469 2d61 7363 6969 3d22 3541 3436  " ti-ascii="5A46
+00033460: 3732 3631 3633 3331 4636 3331 3330 223e  72616331F63130">
+00033470: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00033480: 5a46 7261 6331 e281 8431 303c 2f64 6973  ZFrac1...10</dis
+00033490: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
+000334a0: 6573 7369 626c 653e 5a46 7261 6331 2f31  essible>ZFrac1/1
+000334b0: 303c 2f61 6363 6573 7369 626c 653e 0d0a  0</accessible>..
+000334c0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+000334d0: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+000334e0: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+000334f0: 2076 616c 7565 3d22 2431 4522 3e0d 0a09   value="$1E">...
+00033500: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00033510: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00033520: 6d6f 6465 6c3e 5449 2d38 342b 3c2f 6d6f  model>TI-84+</mo
+00033530: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
+00033540: 6572 7369 6f6e 3e32 2e35 333c 2f6f 732d  ersion>2.53</os-
+00033550: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+00033560: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+00033570: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+00033580: 7363 6969 3d22 4637 223e 0d0a 0909 0909  scii="F7">......
+00033590: 093c 6469 7370 6c61 793e 2e3c 2f64 6973  .<display>.</dis
+000335a0: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
+000335b0: 6573 7369 626c 653e 6d61 7468 7072 696e  essible>mathprin
+000335c0: 7462 6f78 3c2f 6163 6365 7373 6962 6c65  tbox</accessible
+000335d0: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+000335e0: 3ee2 ac9a 3c2f 7661 7269 616e 743e 0d0a  >...</variant>..
+000335f0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00033600: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00033610: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00033620: 2076 616c 7565 3d22 2432 4522 3e0d 0a09   value="$2E">...
+00033630: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00033640: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00033650: 6d6f 6465 6c3e 5449 2d38 342b 3c2f 6d6f  model>TI-84+</mo
+00033660: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
+00033670: 6572 7369 6f6e 3e32 2e35 333c 2f6f 732d  ersion>2.53</os-
+00033680: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+00033690: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+000336a0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+000336b0: 7363 6969 3d22 4636 223e 0d0a 0909 0909  scii="F6">......
+000336c0: 093c 6469 7370 6c61 793e e281 843c 2f64  .<display>...</d
+000336d0: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
+000336e0: 6363 6573 7369 626c 653e 6e2f 643c 2f61  ccessible>n/d</a
+000336f0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+00033700: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+00033710: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+00033720: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+00033730: 7565 3d22 2432 4622 3e0d 0a09 0909 3c76  ue="$2F">.....<v
+00033740: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+00033750: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00033760: 6c3e 5449 2d38 342b 3c2f 6d6f 6465 6c3e  l>TI-84+</model>
+00033770: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
+00033780: 6f6e 3e32 2e35 333c 2f6f 732d 7665 7273  on>2.53</os-vers
+00033790: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
+000337a0: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
+000337b0: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
+000337c0: 3d22 4635 223e 0d0a 0909 0909 093c 6469  ="F5">.......<di
+000337d0: 7370 6c61 793e f3b8 8fb5 3c2f 6469 7370  splay>....</disp
+000337e0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+000337f0: 7373 6962 6c65 3e55 6e2f 643c 2f61 6363  ssible>Un/d</acc
+00033800: 6573 7369 626c 653e 0d0a 0909 0909 093c  essible>.......<
+00033810: 7661 7269 616e 743e e1b5 a43c 2f76 6172  variant>...</var
+00033820: 6961 6e74 3e0d 0a09 0909 093c 2f6c 616e  iant>......</lan
+00033830: 673e 0d0a 0909 093c 2f76 6572 7369 6f6e  g>.....</version
+00033840: 3e0d 0a09 093c 2f74 6f6b 656e 3e0d 0a09  >....</token>...
+00033850: 093c 746f 6b65 6e20 7661 6c75 653d 2224  .<token value="$
+00033860: 3330 223e 0d0a 0909 093c 7665 7273 696f  30">.....<versio
+00033870: 6e3e 0d0a 0909 0909 3c73 696e 6365 3e0d  n>......<since>.
+00033880: 0a09 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+00033890: 3834 2b3c 2f6d 6f64 656c 3e0d 0a09 0909  84+</model>.....
+000338a0: 0909 3c6f 732d 7665 7273 696f 6e3e 322e  ..<os-version>2.
+000338b0: 3533 3c2f 6f73 2d76 6572 7369 6f6e 3e0d  53</os-version>.
+000338c0: 0a09 0909 093c 2f73 696e 6365 3e0d 0a09  .....</since>...
+000338d0: 0909 093c 6c61 6e67 2063 6f64 653d 2265  ...<lang code="e
+000338e0: 6e22 2074 692d 6173 6369 693d 2230 3536  n" ti-ascii="056
+000338f0: 4546 3636 3443 4630 3535 3536 4546 3636  EF664CF05556EF66
+00033900: 3422 3e0d 0a09 0909 0909 3c64 6973 706c  4">.......<displ
+00033910: 6179 3ee2 96ba 6ee2 8184 64e2 9784 e296  ay>...n...d.....
+00033920: ba55 6ee2 8184 643c 2f64 6973 706c 6179  .Un...d</display
+00033930: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
+00033940: 626c 653e 2667 743b 6e2f 6426 6c74 3b26  ble>&gt;n/d&lt;&
+00033950: 6774 3b55 6e2f 643c 2f61 6363 6573 7369  gt;Un/d</accessi
+00033960: 626c 653e 0d0a 0909 0909 093c 7661 7269  ble>.......<vari
+00033970: 616e 743e e296 ba6e 2f64 e297 84e2 96ba  ant>...n/d......
+00033980: 556e 2f64 3c2f 7661 7269 616e 743e 0d0a  Un/d</variant>..
+00033990: 0909 0909 093c 7661 7269 616e 743e 2667  .....<variant>&g
+000339a0: 743b 6ee2 8184 6426 6c74 3b26 6774 3b55  t;n...d&lt;&gt;U
+000339b0: 6ee2 8184 643c 2f76 6172 6961 6e74 3e0d  n...d</variant>.
+000339c0: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+000339d0: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+000339e0: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+000339f0: 6e20 7661 6c75 653d 2224 3331 223e 0d0a  n value="$31">..
+00033a00: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00033a10: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00033a20: 3c6d 6f64 656c 3e54 492d 3834 2b3c 2f6d  <model>TI-84+</m
+00033a30: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+00033a40: 7665 7273 696f 6e3e 322e 3533 3c2f 6f73  version>2.53</os
+00033a50: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
+00033a60: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
+00033a70: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
+00033a80: 6173 6369 693d 2230 3534 3643 4630 3534  ascii="0546CF054
+00033a90: 3422 3e0d 0a09 0909 0909 3c64 6973 706c  4">.......<displ
+00033aa0: 6179 3ee2 96ba 46e2 9784 e296 ba44 3c2f  ay>...F......D</
+00033ab0: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
+00033ac0: 6163 6365 7373 6962 6c65 3e26 6774 3b46  accessible>&gt;F
+00033ad0: 266c 743b 2667 743b 443c 2f61 6363 6573  &lt;&gt;D</acces
+00033ae0: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
+00033af0: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
+00033b00: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
+00033b10: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+00033b20: 2433 3222 3e0d 0a09 0909 3c76 6572 7369  $32">.....<versi
+00033b30: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
+00033b40: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
+00033b50: 2d38 342b 3c2f 6d6f 6465 6c3e 0d0a 0909  -84+</model>....
+00033b60: 0909 093c 6f73 2d76 6572 7369 6f6e 3e32  ...<os-version>2
+00033b70: 2e35 333c 2f6f 732d 7665 7273 696f 6e3e  .53</os-version>
+00033b80: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
+00033b90: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
+00033ba0: 656e 2220 7469 2d61 7363 6969 3d22 3732  en" ti-ascii="72
+00033bb0: 3635 3644 3631 3639 3645 3634 3635 3732  656D61696E646572
+00033bc0: 3238 223e 0d0a 0909 0909 093c 6469 7370  28">.......<disp
+00033bd0: 6c61 793e 7265 6d61 696e 6465 7228 3c2f  lay>remainder(</
+00033be0: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
+00033bf0: 6163 6365 7373 6962 6c65 3e72 656d 6169  accessible>remai
+00033c00: 6e64 6572 283c 2f61 6363 6573 7369 626c  nder(</accessibl
+00033c10: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00033c20: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+00033c30: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+00033c40: 6f6b 656e 2076 616c 7565 3d22 2433 3322  oken value="$33"
+00033c50: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00033c60: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+00033c70: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+00033c80: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
+00033c90: 6f73 2d76 6572 7369 6f6e 3e32 2e35 333c  os-version>2.53<
+00033ca0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00033cb0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00033cc0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00033cd0: 7469 2d61 7363 6969 3d22 4336 3238 223e  ti-ascii="C628">
+00033ce0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00033cf0: cea3 283c 2f64 6973 706c 6179 3e0d 0a09  ..(</display>...
+00033d00: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
+00033d10: 5369 676d 6128 3c2f 6163 6365 7373 6962  Sigma(</accessib
+00033d20: 6c65 3e0d 0a09 0909 093c 2f6c 616e 673e  le>......</lang>
+00033d30: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
+00033d40: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
+00033d50: 746f 6b65 6e20 7661 6c75 653d 2224 3334  token value="$34
+00033d60: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
+00033d70: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
+00033d80: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
+00033d90: 2b3c 2f6d 6f64 656c 3e0d 0a09 0909 0909  +</model>.......
+00033da0: 3c6f 732d 7665 7273 696f 6e3e 322e 3533  <os-version>2.53
+00033db0: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
+00033dc0: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
+00033dd0: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
+00033de0: 2074 692d 6173 6369 693d 2236 4336 4636   ti-ascii="6C6F6
+00033df0: 3734 3234 3135 3334 3532 3822 3e0d 0a09  74241534528">...
+00033e00: 0909 0909 3c64 6973 706c 6179 3e6c 6f67  ....<display>log
+00033e10: 4241 5345 283c 2f64 6973 706c 6179 3e0d  BASE(</display>.
+00033e20: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+00033e30: 653e 6c6f 6742 4153 4528 3c2f 6163 6365  e>logBASE(</acce
+00033e40: 7373 6962 6c65 3e0d 0a09 0909 093c 2f6c  ssible>......</l
+00033e50: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
+00033e60: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
+00033e70: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
+00033e80: 2224 3335 223e 0d0a 0909 093c 7665 7273  "$35">.....<vers
+00033e90: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
+00033ea0: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
+00033eb0: 492d 3834 2b3c 2f6d 6f64 656c 3e0d 0a09  I-84+</model>...
+00033ec0: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
+00033ed0: 322e 3533 3c2f 6f73 2d76 6572 7369 6f6e  2.53</os-version
+00033ee0: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
+00033ef0: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
+00033f00: 2265 6e22 2074 692d 6173 6369 693d 2237  "en" ti-ascii="7
+00033f10: 3236 3136 4536 3434 3936 4537 3434 4536  2616E64496E744E6
+00033f20: 4635 3236 3537 3032 3822 3e0d 0a09 0909  F52657028">.....
+00033f30: 0909 3c64 6973 706c 6179 3e72 616e 6449  ..<display>randI
+00033f40: 6e74 4e6f 5265 7028 3c2f 6469 7370 6c61  ntNoRep(</displa
+00033f50: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
+00033f60: 6962 6c65 3e72 616e 6449 6e74 4e6f 5265  ible>randIntNoRe
+00033f70: 7028 3c2f 6163 6365 7373 6962 6c65 3e0d  p(</accessible>.
+00033f80: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+00033f90: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00033fa0: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+00033fb0: 6e20 7661 6c75 653d 2224 3337 223e 0d0a  n value="$37">..
+00033fc0: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00033fd0: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00033fe0: 3c6d 6f64 656c 3e54 492d 3834 2b3c 2f6d  <model>TI-84+</m
+00033ff0: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+00034000: 7665 7273 696f 6e3e 322e 3533 3c2f 6f73  version>2.53</os
+00034010: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
+00034020: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
+00034030: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
+00034040: 6173 6369 693d 2234 4434 3135 3434 3835  ascii="4D4154485
+00034050: 3035 3234 3934 4535 3422 3e0d 0a09 0909  052494E54">.....
+00034060: 0909 3c64 6973 706c 6179 3e4d 4154 4850  ..<display>MATHP
+00034070: 5249 4e54 3c2f 6469 7370 6c61 793e 0d0a  RINT</display>..
+00034080: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
+00034090: 3e5b 4d41 5448 5052 494e 545d 3c2f 6163  >[MATHPRINT]</ac
+000340a0: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
+000340b0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
+000340c0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
+000340d0: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
+000340e0: 653d 2224 3338 223e 0d0a 0909 093c 7665  e="$38">.....<ve
+000340f0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
+00034100: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
+00034110: 3e54 492d 3834 2b3c 2f6d 6f64 656c 3e0d  >TI-84+</model>.
+00034120: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+00034130: 6e3e 322e 3533 3c2f 6f73 2d76 6572 7369  n>2.53</os-versi
+00034140: 6f6e 3e0d 0a09 0909 093c 2f73 696e 6365  on>......</since
+00034150: 3e0d 0a09 0909 093c 6c61 6e67 2063 6f64  >......<lang cod
+00034160: 653d 2265 6e22 2074 692d 6173 6369 693d  e="en" ti-ascii=
+00034170: 2234 3334 4334 3135 3335 3334 3934 3322  "434C4153534943"
+00034180: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
+00034190: 3e43 4c41 5353 4943 3c2f 6469 7370 6c61  >CLASSIC</displa
+000341a0: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
+000341b0: 6962 6c65 3e5b 434c 4153 5349 435d 3c2f  ible>[CLASSIC]</
+000341c0: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
+000341d0: 093c 2f6c 616e 673e 0d0a 0909 093c 2f76  .</lang>.....</v
+000341e0: 6572 7369 6f6e 3e0d 0a09 093c 2f74 6f6b  ersion>....</tok
+000341f0: 656e 3e0d 0a09 093c 746f 6b65 6e20 7661  en>....<token va
+00034200: 6c75 653d 2224 3339 223e 0d0a 0909 093c  lue="$39">.....<
+00034210: 7665 7273 696f 6e3e 0d0a 0909 0909 3c73  version>......<s
+00034220: 696e 6365 3e0d 0a09 0909 0909 3c6d 6f64  ince>.......<mod
+00034230: 656c 3e54 492d 3834 2b3c 2f6d 6f64 656c  el>TI-84+</model
+00034240: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
+00034250: 696f 6e3e 322e 3533 3c2f 6f73 2d76 6572  ion>2.53</os-ver
+00034260: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
+00034270: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
+00034280: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
+00034290: 693d 2236 4546 3636 3422 3e0d 0a09 0909  i="6EF664">.....
+000342a0: 0909 3c64 6973 706c 6179 3e6e e281 8464  ..<display>n...d
+000342b0: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+000342c0: 093c 6163 6365 7373 6962 6c65 3e5b 6e2f  .<accessible>[n/
+000342d0: 645d 3c2f 6163 6365 7373 6962 6c65 3e0d  d]</accessible>.
+000342e0: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+000342f0: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00034300: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+00034310: 6e20 7661 6c75 653d 2224 3341 223e 0d0a  n value="$3A">..
+00034320: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00034330: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00034340: 3c6d 6f64 656c 3e54 492d 3834 2b3c 2f6d  <model>TI-84+</m
+00034350: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+00034360: 7665 7273 696f 6e3e 322e 3533 3c2f 6f73  version>2.53</os
+00034370: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
+00034380: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
+00034390: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
+000343a0: 6173 6369 693d 2235 3536 4546 3636 3422  ascii="556EF664"
+000343b0: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
+000343c0: 3e55 6ee2 8184 643c 2f64 6973 706c 6179  >Un...d</display
+000343d0: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
+000343e0: 626c 653e 5b55 6e2f 645d 3c2f 6163 6365  ble>[Un/d]</acce
+000343f0: 7373 6962 6c65 3e0d 0a09 0909 093c 2f6c  ssible>......</l
+00034400: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
+00034410: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
+00034420: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
+00034430: 2224 3342 223e 0d0a 0909 093c 7665 7273  "$3B">.....<vers
+00034440: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
+00034450: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
+00034460: 492d 3834 2b3c 2f6d 6f64 656c 3e0d 0a09  I-84+</model>...
+00034470: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
+00034480: 322e 3533 3c2f 6f73 2d76 6572 7369 6f6e  2.53</os-version
+00034490: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
+000344a0: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
+000344b0: 2265 6e22 2074 692d 6173 6369 693d 2234  "en" ti-ascii="4
+000344c0: 3135 3535 3434 4622 3e0d 0a09 0909 0909  155544F">.......
+000344d0: 3c64 6973 706c 6179 3e41 5554 4f3c 2f64  <display>AUTO</d
+000344e0: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
+000344f0: 6363 6573 7369 626c 653e 5b41 5554 4f5d  ccessible>[AUTO]
+00034500: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
+00034510: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
+00034520: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
+00034530: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
+00034540: 7661 6c75 653d 2224 3343 223e 0d0a 0909  value="$3C">....
+00034550: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
+00034560: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
+00034570: 6f64 656c 3e54 492d 3834 2b3c 2f6d 6f64  odel>TI-84+</mod
+00034580: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
+00034590: 7273 696f 6e3e 322e 3533 3c2f 6f73 2d76  rsion>2.53</os-v
+000345a0: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
+000345b0: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
+000345c0: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
+000345d0: 6369 693d 2234 3434 3534 3322 3e0d 0a09  cii="444543">...
+000345e0: 0909 0909 3c64 6973 706c 6179 3e44 4543  ....<display>DEC
+000345f0: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00034600: 093c 6163 6365 7373 6962 6c65 3e5b 4445  .<accessible>[DE
+00034610: 435d 3c2f 6163 6365 7373 6962 6c65 3e0d  C]</accessible>.
+00034620: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+00034630: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00034640: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+00034650: 6e20 7661 6c75 653d 2224 3344 223e 0d0a  n value="$3D">..
+00034660: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00034670: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00034680: 3c6d 6f64 656c 3e54 492d 3834 2b3c 2f6d  <model>TI-84+</m
+00034690: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+000346a0: 7665 7273 696f 6e3e 322e 3533 3c2f 6f73  version>2.53</os
+000346b0: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
+000346c0: 2f73 696e 6365 3e0d 0a09 0909 093c 756e  /since>......<un
+000346d0: 7469 6c3e 0d0a 0909 0909 093c 6d6f 6465  til>.......<mode
+000346e0: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
+000346f0: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
+00034700: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
+00034710: 7273 696f 6e3e 0d0a 0909 0909 3c2f 756e  rsion>......</un
+00034720: 7469 6c3e 0d0a 0909 0909 3c6c 616e 6720  til>......<lang 
+00034730: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+00034740: 6969 3d22 3436 3532 3431 3433 223e 0d0a  ii="46524143">..
+00034750: 0909 0909 093c 6469 7370 6c61 793e 4652  .....<display>FR
+00034760: 4143 3c2f 6469 7370 6c61 793e 0d0a 0909  AC</display>....
+00034770: 0909 093c 6163 6365 7373 6962 6c65 3e5b  ...<accessible>[
+00034780: 4652 4143 5d3c 2f61 6363 6573 7369 626c  FRAC]</accessibl
+00034790: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+000347a0: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+000347b0: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+000347c0: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+000347d0: 3c6d 6f64 656c 3e54 492d 3834 2b43 5345  <model>TI-84+CSE
+000347e0: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
+000347f0: 6f73 2d76 6572 7369 6f6e 3e34 2e30 3c2f  os-version>4.0</
+00034800: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
+00034810: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
+00034820: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
+00034830: 692d 6173 6369 693d 2234 3635 3234 3134  i-ascii="4652414
+00034840: 3332 4434 3135 3035 3035 3234 4635 3822  32D415050524F58"
+00034850: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
+00034860: 3e46 5241 432d 4150 5052 4f58 3c2f 6469  >FRAC-APPROX</di
+00034870: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00034880: 6365 7373 6962 6c65 3e5b 4652 4143 2d41  cessible>[FRAC-A
+00034890: 5050 524f 585d 3c2f 6163 6365 7373 6962  PPROX]</accessib
+000348a0: 6c65 3e0d 0a09 0909 093c 2f6c 616e 673e  le>......</lang>
+000348b0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
+000348c0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
+000348d0: 746f 6b65 6e20 7661 6c75 653d 2224 3346  token value="$3F
+000348e0: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
+000348f0: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
+00034900: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
+00034910: 2b3c 2f6d 6f64 656c 3e0d 0a09 0909 0909  +</model>.......
+00034920: 3c6f 732d 7665 7273 696f 6e3e 322e 3535  <os-version>2.55
+00034930: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
+00034940: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
+00034950: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
+00034960: 2074 692d 6173 6369 693d 2235 3335 3434   ti-ascii="53544
+00034970: 3135 3435 3734 3935 4134 3135 3234 3432  15457495A4152442
+00034980: 3034 4634 4522 3e0d 0a09 0909 0909 3c64  04F4E">.......<d
+00034990: 6973 706c 6179 3e53 5441 5457 495a 4152  isplay>STATWIZAR
+000349a0: 4420 4f4e 3c2f 6469 7370 6c61 793e 0d0a  D ON</display>..
+000349b0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
+000349c0: 3e5b 5354 4154 5749 5a41 5244 204f 4e5d  >[STATWIZARD ON]
+000349d0: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
+000349e0: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
+000349f0: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
+00034a00: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
+00034a10: 7661 6c75 653d 2224 3430 223e 0d0a 0909  value="$40">....
+00034a20: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
+00034a30: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
+00034a40: 6f64 656c 3e54 492d 3834 2b3c 2f6d 6f64  odel>TI-84+</mod
+00034a50: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
+00034a60: 7273 696f 6e3e 322e 3535 3c2f 6f73 2d76  rsion>2.55</os-v
+00034a70: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
+00034a80: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
+00034a90: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
+00034aa0: 6369 693d 2235 3335 3434 3135 3435 3734  cii="53544154574
+00034ab0: 3935 4134 3135 3234 3432 3034 4634 3634  95A415244204F464
+00034ac0: 3622 3e0d 0a09 0909 0909 3c64 6973 706c  6">.......<displ
+00034ad0: 6179 3e53 5441 5457 495a 4152 4420 4f46  ay>STATWIZARD OF
+00034ae0: 463c 2f64 6973 706c 6179 3e0d 0a09 0909  F</display>.....
+00034af0: 0909 3c61 6363 6573 7369 626c 653e 5b53  ..<accessible>[S
+00034b00: 5441 5457 495a 4152 4420 4f46 465d 3c2f  TATWIZARD OFF]</
+00034b10: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
+00034b20: 093c 2f6c 616e 673e 0d0a 0909 093c 2f76  .</lang>.....</v
+00034b30: 6572 7369 6f6e 3e0d 0a09 093c 2f74 6f6b  ersion>....</tok
+00034b40: 656e 3e0d 0a09 093c 746f 6b65 6e20 7661  en>....<token va
+00034b50: 6c75 653d 2224 3431 223e 0d0a 0909 093c  lue="$41">.....<
+00034b60: 7665 7273 696f 6e3e 0d0a 0909 0909 3c73  version>......<s
+00034b70: 696e 6365 3e0d 0a09 0909 0909 3c6d 6f64  ince>.......<mod
+00034b80: 656c 3e54 492d 3834 2b43 5345 3c2f 6d6f  el>TI-84+CSE</mo
+00034b90: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
+00034ba0: 6572 7369 6f6e 3e34 2e30 3c2f 6f73 2d76  ersion>4.0</os-v
+00034bb0: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
+00034bc0: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
+00034bd0: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
+00034be0: 6369 693d 2234 3234 4335 3534 3522 3e0d  cii="424C5545">.
+00034bf0: 0a09 0909 0909 3c64 6973 706c 6179 3e42  ......<display>B
+00034c00: 4c55 453c 2f64 6973 706c 6179 3e0d 0a09  LUE</display>...
+00034c10: 0909 0909 3c61 6363 6573 7369 626c 653e  ....<accessible>
+00034c20: 424c 5545 3c2f 6163 6365 7373 6962 6c65  BLUE</accessible
+00034c30: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+00034c40: 3e42 6c75 653c 2f76 6172 6961 6e74 3e0d  >Blue</variant>.
+00034c50: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+00034c60: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00034c70: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+00034c80: 6e20 7661 6c75 653d 2224 3432 223e 0d0a  n value="$42">..
+00034c90: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00034ca0: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00034cb0: 3c6d 6f64 656c 3e54 492d 3834 2b43 5345  <model>TI-84+CSE
+00034cc0: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
+00034cd0: 6f73 2d76 6572 7369 6f6e 3e34 2e30 3c2f  os-version>4.0</
+00034ce0: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
+00034cf0: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
+00034d00: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
+00034d10: 692d 6173 6369 693d 2235 3234 3534 3422  i-ascii="524544"
+00034d20: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
+00034d30: 3e52 4544 3c2f 6469 7370 6c61 793e 0d0a  >RED</display>..
+00034d40: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
+00034d50: 3e52 4544 3c2f 6163 6365 7373 6962 6c65  >RED</accessible
+00034d60: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+00034d70: 3e52 6564 3c2f 7661 7269 616e 743e 0d0a  >Red</variant>..
+00034d80: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00034d90: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00034da0: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00034db0: 2076 616c 7565 3d22 2434 3322 3e0d 0a09   value="$43">...
+00034dc0: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00034dd0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00034de0: 6d6f 6465 6c3e 5449 2d38 342b 4353 453c  model>TI-84+CSE<
+00034df0: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+00034e00: 732d 7665 7273 696f 6e3e 342e 303c 2f6f  s-version>4.0</o
+00034e10: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
+00034e20: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
+00034e30: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+00034e40: 2d61 7363 6969 3d22 3432 3443 3431 3433  -ascii="424C4143
+00034e50: 3442 223e 0d0a 0909 0909 093c 6469 7370  4B">.......<disp
+00034e60: 6c61 793e 424c 4143 4b3c 2f64 6973 706c  lay>BLACK</displ
+00034e70: 6179 3e0d 0a09 0909 0909 3c61 6363 6573  ay>.......<acces
+00034e80: 7369 626c 653e 424c 4143 4b3c 2f61 6363  sible>BLACK</acc
+00034e90: 6573 7369 626c 653e 0d0a 0909 0909 093c  essible>.......<
+00034ea0: 7661 7269 616e 743e 426c 6163 6b3c 2f76  variant>Black</v
+00034eb0: 6172 6961 6e74 3e0d 0a09 0909 093c 2f6c  ariant>......</l
+00034ec0: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
+00034ed0: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
+00034ee0: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
+00034ef0: 2224 3434 223e 0d0a 0909 093c 7665 7273  "$44">.....<vers
+00034f00: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
+00034f10: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
+00034f20: 492d 3834 2b43 5345 3c2f 6d6f 6465 6c3e  I-84+CSE</model>
+00034f30: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
+00034f40: 6f6e 3e34 2e30 3c2f 6f73 2d76 6572 7369  on>4.0</os-versi
+00034f50: 6f6e 3e0d 0a09 0909 093c 2f73 696e 6365  on>......</since
+00034f60: 3e0d 0a09 0909 093c 6c61 6e67 2063 6f64  >......<lang cod
+00034f70: 653d 2265 6e22 2074 692d 6173 6369 693d  e="en" ti-ascii=
+00034f80: 2234 4434 3134 3734 3534 4535 3434 3122  "4D4147454E5441"
+00034f90: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
+00034fa0: 3e4d 4147 454e 5441 3c2f 6469 7370 6c61  >MAGENTA</displa
+00034fb0: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
+00034fc0: 6962 6c65 3e4d 4147 454e 5441 3c2f 6163  ible>MAGENTA</ac
+00034fd0: 6365 7373 6962 6c65 3e0d 0a09 0909 0909  cessible>.......
+00034fe0: 3c76 6172 6961 6e74 3e4d 6167 656e 7461  <variant>Magenta
+00034ff0: 3c2f 7661 7269 616e 743e 0d0a 0909 0909  </variant>......
+00035000: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+00035010: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+00035020: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+00035030: 7565 3d22 2434 3522 3e0d 0a09 0909 3c76  ue="$45">.....<v
+00035040: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+00035050: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00035060: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
+00035070: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
+00035080: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
+00035090: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+000350a0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+000350b0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+000350c0: 6969 3d22 3437 3532 3435 3435 3445 223e  ii="475245454E">
+000350d0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+000350e0: 4752 4545 4e3c 2f64 6973 706c 6179 3e0d  GREEN</display>.
+000350f0: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+00035100: 653e 4752 4545 4e3c 2f61 6363 6573 7369  e>GREEN</accessi
+00035110: 626c 653e 0d0a 0909 0909 093c 7661 7269  ble>.......<vari
+00035120: 616e 743e 4772 6565 6e3c 2f76 6172 6961  ant>Green</varia
+00035130: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
+00035140: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
+00035150: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
+00035160: 746f 6b65 6e20 7661 6c75 653d 2224 3436  token value="$46
+00035170: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
+00035180: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
+00035190: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
+000351a0: 2b43 5345 3c2f 6d6f 6465 6c3e 0d0a 0909  +CSE</model>....
+000351b0: 0909 093c 6f73 2d76 6572 7369 6f6e 3e34  ...<os-version>4
+000351c0: 2e30 3c2f 6f73 2d76 6572 7369 6f6e 3e0d  .0</os-version>.
+000351d0: 0a09 0909 093c 2f73 696e 6365 3e0d 0a09  .....</since>...
+000351e0: 0909 093c 6c61 6e67 2063 6f64 653d 2265  ...<lang code="e
+000351f0: 6e22 2074 692d 6173 6369 693d 2234 4635  n" ti-ascii="4F5
+00035200: 3234 3134 4534 3734 3522 3e0d 0a09 0909  2414E4745">.....
+00035210: 0909 3c64 6973 706c 6179 3e4f 5241 4e47  ..<display>ORANG
+00035220: 453c 2f64 6973 706c 6179 3e0d 0a09 0909  E</display>.....
+00035230: 0909 3c61 6363 6573 7369 626c 653e 4f52  ..<accessible>OR
+00035240: 414e 4745 3c2f 6163 6365 7373 6962 6c65  ANGE</accessible
+00035250: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+00035260: 3e4f 7261 6e67 653c 2f76 6172 6961 6e74  >Orange</variant
+00035270: 3e0d 0a09 0909 093c 2f6c 616e 673e 0d0a  >......</lang>..
+00035280: 0909 093c 2f76 6572 7369 6f6e 3e0d 0a09  ...</version>...
+00035290: 093c 2f74 6f6b 656e 3e0d 0a09 093c 746f  .</token>....<to
+000352a0: 6b65 6e20 7661 6c75 653d 2224 3437 223e  ken value="$47">
+000352b0: 0d0a 0909 093c 7665 7273 696f 6e3e 0d0a  .....<version>..
+000352c0: 0909 0909 3c73 696e 6365 3e0d 0a09 0909  ....<since>.....
+000352d0: 0909 3c6d 6f64 656c 3e54 492d 3834 2b43  ..<model>TI-84+C
+000352e0: 5345 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  SE</model>......
+000352f0: 093c 6f73 2d76 6572 7369 6f6e 3e34 2e30  .<os-version>4.0
+00035300: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
+00035310: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
+00035320: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
+00035330: 2074 692d 6173 6369 693d 2234 3235 3234   ti-ascii="42524
+00035340: 4635 3734 4522 3e0d 0a09 0909 0909 3c64  F574E">.......<d
+00035350: 6973 706c 6179 3e42 524f 574e 3c2f 6469  isplay>BROWN</di
+00035360: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00035370: 6365 7373 6962 6c65 3e42 524f 574e 3c2f  cessible>BROWN</
+00035380: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
+00035390: 0909 3c76 6172 6961 6e74 3e42 726f 776e  ..<variant>Brown
+000353a0: 3c2f 7661 7269 616e 743e 0d0a 0909 0909  </variant>......
+000353b0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+000353c0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+000353d0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+000353e0: 7565 3d22 2434 3822 3e0d 0a09 0909 3c76  ue="$48">.....<v
+000353f0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+00035400: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00035410: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
+00035420: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
+00035430: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
+00035440: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+00035450: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+00035460: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+00035470: 6969 3d22 3445 3431 3536 3539 223e 0d0a  ii="4E415659">..
+00035480: 0909 0909 093c 6469 7370 6c61 793e 4e41  .....<display>NA
+00035490: 5659 3c2f 6469 7370 6c61 793e 0d0a 0909  VY</display>....
+000354a0: 0909 093c 6163 6365 7373 6962 6c65 3e4e  ...<accessible>N
+000354b0: 4156 593c 2f61 6363 6573 7369 626c 653e  AVY</accessible>
+000354c0: 0d0a 0909 0909 093c 7661 7269 616e 743e  .......<variant>
+000354d0: 4e61 7679 3c2f 7661 7269 616e 743e 0d0a  Navy</variant>..
+000354e0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+000354f0: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00035500: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00035510: 2076 616c 7565 3d22 2434 3922 3e0d 0a09   value="$49">...
+00035520: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00035530: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00035540: 6d6f 6465 6c3e 5449 2d38 342b 4353 453c  model>TI-84+CSE<
+00035550: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+00035560: 732d 7665 7273 696f 6e3e 342e 303c 2f6f  s-version>4.0</o
+00035570: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
+00035580: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
+00035590: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+000355a0: 2d61 7363 6969 3d22 3443 3534 3432 3443  -ascii="4C54424C
+000355b0: 3535 3435 223e 0d0a 0909 0909 093c 6469  5545">.......<di
+000355c0: 7370 6c61 793e 4c54 424c 5545 3c2f 6469  splay>LTBLUE</di
+000355d0: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+000355e0: 6365 7373 6962 6c65 3e4c 5442 4c55 453c  cessible>LTBLUE<
+000355f0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00035600: 0909 093c 7661 7269 616e 743e 4c74 426c  ...<variant>LtBl
+00035610: 7565 3c2f 7661 7269 616e 743e 0d0a 0909  ue</variant>....
+00035620: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+00035630: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+00035640: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+00035650: 616c 7565 3d22 2434 4122 3e0d 0a09 0909  alue="$4A">.....
+00035660: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+00035670: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+00035680: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
+00035690: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+000356a0: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
+000356b0: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+000356c0: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+000356d0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+000356e0: 7363 6969 3d22 3539 3435 3443 3443 3446  scii="59454C4C4F
+000356f0: 3537 223e 0d0a 0909 0909 093c 6469 7370  57">.......<disp
+00035700: 6c61 793e 5945 4c4c 4f57 3c2f 6469 7370  lay>YELLOW</disp
+00035710: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+00035720: 7373 6962 6c65 3e59 454c 4c4f 573c 2f61  ssible>YELLOW</a
+00035730: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+00035740: 093c 7661 7269 616e 743e 5965 6c6c 6f77  .<variant>Yellow
+00035750: 3c2f 7661 7269 616e 743e 0d0a 0909 0909  </variant>......
+00035760: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+00035770: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+00035780: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+00035790: 7565 3d22 2434 4222 3e0d 0a09 0909 3c76  ue="$4B">.....<v
+000357a0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+000357b0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+000357c0: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
+000357d0: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
+000357e0: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
+000357f0: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+00035800: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+00035810: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+00035820: 6969 3d22 3537 3438 3439 3534 3435 223e  ii="5748495445">
+00035830: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00035840: 5748 4954 453c 2f64 6973 706c 6179 3e0d  WHITE</display>.
+00035850: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+00035860: 653e 5748 4954 453c 2f61 6363 6573 7369  e>WHITE</accessi
+00035870: 626c 653e 0d0a 0909 0909 093c 7661 7269  ble>.......<vari
+00035880: 616e 743e 5768 6974 653c 2f76 6172 6961  ant>White</varia
+00035890: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
+000358a0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
+000358b0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
+000358c0: 746f 6b65 6e20 7661 6c75 653d 2224 3443  token value="$4C
+000358d0: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
+000358e0: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
+000358f0: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
+00035900: 2b43 5345 3c2f 6d6f 6465 6c3e 0d0a 0909  +CSE</model>....
+00035910: 0909 093c 6f73 2d76 6572 7369 6f6e 3e34  ...<os-version>4
+00035920: 2e30 3c2f 6f73 2d76 6572 7369 6f6e 3e0d  .0</os-version>.
+00035930: 0a09 0909 093c 2f73 696e 6365 3e0d 0a09  .....</since>...
+00035940: 0909 093c 6c61 6e67 2063 6f64 653d 2265  ...<lang code="e
+00035950: 6e22 2074 692d 6173 6369 693d 2234 4335  n" ti-ascii="4C5
+00035960: 3434 3735 3234 3135 3922 3e0d 0a09 0909  447524159">.....
+00035970: 0909 3c64 6973 706c 6179 3e4c 5447 5241  ..<display>LTGRA
+00035980: 593c 2f64 6973 706c 6179 3e0d 0a09 0909  Y</display>.....
+00035990: 0909 3c61 6363 6573 7369 626c 653e 4c54  ..<accessible>LT
+000359a0: 4752 4159 3c2f 6163 6365 7373 6962 6c65  GRAY</accessible
+000359b0: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+000359c0: 3e4c 7447 7261 793c 2f76 6172 6961 6e74  >LtGray</variant
+000359d0: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+000359e0: 3e4c 5447 5245 593c 2f76 6172 6961 6e74  >LTGREY</variant
+000359f0: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+00035a00: 3e4c 7447 7265 793c 2f76 6172 6961 6e74  >LtGrey</variant
+00035a10: 3e0d 0a09 0909 093c 2f6c 616e 673e 0d0a  >......</lang>..
+00035a20: 0909 093c 2f76 6572 7369 6f6e 3e0d 0a09  ...</version>...
+00035a30: 093c 2f74 6f6b 656e 3e0d 0a09 093c 746f  .</token>....<to
+00035a40: 6b65 6e20 7661 6c75 653d 2224 3444 223e  ken value="$4D">
+00035a50: 0d0a 0909 093c 7665 7273 696f 6e3e 0d0a  .....<version>..
+00035a60: 0909 0909 3c73 696e 6365 3e0d 0a09 0909  ....<since>.....
+00035a70: 0909 3c6d 6f64 656c 3e54 492d 3834 2b43  ..<model>TI-84+C
+00035a80: 5345 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  SE</model>......
+00035a90: 093c 6f73 2d76 6572 7369 6f6e 3e34 2e30  .<os-version>4.0
+00035aa0: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
+00035ab0: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
+00035ac0: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
+00035ad0: 2074 692d 6173 6369 693d 2234 4434 3534   ti-ascii="4D454
+00035ae0: 3434 3735 3234 3135 3922 3e0d 0a09 0909  447524159">.....
+00035af0: 0909 3c64 6973 706c 6179 3e4d 4544 4752  ..<display>MEDGR
+00035b00: 4159 3c2f 6469 7370 6c61 793e 0d0a 0909  AY</display>....
+00035b10: 0909 093c 6163 6365 7373 6962 6c65 3e4d  ...<accessible>M
+00035b20: 4544 4752 4159 3c2f 6163 6365 7373 6962  EDGRAY</accessib
+00035b30: 6c65 3e0d 0a09 0909 0909 3c76 6172 6961  le>.......<varia
+00035b40: 6e74 3e4d 6564 4772 6179 3c2f 7661 7269  nt>MedGray</vari
+00035b50: 616e 743e 0d0a 0909 0909 093c 7661 7269  ant>.......<vari
+00035b60: 616e 743e 4d45 4447 5245 593c 2f76 6172  ant>MEDGREY</var
+00035b70: 6961 6e74 3e0d 0a09 0909 0909 3c76 6172  iant>.......<var
+00035b80: 6961 6e74 3e4d 6564 4772 6579 3c2f 7661  iant>MedGrey</va
+00035b90: 7269 616e 743e 0d0a 0909 0909 3c2f 6c61  riant>......</la
+00035ba0: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
+00035bb0: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
+00035bc0: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+00035bd0: 2434 4522 3e0d 0a09 0909 3c76 6572 7369  $4E">.....<versi
+00035be0: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
+00035bf0: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
+00035c00: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
+00035c10: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+00035c20: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
+00035c30: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
+00035c40: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
+00035c50: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+00035c60: 3437 3532 3431 3539 223e 0d0a 0909 0909  47524159">......
+00035c70: 093c 6469 7370 6c61 793e 4752 4159 3c2f  .<display>GRAY</
+00035c80: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
+00035c90: 6163 6365 7373 6962 6c65 3e47 5241 593c  accessible>GRAY<
+00035ca0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00035cb0: 0909 093c 7661 7269 616e 743e 4772 6179  ...<variant>Gray
+00035cc0: 3c2f 7661 7269 616e 743e 0d0a 0909 0909  </variant>......
+00035cd0: 093c 7661 7269 616e 743e 4752 4559 3c2f  .<variant>GREY</
+00035ce0: 7661 7269 616e 743e 0d0a 0909 0909 093c  variant>.......<
+00035cf0: 7661 7269 616e 743e 4772 6579 3c2f 7661  variant>Grey</va
+00035d00: 7269 616e 743e 0d0a 0909 0909 3c2f 6c61  riant>......</la
+00035d10: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
+00035d20: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
+00035d30: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+00035d40: 2434 4622 3e0d 0a09 0909 3c76 6572 7369  $4F">.....<versi
+00035d50: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
+00035d60: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
+00035d70: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
+00035d80: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+00035d90: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
+00035da0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
+00035db0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
+00035dc0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+00035dd0: 3434 3431 3532 3442 3437 3532 3431 3539  4441524B47524159
+00035de0: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00035df0: 793e 4441 524b 4752 4159 3c2f 6469 7370  y>DARKGRAY</disp
+00035e00: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+00035e10: 7373 6962 6c65 3e44 4152 4b47 5241 593c  ssible>DARKGRAY<
+00035e20: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00035e30: 0909 093c 7661 7269 616e 743e 4461 726b  ...<variant>Dark
+00035e40: 4772 6179 3c2f 7661 7269 616e 743e 0d0a  Gray</variant>..
+00035e50: 0909 0909 093c 7661 7269 616e 743e 4441  .....<variant>DA
+00035e60: 524b 4752 4559 3c2f 7661 7269 616e 743e  RKGREY</variant>
+00035e70: 0d0a 0909 0909 093c 7661 7269 616e 743e  .......<variant>
+00035e80: 4461 726b 4772 6579 3c2f 7661 7269 616e  DarkGrey</varian
+00035e90: 743e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  t>......</lang>.
+00035ea0: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+00035eb0: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+00035ec0: 6f6b 656e 2076 616c 7565 3d22 2435 3022  oken value="$50"
+00035ed0: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00035ee0: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+00035ef0: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+00035f00: 4353 453c 2f6d 6f64 656c 3e0d 0a09 0909  CSE</model>.....
+00035f10: 0909 3c6f 732d 7665 7273 696f 6e3e 342e  ..<os-version>4.
+00035f20: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
+00035f30: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
+00035f40: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00035f50: 2220 7469 2d61 7363 6969 3d22 3439 3644  " ti-ascii="496D
+00035f60: 3631 3637 3635 3331 223e 0d0a 0909 0909  61676531">......
+00035f70: 093c 6469 7370 6c61 793e 496d 6167 6531  .<display>Image1
+00035f80: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00035f90: 093c 6163 6365 7373 6962 6c65 3e49 6d61  .<accessible>Ima
+00035fa0: 6765 313c 2f61 6363 6573 7369 626c 653e  ge1</accessible>
+00035fb0: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
+00035fc0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
+00035fd0: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
+00035fe0: 656e 2076 616c 7565 3d22 2435 3122 3e0d  en value="$51">.
+00035ff0: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
+00036000: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
+00036010: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
+00036020: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
+00036030: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
+00036040: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00036050: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00036060: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00036070: 7469 2d61 7363 6969 3d22 3439 3644 3631  ti-ascii="496D61
+00036080: 3637 3635 3332 223e 0d0a 0909 0909 093c  676532">.......<
+00036090: 6469 7370 6c61 793e 496d 6167 6532 3c2f  display>Image2</
+000360a0: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
+000360b0: 6163 6365 7373 6962 6c65 3e49 6d61 6765  accessible>Image
+000360c0: 323c 2f61 6363 6573 7369 626c 653e 0d0a  2</accessible>..
+000360d0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+000360e0: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+000360f0: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00036100: 2076 616c 7565 3d22 2435 3222 3e0d 0a09   value="$52">...
+00036110: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00036120: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00036130: 6d6f 6465 6c3e 5449 2d38 342b 4353 453c  model>TI-84+CSE<
+00036140: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+00036150: 732d 7665 7273 696f 6e3e 342e 303c 2f6f  s-version>4.0</o
+00036160: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
+00036170: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
+00036180: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+00036190: 2d61 7363 6969 3d22 3439 3644 3631 3637  -ascii="496D6167
+000361a0: 3635 3333 223e 0d0a 0909 0909 093c 6469  6533">.......<di
+000361b0: 7370 6c61 793e 496d 6167 6533 3c2f 6469  splay>Image3</di
+000361c0: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+000361d0: 6365 7373 6962 6c65 3e49 6d61 6765 333c  cessible>Image3<
+000361e0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+000361f0: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+00036200: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+00036210: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+00036220: 616c 7565 3d22 2435 3322 3e0d 0a09 0909  alue="$53">.....
+00036230: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+00036240: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+00036250: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
+00036260: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+00036270: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
+00036280: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+00036290: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+000362a0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+000362b0: 7363 6969 3d22 3439 3644 3631 3637 3635  scii="496D616765
+000362c0: 3334 223e 0d0a 0909 0909 093c 6469 7370  34">.......<disp
+000362d0: 6c61 793e 496d 6167 6534 3c2f 6469 7370  lay>Image4</disp
+000362e0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+000362f0: 7373 6962 6c65 3e49 6d61 6765 343c 2f61  ssible>Image4</a
+00036300: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+00036310: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+00036320: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+00036330: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+00036340: 7565 3d22 2435 3422 3e0d 0a09 0909 3c76  ue="$54">.....<v
+00036350: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+00036360: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00036370: 6c3e 5449 2d38 342b 4353 453c 2f6d 6f64  l>TI-84+CSE</mod
+00036380: 656c 3e0d 0a09 0909 0909 3c6f 732d 7665  el>.......<os-ve
+00036390: 7273 696f 6e3e 342e 303c 2f6f 732d 7665  rsion>4.0</os-ve
+000363a0: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+000363b0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+000363c0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+000363d0: 6969 3d22 3439 3644 3631 3637 3635 3335  ii="496D61676535
+000363e0: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+000363f0: 793e 496d 6167 6535 3c2f 6469 7370 6c61  y>Image5</displa
+00036400: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
+00036410: 6962 6c65 3e49 6d61 6765 353c 2f61 6363  ible>Image5</acc
+00036420: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
+00036430: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
+00036440: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
+00036450: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
+00036460: 3d22 2435 3522 3e0d 0a09 0909 3c76 6572  ="$55">.....<ver
+00036470: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
+00036480: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
+00036490: 5449 2d38 342b 4353 453c 2f6d 6f64 656c  TI-84+CSE</model
+000364a0: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
+000364b0: 696f 6e3e 342e 303c 2f6f 732d 7665 7273  ion>4.0</os-vers
+000364c0: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
+000364d0: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
+000364e0: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
+000364f0: 3d22 3439 3644 3631 3637 3635 3336 223e  ="496D61676536">
+00036500: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00036510: 496d 6167 6536 3c2f 6469 7370 6c61 793e  Image6</display>
+00036520: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+00036530: 6c65 3e49 6d61 6765 363c 2f61 6363 6573  le>Image6</acces
+00036540: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
+00036550: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
+00036560: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
+00036570: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+00036580: 2435 3622 3e0d 0a09 0909 3c76 6572 7369  $56">.....<versi
+00036590: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
+000365a0: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
+000365b0: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
+000365c0: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+000365d0: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
+000365e0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
+000365f0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
+00036600: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+00036610: 3439 3644 3631 3637 3635 3337 223e 0d0a  496D61676537">..
+00036620: 0909 0909 093c 6469 7370 6c61 793e 496d  .....<display>Im
+00036630: 6167 6537 3c2f 6469 7370 6c61 793e 0d0a  age7</display>..
+00036640: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
+00036650: 3e49 6d61 6765 373c 2f61 6363 6573 7369  >Image7</accessi
+00036660: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
+00036670: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
+00036680: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
+00036690: 3c74 6f6b 656e 2076 616c 7565 3d22 2435  <token value="$5
+000366a0: 3722 3e0d 0a09 0909 3c76 6572 7369 6f6e  7">.....<version
+000366b0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
+000366c0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
+000366d0: 342b 4353 453c 2f6d 6f64 656c 3e0d 0a09  4+CSE</model>...
+000366e0: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
+000366f0: 342e 303c 2f6f 732d 7665 7273 696f 6e3e  4.0</os-version>
+00036700: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
+00036710: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
+00036720: 656e 2220 7469 2d61 7363 6969 3d22 3439  en" ti-ascii="49
+00036730: 3644 3631 3637 3635 3338 223e 0d0a 0909  6D61676538">....
+00036740: 0909 093c 6469 7370 6c61 793e 496d 6167  ...<display>Imag
+00036750: 6538 3c2f 6469 7370 6c61 793e 0d0a 0909  e8</display>....
+00036760: 0909 093c 6163 6365 7373 6962 6c65 3e49  ...<accessible>I
+00036770: 6d61 6765 383c 2f61 6363 6573 7369 626c  mage8</accessibl
+00036780: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00036790: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+000367a0: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+000367b0: 6f6b 656e 2076 616c 7565 3d22 2435 3822  oken value="$58"
+000367c0: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+000367d0: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+000367e0: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+000367f0: 4353 453c 2f6d 6f64 656c 3e0d 0a09 0909  CSE</model>.....
+00036800: 0909 3c6f 732d 7665 7273 696f 6e3e 342e  ..<os-version>4.
+00036810: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
+00036820: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
+00036830: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00036840: 2220 7469 2d61 7363 6969 3d22 3439 3644  " ti-ascii="496D
+00036850: 3631 3637 3635 3339 223e 0d0a 0909 0909  61676539">......
+00036860: 093c 6469 7370 6c61 793e 496d 6167 6539  .<display>Image9
+00036870: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00036880: 093c 6163 6365 7373 6962 6c65 3e49 6d61  .<accessible>Ima
+00036890: 6765 393c 2f61 6363 6573 7369 626c 653e  ge9</accessible>
+000368a0: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
+000368b0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
+000368c0: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
+000368d0: 656e 2076 616c 7565 3d22 2435 3922 3e0d  en value="$59">.
+000368e0: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
+000368f0: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
+00036900: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
+00036910: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
+00036920: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
+00036930: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00036940: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00036950: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00036960: 7469 2d61 7363 6969 3d22 3439 3644 3631  ti-ascii="496D61
+00036970: 3637 3635 3330 223e 0d0a 0909 0909 093c  676530">.......<
+00036980: 6469 7370 6c61 793e 496d 6167 6530 3c2f  display>Image0</
+00036990: 6469 7370 6c61 793e 0d0a 0909 0909 093c  display>.......<
+000369a0: 6163 6365 7373 6962 6c65 3e49 6d61 6765  accessible>Image
+000369b0: 303c 2f61 6363 6573 7369 626c 653e 0d0a  0</accessible>..
+000369c0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+000369d0: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+000369e0: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+000369f0: 2076 616c 7565 3d22 2435 4122 3e0d 0a09   value="$5A">...
+00036a00: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00036a10: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00036a20: 6d6f 6465 6c3e 5449 2d38 342b 4353 453c  model>TI-84+CSE<
+00036a30: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+00036a40: 732d 7665 7273 696f 6e3e 342e 303c 2f6f  s-version>4.0</o
+00036a50: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
+00036a60: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
+00036a70: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+00036a80: 2d61 7363 6969 3d22 3437 3732 3639 3634  -ascii="47726964
+00036a90: 3443 3639 3645 3635 3230 223e 0d0a 0909  4C696E6520">....
+00036aa0: 0909 093c 6469 7370 6c61 793e 4772 6964  ...<display>Grid
+00036ab0: 4c69 6e65 2623 3033 323b 3c2f 6469 7370  Line&#032;</disp
+00036ac0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+00036ad0: 7373 6962 6c65 3e47 7269 644c 696e 6526  ssible>GridLine&
+00036ae0: 2330 3332 3b3c 2f61 6363 6573 7369 626c  #032;</accessibl
+00036af0: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00036b00: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+00036b10: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+00036b20: 6f6b 656e 2076 616c 7565 3d22 2435 4222  oken value="$5B"
+00036b30: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00036b40: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+00036b50: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+00036b60: 4353 453c 2f6d 6f64 656c 3e0d 0a09 0909  CSE</model>.....
+00036b70: 0909 3c6f 732d 7665 7273 696f 6e3e 342e  ..<os-version>4.
+00036b80: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
+00036b90: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
+00036ba0: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00036bb0: 2220 7469 2d61 7363 6969 3d22 3432 3631  " ti-ascii="4261
+00036bc0: 3633 3642 3637 3732 3646 3735 3645 3634  636B67726F756E64
+00036bd0: 3446 3645 3230 223e 0d0a 0909 0909 093c  4F6E20">.......<
+00036be0: 6469 7370 6c61 793e 4261 636b 6772 6f75  display>Backgrou
+00036bf0: 6e64 4f6e 2623 3033 323b 3c2f 6469 7370  ndOn&#032;</disp
+00036c00: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+00036c10: 7373 6962 6c65 3e42 6163 6b67 726f 756e  ssible>Backgroun
+00036c20: 644f 6e26 2330 3332 3b3c 2f61 6363 6573  dOn&#032;</acces
+00036c30: 7369 626c 653e 0d0a 0909 0909 3c2f 6c61  sible>......</la
+00036c40: 6e67 3e0d 0a09 0909 3c2f 7665 7273 696f  ng>.....</versio
+00036c50: 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a  n>....</token>..
+00036c60: 0909 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+00036c70: 2436 3422 3e0d 0a09 0909 3c76 6572 7369  $64">.....<versi
+00036c80: 6f6e 3e0d 0a09 0909 093c 7369 6e63 653e  on>......<since>
+00036c90: 0d0a 0909 0909 093c 6d6f 6465 6c3e 5449  .......<model>TI
+00036ca0: 2d38 342b 4353 453c 2f6d 6f64 656c 3e0d  -84+CSE</model>.
+00036cb0: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+00036cc0: 6e3e 342e 303c 2f6f 732d 7665 7273 696f  n>4.0</os-versio
+00036cd0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
+00036ce0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
+00036cf0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+00036d00: 3432 3631 3633 3642 3637 3732 3646 3735  4261636B67726F75
+00036d10: 3645 3634 3446 3636 3636 223e 0d0a 0909  6E644F6666">....
+00036d20: 0909 093c 6469 7370 6c61 793e 4261 636b  ...<display>Back
+00036d30: 6772 6f75 6e64 4f66 663c 2f64 6973 706c  groundOff</displ
+00036d40: 6179 3e0d 0a09 0909 0909 3c61 6363 6573  ay>.......<acces
+00036d50: 7369 626c 653e 4261 636b 6772 6f75 6e64  sible>Background
+00036d60: 4f66 663c 2f61 6363 6573 7369 626c 653e  Off</accessible>
+00036d70: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
+00036d80: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
+00036d90: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
+00036da0: 656e 2076 616c 7565 3d22 2436 3522 3e0d  en value="$65">.
+00036db0: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
+00036dc0: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
+00036dd0: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
+00036de0: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
+00036df0: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
+00036e00: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00036e10: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00036e20: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00036e30: 7469 2d61 7363 6969 3d22 3437 3732 3631  ti-ascii="477261
+00036e40: 3730 3638 3433 3646 3643 3646 3732 3238  7068436F6C6F7228
+00036e50: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00036e60: 793e 4772 6170 6843 6f6c 6f72 283c 2f64  y>GraphColor(</d
+00036e70: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
+00036e80: 6363 6573 7369 626c 653e 4772 6170 6843  ccessible>GraphC
+00036e90: 6f6c 6f72 283c 2f61 6363 6573 7369 626c  olor(</accessibl
+00036ea0: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00036eb0: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+00036ec0: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+00036ed0: 6f6b 656e 2076 616c 7565 3d22 2436 3622  oken value="$66"
+00036ee0: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00036ef0: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+00036f00: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+00036f10: 4353 453c 2f6d 6f64 656c 3e0d 0a09 0909  CSE</model>.....
+00036f20: 0909 3c6f 732d 7665 7273 696f 6e3e 342e  ..<os-version>4.
+00036f30: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
+00036f40: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
+00036f50: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00036f60: 2220 7469 2d61 7363 6969 3d22 3531 3735  " ti-ascii="5175
+00036f70: 3639 3633 3642 3530 3643 3646 3734 3236  69636B506C6F7426
+00036f80: 3436 3639 3734 3244 3435 3531 223e 0d0a  4669742D4551">..
+00036f90: 0909 0909 093c 6469 7370 6c61 793e 5175  .....<display>Qu
+00036fa0: 6963 6b50 6c6f 7426 616d 703b 4669 742d  ickPlot&amp;Fit-
+00036fb0: 4551 3c2f 6469 7370 6c61 793e 0d0a 0909  EQ</display>....
+00036fc0: 0909 093c 6163 6365 7373 6962 6c65 3e51  ...<accessible>Q
+00036fd0: 7569 636b 506c 6f74 2661 6d70 3b46 6974  uickPlot&amp;Fit
+00036fe0: 2d45 513c 2f61 6363 6573 7369 626c 653e  -EQ</accessible>
+00036ff0: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
+00037000: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
+00037010: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
+00037020: 656e 2076 616c 7565 3d22 2436 3722 3e0d  en value="$67">.
+00037030: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
+00037040: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
+00037050: 093c 6d6f 6465 6c3e 5449 2d38 342b 4353  .<model>TI-84+CS
+00037060: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
+00037070: 3c6f 732d 7665 7273 696f 6e3e 342e 303c  <os-version>4.0<
+00037080: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00037090: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+000370a0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+000370b0: 7469 2d61 7363 6969 3d22 3534 3635 3738  ti-ascii="546578
+000370c0: 3734 3433 3646 3643 3646 3732 3238 223e  74436F6C6F7228">
+000370d0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+000370e0: 5465 7874 436f 6c6f 7228 3c2f 6469 7370  TextColor(</disp
+000370f0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+00037100: 7373 6962 6c65 3e54 6578 7443 6f6c 6f72  ssible>TextColor
+00037110: 283c 2f61 6363 6573 7369 626c 653e 0d0a  (</accessible>..
+00037120: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00037130: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00037140: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00037150: 2076 616c 7565 3d22 2436 3822 3e0d 0a09   value="$68">...
+00037160: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00037170: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00037180: 6d6f 6465 6c3e 5449 2d38 342b 4353 453c  model>TI-84+CSE<
+00037190: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+000371a0: 732d 7665 7273 696f 6e3e 342e 303c 2f6f  s-version>4.0</o
+000371b0: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
+000371c0: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
+000371d0: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+000371e0: 2d61 7363 6969 3d22 3431 3733 3644 3338  -ascii="41736D38
+000371f0: 3334 3433 3530 3732 3637 3644 223e 0d0a  34435072676D">..
+00037200: 0909 0909 093c 6469 7370 6c61 793e 4173  .....<display>As
+00037210: 6d38 3443 5072 676d 3c2f 6469 7370 6c61  m84CPrgm</displa
+00037220: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
+00037230: 6962 6c65 3e41 736d 3834 4350 7267 6d3c  ible>Asm84CPrgm<
+00037240: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00037250: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+00037260: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+00037270: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+00037280: 616c 7565 3d22 2436 4122 3e0d 0a09 0909  alue="$6A">.....
+00037290: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+000372a0: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+000372b0: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
+000372c0: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+000372d0: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
+000372e0: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+000372f0: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+00037300: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+00037310: 7363 6969 3d22 3434 3635 3734 3635 3633  scii="4465746563
+00037320: 3734 3431 3733 3739 3644 3446 3645 223e  744173796D4F6E">
+00037330: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00037340: 4465 7465 6374 4173 796d 4f6e 3c2f 6469  DetectAsymOn</di
+00037350: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00037360: 6365 7373 6962 6c65 3e44 6574 6563 7441  cessible>DetectA
+00037370: 7379 6d4f 6e3c 2f61 6363 6573 7369 626c  symOn</accessibl
+00037380: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00037390: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+000373a0: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+000373b0: 6f6b 656e 2076 616c 7565 3d22 2436 4222  oken value="$6B"
+000373c0: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+000373d0: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+000373e0: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+000373f0: 4353 453c 2f6d 6f64 656c 3e0d 0a09 0909  CSE</model>.....
+00037400: 0909 3c6f 732d 7665 7273 696f 6e3e 342e  ..<os-version>4.
+00037410: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
+00037420: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
+00037430: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00037440: 2220 7469 2d61 7363 6969 3d22 3434 3635  " ti-ascii="4465
+00037450: 3734 3635 3633 3734 3431 3733 3739 3644  746563744173796D
+00037460: 3446 3636 3636 223e 0d0a 0909 0909 093c  4F6666">.......<
+00037470: 6469 7370 6c61 793e 4465 7465 6374 4173  display>DetectAs
+00037480: 796d 4f66 663c 2f64 6973 706c 6179 3e0d  ymOff</display>.
+00037490: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+000374a0: 653e 4465 7465 6374 4173 796d 4f66 663c  e>DetectAsymOff<
+000374b0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+000374c0: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+000374d0: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+000374e0: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+000374f0: 616c 7565 3d22 2436 4322 3e0d 0a09 0909  alue="$6C">.....
+00037500: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+00037510: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+00037520: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
+00037530: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+00037540: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
+00037550: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+00037560: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+00037570: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+00037580: 7363 6969 3d22 3432 3646 3732 3634 3635  scii="426F726465
+00037590: 3732 3433 3646 3643 3646 3732 3230 223e  72436F6C6F7220">
+000375a0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+000375b0: 426f 7264 6572 436f 6c6f 7226 2330 3332  BorderColor&#032
+000375c0: 3b3c 2f64 6973 706c 6179 3e0d 0a09 0909  ;</display>.....
+000375d0: 0909 3c61 6363 6573 7369 626c 653e 426f  ..<accessible>Bo
+000375e0: 7264 6572 436f 6c6f 7226 2330 3332 3b3c  rderColor&#032;<
+000375f0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00037600: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+00037610: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+00037620: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+00037630: 616c 7565 3d22 2437 3322 3e0d 0a09 0909  alue="$73">.....
+00037640: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+00037650: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+00037660: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
+00037670: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+00037680: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
+00037690: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+000376a0: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+000376b0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+000376c0: 7363 6969 3d22 4639 223e 0d0a 0909 0909  scii="F9">......
+000376d0: 093c 6469 7370 6c61 793e 2e3c 2f64 6973  .<display>.</dis
+000376e0: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
+000376f0: 6573 7369 626c 653e 706c 6f74 7469 6e79  essible>plottiny
+00037700: 646f 743c 2f61 6363 6573 7369 626c 653e  dot</accessible>
+00037710: 0d0a 0909 0909 093c 7661 7269 616e 743e  .......<variant>
+00037720: c2b7 3c2f 7661 7269 616e 743e 0d0a 0909  ..</variant>....
+00037730: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+00037740: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+00037750: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+00037760: 616c 7565 3d22 2437 3422 3e0d 0a09 0909  alue="$74">.....
+00037770: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+00037780: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+00037790: 6465 6c3e 5449 2d38 342b 4353 453c 2f6d  del>TI-84+CSE</m
+000377a0: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+000377b0: 7665 7273 696f 6e3e 342e 303c 2f6f 732d  version>4.0</os-
+000377c0: 7665 7273 696f 6e3e 0d0a 0909 0909 3c2f  version>......</
+000377d0: 7369 6e63 653e 0d0a 0909 0909 3c6c 616e  since>......<lan
+000377e0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+000377f0: 7363 6969 3d22 3534 3638 3639 3645 223e  scii="5468696E">
+00037800: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+00037810: 5468 696e 3c2f 6469 7370 6c61 793e 0d0a  Thin</display>..
+00037820: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
+00037830: 3e54 6869 6e3c 2f61 6363 6573 7369 626c  >Thin</accessibl
+00037840: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00037850: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+00037860: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+00037870: 6f6b 656e 2076 616c 7565 3d22 2437 3522  oken value="$75"
+00037880: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00037890: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+000378a0: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+000378b0: 4353 453c 2f6d 6f64 656c 3e0d 0a09 0909  CSE</model>.....
+000378c0: 0909 3c6f 732d 7665 7273 696f 6e3e 342e  ..<os-version>4.
+000378d0: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
+000378e0: 0909 0909 3c2f 7369 6e63 653e 0d0a 0909  ....</since>....
+000378f0: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00037900: 2220 7469 2d61 7363 6969 3d22 3434 3646  " ti-ascii="446F
+00037910: 3734 3244 3534 3638 3639 3645 223e 0d0a  742D5468696E">..
+00037920: 0909 0909 093c 6469 7370 6c61 793e 446f  .....<display>Do
+00037930: 742d 5468 696e 3c2f 6469 7370 6c61 793e  t-Thin</display>
+00037940: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+00037950: 6c65 3e44 6f74 2d54 6869 6e3c 2f61 6363  le>Dot-Thin</acc
+00037960: 6573 7369 626c 653e 0d0a 0909 0909 3c2f  essible>......</
+00037970: 6c61 6e67 3e0d 0a09 0909 3c2f 7665 7273  lang>.....</vers
+00037980: 696f 6e3e 0d0a 0909 3c2f 746f 6b65 6e3e  ion>....</token>
+00037990: 0d0a 0909 3c74 6f6b 656e 2076 616c 7565  ....<token value
+000379a0: 3d22 2437 3922 3e0d 0a09 0909 3c76 6572  ="$79">.....<ver
+000379b0: 7369 6f6e 3e0d 0a09 0909 093c 7369 6e63  sion>......<sinc
+000379c0: 653e 0d0a 0909 0909 093c 6d6f 6465 6c3e  e>.......<model>
+000379d0: 5449 2d38 342b 4345 3c2f 6d6f 6465 6c3e  TI-84+CE</model>
+000379e0: 0d0a 0909 0909 093c 6f73 2d76 6572 7369  .......<os-versi
+000379f0: 6f6e 3e35 2e30 2e30 3c2f 6f73 2d76 6572  on>5.0.0</os-ver
+00037a00: 7369 6f6e 3e0d 0a09 0909 093c 2f73 696e  sion>......</sin
+00037a10: 6365 3e0d 0a09 0909 093c 6c61 6e67 2063  ce>......<lang c
+00037a20: 6f64 653d 2265 6e22 2074 692d 6173 6369  ode="en" ti-asci
+00037a30: 693d 2235 3036 4337 3935 3336 4436 4337  i="506C79536D6C7
+00037a40: 3433 3222 3e0d 0a09 0909 0909 3c64 6973  432">.......<dis
+00037a50: 706c 6179 3e50 6c79 536d 6c74 323c 2f64  play>PlySmlt2</d
+00037a60: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
+00037a70: 6363 6573 7369 626c 653e 506c 7953 6d6c  ccessible>PlySml
+00037a80: 7432 3c2f 6163 6365 7373 6962 6c65 3e0d  t2</accessible>.
+00037a90: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+00037aa0: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00037ab0: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+00037ac0: 6e20 7661 6c75 653d 2224 3741 223e 0d0a  n value="$7A">..
+00037ad0: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00037ae0: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00037af0: 3c6d 6f64 656c 3e54 492d 3834 2b43 453c  <model>TI-84+CE<
+00037b00: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+00037b10: 732d 7665 7273 696f 6e3e 352e 302e 303c  s-version>5.0.0<
+00037b20: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00037b30: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00037b40: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00037b50: 7469 2d61 7363 6969 3d22 3431 3733 3644  ti-ascii="41736D
+00037b60: 3338 3334 3433 3435 3530 3732 3637 3644  383443455072676D
+00037b70: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00037b80: 793e 4173 6d38 3443 4550 7267 6d3c 2f64  y>Asm84CEPrgm</d
+00037b90: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
+00037ba0: 6363 6573 7369 626c 653e 4173 6d38 3443  ccessible>Asm84C
+00037bb0: 4550 7267 6d3c 2f61 6363 6573 7369 626c  EPrgm</accessibl
+00037bc0: 653e 0d0a 0909 0909 3c2f 6c61 6e67 3e0d  e>......</lang>.
+00037bd0: 0a09 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+00037be0: 0909 3c2f 746f 6b65 6e3e 0d0a 0909 3c74  ..</token>....<t
+00037bf0: 6f6b 656e 2076 616c 7565 3d22 2438 3122  oken value="$81"
+00037c00: 3e0d 0a09 0909 3c76 6572 7369 6f6e 3e0d  >.....<version>.
+00037c10: 0a09 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+00037c20: 0909 093c 6d6f 6465 6c3e 5449 2d38 342b  ...<model>TI-84+
+00037c30: 4345 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  CE</model>......
+00037c40: 093c 6f73 2d76 6572 7369 6f6e 3e35 2e31  .<os-version>5.1
+00037c50: 2e30 3c2f 6f73 2d76 6572 7369 6f6e 3e0d  .0</os-version>.
+00037c60: 0a09 0909 093c 2f73 696e 6365 3e0d 0a09  .....</since>...
+00037c70: 0909 093c 6c61 6e67 2063 6f64 653d 2265  ...<lang code="e
+00037c80: 6e22 2074 692d 6173 6369 693d 2235 3137  n" ti-ascii="517
+00037c90: 3536 3137 3237 3436 3936 4336 3537 3332  5617274696C65732
+00037ca0: 3035 3336 3537 3437 3436 3936 4536 3743  053657474696E67C
+00037cb0: 4522 3e0d 0a09 0909 0909 3c64 6973 706c  E">.......<displ
+00037cc0: 6179 3e51 7561 7274 696c 6573 2053 6574  ay>Quartiles Set
+00037cd0: 7469 6e67 e280 a63c 2f64 6973 706c 6179  ting...</display
+00037ce0: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
+00037cf0: 626c 653e 5175 6172 7469 6c65 7320 5365  ble>Quartiles Se
+00037d00: 7474 696e 672e 2e2e 3c2f 6163 6365 7373  tting...</access
+00037d10: 6962 6c65 3e0d 0a09 0909 093c 2f6c 616e  ible>......</lan
+00037d20: 673e 0d0a 0909 093c 2f76 6572 7369 6f6e  g>.....</version
+00037d30: 3e0d 0a09 093c 2f74 6f6b 656e 3e0d 0a09  >....</token>...
+00037d40: 093c 746f 6b65 6e20 7661 6c75 653d 2224  .<token value="$
+00037d50: 3832 223e 0d0a 0909 093c 7665 7273 696f  82">.....<versio
+00037d60: 6e3e 0d0a 0909 0909 3c73 696e 6365 3e0d  n>......<since>.
+00037d70: 0a09 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+00037d80: 3834 2b43 453c 2f6d 6f64 656c 3e0d 0a09  84+CE</model>...
+00037d90: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
+00037da0: 352e 322e 303c 2f6f 732d 7665 7273 696f  5.2.0</os-versio
+00037db0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
+00037dc0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
+00037dd0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+00037de0: 3735 3238 3031 3244 3332 3239 223e 0d0a  7528012D3229">..
+00037df0: 0909 0909 093c 6469 7370 6c61 793e 7528  .....<display>u(
+00037e00: f09d 919b 2d32 293c 2f64 6973 706c 6179  ....-2)</display
+00037e10: 3e0d 0a09 0909 0909 3c61 6363 6573 7369  >.......<accessi
+00037e20: 626c 653e 7528 6e2d 3229 3c2f 6163 6365  ble>u(n-2)</acce
+00037e30: 7373 6962 6c65 3e0d 0a09 0909 0909 3c76  ssible>.......<v
+00037e40: 6172 6961 6e74 3e75 28f0 9d92 8f2d 3229  ariant>u(....-2)
+00037e50: 3c2f 7661 7269 616e 743e 0d0a 0909 0909  </variant>......
+00037e60: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+00037e70: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+00037e80: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+00037e90: 7565 3d22 2438 3322 3e0d 0a09 0909 3c76  ue="$83">.....<v
+00037ea0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+00037eb0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00037ec0: 6c3e 5449 2d38 342b 4345 3c2f 6d6f 6465  l>TI-84+CE</mode
+00037ed0: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
+00037ee0: 7369 6f6e 3e35 2e32 2e30 3c2f 6f73 2d76  sion>5.2.0</os-v
+00037ef0: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
+00037f00: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
+00037f10: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
+00037f20: 6369 693d 2237 3632 3830 3132 4433 3232  cii="7628012D322
+00037f30: 3922 3e0d 0a09 0909 0909 3c64 6973 706c  9">.......<displ
+00037f40: 6179 3e76 28f0 9d91 9b2d 3229 3c2f 6469  ay>v(....-2)</di
+00037f50: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00037f60: 6365 7373 6962 6c65 3e76 286e 2d32 293c  cessible>v(n-2)<
+00037f70: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00037f80: 0909 093c 7661 7269 616e 743e 7628 f09d  ...<variant>v(..
+00037f90: 928f 2d32 293c 2f76 6172 6961 6e74 3e0d  ..-2)</variant>.
+00037fa0: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+00037fb0: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00037fc0: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+00037fd0: 6e20 7661 6c75 653d 2224 3834 223e 0d0a  n value="$84">..
+00037fe0: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00037ff0: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00038000: 3c6d 6f64 656c 3e54 492d 3834 2b43 453c  <model>TI-84+CE<
+00038010: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+00038020: 732d 7665 7273 696f 6e3e 352e 322e 303c  s-version>5.2.0<
+00038030: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00038040: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00038050: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00038060: 7469 2d61 7363 6969 3d22 3737 3238 3031  ti-ascii="772801
+00038070: 3244 3332 3239 223e 0d0a 0909 0909 093c  2D3229">.......<
+00038080: 6469 7370 6c61 793e 7728 f09d 919b 2d32  display>w(....-2
+00038090: 293c 2f64 6973 706c 6179 3e0d 0a09 0909  )</display>.....
+000380a0: 0909 3c61 6363 6573 7369 626c 653e 7728  ..<accessible>w(
+000380b0: 6e2d 3229 3c2f 6163 6365 7373 6962 6c65  n-2)</accessible
+000380c0: 3e0d 0a09 0909 0909 3c76 6172 6961 6e74  >.......<variant
+000380d0: 3e77 28f0 9d92 8f2d 3229 3c2f 7661 7269  >w(....-2)</vari
+000380e0: 616e 743e 0d0a 0909 0909 3c2f 6c61 6e67  ant>......</lang
+000380f0: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
+00038100: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
+00038110: 3c74 6f6b 656e 2076 616c 7565 3d22 2438  <token value="$8
+00038120: 3522 3e0d 0a09 0909 3c76 6572 7369 6f6e  5">.....<version
+00038130: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
+00038140: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
+00038150: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
+00038160: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
+00038170: 2e32 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .2.0</os-version
+00038180: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
+00038190: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
+000381a0: 2265 6e22 2074 692d 6173 6369 693d 2237  "en" ti-ascii="7
+000381b0: 3532 3830 3132 4433 3132 3922 3e0d 0a09  528012D3129">...
+000381c0: 0909 0909 3c64 6973 706c 6179 3e75 28f0  ....<display>u(.
+000381d0: 9d91 9b2d 3129 3c2f 6469 7370 6c61 793e  ...-1)</display>
+000381e0: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+000381f0: 6c65 3e75 286e 2d31 293c 2f61 6363 6573  le>u(n-1)</acces
+00038200: 7369 626c 653e 0d0a 0909 0909 093c 7661  sible>.......<va
+00038210: 7269 616e 743e 7528 f09d 928f 2d31 293c  riant>u(....-1)<
+00038220: 2f76 6172 6961 6e74 3e0d 0a09 0909 093c  /variant>......<
+00038230: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
+00038240: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
+00038250: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
+00038260: 653d 2224 3836 223e 0d0a 0909 093c 7665  e="$86">.....<ve
+00038270: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
+00038280: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
+00038290: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
+000382a0: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
+000382b0: 696f 6e3e 352e 322e 303c 2f6f 732d 7665  ion>5.2.0</os-ve
+000382c0: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+000382d0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+000382e0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+000382f0: 6969 3d22 3736 3238 3031 3244 3331 3239  ii="7628012D3129
+00038300: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00038310: 793e 7628 f09d 919b 2d31 293c 2f64 6973  y>v(....-1)</dis
+00038320: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
+00038330: 6573 7369 626c 653e 7628 6e2d 3129 3c2f  essible>v(n-1)</
+00038340: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
+00038350: 0909 3c76 6172 6961 6e74 3e76 28f0 9d92  ..<variant>v(...
+00038360: 8f2d 3129 3c2f 7661 7269 616e 743e 0d0a  .-1)</variant>..
+00038370: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00038380: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00038390: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+000383a0: 2076 616c 7565 3d22 2438 3722 3e0d 0a09   value="$87">...
+000383b0: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+000383c0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+000383d0: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
+000383e0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
+000383f0: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
+00038400: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
+00038410: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
+00038420: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
+00038430: 692d 6173 6369 693d 2237 3732 3830 3132  i-ascii="7728012
+00038440: 4433 3132 3922 3e0d 0a09 0909 0909 3c64  D3129">.......<d
+00038450: 6973 706c 6179 3e77 28f0 9d91 9b2d 3129  isplay>w(....-1)
+00038460: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00038470: 093c 6163 6365 7373 6962 6c65 3e77 286e  .<accessible>w(n
+00038480: 2d31 293c 2f61 6363 6573 7369 626c 653e  -1)</accessible>
+00038490: 0d0a 0909 0909 093c 7661 7269 616e 743e  .......<variant>
+000384a0: 7728 f09d 928f 2d31 293c 2f76 6172 6961  w(....-1)</varia
+000384b0: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
+000384c0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
+000384d0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
+000384e0: 746f 6b65 6e20 7661 6c75 653d 2224 3838  token value="$88
+000384f0: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
+00038500: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
+00038510: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
+00038520: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
+00038530: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
+00038540: 322e 303c 2f6f 732d 7665 7273 696f 6e3e  2.0</os-version>
+00038550: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
+00038560: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
+00038570: 656e 2220 7469 2d61 7363 6969 3d22 3735  en" ti-ascii="75
+00038580: 3238 3031 3239 223e 0d0a 0909 0909 093c  280129">.......<
+00038590: 6469 7370 6c61 793e 7528 f09d 919b 293c  display>u(....)<
+000385a0: 2f64 6973 706c 6179 3e0d 0a09 0909 0909  /display>.......
+000385b0: 3c61 6363 6573 7369 626c 653e 7528 6e29  <accessible>u(n)
+000385c0: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
+000385d0: 0909 0909 3c76 6172 6961 6e74 3e75 28f0  ....<variant>u(.
+000385e0: 9d92 8f29 3c2f 7661 7269 616e 743e 0d0a  ...)</variant>..
+000385f0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00038600: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00038610: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00038620: 2076 616c 7565 3d22 2438 3922 3e0d 0a09   value="$89">...
+00038630: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00038640: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00038650: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
+00038660: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
+00038670: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
+00038680: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
+00038690: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
+000386a0: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
+000386b0: 692d 6173 6369 693d 2237 3632 3830 3132  i-ascii="7628012
+000386c0: 3922 3e0d 0a09 0909 0909 3c64 6973 706c  9">.......<displ
+000386d0: 6179 3e76 28f0 9d91 9b29 3c2f 6469 7370  ay>v(....)</disp
+000386e0: 6c61 793e 0d0a 0909 0909 093c 6163 6365  lay>.......<acce
+000386f0: 7373 6962 6c65 3e76 286e 293c 2f61 6363  ssible>v(n)</acc
+00038700: 6573 7369 626c 653e 0d0a 0909 0909 093c  essible>.......<
+00038710: 7661 7269 616e 743e 7628 f09d 928f 293c  variant>v(....)<
+00038720: 2f76 6172 6961 6e74 3e0d 0a09 0909 093c  /variant>......<
+00038730: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
+00038740: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
+00038750: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
+00038760: 653d 2224 3841 223e 0d0a 0909 093c 7665  e="$8A">.....<ve
+00038770: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
+00038780: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
+00038790: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
+000387a0: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
+000387b0: 696f 6e3e 352e 322e 303c 2f6f 732d 7665  ion>5.2.0</os-ve
+000387c0: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+000387d0: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+000387e0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+000387f0: 6969 3d22 3737 3238 3031 3239 223e 0d0a  ii="77280129">..
+00038800: 0909 0909 093c 6469 7370 6c61 793e 7728  .....<display>w(
+00038810: f09d 919b 293c 2f64 6973 706c 6179 3e0d  ....)</display>.
+00038820: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+00038830: 653e 7728 6e29 3c2f 6163 6365 7373 6962  e>w(n)</accessib
+00038840: 6c65 3e0d 0a09 0909 0909 3c76 6172 6961  le>.......<varia
+00038850: 6e74 3e77 28f0 9d92 8f29 3c2f 7661 7269  nt>w(....)</vari
+00038860: 616e 743e 0d0a 0909 0909 3c2f 6c61 6e67  ant>......</lang
+00038870: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
+00038880: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
+00038890: 3c74 6f6b 656e 2076 616c 7565 3d22 2438  <token value="$8
+000388a0: 4222 3e0d 0a09 0909 3c76 6572 7369 6f6e  B">.....<version
+000388b0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
+000388c0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
+000388d0: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
+000388e0: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
+000388f0: 2e32 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .2.0</os-version
+00038900: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
+00038910: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
+00038920: 2265 6e22 2074 692d 6173 6369 693d 2237  "en" ti-ascii="7
+00038930: 3532 3830 3132 4233 3132 3922 3e0d 0a09  528012B3129">...
+00038940: 0909 0909 3c64 6973 706c 6179 3e75 28f0  ....<display>u(.
+00038950: 9d91 9b2b 3129 3c2f 6469 7370 6c61 793e  ...+1)</display>
+00038960: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+00038970: 6c65 3e75 286e 2b31 293c 2f61 6363 6573  le>u(n+1)</acces
+00038980: 7369 626c 653e 0d0a 0909 0909 093c 7661  sible>.......<va
+00038990: 7269 616e 743e 7528 f09d 928f 2b31 293c  riant>u(....+1)<
+000389a0: 2f76 6172 6961 6e74 3e0d 0a09 0909 093c  /variant>......<
+000389b0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
+000389c0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
+000389d0: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
+000389e0: 653d 2224 3843 223e 0d0a 0909 093c 7665  e="$8C">.....<ve
+000389f0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
+00038a00: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
+00038a10: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
+00038a20: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
+00038a30: 696f 6e3e 352e 322e 303c 2f6f 732d 7665  ion>5.2.0</os-ve
+00038a40: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+00038a50: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+00038a60: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+00038a70: 6969 3d22 3736 3238 3031 3242 3331 3239  ii="7628012B3129
+00038a80: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00038a90: 793e 7628 f09d 919b 2b31 293c 2f64 6973  y>v(....+1)</dis
+00038aa0: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
+00038ab0: 6573 7369 626c 653e 7628 6e2b 3129 3c2f  essible>v(n+1)</
+00038ac0: 6163 6365 7373 6962 6c65 3e0d 0a09 0909  accessible>.....
+00038ad0: 0909 3c76 6172 6961 6e74 3e76 28f0 9d92  ..<variant>v(...
+00038ae0: 8f2b 3129 3c2f 7661 7269 616e 743e 0d0a  .+1)</variant>..
+00038af0: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00038b00: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00038b10: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00038b20: 2076 616c 7565 3d22 2438 4422 3e0d 0a09   value="$8D">...
+00038b30: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00038b40: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00038b50: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
+00038b60: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
+00038b70: 2d76 6572 7369 6f6e 3e35 2e32 2e30 3c2f  -version>5.2.0</
+00038b80: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
+00038b90: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
+00038ba0: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
+00038bb0: 692d 6173 6369 693d 2237 3732 3830 3132  i-ascii="7728012
+00038bc0: 4233 3132 3922 3e0d 0a09 0909 0909 3c64  B3129">.......<d
+00038bd0: 6973 706c 6179 3e77 28f0 9d91 9b2b 3129  isplay>w(....+1)
+00038be0: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00038bf0: 093c 6163 6365 7373 6962 6c65 3e77 286e  .<accessible>w(n
+00038c00: 2b31 293c 2f61 6363 6573 7369 626c 653e  +1)</accessible>
+00038c10: 0d0a 0909 0909 093c 7661 7269 616e 743e  .......<variant>
+00038c20: 7728 f09d 928f 2b31 293c 2f76 6172 6961  w(....+1)</varia
+00038c30: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
+00038c40: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
+00038c50: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
+00038c60: 746f 6b65 6e20 7661 6c75 653d 2224 3845  token value="$8E
+00038c70: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
+00038c80: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
+00038c90: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
+00038ca0: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
+00038cb0: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
+00038cc0: 322e 303c 2f6f 732d 7665 7273 696f 6e3e  2.0</os-version>
+00038cd0: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
+00038ce0: 0909 0909 3c75 6e74 696c 3e0d 0a09 0909  ....<until>.....
+00038cf0: 0909 3c6d 6f64 656c 3e54 492d 3834 2b43  ..<model>TI-84+C
+00038d00: 453c 2f6d 6f64 656c 3e0d 0a09 0909 0909  E</model>.......
+00038d10: 3c6f 732d 7665 7273 696f 6e3e 352e 332e  <os-version>5.3.
+00038d20: 303c 2f6f 732d 7665 7273 696f 6e3e 0d0a  0</os-version>..
+00038d30: 0909 0909 3c2f 756e 7469 6c3e 0d0a 0909  ....</until>....
+00038d40: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+00038d50: 2220 7469 2d61 7363 6969 3d22 3730 3639  " ti-ascii="7069
+00038d60: 3635 3633 3635 3537 3639 3733 3635 3238  6563655769736528
+00038d70: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00038d80: 793e 7069 6563 6557 6973 6528 3c2f 6469  y>pieceWise(</di
+00038d90: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00038da0: 6365 7373 6962 6c65 3e70 6965 6365 5769  cessible>pieceWi
+00038db0: 7365 283c 2f61 6363 6573 7369 626c 653e  se(</accessible>
+00038dc0: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
+00038dd0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
+00038de0: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
+00038df0: 656e 2076 616c 7565 3d22 2438 4622 3e0d  en value="$8F">.
+00038e00: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
+00038e10: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
+00038e20: 093c 6d6f 6465 6c3e 5449 2d38 342b 4345  .<model>TI-84+CE
+00038e30: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
+00038e40: 6f73 2d76 6572 7369 6f6e 3e35 2e32 2e30  os-version>5.2.0
+00038e50: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
+00038e60: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
+00038e70: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
+00038e80: 2074 692d 6173 6369 693d 2235 3334 3535   ti-ascii="53455
+00038e90: 3132 3830 3132 3922 3e0d 0a09 0909 0909  1280129">.......
+00038ea0: 3c64 6973 706c 6179 3e53 4551 28f0 9d91  <display>SEQ(...
+00038eb0: 9b29 3c2f 6469 7370 6c61 793e 0d0a 0909  .)</display>....
+00038ec0: 0909 093c 6163 6365 7373 6962 6c65 3e53  ...<accessible>S
+00038ed0: 4551 286e 293c 2f61 6363 6573 7369 626c  EQ(n)</accessibl
+00038ee0: 653e 0d0a 0909 0909 093c 7661 7269 616e  e>.......<varian
+00038ef0: 743e 5345 5128 f09d 928f 293c 2f76 6172  t>SEQ(....)</var
+00038f00: 6961 6e74 3e0d 0a09 0909 093c 2f6c 616e  iant>......</lan
+00038f10: 673e 0d0a 0909 093c 2f76 6572 7369 6f6e  g>.....</version
+00038f20: 3e0d 0a09 093c 2f74 6f6b 656e 3e0d 0a09  >....</token>...
+00038f30: 093c 746f 6b65 6e20 7661 6c75 653d 2224  .<token value="$
+00038f40: 3930 223e 0d0a 0909 093c 7665 7273 696f  90">.....<versio
+00038f50: 6e3e 0d0a 0909 0909 3c73 696e 6365 3e0d  n>......<since>.
+00038f60: 0a09 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+00038f70: 3834 2b43 453c 2f6d 6f64 656c 3e0d 0a09  84+CE</model>...
+00038f80: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
+00038f90: 352e 322e 303c 2f6f 732d 7665 7273 696f  5.2.0</os-versio
+00038fa0: 6e3e 0d0a 0909 0909 3c2f 7369 6e63 653e  n>......</since>
+00038fb0: 0d0a 0909 0909 3c6c 616e 6720 636f 6465  ......<lang code
+00038fc0: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+00038fd0: 3533 3435 3531 3238 3031 3242 3331 3239  53455128012B3129
+00038fe0: 223e 0d0a 0909 0909 093c 6469 7370 6c61  ">.......<displa
+00038ff0: 793e 5345 5128 f09d 919b 2b31 293c 2f64  y>SEQ(....+1)</d
+00039000: 6973 706c 6179 3e0d 0a09 0909 0909 3c61  isplay>.......<a
+00039010: 6363 6573 7369 626c 653e 5345 5128 6e2b  ccessible>SEQ(n+
+00039020: 3129 3c2f 6163 6365 7373 6962 6c65 3e0d  1)</accessible>.
+00039030: 0a09 0909 0909 3c76 6172 6961 6e74 3e53  ......<variant>S
+00039040: 4551 28f0 9d92 8f2b 3129 3c2f 7661 7269  EQ(....+1)</vari
+00039050: 616e 743e 0d0a 0909 0909 3c2f 6c61 6e67  ant>......</lang
+00039060: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
+00039070: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
+00039080: 3c74 6f6b 656e 2076 616c 7565 3d22 2439  <token value="$9
+00039090: 3122 3e0d 0a09 0909 3c76 6572 7369 6f6e  1">.....<version
+000390a0: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
+000390b0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
+000390c0: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
+000390d0: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
+000390e0: 2e32 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .2.0</os-version
+000390f0: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
+00039100: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
+00039110: 2265 6e22 2074 692d 6173 6369 693d 2235  "en" ti-ascii="5
+00039120: 3334 3535 3132 3830 3132 4233 3232 3922  3455128012B3229"
+00039130: 3e0d 0a09 0909 0909 3c64 6973 706c 6179  >.......<display
+00039140: 3e53 4551 28f0 9d91 9b2b 3229 3c2f 6469  >SEQ(....+2)</di
+00039150: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00039160: 6365 7373 6962 6c65 3e53 4551 286e 2b32  cessible>SEQ(n+2
+00039170: 293c 2f61 6363 6573 7369 626c 653e 0d0a  )</accessible>..
+00039180: 0909 0909 093c 7661 7269 616e 743e 5345  .....<variant>SE
+00039190: 5128 f09d 928f 2b32 293c 2f76 6172 6961  Q(....+2)</varia
+000391a0: 6e74 3e0d 0a09 0909 093c 2f6c 616e 673e  nt>......</lang>
+000391b0: 0d0a 0909 093c 2f76 6572 7369 6f6e 3e0d  .....</version>.
+000391c0: 0a09 093c 2f74 6f6b 656e 3e0d 0a09 093c  ...</token>....<
+000391d0: 746f 6b65 6e20 7661 6c75 653d 2224 3932  token value="$92
+000391e0: 223e 0d0a 0909 093c 7665 7273 696f 6e3e  ">.....<version>
+000391f0: 0d0a 0909 0909 3c73 696e 6365 3e0d 0a09  ......<since>...
+00039200: 0909 0909 3c6d 6f64 656c 3e54 492d 3834  ....<model>TI-84
+00039210: 2b43 453c 2f6d 6f64 656c 3e0d 0a09 0909  +CE</model>.....
+00039220: 0909 3c6f 732d 7665 7273 696f 6e3e 352e  ..<os-version>5.
+00039230: 322e 303c 2f6f 732d 7665 7273 696f 6e3e  2.0</os-version>
+00039240: 0d0a 0909 0909 3c2f 7369 6e63 653e 0d0a  ......</since>..
+00039250: 0909 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
+00039260: 656e 2220 7469 2d61 7363 6969 3d22 3443  en" ti-ascii="4C
+00039270: 3435 3436 3534 223e 0d0a 0909 0909 093c  454654">.......<
+00039280: 6469 7370 6c61 793e 4c45 4654 3c2f 6469  display>LEFT</di
+00039290: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+000392a0: 6365 7373 6962 6c65 3e4c 4546 543c 2f61  cessible>LEFT</a
+000392b0: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+000392c0: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+000392d0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+000392e0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+000392f0: 7565 3d22 2439 3322 3e0d 0a09 0909 3c76  ue="$93">.....<v
+00039300: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+00039310: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+00039320: 6c3e 5449 2d38 342b 4345 3c2f 6d6f 6465  l>TI-84+CE</mode
+00039330: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
+00039340: 7369 6f6e 3e35 2e32 2e30 3c2f 6f73 2d76  sion>5.2.0</os-v
+00039350: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
+00039360: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
+00039370: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
+00039380: 6369 693d 2234 3334 3534 4535 3434 3535  cii="43454E54455
+00039390: 3222 3e0d 0a09 0909 0909 3c64 6973 706c  2">.......<displ
+000393a0: 6179 3e43 454e 5445 523c 2f64 6973 706c  ay>CENTER</displ
+000393b0: 6179 3e0d 0a09 0909 0909 3c61 6363 6573  ay>.......<acces
+000393c0: 7369 626c 653e 4345 4e54 4552 3c2f 6163  sible>CENTER</ac
+000393d0: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
+000393e0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
+000393f0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
+00039400: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
+00039410: 653d 2224 3934 223e 0d0a 0909 093c 7665  e="$94">.....<ve
+00039420: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
+00039430: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
+00039440: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
+00039450: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
+00039460: 696f 6e3e 352e 322e 303c 2f6f 732d 7665  ion>5.2.0</os-ve
+00039470: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+00039480: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+00039490: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+000394a0: 6969 3d22 3532 3439 3437 3438 3534 223e  ii="5249474854">
+000394b0: 0d0a 0909 0909 093c 6469 7370 6c61 793e  .......<display>
+000394c0: 5249 4748 543c 2f64 6973 706c 6179 3e0d  RIGHT</display>.
+000394d0: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+000394e0: 653e 5249 4748 543c 2f61 6363 6573 7369  e>RIGHT</accessi
+000394f0: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
+00039500: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
+00039510: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
+00039520: 3c74 6f6b 656e 2076 616c 7565 3d22 2439  <token value="$9
+00039530: 3522 3e0d 0a09 0909 3c76 6572 7369 6f6e  5">.....<version
+00039540: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
+00039550: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
+00039560: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
+00039570: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
+00039580: 2e32 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .2.0</os-version
+00039590: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
+000395a0: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
+000395b0: 2265 6e22 2074 692d 6173 6369 693d 2236  "en" ti-ascii="6
+000395c0: 3936 4537 3634 3236 3936 4536 4636 4432  96E7642696E6F6D2
+000395d0: 3822 3e0d 0a09 0909 0909 3c64 6973 706c  8">.......<displ
+000395e0: 6179 3e69 6e76 4269 6e6f 6d28 3c2f 6469  ay>invBinom(</di
+000395f0: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00039600: 6365 7373 6962 6c65 3e69 6e76 4269 6e6f  cessible>invBino
+00039610: 6d28 3c2f 6163 6365 7373 6962 6c65 3e0d  m(</accessible>.
+00039620: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+00039630: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00039640: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+00039650: 6e20 7661 6c75 653d 2224 3936 223e 0d0a  n value="$96">..
+00039660: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+00039670: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+00039680: 3c6d 6f64 656c 3e54 492d 3834 2b43 453c  <model>TI-84+CE<
+00039690: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+000396a0: 732d 7665 7273 696f 6e3e 352e 322e 303c  s-version>5.2.0<
+000396b0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+000396c0: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+000396d0: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+000396e0: 7469 2d61 7363 6969 3d22 3537 3631 3639  ti-ascii="576169
+000396f0: 3734 3230 223e 0d0a 0909 0909 093c 6469  7420">.......<di
+00039700: 7370 6c61 793e 5761 6974 2623 3033 323b  splay>Wait&#032;
+00039710: 3c2f 6469 7370 6c61 793e 0d0a 0909 0909  </display>......
+00039720: 093c 6163 6365 7373 6962 6c65 3e57 6169  .<accessible>Wai
+00039730: 7426 2330 3332 3b3c 2f61 6363 6573 7369  t&#032;</accessi
+00039740: 626c 653e 0d0a 0909 0909 3c2f 6c61 6e67  ble>......</lang
+00039750: 3e0d 0a09 0909 3c2f 7665 7273 696f 6e3e  >.....</version>
+00039760: 0d0a 0909 3c2f 746f 6b65 6e3e 0d0a 0909  ....</token>....
+00039770: 3c74 6f6b 656e 2076 616c 7565 3d22 2439  <token value="$9
+00039780: 3722 3e0d 0a09 0909 3c76 6572 7369 6f6e  7">.....<version
+00039790: 3e0d 0a09 0909 093c 7369 6e63 653e 0d0a  >......<since>..
+000397a0: 0909 0909 093c 6d6f 6465 6c3e 5449 2d38  .....<model>TI-8
+000397b0: 342b 4345 3c2f 6d6f 6465 6c3e 0d0a 0909  4+CE</model>....
+000397c0: 0909 093c 6f73 2d76 6572 7369 6f6e 3e35  ...<os-version>5
+000397d0: 2e32 2e30 3c2f 6f73 2d76 6572 7369 6f6e  .2.0</os-version
+000397e0: 3e0d 0a09 0909 093c 2f73 696e 6365 3e0d  >......</since>.
+000397f0: 0a09 0909 093c 6c61 6e67 2063 6f64 653d  .....<lang code=
+00039800: 2265 6e22 2074 692d 6173 6369 693d 2237  "en" ti-ascii="7
+00039810: 3436 4635 3337 3437 3236 3936 4536 3732  46F537472696E672
+00039820: 3822 3e0d 0a09 0909 0909 3c64 6973 706c  8">.......<displ
+00039830: 6179 3e74 6f53 7472 696e 6728 3c2f 6469  ay>toString(</di
+00039840: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00039850: 6365 7373 6962 6c65 3e74 6f53 7472 696e  cessible>toStrin
+00039860: 6728 3c2f 6163 6365 7373 6962 6c65 3e0d  g(</accessible>.
+00039870: 0a09 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+00039880: 093c 2f76 6572 7369 6f6e 3e0d 0a09 093c  .</version>....<
+00039890: 2f74 6f6b 656e 3e0d 0a09 093c 746f 6b65  /token>....<toke
+000398a0: 6e20 7661 6c75 653d 2224 3938 223e 0d0a  n value="$98">..
+000398b0: 0909 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+000398c0: 0909 3c73 696e 6365 3e0d 0a09 0909 0909  ..<since>.......
+000398d0: 3c6d 6f64 656c 3e54 492d 3834 2b43 453c  <model>TI-84+CE<
+000398e0: 2f6d 6f64 656c 3e0d 0a09 0909 0909 3c6f  /model>.......<o
+000398f0: 732d 7665 7273 696f 6e3e 352e 322e 303c  s-version>5.2.0<
+00039900: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+00039910: 0909 3c2f 7369 6e63 653e 0d0a 0909 0909  ..</since>......
+00039920: 3c6c 616e 6720 636f 6465 3d22 656e 2220  <lang code="en" 
+00039930: 7469 2d61 7363 6969 3d22 3635 3736 3631  ti-ascii="657661
+00039940: 3643 3238 223e 0d0a 0909 0909 093c 6469  6C28">.......<di
+00039950: 7370 6c61 793e 6576 616c 283c 2f64 6973  splay>eval(</dis
+00039960: 706c 6179 3e0d 0a09 0909 0909 3c61 6363  play>.......<acc
+00039970: 6573 7369 626c 653e 6576 616c 283c 2f61  essible>eval(</a
+00039980: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+00039990: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+000399a0: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+000399b0: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+000399c0: 7565 3d22 2439 4522 3e0d 0a09 0909 3c76  ue="$9E">.....<v
+000399d0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+000399e0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+000399f0: 6c3e 5449 2d38 342b 4345 3c2f 6d6f 6465  l>TI-84+CE</mode
+00039a00: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
+00039a10: 7369 6f6e 3e35 2e33 2e30 3c2f 6f73 2d76  sion>5.3.0</os-v
+00039a20: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
+00039a30: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
+00039a40: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
+00039a50: 6369 693d 2234 3537 3836 3536 3337 3537  cii="45786563757
+00039a60: 3436 3532 3035 3037 3236 4636 3737 3236  4652050726F67726
+00039a70: 3136 4422 3e0d 0a09 0909 0909 3c64 6973  16D">.......<dis
+00039a80: 706c 6179 3e45 7865 6375 7465 2050 726f  play>Execute Pro
+00039a90: 6772 616d 3c2f 6469 7370 6c61 793e 0d0a  gram</display>..
+00039aa0: 0909 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
+00039ab0: 3e45 7865 6375 7465 2050 726f 6772 616d  >Execute Program
+00039ac0: 3c2f 6163 6365 7373 6962 6c65 3e0d 0a09  </accessible>...
+00039ad0: 0909 093c 2f6c 616e 673e 0d0a 0909 093c  ...</lang>.....<
+00039ae0: 2f76 6572 7369 6f6e 3e0d 0a09 093c 2f74  /version>....</t
+00039af0: 6f6b 656e 3e0d 0a09 093c 746f 6b65 6e20  oken>....<token 
+00039b00: 7661 6c75 653d 2224 3946 223e 0d0a 0909  value="$9F">....
+00039b10: 093c 7665 7273 696f 6e3e 0d0a 0909 0909  .<version>......
+00039b20: 3c73 696e 6365 3e0d 0a09 0909 0909 3c6d  <since>.......<m
+00039b30: 6f64 656c 3e54 492d 3834 2b43 453c 2f6d  odel>TI-84+CE</m
+00039b40: 6f64 656c 3e0d 0a09 0909 0909 3c6f 732d  odel>.......<os-
+00039b50: 7665 7273 696f 6e3e 352e 332e 303c 2f6f  version>5.3.0</o
+00039b60: 732d 7665 7273 696f 6e3e 0d0a 0909 0909  s-version>......
+00039b70: 3c2f 7369 6e63 653e 0d0a 0909 0909 3c6c  </since>......<l
+00039b80: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+00039b90: 2d61 7363 6969 3d22 3535 3645 3634 3646  -ascii="556E646F
+00039ba0: 3230 3433 3643 3635 3631 3732 223e 0d0a  20436C656172">..
+00039bb0: 0909 0909 093c 6469 7370 6c61 793e 556e  .....<display>Un
+00039bc0: 646f 2043 6c65 6172 3c2f 6469 7370 6c61  do Clear</displa
+00039bd0: 793e 0d0a 0909 0909 093c 6163 6365 7373  y>.......<access
+00039be0: 6962 6c65 3e55 6e64 6f20 436c 6561 723c  ible>Undo Clear<
+00039bf0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+00039c00: 0909 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f  ..</lang>.....</
+00039c10: 7665 7273 696f 6e3e 0d0a 0909 3c2f 746f  version>....</to
+00039c20: 6b65 6e3e 0d0a 0909 3c74 6f6b 656e 2076  ken>....<token v
+00039c30: 616c 7565 3d22 2441 3022 3e0d 0a09 0909  alue="$A0">.....
+00039c40: 3c76 6572 7369 6f6e 3e0d 0a09 0909 093c  <version>......<
+00039c50: 7369 6e63 653e 0d0a 0909 0909 093c 6d6f  since>.......<mo
+00039c60: 6465 6c3e 5449 2d38 342b 4345 3c2f 6d6f  del>TI-84+CE</mo
+00039c70: 6465 6c3e 0d0a 0909 0909 093c 6f73 2d76  del>.......<os-v
+00039c80: 6572 7369 6f6e 3e35 2e33 2e30 3c2f 6f73  ersion>5.3.0</os
+00039c90: 2d76 6572 7369 6f6e 3e0d 0a09 0909 093c  -version>......<
+00039ca0: 2f73 696e 6365 3e0d 0a09 0909 093c 6c61  /since>......<la
+00039cb0: 6e67 2063 6f64 653d 2265 6e22 2074 692d  ng code="en" ti-
+00039cc0: 6173 6369 693d 2234 3936 4537 3336 3537  ascii="496E73657
+00039cd0: 3237 3432 3034 4336 3936 4536 3532 3034  274204C696E65204
+00039ce0: 3136 3236 4637 3636 3522 3e0d 0a09 0909  1626F7665">.....
+00039cf0: 0909 3c64 6973 706c 6179 3e49 6e73 6572  ..<display>Inser
+00039d00: 7420 4c69 6e65 2041 626f 7665 3c2f 6469  t Line Above</di
+00039d10: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00039d20: 6365 7373 6962 6c65 3e49 6e73 6572 7420  cessible>Insert 
+00039d30: 4c69 6e65 2041 626f 7665 3c2f 6163 6365  Line Above</acce
+00039d40: 7373 6962 6c65 3e0d 0a09 0909 093c 2f6c  ssible>......</l
+00039d50: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
+00039d60: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
+00039d70: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
+00039d80: 2224 4131 223e 0d0a 0909 093c 7665 7273  "$A1">.....<vers
+00039d90: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
+00039da0: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
+00039db0: 492d 3834 2b43 453c 2f6d 6f64 656c 3e0d  I-84+CE</model>.
+00039dc0: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+00039dd0: 6e3e 352e 332e 303c 2f6f 732d 7665 7273  n>5.3.0</os-vers
+00039de0: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
+00039df0: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
+00039e00: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
+00039e10: 3d22 3433 3735 3734 3230 3443 3639 3645  ="437574204C696E
+00039e20: 3635 223e 0d0a 0909 0909 093c 6469 7370  65">.......<disp
+00039e30: 6c61 793e 4375 7420 4c69 6e65 3c2f 6469  lay>Cut Line</di
+00039e40: 7370 6c61 793e 0d0a 0909 0909 093c 6163  splay>.......<ac
+00039e50: 6365 7373 6962 6c65 3e43 7574 204c 696e  cessible>Cut Lin
+00039e60: 653c 2f61 6363 6573 7369 626c 653e 0d0a  e</accessible>..
+00039e70: 0909 0909 3c2f 6c61 6e67 3e0d 0a09 0909  ....</lang>.....
+00039e80: 3c2f 7665 7273 696f 6e3e 0d0a 0909 3c2f  </version>....</
+00039e90: 746f 6b65 6e3e 0d0a 0909 3c74 6f6b 656e  token>....<token
+00039ea0: 2076 616c 7565 3d22 2441 3222 3e0d 0a09   value="$A2">...
+00039eb0: 0909 3c76 6572 7369 6f6e 3e0d 0a09 0909  ..<version>.....
+00039ec0: 093c 7369 6e63 653e 0d0a 0909 0909 093c  .<since>.......<
+00039ed0: 6d6f 6465 6c3e 5449 2d38 342b 4345 3c2f  model>TI-84+CE</
+00039ee0: 6d6f 6465 6c3e 0d0a 0909 0909 093c 6f73  model>.......<os
+00039ef0: 2d76 6572 7369 6f6e 3e35 2e33 2e30 3c2f  -version>5.3.0</
+00039f00: 6f73 2d76 6572 7369 6f6e 3e0d 0a09 0909  os-version>.....
+00039f10: 093c 2f73 696e 6365 3e0d 0a09 0909 093c  .</since>......<
+00039f20: 6c61 6e67 2063 6f64 653d 2265 6e22 2074  lang code="en" t
+00039f30: 692d 6173 6369 693d 2234 3336 4637 3037  i-ascii="436F707
+00039f40: 3932 3034 4336 3936 4536 3522 3e0d 0a09  9204C696E65">...
+00039f50: 0909 0909 3c64 6973 706c 6179 3e43 6f70  ....<display>Cop
+00039f60: 7920 4c69 6e65 3c2f 6469 7370 6c61 793e  y Line</display>
+00039f70: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+00039f80: 6c65 3e43 6f70 7920 4c69 6e65 3c2f 6163  le>Copy Line</ac
+00039f90: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
+00039fa0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
+00039fb0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
+00039fc0: 3e0d 0a09 093c 746f 6b65 6e20 7661 6c75  >....<token valu
+00039fd0: 653d 2224 4133 223e 0d0a 0909 093c 7665  e="$A3">.....<ve
+00039fe0: 7273 696f 6e3e 0d0a 0909 0909 3c73 696e  rsion>......<sin
+00039ff0: 6365 3e0d 0a09 0909 0909 3c6d 6f64 656c  ce>.......<model
+0003a000: 3e54 492d 3834 2b43 453c 2f6d 6f64 656c  >TI-84+CE</model
+0003a010: 3e0d 0a09 0909 0909 3c6f 732d 7665 7273  >.......<os-vers
+0003a020: 696f 6e3e 352e 332e 303c 2f6f 732d 7665  ion>5.3.0</os-ve
+0003a030: 7273 696f 6e3e 0d0a 0909 0909 3c2f 7369  rsion>......</si
+0003a040: 6e63 653e 0d0a 0909 0909 3c6c 616e 6720  nce>......<lang 
+0003a050: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+0003a060: 6969 3d22 3530 3631 3733 3734 3635 3230  ii="506173746520
+0003a070: 3443 3639 3645 3635 3230 3432 3635 3643  4C696E652042656C
+0003a080: 3646 3737 223e 0d0a 0909 0909 093c 6469  6F77">.......<di
+0003a090: 7370 6c61 793e 5061 7374 6520 4c69 6e65  splay>Paste Line
+0003a0a0: 2042 656c 6f77 3c2f 6469 7370 6c61 793e   Below</display>
+0003a0b0: 0d0a 0909 0909 093c 6163 6365 7373 6962  .......<accessib
+0003a0c0: 6c65 3e50 6173 7465 204c 696e 6520 4265  le>Paste Line Be
+0003a0d0: 6c6f 773c 2f61 6363 6573 7369 626c 653e  low</accessible>
+0003a0e0: 0d0a 0909 0909 3c2f 6c61 6e67 3e0d 0a09  ......</lang>...
+0003a0f0: 0909 3c2f 7665 7273 696f 6e3e 0d0a 0909  ..</version>....
+0003a100: 3c2f 746f 6b65 6e3e 0d0a 0909 3c74 6f6b  </token>....<tok
+0003a110: 656e 2076 616c 7565 3d22 2441 3422 3e0d  en value="$A4">.
+0003a120: 0a09 0909 3c76 6572 7369 6f6e 3e0d 0a09  ....<version>...
+0003a130: 0909 093c 7369 6e63 653e 0d0a 0909 0909  ...<since>......
+0003a140: 093c 6d6f 6465 6c3e 5449 2d38 342b 4345  .<model>TI-84+CE
+0003a150: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 093c  </model>.......<
+0003a160: 6f73 2d76 6572 7369 6f6e 3e35 2e33 2e30  os-version>5.3.0
+0003a170: 3c2f 6f73 2d76 6572 7369 6f6e 3e0d 0a09  </os-version>...
+0003a180: 0909 093c 2f73 696e 6365 3e0d 0a09 0909  ...</since>.....
+0003a190: 093c 6c61 6e67 2063 6f64 653d 2265 6e22  .<lang code="en"
+0003a1a0: 2074 692d 6173 6369 693d 2234 3936 4537   ti-ascii="496E7
+0003a1b0: 3336 3537 3237 3432 3034 3336 4636 4436  365727420436F6D6
+0003a1c0: 4436 3536 4537 3432 3034 3136 3236 4637  D656E742041626F7
+0003a1d0: 3636 3522 3e0d 0a09 0909 0909 3c64 6973  665">.......<dis
+0003a1e0: 706c 6179 3e49 6e73 6572 7420 436f 6d6d  play>Insert Comm
+0003a1f0: 656e 7420 4162 6f76 653c 2f64 6973 706c  ent Above</displ
+0003a200: 6179 3e0d 0a09 0909 0909 3c61 6363 6573  ay>.......<acces
+0003a210: 7369 626c 653e 496e 7365 7274 2043 6f6d  sible>Insert Com
+0003a220: 6d65 6e74 2041 626f 7665 3c2f 6163 6365  ment Above</acce
+0003a230: 7373 6962 6c65 3e0d 0a09 0909 093c 2f6c  ssible>......</l
+0003a240: 616e 673e 0d0a 0909 093c 2f76 6572 7369  ang>.....</versi
+0003a250: 6f6e 3e0d 0a09 093c 2f74 6f6b 656e 3e0d  on>....</token>.
+0003a260: 0a09 093c 746f 6b65 6e20 7661 6c75 653d  ...<token value=
+0003a270: 2224 4135 223e 0d0a 0909 093c 7665 7273  "$A5">.....<vers
+0003a280: 696f 6e3e 0d0a 0909 0909 3c73 696e 6365  ion>......<since
+0003a290: 3e0d 0a09 0909 0909 3c6d 6f64 656c 3e54  >.......<model>T
+0003a2a0: 492d 3834 2b43 453c 2f6d 6f64 656c 3e0d  I-84+CE</model>.
+0003a2b0: 0a09 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+0003a2c0: 6e3e 352e 332e 303c 2f6f 732d 7665 7273  n>5.3.0</os-vers
+0003a2d0: 696f 6e3e 0d0a 0909 0909 3c2f 7369 6e63  ion>......</sinc
+0003a2e0: 653e 0d0a 0909 0909 3c6c 616e 6720 636f  e>......<lang co
+0003a2f0: 6465 3d22 656e 2220 7469 2d61 7363 6969  de="en" ti-ascii
+0003a300: 3d22 3531 3735 3639 3734 3230 3435 3634  ="51756974204564
+0003a310: 3639 3734 3646 3732 223e 0d0a 0909 0909  69746F72">......
+0003a320: 093c 6469 7370 6c61 793e 5175 6974 2045  .<display>Quit E
+0003a330: 6469 746f 723c 2f64 6973 706c 6179 3e0d  ditor</display>.
+0003a340: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+0003a350: 653e 5175 6974 2045 6469 746f 723c 2f61  e>Quit Editor</a
+0003a360: 6363 6573 7369 626c 653e 0d0a 0909 0909  ccessible>......
+0003a370: 3c2f 6c61 6e67 3e0d 0a09 0909 3c2f 7665  </lang>.....</ve
+0003a380: 7273 696f 6e3e 0d0a 0909 3c2f 746f 6b65  rsion>....</toke
+0003a390: 6e3e 0d0a 0909 3c74 6f6b 656e 2076 616c  n>....<token val
+0003a3a0: 7565 3d22 2441 3622 3e0d 0a09 0909 3c76  ue="$A6">.....<v
+0003a3b0: 6572 7369 6f6e 3e0d 0a09 0909 093c 7369  ersion>......<si
+0003a3c0: 6e63 653e 0d0a 0909 0909 093c 6d6f 6465  nce>.......<mode
+0003a3d0: 6c3e 5449 2d38 342b 4345 3c2f 6d6f 6465  l>TI-84+CE</mode
+0003a3e0: 6c3e 0d0a 0909 0909 093c 6f73 2d76 6572  l>.......<os-ver
+0003a3f0: 7369 6f6e 3e35 2e33 2e30 3c2f 6f73 2d76  sion>5.3.0</os-v
+0003a400: 6572 7369 6f6e 3e0d 0a09 0909 093c 2f73  ersion>......</s
+0003a410: 696e 6365 3e0d 0a09 0909 093c 6c61 6e67  ince>......<lang
+0003a420: 2063 6f64 653d 2265 6e22 2074 692d 6173   code="en" ti-as
+0003a430: 6369 693d 2237 3036 3936 3536 3336 3537  cii="70696563657
+0003a440: 3736 3937 3336 3532 3822 3e0d 0a09 0909  769736528">.....
+0003a450: 0909 3c64 6973 706c 6179 3e70 6965 6365  ..<display>piece
+0003a460: 7769 7365 283c 2f64 6973 706c 6179 3e0d  wise(</display>.
+0003a470: 0a09 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+0003a480: 653e 7069 6563 6577 6973 6528 3c2f 6163  e>piecewise(</ac
+0003a490: 6365 7373 6962 6c65 3e0d 0a09 0909 093c  cessible>......<
+0003a4a0: 2f6c 616e 673e 0d0a 0909 093c 2f76 6572  /lang>.....</ver
+0003a4b0: 7369 6f6e 3e0d 0a09 093c 2f74 6f6b 656e  sion>....</token
+0003a4c0: 3e0d 0a09 3c2f 7477 6f2d 6279 7465 3e0d  >...</two-byte>.
+0003a4d0: 0a09 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+0003a4e0: 2446 3022 3e0d 0a09 093c 7665 7273 696f  $F0">....<versio
+0003a4f0: 6e3e 0d0a 0909 093c 7369 6e63 653e 0d0a  n>.....<since>..
+0003a500: 0909 0909 3c6d 6f64 656c 3e54 492d 3832  ....<model>TI-82
+0003a510: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 3c6f  </model>......<o
+0003a520: 732d 7665 7273 696f 6e3e 312e 303c 2f6f  s-version>1.0</o
+0003a530: 732d 7665 7273 696f 6e3e 0d0a 0909 093c  s-version>.....<
+0003a540: 2f73 696e 6365 3e0d 0a09 0909 3c6c 616e  /since>.....<lan
+0003a550: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+0003a560: 7363 6969 3d22 3545 223e 0d0a 0909 0909  scii="5E">......
+0003a570: 3c64 6973 706c 6179 3e5e 3c2f 6469 7370  <display>^</disp
+0003a580: 6c61 793e 0d0a 0909 0909 3c61 6363 6573  lay>......<acces
+0003a590: 7369 626c 653e 5e3c 2f61 6363 6573 7369  sible>^</accessi
+0003a5a0: 626c 653e 0d0a 0909 093c 2f6c 616e 673e  ble>.....</lang>
+0003a5b0: 0d0a 0909 3c2f 7665 7273 696f 6e3e 0d0a  ....</version>..
+0003a5c0: 093c 2f74 6f6b 656e 3e0d 0a09 3c74 6f6b  .</token>...<tok
+0003a5d0: 656e 2076 616c 7565 3d22 2446 3122 3e0d  en value="$F1">.
+0003a5e0: 0a09 093c 7665 7273 696f 6e3e 0d0a 0909  ...<version>....
+0003a5f0: 093c 7369 6e63 653e 0d0a 0909 0909 3c6d  .<since>......<m
+0003a600: 6f64 656c 3e54 492d 3832 3c2f 6d6f 6465  odel>TI-82</mode
+0003a610: 6c3e 0d0a 0909 0909 3c6f 732d 7665 7273  l>......<os-vers
+0003a620: 696f 6e3e 312e 303c 2f6f 732d 7665 7273  ion>1.0</os-vers
+0003a630: 696f 6e3e 0d0a 0909 093c 2f73 696e 6365  ion>.....</since
+0003a640: 3e0d 0a09 0909 3c6c 616e 6720 636f 6465  >.....<lang code
+0003a650: 3d22 656e 2220 7469 2d61 7363 6969 3d22  ="en" ti-ascii="
+0003a660: 4344 3130 223e 0d0a 0909 0909 3c64 6973  CD10">......<dis
+0003a670: 706c 6179 3ecb a3e2 889a 3c2f 6469 7370  play>.....</disp
+0003a680: 6c61 793e 0d0a 0909 0909 3c61 6363 6573  lay>......<acces
+0003a690: 7369 626c 653e 7872 6f6f 743c 2f61 6363  sible>xroot</acc
+0003a6a0: 6573 7369 626c 653e 0d0a 0909 093c 2f6c  essible>.....</l
+0003a6b0: 616e 673e 0d0a 0909 3c2f 7665 7273 696f  ang>....</versio
+0003a6c0: 6e3e 0d0a 093c 2f74 6f6b 656e 3e0d 0a09  n>...</token>...
+0003a6d0: 3c74 6f6b 656e 2076 616c 7565 3d22 2446  <token value="$F
+0003a6e0: 3222 3e0d 0a09 093c 7665 7273 696f 6e3e  2">....<version>
+0003a6f0: 0d0a 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+0003a700: 0909 3c6d 6f64 656c 3e54 492d 3832 3c2f  ..<model>TI-82</
+0003a710: 6d6f 6465 6c3e 0d0a 0909 0909 3c6f 732d  model>......<os-
+0003a720: 7665 7273 696f 6e3e 312e 303c 2f6f 732d  version>1.0</os-
+0003a730: 7665 7273 696f 6e3e 0d0a 0909 093c 2f73  version>.....</s
+0003a740: 696e 6365 3e0d 0a09 0909 3c6c 616e 6720  ince>.....<lang 
+0003a750: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+0003a760: 6969 3d22 3331 3244 3536 3631 3732 3230  ii="312D56617220
+0003a770: 3533 3734 3631 3734 3733 3230 223e 0d0a  537461747320">..
+0003a780: 0909 0909 3c64 6973 706c 6179 3e31 2d56  ....<display>1-V
+0003a790: 6172 2053 7461 7473 2623 3033 323b 3c2f  ar Stats&#032;</
+0003a7a0: 6469 7370 6c61 793e 0d0a 0909 0909 3c61  display>......<a
+0003a7b0: 6363 6573 7369 626c 653e 312d 5661 7220  ccessible>1-Var 
+0003a7c0: 5374 6174 7326 2330 3332 3b3c 2f61 6363  Stats&#032;</acc
+0003a7d0: 6573 7369 626c 653e 0d0a 0909 093c 2f6c  essible>.....</l
+0003a7e0: 616e 673e 0d0a 0909 3c2f 7665 7273 696f  ang>....</versio
+0003a7f0: 6e3e 0d0a 093c 2f74 6f6b 656e 3e0d 0a09  n>...</token>...
+0003a800: 3c74 6f6b 656e 2076 616c 7565 3d22 2446  <token value="$F
+0003a810: 3322 3e0d 0a09 093c 7665 7273 696f 6e3e  3">....<version>
+0003a820: 0d0a 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+0003a830: 0909 3c6d 6f64 656c 3e54 492d 3832 3c2f  ..<model>TI-82</
+0003a840: 6d6f 6465 6c3e 0d0a 0909 0909 3c6f 732d  model>......<os-
+0003a850: 7665 7273 696f 6e3e 312e 303c 2f6f 732d  version>1.0</os-
+0003a860: 7665 7273 696f 6e3e 0d0a 0909 093c 2f73  version>.....</s
+0003a870: 696e 6365 3e0d 0a09 0909 3c6c 616e 6720  ince>.....<lang 
+0003a880: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+0003a890: 6969 3d22 3332 3244 3536 3631 3732 3230  ii="322D56617220
+0003a8a0: 3533 3734 3631 3734 3733 3230 223e 0d0a  537461747320">..
+0003a8b0: 0909 0909 3c64 6973 706c 6179 3e32 2d56  ....<display>2-V
+0003a8c0: 6172 2053 7461 7473 2623 3033 323b 3c2f  ar Stats&#032;</
+0003a8d0: 6469 7370 6c61 793e 0d0a 0909 0909 3c61  display>......<a
+0003a8e0: 6363 6573 7369 626c 653e 322d 5661 7220  ccessible>2-Var 
+0003a8f0: 5374 6174 7326 2330 3332 3b3c 2f61 6363  Stats&#032;</acc
+0003a900: 6573 7369 626c 653e 0d0a 0909 093c 2f6c  essible>.....</l
+0003a910: 616e 673e 0d0a 0909 3c2f 7665 7273 696f  ang>....</versio
+0003a920: 6e3e 0d0a 093c 2f74 6f6b 656e 3e0d 0a09  n>...</token>...
+0003a930: 3c74 6f6b 656e 2076 616c 7565 3d22 2446  <token value="$F
+0003a940: 3422 3e0d 0a09 093c 7665 7273 696f 6e3e  4">....<version>
+0003a950: 0d0a 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+0003a960: 0909 3c6d 6f64 656c 3e54 492d 3832 3c2f  ..<model>TI-82</
+0003a970: 6d6f 6465 6c3e 0d0a 0909 0909 3c6f 732d  model>......<os-
+0003a980: 7665 7273 696f 6e3e 312e 303c 2f6f 732d  version>1.0</os-
+0003a990: 7665 7273 696f 6e3e 0d0a 0909 093c 2f73  version>.....</s
+0003a9a0: 696e 6365 3e0d 0a09 0909 3c6c 616e 6720  ince>.....<lang 
+0003a9b0: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+0003a9c0: 6969 3d22 3443 3639 3645 3532 3635 3637  ii="4C696E526567
+0003a9d0: 3238 3631 3242 3632 3738 3239 3230 223e  28612B62782920">
+0003a9e0: 0d0a 0909 0909 3c64 6973 706c 6179 3e4c  ......<display>L
+0003a9f0: 696e 5265 6728 612b 6278 2926 2330 3332  inReg(a+bx)&#032
+0003aa00: 3b3c 2f64 6973 706c 6179 3e0d 0a09 0909  ;</display>.....
+0003aa10: 093c 6163 6365 7373 6962 6c65 3e4c 696e  .<accessible>Lin
+0003aa20: 5265 6728 612b 6278 2926 2330 3332 3b3c  Reg(a+bx)&#032;<
+0003aa30: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+0003aa40: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
+0003aa50: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
+0003aa60: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
+0003aa70: 3d22 2446 3522 3e0d 0a09 093c 7665 7273  ="$F5">....<vers
+0003aa80: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
+0003aa90: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+0003aaa0: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
+0003aab0: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
+0003aac0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+0003aad0: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
+0003aae0: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+0003aaf0: 2d61 7363 6969 3d22 3435 3738 3730 3532  -ascii="45787052
+0003ab00: 3635 3637 3230 223e 0d0a 0909 0909 3c64  656720">......<d
+0003ab10: 6973 706c 6179 3e45 7870 5265 6726 2330  isplay>ExpReg&#0
+0003ab20: 3332 3b3c 2f64 6973 706c 6179 3e0d 0a09  32;</display>...
+0003ab30: 0909 093c 6163 6365 7373 6962 6c65 3e45  ...<accessible>E
+0003ab40: 7870 5265 6726 2330 3332 3b3c 2f61 6363  xpReg&#032;</acc
+0003ab50: 6573 7369 626c 653e 0d0a 0909 093c 2f6c  essible>.....</l
+0003ab60: 616e 673e 0d0a 0909 3c2f 7665 7273 696f  ang>....</versio
+0003ab70: 6e3e 0d0a 093c 2f74 6f6b 656e 3e0d 0a09  n>...</token>...
+0003ab80: 3c74 6f6b 656e 2076 616c 7565 3d22 2446  <token value="$F
+0003ab90: 3622 3e0d 0a09 093c 7665 7273 696f 6e3e  6">....<version>
+0003aba0: 0d0a 0909 093c 7369 6e63 653e 0d0a 0909  .....<since>....
+0003abb0: 0909 3c6d 6f64 656c 3e54 492d 3832 3c2f  ..<model>TI-82</
+0003abc0: 6d6f 6465 6c3e 0d0a 0909 0909 3c6f 732d  model>......<os-
+0003abd0: 7665 7273 696f 6e3e 312e 303c 2f6f 732d  version>1.0</os-
+0003abe0: 7665 7273 696f 6e3e 0d0a 0909 093c 2f73  version>.....</s
+0003abf0: 696e 6365 3e0d 0a09 0909 3c6c 616e 6720  ince>.....<lang 
+0003ac00: 636f 6465 3d22 656e 2220 7469 2d61 7363  code="en" ti-asc
+0003ac10: 6969 3d22 3443 3645 3532 3635 3637 3230  ii="4C6E52656720
+0003ac20: 223e 0d0a 0909 0909 3c64 6973 706c 6179  ">......<display
+0003ac30: 3e4c 6e52 6567 2623 3033 323b 3c2f 6469  >LnReg&#032;</di
+0003ac40: 7370 6c61 793e 0d0a 0909 0909 3c61 6363  splay>......<acc
+0003ac50: 6573 7369 626c 653e 4c6e 5265 6726 2330  essible>LnReg&#0
+0003ac60: 3332 3b3c 2f61 6363 6573 7369 626c 653e  32;</accessible>
+0003ac70: 0d0a 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+0003ac80: 3c2f 7665 7273 696f 6e3e 0d0a 093c 2f74  </version>...</t
+0003ac90: 6f6b 656e 3e0d 0a09 3c74 6f6b 656e 2076  oken>...<token v
+0003aca0: 616c 7565 3d22 2446 3722 3e0d 0a09 093c  alue="$F7">....<
+0003acb0: 7665 7273 696f 6e3e 0d0a 0909 093c 7369  version>.....<si
+0003acc0: 6e63 653e 0d0a 0909 0909 3c6d 6f64 656c  nce>......<model
+0003acd0: 3e54 492d 3832 3c2f 6d6f 6465 6c3e 0d0a  >TI-82</model>..
+0003ace0: 0909 0909 3c6f 732d 7665 7273 696f 6e3e  ....<os-version>
+0003acf0: 312e 303c 2f6f 732d 7665 7273 696f 6e3e  1.0</os-version>
+0003ad00: 0d0a 0909 093c 2f73 696e 6365 3e0d 0a09  .....</since>...
+0003ad10: 0909 3c6c 616e 6720 636f 6465 3d22 656e  ..<lang code="en
+0003ad20: 2220 7469 2d61 7363 6969 3d22 3530 3737  " ti-ascii="5077
+0003ad30: 3732 3532 3635 3637 3230 223e 0d0a 0909  7252656720">....
+0003ad40: 0909 3c64 6973 706c 6179 3e50 7772 5265  ..<display>PwrRe
+0003ad50: 6726 2330 3332 3b3c 2f64 6973 706c 6179  g&#032;</display
+0003ad60: 3e0d 0a09 0909 093c 6163 6365 7373 6962  >......<accessib
+0003ad70: 6c65 3e50 7772 5265 6726 2330 3332 3b3c  le>PwrReg&#032;<
+0003ad80: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+0003ad90: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
+0003ada0: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
+0003adb0: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
+0003adc0: 3d22 2446 3822 3e0d 0a09 093c 7665 7273  ="$F8">....<vers
+0003add0: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
+0003ade0: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+0003adf0: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
+0003ae00: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
+0003ae10: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+0003ae20: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
+0003ae30: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+0003ae40: 2d61 7363 6969 3d22 3444 3635 3634 3244  -ascii="4D65642D
+0003ae50: 3444 3635 3634 3230 223e 0d0a 0909 0909  4D656420">......
+0003ae60: 3c64 6973 706c 6179 3e4d 6564 2d4d 6564  <display>Med-Med
+0003ae70: 2623 3033 323b 3c2f 6469 7370 6c61 793e  &#032;</display>
+0003ae80: 0d0a 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+0003ae90: 653e 4d65 642d 4d65 6426 2330 3332 3b3c  e>Med-Med&#032;<
+0003aea0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+0003aeb0: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
+0003aec0: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
+0003aed0: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
+0003aee0: 3d22 2446 3922 3e0d 0a09 093c 7665 7273  ="$F9">....<vers
+0003aef0: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
+0003af00: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+0003af10: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
+0003af20: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
+0003af30: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+0003af40: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
+0003af50: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+0003af60: 2d61 7363 6969 3d22 3531 3735 3631 3634  -ascii="51756164
+0003af70: 3532 3635 3637 3230 223e 0d0a 0909 0909  52656720">......
+0003af80: 3c64 6973 706c 6179 3e51 7561 6452 6567  <display>QuadReg
+0003af90: 2623 3033 323b 3c2f 6469 7370 6c61 793e  &#032;</display>
+0003afa0: 0d0a 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+0003afb0: 653e 5175 6164 5265 6726 2330 3332 3b3c  e>QuadReg&#032;<
+0003afc0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+0003afd0: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
+0003afe0: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
+0003aff0: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
+0003b000: 3d22 2446 4122 3e0d 0a09 093c 7665 7273  ="$FA">....<vers
+0003b010: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
+0003b020: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+0003b030: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
+0003b040: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
+0003b050: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+0003b060: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
+0003b070: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+0003b080: 2d61 7363 6969 3d22 3433 3643 3732 3443  -ascii="436C724C
+0003b090: 3639 3733 3734 3230 223e 0d0a 0909 0909  69737420">......
+0003b0a0: 3c64 6973 706c 6179 3e43 6c72 4c69 7374  <display>ClrList
+0003b0b0: 2623 3033 323b 3c2f 6469 7370 6c61 793e  &#032;</display>
+0003b0c0: 0d0a 0909 0909 3c61 6363 6573 7369 626c  ......<accessibl
+0003b0d0: 653e 436c 724c 6973 7426 2330 3332 3b3c  e>ClrList&#032;<
+0003b0e0: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+0003b0f0: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
+0003b100: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
+0003b110: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
+0003b120: 3d22 2446 4222 3e0d 0a09 093c 7665 7273  ="$FB">....<vers
+0003b130: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
+0003b140: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+0003b150: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
+0003b160: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
+0003b170: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+0003b180: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
+0003b190: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+0003b1a0: 2d61 7363 6969 3d22 3433 3643 3732 3534  -ascii="436C7254
+0003b1b0: 3631 3632 3643 3635 223e 0d0a 0909 0909  61626C65">......
+0003b1c0: 3c64 6973 706c 6179 3e43 6c72 5461 626c  <display>ClrTabl
+0003b1d0: 653c 2f64 6973 706c 6179 3e0d 0a09 0909  e</display>.....
+0003b1e0: 093c 6163 6365 7373 6962 6c65 3e43 6c72  .<accessible>Clr
+0003b1f0: 5461 626c 653c 2f61 6363 6573 7369 626c  Table</accessibl
+0003b200: 653e 0d0a 0909 093c 2f6c 616e 673e 0d0a  e>.....</lang>..
+0003b210: 0909 3c2f 7665 7273 696f 6e3e 0d0a 093c  ..</version>...<
+0003b220: 2f74 6f6b 656e 3e0d 0a09 3c74 6f6b 656e  /token>...<token
+0003b230: 2076 616c 7565 3d22 2446 4322 3e0d 0a09   value="$FC">...
+0003b240: 093c 7665 7273 696f 6e3e 0d0a 0909 093c  .<version>.....<
+0003b250: 7369 6e63 653e 0d0a 0909 0909 3c6d 6f64  since>......<mod
+0003b260: 656c 3e54 492d 3832 3c2f 6d6f 6465 6c3e  el>TI-82</model>
+0003b270: 0d0a 0909 0909 3c6f 732d 7665 7273 696f  ......<os-versio
+0003b280: 6e3e 312e 303c 2f6f 732d 7665 7273 696f  n>1.0</os-versio
+0003b290: 6e3e 0d0a 0909 093c 2f73 696e 6365 3e0d  n>.....</since>.
+0003b2a0: 0a09 0909 3c6c 616e 6720 636f 6465 3d22  ....<lang code="
+0003b2b0: 656e 2220 7469 2d61 7363 6969 3d22 3438  en" ti-ascii="48
+0003b2c0: 3639 3733 3734 3646 3637 3732 3631 3644  6973746F6772616D
+0003b2d0: 223e 0d0a 0909 0909 3c64 6973 706c 6179  ">......<display
+0003b2e0: 3e48 6973 746f 6772 616d 3c2f 6469 7370  >Histogram</disp
+0003b2f0: 6c61 793e 0d0a 0909 0909 3c61 6363 6573  lay>......<acces
+0003b300: 7369 626c 653e 4869 7374 6f67 7261 6d3c  sible>Histogram<
+0003b310: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+0003b320: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
+0003b330: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
+0003b340: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
+0003b350: 3d22 2446 4422 3e0d 0a09 093c 7665 7273  ="$FD">....<vers
+0003b360: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
+0003b370: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+0003b380: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
+0003b390: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
+0003b3a0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+0003b3b0: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
+0003b3c0: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+0003b3d0: 2d61 7363 6969 3d22 3738 3739 3443 3639  -ascii="78794C69
+0003b3e0: 3645 3635 223e 0d0a 0909 0909 3c64 6973  6E65">......<dis
+0003b3f0: 706c 6179 3e78 794c 696e 653c 2f64 6973  play>xyLine</dis
+0003b400: 706c 6179 3e0d 0a09 0909 093c 6163 6365  play>......<acce
+0003b410: 7373 6962 6c65 3e78 794c 696e 653c 2f61  ssible>xyLine</a
+0003b420: 6363 6573 7369 626c 653e 0d0a 0909 093c  ccessible>.....<
+0003b430: 2f6c 616e 673e 0d0a 0909 3c2f 7665 7273  /lang>....</vers
+0003b440: 696f 6e3e 0d0a 093c 2f74 6f6b 656e 3e0d  ion>...</token>.
+0003b450: 0a09 3c74 6f6b 656e 2076 616c 7565 3d22  ..<token value="
+0003b460: 2446 4522 3e0d 0a09 093c 7665 7273 696f  $FE">....<versio
+0003b470: 6e3e 0d0a 0909 093c 7369 6e63 653e 0d0a  n>.....<since>..
+0003b480: 0909 0909 3c6d 6f64 656c 3e54 492d 3832  ....<model>TI-82
+0003b490: 3c2f 6d6f 6465 6c3e 0d0a 0909 0909 3c6f  </model>......<o
+0003b4a0: 732d 7665 7273 696f 6e3e 312e 303c 2f6f  s-version>1.0</o
+0003b4b0: 732d 7665 7273 696f 6e3e 0d0a 0909 093c  s-version>.....<
+0003b4c0: 2f73 696e 6365 3e0d 0a09 0909 3c6c 616e  /since>.....<lan
+0003b4d0: 6720 636f 6465 3d22 656e 2220 7469 2d61  g code="en" ti-a
+0003b4e0: 7363 6969 3d22 3533 3633 3631 3734 3734  scii="5363617474
+0003b4f0: 3635 3732 223e 0d0a 0909 0909 3c64 6973  6572">......<dis
+0003b500: 706c 6179 3e53 6361 7474 6572 3c2f 6469  play>Scatter</di
+0003b510: 7370 6c61 793e 0d0a 0909 0909 3c61 6363  splay>......<acc
+0003b520: 6573 7369 626c 653e 5363 6174 7465 723c  essible>Scatter<
+0003b530: 2f61 6363 6573 7369 626c 653e 0d0a 0909  /accessible>....
+0003b540: 093c 2f6c 616e 673e 0d0a 0909 3c2f 7665  .</lang>....</ve
+0003b550: 7273 696f 6e3e 0d0a 093c 2f74 6f6b 656e  rsion>...</token
+0003b560: 3e0d 0a09 3c74 6f6b 656e 2076 616c 7565  >...<token value
+0003b570: 3d22 2446 4622 3e0d 0a09 093c 7665 7273  ="$FF">....<vers
+0003b580: 696f 6e3e 0d0a 0909 093c 7369 6e63 653e  ion>.....<since>
+0003b590: 0d0a 0909 0909 3c6d 6f64 656c 3e54 492d  ......<model>TI-
+0003b5a0: 3832 3c2f 6d6f 6465 6c3e 0d0a 0909 0909  82</model>......
+0003b5b0: 3c6f 732d 7665 7273 696f 6e3e 312e 303c  <os-version>1.0<
+0003b5c0: 2f6f 732d 7665 7273 696f 6e3e 0d0a 0909  /os-version>....
+0003b5d0: 093c 2f73 696e 6365 3e0d 0a09 0909 3c6c  .</since>.....<l
+0003b5e0: 616e 6720 636f 6465 3d22 656e 2220 7469  ang code="en" ti
+0003b5f0: 2d61 7363 6969 3d22 3443 3639 3645 3532  -ascii="4C696E52
+0003b600: 3635 3637 3238 3631 3738 3242 3632 3239  65672861782B6229
+0003b610: 3230 223e 0d0a 0909 0909 3c64 6973 706c  20">......<displ
+0003b620: 6179 3e4c 696e 5265 6728 6178 2b62 2926  ay>LinReg(ax+b)&
+0003b630: 2330 3332 3b3c 2f64 6973 706c 6179 3e0d  #032;</display>.
+0003b640: 0a09 0909 093c 6163 6365 7373 6962 6c65  .....<accessible
+0003b650: 3e4c 696e 5265 6728 6178 2b62 2926 2330  >LinReg(ax+b)&#0
+0003b660: 3332 3b3c 2f61 6363 6573 7369 626c 653e  32;</accessible>
+0003b670: 0d0a 0909 093c 2f6c 616e 673e 0d0a 0909  .....</lang>....
+0003b680: 3c2f 7665 7273 696f 6e3e 0d0a 093c 2f74  </version>...</t
+0003b690: 6f6b 656e 3e0d 0a3c 2f74 6f6b 656e 733e  oken>..</tokens>
+0003b6a0: 0d0a                                     ..
```

### Comparing `tivars-0.9.0/tivars/tokens/scripts/build.py` & `tivars-0.9.1/tivars/tokens/scripts/build.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/tokens/scripts/formats.py` & `tivars-0.9.1/tivars/tokens/scripts/formats.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/tokens/scripts/parse.py` & `tivars-0.9.1/tivars/tokens/scripts/parse.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/tokens/scripts/tokenide.py` & `tivars-0.9.1/tivars/tokens/scripts/tokenide.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/tokens/scripts/trie.py` & `tivars-0.9.1/tivars/tokens/scripts/trie.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/__init__.py` & `tivars-0.9.1/tivars/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/appvar.py` & `tivars-0.9.1/tivars/types/appvar.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/complex.py` & `tivars-0.9.1/tivars/types/complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Complex numeric types
 """
 
 
-from typing import Type
 from warnings import warn
 
 from tivars.data import *
 from tivars.models import *
 from tivars.numeric import *
 from tivars.var import TIEntry
 from .real import *
@@ -75,16 +74,17 @@
         Converts `RealEntry` -> ``bytes``
 
         :param value: The value to convert
         :param instance: The instance containing the data section
         :return: The data of ``value``
         """
 
-        instance.imag_subtype_id = value.subtype_id = value.imag_subtype_id
-        instance.coerce()
+        if instance is not None:
+            instance.imag_subtype_id = value.subtype_id = value.imag_subtype_id
+            instance.coerce()
 
         return type(value).set(value)
 
 
 class ComplexEntry(TIEntry):
     """
     Base class for complex numeric types
@@ -200,23 +200,23 @@
         """
         The sign bit for the complex part
 
         If this bit is set, the complex part is negative.
         """
 
     @property
-    def real_type(self) -> Type['RealEntry']:
+    def real_type(self) -> type['RealEntry']:
         """
         :return: The subclass of `RealEntry` corresponding to this entry's `real_subtype_id`.
         """
 
         return self.get_type(self.real_subtype_id).real_analogue
 
     @property
-    def imag_type(self) -> Type['RealEntry']:
+    def imag_type(self) -> type['RealEntry']:
         """
         :return: The subclass of `RealEntry` corresponding to this entry's `imag_subtype_id`.
         """
 
         return self.get_type(self.imag_subtype_id).real_analogue
 
     def clear(self):
@@ -438,7 +438,11 @@
     flash_only = True
 
     is_exact = True
 
     real_analogue = TIRealPiFraction
 
     _type_id = 0x1F
+
+
+__all__ = ["TIComplex", "TIComplexFraction", "TIComplexRadical", "TIComplexPi", "TIComplexPiFraction",
+           "ComplexEntry", "RealPart", "ImaginaryPart"]
```

### Comparing `tivars-0.9.0/tivars/types/flash.py` & `tivars-0.9.1/tivars/types/flash.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/gdb.py` & `tivars-0.9.1/tivars/types/gdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 GDBs and their settings
 """
 
 
-import io
 import json
 import os
 
-from typing import Iterator
+from collections.abc import Iterator
+from io import BytesIO
 from warnings import catch_warnings, filterwarnings, warn
 
 from tivars.flags import *
 from tivars.data import *
 from tivars.models import *
+from tivars.tokenizer import decode
 from tivars.var import TIEntry, SizedEntry
 from .real import *
 from .tokenized import TIEquation
 
 
 class GraphMode(Flags):
     """
@@ -190,15 +191,15 @@
 
             The ``n``th equation in a GDB is interfaced by the converter ``TIGraphedEquation[n]``.
             """
 
             _T = TIGraphedEquation
 
             @classmethod
-            def get(cls, data: bytes, *, instance=None, **kwargs) -> _T:
+            def get(cls, data: bytes, *, instance=None) -> _T:
                 """
                 Converts ``bytes`` -> `TIGraphedEquation` by finding the equation at ``index`` within a GDB
 
                 :param data: The raw bytes to convert
                 :param instance: The instance which contains the data section
                 :return: The bytes in ``data``, unchanged
                 """
@@ -272,15 +273,23 @@
 
     @View(calc_data, Integer)[1:3]
     def length(self) -> int:
         """
         The length of this entry's user data section
         """
 
-    def load_data_section(self, data: io.BytesIO):
+    @property
+    def json_name(self) -> str:
+        """
+        :return: The name of this equation used in the GDB JSON format
+        """
+
+        return decode(self.raw.name, mode="accessible")[0].strip("{}|")
+
+    def load_data_section(self, data: BytesIO):
         flag_byte = data.read(1)
         data_length = int.from_bytes(length_bytes := data.read(2), 'little')
         self.raw.calc_data = bytearray(flag_byte + length_bytes + data.read(data_length))
 
     @Loader[dict]
     def load_dict(self, dct: dict):
         """
@@ -365,20 +374,23 @@
     extensions = {
         None: "8xd",
         TI_82: "82d",
         TI_83: "83d",
         TI_83P: "8xd"
     }
 
+    min_data_length = 61
+
+    leading_name_byte = b'\x61'
+
     mode_byte = 0x00
     """
     The byte which identifies the GDB type
     """
 
-    min_data_length = 61
     has_color = False
     """
     Whether this GDB type carries color information
     """
 
     num_equations = 0
     """
@@ -518,45 +530,45 @@
         """
         Finds the color portion of a GDB if it exists
 
         :param data: The data to find the color portion of (defaults to this GDB's data)
         :return: The color portion of ``data``, which may be empty
         """
 
-        data = io.BytesIO(data or self.calc_data[self.offset + self.num_styles:])
+        data = BytesIO(data or self.calc_data[self.offset + self.num_styles:])
         temp = TIGraphedEquation()
         for i in range(self.num_equations):
             temp.load_data_section(data)
 
         return data.read()
 
     def get_equations(self, data: bytes = None) -> tuple[TIGraphedEquation, ...]:
         """
         Extracts the equations stored in a GDB into a ``tuple``
 
         :param data: The data to extract equations from (defaults to this GDB's data)
         :return: A ``tuple`` of equations stored in ``data``
         """
 
-        data = io.BytesIO(data or self.calc_data[self.offset:])
+        data = BytesIO(data or self.calc_data[self.offset:])
         equations = tuple(TIGraphedEquation(name=name) for name in self.equation_names)
 
         # Load styles
         for i in range(self.num_styles):
             style = data.read(1)
             for j in range(r := self.num_equations // self.num_styles):
                 equations[r * i + j].raw.style = style
 
         # Load data sections
         for i in range(self.num_equations):
             equations[i].load_data_section(data)
 
         # Load colors (if they exist)
         if rest := data.read():
-            data = io.BytesIO(rest)
+            data = BytesIO(rest)
             data.seek(3, 1)
 
             for i in range(self.num_styles):
                 color = data.read(1)
                 for j in range(r := self.num_equations // self.num_styles):
                     equations[r * i + j].raw.color = color
 
@@ -916,15 +928,15 @@
     def dict(self) -> dict:
         return super().dict() | {
             "specificData": {
                 "settings": {
                     "Xres": int(self.Xres)
                 },
                 "equations": {
-                    equation.name: equation.dict() for equation in self.equations
+                    equation.json_name: equation.dict() for equation in self.equations
                 }
             }
         }
 
 
 class TIFuncGDB(TIGDB, TIMonoFuncGDB):
     """
@@ -1098,15 +1110,15 @@
             "specificData": {
                 "settings": {
                     "Tmin": self.Tmin.json_number(),
                     "Tmax": self.Tmax.json_number(),
                     "Tstep": self.Tstep.json_number(),
                 },
                 "equations": {
-                    equation.name: equation.dict() for equation in self.equations
+                    equation.json_name: equation.dict() for equation in self.equations
                 }
             }
         }
 
 
 class TIParamGDB(TIGDB, TIMonoParamGDB):
     """
@@ -1234,15 +1246,15 @@
             "specificData": {
                 "settings": {
                     "Thetamin": self.Thetamin.json_number(),
                     "Thetamax": self.Thetamax.json_number(),
                     "Thetastep": self.Thetastep.json_number(),
                 },
                 "equations": {
-                    equation.name: equation.dict() for equation in self.equations
+                    equation.json_name: equation.dict() for equation in self.equations
                 }
             }
         }
 
 
 class TIPolarGDB(TIGDB, TIMonoPolarGDB):
     """
@@ -1482,15 +1494,15 @@
                     "unMinp1": self.unMinp1.json_number(),
                     "vnMin": self.vnMinp1.json_number(),
                     "vnMinp1": self.vnMinp1.json_number(),
                     "wnMin": self.wnMin.json_number(),
                     "wnMinp1": self.wnMinp1.json_number()
                 },
                 "equations": {
-                    equation.name: equation.dict() for equation in self.equations
+                    equation.json_name: equation.dict() for equation in self.equations
                 }
             }
         }
 
 
 class TISeqGDB(TIGDB, TIMonoSeqGDB):
     """
```

### Comparing `tivars-0.9.0/tivars/types/group.py` & `tivars-0.9.1/tivars/types/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Groups
 """
 
 
-import io
-
-from typing import Sequence
+from collections.abc import Sequence
+from io import BytesIO
 from warnings import warn
 
 from tivars.data import *
 from tivars.models import *
 from tivars.var import TIEntry, SizedEntry
 from .gdb import TIGraphedEquation
 
@@ -54,14 +53,18 @@
 
         if not entries:
             warn("Groups are expected to be non-empty.",
                  UserWarning)
 
             return TIGroup(name=name)
 
+        elif len(entries) < 2:
+            warn("Groups are expected to have at least two entries.",
+                 UserWarning)
+
         group = TIGroup(for_flash=entries[0].meta_length > TIEntry.base_meta_length, name=name)
 
         for index, entry in enumerate(entries):
             name = entry.raw.name.rstrip(b'\x00')
             vat = bytearray([entry.type_id, 0, entry.version, 0, 0, entry.archived])
 
             if entry.archived:
@@ -80,18 +83,14 @@
 
                 case _:
                     vat += name.ljust(3, b'\x00')
 
             group.data += vat
             group.data += entry.calc_data
 
-        if len(entries) < 2:
-            warn("Groups are expected to have at least two entries.",
-                 UserWarning)
-
         return group
 
     def get_min_os(self, data: bytes = None) -> OsVersion:
         return max([entry.get_min_os() for entry in self.ungroup(data)], default=OsVersions.INITIAL)
 
     def get_version(self, data: bytes = None) -> int:
         return max([entry.get_version() for entry in self.ungroup(data)], default=0x00)
@@ -102,15 +101,15 @@
 
         All VAT data is ignored.
 
         :param data: The data to ungroup (defaults to this group's data)
         :return: A ``list`` of entries stored in ``data``
         """
 
-        data = io.BytesIO(data or self.data[:])
+        data = BytesIO(data or self.data[:])
         entries = []
 
         index = 1
         while type_byte := data.read(1):
             _, version = data.read(2)
 
             match type_id := type_byte[0] & 63:
```

### Comparing `tivars-0.9.0/tivars/types/json/func.default.json` & `tivars-0.9.1/tivars/types/json/func.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/json/param.default.json` & `tivars-0.9.1/tivars/types/json/param.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/json/polar.default.json` & `tivars-0.9.1/tivars/types/json/polar.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/json/seq.default.json` & `tivars-0.9.1/tivars/types/json/seq.default.json`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/list.py` & `tivars-0.9.1/tivars/types/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Lists
 """
 
 
 import re
 
+from collections.abc import Iterator, Sequence
 from io import BytesIO
-from typing import Iterator, Sequence
 from warnings import warn
 
 from tivars.data import *
 from tivars.models import *
 from tivars.tokenizer import *
 from tivars.var import TIEntry
 from .complex import ComplexEntry
@@ -52,27 +52,30 @@
         """
         Converts ``str`` -> ``bytes`` to match appearance in the memory viewer
 
         :param value: The value to convert
         :return: The name encoding of ``value``
         """
 
-        varname = value[:7].upper()
-        varname = re.sub(r"(\u03b8|\u0398|\u03F4|\u1DBF)", "θ", varname)
+        varname = value.upper()
+        varname = re.sub(r"[\u0398\u03F4\u1DBF]", "θ", varname)
         varname = re.sub(r"]", "|L", varname)
-        varname = re.sub(r"[^θa-zA-Z0-9]", "", varname)
+
+        if not re.fullmatch(r"(L\d)|(\|L|.)?([A-Z]|\u03b8)([0-9A-Z]|\u03b8){,4}|IDList", varname):
+            warn(f"List has an invalid name: '{varname}'.",
+                 BytesWarning)
 
         if "IDList" in varname:
-            return b']@'
+            return b'\x5D\x40'
 
-        elif varname.startswith("|L"):
-            return super().set(varname[-5:])
+        elif re.fullmatch(r"L\d", varname):
+            return super().set(varname[:2])
 
         else:
-            return super().set(varname[:2])
+            return super().set(varname[-5:])
 
 
 class ListEntry(TIEntry):
     """
     Base class for all list entries
 
     A list entry is a one-dimensional array of `RealEntry` or `ComplexEntry` elements.
@@ -169,15 +172,16 @@
     def load_list(self, lst: Sequence[_E]):
         """
         Loads a sequence into this list
 
         :param lst: The list to load
         """
 
-        self.load_bytes(int.to_bytes(len(lst), 2, 'little') + b''.join(entry.calc_data for entry in lst))
+        self.length = len(lst)
+        self.data = b''.join(entry.calc_data for entry in lst)
 
     def list(self) -> list[_E]:
         """
         :return: A ``list`` of the elements in this list
         """
 
         it = zip(*[iter(self.data)] * self._E.min_data_length)
```

### Comparing `tivars-0.9.0/tivars/types/matrix.py` & `tivars-0.9.1/tivars/types/matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Matrices
 """
 
 
+from collections.abc import Iterator, Sequence
 from io import BytesIO
-from typing import Iterator, Sequence
 from warnings import warn
 
 from tivars.data import *
 from tivars.models import *
 from tivars.var import TIEntry
 from .real import RealEntry
 
@@ -28,14 +28,16 @@
         TI_82: "82m",
         TI_83: "83m",
         TI_83P: "8xm"
     }
 
     min_data_length = 2
 
+    leading_name_byte = b'\x5C'
+
     _type_id = 0x02
 
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "[A]",
                  version: int = None, archived: bool = None,
                  data: bytes = None):
 
@@ -153,16 +155,17 @@
 
         :param matrix: The matrix to load
         """
 
         if len({len(row) for row in matrix}) > 1:
             raise IndexError("matrix has uneven rows")
 
-        self.load_bytes(bytes([len(matrix[0]), len(matrix)]) +
-                        b''.join(entry.calc_data for row in matrix for entry in row))
+        self.width = len(matrix[0] if matrix else [])
+        self.height = len(matrix)
+        self.data = b''.join(entry.calc_data for row in matrix for entry in row)
 
     def matrix(self) -> list[list[RealEntry]]:
         """
         :return: A two-dimensional ``list`` of the elements in this matrix
         """
 
         it = zip(*[iter(self.data)] * RealEntry.min_data_length)
```

### Comparing `tivars-0.9.0/tivars/types/picture.py` & `tivars-0.9.1/tivars/types/picture.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 Pictures and images
 """
 
 
-from typing import Iterator, Sequence
+import re
+
+
+from collections.abc import Iterator, Sequence
 from warnings import warn
 
 from tivars.data import *
 from tivars.models import *
 from tivars.tokenizer import TokenizedString
 from tivars.var import SizedEntry
 
@@ -246,14 +249,16 @@
 
     pil_mode = "L"
     pixel_type = int
     np_shape = (height, width)
 
     has_color = False
 
+    leading_name_byte = b'\x60'
+
     _type_id = 0x07
 
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "Pic1",
                  version: int = None, archived: bool = True,
                  data: bytes = None):
 
@@ -297,14 +302,16 @@
     data_width = width // 2
     data_height = height
 
     pil_mode = "RGB"
     pixel_type = RGB
     np_shape = (height, width, 3)
 
+    leading_name_byte = b'\x60'
+
     _type_id = 0x07
 
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "Pic1",
                  version: int = None, archived: bool = True,
                  data: bytes = None):
 
@@ -335,14 +342,19 @@
 
     @classmethod
     def get(cls, data: bytes, **kwargs) -> _T:
         return f"Image{data[1] + 1}"
 
     @classmethod
     def set(cls, value: _T, **kwargs) -> bytes:
+        if not re.fullmatch(r"(Image)?\d", value):
+            warn(f"'{value}' is not a valid image name; defaulting to 'Image1'.",
+                 BytesWarning)
+            value = "Image1"
+
         return b"\x3C" + bytes([int(value[-1], 16) - 1])
 
 
 class TIImage(PictureEntry, register=True):
     """
     Parser for color images
 
@@ -369,15 +381,16 @@
     data_width = 2 * width + 2
     data_height = height
 
     pil_mode = "RGB"
     pixel_type = RGB
     np_shape = (height, width, 3)
 
-    leading_bytes = b'\x81'
+    leading_name_byte = b'\x3C'
+    leading_data_bytes = b'\x81'
 
     _type_id = 0x1A
 
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "Image1",
                  version: int = None, archived: bool = True,
                  data: bytes = None):
```

### Comparing `tivars-0.9.0/tivars/types/real.py` & `tivars-0.9.1/tivars/types/real.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Real numeric types
 """
 
 
 import copy
-import decimal as dec
-import fractions as frac
 import re
 
-from typing import Type
+from decimal import Decimal, localcontext
+from fractions import Fraction
 from warnings import warn
 
 from tivars.data import *
 from tivars.models import *
 from tivars.numeric import *
 from tivars.var import TIEntry
 
@@ -110,15 +109,15 @@
         """
         The sign bit for the number
 
         If this bit is used, the number is negative when set.
         """
 
     @property
-    def subtype(self) -> Type['RealEntry']:
+    def subtype(self) -> type['RealEntry']:
         """
         :return: The subtype of this real number
         """
 
         return self.get_type(self.subtype_id)
 
     @property
@@ -144,40 +143,40 @@
 
             case _:
                 return OsVersions.INITIAL
 
     def supported_by(self, model: TIModel) -> bool:
         return super().supported_by(model) and (self.subtype_id <= 0x19 or model.has(TIFeature.ExactMath))
 
-    @Loader[dec.Decimal]
-    def load_decimal(self, decimal: dec.Decimal):
+    @Loader[Decimal]
+    def load_decimal(self, decimal: Decimal):
         """
         Loads a ``decimal`` into this real number
 
         :param decimal: The decimal to load
         """
 
         raise NotImplementedError
 
-    def decimal(self) -> dec.Decimal:
+    def decimal(self) -> Decimal:
         """
         :return: A ``decimal`` object corresponding to this real number
         """
 
         raise NotImplementedError
 
     @Loader[float, int]
     def load_float(self, decimal: float):
         """
         Loads a ``float`` into this real number, upcasting as necessary
 
         :param decimal: The float to load
         """
 
-        self.load_decimal(dec.Decimal(decimal))
+        self.load_decimal(Decimal(decimal))
 
     def json_number(self) -> float | str:
         """
         Encoder for JSON implementations with potentially low precision
 
         :return: A ``float`` or ``str`` depending on whether this real number can be stored in a single-precision float
         """
@@ -251,23 +250,23 @@
     def mantissa(self) -> int:
         """
         The mantissa of the real number
 
         The mantissa is 14 digits stored in BCD format, two digits per byte.
         """
 
-    @Loader[dec.Decimal]
-    def load_decimal(self, decimal: dec.Decimal):
+    @Loader[Decimal]
+    def load_decimal(self, decimal: Decimal):
         self.load_string(str(decimal))
 
-    def decimal(self) -> dec.Decimal:
-        with dec.localcontext() as ctx:
+    def decimal(self) -> Decimal:
+        with localcontext() as ctx:
             ctx.prec = 14
-            decimal = dec.Decimal(self.sign * self.mantissa)
-            decimal *= dec.Decimal(10) ** (self.exponent - 0x80 - 13)
+            decimal = Decimal(self.sign * self.mantissa)
+            decimal *= Decimal(10) ** (self.exponent - 0x80 - 13)
 
         return decimal
 
     @Loader[str]
     def load_string(self, string: str):
         if not string:
             self.mantissa, self.exponent, self.sign_bit = 0, 0x80, False
@@ -344,28 +343,28 @@
 
     is_exact = True
 
     imag_subtype_id = 0x1B
 
     _type_id = 0x18
 
-    @Loader[frac.Fraction]
-    def load_fraction(self, fraction: frac.Fraction):
-        with dec.localcontext() as ctx:
+    @Loader[Fraction]
+    def load_fraction(self, fraction: Fraction):
+        with localcontext() as ctx:
             ctx.prec = 14
-            decimal = dec.Decimal(fraction.numerator) / fraction.denominator
+            decimal = Decimal(fraction.numerator) / fraction.denominator
 
         super().load_string(str(decimal))
 
-    def fraction(self) -> frac.Fraction:
-        return frac.Fraction(self.decimal()).limit_denominator(10000)
+    def fraction(self) -> Fraction:
+        return Fraction(self.decimal()).limit_denominator(10000)
 
     @Loader[str]
     def load_string(self, string: str):
-        self.load_fraction(frac.Fraction(squash(string)))
+        self.load_fraction(Fraction(squash(string)))
 
     def string(self) -> str:
         if self.fraction():
             return "%d / %d" % self.fraction().as_integer_ratio()
 
         else:
             return "0"
@@ -440,21 +439,21 @@
         The left radicand of the real radical
         """
 
     @property
     def sign(self) -> int:
         return -1 if self.decimal() < 0 else 1
 
-    @Loader[dec.Decimal]
-    def load_decimal(self, decimal: dec.Decimal):
+    @Loader[Decimal]
+    def load_decimal(self, decimal: Decimal):
         raise NotImplementedError
 
-    def decimal(self) -> dec.Decimal:
-        return (self.left_scalar * (-1 if self.sign_type % 2 else 1) * dec.Decimal(self.left_radicand).sqrt() +
-                self.right_scalar * (-1 if self.sign_type > 1 else 1) * dec.Decimal(self.right_radicand).sqrt()) \
+    def decimal(self) -> Decimal:
+        return (self.left_scalar * (-1 if self.sign_type % 2 else 1) * Decimal(self.left_radicand).sqrt() +
+                self.right_scalar * (-1 if self.sign_type > 1 else 1) * Decimal(self.right_radicand).sqrt()) \
             / self.denominator
 
     @Loader[str]
     def load_string(self, string: str):
         if not string:
             self.sign_type, self.denominator = 0, 1
             self.left_scalar, self.left_radicand = 0, 0
@@ -591,20 +590,20 @@
 
     is_exact = True
 
     imag_subtype_id = 0x1E
 
     _type_id = 0x20
 
-    @Loader[dec.Decimal]
-    def load_decimal(self, decimal: dec.Decimal):
+    @Loader[Decimal]
+    def load_decimal(self, decimal: Decimal):
         raise NotImplementedError
 
-    def decimal(self) -> dec.Decimal:
-        with dec.localcontext() as ctx:
+    def decimal(self) -> Decimal:
+        with localcontext() as ctx:
             ctx.prec = 14
 
             return super().decimal() * pi
 
     @Loader[str]
     def load_string(self, string: str):
         string = replacer(string, {"pi": "π", "*": ""})
@@ -634,16 +633,16 @@
 
     flash_only = True
 
     imag_subtype_id = 0x1F
 
     _type_id = 0x21
 
-    def fraction(self) -> frac.Fraction:
-        return frac.Fraction(self.decimal() / pi).limit_denominator(10000)
+    def fraction(self) -> Fraction:
+        return Fraction(self.decimal() / pi).limit_denominator(10000)
 
     @Loader[str]
     def load_string(self, string: str):
         replacer(string, {"pi": "π", "*": ""})
 
         if string != "0" and "π" not in string:
             raise ValueError("value must be a fractional multiple of π")
```

### Comparing `tivars-0.9.0/tivars/types/settings.py` & `tivars-0.9.1/tivars/types/settings.py`

 * *Files identical despite different names*

### Comparing `tivars-0.9.0/tivars/types/tokenized.py` & `tivars-0.9.1/tivars/types/tokenized.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,40 +58,40 @@
                 return super().__format__(format_spec)
 
     @staticmethod
     def decode(data: bytes, *, lang: str = "en", mode: str = "display") -> str | bytes:
         """
         Decodes a byte stream into a string of tokens
 
-        Each token is represented using one of three different representations formats, dictated by ``mode``:
-            - ``display``: Represents the tokens with Unicode characters matching the calculator's display
-            - ``accessible``: Represents the tokens with ASCII-only equivalents, often requiring multi-character glyphs
-            - ``ti_ascii``: Represents the tokens with their internal font indices (returns a ``bytes`` object)
+        For detailed information on tokenization modes, see `tivars.tokenizer.decode`.
 
-        :param data: The bytes to decode
+        :param data: The token bytes to decode
         :param lang: The language used in ``string`` (defaults to English, ``en``)
         :param mode: The form of token representation to use for output (defaults to ``display``)
         :return: A string of token representations
         """
 
         return decode(data, lang=lang, mode=mode)[0]
 
     @staticmethod
-    def encode(string: str, *, model: TIModel = None, lang: str = None) -> bytes:
+    def encode(string: str, *, model: TIModel = None, lang: str = None, mode: str = "max") -> bytes:
         """
         Encodes a string of token represented in text into a byte stream
 
-        :param string: The tokens to encode
+        For detailed information on tokenization modes, see `tivars.tokenizer.encode`.
+
+        :param string: The text string to encode
         :param model: The model to target when encoding (defaults to no specific model)
         :param lang: The language used in ``string`` (defaults to English, ``en``)
+        :param mode: The tokenization mode to use (defaults to ``max``)
         :return: A stream of token bytes
         """
 
         model = model or TI_84PCE
-        return encode(string, model.get_trie(lang))[0]
+        return encode(string, trie=model.get_trie(lang), mode=mode)[0]
 
     def get_min_os(self, data: bytes = None) -> OsVersion:
         return decode(data or self.data)[1]
 
     def get_version(self, data: bytes = None) -> int:
         match self.get_min_os(data):
             case os if os >= TI_84PCE.OS("5.3"):
@@ -149,97 +149,57 @@
     def load_string(self, string: str, *, model: TIModel = None, lang: str = None):
         self.data = self.encode(string, model=model, lang=lang)
 
     def string(self) -> str:
         return format(self, "")
 
 
-class EquationName(TokenizedString):
-    """
-    Converter for the name section of equations
-
-    Equation names can be any of the following:
-
-    - ``Y1`` - ``Y0``
-    - ``X1T`` - ``X6T``
-    - ``Y1T`` - ``Y6T``
-    - ``r1`` - ``r6``
-    - ``u``, ``v``, or ``w``.
-    """
-
-    _T = str
-
-    @classmethod
-    def get(cls, data: bytes, **kwargs) -> _T:
-        """
-        Converts ``bytes`` -> ``str`` as done by the memory viewer
-
-        :param data: The raw bytes to convert
-        :return: The equation name contained in ``data``
-        """
-
-        varname = super().get(data)
-
-        if varname.startswith("|"):
-            return varname[1:]
-
-        else:
-            return varname.upper().strip("{}")
-
-    @classmethod
-    def set(cls, value: _T, **kwargs) -> bytes:
-        """
-        Converts ``str`` -> ``bytes`` to match appearance in the memory viewer
-
-        :param value: The value to convert
-        :return: The name encoding of ``value``
-        """
-
-        varname = value[:8].lower()
-
-        if varname.startswith("|") or varname in ("u", "v", "w"):
-            varname = "|" + varname[-1]
-
-        elif varname[0] != "{" and varname[-1] != "}":
-            varname = "{" + varname + "}"
-
-        return super().set(varname)
-
-
 class TIEquation(TokenizedEntry, register=True):
     """
     Parser for equations
 
     A `TIEquation` is a stream of tokens that is evaluated either for graphing or on the homescreen.
     """
 
     extensions = {
         None: "8xy",
         TI_82: "82y",
         TI_83: "83y",
         TI_83P: "8xy"
     }
 
+    leading_name_byte = b'\x5E'
+
     _type_id = 0x03
 
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "Y1",
                  version: int = None, archived: bool = None,
                  data: bytes = None):
 
         super().__init__(init, for_flash=for_flash, name=name, version=version, archived=archived, data=data)
 
-    @Section(8, EquationName)
-    def name(self) -> str:
+    @Section(8, TokenizedString)
+    def name(self, value) -> str:
         """
         The name of the entry
 
-        Must be one of the equation names
+        Must be an equation name used in function, parametric, polar, or sequence mode.
+        (See https://ti-toolkit.github.io/tokens-wiki/categories/Y%3D%20Functions.html)
         """
 
+        varname = value
+        if varname in ("u", "v", "w"):
+            varname = "|" + varname
+
+        elif match := re.fullmatch(r"\{?([XYr]\dT?)}?", varname):
+            varname = "{" + match[1] + "}"
+
+        return varname
+
 
 class TINewEquation(TIEquation, register=True):
     """
     Parser for internal equations
 
     A `TINewEquation` is simply a `TIEquation` with certain internal uses.
     """
@@ -257,36 +217,34 @@
     extensions = {
         None: "8xs",
         TI_82: "82s",
         TI_83: "83s",
         TI_83P: "8xs"
     }
 
+    leading_name_byte = b'\xAA'
+
     _type_id = 0x04
 
     def __init__(self, init=None, *,
                  for_flash: bool = True, name: str = "Str1",
                  version: int = None, archived: bool = None,
                  data: bytes = None):
 
         super().__init__(init, for_flash=for_flash, name=name, version=version, archived=archived, data=data)
 
     @Section(8, TokenizedString)
     def name(self, value) -> str:
         """
         The name of the entry
 
-        Must be one of the string names: ``Str1`` - ``Str0``
+        Must be one of the string names: ``Str1`` - ``Str0``.
         """
 
-        if not re.fullmatch(r"Str\d", varname := value[:4].capitalize()):
-            warn(f"String has an invalid name: {varname}.",
-                 BytesWarning)
-
-        return varname
+        return value.capitalize()
 
     @Loader[str]
     def load_string(self, string: str, *, model: TIModel = None):
         super().load_string(string.strip("\"'"))
 
     def string(self) -> str:
         return f"\"{super().string()}\""
@@ -321,34 +279,14 @@
                   b'\xEF\x7B': TI_84PCE}
     """
     Tokens which identify the program as containing assembly code
     """
 
     _type_id = 0x05
 
-    @Section(8, TokenizedString)
-    def name(self, value) -> str:
-        """
-        The name of the entry
-
-        Names must 1 to 8 characters in length.
-        The name can include any characters A-Z, 0-9, or θ.
-        The name cannot start with a digit.
-        """
-
-        varname = value[:8].upper()
-        varname = re.sub(r"(\u03b8|\u0398|\u03F4|\u1DBF)", "θ", varname)
-        varname = re.sub(r"[^θa-zA-Z0-9]", "", varname)
-
-        if not varname or varname[0].isnumeric():
-            warn(f"Program has an invalid name: {varname}.",
-                 BytesWarning)
-
-        return varname
-
     def protect(self):
         """
         Cast this program to a protected program
         """
 
         self.type_id = 0x06
         self.coerce()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tivars-0.9.0/tivars/var.py` & `tivars-0.9.1/tivars/var.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 """
 The fundamental var components
 """
 
 
+from collections.abc import Iterator
 from io import BytesIO
-from typing import BinaryIO, Iterator, Type
+from sys import version_info
+from typing import BinaryIO
 from warnings import warn
 
 from .data import *
 from .models import *
 from .tokenizer import TokenizedString
 
 
+match version_info[:2]:
+    case 3, 10:
+        Self = 'TIEntry'
+
+    case _:
+        from typing import Self
+
+
 class TIHeader:
     """
     Parser for var file headers
 
     All var files require a header which includes a number of magic bytes, data lengths, and a customizable comment.
     """
 
@@ -37,15 +47,15 @@
             :return: The bytes contained in this header
             """
 
             return self.magic + self.extra + self.product_id + self.comment
 
     def __init__(self, model: TIModel = None, *,
                  magic: str = None, extra: bytes = b'\x1a\x0a', product_id: int = None,
-                 comment: str = "Created with tivars_lib_py v0.9.0",
+                 comment: str = "Created with tivars_lib_py v0.9.1",
                  data: bytes = None):
         """
         Creates an empty header which targets a specified model
 
         :param model: A minimum `TIModel` to target (defaults to ``TI_83P``)
         :param magic: File magic at the start of the header (default to the model's magic)
         :param extra: Extra export bytes for the header (defaults to ``$1a0a``)
@@ -227,14 +237,20 @@
 
 
 class TIEntry(Dock, Converter):
     """
     Base class for all var entries
 
     A var file is made of one or more entries, each of which contain the data of the familiar var types.
+
+    **Even though most var files have just one entry, an entry does NOT constitute a complete var file.**
+    **All var files require an attached header and other metadata.**
+
+    **Use** `TIEntry.export` **to create a new** `TIVar` **containing the entry, with an optional custom header.**
+    **Use** `TIEntry.save` **to export and save the entry in a var file in the current directory.**
     """
 
     _T = 'TIEntry'
 
     flash_only = False
     """
     Whether this entry only supports flash chips
@@ -256,17 +272,22 @@
     min_data_length = 0
     """
     The minimum length of this entry's data
     
     If an entry's data is fixed in size, this value is necessarily the length of the data
     """
 
-    leading_bytes = b''
+    leading_name_byte = b''
+    """
+    Byte that always begins the name of this entry
+    """
+
+    leading_data_bytes = b''
     """
-    Bytes that always occur at the start of this entry's data
+    Bytes that always begin this entry's data
     """
 
     _type_id = None
     _type_ids = {}
 
     class Raw:
         """
@@ -374,15 +395,15 @@
     def __bytes__(self) -> bytes:
         """
         :return: The bytes contained in this entry
         """
 
         return self.bytes()
 
-    def __copy__(self) -> 'TIEntry':
+    def __copy__(self) -> Self:
         """
         :return: A copy of this entry
         """
 
         new = self.__class__()
         new.load_bytes(self.bytes())
         return new
@@ -542,15 +563,15 @@
         """
         :return: The meta section of this entry
         """
 
         return self.raw.calc_data_length + self.raw.type_id + self.raw.name + self.raw.version + self.raw.archived
 
     @classmethod
-    def get_type(cls, type_id: int) -> Type['TIEntry']:
+    def get_type(cls, type_id: int) -> type['TIEntry'] | None:
         """
         Gets the subclass corresponding to a type ID if one is registered
 
         :param type_id: The type ID to search by
         :return: A subclass of `TIEntry` with corresponding type ID or ``None``
         """
 
@@ -568,15 +589,15 @@
         meta_length = int.from_bytes(stream.read(2), 'little')
         data_length = int.from_bytes(stream.read(2), 'little')
         stream.seek(-4, 1)
 
         return 2 + meta_length + 2 + data_length
 
     @classmethod
-    def register(cls, var_type: Type['TIEntry'], override: int = None):
+    def register(cls, var_type: type['TIEntry'], override: int = None):
         """
         Registers a subtype with this class for coercion
 
         :param var_type: The `TIEntry` subtype to register
         :param override: A type ID to use for registry that differs from that of the var type
         """
 
@@ -593,15 +614,15 @@
             raise TypeError("entry does not support archiving.")
 
     def clear(self):
         """
         Clears this entry's data
         """
 
-        self.raw.calc_data = bytearray(self.leading_bytes)
+        self.raw.calc_data = bytearray(self.leading_data_bytes)
         self.raw.calc_data.extend(bytearray(self.min_data_length - self.calc_data_length))
 
     def get_min_os(self, data: bytes = None) -> OsVersion:
         """
         Determines the minimum OS that supports this entry's data
 
         :param data: The data to find the minimum support for (defaults to this entry's data)
@@ -725,14 +746,18 @@
 
         if self.versions != [0x00] and self.version not in self.versions:
             warn(f"The version (0x{self.version:02x}) is not recognized.",
                  BytesWarning)
 
     def bytes(self) -> bytes:
         """
+        The bytes contained in this entry, without any var file header or metadata.
+
+        **These bytes do NOT constitute a complete var file. Use** `.export` **and** `.save` **to save a var file.**
+
         :return: The bytes contained in this entry
         """
 
         return self.raw.bytes()
 
     def load_data_section(self, data: BytesIO):
         """
@@ -794,46 +819,54 @@
         """
         :return: A string representation of this entry
         """
 
         raise NotImplementedError
 
     @classmethod
-    def open(cls, filename: str) -> 'TIEntry':
+    def open(cls, filename: str) -> Self:
         """
         Creates a new entry from a file given a filename
 
         :param filename: A filename to open
         :return: The (first) entry stored in the file
         """
 
         if cls._type_id is not None and \
                 not any(filename.endswith(extension) for extension in cls.extensions.values()):
             warn(f"File extension .{filename.split('.')[-1]} not recognized for var type {cls}; "
                  f"attempting to read anyway.",
                  UserWarning)
 
         with open(filename, 'rb') as file:
-            file.seek(55)
+            # Use header for sanity check
+            header = TIHeader()
+            header.load_from_file(file)
+            file.seek(2, 1)
 
             entry = cls()
             entry.load_bytes(file.read(cls.next_entry_length(file)))
 
             file.seek(2, 1)
 
-            if file.read():
-                warn("The selected var file contains multiple entries; only the first will be loaded. "
-                     "Use load_from_file to select a particular entry, or load the entire file into a TIVar object.",
-                     UserWarning)
+            if remaining := file.read():
+                if remaining.startswith(b"\x0B\x00") or remaining.startswith(b"\x0D\x00"):
+                    warn("The selected var file contains multiple entries; only the first will be loaded. "
+                         "Use load_from_file to select a particular entry, or load the entire file into a TIVar object.",
+                         UserWarning)
+
+                else:
+                    warn(f"The selected var file contains unexpected additional data: {remaining}.",
+                         BytesWarning)
 
         return entry
 
     def save(self, filename: str = None, *, header: TIHeader = None, model: TIModel = None):
         """
-        Saves this entry as a var file given a filename and optional header and targeted model
+        Saves this entry as a var file in the current directory given a filename and optional header and targeted model
 
         :param filename: A filename to save to (defaults to the var's name and extension)
         :param header: A `TIHeader` to attach (defaults to an empty header)
         :param model: A `TIModel` to target (defaults to ``None``)
         """
 
         self.export(header=header, model=model).save(filename)
@@ -1200,23 +1233,23 @@
         """
 
     @View(calc_data, SizedData)[2:]
     def data(self) -> bytes:
         pass
 
     def clear(self):
-        self.raw.calc_data = bytearray([0, 0, *self.leading_bytes])
+        self.raw.calc_data = bytearray([0, 0, *self.leading_data_bytes])
         self.raw.calc_data.extend(bytearray(self.min_data_length - self.calc_data_length))
-        self.length = len(self.leading_bytes) + len(self.data)
+        self.length = len(self.leading_data_bytes) + len(self.data)
 
     @Loader[bytes, bytearray, BytesIO]
     def load_bytes(self, data: bytes | BytesIO):
         super().load_bytes(data)
 
-        if self.length != (data_length := len(self.leading_bytes) + len(self.data)):
+        if self.length != (data_length := len(self.leading_data_bytes) + len(self.data)):
             warn(f"The entry has an unexpected data length (expected {self.length}, got {data_length}).",
                  BytesWarning)
 
     def load_data_section(self, data: BytesIO):
         data_length = int.from_bytes(length_bytes := data.read(2), 'little')
         self.raw.calc_data = bytearray(length_bytes + data.read(data_length))
```

### Comparing `tivars-0.9.0/tivars.egg-info/PKG-INFO` & `tivars-0.9.1/tivars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tivars
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for interacting with TI-(e)z80 (82/83/84 series) calculator files
 License: The MIT License (MIT)
         
         Copyright (c) 2023 kg583
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -39,15 +39,15 @@
 
 `tivars_lib_py` is a Python package for interacting with TI-(e)z80 (82/83/84 series) calculator files, i.e. lists, programs, matrices, appvars, etc.
 
 Much of the functionality of this package has been ported over from [tivars_lib_cpp](https://github.com/adriweb/tivars_lib_cpp). However, a number of changes have been made to the API to better suit Python's strengths and capabilities as a language (e.g. scripting, dynamic typing).
 
 ## Installation
 
-The current release version is `v0.9.0`. All versions require Python 3.10+ to run.
+The current release version is `v0.9.1`. All versions require Python 3.10+ to run.
 
 ### As a Package
 
 Install the `tivars` package from PyPI using `pip`:
 ```
 pip install tivars
 ```
```

### Comparing `tivars-0.9.0/tivars.egg-info/SOURCES.txt` & `tivars-0.9.1/tivars.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 tivars/PIL/TI8xiPlugin.py
 tivars/PIL/__init__.py
 tivars/PIL/common.py
 tivars/models/__init__.py
 tivars/models/model.py
 tivars/models/versions.py
 tivars/tokenizer/__init__.py
+tivars/tokenizer/decoder.py
+tivars/tokenizer/encoder.py
+tivars/tokenizer/state.py
 tivars/tokens/73.xml
 tivars/tokens/8X.xml
 tivars/tokens/scripts/__init__.py
 tivars/tokens/scripts/build.py
 tivars/tokens/scripts/formats.py
 tivars/tokens/scripts/parse.py
 tivars/tokens/scripts/tokenide.py
```

