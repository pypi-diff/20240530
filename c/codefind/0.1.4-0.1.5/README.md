# Comparing `tmp/codefind-0.1.4.tar.gz` & `tmp/codefind-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefind-0.1.4.tar", max compression
+gzip compressed data, was "codefind-0.1.5.tar", max compression
```

## Comparing `codefind-0.1.4.tar` & `codefind-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      371 2024-04-22 16:03:18.898970 codefind-0.1.4/codefind/__init__.py
--rw-r--r--   0        0        0     5120 2024-04-22 16:03:50.460448 codefind-0.1.4/codefind/registry.py
--rw-r--r--   0        0        0       18 2024-04-22 16:10:01.154137 codefind-0.1.4/codefind/version.py
--rw-r--r--   0        0        0      523 2024-04-22 16:10:01.077673 codefind-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 codefind-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      371 2024-04-22 16:03:18.898970 codefind-0.1.5/codefind/__init__.py
+-rw-r--r--   0        0        0     5416 2024-05-30 20:57:24.324545 codefind-0.1.5/codefind/registry.py
+-rw-r--r--   0        0        0       18 2024-05-30 21:53:26.813454 codefind-0.1.5/codefind/version.py
+-rw-r--r--   0        0        0      523 2024-05-30 21:53:26.788961 codefind-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 codefind-0.1.5/PKG-INFO
```

### Comparing `codefind-0.1.4/codefind/registry.py` & `codefind-0.1.5/codefind/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,22 @@
         for p in paths:
             self.codes.setdefault(p, code)
             self.currcodes[p] = code
         self.backcodes[code].update(paths)
 
     def assimilate(self, code, path=()):
         if code.co_name == "<module>":  # pragma: no cover
-            # Typically triggered by the audit hook
-            name = code.co_filename
+            # TODO: Not tested and I forget what the problem is.
+            # I had to add a condition, because it seems that it would get
+            # triggered in other situations.
+            if not path or path[-1] != code.co_filename:
+                # Typically triggered by the audit hook
+                name = code.co_filename
+            else:
+                name = None
         elif code.co_name.startswith("<"):
             return
         else:
             name = code.co_name
         if name:
             path = (*path, name)
             self._setcodepaths(
```

### Comparing `codefind-0.1.4/pyproject.toml` & `codefind-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codefind"
-version = "0.1.4"
+version = "0.1.5"
 description = "Find code objects and their referents"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `codefind-0.1.4/PKG-INFO` & `codefind-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefind
-Version: 0.1.4
+Version: 0.1.5
 Summary: Find code objects and their referents
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

