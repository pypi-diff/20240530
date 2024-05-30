# Comparing `tmp/whotfis_py-0.0.1.tar.gz` & `tmp/whotfis_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whotfis_py-0.0.1.tar", last modified: Thu May 30 18:55:09 2024, max compression
+gzip compressed data, was "whotfis_py-0.0.2.tar", last modified: Thu May 30 19:19:07 2024, max compression
```

## Comparing `whotfis_py-0.0.1.tar` & `whotfis_py-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 18:55:09.995073 whotfis_py-0.0.1/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      545 2024-05-30 18:55:09.994900 whotfis_py-0.0.1/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       62 2024-05-30 17:14:37.000000 whotfis_py-0.0.1/README.md
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-30 18:55:09.995118 whotfis_py-0.0.1/setup.cfg
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      810 2024-05-30 14:16:39.000000 whotfis_py-0.0.1/setup.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 18:55:09.994718 whotfis_py-0.0.1/whotfis_py.egg-info/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      545 2024-05-30 18:55:09.000000 whotfis_py-0.0.1/whotfis_py.egg-info/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      154 2024-05-30 18:55:09.000000 whotfis_py-0.0.1/whotfis_py.egg-info/SOURCES.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 18:55:09.000000 whotfis_py-0.0.1/whotfis_py.egg-info/dependency_links.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 18:55:09.000000 whotfis_py-0.0.1/whotfis_py.egg-info/top_level.txt
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:19:07.313479 whotfis_py-0.0.2/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.2/LICENSE
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:19:07.313269 whotfis_py-0.0.2/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       67 2024-05-30 18:44:34.000000 whotfis_py-0.0.2/README.md
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-30 19:19:07.313514 whotfis_py-0.0.2/setup.cfg
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      766 2024-05-30 19:18:46.000000 whotfis_py-0.0.2/setup.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:19:07.312589 whotfis_py-0.0.2/whotfis-py/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      631 2024-05-30 18:52:25.000000 whotfis_py-0.0.2/whotfis-py/__init__.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2412 2024-05-30 18:33:09.000000 whotfis_py-0.0.2/whotfis-py/parser.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1639 2024-05-30 18:19:52.000000 whotfis_py-0.0.2/whotfis-py/registries.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4108 2024-05-30 18:14:07.000000 whotfis_py-0.0.2/whotfis-py/result.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:19:07.313119 whotfis_py-0.0.2/whotfis_py.egg-info/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      252 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/SOURCES.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/dependency_links.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/top_level.txt
```

### Comparing `whotfis_py-0.0.1/PKG-INFO` & `whotfis_py-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple package to interact with the whois command line tool
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Installation
+To install the package, just run the following command:
+```bash
+pip install whotfis-py
+```
+# Usage
+```python
 
-A simple package to interact with the whois command line tool without losing time in parsing
```

### Comparing `whotfis_py-0.0.1/setup.py` & `whotfis_py-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = "Simple package to interact with the whois command line tool"
-LONG_DESCRIPTION = "A simple package to interact with the whois command line tool without losing time in parsing"
 
 setup(
     name="whotfis-py",
     version=VERSION,
     author="Valerio Pio De Nicola",
     author_email="valeriopio02@gmail.com",
     description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
+    long_description=open('whotfis-py/README.md').read(),
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'whois', 'whois command line', 'whois python', 'whois python package'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

### Comparing `whotfis_py-0.0.1/whotfis_py.egg-info/PKG-INFO` & `whotfis_py-0.0.2/whotfis_py.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple package to interact with the whois command line tool
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Installation
+To install the package, just run the following command:
+```bash
+pip install whotfis-py
+```
+# Usage
+```python
 
-A simple package to interact with the whois command line tool without losing time in parsing
```

