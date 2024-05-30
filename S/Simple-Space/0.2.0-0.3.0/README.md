# Comparing `tmp/simple_space-0.2.0.tar.gz` & `tmp/simple_space-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-0.2.0.tar", last modified: Thu May 30 18:44:00 2024, max compression
+gzip compressed data, was "simple_space-0.3.0.tar", last modified: Thu May 30 18:56:06 2024, max compression
```

## Comparing `simple_space-0.2.0.tar` & `simple_space-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:44:00.992218 simple_space-0.2.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.2.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11045 2024-05-30 18:44:00.992218 simple_space-0.2.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     9972 2024-05-30 18:05:04.000000 simple_space-0.2.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:44:00.992218 simple_space-0.2.0/SimpleS/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:44:00.992218 simple_space-0.2.0/SimpleS/ImageRelated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.2.0/SimpleS/ImageRelated/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.2.0/SimpleS/ImageRelated/basics.py
--rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.2.0/SimpleS/ImageRelated/enhancements.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:44:00.992218 simple_space-0.2.0/SimpleS/Points/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.2.0/SimpleS/Points/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    12512 2024-05-30 15:58:52.000000 simple_space-0.2.0/SimpleS/Points/dimentions.py
--rw-rw-r--   0 user      (1000) user      (1000)       88 2024-05-30 15:58:29.000000 simple_space-0.2.0/SimpleS/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2024-05-30 07:41:04.000000 simple_space-0.2.0/SimpleS/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:44:00.992218 simple_space-0.2.0/Simple_Space.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11045 2024-05-30 18:44:00.000000 simple_space-0.2.0/Simple_Space.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      405 2024-05-30 18:44:00.000000 simple_space-0.2.0/Simple_Space.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 18:44:00.000000 simple_space-0.2.0/Simple_Space.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 18:44:00.000000 simple_space-0.2.0/Simple_Space.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 18:44:00.000000 simple_space-0.2.0/Simple_Space.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 18:43:45.000000 simple_space-0.2.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 18:44:00.992218 simple_space-0.2.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.817522 simple_space-0.3.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.3.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11045 2024-05-30 18:56:06.817522 simple_space-0.3.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     9972 2024-05-30 18:05:04.000000 simple_space-0.3.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.813522 simple_space-0.3.0/SimpleS/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.813522 simple_space-0.3.0/SimpleS/ImageRelated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.3.0/SimpleS/ImageRelated/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.3.0/SimpleS/ImageRelated/basics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.3.0/SimpleS/ImageRelated/enhancements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.813522 simple_space-0.3.0/SimpleS/Points/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.3.0/SimpleS/Points/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12512 2024-05-30 15:58:52.000000 simple_space-0.3.0/SimpleS/Points/dimentions.py
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2024-05-30 18:54:16.000000 simple_space-0.3.0/SimpleS/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2024-05-30 07:41:04.000000 simple_space-0.3.0/SimpleS/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 18:56:06.817522 simple_space-0.3.0/Simple_Space.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11045 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      405 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 18:56:06.000000 simple_space-0.3.0/Simple_Space.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 18:54:38.000000 simple_space-0.3.0/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 18:56:06.817522 simple_space-0.3.0/setup.cfg
```

### Comparing `simple_space-0.2.0/LICENSE` & `simple_space-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_space-0.2.0/PKG-INFO` & `simple_space-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.2.0/README.md` & `simple_space-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_space-0.2.0/SimpleS/ImageRelated/basics.py` & `simple_space-0.3.0/SimpleS/ImageRelated/basics.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.2.0/SimpleS/ImageRelated/enhancements.py` & `simple_space-0.3.0/SimpleS/ImageRelated/enhancements.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.2.0/SimpleS/Points/dimentions.py` & `simple_space-0.3.0/SimpleS/Points/dimentions.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.2.0/SimpleS/utils.py` & `simple_space-0.3.0/SimpleS/utils.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.2.0/Simple_Space.egg-info/PKG-INFO` & `simple_space-0.3.0/Simple_Space.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.2.0/pyproject.toml` & `simple_space-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Space"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Try at Better Understanding Space."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
```

