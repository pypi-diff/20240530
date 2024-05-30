# Comparing `tmp/lemniscat.runtime-0.5.2.tar.gz` & `tmp/lemniscat_runtime-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemniscat.runtime-0.5.2.tar", last modified: Sun Mar 24 18:29:04 2024, max compression
+gzip compressed data, was "lemniscat_runtime-0.6.0.tar", last modified: Thu May 30 08:36:13 2024, max compression
```

## Comparing `lemniscat.runtime-0.5.2.tar` & `lemniscat_runtime-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.104556 lemniscat.runtime-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-24 18:29:04.100556 lemniscat.runtime-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-24 18:29:00.000000 lemniscat.runtime-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:29:04.104556 lemniscat.runtime-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.096557 lemniscat.runtime-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.096557 lemniscat.runtime-0.5.2/src/lemniscat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.100556 lemniscat.runtime-0.5.2/src/lemniscat/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.100556 lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/engine_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/engine_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/engine_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/lem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.100556 lemniscat.runtime-0.5.2/src/lemniscat/runtime/model/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/model/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.100556 lemniscat.runtime-0.5.2/src/lemniscat/runtime/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/plugin/pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-24 18:28:55.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/plugin/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-24 18:28:59.000000 lemniscat.runtime-0.5.2/src/lemniscat/runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:29:04.100556 lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-24 18:29:04.000000 lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-24 18:29:04.000000 lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:29:04.000000 lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-24 18:29:04.000000 lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-24 18:29:04.000000 lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-24 18:29:04.000000 lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-30 08:36:09.000000 lemniscat_runtime-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.416681 lemniscat_runtime-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.416681 lemniscat_runtime-0.6.0/src/lemniscat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/src/lemniscat/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/engine_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/engine_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/engine_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/lem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/src/lemniscat/runtime/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/model/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/src/lemniscat/runtime/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/plugin/pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-30 08:35:58.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/plugin/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 08:36:08.000000 lemniscat_runtime-0.6.0/src/lemniscat/runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 08:36:13.420681 lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-30 08:36:13.000000 lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-30 08:36:13.000000 lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 08:36:13.000000 lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 08:36:13.000000 lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 08:36:13.000000 lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 08:36:13.000000 lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/top_level.txt
```

### Comparing `lemniscat.runtime-0.5.2/LICENSE` & `lemniscat_runtime-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lemniscat.runtime-0.5.2/PKG-INFO` & `lemniscat_runtime-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemniscat.runtime
-Version: 0.5.2
+Version: 0.6.0
 Summary: A runtime to provide product oriented in DevOps approach
 Author-email: Philippe MORISSEAU <philippe.morisseau@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lemniscat-devops/lemniscat.runtime
 Project-URL: Issues, https://github.com/lemniscat-devops/lemniscat.runtime/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lemniscat.runtime-0.5.2/pyproject.toml` & `lemniscat_runtime-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lemniscat.runtime"
-version = "0.5.2"
+version = "0.6.0"
 authors = [
   { name="Philippe MORISSEAU", email="philippe.morisseau@outlook.com" },
 ]
 description = "A runtime to provide product oriented in DevOps approach"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
```

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/engine_manifest.py` & `lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/engine_manifest.py`

 * *Files identical despite different names*

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/engine_runtime.py` & `lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/engine_runtime.py`

 * *Files identical despite different names*

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat/runtime/engine/engine_variables.py` & `lemniscat_runtime-0.6.0/src/lemniscat/runtime/engine/engine_variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,25 @@
         
         self._logger = logger
         self._logger.info("Loading variables")
         conf = args[0]['configFiles']
         configFiles = ast.literal_eval(conf)
         for file in configFiles:
             self._logger.debug(f"Loading variables from file: {file}...")
-            with open(file, 'r') as f:
-                variables = json.load(f)
-            for key in variables:
-                self._variables[key] = VariableValue(variables[key])
-            self._logger.debug(f"{len(variables)} loaded.")    
+            if(file.endswith('.json')):
+                with open(file, 'r') as f:
+                    variables = json.load(f)
+                for key in variables:
+                    self._variables[key] = VariableValue(variables[key])
+                self._logger.debug(f"{len(variables)} loaded.")
+            if(file.endswith('.yaml') or file.endswith('.yml')):
+                variables = FileSystem.load_configuration_path(file)
+                for key in variables:
+                    self._variables[key] = VariableValue(variables[key])
+                self._logger.debug(f"{len(variables)} loaded.")
         
         self._logger.debug(f"Loading variables from manifest...")
         self.__append_manifestVariables(args[0]['manifest'])
         self._logger.debug(f"{len(variables)} loaded.")
         
         self._logger.debug(f"Override variables from parameters...")
         override = json.loads(args[0]['extraVariables'])
```

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat/runtime/lem.py` & `lemniscat_runtime-0.6.0/src/lemniscat/runtime/lem.py`

 * *Files identical despite different names*

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat/runtime/model/models.py` & `lemniscat_runtime-0.6.0/src/lemniscat/runtime/model/models.py`

 * *Files identical despite different names*

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat/runtime/plugin/pluginmanager.py` & `lemniscat_runtime-0.6.0/src/lemniscat/runtime/plugin/pluginmanager.py`

 * *Files identical despite different names*

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat/runtime/plugin/utilities.py` & `lemniscat_runtime-0.6.0/src/lemniscat/runtime/plugin/utilities.py`

 * *Files identical despite different names*

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/PKG-INFO` & `lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemniscat.runtime
-Version: 0.5.2
+Version: 0.6.0
 Summary: A runtime to provide product oriented in DevOps approach
 Author-email: Philippe MORISSEAU <philippe.morisseau@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lemniscat-devops/lemniscat.runtime
 Project-URL: Issues, https://github.com/lemniscat-devops/lemniscat.runtime/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lemniscat.runtime-0.5.2/src/lemniscat.runtime.egg-info/SOURCES.txt` & `lemniscat_runtime-0.6.0/src/lemniscat.runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

