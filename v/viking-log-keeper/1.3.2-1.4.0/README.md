# Comparing `tmp/viking-log-keeper-1.3.2.tar.gz` & `tmp/viking-log-keeper-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viking-log-keeper-1.3.2.tar", last modified: Fri May 24 18:15:46 2024, max compression
+gzip compressed data, was "viking-log-keeper-1.4.0.tar", last modified: Wed May 29 22:03:10 2024, max compression
```

## Comparing `viking-log-keeper-1.3.2.tar` & `viking-log-keeper-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:15:46.684948 viking-log-keeper-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-24 18:15:46.684948 viking-log-keeper-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:15:46.684948 viking-log-keeper-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:15:46.680948 viking-log-keeper-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:15:46.680948 viking-log-keeper-1.3.2/src/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/dashboard/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/dashboard/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/dashboard/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/dashboard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:15:46.680948 viking-log-keeper-1.3.2/src/log_keeper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/log_keeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/log_keeper/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/log_keeper/ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/log_keeper/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/log_keeper/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-24 18:15:39.000000 viking-log-keeper-1.3.2/src/log_keeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:15:46.684948 viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-24 18:15:46.000000 viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-24 18:15:46.000000 viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:15:46.000000 viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-24 18:15:46.000000 viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-24 18:15:46.000000 viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 18:15:46.000000 viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:10.299566 viking-log-keeper-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-29 22:03:10.299566 viking-log-keeper-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:03:10.299566 viking-log-keeper-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:10.295566 viking-log-keeper-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:10.295566 viking-log-keeper-1.4.0/src/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/dashboard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/dashboard/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/dashboard/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/dashboard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:10.295566 viking-log-keeper-1.4.0/src/log_keeper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/log_keeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/log_keeper/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/log_keeper/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/log_keeper/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/log_keeper/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/src/log_keeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:10.295566 viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-29 22:03:10.000000 viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-29 22:03:10.000000 viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:03:10.000000 viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 22:03:10.000000 viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-29 22:03:10.000000 viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 22:03:10.000000 viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:03:10.299566 viking-log-keeper-1.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-29 22:03:01.000000 viking-log-keeper-1.4.0/test/test_dashboard.py
```

### Comparing `viking-log-keeper-1.3.2/LICENSE` & `viking-log-keeper-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/PKG-INFO` & `viking-log-keeper-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viking-log-keeper
-Version: 1.3.2
+Version: 1.4.0
 Summary: 661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard.
 Home-page: https://github.com/mjennings061/viking-log-keeper
 Author: Michael Jennings
 Author-email: mjennings061@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `viking-log-keeper-1.3.2/README.md` & `viking-log-keeper-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/setup.py` & `viking-log-keeper-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         destination = desktop / BAT_FILE_NAME
         shutil.copyfile(source, destination)
         logging.info('%s has been copied to %s', BAT_FILE_NAME, str(desktop))
 
 
 setup(
     name="viking-log-keeper",
-    version="1.3.2",
+    version="1.4.0",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     url="https://github.com/mjennings061/viking-log-keeper",
     license="MIT",
     author="Michael Jennings",
     author_email="mjennings061@gmail.com",
     description="661 VGS - Function to collate 2965D log sheets into a"
```

### Comparing `viking-log-keeper-1.3.2/src/dashboard/auth.py` & `viking-log-keeper-1.4.0/src/dashboard/auth.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/dashboard/main.py` & `viking-log-keeper-1.4.0/src/dashboard/main.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/dashboard/plots.py` & `viking-log-keeper-1.4.0/src/dashboard/plots.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/dashboard/utils.py` & `viking-log-keeper-1.4.0/src/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/log_keeper/get_config.py` & `viking-log-keeper-1.4.0/src/log_keeper/get_config.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/log_keeper/ingest.py` & `viking-log-keeper-1.4.0/src/log_keeper/ingest.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/log_keeper/main.py` & `viking-log-keeper-1.4.0/src/log_keeper/main.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/log_keeper/output.py` & `viking-log-keeper-1.4.0/src/log_keeper/output.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/log_keeper/utils.py` & `viking-log-keeper-1.4.0/src/log_keeper/utils.py`

 * *Files identical despite different names*

### Comparing `viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/PKG-INFO` & `viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viking-log-keeper
-Version: 1.3.2
+Version: 1.4.0
 Summary: 661 VGS - Function to collate 2965D log sheets into a master log, database, and dashboard.
 Home-page: https://github.com/mjennings061/viking-log-keeper
 Author: Michael Jennings
 Author-email: mjennings061@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `viking-log-keeper-1.3.2/src/viking_log_keeper.egg-info/SOURCES.txt` & `viking-log-keeper-1.4.0/src/viking_log_keeper.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 src/log_keeper/output.py
 src/log_keeper/utils.py
 src/viking_log_keeper.egg-info/PKG-INFO
 src/viking_log_keeper.egg-info/SOURCES.txt
 src/viking_log_keeper.egg-info/dependency_links.txt
 src/viking_log_keeper.egg-info/entry_points.txt
 src/viking_log_keeper.egg-info/requires.txt
-src/viking_log_keeper.egg-info/top_level.txt
+src/viking_log_keeper.egg-info/top_level.txt
+test/test_dashboard.py
```

