# Comparing `tmp/yappr-1.0.6.tar.gz` & `tmp/yappr-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yappr-1.0.6.tar", last modified: Tue May  7 13:07:26 2024, max compression
+gzip compressed data, was "yappr-1.0.7.tar", last modified: Thu May 30 07:19:19 2024, max compression
```

## Comparing `yappr-1.0.6.tar` & `yappr-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:26.379246 yappr-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 13:07:19.000000 yappr-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 13:07:19.000000 yappr-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-07 13:07:26.379246 yappr-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 13:07:19.000000 yappr-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 13:07:19.000000 yappr-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:07:26.379246 yappr-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:26.379246 yappr-1.0.6/yappr/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 13:07:19.000000 yappr-1.0.6/yappr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-07 13:07:19.000000 yappr-1.0.6/yappr/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-07 13:07:19.000000 yappr-1.0.6/yappr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:19.000000 yappr-1.0.6/yappr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-07 13:07:19.000000 yappr-1.0.6/yappr/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:07:26.379246 yappr-1.0.6/yappr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-07 13:07:26.000000 yappr-1.0.6/yappr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 13:07:26.000000 yappr-1.0.6/yappr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:07:26.000000 yappr-1.0.6/yappr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 13:07:26.000000 yappr-1.0.6/yappr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:19:19.002410 yappr-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-30 07:19:12.000000 yappr-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 07:19:12.000000 yappr-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-30 07:19:18.998410 yappr-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-30 07:19:12.000000 yappr-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-30 07:19:12.000000 yappr-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:19:19.002410 yappr-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:19:18.998410 yappr-1.0.7/yappr/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 07:19:12.000000 yappr-1.0.7/yappr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-30 07:19:12.000000 yappr-1.0.7/yappr/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-30 07:19:12.000000 yappr-1.0.7/yappr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 07:19:12.000000 yappr-1.0.7/yappr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-30 07:19:12.000000 yappr-1.0.7/yappr/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:19:18.998410 yappr-1.0.7/yappr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-30 07:19:18.000000 yappr-1.0.7/yappr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 07:19:18.000000 yappr-1.0.7/yappr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:19:18.000000 yappr-1.0.7/yappr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 07:19:18.000000 yappr-1.0.7/yappr.egg-info/top_level.txt
```

### Comparing `yappr-1.0.6/LICENSE` & `yappr-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yappr-1.0.6/PKG-INFO` & `yappr-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappr
-Version: 1.0.6
+Version: 1.0.7
 Summary: Yet another python package updater
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `yappr-1.0.6/README.md` & `yappr-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `yappr-1.0.6/pyproject.toml` & `yappr-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yappr"
-version = "1.0.6"
+version = "1.0.7"
 dependencies = []
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Yet another python package updater"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

### Comparing `yappr-1.0.6/yappr/decorator.py` & `yappr-1.0.7/yappr/decorator.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,18 +22,21 @@
     def decorator(
         func: Callable[Param, Any],
     ) -> Callable[Param, None]:
 
         def wrapped(*args: Param.args, **kwargs: Param.kwargs) -> None:
             # Initialize updater, updater needs to start as
             # soon as the script starts
-            parser = ArgumentParser()
+            parser = ArgumentParser(add_help=False)
             parser.add_argument("--no-updater", action="store_true")
-            cmd_args, _ = parser.parse_known_args(["--no-updater"])
-            if not cmd_args.no_updater:
+            parser.add_argument("-h", "--help", action="store_true")
+            parser.add_argument("-v", "--version", action="store_true")
+            cmd_args, _ = parser.parse_known_args()
+            # do not run updater on help or version command
+            if not (cmd_args.no_updater or cmd_args.help or cmd_args.version):
                 Thread(target=updater.check_for_updates_loop).start()
 
             while True:
                 try:
                     # Import non-standard libraries only after
                     # updater script has started
                     out = func(*args, **kwargs)
```

### Comparing `yappr-1.0.6/yappr/logger.py` & `yappr-1.0.7/yappr/logger.py`

 * *Files identical despite different names*

### Comparing `yappr-1.0.6/yappr/updater.py` & `yappr-1.0.7/yappr/updater.py`

 * *Files identical despite different names*

### Comparing `yappr-1.0.6/yappr.egg-info/PKG-INFO` & `yappr-1.0.7/yappr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yappr
-Version: 1.0.6
+Version: 1.0.7
 Summary: Yet another python package updater
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

