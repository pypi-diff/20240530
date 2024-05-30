# Comparing `tmp/baostockhelloworld-0.0.2.tar.gz` & `tmp/baostockhelloworld-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baostockhelloworld-0.0.2.tar", last modified: Wed May 29 08:48:05 2024, max compression
+gzip compressed data, was "dist\baostockhelloworld-0.0.4.tar", last modified: Thu May 30 02:22:40 2024, max compression
```

## Comparing `baostockhelloworld-0.0.2.tar` & `baostockhelloworld-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/baostockhelloworld.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/baostockhelloworld.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1353 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/baostockhelloworld.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       15 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/baostockhelloworld.egg-info/requires.txt
--rw-rw-rw-   0        0        0      217 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/baostockhelloworld.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/baostockhelloworld.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1353 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-29 08:48:05.000000 baostockhelloworld-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1406 2024-05-29 08:44:57.000000 baostockhelloworld-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld/
+drwxrwxrwx   0        0        0        0 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld/util/
+-rw-rw-rw-   0        0        0      428 2024-05-29 09:35:44.000000 baostockhelloworld-0.0.4/baostockhelloworld/util/helloworldutil.py
+-rw-rw-rw-   0        0        0        0 2018-02-12 05:53:24.000000 baostockhelloworld-0.0.4/baostockhelloworld/util/__init__.py
+-rw-rw-rw-   0        0        0      318 2024-05-30 01:46:36.000000 baostockhelloworld-0.0.4/baostockhelloworld/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1353 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      326 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       19 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/baostockhelloworld.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1353 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-30 02:22:40.000000 baostockhelloworld-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2024-05-30 01:47:04.000000 baostockhelloworld-0.0.4/setup.py
```

### Comparing `baostockhelloworld-0.0.2/baostockhelloworld.egg-info/PKG-INFO` & `baostockhelloworld-0.0.4/baostockhelloworld.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: baostockhelloworld
-Version: 0.0.2
+Version: 0.0.4
 Summary: A tool for outputs helloworld string information on the console
 Home-page: http://www.baostock.com
 Author: baostock
 Author-email: baostock@163.com
 License: BSD License
 Description: 
         BaoStock
```

### Comparing `baostockhelloworld-0.0.2/PKG-INFO` & `baostockhelloworld-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: baostockhelloworld
-Version: 0.0.2
+Version: 0.0.4
 Summary: A tool for outputs helloworld string information on the console
 Home-page: http://www.baostock.com
 Author: baostock
 Author-email: baostock@163.com
 License: BSD License
 Description: 
         BaoStock
```

### Comparing `baostockhelloworld-0.0.2/setup.py` & `baostockhelloworld-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     HelloWorld!
 
 """
 
 
 setup(
     name='baostockhelloworld',
-    version='0.0.2',
+    version='0.0.4',
     description=(
         'A tool for outputs helloworld string information on the console'
     ),
     long_description=long_desc,
     author='baostock',
     author_email='baostock@163.com',
     license='BSD License',
```

