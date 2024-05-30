# Comparing `tmp/habslib-0.1.8.tar.gz` & `tmp/habslib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habslib-0.1.8.tar", last modified: Tue May 28 16:40:50 2024, max compression
+gzip compressed data, was "habslib-0.1.9.tar", last modified: Wed May 29 07:38:33 2024, max compression
```

## Comparing `habslib-0.1.8.tar` & `habslib-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:40:50.291334 habslib-0.1.8/
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:40:50.289799 habslib-0.1.8/HABSlib/
--rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.8/HABSlib/__init__.py
--rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.8/HABSlib/board_manager.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.8/HABSlib/config.py
--rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.8/HABSlib/crypt.py
--rw-r--r--   0 do         (501) staff       (20)    15619 2024-05-28 16:36:52.000000 habslib-0.1.8/HABSlib/service.py
--rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.8/HABSlib/utils.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:40:50.290971 habslib-0.1.8/HABSlib.egg-info/
--rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 16:40:50.000000 habslib-0.1.8/HABSlib.egg-info/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)      399 2024-05-28 16:40:50.000000 habslib-0.1.8/HABSlib.egg-info/SOURCES.txt
--rw-r--r--   0 do         (501) staff       (20)        1 2024-05-28 16:40:50.000000 habslib-0.1.8/HABSlib.egg-info/dependency_links.txt
--rw-r--r--   0 do         (501) staff       (20)      167 2024-05-28 16:40:50.000000 habslib-0.1.8/HABSlib.egg-info/requires.txt
--rw-r--r--   0 do         (501) staff       (20)       14 2024-05-28 16:40:50.000000 habslib-0.1.8/HABSlib.egg-info/top_level.txt
--rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.8/LICENCE
--rw-r--r--   0 do         (501) staff       (20)       42 2024-05-27 22:43:14.000000 habslib-0.1.8/MANIFEST.in
--rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 16:40:50.291162 habslib-0.1.8/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)     1215 2024-05-28 15:35:25.000000 habslib-0.1.8/README.md
--rw-r--r--   0 do         (501) staff       (20)      172 2024-05-28 15:44:25.000000 habslib-0.1.8/requirements.txt
--rw-r--r--   0 do         (501) staff       (20)       38 2024-05-28 16:40:50.291366 habslib-0.1.8/setup.cfg
--rw-r--r--   0 do         (501) staff       (20)     1018 2024-05-28 16:36:59.000000 habslib-0.1.8/setup.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:40:50.290784 habslib-0.1.8/tests/
--rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.8/tests/__init__.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.8/tests/config.py
--rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.8/tests/conftest.py
--rw-r--r--   0 do         (501) staff       (20)     8909 2024-05-28 15:51:37.000000 habslib-0.1.8/tests/test_habslib.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-29 07:38:33.521508 habslib-0.1.9/
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-29 07:38:33.519987 habslib-0.1.9/HABSlib/
+-rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.9/HABSlib/__init__.py
+-rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.9/HABSlib/board_manager.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.9/HABSlib/config.py
+-rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.9/HABSlib/crypt.py
+-rw-r--r--   0 do         (501) staff       (20)     1142 2024-05-23 15:47:32.000000 habslib-0.1.9/HABSlib/metadata.json
+-rw-r--r--   0 do         (501) staff       (20)    15619 2024-05-29 07:37:49.000000 habslib-0.1.9/HABSlib/service.py
+-rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.9/HABSlib/utils.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-29 07:38:33.521159 habslib-0.1.9/HABSlib.egg-info/
+-rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-29 07:38:33.000000 habslib-0.1.9/HABSlib.egg-info/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)      421 2024-05-29 07:38:33.000000 habslib-0.1.9/HABSlib.egg-info/SOURCES.txt
+-rw-r--r--   0 do         (501) staff       (20)        1 2024-05-29 07:38:33.000000 habslib-0.1.9/HABSlib.egg-info/dependency_links.txt
+-rw-r--r--   0 do         (501) staff       (20)      167 2024-05-29 07:38:33.000000 habslib-0.1.9/HABSlib.egg-info/requires.txt
+-rw-r--r--   0 do         (501) staff       (20)        1 2024-05-29 07:38:33.000000 habslib-0.1.9/HABSlib.egg-info/top_level.txt
+-rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.9/LICENCE
+-rw-r--r--   0 do         (501) staff       (20)       73 2024-05-29 07:32:04.000000 habslib-0.1.9/MANIFEST.in
+-rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-29 07:38:33.521340 habslib-0.1.9/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)     1215 2024-05-28 15:35:25.000000 habslib-0.1.9/README.md
+-rw-r--r--   0 do         (501) staff       (20)      172 2024-05-28 15:44:25.000000 habslib-0.1.9/requirements.txt
+-rw-r--r--   0 do         (501) staff       (20)       38 2024-05-29 07:38:33.521549 habslib-0.1.9/setup.cfg
+-rw-r--r--   0 do         (501) staff       (20)     1064 2024-05-29 07:34:06.000000 habslib-0.1.9/setup.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-29 07:38:33.520959 habslib-0.1.9/tests/
+-rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.9/tests/__init__.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.9/tests/config.py
+-rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.9/tests/conftest.py
+-rw-r--r--   0 do         (501) staff       (20)     8909 2024-05-28 15:51:37.000000 habslib-0.1.9/tests/test_habslib.py
```

### Comparing `habslib-0.1.8/HABSlib/board_manager.py` & `habslib-0.1.9/HABSlib/board_manager.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.8/HABSlib/crypt.py` & `habslib-0.1.9/HABSlib/crypt.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.8/HABSlib/service.py` & `habslib-0.1.9/HABSlib/service.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.8/HABSlib/utils.py` & `habslib-0.1.9/HABSlib/utils.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.8/HABSlib.egg-info/PKG-INFO` & `habslib-0.1.9/HABSlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `habslib-0.1.8/LICENCE` & `habslib-0.1.9/LICENCE`

 * *Files identical despite different names*

### Comparing `habslib-0.1.8/PKG-INFO` & `habslib-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `habslib-0.1.8/README.md` & `habslib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `habslib-0.1.8/setup.py` & `habslib-0.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="HABSlib",
-    version="0.1.8",
+    version="0.1.9",
     author="Domenico Guarino",
     author_email="domenico@habs.ai",
     description="A library for interacting with the HABS BrainOS API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Olocufier/HABS.git",
-    packages=find_packages(),
+    packages=find_packages(where="HABSlib"),
+    include_package_data=True,
     install_requires=[
         "asyncio==3.4.3",
         "brainflow==5.12.1",
         "numpy==1.26.4",
         "requests==2.31.0",
         "scipy==1.13.0",
         "urllib3==2.2.1",
```

### Comparing `habslib-0.1.8/tests/conftest.py` & `habslib-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.8/tests/test_habslib.py` & `habslib-0.1.9/tests/test_habslib.py`

 * *Files identical despite different names*

