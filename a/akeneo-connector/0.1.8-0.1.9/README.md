# Comparing `tmp/akeneo_connector-0.1.8.tar.gz` & `tmp/akeneo_connector-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akeneo_connector-0.1.8.tar", last modified: Wed Apr 10 13:33:06 2024, max compression
+gzip compressed data, was "akeneo_connector-0.1.9.tar", last modified: Wed Apr 10 14:07:47 2024, max compression
```

## Comparing `akeneo_connector-0.1.8.tar` & `akeneo_connector-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:06.423563 akeneo_connector-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-10 13:32:57.000000 akeneo_connector-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-10 13:33:06.419563 akeneo_connector-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-10 13:32:57.000000 akeneo_connector-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:06.419563 akeneo_connector-0.1.8/akeneo_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 13:32:57.000000 akeneo_connector-0.1.8/akeneo_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-10 13:32:57.000000 akeneo_connector-0.1.8/akeneo_connector/akeneo_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-10 13:32:57.000000 akeneo_connector-0.1.8/akeneo_connector/akeneo_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-10 13:32:57.000000 akeneo_connector-0.1.8/akeneo_connector/akeneo_product.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:33:06.419563 akeneo_connector-0.1.8/akeneo_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-10 13:33:06.000000 akeneo_connector-0.1.8/akeneo_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 13:33:06.000000 akeneo_connector-0.1.8/akeneo_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:33:06.000000 akeneo_connector-0.1.8/akeneo_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:33:06.000000 akeneo_connector-0.1.8/akeneo_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 13:33:06.000000 akeneo_connector-0.1.8/akeneo_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:33:06.423563 akeneo_connector-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-10 13:33:03.000000 akeneo_connector-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:07:47.473049 akeneo_connector-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-10 14:07:40.000000 akeneo_connector-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-10 14:07:47.473049 akeneo_connector-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-10 14:07:40.000000 akeneo_connector-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:07:47.473049 akeneo_connector-0.1.9/akeneo_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 14:07:40.000000 akeneo_connector-0.1.9/akeneo_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-10 14:07:40.000000 akeneo_connector-0.1.9/akeneo_connector/akeneo_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-10 14:07:40.000000 akeneo_connector-0.1.9/akeneo_connector/akeneo_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-10 14:07:40.000000 akeneo_connector-0.1.9/akeneo_connector/akeneo_product.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:07:47.473049 akeneo_connector-0.1.9/akeneo_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-10 14:07:47.000000 akeneo_connector-0.1.9/akeneo_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 14:07:47.000000 akeneo_connector-0.1.9/akeneo_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:07:47.000000 akeneo_connector-0.1.9/akeneo_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:07:47.000000 akeneo_connector-0.1.9/akeneo_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 14:07:47.000000 akeneo_connector-0.1.9/akeneo_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:07:47.473049 akeneo_connector-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-10 14:07:44.000000 akeneo_connector-0.1.9/setup.py
```

### Comparing `akeneo_connector-0.1.8/LICENSE` & `akeneo_connector-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.8/PKG-INFO` & `akeneo_connector-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.8
+Version: 0.1.9
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.8/README.md` & `akeneo_connector-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.8/akeneo_connector/akeneo_connector.py` & `akeneo_connector-0.1.9/akeneo_connector/akeneo_connector.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.8/akeneo_connector/akeneo_paginator.py` & `akeneo_connector-0.1.9/akeneo_connector/akeneo_paginator.py`

 * *Files identical despite different names*

### Comparing `akeneo_connector-0.1.8/akeneo_connector/akeneo_product.py` & `akeneo_connector-0.1.9/akeneo_connector/akeneo_product.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,37 +115,41 @@
             attribute (str): The attribute to get the values for.
 
         Returns:
             list: The values of the attribute.
         """
         return self.values.get(attribute, [])
     
-    def get_value(self, attribute: str, locale: str | None = None, scope: str | None = None) -> Value:
+    def get_value(self, attribute: str, locale: str | None = None, scope: str | None = None) -> any:
         """
         Gets the value for the given attribute.
 
         Args:
             attribute (str): The attribute to get the value for.
             locale (str): The locale of the value.
             scope (str): The scope of the value.
 
         Returns:
-            str: The value of the attribute.
+            str: The value of the attribute. None if not found.
         """
         # Failsafe
         if attribute not in self.values:
             return None
 
         # Try to find the value with locale and scope
         for value in self.values[attribute]:
             if value.get('locale') == locale and value.get('scope') == scope:
                 return value.get('data')
 
-        # Return the first value if locale and scope are not found
-        return self.values[attribute][0].get('data')
+        # Return first value if locale is None and scope is None
+        if locale is None and scope is None:
+            return self.values[attribute][0].get('data')
+        
+        # Return None if locale and scope are not found
+        return None
     
 
     def set_value(self, attribute: str, locale: str | None = None, scope: str | None = None, data: str | None = None):
         """
         Sets a value for the given attribute.
 
         Args:
```

### Comparing `akeneo_connector-0.1.8/akeneo_connector.egg-info/PKG-INFO` & `akeneo_connector-0.1.9/akeneo_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akeneo_connector
-Version: 0.1.8
+Version: 0.1.9
 Summary: Akeneo Connector is a Python package that simplifies interacting with Akeneo's REST API. It provides classes for making HTTP requests to Akeneo endpoints, handling pagination in responses, and managing product data in Akeneo.
 Home-page: https://github.com/bakeable/akeneo-connector
 Author: Robin Bakker
 Author-email: robin@bakeable.nl
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `akeneo_connector-0.1.8/setup.py` & `akeneo_connector-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="akeneo_connector",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=[
         'requests >= 2.31.0',
         'python-dotenv >= 1.0.1'
     ],
     author="Robin Bakker",
     author_email="robin@bakeable.nl",
```

