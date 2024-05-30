# Comparing `tmp/dbt_command_center-0.1.3.tar.gz` & `tmp/dbt_command_center-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_command_center-0.1.3.tar", last modified: Thu May 30 10:08:38 2024, max compression
+gzip compressed data, was "dbt_command_center-0.1.4.tar", last modified: Thu May 30 11:00:41 2024, max compression
```

## Comparing `dbt_command_center-0.1.3.tar` & `dbt_command_center-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/dbt_command_center.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 10:08:38.000000 dbt_command_center-0.1.3/dbt_command_center.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:08:38.046618 dbt_command_center-0.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3663778 2024-05-30 10:08:37.000000 dbt_command_center-0.1.3/src/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-30 10:07:51.000000 dbt_command_center-0.1.3/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:00:41.343291 dbt_command_center-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-30 10:59:59.000000 dbt_command_center-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 11:00:41.343291 dbt_command_center-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-30 10:59:59.000000 dbt_command_center-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:00:41.343291 dbt_command_center-0.1.4/dbt_command_center.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-30 11:00:41.000000 dbt_command_center-0.1.4/dbt_command_center.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-30 11:00:41.000000 dbt_command_center-0.1.4/dbt_command_center.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:00:41.000000 dbt_command_center-0.1.4/dbt_command_center.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:00:41.000000 dbt_command_center-0.1.4/dbt_command_center.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 11:00:41.000000 dbt_command_center-0.1.4/dbt_command_center.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 11:00:41.000000 dbt_command_center-0.1.4/dbt_command_center.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:00:41.343291 dbt_command_center-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 10:59:59.000000 dbt_command_center-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:00:41.343291 dbt_command_center-0.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 10:59:59.000000 dbt_command_center-0.1.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3663778 2024-05-30 11:00:40.000000 dbt_command_center-0.1.4/src/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-30 10:59:59.000000 dbt_command_center-0.1.4/src/main.py
```

### Comparing `dbt_command_center-0.1.3/LICENSE` & `dbt_command_center-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_command_center-0.1.3/README.md` & `dbt_command_center-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_command_center-0.1.3/setup.py` & `dbt_command_center-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt-command-center",
-    version="0.1.3",
+    version="0.1.4",
     author="Montara team",
     author_email="support@montara.io",
     description="Stop drilling through dbt logs and start visualizing them",
     long_description="Stop drilling through dbt logs and start visualizing them",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["jsonlines"],
```

### Comparing `dbt_command_center-0.1.3/src/index.html` & `dbt_command_center-0.1.4/src/index.html`

 * *Files identical despite different names*

### Comparing `dbt_command_center-0.1.3/src/main.py` & `dbt_command_center-0.1.4/src/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from http.server import BaseHTTPRequestHandler, HTTPServer
+import shutil
 import subprocess
 import webbrowser
 import jsonlines
 import os
 from urllib.parse import urlparse
 import threading
 import importlib.resources
@@ -46,15 +47,19 @@
 
 
 def main():
     print("Starting Montara new", flush=True)
 
     # Create the montara_target directory if it doesn't exist
     print("Creating montara_target directory", flush=True)
-    if not os.path.exists(MONTARA_TARGET):
+    if os.path.exists(MONTARA_TARGET):
+        shutil.rmtree(MONTARA_TARGET)
+        print(f"Folder '{MONTARA_TARGET}' has been removed.")
+    else:
+        print(f"Folder '{MONTARA_TARGET}' does not exist.")
         os.makedirs(MONTARA_TARGET)
 
     print(f'Compiling dbt and saving the output to "{MONTARA_TARGET}"', flush=True)
     subprocess.run(
         ["dbt", "parse", "--target-path", MONTARA_TARGET],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
```

