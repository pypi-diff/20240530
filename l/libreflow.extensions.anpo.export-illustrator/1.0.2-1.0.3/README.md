# Comparing `tmp/libreflow_extensions_anpo_export_illustrator-1.0.2.tar.gz` & `tmp/libreflow_extensions_anpo_export_illustrator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_extensions_anpo_export_illustrator-1.0.2.tar", last modified: Wed May 29 20:39:53 2024, max compression
+gzip compressed data, was "libreflow_extensions_anpo_export_illustrator-1.0.3.tar", last modified: Wed May 29 20:46:57 2024, max compression
```

## Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2.tar` & `libreflow_extensions_anpo_export_illustrator-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1323 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-29 20:39:53.854260 libreflow_extensions_anpo_export_illustrator-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1278 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.848260 libreflow_extensions_anpo_export_illustrator-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.851260 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.852259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.852259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/
--rw-rw-rw-   0 root         (0) root         (0)     5467 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-29 20:39:53.854260 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     9765 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/scripts/layers2png.jsx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:39:53.853259 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1323 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 20:39:53.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-29 20:39:44.000000 libreflow_extensions_anpo_export_illustrator-1.0.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.360950 libreflow_extensions_anpo_export_illustrator-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-05-29 20:46:57.360950 libreflow_extensions_anpo_export_illustrator-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-29 20:46:57.360950 libreflow_extensions_anpo_export_illustrator-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.355950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.357950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.358950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.358950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.359950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/export_illustrator/
+-rw-rw-rw-   0 root         (0) root         (0)     5467 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/export_illustrator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-29 20:46:57.360950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/export_illustrator/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.359950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/export_illustrator/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     9765 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/export_illustrator/scripts/layers2png.jsx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:46:57.359950 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow.extensions.anpo.export_illustrator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-05-29 20:46:57.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 20:46:57.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 20:46:57.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow.extensions.anpo.export_illustrator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 20:46:57.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow.extensions.anpo.export_illustrator.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-05-29 20:46:47.000000 libreflow_extensions_anpo_export_illustrator-1.0.3/versioneer.py
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/CHANGELOG.md` & `libreflow_extensions_anpo_export_illustrator-1.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/PKG-INFO` & `libreflow_extensions_anpo_export_illustrator-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.export-illustrator
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://gitlab.com/lfs.coop/libreflow/
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/setup.py` & `libreflow_extensions_anpo_export_illustrator-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,12 +34,12 @@
     keywords="kabaret libreflow",
     install_requires=[],
     python_requires='>=3.7',
     packages=setuptools.find_packages("src"),
     package_dir={"": "src"},
     package_data={
         '': [
-            '*.jsx'
+            'libreflow/extensions/anpo/export_illustrator/scripts/layers2png.jsx'
         ],
     },
 
 )
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/__init__.py` & `libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/export_illustrator/__init__.py`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow/extensions/anpo/export_illustrator/scripts/layers2png.jsx` & `libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow/extensions/anpo/export_illustrator/scripts/layers2png.jsx`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO` & `libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow.extensions.anpo.export_illustrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow.extensions.anpo.export-illustrator
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://gitlab.com/lfs.coop/libreflow/
 Author: LFS
 Author-email: libreflow@lfs.coop
 License: LGPLv3+
 Keywords: kabaret libreflow
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt` & `libreflow_extensions_anpo_export_illustrator-1.0.3/src/libreflow.extensions.anpo.export_illustrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_extensions_anpo_export_illustrator-1.0.2/versioneer.py` & `libreflow_extensions_anpo_export_illustrator-1.0.3/versioneer.py`

 * *Files identical despite different names*

