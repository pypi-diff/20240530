# Comparing `tmp/asp_selftest-0.0.7.tar.gz` & `tmp/asp_selftest-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asp_selftest-0.0.7.tar", last modified: Mon May 27 09:47:49 2024, max compression
+gzip compressed data, was "asp_selftest-0.0.8.tar", last modified: Mon May 27 10:05:12 2024, max compression
```

## Comparing `asp_selftest-0.0.7.tar` & `asp_selftest-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.079930 asp_selftest-0.0.7/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.7/LICENSE
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.7/MANIFEST.in
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-27 09:47:49.079704 asp_selftest-0.0.7/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2878 2024-04-25 15:02:28.000000 asp_selftest-0.0.7/README.md
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      789 2024-05-27 09:46:52.000000 asp_selftest-0.0.7/pyproject.toml
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-05-27 09:47:49.079975 asp_selftest-0.0.7/setup.cfg
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.077468 asp_selftest-0.0.7/src/
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.078460 asp_selftest-0.0.7/src/asp_selftest/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      727 2024-05-08 16:37:36.000000 asp_selftest-0.0.7/src/asp_selftest/__init__.py
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      629 2024-05-27 09:44:58.000000 asp_selftest-0.0.7/src/asp_selftest/example.lp
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-05-27 08:26:50.000000 asp_selftest-0.0.7/src/asp_selftest/queens.lp
--rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)    10086 2024-05-27 09:37:55.000000 asp_selftest-0.0.7/src/asp_selftest/runasptests.py
-drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 09:47:49.079464 asp_selftest-0.0.7/src/asp_selftest.egg-info/
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/PKG-INFO
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)      363 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/SOURCES.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/dependency_links.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       55 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/entry_points.txt
--rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-05-27 09:47:49.000000 asp_selftest-0.0.7/src/asp_selftest.egg-info/top_level.txt
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 10:05:12.025401 asp_selftest-0.0.8/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)    35149 2024-02-19 08:25:44.000000 asp_selftest-0.0.8/LICENSE
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       20 2024-04-25 13:29:32.000000 asp_selftest-0.0.8/MANIFEST.in
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-27 10:05:12.025210 asp_selftest-0.0.8/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     2878 2024-04-25 15:02:28.000000 asp_selftest-0.0.8/README.md
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 10:05:12.023819 asp_selftest-0.0.8/bin/
+-rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)      357 2024-05-27 08:09:31.000000 asp_selftest-0.0.8/bin/runasptests.sh
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      847 2024-05-27 10:03:31.000000 asp_selftest-0.0.8/pyproject.toml
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       38 2024-05-27 10:05:12.025441 asp_selftest-0.0.8/setup.cfg
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 10:05:12.023151 asp_selftest-0.0.8/src/
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 10:05:12.024307 asp_selftest-0.0.8/src/asp_selftest/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      727 2024-05-08 16:37:36.000000 asp_selftest-0.0.8/src/asp_selftest/__init__.py
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      629 2024-05-27 09:44:58.000000 asp_selftest-0.0.8/src/asp_selftest/example.lp
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     1277 2024-05-27 08:26:50.000000 asp_selftest-0.0.8/src/asp_selftest/queens.lp
+-rwxr-xr-x   0 erikgroeneveld   (501) staff       (20)    10086 2024-05-27 09:37:55.000000 asp_selftest-0.0.8/src/asp_selftest/runasptests.py
+drwxr-xr-x   0 erikgroeneveld   (501) staff       (20)        0 2024-05-27 10:05:12.025015 asp_selftest-0.0.8/src/asp_selftest.egg-info/
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)     3490 2024-05-27 10:05:11.000000 asp_selftest-0.0.8/src/asp_selftest.egg-info/PKG-INFO
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)      382 2024-05-27 10:05:12.000000 asp_selftest-0.0.8/src/asp_selftest.egg-info/SOURCES.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)        1 2024-05-27 10:05:11.000000 asp_selftest-0.0.8/src/asp_selftest.egg-info/dependency_links.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       55 2024-05-27 10:05:11.000000 asp_selftest-0.0.8/src/asp_selftest.egg-info/entry_points.txt
+-rw-r--r--   0 erikgroeneveld   (501) staff       (20)       13 2024-05-27 10:05:11.000000 asp_selftest-0.0.8/src/asp_selftest.egg-info/top_level.txt
```

### Comparing `asp_selftest-0.0.7/LICENSE` & `asp_selftest-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.7/PKG-INFO` & `asp_selftest-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `asp_selftest-0.0.7/README.md` & `asp_selftest-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.7/pyproject.toml` & `asp_selftest-0.0.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "asp_selftest"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Erik Groeneveld", email="ejgroene@ieee.org" },
 ]
 description = "A tool for running in-source unittests for Anwer Set Programming (ASP)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -20,14 +20,18 @@
 ]
 
 
 [project.scripts]
 asp-tests = "asp_selftest:runasptests"
 
 
+[tool.setuptools]
+script-files = ["bin/runasptests.sh"]
+
+
 [project.urls]
 Homepage = "https://github.com/ejgroene/asp-selftest"
 Issues = "https://github.com/ejgroene/asp-selftest/issues"
 
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `asp_selftest-0.0.7/src/asp_selftest/__init__.py` & `asp_selftest-0.0.8/src/asp_selftest/__init__.py`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.7/src/asp_selftest/example.lp` & `asp_selftest-0.0.8/src/asp_selftest/example.lp`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.7/src/asp_selftest/queens.lp` & `asp_selftest-0.0.8/src/asp_selftest/queens.lp`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.7/src/asp_selftest/runasptests.py` & `asp_selftest-0.0.8/src/asp_selftest/runasptests.py`

 * *Files identical despite different names*

### Comparing `asp_selftest-0.0.7/src/asp_selftest.egg-info/PKG-INFO` & `asp_selftest-0.0.8/src/asp_selftest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asp_selftest
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for running in-source unittests for Anwer Set Programming (ASP)
 Author-email: Erik Groeneveld <ejgroene@ieee.org>
 Project-URL: Homepage, https://github.com/ejgroene/asp-selftest
 Project-URL: Issues, https://github.com/ejgroene/asp-selftest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: ASP
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

