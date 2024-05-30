# Comparing `tmp/pynumint-0.0.8.tar.gz` & `tmp/pynumint-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumint-0.0.8.tar", last modified: Thu May 30 14:07:58 2024, max compression
+gzip compressed data, was "pynumint-0.0.9.tar", last modified: Thu May 30 14:21:23 2024, max compression
```

## Comparing `pynumint-0.0.8.tar` & `pynumint-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.692528 pynumint-0.0.8/
--rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5453 2024-05-30 14:07:58.692528 pynumint-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.625426 pynumint-0.0.8/pynumint/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.692528 pynumint-0.0.8/pynumint/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 14:07:58.689813 pynumint-0.0.8/pynumint/src/pynumint.egg-info/
--rw-rw-rw-   0        0        0     5453 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-30 14:07:58.000000 pynumint-0.0.8/pynumint/src/pynumint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.8/pynumint/src/pynumint.py
--rw-rw-rw-   0        0        0       42 2024-05-30 14:07:58.692528 pynumint-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1836 2024-05-30 14:07:35.000000 pynumint-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.591040 pynumint-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-05-26 10:33:54.000000 pynumint-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5453 2024-05-30 14:21:23.591040 pynumint-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4434 2024-05-30 13:47:32.000000 pynumint-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.561079 pynumint-0.0.9/pynumint/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.591040 pynumint-0.0.9/pynumint/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 14:21:23.581037 pynumint-0.0.9/pynumint/src/pynumint.egg-info/
+-rw-rw-rw-   0        0        0     5453 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-30 14:21:23.000000 pynumint-0.0.9/pynumint/src/pynumint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4237 2024-05-30 07:33:34.000000 pynumint-0.0.9/pynumint/src/pynumint.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:21:23.591040 pynumint-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1856 2024-05-30 14:20:54.000000 pynumint-0.0.9/setup.py
```

### Comparing `pynumint-0.0.8/LICENSE` & `pynumint-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.8/PKG-INFO` & `pynumint-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.8
+Version: 0.0.9
 Summary: pynumint Test Package for Numerical Integration Demo
 Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
 Project-URL: Source, https://github.com/CodeSleuthX/pynumint
```

### Comparing `pynumint-0.0.8/README.md` & `pynumint-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pynumint-0.0.8/pynumint/src/pynumint.egg-info/PKG-INFO` & `pynumint-0.0.9/pynumint/src/pynumint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumint
-Version: 0.0.8
+Version: 0.0.9
 Summary: pynumint Test Package for Numerical Integration Demo
 Home-page: https://github.com/CodeSleuthX/pynumint
 Author: Arjun Jagdale
 Author-email: arjunjagdale14@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/CodeSleuthX/pynumint/issues
 Project-URL: Source, https://github.com/CodeSleuthX/pynumint
```

### Comparing `pynumint-0.0.8/pynumint/src/pynumint.py` & `pynumint-0.0.9/pynumint/src/pynumint.py`

 * *Files identical despite different names*

