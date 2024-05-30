# Comparing `tmp/pinecone_plugin_interface-0.0.5.tar.gz` & `tmp/pinecone_plugin_interface-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_plugin_interface-0.0.5.tar", max compression
+gzip compressed data, was "pinecone_plugin_interface-0.0.6.tar", max compression
```

## Comparing `pinecone_plugin_interface-0.0.5.tar` & `pinecone_plugin_interface-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      356 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/README.md
--rw-r--r--   0        0        0      729 2024-05-29 14:05:56.761092 pinecone_plugin_interface-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/__init__.py
--rw-r--r--   0        0        0      197 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/__init__.py
--rw-r--r--   0        0        0       38 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/constants.py
--rw-r--r--   0        0        0      571 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/discover_namespace_packages.py
--rw-r--r--   0        0        0     1338 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/discover_plugins.py
--rw-r--r--   0        0        0     1543 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/installation.py
--rw-r--r--   0        0        0      428 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/load_and_install.py
--rw-r--r--   0        0        0       52 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/logging.py
--rw-r--r--   0        0        0      467 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/pinecone_plugin.py
--rw-r--r--   0        0        0     2769 2024-05-29 14:05:41.036963 pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/plugin_metadata.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 pinecone_plugin_interface-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      356 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/README.md
+-rw-r--r--   0        0        0      729 2024-05-30 19:33:00.488762 pinecone_plugin_interface-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/constants.py
+-rw-r--r--   0        0        0      571 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/discover_namespace_packages.py
+-rw-r--r--   0        0        0     1338 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/discover_plugins.py
+-rw-r--r--   0        0        0      984 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/installation.py
+-rw-r--r--   0        0        0      428 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/load_and_install.py
+-rw-r--r--   0        0        0       52 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/logging.py
+-rw-r--r--   0        0        0      467 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/pinecone_plugin.py
+-rw-r--r--   0        0        0     1513 2024-05-30 19:32:45.628815 pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/plugin_metadata.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 pinecone_plugin_interface-0.0.6/PKG-INFO
```

### Comparing `pinecone_plugin_interface-0.0.5/pyproject.toml` & `pinecone_plugin_interface-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinecone-plugin-interface"
-version = "0.0.5"
+version = "0.0.6"
 packages = [
     { include="pinecone_plugin_interface", from="src" },
 ]
 description = "Plugin interface for the Pinecone python client"
 authors = ["Pinecone Systems, Inc. <support@pinecone.io>"]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/discover_namespace_packages.py` & `pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/discover_namespace_packages.py`

 * *Files identical despite different names*

### Comparing `pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/actions/discover_plugins.py` & `pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/actions/discover_plugins.py`

 * *Files identical despite different names*

### Comparing `pinecone_plugin_interface-0.0.5/src/pinecone_plugin_interface/plugin_metadata.py` & `pinecone_plugin_interface-0.0.6/src/pinecone_plugin_interface/plugin_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,37 +43,8 @@
     """
 
     implementation_class: Type[PineconePlugin[T, C]]
     """
     This should be a class extending the PineconePlugin abstract base class. This class should expose
     various feature methods with UX in mind, since it's the surface end-users will
     interact with. Often it will be a wrapper around a generated OpenAPI client object.
-    """
-
-    api_version: str
-    """
-    This value will be used to set an appropriate X-Pinecone-API-Version header on
-    the plugin's requests. It will only be used when installing plugins that 
-    include the openapi_client_class attribute. 
-    
-    If you are not building around an OpenAPI generated client class, you can leave this as an 
-    empty string and it will be your responsibility to make sure an appropriate 
-    version header is sent with every request.
-    """
-
-    openapi_api_client_class: type
-    """
-    A reference to the generated ApiClient object used by your plugin. This is used to
-    configure the client with the appropriate base URL and API key. If you are not using
-    an OpenAPI client, you can leave this as None.
-    """
-
-    openapi_api_class: type
-    """
-    If the plugin is built on top of a generated OpenAPI client class, this should be the
-    OpenAPI client class that the plugin uses. If you are not using an OpenAPI client,
-    you can leave this as None.
-
-    Providing this value allows us to automatically instantiate and configure all openapi client
-    objects in a consistent way across the entire SDK so that you get the benefit of features like
-    proxy configuration for free in your plugin.
     """
```

### Comparing `pinecone_plugin_interface-0.0.5/PKG-INFO` & `pinecone_plugin_interface-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinecone-plugin-interface
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plugin interface for the Pinecone python client
 Home-page: https://www.pinecone.io
 License: Apache-2.0
 Author: Pinecone Systems, Inc.
 Author-email: support@pinecone.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

