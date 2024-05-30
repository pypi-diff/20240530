# Comparing `tmp/osvg-1.1.0.tar.gz` & `tmp/osvg-1.1.1.tar.gz`

## Comparing `osvg-1.1.0.tar` & `osvg-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/__init__.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/float.py
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/float_math.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/helper.py
--rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/positions.py
--rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/style.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/circle.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/circlebase.py
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/elementbase.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/ellipse.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/group.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/line.py
--rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/line_marker.py
--rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/path.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/polyline.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/rectangle.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/rectanglebase.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/svg.py
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 osvg-1.1.0/osvg/elements/text.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 osvg-1.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 osvg-1.1.0/LICENSE
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 osvg-1.1.0/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 osvg-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 osvg-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/__init__.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/float.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/float_math.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/helper.py
+-rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/positions.py
+-rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/style.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/circle.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/circlebase.py
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/elementbase.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/ellipse.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/group.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/line.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/line_marker.py
+-rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/path.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/polyline.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/rectangle.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/rectanglebase.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/svg.py
+-rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 osvg-1.1.1/osvg/elements/text.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 osvg-1.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 osvg-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 osvg-1.1.1/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 osvg-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 osvg-1.1.1/PKG-INFO
```

### Comparing `osvg-1.1.0/osvg/__init__.py` & `osvg-1.1.1/osvg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,9 @@
     StrokeLineCap,
     StrokeLineJoin,
     StrokeOpacity,
     StrokeWidth,
     Style,
 )
 
-__version__ = "1.1.0"
-version_info = (1, 1, 0)
+__version__ = "1.1.1"
+version_info = (1, 1, 1)
```

### Comparing `osvg-1.1.0/osvg/float.py` & `osvg-1.1.1/osvg/float.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/float_math.py` & `osvg-1.1.1/osvg/float_math.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/helper.py` & `osvg-1.1.1/osvg/helper.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/positions.py` & `osvg-1.1.1/osvg/positions.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/style.py` & `osvg-1.1.1/osvg/style.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/circle.py` & `osvg-1.1.1/osvg/elements/circle.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/circlebase.py` & `osvg-1.1.1/osvg/elements/circlebase.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/elementbase.py` & `osvg-1.1.1/osvg/elements/elementbase.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/ellipse.py` & `osvg-1.1.1/osvg/elements/ellipse.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/group.py` & `osvg-1.1.1/osvg/elements/group.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/line.py` & `osvg-1.1.1/osvg/elements/line.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/line_marker.py` & `osvg-1.1.1/osvg/elements/line_marker.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/path.py` & `osvg-1.1.1/osvg/elements/path.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/polyline.py` & `osvg-1.1.1/osvg/elements/polyline.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/rectangle.py` & `osvg-1.1.1/osvg/elements/rectangle.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/rectanglebase.py` & `osvg-1.1.1/osvg/elements/rectanglebase.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/svg.py` & `osvg-1.1.1/osvg/elements/svg.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/osvg/elements/text.py` & `osvg-1.1.1/osvg/elements/text.py`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/LICENSE` & `osvg-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/README.md` & `osvg-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `osvg-1.1.0/pyproject.toml` & `osvg-1.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,29 @@
 [tool.hatch.build]
 include = [
   "/osvg",
 ]
 
 [project]
 name = "osvg"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "osvg is a python API to create SVG XML code with object-oriented elements"
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = [
+  "typing_extensions",
+]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Intended Audience :: Developers",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/ko.no/osvg"
```

### Comparing `osvg-1.1.0/PKG-INFO` & `osvg-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.3
 Name: osvg
-Version: 1.1.0
+Version: 1.1.1
 Summary: osvg is a python API to create SVG XML code with object-oriented elements
 Project-URL: Homepage, https://gitlab.com/ko.no/osvg
 Project-URL: Bug Tracker, https://gitlab.com/ko.no/osvg/-/issues
 Author-email: Korte Noack <korte@8lacht.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # Object-oriented Scalable Vector Graphics
 
 ## Table of Content
 
 - [Installation](#installation)
```

