# Comparing `tmp/gdaicommons-0.0.3.tar.gz` & `tmp/gdaicommons-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdaicommons-0.0.3.tar", last modified: Sun May 26 17:32:07 2024, max compression
+gzip compressed data, was "gdaicommons-0.0.4.tar", last modified: Thu May 30 06:17:15 2024, max compression
```

## Comparing `gdaicommons-0.0.3.tar` & `gdaicommons-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:32:07.207568 gdaicommons-0.0.3/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.3/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-26 17:32:07.207568 gdaicommons-0.0.3/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.3/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-05-26 17:31:43.000000 gdaicommons-0.0.3/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-26 17:32:07.207568 gdaicommons-0.0.3/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:32:07.207568 gdaicommons-0.0.3/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:32:07.207568 gdaicommons-0.0.3/src/gdaicommons/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:22:49.000000 gdaicommons-0.0.3/src/gdaicommons/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2545 2024-05-26 14:10:41.000000 gdaicommons-0.0.3/src/gdaicommons/textclassification.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1216 2024-05-26 17:13:36.000000 gdaicommons-0.0.3/src/gdaicommons/transformations.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:32:07.207568 gdaicommons-0.0.3/src/gdaicommons.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-26 17:32:07.000000 gdaicommons-0.0.3/src/gdaicommons.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      309 2024-05-26 17:32:07.000000 gdaicommons-0.0.3/src/gdaicommons.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-26 17:32:07.000000 gdaicommons-0.0.3/src/gdaicommons.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-26 17:32:07.000000 gdaicommons-0.0.3/src/gdaicommons.egg-info/top_level.txt
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:32:07.207568 gdaicommons-0.0.3/tests/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      270 2024-05-26 14:00:18.000000 gdaicommons-0.0.3/tests/test_suite.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.4/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.4/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-05-30 06:14:44.000000 gdaicommons-0.0.4/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/gdaicommons/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 17:22:49.000000 gdaicommons-0.0.4/src/gdaicommons/__init__.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/gdaicommons/nlp/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-30 05:04:54.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2765 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/fill_mask.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2830 2024-05-30 06:08:30.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text2text_generation.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1839 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_classification.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2930 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_generation.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1831 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_labelling.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2817 2024-05-30 06:01:23.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/text_summarization.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     7807 2024-05-30 05:47:59.000000 gdaicommons-0.0.4/src/gdaicommons/nlp/transformations.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      262 2024-05-30 06:15:40.000000 gdaicommons-0.0.4/src/gdaicommons/utils.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/src/gdaicommons.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      571 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-30 06:17:15.000000 gdaicommons-0.0.4/src/gdaicommons.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-30 06:17:15.912367 gdaicommons-0.0.4/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      833 2024-05-30 06:03:21.000000 gdaicommons-0.0.4/tests/test_suite.py
```

### Comparing `gdaicommons-0.0.3/LICENSE` & `gdaicommons-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.3/PKG-INFO` & `gdaicommons-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdaicommons-0.0.3/pyproject.toml` & `gdaicommons-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdaicommons"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "AI transformation libraries and utilities to run on Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdaicommons-0.0.3/src/gdaicommons.egg-info/PKG-INFO` & `gdaicommons-0.0.4/src/gdaicommons.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

