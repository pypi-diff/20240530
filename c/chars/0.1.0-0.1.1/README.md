# Comparing `tmp/chars-0.1.0.tar.gz` & `tmp/chars-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chars-0.1.0.tar", last modified: Thu May 30 06:13:45 2024, max compression
+gzip compressed data, was "chars-0.1.1.tar", last modified: Thu May 30 06:19:57 2024, max compression
```

## Comparing `chars-0.1.0.tar` & `chars-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:13:45.920282 chars-0.1.0/
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)     1070 2024-05-30 06:13:31.000000 chars-0.1.0/LICENSE.txt
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)      575 2024-05-30 06:13:45.920044 chars-0.1.0/PKG-INFO
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)      191 2024-05-30 06:13:32.000000 chars-0.1.0/README.md
-drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:13:45.919862 chars-0.1.0/chars.egg-info/
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)      575 2024-05-30 06:13:45.000000 chars-0.1.0/chars.egg-info/PKG-INFO
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)      223 2024-05-30 06:13:45.000000 chars-0.1.0/chars.egg-info/SOURCES.txt
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)        1 2024-05-30 06:13:45.000000 chars-0.1.0/chars.egg-info/dependency_links.txt
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)       16 2024-05-30 06:13:45.000000 chars-0.1.0/chars.egg-info/top_level.txt
-drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:13:45.919597 chars-0.1.0/charset_project/
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)       71 2024-05-30 06:04:32.000000 chars-0.1.0/charset_project/__init__.py
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)      438 2024-05-30 06:13:38.000000 chars-0.1.0/charset_project/charset.py
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)       38 2024-05-30 06:13:45.920330 chars-0.1.0/setup.cfg
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)      594 2024-05-30 06:13:41.000000 chars-0.1.0/setup.py
-drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:13:45.919700 chars-0.1.0/tests/
--rw-r--r--   0 piyushpaliwal   (501) staff       (20)      727 2024-05-30 06:13:34.000000 chars-0.1.0/tests/test_charset.py
+drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:19:57.213405 chars-0.1.1/
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)     1070 2024-05-30 06:13:31.000000 chars-0.1.1/LICENSE.txt
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)      831 2024-05-30 06:19:57.213153 chars-0.1.1/PKG-INFO
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)      446 2024-05-30 06:18:29.000000 chars-0.1.1/README.md
+drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:19:57.212988 chars-0.1.1/chars.egg-info/
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)      831 2024-05-30 06:19:57.000000 chars-0.1.1/chars.egg-info/PKG-INFO
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)      223 2024-05-30 06:19:57.000000 chars-0.1.1/chars.egg-info/SOURCES.txt
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)        1 2024-05-30 06:19:57.000000 chars-0.1.1/chars.egg-info/dependency_links.txt
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)       16 2024-05-30 06:19:57.000000 chars-0.1.1/chars.egg-info/top_level.txt
+drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:19:57.212520 chars-0.1.1/charset_project/
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)       71 2024-05-30 06:04:32.000000 chars-0.1.1/charset_project/__init__.py
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)      438 2024-05-30 06:13:38.000000 chars-0.1.1/charset_project/charset.py
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)       38 2024-05-30 06:19:57.213456 chars-0.1.1/setup.cfg
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)      594 2024-05-30 06:19:18.000000 chars-0.1.1/setup.py
+drwxr-xr-x   0 piyushpaliwal   (501) staff       (20)        0 2024-05-30 06:19:57.212731 chars-0.1.1/tests/
+-rw-r--r--   0 piyushpaliwal   (501) staff       (20)      727 2024-05-30 06:13:34.000000 chars-0.1.1/tests/test_charset.py
```

### Comparing `chars-0.1.0/LICENSE.txt` & `chars-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chars-0.1.0/PKG-INFO` & `chars-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,33 @@
 Metadata-Version: 2.1
 Name: chars
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for character sets
 Author: PiyushThePal
 Author-email: cool_guy2331708@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # mypackage
 
-mypackage is a simple Python package that provides functions to get different sets of characters including uppercase letters, lowercase letters, numbers, and special characters.
+chars is a simple Python package that provides functions to get different sets of characters including uppercase letters, lowercase letters, numbers, and special characters.
+
+## Features
+
+- Retrieve uppercase letters
+- Retrieve lowercase letters
+- Retrieve numbers
+- Retrieve special characters
+- Retrieve a combination of all character sets
+
+## Installation
+
+You can install the package using `pip`:
+
+```sh
+pip install chars
+```
+END
```

### Comparing `chars-0.1.0/chars.egg-info/PKG-INFO` & `chars-0.1.1/chars.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,33 @@
 Metadata-Version: 2.1
 Name: chars
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for character sets
 Author: PiyushThePal
 Author-email: cool_guy2331708@yahoo.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # mypackage
 
-mypackage is a simple Python package that provides functions to get different sets of characters including uppercase letters, lowercase letters, numbers, and special characters.
+chars is a simple Python package that provides functions to get different sets of characters including uppercase letters, lowercase letters, numbers, and special characters.
+
+## Features
+
+- Retrieve uppercase letters
+- Retrieve lowercase letters
+- Retrieve numbers
+- Retrieve special characters
+- Retrieve a combination of all character sets
+
+## Installation
+
+You can install the package using `pip`:
+
+```sh
+pip install chars
+```
+END
```

### Comparing `chars-0.1.0/setup.py` & `chars-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chars',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     description='A package for character sets',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='PiyushThePal',
     author_email='cool_guy2331708@yahoo.com',
     # url='https://github.com/yourusername/mypackage',
```

### Comparing `chars-0.1.0/tests/test_charset.py` & `chars-0.1.1/tests/test_charset.py`

 * *Files identical despite different names*

