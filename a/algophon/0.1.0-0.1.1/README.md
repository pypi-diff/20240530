# Comparing `tmp/algophon-0.1.0.tar.gz` & `tmp/algophon-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algophon-0.1.0.tar", last modified: Fri May 24 00:10:47 2024, max compression
+gzip compressed data, was "algophon-0.1.1.tar", last modified: Thu May 30 17:59:24 2024, max compression
```

## Comparing `algophon-0.1.0.tar` & `algophon-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.826599 algophon-0.1.0/
--rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.1.0/LICENSE
--rw-r--r--   0 u6052607   (503) staff       (20)    10227 2024-05-24 00:10:47.825284 algophon-0.1.0/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)     9596 2024-05-24 00:09:59.000000 algophon-0.1.0/README.md
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.738799 algophon-0.1.0/algophon/
--rw-r--r--   0 u6052607   (503) staff       (20)      245 2024-05-05 22:24:11.000000 algophon-0.1.0/algophon/__init__.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.756923 algophon-0.1.0/algophon/distance/
--rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-05 22:11:24.000000 algophon-0.1.0/algophon/distance/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5222 2024-05-06 15:22:54.000000 algophon-0.1.0/algophon/distance/edit_distance.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.762670 algophon-0.1.0/algophon/ipa/
--rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.1.0/algophon/ipa/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     3081 2024-05-03 14:26:54.000000 algophon-0.1.0/algophon/ipa/convert.py
--rw-r--r--   0 u6052607   (503) staff       (20)   350576 2024-04-25 00:16:18.000000 algophon-0.1.0/algophon/ipa.txt
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.763248 algophon-0.1.0/algophon/models/
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.778672 algophon-0.1.0/algophon/models/D2L/
--rw-r--r--   0 u6052607   (503) staff       (20)      179 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)    13761 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/d2l.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1854 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/discrepancy.py
--rw-r--r--   0 u6052607   (503) staff       (20)    10969 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/rule.py
--rw-r--r--   0 u6052607   (503) staff       (20)     3205 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/D2L/tier.py
--rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/models/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.1.0/algophon/natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1779 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     8023 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     5780 2024-05-06 15:42:02.000000 algophon-0.1.0/algophon/segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      250 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/symbols.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.789201 algophon-0.1.0/algophon/utils/
--rw-r--r--   0 u6052607   (503) staff       (20)       36 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/utils/__init__.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1114 2024-05-24 00:09:59.000000 algophon-0.1.0/algophon/utils/utils.py
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.823174 algophon-0.1.0/algophon.egg-info/
--rw-r--r--   0 u6052607   (503) staff       (20)    10227 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/PKG-INFO
--rw-r--r--   0 u6052607   (503) staff       (20)      827 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/SOURCES.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/dependency_links.txt
--rw-r--r--   0 u6052607   (503) staff       (20)       12 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/requires.txt
--rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-05-24 00:10:47.000000 algophon-0.1.0/algophon.egg-info/top_level.txt
--rw-r--r--   0 u6052607   (503) staff       (20)      829 2024-05-24 00:09:59.000000 algophon-0.1.0/pyproject.toml
--rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-05-24 00:10:47.826659 algophon-0.1.0/setup.cfg
-drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-24 00:10:47.821769 algophon-0.1.0/tests/
--rw-r--r--   0 u6052607   (503) staff       (20)    29575 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_d2l.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1240 2024-05-05 22:45:04.000000 algophon-0.1.0/tests/test_distance.py
--rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.1.0/tests/test_natclass.py
--rw-r--r--   0 u6052607   (503) staff       (20)     2123 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_seg.py
--rw-r--r--   0 u6052607   (503) staff       (20)     4553 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_seginv.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1941 2024-04-24 23:29:27.000000 algophon-0.1.0/tests/test_segstr.py
--rw-r--r--   0 u6052607   (503) staff       (20)      645 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/test_utils.py
--rw-r--r--   0 u6052607   (503) staff       (20)     1132 2024-05-24 00:09:59.000000 algophon-0.1.0/tests/tester.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.792071 algophon-0.1.1/
+-rw-r--r--   0 u6052607   (503) staff       (20)    11357 2024-04-18 14:18:03.000000 algophon-0.1.1/LICENSE
+-rw-r--r--   0 u6052607   (503) staff       (20)    10312 2024-05-30 17:59:24.791440 algophon-0.1.1/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)     9681 2024-05-30 17:59:16.000000 algophon-0.1.1/README.md
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.716988 algophon-0.1.1/algophon/
+-rw-r--r--   0 u6052607   (503) staff       (20)      245 2024-05-05 22:24:11.000000 algophon-0.1.1/algophon/__init__.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.730034 algophon-0.1.1/algophon/data_structures/
+-rw-r--r--   0 u6052607   (503) staff       (20)       96 2024-05-30 17:59:16.000000 algophon-0.1.1/algophon/data_structures/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)    10563 2024-05-30 17:59:16.000000 algophon-0.1.1/algophon/data_structures/graph.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.733415 algophon-0.1.1/algophon/distance/
+-rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-05 22:11:24.000000 algophon-0.1.1/algophon/distance/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5222 2024-05-06 15:22:54.000000 algophon-0.1.1/algophon/distance/edit_distance.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.738699 algophon-0.1.1/algophon/ipa/
+-rw-r--r--   0 u6052607   (503) staff       (20)       32 2024-04-19 13:49:06.000000 algophon-0.1.1/algophon/ipa/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     3081 2024-05-03 14:26:54.000000 algophon-0.1.1/algophon/ipa/convert.py
+-rw-r--r--   0 u6052607   (503) staff       (20)   350576 2024-04-25 00:16:18.000000 algophon-0.1.1/algophon/ipa.txt
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.739298 algophon-0.1.1/algophon/models/
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.753345 algophon-0.1.1/algophon/models/D2L/
+-rw-r--r--   0 u6052607   (503) staff       (20)      179 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/models/D2L/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)    13761 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/models/D2L/d2l.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1854 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/models/D2L/discrepancy.py
+-rw-r--r--   0 u6052607   (503) staff       (20)    10969 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/models/D2L/rule.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     3205 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/models/D2L/tier.py
+-rw-r--r--   0 u6052607   (503) staff       (20)        0 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/models/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1006 2024-04-19 00:08:37.000000 algophon-0.1.1/algophon/natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1779 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     8023 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     5780 2024-05-06 15:42:02.000000 algophon-0.1.1/algophon/segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      250 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/symbols.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.761933 algophon-0.1.1/algophon/utils/
+-rw-r--r--   0 u6052607   (503) staff       (20)       36 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/utils/__init__.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1114 2024-05-24 00:09:59.000000 algophon-0.1.1/algophon/utils/utils.py
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.790757 algophon-0.1.1/algophon.egg-info/
+-rw-r--r--   0 u6052607   (503) staff       (20)    10312 2024-05-30 17:59:24.000000 algophon-0.1.1/algophon.egg-info/PKG-INFO
+-rw-r--r--   0 u6052607   (503) staff       (20)      928 2024-05-30 17:59:24.000000 algophon-0.1.1/algophon.egg-info/SOURCES.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        1 2024-05-30 17:59:24.000000 algophon-0.1.1/algophon.egg-info/dependency_links.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)       12 2024-05-30 17:59:24.000000 algophon-0.1.1/algophon.egg-info/requires.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)        9 2024-05-30 17:59:24.000000 algophon-0.1.1/algophon.egg-info/top_level.txt
+-rw-r--r--   0 u6052607   (503) staff       (20)      829 2024-05-30 17:59:16.000000 algophon-0.1.1/pyproject.toml
+-rw-r--r--   0 u6052607   (503) staff       (20)       38 2024-05-30 17:59:24.792128 algophon-0.1.1/setup.cfg
+drwxr-xr-x   0 u6052607   (503) staff       (20)        0 2024-05-30 17:59:24.790094 algophon-0.1.1/tests/
+-rw-r--r--   0 u6052607   (503) staff       (20)    29575 2024-05-24 00:09:59.000000 algophon-0.1.1/tests/test_d2l.py
+-rw-r--r--   0 u6052607   (503) staff       (20)    11000 2024-05-30 17:59:16.000000 algophon-0.1.1/tests/test_data_structures.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1240 2024-05-05 22:45:04.000000 algophon-0.1.1/tests/test_distance.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      860 2024-04-19 00:19:07.000000 algophon-0.1.1/tests/test_natclass.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     2123 2024-05-24 00:09:59.000000 algophon-0.1.1/tests/test_seg.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     4553 2024-05-24 00:09:59.000000 algophon-0.1.1/tests/test_seginv.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1941 2024-04-24 23:29:27.000000 algophon-0.1.1/tests/test_segstr.py
+-rw-r--r--   0 u6052607   (503) staff       (20)      645 2024-05-24 00:09:59.000000 algophon-0.1.1/tests/test_utils.py
+-rw-r--r--   0 u6052607   (503) staff       (20)     1307 2024-05-30 17:59:16.000000 algophon-0.1.1/tests/tester.py
```

### Comparing `algophon-0.1.0/LICENSE` & `algophon-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/PKG-INFO` & `algophon-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -263,22 +263,26 @@
 ### Symbols: The `symbols` module
 
 The `symbols` module (technically just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
-SYL_BOUNDARY = '.'
+SYLB = '.'
+MORPHB = '-'
+BOUNDARIES = [LWB, RWB, SYLB, MORPHB]
 PRIMARY_STRESS = 'ˈ'
 SEC_STRESS = 'ˌ'
 LONG = 'ː'
-NASALIZED = '\u0303' # ◌̃
+NASALIZED = '\u0303'  # ◌̃
 UNDERSPECIFIED = '0'
 UNK = '?'
 NEG = '¬'
+EMPTY = '_'
+FUNCTION_COMPOSITION = '∘'
 ```
 
 These can be accessed like this:
 
 ```pycon
 >>> from algophon.symbols import *
 >>> NASALIZED
```

### Comparing `algophon-0.1.0/README.md` & `algophon-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -247,22 +247,26 @@
 ### Symbols: The `symbols` module
 
 The `symbols` module (technically just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
-SYL_BOUNDARY = '.'
+SYLB = '.'
+MORPHB = '-'
+BOUNDARIES = [LWB, RWB, SYLB, MORPHB]
 PRIMARY_STRESS = 'ˈ'
 SEC_STRESS = 'ˌ'
 LONG = 'ː'
-NASALIZED = '\u0303' # ◌̃
+NASALIZED = '\u0303'  # ◌̃
 UNDERSPECIFIED = '0'
 UNK = '?'
 NEG = '¬'
+EMPTY = '_'
+FUNCTION_COMPOSITION = '∘'
 ```
 
 These can be accessed like this:
 
 ```pycon
 >>> from algophon.symbols import *
 >>> NASALIZED
```

### Comparing `algophon-0.1.0/algophon/distance/edit_distance.py` & `algophon-0.1.1/algophon/distance/edit_distance.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/ipa/convert.py` & `algophon-0.1.1/algophon/ipa/convert.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/ipa.txt` & `algophon-0.1.1/algophon/ipa.txt`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/models/D2L/d2l.py` & `algophon-0.1.1/algophon/models/D2L/d2l.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/models/D2L/discrepancy.py` & `algophon-0.1.1/algophon/models/D2L/discrepancy.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/models/D2L/rule.py` & `algophon-0.1.1/algophon/models/D2L/rule.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/models/D2L/tier.py` & `algophon-0.1.1/algophon/models/D2L/tier.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/natclass.py` & `algophon-0.1.1/algophon/natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/seg.py` & `algophon-0.1.1/algophon/seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/seginv.py` & `algophon-0.1.1/algophon/seginv.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/segstr.py` & `algophon-0.1.1/algophon/segstr.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon/utils/utils.py` & `algophon-0.1.1/algophon/utils/utils.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/algophon.egg-info/PKG-INFO` & `algophon-0.1.1/algophon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algophon
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)
 Author: Caleb Belth
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/cbelth/algophon
 Keywords: computational linguistics,phonology,morphology,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -263,22 +263,26 @@
 ### Symbols: The `symbols` module
 
 The `symbols` module (technically just a file...) contains a number of constant variables that store some useful symbols:
 
 ```python
 LWB = '⋊'
 RWB = '⋉'
-SYL_BOUNDARY = '.'
+SYLB = '.'
+MORPHB = '-'
+BOUNDARIES = [LWB, RWB, SYLB, MORPHB]
 PRIMARY_STRESS = 'ˈ'
 SEC_STRESS = 'ˌ'
 LONG = 'ː'
-NASALIZED = '\u0303' # ◌̃
+NASALIZED = '\u0303'  # ◌̃
 UNDERSPECIFIED = '0'
 UNK = '?'
 NEG = '¬'
+EMPTY = '_'
+FUNCTION_COMPOSITION = '∘'
 ```
 
 These can be accessed like this:
 
 ```pycon
 >>> from algophon.symbols import *
 >>> NASALIZED
```

### Comparing `algophon-0.1.0/algophon.egg-info/SOURCES.txt` & `algophon-0.1.1/algophon.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 algophon/segstr.py
 algophon/symbols.py
 algophon.egg-info/PKG-INFO
 algophon.egg-info/SOURCES.txt
 algophon.egg-info/dependency_links.txt
 algophon.egg-info/requires.txt
 algophon.egg-info/top_level.txt
+algophon/data_structures/__init__.py
+algophon/data_structures/graph.py
 algophon/distance/__init__.py
 algophon/distance/edit_distance.py
 algophon/ipa/__init__.py
 algophon/ipa/convert.py
 algophon/models/__init__.py
 algophon/models/D2L/__init__.py
 algophon/models/D2L/d2l.py
 algophon/models/D2L/discrepancy.py
 algophon/models/D2L/rule.py
 algophon/models/D2L/tier.py
 algophon/utils/__init__.py
 algophon/utils/utils.py
 tests/test_d2l.py
+tests/test_data_structures.py
 tests/test_distance.py
 tests/test_natclass.py
 tests/test_seg.py
 tests/test_seginv.py
 tests/test_segstr.py
 tests/test_utils.py
 tests/tester.py
```

### Comparing `algophon-0.1.0/pyproject.toml` & `algophon-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "algophon"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Caleb Belth" },
 ]
 description = "Tools for an algorithmic approach to phonology (some useful to computational phonology and morphology more broadly)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "Apache 2.0" }
```

### Comparing `algophon-0.1.0/tests/test_d2l.py` & `algophon-0.1.1/tests/test_d2l.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/tests/test_distance.py` & `algophon-0.1.1/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/tests/test_natclass.py` & `algophon-0.1.1/tests/test_natclass.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/tests/test_seg.py` & `algophon-0.1.1/tests/test_seg.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/tests/test_seginv.py` & `algophon-0.1.1/tests/test_seginv.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/tests/test_segstr.py` & `algophon-0.1.1/tests/test_segstr.py`

 * *Files identical despite different names*

### Comparing `algophon-0.1.0/tests/test_utils.py` & `algophon-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

