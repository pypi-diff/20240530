# Comparing `tmp/fjsim-1.0.tar.gz` & `tmp/fjsim-1.1.tar.gz`

## Comparing `fjsim-1.0.tar` & `fjsim-1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 fjsim-1.0/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fjsim-1.0/src/example.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fjsim-1.0/LICENSE.txt
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 fjsim-1.0/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 fjsim-1.0/pyproject.toml
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fjsim-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 fjsim-1.1/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fjsim-1.1/src/example.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fjsim-1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 fjsim-1.1/README.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fjsim-1.1/pyproject.toml
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fjsim-1.1/PKG-INFO
```

### Comparing `fjsim-1.0/src/__init__.py` & `fjsim-1.1/src/__init__.py`

 * *Files identical despite different names*

### Comparing `fjsim-1.0/LICENSE.txt` & `fjsim-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fjsim-1.0/README.md` & `fjsim-1.1/README.md`

 * *Files identical despite different names*

### Comparing `fjsim-1.0/pyproject.toml` & `fjsim-1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FJsim"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Giorgio Sorgente", email="giorgiosorgente@hotmail.com" },
 ]
 description = "A module capable of simulating the spreading of an opinon in a given network using the Friedkin-Johnsen model."
 readme = "README.md"
 requires-python = ">=3.9.10"
 classifiers = [
@@ -19,8 +19,8 @@
 
 [project.urls]
 Homepage = "https://github.com/Giorgio-ctrl/Friedkin-Johnsen-model-simulator"
 Issues = "https://github.com/Giorgio-ctrl/Friedkin-Johnsen-model-simulator/issues"
 
 
 [tool.hatch.build.targets.wheel]
-packages = ["src"]
+packages = ["FJsim"]
```

### Comparing `fjsim-1.0/PKG-INFO` & `fjsim-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FJsim
-Version: 1.0
+Version: 1.1
 Summary: A module capable of simulating the spreading of an opinon in a given network using the Friedkin-Johnsen model.
 Project-URL: Homepage, https://github.com/Giorgio-ctrl/Friedkin-Johnsen-model-simulator
 Project-URL: Issues, https://github.com/Giorgio-ctrl/Friedkin-Johnsen-model-simulator/issues
 Author-email: Giorgio Sorgente <giorgiosorgente@hotmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

