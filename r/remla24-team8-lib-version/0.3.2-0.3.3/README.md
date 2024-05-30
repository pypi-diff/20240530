# Comparing `tmp/remla24_team8_lib_version-0.3.2.tar.gz` & `tmp/remla24_team8_lib_version-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla24_team8_lib_version-0.3.2.tar", max compression
+gzip compressed data, was "remla24_team8_lib_version-0.3.3.tar", max compression
```

## Comparing `remla24_team8_lib_version-0.3.2.tar` & `remla24_team8_lib_version-0.3.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-05-21 17:08:03.326503 remla24_team8_lib_version-0.3.2/README.md
--rw-r--r--   0        0        0      631 2024-05-21 17:22:16.072798 remla24_team8_lib_version-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 16:22:43.564527 remla24_team8_lib_version-0.3.2/src/lib_version/__init__.py
--rw-r--r--   0        0        0      660 2024-05-21 16:56:44.925177 remla24_team8_lib_version-0.3.2/src/lib_version/versioning.py
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 remla24_team8_lib_version-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1131 2024-05-30 15:27:12.621057 remla24_team8_lib_version-0.3.3/README.md
+-rw-r--r--   0        0        0      639 2024-05-30 15:27:12.621057 remla24_team8_lib_version-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 15:27:12.621057 remla24_team8_lib_version-0.3.3/src/remla24_team8_lib_version/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-30 15:27:12.621057 remla24_team8_lib_version-0.3.3/src/remla24_team8_lib_version/__main__.py
+-rw-r--r--   0        0        0      593 2024-05-30 15:27:12.621057 remla24_team8_lib_version-0.3.3/src/remla24_team8_lib_version/versioning.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 remla24_team8_lib_version-0.3.3/PKG-INFO
```

### Comparing `remla24_team8_lib_version-0.3.2/README.md` & `remla24_team8_lib_version-0.3.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 ```
 
 ## Usage
 
 To get the current version include the following lines:
 
 ```python
-import lib_version.versioning as versioning
-util = VersionUtil()
-print(util.get_version())
-```
+from remla24_team8_lib_version import versioning
 
+print(versioning.VersionUtil().version)
+```
+or from command-line
 
+```bash
+python3 -m remla24_team8_lib_version
+```
```

### Comparing `remla24_team8_lib_version-0.3.2/pyproject.toml` & `remla24_team8_lib_version-0.3.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "remla24-team8-lib-version"
-version = "0.3.2"
+version = "0.3.3"
 description = "A version-aware library that can can be asked for the version of the library"
 authors = [
     "Tip ten Brink <T.M.tenBrink@student.tudelft.nl>", 
     "Felipe Bononi Bello <bello2001felipe@gmail.com>", 
     "Dielof van Loon <d.i.vanloon@student.tudelft.nl>", 
     "Sayf El Kaddouri <sayfgmaul@gmail.com>"
 ]
 readme = "README.md"
-packages = [
-    { include = "lib_version", from = "src"},
-]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-importlib-resources = "^6.4.0"
+
+[tool.poetry.scripts]
+get_version = "remla24_team8_lib_version.versioning:VersionUtil.get_version"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `remla24_team8_lib_version-0.3.2/PKG-INFO` & `remla24_team8_lib_version-0.3.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: remla24-team8-lib-version
-Version: 0.3.2
+Version: 0.3.3
 Summary: A version-aware library that can can be asked for the version of the library
 Author: Tip ten Brink
 Author-email: T.M.tenBrink@student.tudelft.nl
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: importlib-resources (>=6.4.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # lib-version
 
 A version-aware library that can can be asked for the version of the library. This can be useful, for example, for verbose system information in log messages or data records. The library may also contain other logic.
 
 • Create a VersionUtil class that can be asked for its version.
@@ -29,15 +28,18 @@
 ```
 
 ## Usage
 
 To get the current version include the following lines:
 
 ```python
-import lib_version.versioning as versioning
-util = VersionUtil()
-print(util.get_version())
-```
+from remla24_team8_lib_version import versioning
 
+print(versioning.VersionUtil().version)
+```
+or from command-line
 
+```bash
+python3 -m remla24_team8_lib_version
+```
```

