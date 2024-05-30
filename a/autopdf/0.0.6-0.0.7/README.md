# Comparing `tmp/autopdf-0.0.6.tar.gz` & `tmp/autopdf-0.0.7.tar.gz`

## Comparing `autopdf-0.0.6.tar` & `autopdf-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 autopdf-0.0.6/src/autopdf/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 autopdf-0.0.6/src/autopdf/clusterer.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 autopdf-0.0.6/src/autopdf/editor.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 autopdf-0.0.6/src/autopdf/exporting.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 autopdf-0.0.6/src/autopdf/to_md.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 autopdf-0.0.6/src/autopdf/to_txt.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 autopdf-0.0.6/LICENSE
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 autopdf-0.0.6/README.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 autopdf-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 autopdf-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 autopdf-0.0.7/src/autopdf/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 autopdf-0.0.7/src/autopdf/clusterer.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 autopdf-0.0.7/src/autopdf/editor.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 autopdf-0.0.7/src/autopdf/exporting.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 autopdf-0.0.7/src/autopdf/to_md.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 autopdf-0.0.7/src/autopdf/to_txt.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 autopdf-0.0.7/LICENSE
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 autopdf-0.0.7/README.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 autopdf-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 autopdf-0.0.7/PKG-INFO
```

### Comparing `autopdf-0.0.6/src/autopdf/clusterer.py` & `autopdf-0.0.7/src/autopdf/clusterer.py`

 * *Files identical despite different names*

### Comparing `autopdf-0.0.6/src/autopdf/editor.py` & `autopdf-0.0.7/src/autopdf/editor.py`

 * *Files identical despite different names*

### Comparing `autopdf-0.0.6/src/autopdf/exporting.py` & `autopdf-0.0.7/src/autopdf/exporting.py`

 * *Files identical despite different names*

### Comparing `autopdf-0.0.6/src/autopdf/to_md.py` & `autopdf-0.0.7/src/autopdf/to_md.py`

 * *Files identical despite different names*

### Comparing `autopdf-0.0.6/src/autopdf/to_txt.py` & `autopdf-0.0.7/src/autopdf/to_txt.py`

 * *Files identical despite different names*

### Comparing `autopdf-0.0.6/LICENSE` & `autopdf-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autopdf-0.0.6/pyproject.toml` & `autopdf-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autopdf"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Gustavo L. Matos", email="matosgustavo@statmatos.com" },
 ]
 
 dependencies = [
   'pandas', 'numpy', 'pdfminer', 'scikit-learn',
 ]
```

### Comparing `autopdf-0.0.6/PKG-INFO` & `autopdf-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autopdf
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extracts PDF text to .md or .txt in reading order!
 Project-URL: Homepage, https://github.com/GustaMatos0/autopdf
 Project-URL: Issues, https://github.com/GustaMatos0/autopdf/issues
 Author-email: "Gustavo L. Matos" <matosgustavo@statmatos.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

