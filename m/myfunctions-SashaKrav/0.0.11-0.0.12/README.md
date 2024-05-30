# Comparing `tmp/myfunctions_SashaKrav-0.0.11.tar.gz` & `tmp/myfunctions_SashaKrav-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/SashaKrav/Python-class/class5/dist/tmpt5w4b34m/myfunctions_SashaKrav-0.0.11.tar", last modified: Thu May 30 01:19:12 2024, max compression
+gzip compressed data, was "/mnt/SashaKrav/Python-class/class5/dist/tmp1m9gqr14/myfunctions_SashaKrav-0.0.12.tar", last modified: Thu May 30 01:27:30 2024, max compression
```

## Comparing `myfunctions_SashaKrav-0.0.11.tar` & `myfunctions_SashaKrav-0.0.12.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      631 2024-05-30 01:18:51.000000 myfunctions_SashaKrav-0.0.11/setup.py
-drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/top_level.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      198 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/SOURCES.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/dependency_links.txt
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     2243 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/PKG-INFO
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     1803 2024-05-30 01:18:40.000000 myfunctions_SashaKrav-0.0.11/README.md
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     2243 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/PKG-INFO
--rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)       38 2024-05-30 01:19:12.000000 myfunctions_SashaKrav-0.0.11/setup.cfg
+drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      631 2024-05-30 01:27:15.000000 myfunctions_SashaKrav-0.0.12/setup.py
+drwxrwxr-x   0 SashaKrav  (1628) SashaKrav  (1629)        0 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/myfunctions_SashaKrav.egg-info/
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/myfunctions_SashaKrav.egg-info/top_level.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)      198 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/myfunctions_SashaKrav.egg-info/SOURCES.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)        1 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/myfunctions_SashaKrav.egg-info/dependency_links.txt
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     2243 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/myfunctions_SashaKrav.egg-info/PKG-INFO
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     1803 2024-05-30 01:18:40.000000 myfunctions_SashaKrav-0.0.12/README.md
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)     2243 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/PKG-INFO
+-rw-rw-r--   0 SashaKrav  (1628) SashaKrav  (1629)       38 2024-05-30 01:27:30.000000 myfunctions_SashaKrav-0.0.12/setup.cfg
```

### Comparing `myfunctions_SashaKrav-0.0.11/myfunctions_SashaKrav.egg-info/PKG-INFO` & `myfunctions_SashaKrav-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: myfunctions-SashaKrav
-Version: 0.0.11
+Name: myfunctions_SashaKrav
+Version: 0.0.12
 Summary: A description of your package
 Home-page: https://github.com/SashaKrav
 Author: SashaKrav
 Author-email: kravcov4k@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_SashaKrav-0.0.11/README.md` & `myfunctions_SashaKrav-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_SashaKrav-0.0.11/PKG-INFO` & `myfunctions_SashaKrav-0.0.12/myfunctions_SashaKrav.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: myfunctions_SashaKrav
-Version: 0.0.11
+Name: myfunctions-SashaKrav
+Version: 0.0.12
 Summary: A description of your package
 Home-page: https://github.com/SashaKrav
 Author: SashaKrav
 Author-email: kravcov4k@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

