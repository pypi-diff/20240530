# Comparing `tmp/apkpatcher-0.1.3.tar.gz` & `tmp/apkpatcher-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apkpatcher-0.1.3.tar", last modified: Wed May 15 10:54:34 2024, max compression
+gzip compressed data, was "apkpatcher-0.1.4.tar", last modified: Thu May 30 07:52:33 2024, max compression
```

## Comparing `apkpatcher-0.1.3.tar` & `apkpatcher-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.960172 apkpatcher-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    23045 2024-05-15 10:54:34.959172 apkpatcher-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 10:54:34.960172 apkpatcher-0.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.956172 apkpatcher-0.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.957172 apkpatcher-0.1.3/src/apkpatcher/
--rw-rw-rw-   0 root         (0) root         (0)    26510 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-15 10:54:07.000000 apkpatcher-0.1.3/src/apkpatcher/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 10:54:34.959172 apkpatcher-0.1.3/src/apkpatcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23045 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-15 10:54:34.000000 apkpatcher-0.1.3/src/apkpatcher.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.196462 apkpatcher-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23045 2024-05-30 07:52:33.196462 apkpatcher-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 07:52:33.196462 apkpatcher-0.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.192462 apkpatcher-0.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.194462 apkpatcher-0.1.4/src/apkpatcher/
+-rw-rw-rw-   0 root         (0) root         (0)    26590 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-30 07:52:06.000000 apkpatcher-0.1.4/src/apkpatcher/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 07:52:33.195462 apkpatcher-0.1.4/src/apkpatcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23045 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-30 07:52:33.000000 apkpatcher-0.1.4/src/apkpatcher.egg-info/top_level.txt
```

### Comparing `apkpatcher-0.1.3/LICENSE` & `apkpatcher-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.3/PKG-INFO` & `apkpatcher-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
```

### Comparing `apkpatcher-0.1.3/README.md` & `apkpatcher-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.3/pyproject.toml` & `apkpatcher-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apkpatcher-0.1.3/src/apkpatcher/__init__.py` & `apkpatcher-0.1.4/src/apkpatcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import time
 import signal
 import shutil
 import os.path
 import argparse
 import tempfile
 import subprocess
-import sty
 import logging
 from pathlib import Path
 
 from androguard.core import axml
 from . import conf
 import pyaxml
 import xml.etree.ElementTree as ET
@@ -258,15 +257,16 @@
 
     def extract_apk(self):
         '''
         Extract the apk on the temporary folder
         '''
 
         logging.info(f"Extracting {self.apk} (without resources) to {self.final_dir}")
-        subprocess.check_output(['apktool', '-f', '-r', 'd', '-o', self.final_dir , self.apk])
+        result = subprocess.check_output(" ".join(['apktool', '-f', '-r', 'd', '-o', self.final_dir , self.apk]), shell=True)
+        print(result.decode('utf-8'))
 
     def sign_and_zipalign(self, apk_path):
         '''
         sign and zipalign file
         '''
 
         logging.info('Optimizing with zipalign...')
@@ -326,15 +326,15 @@
                 timestamp = str(time.time()).replace('.', '')
                 new_file_name = target_file.replace('.apk', '_{0}.apk'.format(timestamp))
                 target_file = new_file_name
 
         logging.info('Repackaging apk to {0}'.format(target_file))
         logging.info('This may take some time...')
 
-        subprocess.check_output(['apktool', 'b', '-o', target_file, self.final_dir])
+        subprocess.check_output(" ".join(['apktool', 'b', '-o', target_file, self.final_dir]), shell=True)
 
         return target_file
 
 
 ################################################################################
 #                                                                              #
 #                INJECT NATIVE CODE                                            #
```

### Comparing `apkpatcher-0.1.3/src/apkpatcher/cli.py` & `apkpatcher-0.1.4/src/apkpatcher/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -34,14 +34,22 @@
         print(f"version {conf.VERSION}")
         return 0
 
     if len(sys.argv) == 1 or not (args.apk and \
                                   args.sdktools and \
                                   args.version_buildtools):
         print("apkpatcher -a <apk> -s <sdktools> -b <version> [options]")
+        if not args.apk:
+            print("\nArgument apk is missing, you should add '-a myapk.apk'")
+        if not args.sdktools:
+            print("\nArgument sdktools is missing, you should add '-s /usr/lib/android-sdk'")
+            print("If you didn't have installed sdktools follow this tutorial: https://madsquirrels.gitlab.io/mobile/asthook/how.install.html#setup-sdktools")
+        if not args.version_buildtools:
+            print("\nArgument version_buildtools is missing, you should add '-b 30.0.2'")
+            print("To know buildtools installed you can use: sdkmanager --list")
         parser.print_help()
         return 1
 
     if args.verbosity:
         if args.verbosity == 3:
             logging.basicConfig(level=logging.DEBUG)
         if args.verbosity == 2:
```

### Comparing `apkpatcher-0.1.3/src/apkpatcher.egg-info/PKG-INFO` & `apkpatcher-0.1.4/src/apkpatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apkpatcher
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tool use as library or in cli to patch an APK, inject some libraries inside the APK or add a custom certificate
 Author-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 Maintainer-email: "Benoit Forgette (MadSquirrel)" <benoit.forgette@ci-yow.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc., <http://fsf.org/>
```

