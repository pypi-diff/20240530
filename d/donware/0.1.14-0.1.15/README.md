# Comparing `tmp/donware-0.1.14.tar.gz` & `tmp/donware-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donware-0.1.14.tar", last modified: Sun May 19 06:17:06 2024, max compression
+gzip compressed data, was "donware-0.1.15.tar", last modified: Thu May 30 00:58:25 2024, max compression
```

## Comparing `donware-0.1.14.tar` & `donware-0.1.15.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:17:06.467984 donware-0.1.14/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 06:16:38.000000 donware-0.1.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 06:16:38.000000 donware-0.1.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-19 06:17:06.467984 donware-0.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 06:16:38.000000 donware-0.1.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:17:06.467984 donware-0.1.14/donware/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-19 06:16:38.000000 donware-0.1.14/donware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:17:06.467984 donware-0.1.14/donware/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:16:38.000000 donware-0.1.14/donware/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:17:06.467984 donware-0.1.14/donware/src/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:16:38.000000 donware-0.1.14/donware/src/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:17:06.467984 donware-0.1.14/donware/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:16:38.000000 donware-0.1.14/donware/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-19 06:16:38.000000 donware-0.1.14/donware/src/utils/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 06:16:38.000000 donware-0.1.14/donware/src/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-19 06:16:38.000000 donware-0.1.14/donware/src/utils/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:17:06.467984 donware-0.1.14/donware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-19 06:17:06.000000 donware-0.1.14/donware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-19 06:17:06.000000 donware-0.1.14/donware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 06:17:06.000000 donware-0.1.14/donware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 06:17:06.000000 donware-0.1.14/donware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 06:17:06.467984 donware-0.1.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-19 06:16:38.000000 donware-0.1.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:25.316025 donware-0.1.15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-30 00:58:03.000000 donware-0.1.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 00:58:03.000000 donware-0.1.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-30 00:58:25.316025 donware-0.1.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-30 00:58:03.000000 donware-0.1.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:25.312024 donware-0.1.15/donware/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 00:58:03.000000 donware-0.1.15/donware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:25.316025 donware-0.1.15/donware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:03.000000 donware-0.1.15/donware/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:25.316025 donware-0.1.15/donware/src/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:03.000000 donware-0.1.15/donware/src/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:25.316025 donware-0.1.15/donware/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:03.000000 donware-0.1.15/donware/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-30 00:58:03.000000 donware-0.1.15/donware/src/utils/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-30 00:58:03.000000 donware-0.1.15/donware/src/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-30 00:58:03.000000 donware-0.1.15/donware/src/utils/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:58:25.316025 donware-0.1.15/donware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-30 00:58:25.000000 donware-0.1.15/donware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-30 00:58:25.000000 donware-0.1.15/donware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 00:58:25.000000 donware-0.1.15/donware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 00:58:25.000000 donware-0.1.15/donware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 00:58:25.316025 donware-0.1.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-30 00:58:03.000000 donware-0.1.15/setup.py
```

### Comparing `donware-0.1.14/LICENSE` & `donware-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `donware-0.1.14/PKG-INFO` & `donware-0.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donware
-Version: 0.1.14
+Version: 0.1.15
 Summary: Don's personal toolkits for data science and machine learning.
 Home-page: https://github.com/Don-Yin/donware
 Author: Don Yin
 Author-email: Don_Yin@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `donware-0.1.14/donware/src/utils/images.py` & `donware-0.1.15/donware/src/utils/images.py`

 * *Files identical despite different names*

### Comparing `donware-0.1.14/donware/src/utils/package.py` & `donware-0.1.15/donware/src/utils/package.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from terminal import banner
+from donware import banner
 from rich import print
 import inspect
 
 
 def inspect_package(package):
     """
     Lists all functions within a given package along with their docstrings.
```

### Comparing `donware-0.1.14/donware/src/utils/terminal.py` & `donware-0.1.15/donware/src/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `donware-0.1.14/donware.egg-info/PKG-INFO` & `donware-0.1.15/donware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donware
-Version: 0.1.14
+Version: 0.1.15
 Summary: Don's personal toolkits for data science and machine learning.
 Home-page: https://github.com/Don-Yin/donware
 Author: Don Yin
 Author-email: Don_Yin@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `donware-0.1.14/setup.py` & `donware-0.1.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="donware",
-    version="0.1.14",
+    version="0.1.15",
     author="Don Yin",
     author_email="Don_Yin@outlook.com",
     description="Don's personal toolkits for data science and machine learning.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Don-Yin/donware",
     packages=find_packages(),
```

