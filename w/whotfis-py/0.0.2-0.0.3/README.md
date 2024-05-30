# Comparing `tmp/whotfis_py-0.0.2.tar.gz` & `tmp/whotfis_py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whotfis_py-0.0.2.tar", last modified: Thu May 30 19:19:07 2024, max compression
+gzip compressed data, was "whotfis_py-0.0.3.tar", last modified: Thu May 30 19:22:43 2024, max compression
```

## Comparing `whotfis_py-0.0.2.tar` & `whotfis_py-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:19:07.313479 whotfis_py-0.0.2/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.2/LICENSE
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:19:07.313269 whotfis_py-0.0.2/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       67 2024-05-30 18:44:34.000000 whotfis_py-0.0.2/README.md
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-30 19:19:07.313514 whotfis_py-0.0.2/setup.cfg
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      766 2024-05-30 19:18:46.000000 whotfis_py-0.0.2/setup.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:19:07.312589 whotfis_py-0.0.2/whotfis-py/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      631 2024-05-30 18:52:25.000000 whotfis_py-0.0.2/whotfis-py/__init__.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2412 2024-05-30 18:33:09.000000 whotfis_py-0.0.2/whotfis-py/parser.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1639 2024-05-30 18:19:52.000000 whotfis_py-0.0.2/whotfis-py/registries.py
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4108 2024-05-30 18:14:07.000000 whotfis_py-0.0.2/whotfis-py/result.py
-drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:19:07.313119 whotfis_py-0.0.2/whotfis_py.egg-info/
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/PKG-INFO
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      252 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/SOURCES.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/dependency_links.txt
--rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-30 19:19:07.000000 whotfis_py-0.0.2/whotfis_py.egg-info/top_level.txt
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:22:43.316008 whotfis_py-0.0.3/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)    11357 2024-05-30 18:44:34.000000 whotfis_py-0.0.3/LICENSE
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       68 2024-05-30 19:22:27.000000 whotfis_py-0.0.3/MANIFEST.in
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:22:43.315797 whotfis_py-0.0.3/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       67 2024-05-30 18:44:34.000000 whotfis_py-0.0.3/README.md
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       38 2024-05-30 19:22:43.316047 whotfis_py-0.0.3/setup.cfg
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      766 2024-05-30 19:22:41.000000 whotfis_py-0.0.3/setup.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:22:43.314892 whotfis_py-0.0.3/whotfis-py/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      631 2024-05-30 18:52:25.000000 whotfis_py-0.0.3/whotfis-py/__init__.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     2412 2024-05-30 18:33:09.000000 whotfis_py-0.0.3/whotfis-py/parser.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     1639 2024-05-30 18:19:52.000000 whotfis_py-0.0.3/whotfis-py/registries.py
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)     4108 2024-05-30 18:14:07.000000 whotfis_py-0.0.3/whotfis-py/result.py
+drwxr-xr-x   0 valeriopiodenicola   (501) staff       (20)        0 2024-05-30 19:22:43.315596 whotfis_py-0.0.3/whotfis_py.egg-info/
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      639 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/PKG-INFO
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)      264 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/SOURCES.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)        1 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/dependency_links.txt
+-rw-r--r--   0 valeriopiodenicola   (501) staff       (20)       11 2024-05-30 19:22:43.000000 whotfis_py-0.0.3/whotfis_py.egg-info/top_level.txt
```

### Comparing `whotfis_py-0.0.2/LICENSE` & `whotfis_py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.2/PKG-INFO` & `whotfis_py-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple package to interact with the whois command line tool
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `whotfis_py-0.0.2/setup.py` & `whotfis_py-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = "Simple package to interact with the whois command line tool"
 
 setup(
     name="whotfis-py",
     version=VERSION,
     author="Valerio Pio De Nicola",
     author_email="valeriopio02@gmail.com",
```

### Comparing `whotfis_py-0.0.2/whotfis-py/__init__.py` & `whotfis_py-0.0.3/whotfis-py/__init__.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.2/whotfis-py/parser.py` & `whotfis_py-0.0.3/whotfis-py/parser.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.2/whotfis-py/registries.py` & `whotfis_py-0.0.3/whotfis-py/registries.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.2/whotfis-py/result.py` & `whotfis_py-0.0.3/whotfis-py/result.py`

 * *Files identical despite different names*

### Comparing `whotfis_py-0.0.2/whotfis_py.egg-info/PKG-INFO` & `whotfis_py-0.0.3/whotfis_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whotfis-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple package to interact with the whois command line tool
 Author: Valerio Pio De Nicola
 Author-email: valeriopio02@gmail.com
 Keywords: python,whois,whois command line,whois python,whois python package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

