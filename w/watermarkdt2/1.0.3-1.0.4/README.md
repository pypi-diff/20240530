# Comparing `tmp/watermarkdt2-1.0.3.tar.gz` & `tmp/watermarkdt2-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watermarkdt2-1.0.3.tar", last modified: Thu May 30 08:28:27 2024, max compression
+gzip compressed data, was "watermarkdt2-1.0.4.tar", last modified: Thu May 30 08:29:40 2024, max compression
```

## Comparing `watermarkdt2-1.0.3.tar` & `watermarkdt2-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 08:28:27.071427 watermarkdt2-1.0.3/
--rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 08:28:27.071427 watermarkdt2-1.0.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      333 2024-05-30 03:43:12.000000 watermarkdt2-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 08:28:27.071427 watermarkdt2-1.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1283 2024-05-30 08:25:06.000000 watermarkdt2-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 08:28:27.067427 watermarkdt2-1.0.3/watermarkdt2/
--rw-rw-r--   0 root         (0) root         (0)      382 2024-05-30 04:11:41.000000 watermarkdt2-1.0.3/watermarkdt2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7376 2024-05-30 08:25:06.000000 watermarkdt2-1.0.3/watermarkdt2/watermarkdt2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 08:28:27.070427 watermarkdt2-1.0.3/watermarkdt2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 08:28:26.000000 watermarkdt2-1.0.3/watermarkdt2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2024-05-30 08:28:26.000000 watermarkdt2-1.0.3/watermarkdt2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 08:28:26.000000 watermarkdt2-1.0.3/watermarkdt2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 08:28:26.000000 watermarkdt2-1.0.3/watermarkdt2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 08:29:40.975074 watermarkdt2-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 08:29:40.975074 watermarkdt2-1.0.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      333 2024-05-30 03:43:12.000000 watermarkdt2-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 08:29:40.975074 watermarkdt2-1.0.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1283 2024-05-30 08:29:08.000000 watermarkdt2-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 08:29:40.973074 watermarkdt2-1.0.4/watermarkdt2/
+-rw-rw-r--   0 root         (0) root         (0)      710 2024-05-30 08:28:40.000000 watermarkdt2-1.0.4/watermarkdt2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7376 2024-05-30 08:25:06.000000 watermarkdt2-1.0.4/watermarkdt2/watermarkdt2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 08:29:40.974074 watermarkdt2-1.0.4/watermarkdt2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-05-30 08:29:40.000000 watermarkdt2-1.0.4/watermarkdt2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2024-05-30 08:29:40.000000 watermarkdt2-1.0.4/watermarkdt2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 08:29:40.000000 watermarkdt2-1.0.4/watermarkdt2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 08:29:40.000000 watermarkdt2-1.0.4/watermarkdt2.egg-info/top_level.txt
```

### Comparing `watermarkdt2-1.0.3/PKG-INFO` & `watermarkdt2-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermarkdt2
-Version: 1.0.3
+Version: 1.0.4
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

### Comparing `watermarkdt2-1.0.3/setup.py` & `watermarkdt2-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="watermarkdt2",
-    version="1.0.3",
+    version="1.0.4",
     description="dan tri filter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="xuantrangk54",
     author_email="xuantrangk54@gmail.com",
     license="MIT",
```

### Comparing `watermarkdt2-1.0.3/watermarkdt2/watermarkdt2.py` & `watermarkdt2-1.0.4/watermarkdt2/watermarkdt2.py`

 * *Files identical despite different names*

### Comparing `watermarkdt2-1.0.3/watermarkdt2.egg-info/PKG-INFO` & `watermarkdt2-1.0.4/watermarkdt2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermarkdt2
-Version: 1.0.3
+Version: 1.0.4
 Summary: dan tri filter
 Home-page: https://medium-multiply.readthedocs.io/
 Author: xuantrangk54
 Author-email: xuantrangk54@gmail.com
 License: MIT
 Description: # DantriFilter docs
```

