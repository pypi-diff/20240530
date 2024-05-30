# Comparing `tmp/redbacktechpy-0.3.1.tar.gz` & `tmp/redbacktechpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-0.3.1.tar", last modified: Thu May 30 07:32:55 2024, max compression
+gzip compressed data, was "redbacktechpy-0.5.0.tar", last modified: Thu May 30 07:45:47 2024, max compression
```

## Comparing `redbacktechpy-0.3.1.tar` & `redbacktechpy-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:32:55.274467 redbacktechpy-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:32:55.274467 redbacktechpy-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:32:55.274467 redbacktechpy-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:32:55.270467 redbacktechpy-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:32:55.270467 redbacktechpy-0.3.1/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26021 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 07:32:50.000000 redbacktechpy-0.3.1/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:32:55.274467 redbacktechpy-0.3.1/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:32:55.000000 redbacktechpy-0.3.1/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 07:32:55.000000 redbacktechpy-0.3.1/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:32:55.000000 redbacktechpy-0.3.1/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 07:32:55.000000 redbacktechpy-0.3.1/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 07:32:55.000000 redbacktechpy-0.3.1/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.830552 redbacktechpy-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.830552 redbacktechpy-0.5.0/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26024 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-30 07:45:43.000000 redbacktechpy-0.5.0/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 07:45:47.834552 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 07:45:47.000000 redbacktechpy-0.5.0/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-0.3.1/LICENSE` & `redbacktechpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.3.1/PKG-INFO` & `redbacktechpy-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 0.3.1
+Version: 0.5.0
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-0.3.1/pyproject.toml` & `redbacktechpy-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "0.3.1"
+version = "0.5.0"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-0.3.1/src/redbacktechpy/__init__.py` & `redbacktechpy-0.5.0/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.3.1/src/redbacktechpy/constants.py` & `redbacktechpy-0.5.0/src/redbacktechpy/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from str_enum import StrEnum
+from .str_enum import StrEnum
 
 TIMEOUT = 5 * 60
 DEVICEINFOREFRESH = 30 * 60  #Number of seconds to wait before refreshing device info as it doesn't change very often
 
 AUTH_ERROR_CODES = [
     'unauthorized_client',
     'Login session expired.',
```

### Comparing `redbacktechpy-0.3.1/src/redbacktechpy/model.py` & `redbacktechpy-0.5.0/src/redbacktechpy/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Data classes for Redback Tech API """
 from __future__ import annotations
 
-from dataclasses import dataclass
+from .dataclasses import dataclass
 import datetime
 from typing import Any, Optional
 
 
 @dataclass
 class Site:
     """Dataclass for Redback Sites."""
```

### Comparing `redbacktechpy-0.3.1/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-0.5.0/src/redbacktechpy/redbacktech_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from aiohttp import ClientResponse, ClientSession
 from typing import Any
 import asyncio
 from datetime import datetime, timedelta, timezone
 from bs4 import BeautifulSoup
 import logging
 
-from constants import (
+from .constants import (
     BaseUrl, 
     Endpoint, 
     Header,
     InverterOperationType,
     TIMEOUT,
     AUTH_ERROR_CODES,
     DEVICEINFOREFRESH,
 )
 
-from model import (
+from .model import (
     Inverters,
     Batterys,
 )
-from exceptions import (
+from .exceptions import (
         AuthError, 
         RedbackTechClientError,
 )
 
 LOGGER = logging.getLogger(__name__)
 
 class RedbackTechClient:
```

### Comparing `redbacktechpy-0.3.1/src/redbacktechpy/str_enum.py` & `redbacktechpy-0.5.0/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-0.3.1/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-0.5.0/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 0.3.1
+Version: 0.5.0
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

