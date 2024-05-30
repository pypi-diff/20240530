# Comparing `tmp/inflow_haisslab-1.2.7.tar.gz` & `tmp/inflow_haisslab-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inflow_haisslab-1.2.7.tar", last modified: Fri Mar 22 13:00:31 2024, max compression
+gzip compressed data, was "inflow_haisslab-1.2.8.tar", last modified: Tue Mar 26 17:03:33 2024, max compression
```

## Comparing `inflow_haisslab-1.2.7.tar` & `inflow_haisslab-1.2.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2942 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/__init__.py
--rw-r--r--   0        0        0      138 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/bins/__init__.py
--rw-r--r--   0        0        0     2158 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/bins/content.py
--rw-r--r--   0        0        0      518 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/__init__.py
--rw-r--r--   0        0        0    12010 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/config.py
--rw-r--r--   0        0        0    13126 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/decorators.py
--rw-r--r--   0        0        0    10938 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/logging.py
--rw-r--r--   0        0        0     1281 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/optimization.py
--rw-r--r--   0        0        0    31911 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/pipelining.py
--rw-r--r--   0        0        0     3493 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/special_types.py
--rw-r--r--   0        0        0       87 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/time.py
--rw-r--r--   0        0        0     1197 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/core/utils.py
--rw-r--r--   0        0        0      148 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/ios/__init__.py
--rw-r--r--   0        0        0     2263 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/ios/helpers.py
--rw-r--r--   0        0        0    11091 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/ios/load.py
--rw-r--r--   0        0        0     4291 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/ios/save.py
--rw-r--r--   0        0        0      117 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/masks/__init__.py
--rw-r--r--   0        0        0    11739 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/masks/create.py
--rw-r--r--   0        0        0       24 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/pandex/__init__.py
--rw-r--r--   0        0        0     4704 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/pandex/accessors.py
--rw-r--r--   0        0        0      405 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/path/__init__.py
--rw-r--r--   0        0        0     2913 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/path/extract.py
--rw-r--r--   0        0        0     2316 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/path/find.py
--rw-r--r--   0        0        0    20318 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/path/one_alf.py
--rw-r--r--   0        0        0      511 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/path/pattern.py
--rw-r--r--   0        0        0      155 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/plots/__init__.py
--rw-r--r--   0        0        0      818 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/plots/artists.py
--rw-r--r--   0        0        0       26 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/plots/captions.py
--rw-r--r--   0        0        0     2499 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/plots/colors.py
--rw-r--r--   0        0        0    13096 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/plots/custom.py
--rw-r--r--   0        0        0    14276 2024-03-22 13:00:21.171300 inflow_haisslab-1.2.7/Inflow/plots/graphviz.py
--rw-r--r--   0        0        0    16687 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/plots/utils.py
--rw-r--r--   0        0        0     2065 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/signal/__init__.py
--rw-r--r--   0        0        0     4943 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/signal/filters.py
--rw-r--r--   0        0        0     3819 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/signal/fits.py
--rw-r--r--   0        0        0     1601 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/signal/fluo.py
--rw-r--r--   0        0        0     3505 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/signal/norms.py
--rw-r--r--   0        0        0       57 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/tdms/__init__.py
--rw-r--r--   0        0        0     3124 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/tdms/content.py
--rw-r--r--   0        0        0     2411 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/tiff/__init__.py
--rw-r--r--   0        0        0    27307 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/tiff/content.py
--rw-r--r--   0        0        0   160256 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/Inflow/tiff/tiff_metadata_parse.dll
--rw-r--r--   0        0        0     1064 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/LICENSE
--rw-r--r--   0        0        0     1776 2024-03-22 13:00:21.175300 inflow_haisslab-1.2.7/README.md
--rw-r--r--   0        0        0     1415 2024-03-22 13:00:31.091184 inflow_haisslab-1.2.7/pyproject.toml
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 inflow_haisslab-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     2953 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/__init__.py
+-rw-r--r--   0        0        0      138 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/bins/__init__.py
+-rw-r--r--   0        0        0     2158 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/bins/content.py
+-rw-r--r--   0        0        0      518 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/__init__.py
+-rw-r--r--   0        0        0    12010 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/config.py
+-rw-r--r--   0        0        0    13126 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/decorators.py
+-rw-r--r--   0        0        0    10938 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/logging.py
+-rw-r--r--   0        0        0     1281 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/optimization.py
+-rw-r--r--   0        0        0    31911 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/pipelining.py
+-rw-r--r--   0        0        0     3493 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/special_types.py
+-rw-r--r--   0        0        0       87 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/time.py
+-rw-r--r--   0        0        0     1197 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/core/utils.py
+-rw-r--r--   0        0        0      148 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/ios/__init__.py
+-rw-r--r--   0        0        0     2263 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/ios/helpers.py
+-rw-r--r--   0        0        0    11091 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/ios/load.py
+-rw-r--r--   0        0        0     4291 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/ios/save.py
+-rw-r--r--   0        0        0      117 2024-03-26 17:03:23.914118 inflow_haisslab-1.2.8/Inflow/masks/__init__.py
+-rw-r--r--   0        0        0    11739 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/masks/create.py
+-rw-r--r--   0        0        0       24 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/pandex/__init__.py
+-rw-r--r--   0        0        0     4704 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/pandex/accessors.py
+-rw-r--r--   0        0        0      405 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/path/__init__.py
+-rw-r--r--   0        0        0     2913 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/path/extract.py
+-rw-r--r--   0        0        0     2316 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/path/find.py
+-rw-r--r--   0        0        0    20318 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/path/one_alf.py
+-rw-r--r--   0        0        0      511 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/path/pattern.py
+-rw-r--r--   0        0        0      155 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/plots/__init__.py
+-rw-r--r--   0        0        0      818 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/plots/artists.py
+-rw-r--r--   0        0        0       26 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/plots/captions.py
+-rw-r--r--   0        0        0     2499 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/plots/colors.py
+-rw-r--r--   0        0        0    13096 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/plots/custom.py
+-rw-r--r--   0        0        0    14276 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/plots/graphviz.py
+-rw-r--r--   0        0        0    16687 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/plots/utils.py
+-rw-r--r--   0        0        0     2065 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/signal/__init__.py
+-rw-r--r--   0        0        0     4943 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/signal/filters.py
+-rw-r--r--   0        0        0     3819 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/signal/fits.py
+-rw-r--r--   0        0        0     1601 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/signal/fluo.py
+-rw-r--r--   0        0        0     3505 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/signal/norms.py
+-rw-r--r--   0        0        0       57 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/tdms/__init__.py
+-rw-r--r--   0        0        0     3124 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/tdms/content.py
+-rw-r--r--   0        0        0     2411 2024-03-26 17:03:23.918118 inflow_haisslab-1.2.8/Inflow/tiff/__init__.py
+-rw-r--r--   0        0        0    27307 2024-03-26 17:03:23.922118 inflow_haisslab-1.2.8/Inflow/tiff/content.py
+-rw-r--r--   0        0        0   160256 2024-03-26 17:03:23.922118 inflow_haisslab-1.2.8/Inflow/tiff/tiff_metadata_parse.dll
+-rw-r--r--   0        0        0     1064 2024-03-26 17:03:23.922118 inflow_haisslab-1.2.8/LICENSE
+-rw-r--r--   0        0        0     1776 2024-03-26 17:03:23.922118 inflow_haisslab-1.2.8/README.md
+-rw-r--r--   0        0        0     1415 2024-03-26 17:03:33.617979 inflow_haisslab-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 inflow_haisslab-1.2.8/PKG-INFO
```

### Comparing `inflow_haisslab-1.2.7/Inflow/__init__.py` & `inflow_haisslab-1.2.8/Inflow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-__version__ = "1.2.7"
+__version__ = "1.2.8"
 
 
 # external imports
 import os, sys
 
 # TODO : remove this part once the paramiko warning deprecation have been resolved by Suite2p developpers
 import warnings
 
-try:
-    from cryptography.utils import CryptographyDeprecationWarning
+# try:
+#     from cryptography.utils import CryptographyDeprecationWarning
 
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=CryptographyDeprecationWarning)
-        import paramiko
-except ModuleNotFoundError:
-    pass
+#     with warnings.catch_warnings():
+#         warnings.filterwarnings("ignore", category=CryptographyDeprecationWarning)
+#         import paramiko
+# except ModuleNotFoundError:
+#     pass
 # end
 
 # one level down imports
 from . import signal
 from . import tdms
 from . import tiff
 from . import path
@@ -48,31 +48,31 @@
 
 
 def run_suite2p_gui_asking_session():
     import one
 
     connector = one.ONE(data_access_mode="remote")
     session_label = ask_for_session_label_gui()
-    print(f"{session_label = }")
+    print(f"{session_label=}")
     session_id = connector.to_eid(session_label)
-    print(f"{session_id = }")
+    print(f"{session_id=}")
     session_details = connector.search(id=session_id, details=True)
     run_suite2p_gui(session_details, allow_blank=False)
 
 
 def run_suite2p_gui(session_details=None, plane=0, statfile=None, allow_blank=True):
     from suite2p import gui as suite2p_gui_module
     from PyQt5 import QtWidgets
 
     if statfile is None:
         from .ios.helpers import get_suite2p_path
         from logging import getLogger
 
         try:
-            statfile = get_suite2p_path(session_details=session_details, plane=plane, file="stat\.npy")[0]
+            statfile = get_suite2p_path(session_details=session_details, plane=plane, file="stat\\.npy")[0]
             getLogger().load(f"Opening GUI directly at stat file {statfile}")
         except (
             IndexError,
             ValueError,
             AttributeError,
         ):  # session_details is None or no stat file found at session_details.path
             statfile = None
```

### Comparing `inflow_haisslab-1.2.7/Inflow/bins/content.py` & `inflow_haisslab-1.2.8/Inflow/bins/content.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/__init__.py` & `inflow_haisslab-1.2.8/Inflow/core/__init__.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/config.py` & `inflow_haisslab-1.2.8/Inflow/core/config.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/decorators.py` & `inflow_haisslab-1.2.8/Inflow/core/decorators.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/logging.py` & `inflow_haisslab-1.2.8/Inflow/core/logging.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/optimization.py` & `inflow_haisslab-1.2.8/Inflow/core/optimization.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/pipelining.py` & `inflow_haisslab-1.2.8/Inflow/core/pipelining.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/special_types.py` & `inflow_haisslab-1.2.8/Inflow/core/special_types.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/core/utils.py` & `inflow_haisslab-1.2.8/Inflow/core/utils.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/ios/helpers.py` & `inflow_haisslab-1.2.8/Inflow/ios/helpers.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/ios/load.py` & `inflow_haisslab-1.2.8/Inflow/ios/load.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/ios/save.py` & `inflow_haisslab-1.2.8/Inflow/ios/save.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/masks/create.py` & `inflow_haisslab-1.2.8/Inflow/masks/create.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/pandex/accessors.py` & `inflow_haisslab-1.2.8/Inflow/pandex/accessors.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/path/extract.py` & `inflow_haisslab-1.2.8/Inflow/path/extract.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/path/find.py` & `inflow_haisslab-1.2.8/Inflow/path/find.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/path/one_alf.py` & `inflow_haisslab-1.2.8/Inflow/path/one_alf.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/plots/artists.py` & `inflow_haisslab-1.2.8/Inflow/plots/artists.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/plots/colors.py` & `inflow_haisslab-1.2.8/Inflow/plots/colors.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/plots/custom.py` & `inflow_haisslab-1.2.8/Inflow/plots/custom.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/plots/graphviz.py` & `inflow_haisslab-1.2.8/Inflow/plots/graphviz.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/plots/utils.py` & `inflow_haisslab-1.2.8/Inflow/plots/utils.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/signal/__init__.py` & `inflow_haisslab-1.2.8/Inflow/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/signal/filters.py` & `inflow_haisslab-1.2.8/Inflow/signal/filters.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/signal/fits.py` & `inflow_haisslab-1.2.8/Inflow/signal/fits.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/signal/fluo.py` & `inflow_haisslab-1.2.8/Inflow/signal/fluo.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/signal/norms.py` & `inflow_haisslab-1.2.8/Inflow/signal/norms.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/tdms/content.py` & `inflow_haisslab-1.2.8/Inflow/tdms/content.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/tiff/__init__.py` & `inflow_haisslab-1.2.8/Inflow/tiff/__init__.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/tiff/content.py` & `inflow_haisslab-1.2.8/Inflow/tiff/content.py`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/Inflow/tiff/tiff_metadata_parse.dll` & `inflow_haisslab-1.2.8/Inflow/tiff/tiff_metadata_parse.dll`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/LICENSE` & `inflow_haisslab-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/README.md` & `inflow_haisslab-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `inflow_haisslab-1.2.7/pyproject.toml` & `inflow_haisslab-1.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
-version = "1.2.7"
+version = "1.2.8"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://gitlab.pasteur.fr/haisslab/analysis-packages/Inflow"
```

### Comparing `inflow_haisslab-1.2.7/PKG-INFO` & `inflow_haisslab-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inflow-haisslab
-Version: 1.2.7
+Version: 1.2.8
 Summary: General python code for analysis pipeline
 Author-Email: Timothé Jost-MOUSSEAU <timothe.jost-mousseau@pasteur.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

