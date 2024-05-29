# Comparing `tmp/abstract_factories-0.2.4.tar.gz` & `tmp/abstract_factories-0.2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_factories-0.2.4.tar", last modified: Wed May 29 21:22:04 2024, max compression
+gzip compressed data, was "abstract_factories-0.2.41.tar", last modified: Wed May 29 21:42:18 2024, max compression
```

## Comparing `abstract_factories-0.2.4.tar` & `abstract_factories-0.2.41.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:22:04.969854 abstract_factories-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-29 21:22:04.969854 abstract_factories-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-29 21:22:01.000000 abstract_factories-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:22:04.969854 abstract_factories-0.2.4/abstract_factories/
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-29 21:22:01.000000 abstract_factories-0.2.4/abstract_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 21:22:01.000000 abstract_factories-0.2.4/abstract_factories/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-29 21:22:01.000000 abstract_factories-0.2.4/abstract_factories/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-29 21:22:01.000000 abstract_factories-0.2.4/abstract_factories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:22:04.969854 abstract_factories-0.2.4/abstract_factories.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-29 21:22:04.000000 abstract_factories-0.2.4/abstract_factories.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-29 21:22:04.000000 abstract_factories-0.2.4/abstract_factories.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:22:04.000000 abstract_factories-0.2.4/abstract_factories.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 21:22:04.000000 abstract_factories-0.2.4/abstract_factories.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 21:22:04.969854 abstract_factories-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-29 21:22:01.000000 abstract_factories-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:22:04.969854 abstract_factories-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-29 21:22:01.000000 abstract_factories-0.2.4/tests/test_abstract_factories_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:42:18.414432 abstract_factories-0.2.41/
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-29 21:42:18.414432 abstract_factories-0.2.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-29 21:42:14.000000 abstract_factories-0.2.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:42:18.414432 abstract_factories-0.2.41/abstract_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-29 21:42:14.000000 abstract_factories-0.2.41/abstract_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 21:42:14.000000 abstract_factories-0.2.41/abstract_factories/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-29 21:42:14.000000 abstract_factories-0.2.41/abstract_factories/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-29 21:42:14.000000 abstract_factories-0.2.41/abstract_factories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:42:18.414432 abstract_factories-0.2.41/abstract_factories.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-29 21:42:18.000000 abstract_factories-0.2.41/abstract_factories.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-29 21:42:18.000000 abstract_factories-0.2.41/abstract_factories.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:42:18.000000 abstract_factories-0.2.41/abstract_factories.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 21:42:18.000000 abstract_factories-0.2.41/abstract_factories.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 21:42:18.414432 abstract_factories-0.2.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-29 21:42:14.000000 abstract_factories-0.2.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:42:18.414432 abstract_factories-0.2.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-29 21:42:14.000000 abstract_factories-0.2.41/tests/test_abstract_factories_items.py
```

### Comparing `abstract_factories-0.2.4/PKG-INFO` & `abstract_factories-0.2.41/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_factories
-Version: 0.2.4
+Version: 0.2.41
 Summary: Abstract Factory design pattern classes for scalable data in dynamic environments.
 Home-page: https://github.com/ldunham1/abstract_factories
 Author: Lee Dunham
 Author-email: leedunham@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,17 @@
   > fragile or large to update.
   > Providing there's no functional or notable impact 
   > supporting 2.7, I have no reason to ignore its existence _yet_.
 
 ---
 
 ## Installation
-Clone the project locally.
+```bash
+pip install abstract-factories
+```
 
 ---
 
 ## Usage
 Initialize AbstractTypeFactory or AbstractInstanceFactory with the abstract type.  
 Optionally, provide the attribute/method name to identify items by name (and optionally version).
 ```python
```

### Comparing `abstract_factories-0.2.4/README.md` & `abstract_factories-0.2.41/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
   > fragile or large to update.
   > Providing there's no functional or notable impact 
   > supporting 2.7, I have no reason to ignore its existence _yet_.
 
 ---
 
 ## Installation
-Clone the project locally.
+```bash
+pip install abstract-factories
+```
 
 ---
 
 ## Usage
 Initialize AbstractTypeFactory or AbstractInstanceFactory with the abstract type.  
 Optionally, provide the attribute/method name to identify items by name (and optionally version).
 ```python
```

### Comparing `abstract_factories-0.2.4/abstract_factories/__init__.py` & `abstract_factories-0.2.41/abstract_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `abstract_factories-0.2.4/abstract_factories/core.py` & `abstract_factories-0.2.41/abstract_factories/core.py`

 * *Files identical despite different names*

### Comparing `abstract_factories-0.2.4/abstract_factories/utils.py` & `abstract_factories-0.2.41/abstract_factories/utils.py`

 * *Files identical despite different names*

### Comparing `abstract_factories-0.2.4/abstract_factories.egg-info/PKG-INFO` & `abstract_factories-0.2.41/abstract_factories.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_factories
-Version: 0.2.4
+Version: 0.2.41
 Summary: Abstract Factory design pattern classes for scalable data in dynamic environments.
 Home-page: https://github.com/ldunham1/abstract_factories
 Author: Lee Dunham
 Author-email: leedunham@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,17 @@
   > fragile or large to update.
   > Providing there's no functional or notable impact 
   > supporting 2.7, I have no reason to ignore its existence _yet_.
 
 ---
 
 ## Installation
-Clone the project locally.
+```bash
+pip install abstract-factories
+```
 
 ---
 
 ## Usage
 Initialize AbstractTypeFactory or AbstractInstanceFactory with the abstract type.  
 Optionally, provide the attribute/method name to identify items by name (and optionally version).
 ```python
```

### Comparing `abstract_factories-0.2.4/setup.py` & `abstract_factories-0.2.41/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 
 setup(
     name='abstract_factories',
     packages=['abstract_factories'],
-    version='0.2.4',
+    version='0.2.41',
     license='MIT',
     description='Abstract Factory design pattern classes for scalable data in dynamic environments.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Lee Dunham',
     author_email='leedunham@gmail.com',
     url='https://github.com/ldunham1/abstract_factories',
```

### Comparing `abstract_factories-0.2.4/tests/test_abstract_factories_items.py` & `abstract_factories-0.2.41/tests/test_abstract_factories_items.py`

 * *Files identical despite different names*

