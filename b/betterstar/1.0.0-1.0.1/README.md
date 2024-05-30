# Comparing `tmp/betterstar-1.0.0.tar.gz` & `tmp/betterstar-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterstar-1.0.0.tar", last modified: Thu May 30 10:51:32 2024, max compression
+gzip compressed data, was "betterstar-1.0.1.tar", last modified: Thu May 30 11:03:04 2024, max compression
```

## Comparing `betterstar-1.0.0.tar` & `betterstar-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:51:32.975211 betterstar-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-30 10:51:25.000000 betterstar-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 10:51:25.000000 betterstar-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 10:51:32.975211 betterstar-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-30 10:51:25.000000 betterstar-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:51:32.975211 betterstar-1.0.0/betterstar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 10:51:32.000000 betterstar-1.0.0/betterstar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 10:51:32.000000 betterstar-1.0.0/betterstar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:51:32.000000 betterstar-1.0.0/betterstar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 10:51:32.000000 betterstar-1.0.0/betterstar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 10:51:32.000000 betterstar-1.0.0/betterstar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:51:32.975211 betterstar-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-30 10:51:25.000000 betterstar-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:51:32.975211 betterstar-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 10:51:25.000000 betterstar-1.0.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 10:51:25.000000 betterstar-1.0.0/src/betterstar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:03:04.331694 betterstar-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-30 11:02:56.000000 betterstar-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 11:02:56.000000 betterstar-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 11:03:04.331694 betterstar-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-30 11:02:56.000000 betterstar-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:03:04.331694 betterstar-1.0.1/betterstar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-30 11:03:04.000000 betterstar-1.0.1/betterstar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 11:03:04.000000 betterstar-1.0.1/betterstar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:03:04.000000 betterstar-1.0.1/betterstar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 11:03:04.000000 betterstar-1.0.1/betterstar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 11:03:04.000000 betterstar-1.0.1/betterstar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:03:04.331694 betterstar-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-30 11:02:56.000000 betterstar-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:03:04.331694 betterstar-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 11:02:56.000000 betterstar-1.0.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 11:02:56.000000 betterstar-1.0.1/src/betterstar.py
```

### Comparing `betterstar-1.0.0/LICENSE` & `betterstar-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betterstar-1.0.0/PKG-INFO` & `betterstar-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterstar
-Version: 1.0.0
+Version: 1.0.1
 Summary: A better looking star marker for matplotlib plots.
 Home-page: https://github.com/muederotter/betterstar
 Author: Ole Meiforth
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `betterstar-1.0.0/README.md` & `betterstar-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `betterstar-1.0.0/betterstar.egg-info/PKG-INFO` & `betterstar-1.0.1/betterstar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterstar
-Version: 1.0.0
+Version: 1.0.1
 Summary: A better looking star marker for matplotlib plots.
 Home-page: https://github.com/muederotter/betterstar
 Author: Ole Meiforth
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `betterstar-1.0.0/setup.py` & `betterstar-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="betterstar",
-    version="1.0.0",
+    version="1.0.1",
     author="Ole Meiforth",
     description="A better looking star marker for matplotlib plots.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/muederotter/betterstar',
     packages=find_packages(),
     classifiers=[
```

