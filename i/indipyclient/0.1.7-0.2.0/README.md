# Comparing `tmp/indipyclient-0.1.7.tar.gz` & `tmp/indipyclient-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.1.7.tar` & `indipyclient-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.7/LICENSE
--rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.7/README.md
--rw-r--r--   0        0        0      332 2024-05-27 15:52:53.000000 indipyclient-0.1.7/indipyclient/__init__.py
--rw-r--r--   0        0        0     4801 2024-05-24 10:02:09.000000 indipyclient-0.1.7/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.7/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19750 2024-05-24 09:23:15.000000 indipyclient-0.1.7/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.7/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.7/indipyclient/console/windows.py
--rw-r--r--   0        0        0    27266 2024-05-22 18:24:53.000000 indipyclient-0.1.7/indipyclient/events.py
--rw-r--r--   0        0        0    34831 2024-05-27 14:52:06.000000 indipyclient-0.1.7/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16339 2024-05-15 11:03:42.000000 indipyclient-0.1.7/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27619 2024-05-27 11:57:25.000000 indipyclient-0.1.7/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-05-27 15:52:41.000000 indipyclient-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.2.0/README.md
+-rw-r--r--   0        0        0      332 2024-05-30 16:39:42.000000 indipyclient-0.2.0/indipyclient/__init__.py
+-rw-r--r--   0        0        0     4801 2024-05-24 10:02:09.000000 indipyclient-0.2.0/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.2.0/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19750 2024-05-24 09:23:15.000000 indipyclient-0.2.0/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.2.0/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.2.0/indipyclient/console/windows.py
+-rw-r--r--   0        0        0    27266 2024-05-22 18:24:53.000000 indipyclient-0.2.0/indipyclient/events.py
+-rw-r--r--   0        0        0    34959 2024-05-30 16:25:36.000000 indipyclient-0.2.0/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16339 2024-05-15 11:03:42.000000 indipyclient-0.2.0/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27619 2024-05-27 11:57:25.000000 indipyclient-0.2.0/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-30 16:39:20.000000 indipyclient-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.2.0/PKG-INFO
```

### Comparing `indipyclient-0.1.7/LICENSE` & `indipyclient-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/README.md` & `indipyclient-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/indipyclient/__main__.py` & `indipyclient-0.2.0/indipyclient/__main__.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/indipyclient/console/consoleclient.py` & `indipyclient-0.2.0/indipyclient/console/consoleclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/indipyclient/console/widgets.py` & `indipyclient-0.2.0/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/indipyclient/console/windows.py` & `indipyclient-0.2.0/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/indipyclient/events.py` & `indipyclient-0.2.0/indipyclient/events.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/indipyclient/ipyclient.py` & `indipyclient-0.2.0/indipyclient/ipyclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,17 @@
            1 for transmitted/received vector tags only,
            2 for transmitted/received vectors, members and contents (apart from BLOBs)
            3 for all transmitted/received data including BLOBs."""
         if verbose not in (0,1,2,3):
             raise ValueError
         self._verbose = verbose
 
+    async def hardware(self):
+        """Override this to operate any required client hardware"""
+        pass
 
     def shutdown(self):
         "Shuts down the client"
         self._stop = True
 
     def report(self, message):
         """If logging is enabled message will be logged at level INFO.
@@ -739,15 +742,15 @@
            event is an object with attributes according to the data received."""
         pass
 
 
     async def asyncrun(self):
         "Await this method to run the client."
         self._stop = False
-        await asyncio.gather(self._comms(), self._rxhandler(), self._timeout_monitor())
+        await asyncio.gather(self._comms(), self._rxhandler(), self._timeout_monitor(), self.hardware())
         self.stopped = True
 
 
 class Device(collections.UserDict):
 
     "Each device is a mapping of vector name to vector object."
```

### Comparing `indipyclient-0.1.7/indipyclient/propertymembers.py` & `indipyclient-0.2.0/indipyclient/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/indipyclient/propertyvectors.py` & `indipyclient-0.2.0/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.7/pyproject.toml` & `indipyclient-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.1.7"
+version = "0.2.0"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.1.7/PKG-INFO` & `indipyclient-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.1.7
+Version: 0.2.0
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

