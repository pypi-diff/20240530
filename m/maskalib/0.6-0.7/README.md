# Comparing `tmp/maskalib-0.6.tar.gz` & `tmp/maskalib-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maskalib-0.6.tar", last modified: Wed May 29 11:00:02 2024, max compression
+gzip compressed data, was "maskalib-0.7.tar", last modified: Thu May 30 02:12:34 2024, max compression
```

## Comparing `maskalib-0.6.tar` & `maskalib-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:00:02.827686 maskalib-0.6/
--rw-rw-rw-   0        0        0     1112 2024-05-29 11:00:02.826180 maskalib-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-26 02:18:54.000000 maskalib-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:00:02.822182 maskalib-0.6/maskalib/
--rw-rw-rw-   0        0        0     8267 2024-05-26 01:56:06.000000 maskalib-0.6/maskalib/MaskaAI.py
--rw-rw-rw-   0        0        0     8107 2024-05-26 02:00:24.000000 maskalib-0.6/maskalib/MaskaAIPremium.py
--rw-rw-rw-   0        0        0      135 2024-05-29 00:21:54.000000 maskalib-0.6/maskalib/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-26 01:47:54.000000 maskalib-0.6/maskalib/main.py
--rw-rw-rw-   0        0        0     6806 2024-05-29 10:58:45.000000 maskalib-0.6/maskalib/ps99invest.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:00:02.826180 maskalib-0.6/maskalib.egg-info/
--rw-rw-rw-   0        0        0     1112 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-29 11:00:02.000000 maskalib-0.6/maskalib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 11:00:02.827686 maskalib-0.6/setup.cfg
--rw-rw-rw-   0        0        0      373 2024-05-29 10:59:19.000000 maskalib-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:12:34.398569 maskalib-0.7/
+-rw-rw-rw-   0        0        0     1112 2024-05-30 02:12:34.397568 maskalib-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-26 02:18:54.000000 maskalib-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 02:12:34.392544 maskalib-0.7/maskalib/
+-rw-rw-rw-   0        0        0     8267 2024-05-26 01:56:06.000000 maskalib-0.7/maskalib/MaskaAI.py
+-rw-rw-rw-   0        0        0     8107 2024-05-26 02:00:24.000000 maskalib-0.7/maskalib/MaskaAIPremium.py
+-rw-rw-rw-   0        0        0      174 2024-05-30 02:09:07.000000 maskalib-0.7/maskalib/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-26 01:47:54.000000 maskalib-0.7/maskalib/main.py
+-rw-rw-rw-   0        0        0    19666 2024-05-30 02:07:54.000000 maskalib-0.7/maskalib/ps99invest.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:12:34.396566 maskalib-0.7/maskalib.egg-info/
+-rw-rw-rw-   0        0        0     1112 2024-05-30 02:12:34.000000 maskalib-0.7/maskalib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-30 02:12:34.000000 maskalib-0.7/maskalib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 02:12:34.000000 maskalib-0.7/maskalib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 02:12:34.000000 maskalib-0.7/maskalib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 02:12:34.398569 maskalib-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      373 2024-05-30 02:12:16.000000 maskalib-0.7/setup.py
```

### Comparing `maskalib-0.6/PKG-INFO` & `maskalib-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maskalib
-Version: 0.6
+Version: 0.7
 Description-Content-Type: text/markdown
 
 # Maskalib
 
 Maskalib is a Python library for [describe the purpose of your library].
 
 ## Installation
```

### Comparing `maskalib-0.6/README.md` & `maskalib-0.7/README.md`

 * *Files identical despite different names*

### Comparing `maskalib-0.6/maskalib/MaskaAI.py` & `maskalib-0.7/maskalib/MaskaAI.py`

 * *Files identical despite different names*

### Comparing `maskalib-0.6/maskalib/MaskaAIPremium.py` & `maskalib-0.7/maskalib/MaskaAIPremium.py`

 * *Files identical despite different names*

### Comparing `maskalib-0.6/maskalib.egg-info/PKG-INFO` & `maskalib-0.7/maskalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maskalib
-Version: 0.6
+Version: 0.7
 Description-Content-Type: text/markdown
 
 # Maskalib
 
 Maskalib is a Python library for [describe the purpose of your library].
 
 ## Installation
```

