# Comparing `tmp/my_dc09_spt-0.1.1.tar.gz` & `tmp/my_dc09_spt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_dc09_spt-0.1.1.tar", last modified: Thu May 30 09:46:13 2024, max compression
+gzip compressed data, was "my_dc09_spt-0.1.2.tar", last modified: Thu May 30 10:01:44 2024, max compression
```

## Comparing `my_dc09_spt-0.1.1.tar` & `my_dc09_spt-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:46:13.297605 my_dc09_spt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-30 09:46:13.293605 my_dc09_spt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:46:13.293605 my_dc09_spt-0.1.1/dc09_spt/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:46:13.293605 my_dc09_spt-0.1.1/dc09_spt/comm/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/comm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/comm/transpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/comm/transpathtcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/comm/transpathudp.py
--rw-r--r--   0 runner    (1001) docker     (127)    26625 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/dc09_spt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:46:13.293605 my_dc09_spt-0.1.1/dc09_spt/msg/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/msg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/msg/dc03_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/msg/dc05_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/msg/dc09_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/param.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/dc09_spt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:46:13.293605 my_dc09_spt-0.1.1/example/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/example/testdailler.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/example/testsendmsg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:46:13.293605 my_dc09_spt-0.1.1/my_dc09_spt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-30 09:46:13.000000 my_dc09_spt-0.1.1/my_dc09_spt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-30 09:46:13.000000 my_dc09_spt-0.1.1/my_dc09_spt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:46:13.000000 my_dc09_spt-0.1.1/my_dc09_spt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 09:46:13.000000 my_dc09_spt-0.1.1/my_dc09_spt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 09:46:13.000000 my_dc09_spt-0.1.1/my_dc09_spt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 09:46:13.297605 my_dc09_spt-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-30 09:46:05.000000 my_dc09_spt-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:01:44.852632 my_dc09_spt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-30 10:01:44.852632 my_dc09_spt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:01:44.848632 my_dc09_spt-0.1.2/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/example/testdailler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/example/testsendmsg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:01:44.852632 my_dc09_spt-0.1.2/my_dc09_spt/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:01:44.852632 my_dc09_spt-0.1.2/my_dc09_spt/comm/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/comm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/comm/transpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/comm/transpathtcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/comm/transpathudp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26637 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/dc09_spt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:01:44.852632 my_dc09_spt-0.1.2/my_dc09_spt/msg/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/msg/dc03_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/msg/dc05_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/msg/dc09_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/my_dc09_spt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 10:01:44.852632 my_dc09_spt-0.1.2/my_dc09_spt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-30 10:01:44.000000 my_dc09_spt-0.1.2/my_dc09_spt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-30 10:01:44.000000 my_dc09_spt-0.1.2/my_dc09_spt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 10:01:44.000000 my_dc09_spt-0.1.2/my_dc09_spt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 10:01:44.000000 my_dc09_spt-0.1.2/my_dc09_spt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-30 10:01:44.000000 my_dc09_spt-0.1.2/my_dc09_spt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 10:01:44.852632 my_dc09_spt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-30 10:01:40.000000 my_dc09_spt-0.1.2/setup.py
```

### Comparing `my_dc09_spt-0.1.1/LICENSE` & `my_dc09_spt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `my_dc09_spt-0.1.1/PKG-INFO` & `my_dc09_spt-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_dc09_spt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A dialler implementation using the SIA-DC09 protocol
 Home-page: https://github.com/jvanovost/dc09_spt
 Author: Jacq. van Ovost
 Author-email: jacq.van.ovost@gmail.com
 Keywords: DC09,SIA DC09,SPT,Alarm transmitter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `my_dc09_spt-0.1.1/README.md` & `my_dc09_spt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `my_dc09_spt-0.1.1/dc09_spt/comm/transpath.py` & `my_dc09_spt-0.1.2/my_dc09_spt/comm/transpath.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ----------------------------
 # Transmit class
 # (c 2018 van Ovost Automatisering b.v.
 # Author : Jacq. van Ovost
 # ----------------------------
 import logging
-from dc09_spt.comm.transpathtcp import TransPathTCP
-from dc09_spt.comm.transpathudp import TransPathUDP
+from my_dc09_spt.comm.transpathtcp import TransPathTCP
+from my_dc09_spt.comm.transpathudp import TransPathUDP
 
 
 class TransPath:
     """
     Handle the basic tasks for establishing and maintaining a transmit path
     """
     def __init__(self,  host,  port,  account, *, key=None,  receiver=None,  line=None,  timeout=5.0,  type=None):
```

### Comparing `my_dc09_spt-0.1.1/dc09_spt/comm/transpathtcp.py` & `my_dc09_spt-0.1.2/my_dc09_spt/comm/transpathtcp.py`

 * *Files identical despite different names*

### Comparing `my_dc09_spt-0.1.1/dc09_spt/comm/transpathudp.py` & `my_dc09_spt-0.1.2/my_dc09_spt/comm/transpathudp.py`

 * *Files identical despite different names*

### Comparing `my_dc09_spt-0.1.1/dc09_spt/dc09_spt.py` & `my_dc09_spt-0.1.2/my_dc09_spt/dc09_spt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # ----------------------------
 # Dialler class
 # (c 2018 van Ovost Automatisering b.v.
 # Author : Jacq. van Ovost
 # ----------------------------
-from dc09_spt.msg.dc09_msg import *
-from dc09_spt.msg.dc05_msg import *
-from dc09_spt.msg.dc03_msg import *
+from my_dc09_spt.msg.dc09_msg import *
+from my_dc09_spt.msg.dc05_msg import *
+from my_dc09_spt.msg.dc03_msg import *
 import time
 import threading
 from collections import deque
 import logging
-from dc09_spt.comm.transpath import TransPath
+from my_dc09_spt.comm.transpath import TransPath
 
 
 class dc09_spt:
     """
     Handle the basic tasks of SPT (Secured Premises Transciever)
 
     Copyright (c) 2018  van Ovost Automatisering b.v.
```

### Comparing `my_dc09_spt-0.1.1/dc09_spt/msg/dc03_msg.py` & `my_dc09_spt-0.1.2/my_dc09_spt/msg/dc03_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ----------------------------
 # Class to implement the SIA DC03 message
 # (c 2018 van Ovost Automatisering b.v.
 # Author : Jacq. van Ovost
 # ----------------------------
 import time
-from dc09_spt.param import *
+from my_dc09_spt.param import *
 import logging
 """
 
     Copyright (c) 2018  van Ovost Automatisering b.v.
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
```

### Comparing `my_dc09_spt-0.1.1/dc09_spt/msg/dc05_msg.py` & `my_dc09_spt-0.1.2/my_dc09_spt/msg/dc05_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ----------------------------
 # Class to implement the SIA DC05 message
 # (c 2018 van Ovost Automatisering b.v.
 # Author : Jacq. van Ovost
 # ----------------------------
-from dc09_spt.param import *
+from my_dc09_spt.param import *
 """
 
 Copyright (c) 2018  van Ovost Automatisering b.v.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 you may obtain a copy of the License at
```

### Comparing `my_dc09_spt-0.1.1/dc09_spt/msg/dc09_msg.py` & `my_dc09_spt-0.1.2/my_dc09_spt/msg/dc09_msg.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # (c 2018 van Ovost Automatisering b.v.
 # Author : Jacq. van Ovost
 # ----------------------------
 import datetime
 import random
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
-from dc09_spt.utils import convert_timestamp_to_dc09_datetime
+from my_dc09_spt.utils import convert_timestamp_to_dc09_datetime
 
 
 class dc09_msg:
     """
     SIA DC09 message block implementation
     
     This class serves to build a message block from an DC07 payload message as constructed in:
```

### Comparing `my_dc09_spt-0.1.1/dc09_spt/param.py` & `my_dc09_spt-0.1.2/my_dc09_spt/param.py`

 * *Files identical despite different names*

### Comparing `my_dc09_spt-0.1.1/example/testdailler.py` & `my_dc09_spt-0.1.2/example/testdailler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ----------------------------
 # Test dialler to show use of dc09_msg class
 # (c 2018 van Ovost Automatisering b.v.
 # Author : Jacq. van Ovost
 # ----------------------------
 import sys
 sys.path.append('../')
-from dc09_spt import dc09_spt
+from my_dc09_spt import dc09_spt
 
 import logging
 logging.basicConfig(format='%(module)-12s %(asctime)s %(levelname)-8s %(message)s')
 logger = logging.getLogger()
 #handler = logging.StreamHandler()
 #logger.addHandler(handler)
 logger.setLevel(logging.DEBUG)
```

### Comparing `my_dc09_spt-0.1.1/example/testsendmsg.py` & `my_dc09_spt-0.1.2/example/testsendmsg.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Test dialler to show use of dc09_msg class
 # (c 2018 van Ovost Automatisering b.v.
 # Author : Jacq. van Ovost
 # ----------------------------
 import sys
 
 sys.path.append('../')
-from dc09_spt import dc09_spt
+from my_dc09_spt import dc09_spt
 
 import logging
 logging.basicConfig(format='%(module)-12s %(asctime)s %(levelname)-8s %(message)s')
 logger = logging.getLogger()
 #handler = logging.StreamHandler()
 #logger.addHandler(handler)
 logger.setLevel(logging.DEBUG)
```

### Comparing `my_dc09_spt-0.1.1/my_dc09_spt.egg-info/PKG-INFO` & `my_dc09_spt-0.1.2/my_dc09_spt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_dc09_spt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A dialler implementation using the SIA-DC09 protocol
 Home-page: https://github.com/jvanovost/dc09_spt
 Author: Jacq. van Ovost
 Author-email: jacq.van.ovost@gmail.com
 Keywords: DC09,SIA DC09,SPT,Alarm transmitter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `my_dc09_spt-0.1.1/my_dc09_spt.egg-info/SOURCES.txt` & `my_dc09_spt-0.1.2/my_dc09_spt.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 LICENSE
 README.md
 setup.py
-dc09_spt/__init__.py
-dc09_spt/dc09_spt.py
-dc09_spt/param.py
-dc09_spt/utils.py
-dc09_spt/comm/__init__.py
-dc09_spt/comm/transpath.py
-dc09_spt/comm/transpathtcp.py
-dc09_spt/comm/transpathudp.py
-dc09_spt/msg/__init__.py
-dc09_spt/msg/dc03_msg.py
-dc09_spt/msg/dc05_msg.py
-dc09_spt/msg/dc09_msg.py
 example/__init__.py
 example/testdailler.py
 example/testsendmsg.py
+my_dc09_spt/__init__.py
+my_dc09_spt/dc09_spt.py
+my_dc09_spt/param.py
+my_dc09_spt/utils.py
 my_dc09_spt.egg-info/PKG-INFO
 my_dc09_spt.egg-info/SOURCES.txt
 my_dc09_spt.egg-info/dependency_links.txt
 my_dc09_spt.egg-info/requires.txt
-my_dc09_spt.egg-info/top_level.txt
+my_dc09_spt.egg-info/top_level.txt
+my_dc09_spt/comm/__init__.py
+my_dc09_spt/comm/transpath.py
+my_dc09_spt/comm/transpathtcp.py
+my_dc09_spt/comm/transpathudp.py
+my_dc09_spt/msg/__init__.py
+my_dc09_spt/msg/dc03_msg.py
+my_dc09_spt/msg/dc05_msg.py
+my_dc09_spt/msg/dc09_msg.py
```

### Comparing `my_dc09_spt-0.1.1/setup.py` & `my_dc09_spt-0.1.2/setup.py`

 * *Files identical despite different names*

