# Comparing `tmp/sysml2py-0.5.2.tar.gz` & `tmp/sysml2py-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.5.2.tar", max compression
+gzip compressed data, was "sysml2py-0.5.3.tar", max compression
```

## Comparing `sysml2py-0.5.2.tar` & `sysml2py-0.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2023-08-12 07:46:58.450418 sysml2py-0.5.2/LICENSE
--rw-r--r--   0        0        0     3757 2023-08-12 07:46:58.450418 sysml2py-0.5.2/README.md
--rw-r--r--   0        0        0     2525 2023-08-12 07:46:59.526465 sysml2py-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4150 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/__init__.py
--rw-r--r--   0        0        0     8377 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/definition.py
--rw-r--r--   0        0        0     1288 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/formatting.py
--rw-r--r--   0        0        0    22294 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/grammar/KerML.tx
--rw-r--r--   0        0        0    10962 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/grammar/KerMLExpressions.tx
--rw-r--r--   0        0        0    49022 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/grammar/SysML.tx
--rw-r--r--   0        0        0    65364 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/grammar/SysML_compiled.tx
--rw-r--r--   0        0        0   201905 2023-08-12 07:46:58.450418 sysml2py-0.5.2/src/sysml2py/grammar/classes.py
--rw-r--r--   0        0        0    28524 2023-08-12 07:46:58.454418 sysml2py-0.5.2/src/sysml2py/textx/KerML.xtext
--rw-r--r--   0        0        0    14284 2023-08-12 07:46:58.454418 sysml2py-0.5.2/src/sysml2py/textx/KerMLExpressions.xtext
--rw-r--r--   0        0        0    60663 2023-08-12 07:46:58.454418 sysml2py-0.5.2/src/sysml2py/textx/SysML.xtext
--rw-r--r--   0        0        0     6279 2023-08-12 07:46:58.454418 sysml2py-0.5.2/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0        0        0    24349 2023-08-12 07:46:58.454418 sysml2py-0.5.2/src/sysml2py/usage.py
--rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 sysml2py-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-30 03:39:42.271735 sysml2py-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3757 2024-05-30 03:39:42.271735 sysml2py-0.5.3/README.md
+-rw-r--r--   0        0        0     2554 2024-05-30 03:39:43.251739 sysml2py-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4758 2024-05-30 03:39:42.271735 sysml2py-0.5.3/src/sysml2py/__init__.py
+-rw-r--r--   0        0        0     8377 2024-05-30 03:39:42.271735 sysml2py-0.5.3/src/sysml2py/definition.py
+-rw-r--r--   0        0        0     1288 2024-05-30 03:39:42.271735 sysml2py-0.5.3/src/sysml2py/formatting.py
+-rw-r--r--   0        0        0    22294 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/grammar/KerML.tx
+-rw-r--r--   0        0        0    10962 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/grammar/KerMLExpressions.tx
+-rw-r--r--   0        0        0    49022 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/grammar/SysML.tx
+-rw-r--r--   0        0        0    65364 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/grammar/SysML_compiled.tx
+-rw-r--r--   0        0        0   201907 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/grammar/classes.py
+-rw-r--r--   0        0        0    28524 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/textx/KerML.xtext
+-rw-r--r--   0        0        0    14284 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/textx/KerMLExpressions.xtext
+-rw-r--r--   0        0        0    60663 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/textx/SysML.xtext
+-rw-r--r--   0        0        0     6279 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0        0        0    24349 2024-05-30 03:39:42.275735 sysml2py-0.5.3/src/sysml2py/usage.py
+-rw-r--r--   0        0        0     4317 1970-01-01 00:00:00.000000 sysml2py-0.5.3/PKG-INFO
```

### Comparing `sysml2py-0.5.2/LICENSE` & `sysml2py-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/README.md` & `sysml2py-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/pyproject.toml` & `sysml2py-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 #requires = ["setuptools>=61.0"]
 #build-backend = "setuptools.build_meta"
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "sysml2py"
-version = "0.5.2"
+version = "0.5.3"
+description = "SysML v2.0 Parser"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
-description = "SysML v2.0 Parser"
 readme = "README.md"
+license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -94,15 +95,15 @@
 
 [project.urls]
 "Homepage" = "https://github.com/Westfall-io/sysml2py"
 "Bug Tracker" = "https://github.com/Westfall-io/sysml2py/issues"
 
 [tool.poetry]
 name = "sysml2py"
-version = "0.5.2"
+version = "0.5.3"
 description = ""
 authors = ["Christopher Cox <chris.cox@westfall.io>"]
 readme = "README.md"
 packages = [{ include = "sysml2py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `sysml2py-0.5.2/src/sysml2py/__init__.py` & `sysml2py-0.5.3/src/sysml2py/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,29 @@
 @author: christophercox
 """
 
 __all__ = ["load", "loads", "load_grammar"]
 __author__ = "Christopher Cox"
 __version__ = "0.1.0"
 
+# These are interchangable
 from sysml2py.usage import Item, Attribute, Part, Port
+
+# These are definition only
 from sysml2py.definition import Model, Package
 
 
 def enforce_grammar():  # pragma: no cover
+    """Enforce grammar compiles the language for xtext
+
+    This opens each of the files: KerMLExpressions, KerML, and SysML and
+    makes a superfile with all of the definitions and strips the comments. This
+    includes changes made to shift from java textx to the python xtext library.
+
+    """
     import re
 
     comments_strip_rule = r"(?:(?:(?<!\\)(\/\/.*\n))|(?:\/\*(?:.|\n)*?\*\/))"
     regex_rule = "\n[ ]*([\w]*)[ ]*:((?:(?:'[^']*')|(?:[^;']*))*;)"
 
     g_list = []
     rule_files = ["KerMLExpressions", "KerML", "SysML"]
@@ -154,8 +164,15 @@
             f"not {fp.__class__.__name__}"
         )
 
     return loads(fp.read())
 
 
 def loads(s: str):
+    """Loads a model from string.
+
+    This shortcut function allows a user to build a model from a string by
+    first instantiating a base model class which builds out a default namespace
+    and then that model loads all elements underneath.
+
+    """
     return Model().load(s)
```

### Comparing `sysml2py-0.5.2/src/sysml2py/definition.py` & `sysml2py-0.5.3/src/sysml2py/definition.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/formatting.py` & `sysml2py-0.5.3/src/sysml2py/formatting.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/grammar/KerML.tx` & `sysml2py-0.5.3/src/sysml2py/grammar/KerML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/grammar/KerMLExpressions.tx` & `sysml2py-0.5.3/src/sysml2py/grammar/KerMLExpressions.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/grammar/SysML.tx` & `sysml2py-0.5.3/src/sysml2py/grammar/SysML.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/grammar/SysML_compiled.tx` & `sysml2py-0.5.3/src/sysml2py/grammar/SysML_compiled.tx`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/grammar/classes.py` & `sysml2py-0.5.3/src/sysml2py/grammar/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -2555,17 +2555,17 @@
             "identification": None,
             "subclassificationpart": None,
         }
         if self.identification is not None:
             output["identification"] = self.identification.get_definition()
 
         if self.subclassificationpart is not None:
-            output[
-                "subclassificationpart"
-            ] = self.subclassificationpart.get_definition()
+            output["subclassificationpart"] = (
+                self.subclassificationpart.get_definition()
+            )
 
         return output
 
 
 class SubclassificationPart:
     def __init__(self, definition):
         if valid_definition(definition, "SubclassificationPart"):
```

### Comparing `sysml2py-0.5.2/src/sysml2py/textx/KerML.xtext` & `sysml2py-0.5.3/src/sysml2py/textx/KerML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/textx/KerMLExpressions.xtext` & `sysml2py-0.5.3/src/sysml2py/textx/KerMLExpressions.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/textx/SysML.xtext` & `sysml2py-0.5.3/src/sysml2py/textx/SysML.xtext`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.5.3/src/sysml2py/textx/xtext_to_textx.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/src/sysml2py/usage.py` & `sysml2py-0.5.3/src/sysml2py/usage.py`

 * *Files identical despite different names*

### Comparing `sysml2py-0.5.2/PKG-INFO` & `sysml2py-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: sysml2py
-Version: 0.5.2
+Version: 0.5.3
 Summary: 
 Author: Christopher Cox
 Author-email: chris.cox@westfall.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astropy (>=5.3.1,<6.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: textx (>=3.1.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # sysml2py
 [![PyPI version](https://badge.fury.io/py/sysml2py.svg)](https://badge.fury.io/py/sysml2py)[![PyPI status](https://img.shields.io/pypi/status/sysml2py.svg)](https://pypi.python.org/pypi/sysml2py/)[![Coverage Status](https://coveralls.io/repos/github/Westfall-io/sysml2py/badge.svg)](https://coveralls.io/github/Westfall-io/sysml2py)![Docstring Coverage](https://raw.githubusercontent.com/Westfall-io/sysml2py/main/doc-cov.svg)[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
```

