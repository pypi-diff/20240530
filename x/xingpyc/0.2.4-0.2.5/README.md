# Comparing `tmp/xingpyc-0.2.4.tar.gz` & `tmp/xingpyc-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.2.4.tar", last modified: Mon May 27 20:23:07 2024, max compression
+gzip compressed data, was "xingpyc-0.2.5.tar", last modified: Wed May 29 11:12:36 2024, max compression
```

## Comparing `xingpyc-0.2.4.tar` & `xingpyc-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 20:23:07.741992 xingpyc-0.2.4/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 20:23:07.741762 xingpyc-0.2.4/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.4/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-27 20:23:03.000000 xingpyc-0.2.4/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-27 20:23:07.742034 xingpyc-0.2.4/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 20:23:07.739893 xingpyc-0.2.4/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 20:23:07.740391 xingpyc-0.2.4/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     9148 2024-05-27 20:22:50.000000 xingpyc-0.2.4/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.4/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 20:23:07.741540 xingpyc-0.2.4/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-27 20:23:07.000000 xingpyc-0.2.4/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-27 20:23:07.000000 xingpyc-0.2.4/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-27 20:23:07.000000 xingpyc-0.2.4/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-27 20:23:07.000000 xingpyc-0.2.4/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-27 20:23:07.000000 xingpyc-0.2.4/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-27 20:23:07.741377 xingpyc-0.2.4/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.4/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.785244 xingpyc-0.2.5/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-29 11:12:36.785044 xingpyc-0.2.5/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.5/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-29 11:12:27.000000 xingpyc-0.2.5/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-29 11:12:36.785284 xingpyc-0.2.5/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.783440 xingpyc-0.2.5/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.783980 xingpyc-0.2.5/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     9148 2024-05-27 20:22:50.000000 xingpyc-0.2.5/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.5/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.784833 xingpyc-0.2.5/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-29 11:12:36.000000 xingpyc-0.2.5/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-29 11:12:36.784691 xingpyc-0.2.5/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.5/tests/test1.py
```

### Comparing `xingpyc-0.2.4/PKG-INFO` & `xingpyc-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.4
+Version: 0.2.5
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.2.4/pyproject.toml` & `xingpyc-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.2.4/src/xingpyc/__init__.py` & `xingpyc-0.2.5/src/xingpyc/__init__.py`

 * *Files identical despite different names*

### Comparing `xingpyc-0.2.4/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.2.5/src/xingpyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.2.4
+Version: 0.2.5
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

