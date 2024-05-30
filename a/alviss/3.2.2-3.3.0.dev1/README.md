# Comparing `tmp/alviss-3.2.2.tar.gz` & `tmp/alviss-3.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alviss-3.2.2.tar", last modified: Mon May  6 13:44:24 2024, max compression
+gzip compressed data, was "alviss-3.3.0.dev1.tar", last modified: Thu May 30 11:27:37 2024, max compression
```

## Comparing `alviss-3.2.2.tar` & `alviss-3.3.0.dev1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.147643 alviss-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 13:44:08.000000 alviss-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-06 13:44:24.147643 alviss-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-06 13:44:08.000000 alviss-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/cli/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/render/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.139643 alviss-3.2.2/alviss/cli/stubber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/stubber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/cli/stubber/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/autoloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17478 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/jsonfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/loaders/yamlfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/quickloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/renderers/static/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/static/_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/renderers/static/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/structs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/cfgstub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/structs/singletonconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/stubber/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/stubber/stubmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/stubber/stubmaker/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-06 13:44:08.000000 alviss-3.2.2/alviss/utils/kwfields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:44:24.143643 alviss-3.2.2/alviss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 13:44:24.000000 alviss-3.2.2/alviss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-06 13:44:08.000000 alviss-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:44:24.147643 alviss-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-06 13:44:08.000000 alviss-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.171177 alviss-3.3.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-30 11:27:37.171177 alviss-3.3.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.163177 alviss-3.3.0.dev1/alviss/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/cli/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/cli/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/cli/render/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/cli/stubber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/cli/stubber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/cli/stubber/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/loaders/autoloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/loaders/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/loaders/jsonfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/loaders/yamlfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/quickloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/renderers/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/renderers/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/renderers/static/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/renderers/static/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/structs/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/structs/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/structs/cfgstub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/structs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/structs/singletonconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.167177 alviss-3.3.0.dev1/alviss/stubber/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/stubber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.171177 alviss-3.3.0.dev1/alviss/stubber/stubmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/stubber/stubmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/stubber/stubmaker/_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10606 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/stubber/stubmaker/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/stubber/stubmaker/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.171177 alviss-3.3.0.dev1/alviss/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/alviss/utils/kwfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:27:37.171177 alviss-3.3.0.dev1/alviss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-30 11:27:37.000000 alviss-3.3.0.dev1/alviss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-30 11:27:37.000000 alviss-3.3.0.dev1/alviss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:27:37.000000 alviss-3.3.0.dev1/alviss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-30 11:27:37.000000 alviss-3.3.0.dev1/alviss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 11:27:37.000000 alviss-3.3.0.dev1/alviss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 11:27:37.000000 alviss-3.3.0.dev1/alviss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:27:37.171177 alviss-3.3.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-30 11:27:27.000000 alviss-3.3.0.dev1/setup.py
```

### Comparing `alviss-3.2.2/LICENSE` & `alviss-3.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/PKG-INFO` & `alviss-3.3.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alviss
-Version: 3.2.2
+Version: 3.3.0.dev1
 Summary: Configuration file reader with some nifty bells and whistles added
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alviss-3.2.2/README.md` & `alviss-3.3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/cli/render/main.py` & `alviss-3.3.0.dev1/alviss/cli/render/main.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/cli/stubber/main.py` & `alviss-3.3.0.dev1/alviss/cli/stubber/main.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/loaders/autoloader.py` & `alviss-3.3.0.dev1/alviss/loaders/autoloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,33 +25,35 @@
     ext = os.path.splitext(file_name)[-1]
     loader = _EXTENSION_LOADER_MAP.get(ext, None)
     if not loader:
         raise AlvissUnknownFileTypeError(f'Dont know how to autoload file extension {ext}', file_name=file_name)
     return loader
 
 
-def raw_load(file_name: str, skip_env_loading: bool = False, skip_fidelius: bool = False, encoding: str = 'utf-8') -> Dict:
+def raw_load(file_name: str, skip_env_loading: bool = False, skip_fidelius: bool = False, skip_py_inject: bool = False, encoding: str = 'utf-8') -> Dict:
     """Loads and parses the given config file and returns the "raw" results as a
     simple python dictionary.
 
     This is mostly intended for the testing and debugging of the configuration
     files themselves if needed.
 
     :param file_name: The file to load
     :param skip_env_loading: Set to True to skip resolving environment variable tags
     :param skip_fidelius: Set to True to skip resolving Fidelius tags
+    :param skip_py_inject: Set to True to skip injecting Python imported values
     :param encoding: Encoding to use when reading the file (utf-8 by default)
     :return: A dict with the results
     """
     loader = guess_loader_class(file_name)()
-    loader.load_file(file_name, no_env_load=skip_env_loading, no_fidelius=skip_fidelius, encoding=encoding)
+    loader.load_file(file_name, no_env_load=skip_env_loading, no_fidelius=skip_fidelius,
+                     no_py_inject=skip_py_inject, encoding=encoding)
     return loader.data
 
 
-def render_load(file_name: str, skip_env_loading: bool = True, skip_fidelius: bool = True, encoding: str = 'utf-8') -> str:
+def render_load(file_name: str, skip_env_loading: bool = True, skip_fidelius: bool = True, skip_py_inject: bool = True, encoding: str = 'utf-8') -> str:
     """Loads and parses the given config file and returns the "render" results
     as a str in the same format the original file used.
 
     The main point of this method is to be able to load and parse an Alviss
     configuration file, including all includes, extensions, internal references,
     environment variables, Fidelius values etc. and render as a single
     value/file of the same format.
@@ -61,20 +63,21 @@
     (i.e. includes, internal references, secret injection via Fidelius during
     deployment and so on).
 
     :param file_name: The file to load
     :param skip_env_loading: Set to True to skip resolving environment variable
                              tags
     :param skip_fidelius: Set to True to skip resolving Fidelius tags
+    :param skip_py_inject: Set to True to skip injecting Python imported values
     :param encoding: Encoding to use when reading the file (utf-8 by default)
     :return: A string representation of the configuration data loaded, in the
              same format as the target file if possible
     """
     loader = guess_loader_class(file_name)()
-    loader.load_file(file_name, no_env_load=skip_env_loading, no_fidelius=skip_fidelius, encoding=encoding)
+    loader.load_file(file_name, no_env_load=skip_env_loading, no_fidelius=skip_fidelius, no_py_inject=skip_py_inject, encoding=encoding)
     return loader.rendered
 
 
 def autoload(file_name: str, encoding: str = 'utf-8') -> BaseConfig:
     """Loads and parses the given config file and returns as a `BaseConfig`
     object.
```

### Comparing `alviss-3.2.2/alviss/loaders/base.py` & `alviss-3.3.0.dev1/alviss/loaders/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = [
     'BaseLoader',
 ]
 
 from alviss.structs import *
 from .interface import *
 from ccptools.tpu import iters
+from ccptools.tpu import strimp
 import os
 import logging
 log = logging.getLogger(__file__)
 
 
 _VAR_PATTERN = re.compile(r'\$\{(?P<var>(?:[^=}\s]+)(?:!?=[^}]*)?)}')
 
@@ -34,14 +35,15 @@
         }
 
         self._skip_resolve: bool = False
         self._skip_env_loading: bool = False
         self._skip_includes: bool = False
         self._skip_extends: bool = False
         self._skip_fidelius: bool = False
+        self._skip_py_inject: bool = False
 
         self._fidelius_keys: Dict[Sequence[str], str] = {}
         self._fidelius_mode: FideliusMode = FideliusMode.ON_DEMAND
         self._fidelius_kwargs: Optional[Dict[str, Any]] = None
         self._find_fidelius_mode()
 
     def set_fidelius_mode(self, mode: Union[FideliusMode, str, int]):
@@ -69,20 +71,22 @@
     def load_file(self,
                   file_name: str,
                   no_resolve: bool = False,
                   no_extend: bool = False,
                   no_includes: bool = False,
                   no_env_load: bool = False,
                   no_fidelius: bool = False,
+                  no_py_inject: bool = False,
                   encoding: str = 'utf-8'):
         self._skip_resolve = no_resolve
         self._skip_env_loading = no_env_load
         self._skip_includes = no_includes
         self._skip_extends = no_extend
         self._skip_fidelius = no_fidelius
+        self._skip_py_inject = no_py_inject
 
         self._file_name = os.path.basename(file_name)
         self._file_path = os.path.dirname(os.path.abspath(file_name))
         if not os.path.exists(file_name):
             raise AlvissFileNotFoundError('File not found', file_name=file_name)
 
         with open(file_name, 'r', encoding=encoding) as fin:
@@ -349,19 +353,38 @@
                 if val is not None:
                     self._resolve_count += 1
                     return val
                 return match.group(0)
 
             self._fidelius_keys[tuple(path)] = match.group(0)
 
+        if not self._skip_py_inject and key.startswith('__PY__:'):
+            val = self._py_inject(key)
+            if val is not None:
+                if val == '' and key.strip().endswith('!='):
+                    return None  # Still unresolved
+                self._resolve_count += 1
+                return val
+            return match.group(0)
+
         val = self._get_str_key(key)
         if val is not None:
             self._resolve_count += 1
         return val
 
+    def _py_inject(self, key: str) -> Any:
+        default = None
+        if '=' in key:
+            key, default = key.split('=', 2)
+            if isinstance(key, str):
+                if key.endswith('!'):
+                    key = key[0:-1]
+
+        return strimp.get_any(key[7:], default)
+
     def _get_str_key(self, key: str) -> Optional[str]:
         return iters.nested_get(self._data, key.split('.'))
 
     def _special_key_extends(self, value: Union[str, List[str]], path: List[str]):
         if not isinstance(value, list):
             value = [value]
         self._extends.extend([(v, tuple(path[:-1])) for v in value])
```

### Comparing `alviss-3.2.2/alviss/loaders/interface.py` & `alviss-3.3.0.dev1/alviss/loaders/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,35 +40,37 @@
     def load_file(self,
                   file_name: str,
                   no_resolve: bool = False,
                   no_extend: bool = False,
                   no_includes: bool = False,
                   no_env_load: bool = False,
                   no_fidelius: bool = False,
+                  no_py_inject: bool = False,
                   encoding: str = 'utf-8'):
         """Loads a config file.
 
         :param file_name: The file to load.
         :param no_resolve: Skips resolving any special tags
         :param no_extend:
         :param no_includes:
         :param no_env_load:
         :param no_fidelius:
+        :param no_py_inject:
         :param encoding:
         """
         pass
 
     # @abc.abstractmethod
     # def load_url(self, url: str):
     #     pass
 
     @abc.abstractmethod
     def load_raw(self, raw_data: str, no_resolve: bool = False,
                  no_extend: bool = False, no_includes: bool = False, no_env_load: bool = False,
-                 no_fidelius: bool = False):
+                 no_fidelius: bool = False, no_py_inject: bool = False):
         """Loads configuration data directly from a string.
 
         The `load_file` method basically just reads a file and passes its
         content to this method in most cases."""
         pass
 
     @property
```

### Comparing `alviss-3.2.2/alviss/loaders/jsonfile.py` & `alviss-3.3.0.dev1/alviss/loaders/jsonfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,22 @@
         return ldr.data
 
     # def load_url(self, url: str):
     #     pass
 
     def load_raw(self, raw_data: str, no_resolve: bool = False,
                  no_extend: bool = False, no_includes: bool = False, no_env_load: bool = False,
-                 no_fidelius: bool = False):
+                 no_fidelius: bool = False, no_py_inject: bool = False):
+        self._skip_resolve = no_resolve
+        self._skip_env_loading = no_env_load
+        self._skip_includes = no_includes
+        self._skip_extends = no_extend
+        self._skip_fidelius = no_fidelius
+        self._skip_py_inject = no_py_inject
+
         self._data = self._load_dict(json.loads(raw_data))
         self._set_chains()
         if not no_extend:
             self._extend()
         if not no_includes:
             self._includes()
         if not no_resolve:
```

### Comparing `alviss-3.2.2/alviss/loaders/yamlfile.py` & `alviss-3.3.0.dev1/alviss/loaders/yamlfile.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 import logging
 log = logging.getLogger(__name__)
 
 
 class YamlFileConfigLoader(BaseLoader):
     def load_raw(self, raw_data: str, no_resolve: bool = False,
                  no_extend: bool = False, no_includes: bool = False, no_env_load: bool = False,
-                 no_fidelius: bool = False):
+                 no_fidelius: bool = False, no_py_inject: bool = False):
+        self._skip_resolve = no_resolve
+        self._skip_env_loading = no_env_load
+        self._skip_includes = no_includes
+        self._skip_extends = no_extend
+        self._skip_fidelius = no_fidelius
+        self._skip_py_inject = no_py_inject
         self._data = self._load_dict(yaml.safe_load(raw_data))
         self._set_chains()
         if not no_extend:
             self._extend()
         if not no_includes:
             self._includes()
         if not no_resolve:
```

### Comparing `alviss-3.2.2/alviss/renderers/static/_simple.py` & `alviss-3.3.0.dev1/alviss/renderers/static/_simple.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/renderers/static/interface.py` & `alviss-3.3.0.dev1/alviss/renderers/static/interface.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/structs/baseconfig.py` & `alviss-3.3.0.dev1/alviss/structs/baseconfig.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/structs/errors.py` & `alviss-3.3.0.dev1/alviss/structs/errors.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/stubber/stubmaker/_simple.py` & `alviss-3.3.0.dev1/alviss/stubber/stubmaker/_simple.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/stubber/stubmaker/_structs.py` & `alviss-3.3.0.dev1/alviss/stubber/stubmaker/_structs.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/stubber/stubmaker/interface.py` & `alviss-3.3.0.dev1/alviss/stubber/stubmaker/interface.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss/utils/kwfields.py` & `alviss-3.3.0.dev1/alviss/utils/kwfields.py`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/alviss.egg-info/PKG-INFO` & `alviss-3.3.0.dev1/alviss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alviss
-Version: 3.2.2
+Version: 3.3.0.dev1
 Summary: Configuration file reader with some nifty bells and whistles added
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alviss-3.2.2/alviss.egg-info/SOURCES.txt` & `alviss-3.3.0.dev1/alviss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alviss-3.2.2/pyproject.toml` & `alviss-3.3.0.dev1/pyproject.toml`

 * *Files identical despite different names*

