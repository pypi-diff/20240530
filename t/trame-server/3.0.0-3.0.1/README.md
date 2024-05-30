# Comparing `tmp/trame-server-3.0.0.tar.gz` & `tmp/trame-server-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-server-3.0.0.tar", last modified: Wed Apr 10 22:56:44 2024, max compression
+gzip compressed data, was "trame-server-3.0.1.tar", last modified: Thu May 30 18:14:59 2024, max compression
```

## Comparing `trame-server-3.0.0.tar` & `trame-server-3.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 22:56:42.000000 trame-server-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 22:56:42.000000 trame-server-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4414 2024-04-10 22:56:44.695624 trame-server-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3681 2024-04-10 22:56:42.000000 trame-server-3.0.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      903 2024-04-10 22:56:44.695624 trame-server-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 22:56:42.000000 trame-server-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/trame_server/
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/LICENSE
--rw-r--r--   0 root         (0) root         (0)      211 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10337 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/client.py
--rw-r--r--   0 root         (0) root         (0)    12544 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/controller.py
--rw-r--r--   0 root         (0) root         (0)    25206 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/core.py
--rw-r--r--   0 root         (0) root         (0)     7658 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/protocol.py
--rw-r--r--   0 root         (0) root         (0)     9229 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/state.py
--rw-r--r--   0 root         (0) root         (0)     1602 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/ui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/trame_server/utils/
--rw-r--r--   0 root         (0) root         (0)     2785 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3075 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/argument_parser.py
--rw-r--r--   0 root         (0) root         (0)     5396 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/browser.py
--rw-r--r--   0 root         (0) root         (0)     4884 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/desktop.py
--rw-r--r--   0 root         (0) root         (0)    10103 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/hot_reload.py
--rw-r--r--   0 root         (0) root         (0)     1966 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     2767 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/namespace.py
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/server.py
--rw-r--r--   0 root         (0) root         (0)      552 2024-04-10 22:56:42.000000 trame-server-3.0.0/trame_server/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:56:44.695624 trame-server-3.0.0/trame_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4414 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-10 22:56:44.000000 trame-server-3.0.0/trame_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:14:59.839369 trame-server-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-30 18:14:56.000000 trame-server-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-30 18:14:56.000000 trame-server-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-05-30 18:14:59.839369 trame-server-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3681 2024-05-30 18:14:56.000000 trame-server-3.0.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      903 2024-05-30 18:14:59.839369 trame-server-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 18:14:56.000000 trame-server-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:14:59.835369 trame-server-3.0.1/trame_server/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      211 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10337 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/client.py
+-rw-r--r--   0 root         (0) root         (0)    12544 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/controller.py
+-rw-r--r--   0 root         (0) root         (0)    25375 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/core.py
+-rw-r--r--   0 root         (0) root         (0)     7929 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     9229 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/state.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/ui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:14:59.839369 trame-server-3.0.1/trame_server/utils/
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/browser.py
+-rw-r--r--   0 root         (0) root         (0)     4884 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/desktop.py
+-rw-r--r--   0 root         (0) root         (0)    10103 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/hot_reload.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/namespace.py
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/server.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-30 18:14:56.000000 trame-server-3.0.1/trame_server/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 18:14:59.839369 trame-server-3.0.1/trame_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-05-30 18:14:59.000000 trame-server-3.0.1/trame_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2024-05-30 18:14:59.000000 trame-server-3.0.1/trame_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 18:14:59.000000 trame-server-3.0.1/trame_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-30 18:14:59.000000 trame-server-3.0.1/trame_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-30 18:14:59.000000 trame-server-3.0.1/trame_server.egg-info/top_level.txt
```

### Comparing `trame-server-3.0.0/LICENSE` & `trame-server-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/PKG-INFO` & `trame-server-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-server
-Version: 3.0.0
+Version: 3.0.1
 Summary: Internal server side implementation of trame
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-server-3.0.0/README.rst` & `trame-server-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/setup.cfg` & `trame-server-3.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-server
-version = 3.0.0
+version = 3.0.1
 description = Internal server side implementation of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-server-3.0.0/trame_server/LICENSE` & `trame-server-3.0.1/trame_server/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/client.py` & `trame-server-3.0.1/trame_server/client.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/controller.py` & `trame-server-3.0.1/trame_server/controller.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/core.py` & `trame-server-3.0.1/trame_server/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,19 @@
         """Return the current server state"""
         state = {
             "name": self._name,
             "state": self.state.initial,
         }
         return state
 
+    def clear_state_client_cache(self, *state_names):
+        protocol = self.protocol
+        if protocol:
+            protocol.clear_state_client_cache(*state_names)
+
     # -------------------------------------------------------------------------
 
     def add_protocol_to_configure(self, configure_protocol_fn):
         """
         Register function that will be called with a wslink.ServerProtocol
         when the server start and is ready for registering new wslink.Protocol.
```

### Comparing `trame-server-3.0.0/trame_server/protocol.py` & `trame-server-3.0.1/trame_server/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,22 @@
     # ---------------------------------------------------------------
 
     def push_actions(self, actions):
         logger.action_s2c(actions)
         self.publish("trame.actions.topic", actions)
 
     # ---------------------------------------------------------------
+    # Internal RPCs
+    # ---------------------------------------------------------------
+
+    def clear_state_client_cache(self, *keys):
+        for k in keys:
+            del self._clients_state[k]
+
+    # ---------------------------------------------------------------
     # RPCs
     # ---------------------------------------------------------------
 
     @exportRpc("trame.force.push")
     def force_push_state(self, *keys):
         state_to_send = {key: self.server.state[key] for key in keys}
         if state_to_send:
```

### Comparing `trame-server-3.0.0/trame_server/state.py` & `trame-server-3.0.1/trame_server/state.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/ui.py` & `trame-server-3.0.1/trame_server/ui.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/__init__.py` & `trame-server-3.0.1/trame_server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/argument_parser.py` & `trame-server-3.0.1/trame_server/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/asynchronous.py` & `trame-server-3.0.1/trame_server/utils/asynchronous.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/desktop.py` & `trame-server-3.0.1/trame_server/utils/desktop.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/hot_reload.py` & `trame-server-3.0.1/trame_server/utils/hot_reload.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/logger.py` & `trame-server-3.0.1/trame_server/utils/logger.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/namespace.py` & `trame-server-3.0.1/trame_server/utils/namespace.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/server.py` & `trame-server-3.0.1/trame_server/utils/server.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server/utils/version.py` & `trame-server-3.0.1/trame_server/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-server-3.0.0/trame_server.egg-info/PKG-INFO` & `trame-server-3.0.1/trame_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-server
-Version: 3.0.0
+Version: 3.0.1
 Summary: Internal server side implementation of trame
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-server-3.0.0/trame_server.egg-info/SOURCES.txt` & `trame-server-3.0.1/trame_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

