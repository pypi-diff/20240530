# Comparing `tmp/myfunctions_nadiaconeaev89-0.0.5.tar.gz` & `tmp/myfunctions_nadiaconeaev89-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpbhczaorc/myfunctions_nadiaconeaev89-0.0.5.tar", last modified: Thu May 30 01:31:57 2024, max compression
+gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpiy6gr1oe/myfunctions_nadiaconeaev89-0.0.6.tar", last modified: Thu May 30 01:32:47 2024, max compression
```

## Comparing `myfunctions_nadiaconeaev89-0.0.5.tar` & `myfunctions_nadiaconeaev89-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 01:31:43.000000 myfunctions_nadiaconeaev89-0.0.5/setup.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.5/README.md
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      438 2024-05-30 01:31:04.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89/math.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89/__init__.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/PKG-INFO
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89.egg-info/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89.egg-info/top_level.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:31:57.000000 myfunctions_nadiaconeaev89-0.0.5/setup.cfg
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      655 2024-05-30 01:32:35.000000 myfunctions_nadiaconeaev89-0.0.6/setup.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.6/README.md
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      438 2024-05-30 01:31:04.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89/math.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89/__init__.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/PKG-INFO
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89.egg-info/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89.egg-info/top_level.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      341 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        3 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89.egg-info/requires.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:32:47.000000 myfunctions_nadiaconeaev89-0.0.6/setup.cfg
```

### Comparing `myfunctions_nadiaconeaev89-0.0.5/README.md` & `myfunctions_nadiaconeaev89-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_nadiaconeaev89-0.0.5/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_nadiaconeaev89
-Version: 0.0.5
+Version: 0.0.6
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_nadiaconeaev89-0.0.5/myfunctions_nadiaconeaev89.egg-info/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.6/myfunctions_nadiaconeaev89.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-nadiaconeaev89
-Version: 0.0.5
+Version: 0.0.6
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

