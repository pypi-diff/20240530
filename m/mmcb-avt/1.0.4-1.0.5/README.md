# Comparing `tmp/mmcb_avt-1.0.4.tar.gz` & `tmp/mmcb_avt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb_avt-1.0.4.tar", last modified: Tue May 28 14:56:12 2024, max compression
+gzip compressed data, was "mmcb_avt-1.0.5.tar", last modified: Thu May 30 13:48:35 2024, max compression
```

## Comparing `mmcb_avt-1.0.4.tar` & `mmcb_avt-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-28 14:56:12.385340 mmcb_avt-1.0.4/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb_avt-1.0.4/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9803 2024-05-28 14:56:12.384145 mmcb_avt-1.0.4/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     8120 2024-03-22 09:07:14.000000 mmcb_avt-1.0.4/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb_avt-1.0.4/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2024-05-28 14:56:12.385595 mmcb_avt-1.0.4/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2707 2024-05-28 14:55:47.000000 mmcb_avt-1.0.4/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-28 14:56:12.352292 mmcb_avt-1.0.4/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-28 14:56:12.372970 mmcb_avt-1.0.4/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb_avt-1.0.4/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    99113 2024-05-28 14:52:29.000000 mmcb_avt-1.0.4/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    34011 2023-09-27 11:50:51.000000 mmcb_avt-1.0.4/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14458 2023-10-03 14:26:21.000000 mmcb_avt-1.0.4/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8822 2023-10-03 14:12:48.000000 mmcb_avt-1.0.4/src/mmcb/dat2plotsep.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb_avt-1.0.4/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33955 2023-10-06 08:18:38.000000 mmcb_avt-1.0.4/src/mmcb/detect.py
--rwxr-xr-x   0 avt        (501) staff       (20)     3499 2023-10-18 11:29:23.000000 mmcb_avt-1.0.4/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4688 2023-10-18 09:27:36.000000 mmcb_avt-1.0.4/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   114635 2023-11-15 22:36:35.000000 mmcb_avt-1.0.4/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24903 2023-09-17 12:51:37.000000 mmcb_avt-1.0.4/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb_avt-1.0.4/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb_avt-1.0.4/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb_avt-1.0.4/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    36055 2024-05-28 14:55:20.000000 mmcb_avt-1.0.4/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    26656 2023-10-27 08:25:32.000000 mmcb_avt-1.0.4/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21588 2024-05-17 20:07:46.000000 mmcb_avt-1.0.4/src/mmcb/psuwatch.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14133 2023-09-11 13:56:44.000000 mmcb_avt-1.0.4/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    41754 2023-09-24 14:48:52.000000 mmcb_avt-1.0.4/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-08-26 19:37:46.000000 mmcb_avt-1.0.4/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb_avt-1.0.4/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-28 14:56:12.382592 mmcb_avt-1.0.4/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9803 2024-05-28 14:56:12.000000 mmcb_avt-1.0.4/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      715 2024-05-28 14:56:12.000000 mmcb_avt-1.0.4/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2024-05-28 14:56:12.000000 mmcb_avt-1.0.4/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      396 2024-05-28 14:56:12.000000 mmcb_avt-1.0.4/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      237 2024-05-28 14:56:12.000000 mmcb_avt-1.0.4/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2024-05-28 14:56:12.000000 mmcb_avt-1.0.4/src/mmcb_avt.egg-info/top_level.txt
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-28 14:56:12.381287 mmcb_avt-1.0.4/tests/
--rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb_avt-1.0.4/tests/test_lexicon.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-30 13:48:35.205407 mmcb_avt-1.0.5/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb_avt-1.0.5/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9803 2024-05-30 13:48:35.203671 mmcb_avt-1.0.5/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     8120 2024-03-22 09:07:14.000000 mmcb_avt-1.0.5/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb_avt-1.0.5/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2024-05-30 13:48:35.205643 mmcb_avt-1.0.5/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2707 2024-05-30 13:48:12.000000 mmcb_avt-1.0.5/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-30 13:48:35.158256 mmcb_avt-1.0.5/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-30 13:48:35.193502 mmcb_avt-1.0.5/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb_avt-1.0.5/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    99200 2024-05-30 13:43:38.000000 mmcb_avt-1.0.5/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    34011 2023-09-27 11:50:51.000000 mmcb_avt-1.0.5/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14458 2023-10-03 14:26:21.000000 mmcb_avt-1.0.5/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8822 2023-10-03 14:12:48.000000 mmcb_avt-1.0.5/src/mmcb/dat2plotsep.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb_avt-1.0.5/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33955 2023-10-06 08:18:38.000000 mmcb_avt-1.0.5/src/mmcb/detect.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     3499 2023-10-18 11:29:23.000000 mmcb_avt-1.0.5/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4688 2023-10-18 09:27:36.000000 mmcb_avt-1.0.5/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   114635 2023-11-15 22:36:35.000000 mmcb_avt-1.0.5/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24903 2023-09-17 12:51:37.000000 mmcb_avt-1.0.5/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb_avt-1.0.5/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb_avt-1.0.5/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb_avt-1.0.5/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    36297 2024-05-30 13:46:55.000000 mmcb_avt-1.0.5/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    26656 2023-10-27 08:25:32.000000 mmcb_avt-1.0.5/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21588 2024-05-17 20:07:46.000000 mmcb_avt-1.0.5/src/mmcb/psuwatch.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14133 2023-09-11 13:56:44.000000 mmcb_avt-1.0.5/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    41754 2023-09-24 14:48:52.000000 mmcb_avt-1.0.5/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-08-26 19:37:46.000000 mmcb_avt-1.0.5/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb_avt-1.0.5/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-30 13:48:35.202191 mmcb_avt-1.0.5/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9803 2024-05-30 13:48:35.000000 mmcb_avt-1.0.5/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      715 2024-05-30 13:48:35.000000 mmcb_avt-1.0.5/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2024-05-30 13:48:35.000000 mmcb_avt-1.0.5/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      396 2024-05-30 13:48:35.000000 mmcb_avt-1.0.5/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      237 2024-05-30 13:48:35.000000 mmcb_avt-1.0.5/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2024-05-30 13:48:35.000000 mmcb_avt-1.0.5/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-05-30 13:48:35.200965 mmcb_avt-1.0.5/tests/
+-rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb_avt-1.0.5/tests/test_lexicon.py
```

### Comparing `mmcb_avt-1.0.4/LICENSE` & `mmcb_avt-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/PKG-INFO` & `mmcb_avt-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 1.0.4
+Version: 1.0.5
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb_avt-1.0.4/README.md` & `mmcb_avt-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/setup.py` & `mmcb_avt-1.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="1.0.4",
+    version="1.0.5",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb_avt-1.0.4/src/mmcb/common.py` & `mmcb_avt-1.0.5/src/mmcb/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -2549,15 +2549,15 @@
         log_with_colour(logging.WARNING, message)
 
 
 ##############################################################################
 # logging
 ##############################################################################
 
-def log_with_colour(level, message):
+def log_with_colour(level, message, quiet=False):
     """
     Write messages to the log file. This can be safely called from threads,
     but NOT from processes.
 
     "Thread Safety
 
     The logging module is intended to be thread-safe without any special work
@@ -2570,18 +2570,23 @@
 
     --------------------------------------------------------------------------
     args
         level : int
             logging level e.g. logging.DEBUG
         message : string
             message to be sent to the log file
+        quiet : bool
+            do not log
     --------------------------------------------------------------------------
     returns : none
     --------------------------------------------------------------------------
     """
+    if quiet:
+        return
+
     if level == logging.WARNING:
         message = (f'{ANSIColours.FG_BLACK}{ANSIColours.BG_YELLOW}'
                    f'{ANSIColours.BOLD}{message}{ANSIColours.ENDC}')
     elif level in {logging.ERROR, logging.CRITICAL}:
         message = (f'{ANSIColours.FG_WHITE}{ANSIColours.BG_RED}'
                    f'{ANSIColours.BOLD}{message}{ANSIColours.ENDC}')
```

### Comparing `mmcb_avt-1.0.4/src/mmcb/configure_environment.py` & `mmcb_avt-1.0.5/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/dat2plot.py` & `mmcb_avt-1.0.5/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/dat2plotsep.py` & `mmcb_avt-1.0.5/src/mmcb/dat2plotsep.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/dat2root.py` & `mmcb_avt-1.0.5/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/detect.py` & `mmcb_avt-1.0.5/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/dmm.py` & `mmcb_avt-1.0.5/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/dmm_interface.py` & `mmcb_avt-1.0.5/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/iv.py` & `mmcb_avt-1.0.5/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/lexicon.py` & `mmcb_avt-1.0.5/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/liveplot.py` & `mmcb_avt-1.0.5/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/log2dat.py` & `mmcb_avt-1.0.5/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/peltier.py` & `mmcb_avt-1.0.5/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/psuset.py` & `mmcb_avt-1.0.5/src/mmcb/psuset.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import argparse
 import logging
 import math
 import sys
 import threading
 import time
+import types
 
 import serial
 import numpy as np
 
 from mmcb import common
 from mmcb import lexicon
 from mmcb import sequence
@@ -44,14 +45,15 @@
     val = float(val)
     if not -1100 <= val <= 1100:
         raise argparse.ArgumentTypeError(
             f'{val}: '
             'voltage value should be between -1100 and 1100')
     return val
 
+
 def check_settlingtime(val):
     """
     check settling time
 
     --------------------------------------------------------------------------
     args
         val : float
@@ -63,14 +65,15 @@
     val = float(val)
     if not 0.0 <= val <= 60.0:
         raise argparse.ArgumentTypeError(
             f'{val}: '
             'settling time value should be between 0 and 60 seconds')
     return val
 
+
 def check_arguments(settings):
     """
     handle command line options
 
     --------------------------------------------------------------------------
     args
         settings : dictionary
@@ -94,19 +97,14 @@
         final values, and at low voltages they may never converge to the set\
         voltage.')
     parser.add_argument(
         'voltage', nargs='*', metavar='voltage',
         help='value in volts, values range -1100 to +1100',
         type=check_voltage, default=None)
     parser.add_argument(
-        '--verbose',
-        action='store_true',
-        help='Display all power supply channels detected, and search terms\
-        supplied')
-    parser.add_argument(
         '--manufacturer', nargs=1, metavar='manufacturer',
         choices=['agilent', 'hameg', 'iseg', 'keithley'],
         help='PSU manufacturer.',
         default=None)
     parser.add_argument(
         '--model', nargs=1, metavar='model',
         choices=['2410', '2614b', 'e3634a', 'e3647a', 'hmp4040', 'shq'],
@@ -181,17 +179,29 @@
             power supply output unchanged (Keithley and Agilent).')
     group2.add_argument(
         '--off',
         action='store_true',
         help='Turn PSU output off, by default the script leaves the power\
             supply output unchanged (Keithley and Agilent).')
 
+    group3 = parser.add_mutually_exclusive_group()
+    group3.add_argument(
+        '--verbose',
+        action='store_true',
+        help='Display all power supply channels detected, and search terms\
+        supplied')
+    group3.add_argument(
+        '-q', '--quiet',
+        action='store_true',
+        help='Minimal text output during normal operation')
+
     args = parser.parse_args()
 
     settings['verbose'] = args.verbose
+    settings['quiet'] = args.quiet
 
     # default: leave power supply settings unchanged
     if args.front:
         settings['rear'] = False
     elif args.rear:
         settings['rear'] = True
 
@@ -486,56 +496,59 @@
     if settings['on'] is not None:
         comtxt = 'output on' if settings['on'] else 'output off'
         command_string = lexicon.power(dev.model, comtxt, channel=dev.channel)
         common.atomic_send_command_read_response(pipeline, ser, dev, command_string)
         common.log_with_colour(logging.INFO, comtxt)
 
     # set voltage
-    if settings['voltage'] is not None:
-        # constrain the voltage to be set to the given number of decimal places
-        voltage = common.decimal_quantize(settings['voltage'], settings['decimal_places'])
-
-        if voltage < 0:
-            message = f'{dev.manufacturer} {dev.model}: cannot use a negative voltage'
-            common.log_with_colour(logging.ERROR, message)
-        else:
-            message = f'voltage set to {common.si_prefix(voltage)}V'
-            common.log_with_colour(logging.INFO, message)
+    if settings['voltage'] is None:
+        # success is not modified before this point
+        return True
+
+    # constrain the voltage to be set to the given number of decimal places
+    voltage = common.decimal_quantize(settings['voltage'], settings['decimal_places'])
+
+    if voltage < 0:
+        message = f'{dev.manufacturer} {dev.model}: cannot use a negative voltage'
+        common.log_with_colour(logging.ERROR, message)
+    else:
+        message = f'voltage set to {common.si_prefix(voltage)}V'
+        common.log_with_colour(logging.INFO, message)
 
-        if dev.manufacturer == 'hameg' and settings['peltier']:
-            measured_voltage = read_measured_voltage(settings, pipeline, ser, dev)
-            if measured_voltage is not None:
-                transition_voltage(settings, pipeline, measured_voltage, voltage, ser, dev)
-        else:
-            common.set_psu_voltage(settings, pipeline, voltage, ser, dev)
+    if dev.manufacturer == 'hameg' and settings['peltier']:
+        measured_voltage = read_measured_voltage(settings, pipeline, ser, dev)
+        if measured_voltage is not None:
+            transition_voltage(settings, pipeline, measured_voltage, voltage, ser, dev)
+    else:
+        common.set_psu_voltage(settings, pipeline, voltage, ser, dev)
 
-        # Agilent E3647A seems to require a minimum of half a second to apply
-        # the setting before any further RS232 interaction is reliable
-        time.sleep(0.5)
-
-        # Arguably the voltage set for the channel should be read back too, so
-        # for the case where the channel output is off, some confirmation that
-        # the value has been set correctly can be given to the user.
-        #
-        # check measured voltage (can only be read back if output is on)
-        if not common.report_output_status(ser, pipeline, dev):
-            # allow a little time for the voltage to settle before reading
-            time.sleep(settings['settlingtime'])
-
-            if dev.manufacturer == 'hameg' and hmp4040_constant_current(ser, pipeline, dev):
-                # When configured as a constant current source, the measured
-                # voltage will not match the set voltage
-                success = True
-            else:
-                success = check_measured_voltage(settings, pipeline, ser, dev, voltage)
-        else:
-            message = 'with PSU output switched off, set voltage cannot be read back'
-            common.log_with_colour(logging.WARNING, message)
-            common.log_with_colour(logging.WARNING, 'assuming all is well')
+    # Agilent E3647A seems to require a minimum of half a second to apply
+    # the setting before any further RS232 interaction is reliable
+    time.sleep(0.5)
+
+    # Arguably the voltage set for the channel should be read back too, so
+    # for the case where the channel output is off, some confirmation that
+    # the value has been set correctly can be given to the user.
+    #
+    # check measured voltage (can only be read back if output is on)
+    if not common.report_output_status(ser, pipeline, dev):
+        # allow a little time for the voltage to settle before reading
+        time.sleep(settings['settlingtime'])
+
+        if dev.manufacturer == 'hameg' and hmp4040_constant_current(ser, pipeline, dev):
+            # When configured as a constant current source, the measured
+            # voltage will not match the set voltage
             success = True
+        else:
+            success = check_measured_voltage(settings, pipeline, ser, dev, voltage)
+    else:
+        message = 'with PSU output switched off, set voltage cannot be read back'
+        common.log_with_colour(logging.WARNING, message)
+        common.log_with_colour(logging.WARNING, 'assuming all is well')
+        success = True
 
     return success
 
 
 def configure_hvpsu(settings, pipeline, ser, dev):
     """
     Amend power supply settings. If a change of voltage has been requested,
@@ -631,39 +644,42 @@
             common.atomic_send_command_read_response(pipeline, ser, dev, command_string)
         else:
             message = f'{dev.manufacturer} {dev.model}: output on/off not supported'
             common.log_with_colour(logging.WARNING, message)
 
     ##############################################################################
     # set voltage
-    if settings['voltage'] is not None:
-        # constrain the voltage to be set to the given number of decimal places
-        voltage = common.decimal_quantize(settings['voltage'], settings['decimal_places'])
-        message = f'setting voltage: {common.si_prefix(voltage)}V'
-        common.log_with_colour(logging.INFO, message)
+    if settings['voltage'] is None:
+        # success is not modified before this point
+        return True
+
+    # constrain the voltage to be set to the given number of decimal places
+    voltage = common.decimal_quantize(settings['voltage'], settings['decimal_places'])
+    message = f'setting voltage: {common.si_prefix(voltage)}V'
+    common.log_with_colour(logging.INFO, message)
 
-        # set voltage
-        if settings['immediate']:
-            common.set_psu_voltage(settings, pipeline, voltage, ser, dev)
-        else:
-            measured_voltage = read_measured_voltage(settings, pipeline, ser, dev)
-            if measured_voltage is not None:
-                transition_voltage(settings, pipeline, measured_voltage, voltage, ser, dev)
-
-        # check set voltage (can only be read back if output is on)
-        if not common.report_output_status(ser, pipeline, dev):
-            # allow a little time for the voltage to settle before reading
-            time.sleep(settings['settlingtime'])
-            success = check_measured_voltage(settings, pipeline, ser, dev, voltage)
-        else:
-            # keithley 2410, 2614b
-            message = 'with PSU output switched off, set voltage cannot be read back'
-            common.log_with_colour(logging.WARNING, message)
-            common.log_with_colour(logging.WARNING, 'assuming all is well')
-            success = True
+    # set voltage
+    if settings['immediate']:
+        common.set_psu_voltage(settings, pipeline, voltage, ser, dev)
+    else:
+        measured_voltage = read_measured_voltage(settings, pipeline, ser, dev)
+        if measured_voltage is not None:
+            transition_voltage(settings, pipeline, measured_voltage, voltage, ser, dev)
+
+    # check set voltage (can only be read back if output is on)
+    if not common.report_output_status(ser, pipeline, dev):
+        # allow a little time for the voltage to settle before reading
+        time.sleep(settings['settlingtime'])
+        success = check_measured_voltage(settings, pipeline, ser, dev, voltage)
+    else:
+        # keithley 2410, 2614b
+        message = 'with PSU output switched off, set voltage cannot be read back'
+        common.log_with_colour(logging.WARNING, message)
+        common.log_with_colour(logging.WARNING, 'assuming all is well')
+        success = True
 
     return success
 
 
 def transition_voltage(settings, pipeline, initial_voltage, target_voltage, ser, dev):
     """
     Gradual voltage transitions.
@@ -759,27 +775,31 @@
 
 ##############################################################################
 # main
 ##############################################################################
 
 def main():
     """ set the voltage on a power supply connected by RS232 """
+
+    status = types.SimpleNamespace(success=0, unreserved_error_code=3)
+
     success = False
     settings = {
         'alias': None,
         'channel': None,
         'current_limit': None,
         'debug': None,
         'decimal_places': 3,
         'immediate': False,
         'manufacturer': None,
         'model': None,
         'on': None,
         'peltier': False,
         'port': None,
+        'quiet': False,
         'rear': None,
         'reset': False,
         'serial': None,
         'settlingtime': 0.5,
         'verbose': None,
         'voltage': None,
         'voltspersecond': 10
@@ -856,32 +876,32 @@
         text = f'selected power supply: {channel.manufacturer} {channel.model}'
         if channel.serial_number:
             text += f' s.no. {channel.serial_number}'
         if channel.channel:
             text += f' channel {channel.channel}'
         if settings['port'] is not None:
             text += f' port {channel.port}'
-        common.log_with_colour(logging.INFO, text)
+        common.log_with_colour(logging.INFO, text, quiet=settings['quiet'])
 
         ##########################################################################
         # set values on given power supply channel
         ##########################################################################
 
         setpsu = {'lvpsu': configure_lvpsu, 'hvpsu': configure_hvpsu}
 
         with serial.Serial(port=channel.port) as ser:
             ser.apply_settings(channel.config)
             ser.reset_input_buffer()
             ser.reset_output_buffer()
             success = setpsu[channel.category](settings, pipeline, ser, channel)
             if success:
-                common.log_with_colour(logging.INFO, 'operation successful')
+                common.log_with_colour(
+                    logging.INFO, 'operation successful',
+                    quiet=settings['quiet']
+                )
 
-    ##########################################################################
-    # 0 command completed successfully
-    # 3 non-reserved error code
-    return 0 if success else 3
+    return status.success if success else status.unreserved_error_code
 
 
 ##############################################################################
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `mmcb_avt-1.0.4/src/mmcb/psustat.py` & `mmcb_avt-1.0.5/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/psuwatch.py` & `mmcb_avt-1.0.5/src/mmcb/psuwatch.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/sense.py` & `mmcb_avt-1.0.5/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/sensors.py` & `mmcb_avt-1.0.5/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/sequence.py` & `mmcb_avt-1.0.5/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb/ult80.py` & `mmcb_avt-1.0.5/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb_avt-1.0.4/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb_avt-1.0.5/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 1.0.4
+Version: 1.0.5
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb_avt-1.0.4/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb_avt-1.0.5/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

