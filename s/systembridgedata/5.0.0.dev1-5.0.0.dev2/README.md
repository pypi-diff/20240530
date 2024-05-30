# Comparing `tmp/systembridgedata-5.0.0.dev1.tar.gz` & `tmp/systembridgedata-5.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgedata-5.0.0.dev1.tar", last modified: Wed May 29 22:18:02 2024, max compression
+gzip compressed data, was "systembridgedata-5.0.0.dev2.tar", last modified: Wed May 29 23:29:20 2024, max compression
```

## Comparing `systembridgedata-5.0.0.dev1.tar` & `systembridgedata-5.0.0.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.244769 systembridgedata-5.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:18:02.244769 systembridgedata-5.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/systembridgedata/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/systembridgedata/module/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/media.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/systembridgedata/module/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 22:18:02.000000 systembridgedata-5.0.0.dev1/systembridgedata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:18:02.240769 systembridgedata-5.0.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:17:42.000000 systembridgedata-5.0.0.dev1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:29:20.025738 systembridgedata-5.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 23:29:20.025738 systembridgedata-5.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 23:29:20.025738 systembridgedata-5.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:29:20.021737 systembridgedata-5.0.0.dev2/systembridgedata/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:29:20.025738 systembridgedata-5.0.0.dev2/systembridgedata/module/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/systembridgedata/module/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:29:20.025738 systembridgedata-5.0.0.dev2/systembridgedata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 23:29:19.000000 systembridgedata-5.0.0.dev2/systembridgedata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 23:29:19.000000 systembridgedata-5.0.0.dev2/systembridgedata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 23:29:19.000000 systembridgedata-5.0.0.dev2/systembridgedata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 23:29:19.000000 systembridgedata-5.0.0.dev2/systembridgedata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 23:29:19.000000 systembridgedata-5.0.0.dev2/systembridgedata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 23:29:20.025738 systembridgedata-5.0.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 23:28:52.000000 systembridgedata-5.0.0.dev2/tests/test_version.py
```

### Comparing `systembridgedata-5.0.0.dev1/LICENSE` & `systembridgedata-5.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/PKG-INFO` & `systembridgedata-5.0.0.dev2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgedata
-Version: 5.0.0.dev1
+Version: 5.0.0.dev2
 Summary: System Bridge Data
 Home-page: https://github.com/timmo001/system-bridge-data
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgedata-5.0.0.dev1/pyproject.toml` & `systembridgedata-5.0.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/setup.py` & `systembridgedata-5.0.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata/module/cpu.py` & `systembridgedata-5.0.0.dev2/systembridgedata/module/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata/module/disks.py` & `systembridgedata-5.0.0.dev2/systembridgedata/module/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata/module/media.py` & `systembridgedata-5.0.0.dev2/systembridgedata/module/media.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata/module/networks.py` & `systembridgedata-5.0.0.dev2/systembridgedata/module/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata/module/processes.py` & `systembridgedata-5.0.0.dev2/systembridgedata/module/processes.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata/module/sensors.py` & `systembridgedata-5.0.0.dev2/systembridgedata/module/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata/module/system.py` & `systembridgedata-5.0.0.dev2/systembridgedata/module/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from typing import Any
 import uuid
 
 import aiohttp
 from packaging.version import parse
 from plyer import uniqueid
 from psutil import boot_time, users
-from psutil._common import suser
+from systembridgemodels.modules.system import SystemUser
 
 from systembridgeshared.base import Base
 from systembridgeshared.common import get_user_data_directory
 
 from .._version import __version__
 
 
@@ -233,17 +233,28 @@
         """Get platform version."""
         return platform.version()
 
     def get_uptime(self) -> float:
         """Get uptime."""
         return os.times().system
 
-    def get_users(self) -> list[suser]:  # pylint: disable=unsubscriptable-object
+    def get_users(self) -> list[SystemUser]:
         """Get users."""
-        return users()
+        active_user_name = self.get_active_user_name()
+        return [
+            SystemUser(
+                name=user.name,
+                active=user.name == active_user_name if active_user_name else False,
+                terminal=user.terminal or "",
+                host=user.host or "",
+                started=user.started,
+                pid=float(user.pid) if user.pid else 0.0,
+            )
+            for user in users()
+        ]
 
     @property
     def _uuid(self) -> str:
         """Get UUID."""
         # cat /var/lib/dbus/machine-id
         if sys.platform == "linux":
             try:
```

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata.egg-info/PKG-INFO` & `systembridgedata-5.0.0.dev2/systembridgedata.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgedata
-Version: 5.0.0.dev1
+Version: 5.0.0.dev2
 Summary: System Bridge Data
 Home-page: https://github.com/timmo001/system-bridge-data
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgedata-5.0.0.dev1/systembridgedata.egg-info/SOURCES.txt` & `systembridgedata-5.0.0.dev2/systembridgedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

