# Comparing `tmp/onc-2.3.4.tar.gz` & `tmp/onc-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onc-2.3.4.tar", last modified: Thu Dec 12 01:50:57 2019, max compression
+gzip compressed data, was "dist/onc-2.3.5.tar", last modified: Thu Dec 12 21:31:00 2019, max compression
```

## Comparing `onc-2.3.4.tar` & `onc-2.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 01:50:57.000000 onc-2.3.4/
--rw-rw-r--   0 dany      (1002) dany      (1002)     1306 2019-12-12 01:50:48.000000 onc-2.3.4/setup.py
--rw-rw-r--   0 dany      (1002) dany      (1002)      704 2019-11-20 18:00:46.000000 onc-2.3.4/README.md
-drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 01:50:57.000000 onc-2.3.4/onc.egg-info/
--rw-rw-r--   0 dany      (1002) dany      (1002)        1 2019-12-12 01:50:57.000000 onc-2.3.4/onc.egg-info/dependency_links.txt
--rw-rw-r--   0 dany      (1002) dany      (1002)       48 2019-12-12 01:50:57.000000 onc-2.3.4/onc.egg-info/requires.txt
--rw-rw-r--   0 dany      (1002) dany      (1002)      554 2019-12-12 01:50:57.000000 onc-2.3.4/onc.egg-info/SOURCES.txt
--rw-rw-r--   0 dany      (1002) dany      (1002)     1431 2019-12-12 01:50:57.000000 onc-2.3.4/onc.egg-info/PKG-INFO
--rw-rw-r--   0 dany      (1002) dany      (1002)        4 2019-12-12 01:50:57.000000 onc-2.3.4/onc.egg-info/top_level.txt
--rw-rw-r--   0 dany      (1002) dany      (1002)     1431 2019-12-12 01:50:57.000000 onc-2.3.4/PKG-INFO
-drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 01:50:57.000000 onc-2.3.4/onc/
--rw-rw-r--   0 dany      (1002) dany      (1002)     4082 2018-12-06 02:58:10.000000 onc-2.3.4/onc/ags.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     5140 2018-12-06 02:58:10.000000 onc-2.3.4/onc/dap.py
-drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 01:50:57.000000 onc-2.3.4/onc/modules/
--rw-rw-r--   0 dany      (1002) dany      (1002)     2865 2019-08-09 00:14:18.000000 onc-2.3.4/onc/modules/_OncRealTime.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     2450 2019-08-19 20:55:34.000000 onc-2.3.4/onc/modules/_PollLog.py
--rw-rw-r--   0 dany      (1002) dany      (1002)        0 2019-06-27 23:07:01.000000 onc-2.3.4/onc/modules/__init__.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     2710 2019-12-12 00:45:59.000000 onc-2.3.4/onc/modules/_util.py
--rw-rw-r--   0 dany      (1002) dany      (1002)       86 2019-06-27 23:10:36.000000 onc-2.3.4/onc/modules/Exceptions.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     8094 2019-12-12 01:45:52.000000 onc-2.3.4/onc/modules/_OncArchive.py
--rw-rw-r--   0 dany      (1002) dany      (1002)    12401 2019-12-12 01:24:13.000000 onc-2.3.4/onc/modules/_OncDelivery.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     7035 2019-11-20 17:10:21.000000 onc-2.3.4/onc/modules/_MultiPage.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     3488 2019-08-28 21:43:03.000000 onc-2.3.4/onc/modules/_OncService.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     3257 2019-11-30 00:50:25.000000 onc-2.3.4/onc/modules/_OncDiscovery.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     5509 2019-12-12 01:07:00.000000 onc-2.3.4/onc/modules/_DataProductFile.py
--rw-rw-r--   0 dany      (1002) dany      (1002)      121 2019-06-27 23:07:00.000000 onc-2.3.4/onc/__init__.py
--rw-rw-r--   0 dany      (1002) dany      (1002)    16817 2019-05-14 21:54:22.000000 onc-2.3.4/onc/sos.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     6499 2019-07-02 17:10:56.000000 onc-2.3.4/onc/nerc.py
--rw-rw-r--   0 dany      (1002) dany      (1002)     5519 2019-08-15 21:30:41.000000 onc-2.3.4/onc/onc.py
-drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 01:50:57.000000 onc-2.3.4/onc/util/
--rw-rw-r--   0 dany      (1002) dany      (1002)        0 2019-04-15 18:52:32.000000 onc-2.3.4/onc/util/__init__.py
--rw-rw-r--   0 dany      (1002) dany      (1002)    10606 2019-05-21 17:30:58.000000 onc-2.3.4/onc/util/util.py
--rw-rw-r--   0 dany      (1002) dany      (1002)       38 2019-12-12 01:50:57.000000 onc-2.3.4/setup.cfg
+drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 21:31:00.000000 onc-2.3.5/
+-rw-rw-r--   0 dany      (1002) dany      (1002)     1306 2019-12-12 21:29:53.000000 onc-2.3.5/setup.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)      704 2019-11-20 18:00:46.000000 onc-2.3.5/README.md
+drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 21:31:00.000000 onc-2.3.5/onc.egg-info/
+-rw-rw-r--   0 dany      (1002) dany      (1002)        1 2019-12-12 21:31:00.000000 onc-2.3.5/onc.egg-info/dependency_links.txt
+-rw-rw-r--   0 dany      (1002) dany      (1002)       48 2019-12-12 21:31:00.000000 onc-2.3.5/onc.egg-info/requires.txt
+-rw-rw-r--   0 dany      (1002) dany      (1002)      554 2019-12-12 21:31:00.000000 onc-2.3.5/onc.egg-info/SOURCES.txt
+-rw-rw-r--   0 dany      (1002) dany      (1002)     1431 2019-12-12 21:31:00.000000 onc-2.3.5/onc.egg-info/PKG-INFO
+-rw-rw-r--   0 dany      (1002) dany      (1002)        4 2019-12-12 21:31:00.000000 onc-2.3.5/onc.egg-info/top_level.txt
+-rw-rw-r--   0 dany      (1002) dany      (1002)     1431 2019-12-12 21:31:00.000000 onc-2.3.5/PKG-INFO
+drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 21:31:00.000000 onc-2.3.5/onc/
+-rw-rw-r--   0 dany      (1002) dany      (1002)     4082 2018-12-06 02:58:10.000000 onc-2.3.5/onc/ags.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     5140 2018-12-06 02:58:10.000000 onc-2.3.5/onc/dap.py
+drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 21:31:00.000000 onc-2.3.5/onc/modules/
+-rw-rw-r--   0 dany      (1002) dany      (1002)     2865 2019-08-09 00:14:18.000000 onc-2.3.5/onc/modules/_OncRealTime.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     2450 2019-08-19 20:55:34.000000 onc-2.3.5/onc/modules/_PollLog.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)        0 2019-06-27 23:07:01.000000 onc-2.3.5/onc/modules/__init__.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     2710 2019-12-12 00:45:59.000000 onc-2.3.5/onc/modules/_util.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)       86 2019-06-27 23:10:36.000000 onc-2.3.5/onc/modules/Exceptions.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     8077 2019-12-12 21:29:27.000000 onc-2.3.5/onc/modules/_OncArchive.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)    12401 2019-12-12 01:24:13.000000 onc-2.3.5/onc/modules/_OncDelivery.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     7035 2019-11-20 17:10:21.000000 onc-2.3.5/onc/modules/_MultiPage.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     3488 2019-08-28 21:43:03.000000 onc-2.3.5/onc/modules/_OncService.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     3257 2019-11-30 00:50:25.000000 onc-2.3.5/onc/modules/_OncDiscovery.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     5509 2019-12-12 01:07:00.000000 onc-2.3.5/onc/modules/_DataProductFile.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)      121 2019-06-27 23:07:00.000000 onc-2.3.5/onc/__init__.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)    16817 2019-05-14 21:54:22.000000 onc-2.3.5/onc/sos.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     6499 2019-07-02 17:10:56.000000 onc-2.3.5/onc/nerc.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)     5519 2019-08-15 21:30:41.000000 onc-2.3.5/onc/onc.py
+drwxrwxr-x   0 dany      (1002) dany      (1002)        0 2019-12-12 21:31:00.000000 onc-2.3.5/onc/util/
+-rw-rw-r--   0 dany      (1002) dany      (1002)        0 2019-04-15 18:52:32.000000 onc-2.3.5/onc/util/__init__.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)    10606 2019-05-21 17:30:58.000000 onc-2.3.5/onc/util/util.py
+-rw-rw-r--   0 dany      (1002) dany      (1002)       38 2019-12-12 21:31:00.000000 onc-2.3.5/setup.cfg
```

### Comparing `onc-2.3.4/setup.py` & `onc-2.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 # Modify this version before publishing a new release
-buildVersion = "2.3.4"
+buildVersion = "2.3.5"
 
 print('setup.py has build version: ' + buildVersion + '. Make sure this is the version you want to upload.')
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
```

### Comparing `onc-2.3.4/README.md` & `onc-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc.egg-info/SOURCES.txt` & `onc-2.3.5/onc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc.egg-info/PKG-INFO` & `onc-2.3.5/onc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onc
-Version: 2.3.4
+Version: 2.3.5
 Summary: Ocean 2.0 API Python Client Library
 Home-page: https://wiki.oceannetworks.ca/display/O2A/Python+Client+Library
 Author: ONC Data Team
 Author-email: data@oceannetworks.ca
 Maintainer: Dany Cabrera
 Maintainer-email: dcabrera@uvic.ca
 License: Apache 2.0
```

### Comparing `onc-2.3.4/PKG-INFO` & `onc-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onc
-Version: 2.3.4
+Version: 2.3.5
 Summary: Ocean 2.0 API Python Client Library
 Home-page: https://wiki.oceannetworks.ca/display/O2A/Python+Client+Library
 Author: ONC Data Team
 Author-email: data@oceannetworks.ca
 Maintainer: Dany Cabrera
 Maintainer-email: dcabrera@uvic.ca
 License: Apache 2.0
```

### Comparing `onc-2.3.4/onc/ags.py` & `onc-2.3.5/onc/ags.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/dap.py` & `onc-2.3.5/onc/dap.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_OncRealTime.py` & `onc-2.3.5/onc/modules/_OncRealTime.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_PollLog.py` & `onc-2.3.5/onc/modules/_PollLog.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_util.py` & `onc-2.3.5/onc/modules/_util.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_OncArchive.py` & `onc-2.3.5/onc/modules/_OncArchive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ._OncService import _OncService
 from ._MultiPage import _MultiPage
 import requests
 import json
-import puremagic
 import humanize
 import os
 import time
 
 from ._util import saveAsFile, _printErrorMessage, _formatDuration
 
 class _OncArchive(_OncService):
```

### Comparing `onc-2.3.4/onc/modules/_OncDelivery.py` & `onc-2.3.5/onc/modules/_OncDelivery.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_MultiPage.py` & `onc-2.3.5/onc/modules/_MultiPage.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_OncService.py` & `onc-2.3.5/onc/modules/_OncService.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_OncDiscovery.py` & `onc-2.3.5/onc/modules/_OncDiscovery.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/modules/_DataProductFile.py` & `onc-2.3.5/onc/modules/_DataProductFile.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/sos.py` & `onc-2.3.5/onc/sos.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/nerc.py` & `onc-2.3.5/onc/nerc.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/onc.py` & `onc-2.3.5/onc/onc.py`

 * *Files identical despite different names*

### Comparing `onc-2.3.4/onc/util/util.py` & `onc-2.3.5/onc/util/util.py`

 * *Files identical despite different names*

