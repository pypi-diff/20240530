# Comparing `tmp/bartesdk-0.1.8.tar.gz` & `tmp/bartesdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bartesdk-0.1.8.tar", last modified: Tue May 21 10:25:46 2024, max compression
+gzip compressed data, was "bartesdk-0.1.9.tar", last modified: Tue May 21 10:36:14 2024, max compression
```

## Comparing `bartesdk-0.1.8.tar` & `bartesdk-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:25:46.629469 bartesdk-0.1.8/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-21 10:23:50.000000 bartesdk-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:25:46.629469 bartesdk-0.1.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-21 10:23:50.000000 bartesdk-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:25:46.629469 bartesdk-0.1.8/bartesdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      185 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:25:46.000000 bartesdk-0.1.8/bartesdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 10:25:46.629469 bartesdk-0.1.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      562 2024-05-21 10:25:27.000000 bartesdk-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:36:14.240140 bartesdk-0.1.9/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-21 10:23:50.000000 bartesdk-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:36:14.240140 bartesdk-0.1.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3800 2024-05-21 10:23:50.000000 bartesdk-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:36:14.236140 bartesdk-0.1.9/bartesdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 10:36:14.240140 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4076 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 10:36:14.000000 bartesdk-0.1.9/bartesdk/bartesdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 10:36:14.240140 bartesdk-0.1.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      612 2024-05-21 10:36:02.000000 bartesdk-0.1.9/setup.py
```

### Comparing `bartesdk-0.1.8/PKG-INFO` & `bartesdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bartesdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bartesdk-0.1.8/README.md` & `bartesdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bartesdk-0.1.8/bartesdk.egg-info/PKG-INFO` & `bartesdk-0.1.9/bartesdk/bartesdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bartesdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

