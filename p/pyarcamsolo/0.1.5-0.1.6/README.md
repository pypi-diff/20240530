# Comparing `tmp/pyarcamsolo-0.1.5.tar.gz` & `tmp/pyarcamsolo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcamsolo-0.1.5.tar", last modified: Mon May 27 20:57:38 2024, max compression
+gzip compressed data, was "pyarcamsolo-0.1.6.tar", last modified: Wed May 29 22:08:10 2024, max compression
```

## Comparing `pyarcamsolo-0.1.5.tar` & `pyarcamsolo-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:57:38.367414 pyarcamsolo-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 20:57:38.367414 pyarcamsolo-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:57:38.367414 pyarcamsolo-0.1.5/pyarcamsolo/
--rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/pyarcamsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/pyarcamsolo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/pyarcamsolo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/pyarcamsolo/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/pyarcamsolo/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/pyarcamsolo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:57:38.367414 pyarcamsolo-0.1.5/pyarcamsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-27 20:57:38.000000 pyarcamsolo-0.1.5/pyarcamsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-27 20:57:38.000000 pyarcamsolo-0.1.5/pyarcamsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:57:38.000000 pyarcamsolo-0.1.5/pyarcamsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 20:57:38.000000 pyarcamsolo-0.1.5/pyarcamsolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 20:57:38.000000 pyarcamsolo-0.1.5/pyarcamsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 20:57:38.000000 pyarcamsolo-0.1.5/pyarcamsolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:57:38.367414 pyarcamsolo-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-27 20:57:14.000000 pyarcamsolo-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:08:10.659237 pyarcamsolo-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-29 22:08:10.659237 pyarcamsolo-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:08:10.659237 pyarcamsolo-0.1.6/pyarcamsolo/
+-rw-r--r--   0 runner    (1001) docker     (127)    24026 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/pyarcamsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/pyarcamsolo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/pyarcamsolo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/pyarcamsolo/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/pyarcamsolo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/pyarcamsolo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:08:10.659237 pyarcamsolo-0.1.6/pyarcamsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-29 22:08:10.000000 pyarcamsolo-0.1.6/pyarcamsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:08:10.000000 pyarcamsolo-0.1.6/pyarcamsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:08:10.000000 pyarcamsolo-0.1.6/pyarcamsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 22:08:10.000000 pyarcamsolo-0.1.6/pyarcamsolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-29 22:08:10.000000 pyarcamsolo-0.1.6/pyarcamsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 22:08:10.000000 pyarcamsolo-0.1.6/pyarcamsolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:08:10.659237 pyarcamsolo-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-29 22:07:45.000000 pyarcamsolo-0.1.6/setup.py
```

### Comparing `pyarcamsolo-0.1.5/LICENSE` & `pyarcamsolo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.5/PKG-INFO` & `pyarcamsolo-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.5/README.md` & `pyarcamsolo-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.5/pyarcamsolo/__init__.py` & `pyarcamsolo-0.1.6/pyarcamsolo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,18 +325,18 @@
             self._full_update = True # always perform a full update on schedule
             self._updater_task = asyncio.create_task(self._updater())
 
     async def connect(self, reconnect=True):
         """Open a connection to the Hi-Fi and start listener thread."""
         _LOGGER.debug(">> ArcamSolo.connect() started")
         if self._connect_lock.locked():
-            _LOGGER.warning("Connection is already in progress, skipping connect.")
+            _LOGGER.debug("Connection is already in progress, skipping connect.")
             return
         if self.available:
-            _LOGGER.warning("Device is connected, skipping connection.")
+            _LOGGER.debug("Device is connected, skipping connection.")
             return
 
         async with self._connect_lock:
             _LOGGER.debug("Opening Arcam connection.")
             if self._writer is not None:
                 raise RuntimeError("Device already connected.")
 
@@ -363,20 +363,20 @@
         _LOGGER.debug(">> ArcamSolo.connect() completed")
 
     async def disconnect(self):
         """Shutdown and close telnet connection to Arcam."""
         _LOGGER.debug(">> ArcamSolo.disconnect() started")
 
         if self._disconnect_lock.locked():
-            _LOGGER.warning(
+            _LOGGER.debug(
                 "Arcam connection is already disconnecting, skipping disconnect"
             )
             return
         if not self.available:
-            _LOGGER.warning("Arcam not connected, skipping disconnect")
+            _LOGGER.debug("Arcam not connected, skipping disconnect")
             return
 
         async with self._disconnect_lock:
             _LOGGER.debug("disconnecting Arcam connection")
             self.available = False
             for zone in self.zones:
                 self._call_zone_callbacks(zone)
@@ -448,16 +448,14 @@
                 await asyncio.sleep(0)  # yield to reconnect task if running
                 if reconnect_task.done():
                     reconnect_task = None  # trigger new task creation
             if reconnect_task is None:
                 _LOGGER.info("reconnecting to ArcamSolo")
                 reconnect_task = asyncio.create_task(self.reconnect())
                 self._reconnect_task = reconnect_task
-            else:
-                _LOGGER.error("ArcamSolo listener reconnection already running")
 
     async def _reconnect_cancel(self):
         """Cancel any active reconnect task."""
         await cancel_task(self._reconnect_task, "reconnect")
         self._reconnect_task = None
 
     # Reader co-routine
```

### Comparing `pyarcamsolo-0.1.5/pyarcamsolo/commands.py` & `pyarcamsolo-0.1.6/pyarcamsolo/commands.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.5/pyarcamsolo/parser.py` & `pyarcamsolo-0.1.6/pyarcamsolo/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     data = response[5:(5+size)] # Sixth byte+ is data
 
     cc = get_command_code(cc)
     ac = get_answer_code(ac)
     # check answer code is valid
     if ac not in ACCEPTED_ANSWER_CODES:
         if ac == "command_invalid_at_this_time":
-            _LOGGER.warning("Command %s is unavailable in current state. Will retry later.", cc)
+            _LOGGER.debug("Command %s is unavailable in current state. Will retry later.", cc)
             return None
         raise ValueError(
             f"Provided response for {cc} is invalid at this time: {get_answer_code(ac)}"
         )
     _LOGGER.debug(">> Decoded response as command %s", cc)
 
     if cc == "volume":
```

### Comparing `pyarcamsolo-0.1.5/pyarcamsolo/util.py` & `pyarcamsolo-0.1.6/pyarcamsolo/util.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.1.5/pyarcamsolo.egg-info/PKG-INFO` & `pyarcamsolo-0.1.6/pyarcamsolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.1.5
+Version: 0.1.6
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.1.5/setup.py` & `pyarcamsolo-0.1.6/setup.py`

 * *Files identical despite different names*

