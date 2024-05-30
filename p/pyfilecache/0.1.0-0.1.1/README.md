# Comparing `tmp/pyfilecache-0.1.0.tar.gz` & `tmp/pyfilecache-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfilecache-0.1.0.tar", last modified: Thu May 30 08:01:09 2024, max compression
+gzip compressed data, was "pyfilecache-0.1.1.tar", last modified: Thu May 30 08:33:27 2024, max compression
```

## Comparing `pyfilecache-0.1.0.tar` & `pyfilecache-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-05-30 08:01:09.654798 pyfilecache-0.1.0/
--rw-r--r--   0 didi       (601) staff       (20)      788 2024-05-30 08:01:09.654521 pyfilecache-0.1.0/PKG-INFO
--rw-r--r--   0 didi       (601) staff       (20)      364 2024-05-30 07:57:40.000000 pyfilecache-0.1.0/README.md
-drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-05-30 08:01:09.652388 pyfilecache-0.1.0/pyfilecache/
--rw-r--r--   0 didi       (601) staff       (20)     2549 2024-05-30 07:52:35.000000 pyfilecache-0.1.0/pyfilecache/__init__.py
-drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-05-30 08:01:09.653884 pyfilecache-0.1.0/pyfilecache.egg-info/
--rw-r--r--   0 didi       (601) staff       (20)      788 2024-05-30 08:01:09.000000 pyfilecache-0.1.0/pyfilecache.egg-info/PKG-INFO
--rw-r--r--   0 didi       (601) staff       (20)      197 2024-05-30 08:01:09.000000 pyfilecache-0.1.0/pyfilecache.egg-info/SOURCES.txt
--rw-r--r--   0 didi       (601) staff       (20)        1 2024-05-30 08:01:09.000000 pyfilecache-0.1.0/pyfilecache.egg-info/dependency_links.txt
--rw-r--r--   0 didi       (601) staff       (20)       12 2024-05-30 08:01:09.000000 pyfilecache-0.1.0/pyfilecache.egg-info/top_level.txt
--rw-r--r--   0 didi       (601) staff       (20)       90 2024-05-30 08:00:37.000000 pyfilecache-0.1.0/pyproject.toml
--rw-r--r--   0 didi       (601) staff       (20)       38 2024-05-30 08:01:09.654914 pyfilecache-0.1.0/setup.cfg
--rw-r--r--   0 didi       (601) staff       (20)      628 2024-05-30 08:00:18.000000 pyfilecache-0.1.0/setup.py
+drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-05-30 08:33:27.675646 pyfilecache-0.1.1/
+-rw-r--r--   0 didi       (601) staff       (20)      788 2024-05-30 08:33:27.675370 pyfilecache-0.1.1/PKG-INFO
+-rw-r--r--   0 didi       (601) staff       (20)      364 2024-05-30 07:57:40.000000 pyfilecache-0.1.1/README.md
+drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-05-30 08:33:27.673179 pyfilecache-0.1.1/pyfilecache/
+-rw-r--r--   0 didi       (601) staff       (20)     2546 2024-05-30 08:30:56.000000 pyfilecache-0.1.1/pyfilecache/__init__.py
+drwxr-xr-x   0 didi       (601) staff       (20)        0 2024-05-30 08:33:27.674916 pyfilecache-0.1.1/pyfilecache.egg-info/
+-rw-r--r--   0 didi       (601) staff       (20)      788 2024-05-30 08:33:27.000000 pyfilecache-0.1.1/pyfilecache.egg-info/PKG-INFO
+-rw-r--r--   0 didi       (601) staff       (20)      197 2024-05-30 08:33:27.000000 pyfilecache-0.1.1/pyfilecache.egg-info/SOURCES.txt
+-rw-r--r--   0 didi       (601) staff       (20)        1 2024-05-30 08:33:27.000000 pyfilecache-0.1.1/pyfilecache.egg-info/dependency_links.txt
+-rw-r--r--   0 didi       (601) staff       (20)       12 2024-05-30 08:33:27.000000 pyfilecache-0.1.1/pyfilecache.egg-info/top_level.txt
+-rw-r--r--   0 didi       (601) staff       (20)       90 2024-05-30 08:00:37.000000 pyfilecache-0.1.1/pyproject.toml
+-rw-r--r--   0 didi       (601) staff       (20)       38 2024-05-30 08:33:27.675752 pyfilecache-0.1.1/setup.cfg
+-rw-r--r--   0 didi       (601) staff       (20)      628 2024-05-30 08:30:41.000000 pyfilecache-0.1.1/setup.py
```

### Comparing `pyfilecache-0.1.0/PKG-INFO` & `pyfilecache-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilecache
-Version: 0.1.0
+Version: 0.1.1
 Summary: cache results of slow function to disk
 Home-page: https://github.com/HellOwhatAs/pyfilecache
 Author: HellOwhatAs
 Author-email: xjq701229@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyfilecache-0.1.0/pyfilecache/__init__.py` & `pyfilecache-0.1.1/pyfilecache/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         with open(index_dir, "wb") as f:
             index[key] = len(index)
             pickle.dump(index, f)
     KEY2INDEX_LOCK.release()
     return index[key], not flag
     
 def file_cache(
-        user_function = None, /, *,
+        user_function = None, *,
         reader: Callable[[TextIOWrapper], Any] = None,
         writer: Callable[[Any, TextIOWrapper], None] = None,
         typed: bool = False
     ):
     
     if reader is None: reader = pickle.load
     if writer is None: writer = pickle.dump
```

### Comparing `pyfilecache-0.1.0/pyfilecache.egg-info/PKG-INFO` & `pyfilecache-0.1.1/pyfilecache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilecache
-Version: 0.1.0
+Version: 0.1.1
 Summary: cache results of slow function to disk
 Home-page: https://github.com/HellOwhatAs/pyfilecache
 Author: HellOwhatAs
 Author-email: xjq701229@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyfilecache-0.1.0/setup.py` & `pyfilecache-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyfilecache",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[],
     author="HellOwhatAs",
     author_email="xjq701229@outlook.com",
     description="cache results of slow function to disk",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

