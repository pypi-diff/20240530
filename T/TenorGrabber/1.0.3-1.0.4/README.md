# Comparing `tmp/tenorgrabber-1.0.3.tar.gz` & `tmp/tenorgrabber-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenorgrabber-1.0.3.tar", last modified: Wed May 29 11:37:17 2024, max compression
+gzip compressed data, was "tenorgrabber-1.0.4.tar", last modified: Wed May 29 11:48:16 2024, max compression
```

## Comparing `tenorgrabber-1.0.3.tar` & `tenorgrabber-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:17.386899 tenorgrabber-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 11:37:13.000000 tenorgrabber-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 11:37:17.386899 tenorgrabber-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-29 11:37:13.000000 tenorgrabber-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:17.386899 tenorgrabber-1.0.3/TenorGrabber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:13.000000 tenorgrabber-1.0.3/TenorGrabber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 11:37:13.000000 tenorgrabber-1.0.3/TenorGrabber/tenorgrabber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:17.386899 tenorgrabber-1.0.3/TenorGrabber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 11:37:17.000000 tenorgrabber-1.0.3/TenorGrabber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 11:37:17.000000 tenorgrabber-1.0.3/TenorGrabber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:37:17.000000 tenorgrabber-1.0.3/TenorGrabber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 11:37:17.000000 tenorgrabber-1.0.3/TenorGrabber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 11:37:17.000000 tenorgrabber-1.0.3/TenorGrabber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:37:17.386899 tenorgrabber-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-29 11:37:13.000000 tenorgrabber-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:17.386899 tenorgrabber-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:13.000000 tenorgrabber-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 11:37:13.000000 tenorgrabber-1.0.3/tests/tenorgrabber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:48:16.029860 tenorgrabber-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 11:48:12.000000 tenorgrabber-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 11:48:16.029860 tenorgrabber-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-29 11:48:12.000000 tenorgrabber-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:48:16.025860 tenorgrabber-1.0.4/TenorGrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:48:12.000000 tenorgrabber-1.0.4/TenorGrabber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 11:48:12.000000 tenorgrabber-1.0.4/TenorGrabber/tenorgrabber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:48:16.029860 tenorgrabber-1.0.4/TenorGrabber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 11:48:16.000000 tenorgrabber-1.0.4/TenorGrabber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 11:48:16.000000 tenorgrabber-1.0.4/TenorGrabber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:48:16.000000 tenorgrabber-1.0.4/TenorGrabber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 11:48:16.000000 tenorgrabber-1.0.4/TenorGrabber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 11:48:16.000000 tenorgrabber-1.0.4/TenorGrabber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:48:16.029860 tenorgrabber-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-29 11:48:12.000000 tenorgrabber-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:48:16.029860 tenorgrabber-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:48:12.000000 tenorgrabber-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 11:48:12.000000 tenorgrabber-1.0.4/tests/tenorgrabber.py
```

### Comparing `tenorgrabber-1.0.3/LICENSE` & `tenorgrabber-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tenorgrabber-1.0.3/PKG-INFO` & `tenorgrabber-1.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: TenorGrabber
-Version: 1.0.3
-Summary: Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
+Version: 1.0.4
+Summary: Get the direct link to a tenor GIF on python3!
 Author: user0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # TenorGrabber
 Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
```

### Comparing `tenorgrabber-1.0.3/README.md` & `tenorgrabber-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tenorgrabber-1.0.3/TenorGrabber.egg-info/PKG-INFO` & `tenorgrabber-1.0.4/TenorGrabber.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: TenorGrabber
-Version: 1.0.3
-Summary: Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
+Version: 1.0.4
+Summary: Get the direct link to a tenor GIF on python3!
 Author: user0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # TenorGrabber
 Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
```

