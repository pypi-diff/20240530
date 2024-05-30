# Comparing `tmp/trace_attributes-4.0.2.tar.gz` & `tmp/trace_attributes-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace_attributes-4.0.2.tar", last modified: Tue May 28 11:00:00 2024, max compression
+gzip compressed data, was "trace_attributes-4.0.3.tar", last modified: Wed May 29 13:57:48 2024, max compression
```

## Comparing `trace_attributes-4.0.2.tar` & `trace_attributes-4.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.222292 trace_attributes-4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.222292 trace_attributes-4.0.2/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/langtrace/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/database_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:57:48.987908 trace_attributes-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-29 13:57:48.987908 trace_attributes-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:57:48.987908 trace_attributes-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:57:48.983907 trace_attributes-4.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:57:48.983907 trace_attributes-4.0.3/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:57:48.983907 trace_attributes-4.0.3/src/python/langtrace/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/src/python/langtrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:57:48.983907 trace_attributes-4.0.3/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:57:48.983907 trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/database_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-29 13:57:36.000000 trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:57:48.987908 trace_attributes-4.0.3/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-29 13:57:48.000000 trace_attributes-4.0.3/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 13:57:48.000000 trace_attributes-4.0.3/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:57:48.000000 trace_attributes-4.0.3/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 13:57:48.000000 trace_attributes-4.0.3/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 13:57:48.000000 trace_attributes-4.0.3/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace_attributes-4.0.2/LICENSE` & `trace_attributes-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.2/PKG-INFO` & `trace_attributes-4.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 4.0.2
+Version: 4.0.3
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=1.8
-Requires-Dist: typing
 
 LangTrace - Trace Attributes
```

### Comparing `trace_attributes-4.0.2/README.md` & `trace_attributes-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.2/setup.py` & `trace_attributes-4.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='4.0.2',
+    version='4.0.3',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
     packages=find_packages(where='src/python'),
     install_requires=[
         'pydantic>=1.8',  # Example dependency, adjust according to your project's needs
-        'typing'
     ],
     python_requires='>=3.6',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

### Comparing `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/__init__.py` & `trace_attributes-4.0.3/src/python/langtrace/trace_attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/database_span_attributes.py` & `trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/database_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/framework_span_attributes.py` & `trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/framework_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/llm_span_attributes.py` & `trace_attributes-4.0.3/src/python/langtrace/trace_attributes/models/llm_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.2/src/python/trace_attributes.egg-info/PKG-INFO` & `trace_attributes-4.0.3/src/python/trace_attributes.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 4.0.2
+Version: 4.0.3
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>=1.8
-Requires-Dist: typing
 
 LangTrace - Trace Attributes
```

### Comparing `trace_attributes-4.0.2/src/python/trace_attributes.egg-info/SOURCES.txt` & `trace_attributes-4.0.3/src/python/trace_attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

