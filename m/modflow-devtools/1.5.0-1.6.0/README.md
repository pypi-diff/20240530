# Comparing `tmp/modflow_devtools-1.5.0.tar.gz` & `tmp/modflow_devtools-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow_devtools-1.5.0.tar", last modified: Wed May 15 17:57:28 2024, max compression
+gzip compressed data, was "modflow_devtools-1.6.0.tar", last modified: Thu May 30 19:11:25 2024, max compression
```

## Comparing `modflow_devtools-1.5.0.tar` & `modflow_devtools-1.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1627 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:57:28.777448 modflow_devtools-1.5.0/modflow_devtools/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    17465 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/latex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/ostags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/modflow_devtools/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/modflow_devtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 17:57:24.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 17:57:28.000000 modflow_devtools-1.5.0/modflow_devtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 17:57:28.781448 modflow_devtools-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 17:57:14.000000 modflow_devtools-1.5.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:11:25.766596 modflow_devtools-1.6.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1627 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-30 19:11:25.766596 modflow_devtools-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:11:25.762596 modflow_devtools-1.6.0/modflow_devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17465 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16091 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/ostags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/modflow_devtools/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:11:25.766596 modflow_devtools-1.6.0/modflow_devtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-30 19:11:25.000000 modflow_devtools-1.6.0/modflow_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 19:11:25.000000 modflow_devtools-1.6.0/modflow_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:11:25.000000 modflow_devtools-1.6.0/modflow_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:11:21.000000 modflow_devtools-1.6.0/modflow_devtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 19:11:25.000000 modflow_devtools-1.6.0/modflow_devtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 19:11:25.000000 modflow_devtools-1.6.0/modflow_devtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:11:25.766596 modflow_devtools-1.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 19:11:08.000000 modflow_devtools-1.6.0/version.txt
```

### Comparing `modflow_devtools-1.5.0/LICENSE.md` & `modflow_devtools-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/PKG-INFO` & `modflow_devtools-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>, Michael Reno <mreno@ucar.edu>, Mike Taves <mwtoews@gmail.com>, Wes Bonelli <wbonelli@ucar.edu>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
```

### Comparing `modflow_devtools-1.5.0/README.md` & `modflow_devtools-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/build.py` & `modflow_devtools-1.6.0/modflow_devtools/build.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/download.py` & `modflow_devtools-1.6.0/modflow_devtools/download.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/fixtures.py` & `modflow_devtools-1.6.0/modflow_devtools/fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/imports.py` & `modflow_devtools-1.6.0/modflow_devtools/imports.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/latex.py` & `modflow_devtools-1.6.0/modflow_devtools/latex.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/markers.py` & `modflow_devtools-1.6.0/modflow_devtools/markers.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/misc.py` & `modflow_devtools-1.6.0/modflow_devtools/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -280,21 +280,49 @@
     selected=None,
     packages=None,
 ) -> List[Path]:
     """
     Find model directories recursively in the given location.
     A model directory is any directory containing one or more
     namefiles. Model directories can be filtered or excluded,
-    by prefix, pattern, namefile name, or packages used.
+    by prefix, pattern, namefile name, or packages used. The
+    directories are returned in order within scenario folders
+    such that groundwater flow model workspaces precede other
+    model types. This allows models which depend on the flow
+    model's outputs to consume its head or budget, and models
+    should successfully run in the sequence returned provided
+    input files (e.g. FMI) refer to output via relative paths.
     """
 
-    namefile_paths = get_namefile_paths(
-        path, prefix, namefile, excluded, selected, packages
-    )
-    model_paths = sorted(list(set([p.parent for p in namefile_paths if p.parent.name])))
+    def keyfunc(v):
+        v = str(v)
+        if "gwf" in v:
+            return 0
+        else:
+            return 1
+
+    model_paths = []
+    globbed = path.rglob(f"{prefix if prefix else ''}*")
+    example_paths = [p for p in globbed if p.is_dir()]
+    for p in example_paths:
+        for mp in sorted(
+            list(
+                set(
+                    [
+                        p.parent
+                        for p in get_namefile_paths(
+                            p, prefix, namefile, excluded, selected, packages
+                        )
+                    ]
+                )
+            ),
+            key=keyfunc,
+        ):
+            if mp not in model_paths:
+                model_paths.append(mp)
     return model_paths
 
 
 def is_connected(hostname):
     """
     Tests whether the given URL is accessible.
     See https://stackoverflow.com/a/20913928/.
```

### Comparing `modflow_devtools-1.5.0/modflow_devtools/ostags.py` & `modflow_devtools-1.6.0/modflow_devtools/ostags.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools/zip.py` & `modflow_devtools-1.6.0/modflow_devtools/zip.py`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/modflow_devtools.egg-info/PKG-INFO` & `modflow_devtools-1.6.0/modflow_devtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>, Michael Reno <mreno@ucar.edu>, Mike Taves <mwtoews@gmail.com>, Wes Bonelli <wbonelli@ucar.edu>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
```

### Comparing `modflow_devtools-1.5.0/modflow_devtools.egg-info/SOURCES.txt` & `modflow_devtools-1.6.0/modflow_devtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modflow_devtools-1.5.0/pyproject.toml` & `modflow_devtools-1.6.0/pyproject.toml`

 * *Files identical despite different names*

