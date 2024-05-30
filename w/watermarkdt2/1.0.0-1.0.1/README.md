# Comparing `tmp/watermarkdt2-1.0.0.tar.gz` & `tmp/watermarkdt2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watermarkdt2-1.0.0.tar", last modified: Thu May 30 03:59:16 2024, max compression
+gzip compressed data, was "watermarkdt2-1.0.1.tar", last modified: Thu May 30 04:12:46 2024, max compression
```

## Comparing `watermarkdt2-1.0.0.tar` & `watermarkdt2-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 03:59:16.922052 watermarkdt2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 03:59:16.921052 watermarkdt2-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      333 2024-05-30 03:43:12.000000 watermarkdt2-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 03:59:16.923052 watermarkdt2-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1283 2024-05-30 03:45:27.000000 watermarkdt2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 03:59:16.916052 watermarkdt2-1.0.0/watermarkdt2/
--rw-rw-r--   0 root         (0) root         (0)      322 2024-05-30 03:43:12.000000 watermarkdt2-1.0.0/watermarkdt2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7389 2024-05-30 03:43:12.000000 watermarkdt2-1.0.0/watermarkdt2/watermarkdt2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 03:59:16.920052 watermarkdt2-1.0.0/watermarkdt2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 03:59:16.000000 watermarkdt2-1.0.0/watermarkdt2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-30 03:59:16.000000 watermarkdt2-1.0.0/watermarkdt2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 03:59:16.000000 watermarkdt2-1.0.0/watermarkdt2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 03:59:16.000000 watermarkdt2-1.0.0/watermarkdt2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 04:12:46.075274 watermarkdt2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 04:12:46.074274 watermarkdt2-1.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      333 2024-05-30 03:43:12.000000 watermarkdt2-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 04:12:46.075274 watermarkdt2-1.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1283 2024-05-30 04:11:41.000000 watermarkdt2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 04:12:46.070274 watermarkdt2-1.0.1/watermarkdt2/
+-rw-rw-r--   0 root         (0) root         (0)      382 2024-05-30 04:11:41.000000 watermarkdt2-1.0.1/watermarkdt2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7389 2024-05-30 03:43:12.000000 watermarkdt2-1.0.1/watermarkdt2/watermarkdt2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 04:12:46.073274 watermarkdt2-1.0.1/watermarkdt2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 04:12:45.000000 watermarkdt2-1.0.1/watermarkdt2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-30 04:12:45.000000 watermarkdt2-1.0.1/watermarkdt2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 04:12:45.000000 watermarkdt2-1.0.1/watermarkdt2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 04:12:45.000000 watermarkdt2-1.0.1/watermarkdt2.egg-info/top_level.txt
```

### Comparing `watermarkdt2-1.0.0/PKG-INFO` & `watermarkdt2-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermarkdt2
-Version: 1.0.0
+Version: 1.0.1
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `watermarkdt2-1.0.0/setup.py` & `watermarkdt2-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="watermarkdt2",
-    version="1.0.0",
+    version="1.0.1",
     description="dan tri filter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="xuantrangk54",
     author_email="xuantrangk54@gmail.com",
     license="MIT",
```

### Comparing `watermarkdt2-1.0.0/watermarkdt2/watermarkdt2.py` & `watermarkdt2-1.0.1/watermarkdt2/watermarkdt2.py`

 * *Files identical despite different names*

### Comparing `watermarkdt2-1.0.0/watermarkdt2.egg-info/PKG-INFO` & `watermarkdt2-1.0.1/watermarkdt2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermarkdt2
-Version: 1.0.0
+Version: 1.0.1
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

