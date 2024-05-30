# Comparing `tmp/allgraph-0.1.tar.gz` & `tmp/allgraph-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allgraph-0.1.tar", last modified: Thu May 30 20:01:30 2024, max compression
+gzip compressed data, was "allgraph-0.2.tar", last modified: Thu May 30 21:10:07 2024, max compression
```

## Comparing `allgraph-0.1.tar` & `allgraph-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 20:01:30.441614 allgraph-0.1/
--rw-rw-rw-   0        0        0    19396 2024-05-30 20:01:30.437613 allgraph-0.1/PKG-INFO
--rw-rw-rw-   0        0        0    19007 2024-05-30 17:00:01.000000 allgraph-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 20:01:30.415608 allgraph-0.1/allgraph/
--rw-rw-rw-   0        0        0      371 2024-05-30 15:52:54.000000 allgraph-0.1/allgraph/__init__.py
--rw-rw-rw-   0        0        0    29851 2024-05-30 12:24:20.000000 allgraph-0.1/allgraph/main.py
-drwxrwxrwx   0        0        0        0 2024-05-30 20:01:30.434612 allgraph-0.1/allgraph.egg-info/
--rw-rw-rw-   0        0        0    19396 2024-05-30 20:01:30.000000 allgraph-0.1/allgraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-30 20:01:30.000000 allgraph-0.1/allgraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 20:01:30.000000 allgraph-0.1/allgraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-30 20:01:30.000000 allgraph-0.1/allgraph.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 20:01:30.000000 allgraph-0.1/allgraph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 20:01:30.442614 allgraph-0.1/setup.cfg
--rw-rw-rw-   0        0        0      615 2024-05-30 17:00:43.000000 allgraph-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:10:07.737880 allgraph-0.2/
+-rw-rw-rw-   0        0        0    19396 2024-05-30 21:10:07.734661 allgraph-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19007 2024-05-30 17:00:01.000000 allgraph-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 21:10:07.707498 allgraph-0.2/allgraph/
+-rw-rw-rw-   0        0        0      371 2024-05-30 15:52:54.000000 allgraph-0.2/allgraph/__init__.py
+-rw-rw-rw-   0        0        0    29851 2024-05-30 12:24:20.000000 allgraph-0.2/allgraph/main.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:10:07.732661 allgraph-0.2/allgraph.egg-info/
+-rw-rw-rw-   0        0        0    19396 2024-05-30 21:10:07.000000 allgraph-0.2/allgraph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-05-30 21:10:07.000000 allgraph-0.2/allgraph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 21:10:07.000000 allgraph-0.2/allgraph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-30 21:10:07.000000 allgraph-0.2/allgraph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 21:10:07.000000 allgraph-0.2/allgraph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 21:10:07.737880 allgraph-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      621 2024-05-30 21:00:49.000000 allgraph-0.2/setup.py
```

### Comparing `allgraph-0.1/PKG-INFO` & `allgraph-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allgraph
-Version: 0.1
+Version: 0.2
 Summary: A library for creating various types of graphs
 Home-page: https://github.com/Arnav7418/AllGraph.py
 Author: Arnav
 Author-email: arnav.singh7418@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `allgraph-0.1/README.md` & `allgraph-0.2/README.md`

 * *Files identical despite different names*

### Comparing `allgraph-0.1/allgraph/main.py` & `allgraph-0.2/allgraph/main.py`

 * *Files identical despite different names*

### Comparing `allgraph-0.1/allgraph.egg-info/PKG-INFO` & `allgraph-0.2/allgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allgraph
-Version: 0.1
+Version: 0.2
 Summary: A library for creating various types of graphs
 Home-page: https://github.com/Arnav7418/AllGraph.py
 Author: Arnav
 Author-email: arnav.singh7418@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `allgraph-0.1/setup.py` & `allgraph-0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='allgraph',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
         'squarify'
     ],
     author='Arnav',
     author_email='arnav.singh7418@gmail.com',
@@ -15,9 +15,10 @@
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Arnav7418/AllGraph.py',  
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3.6',
+    
 )
```

