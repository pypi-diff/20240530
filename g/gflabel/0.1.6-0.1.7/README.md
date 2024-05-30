# Comparing `tmp/gflabel-0.1.6.tar.gz` & `tmp/gflabel-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gflabel-0.1.6.tar", max compression
+gzip compressed data, was "gflabel-0.1.7.tar", max compression
```

## Comparing `gflabel-0.1.6.tar` & `gflabel-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1456 2024-05-20 16:30:40.913903 gflabel-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0    21067 2024-05-20 16:30:40.913903 gflabel-0.1.6/README.md
--rw-r--r--   0        0        0      813 2024-05-20 16:30:40.921903 gflabel-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/__init__.py
--rw-r--r--   0        0        0      220 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/__init__.py
--rw-r--r--   0        0        0     1369 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/plain.py
--rw-r--r--   0        0        0     4148 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/pred.py
--rw-r--r--   0        0        0     3726 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/bases/webb.py
--rwxr-xr-x   0        0        0    13860 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/cli.py
--rw-r--r--   0        0        0    41424 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/fragments.py
--rw-r--r--   0        0        0    12565 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/label.py
--rw-r--r--   0        0        0     3619 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/options.py
--rw-r--r--   0        0        0     4390 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/resources/LICENSE_OpenSans
--rw-r--r--   0        0        0     1068 2024-05-20 16:30:40.921903 gflabel-0.1.6/src/gflabel/resources/LICENSE_symbols
--rw-r--r--   0        0        0   130860 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/OpenSans-Bold.ttf
--rw-r--r--   0        0        0   136604 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/OpenSans-Italic.ttf
--rw-r--r--   0        0        0   130832 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/OpenSans-Regular.ttf
--rw-r--r--   0        0        0   110480 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/resources/chris-pikul-symbols.zip
--rw-r--r--   0        0        0     1739 2024-05-20 16:30:40.925903 gflabel-0.1.6/src/gflabel/util.py
--rw-r--r--   0        0        0    21614 1970-01-01 00:00:00.000000 gflabel-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-05-30 20:19:23.776389 gflabel-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0    21067 2024-05-30 20:19:23.780389 gflabel-0.1.7/README.md
+-rw-r--r--   0        0        0      813 2024-05-30 20:19:23.784390 gflabel-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/bases/__init__.py
+-rw-r--r--   0        0        0     1369 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/bases/plain.py
+-rw-r--r--   0        0        0     4148 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/bases/pred.py
+-rw-r--r--   0        0        0     3726 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/bases/webb.py
+-rwxr-xr-x   0        0        0    13860 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/cli.py
+-rw-r--r--   0        0        0    41435 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/fragments.py
+-rw-r--r--   0        0        0    12565 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/label.py
+-rw-r--r--   0        0        0     3619 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/options.py
+-rw-r--r--   0        0        0     4390 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/resources/LICENSE_OpenSans
+-rw-r--r--   0        0        0     1068 2024-05-30 20:19:23.784390 gflabel-0.1.7/src/gflabel/resources/LICENSE_symbols
+-rw-r--r--   0        0        0   130860 2024-05-30 20:19:23.788390 gflabel-0.1.7/src/gflabel/resources/OpenSans-Bold.ttf
+-rw-r--r--   0        0        0   136604 2024-05-30 20:19:23.788390 gflabel-0.1.7/src/gflabel/resources/OpenSans-Italic.ttf
+-rw-r--r--   0        0        0   130832 2024-05-30 20:19:23.788390 gflabel-0.1.7/src/gflabel/resources/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0   110480 2024-05-30 20:19:23.788390 gflabel-0.1.7/src/gflabel/resources/chris-pikul-symbols.zip
+-rw-r--r--   0        0        0     1739 2024-05-30 20:19:23.788390 gflabel-0.1.7/src/gflabel/util.py
+-rw-r--r--   0        0        0    21614 1970-01-01 00:00:00.000000 gflabel-0.1.7/PKG-INFO
```

### Comparing `gflabel-0.1.6/LICENSE.txt` & `gflabel-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/README.md` & `gflabel-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/pyproject.toml` & `gflabel-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gflabel"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Nicholas Devenish <ndevenish@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -24,15 +24,15 @@
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpversion]
-current_version = "0.1.6"
+current_version = "0.1.7"
 tag = true
 tag_name = "v{new_version}"
 commit = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
```

### Comparing `gflabel-0.1.6/src/gflabel/bases/plain.py` & `gflabel-0.1.7/src/gflabel/bases/plain.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/bases/pred.py` & `gflabel-0.1.7/src/gflabel/bases/pred.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/bases/webb.py` & `gflabel-0.1.7/src/gflabel/bases/webb.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/cli.py` & `gflabel-0.1.7/src/gflabel/cli.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/fragments.py` & `gflabel-0.1.7/src/gflabel/fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,36 +236,35 @@
                 Text(self.text, font_size=options.font.get_allowed_height(height), **f)
         return sketch.sketch
 
 
 @functools.lru_cache
 def _whitespace_width(spacechar: str, height: float, options: RenderOptions) -> float:
     """Calculate the width of a space at a specific text height"""
-    w2 = (
-        Text(
-            f"a{spacechar}a",
-            font_size=options.font.get_allowed_height(height),
-            font=options.font.font,
-            font_style=options.font.font_style,
-            mode=Mode.PRIVATE,
+    with options.font.font_options() as f:
+        w2 = (
+            Text(
+                f"a{spacechar}a",
+                font_size=options.font.get_allowed_height(height),
+                mode=Mode.PRIVATE,
+                **f,
+            )
+            .bounding_box()
+            .size.X
         )
-        .bounding_box()
-        .size.X
-    )
-    wn = (
-        Text(
-            "aa",
-            font_size=options.font.get_allowed_height(height),
-            font=options.font.font,
-            font_style=options.font.font_style,
-            mode=Mode.PRIVATE,
+        wn = (
+            Text(
+                "aa",
+                font_size=options.font.get_allowed_height(height),
+                mode=Mode.PRIVATE,
+                **f,
+            )
+            .bounding_box()
+            .size.X
         )
-        .bounding_box()
-        .size.X
-    )
     return w2 - wn
 
 
 class WhitespaceFragment(Fragment):
     visible = False
 
     def __init__(self, whitespace: str):
@@ -908,17 +907,17 @@
     category: str
     standard: str
     filename: str
 
 
 @functools.cache
 def electronic_symbols_manifest() -> list[ManifestItem]:
-    with importlib.resources.files("gflabel").joinpath("chris-pikul-symbols.zip").open(
-        "rb"
-    ) as f:
+    with importlib.resources.files("gflabel").joinpath("resources").joinpath(
+        "chris-pikul-symbols.zip"
+    ).open("rb") as f:
         zip = zipfile.ZipFile(f)
         return json.loads(zip.read("manifest.json"))
 
 
 def _get_standard_requested(selectors: Iterable[str]) -> str | None:
     """Given a list of selectors, did we ask for a standard?"""
     aliases = {
```

### Comparing `gflabel-0.1.6/src/gflabel/label.py` & `gflabel-0.1.7/src/gflabel/label.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/options.py` & `gflabel-0.1.7/src/gflabel/options.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/resources/LICENSE_OpenSans` & `gflabel-0.1.7/src/gflabel/resources/LICENSE_OpenSans`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/resources/LICENSE_symbols` & `gflabel-0.1.7/src/gflabel/resources/LICENSE_symbols`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/resources/OpenSans-Bold.ttf` & `gflabel-0.1.7/src/gflabel/resources/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/resources/OpenSans-Italic.ttf` & `gflabel-0.1.7/src/gflabel/resources/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/resources/OpenSans-Regular.ttf` & `gflabel-0.1.7/src/gflabel/resources/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/resources/chris-pikul-symbols.zip` & `gflabel-0.1.7/src/gflabel/resources/chris-pikul-symbols.zip`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/src/gflabel/util.py` & `gflabel-0.1.7/src/gflabel/util.py`

 * *Files identical despite different names*

### Comparing `gflabel-0.1.6/PKG-INFO` & `gflabel-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gflabel
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: BSD-3-Clause
 Author: Nicholas Devenish
 Author-email: ndevenish@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

