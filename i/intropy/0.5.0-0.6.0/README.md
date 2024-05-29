# Comparing `tmp/intropy-0.5.0.tar.gz` & `tmp/intropy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intropy-0.5.0.tar", last modified: Tue May  7 22:25:13 2024, max compression
+gzip compressed data, was "intropy-0.6.0.tar", last modified: Wed May 29 22:13:14 2024, max compression
```

## Comparing `intropy-0.5.0.tar` & `intropy-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 22:25:10.000000 intropy-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-07 22:25:13.738426 intropy-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-07 22:25:10.000000 intropy-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/intropy/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-07 22:25:10.000000 intropy-0.5.0/intropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-07 22:25:10.000000 intropy-0.5.0/intropy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/intropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 22:25:13.000000 intropy-0.5.0/intropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-07 22:25:10.000000 intropy-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:25:13.738426 intropy-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:25:13.738426 intropy-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-07 22:25:10.000000 intropy-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-07 22:25:10.000000 intropy-0.5.0/tests/test_cookiecutter.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-07 22:25:10.000000 intropy-0.5.0/tests/test_generated_project_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:13:14.162217 intropy-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 22:12:54.000000 intropy-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-29 22:13:14.162217 intropy-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-29 22:12:54.000000 intropy-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:13:14.158217 intropy-0.6.0/intropy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-29 22:12:54.000000 intropy-0.6.0/intropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-29 22:12:54.000000 intropy-0.6.0/intropy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:13:14.158217 intropy-0.6.0/intropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-29 22:13:14.000000 intropy-0.6.0/intropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-29 22:13:14.000000 intropy-0.6.0/intropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:13:14.000000 intropy-0.6.0/intropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-29 22:13:14.000000 intropy-0.6.0/intropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-29 22:13:14.000000 intropy-0.6.0/intropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 22:13:14.000000 intropy-0.6.0/intropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-29 22:12:54.000000 intropy-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:13:14.162217 intropy-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:13:14.158217 intropy-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-29 22:12:54.000000 intropy-0.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-29 22:12:54.000000 intropy-0.6.0/tests/test_cookiecutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-29 22:12:54.000000 intropy-0.6.0/tests/test_generated_project_test_suite.py
```

### Comparing `intropy-0.5.0/LICENSE` & `intropy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intropy-0.5.0/PKG-INFO` & `intropy-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intropy
-Version: 0.5.0
+Version: 0.6.0
 Summary: Jump-start your python project
 License: MIT License
         
         Copyright (c) 2024 Richard Nordström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `intropy-0.5.0/README.md` & `intropy-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `intropy-0.5.0/intropy/__init__.py` & `intropy-0.6.0/intropy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 import logging
 import logging.config
 import time
 
 INTROPY_ROOT_LOGGER = logging.getLogger(__name__)
```

### Comparing `intropy-0.5.0/intropy/cli.py` & `intropy-0.6.0/intropy/cli.py`

 * *Files identical despite different names*

### Comparing `intropy-0.5.0/intropy.egg-info/PKG-INFO` & `intropy-0.6.0/intropy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intropy
-Version: 0.5.0
+Version: 0.6.0
 Summary: Jump-start your python project
 License: MIT License
         
         Copyright (c) 2024 Richard Nordström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `intropy-0.5.0/pyproject.toml` & `intropy-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     # Dont complain typing
     "@(typing(_extensions)?\\.)?overload",
     "if (typing(_extensions)?\\.)?TYPE_CHECKING:",
 ]
 
 [tool.bumpversion]
-current_version = "0.5.0"
+current_version = "0.6.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 ignore_missing_files = false
```

### Comparing `intropy-0.5.0/tests/test_cli.py` & `intropy-0.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `intropy-0.5.0/tests/test_cookiecutter.py` & `intropy-0.6.0/tests/test_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `intropy-0.5.0/tests/test_generated_project_test_suite.py` & `intropy-0.6.0/tests/test_generated_project_test_suite.py`

 * *Files identical despite different names*

