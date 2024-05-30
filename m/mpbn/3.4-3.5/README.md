# Comparing `tmp/mpbn-3.4.tar.gz` & `tmp/mpbn-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpbn-3.4.tar", last modified: Thu Mar 28 14:33:29 2024, max compression
+gzip compressed data, was "mpbn-3.5.tar", last modified: Thu May 30 11:32:07 2024, max compression
```

## Comparing `mpbn-3.4.tar` & `mpbn-3.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:29.163205 mpbn-3.4/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 14:33:19.000000 mpbn-3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-28 14:33:29.163205 mpbn-3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-28 14:33:19.000000 mpbn-3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:29.159206 mpbn-3.4/mpbn/
--rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:29.163205 mpbn-3.4/mpbn/asplib/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/asplib/eval_circuit.asp
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/asplib/eval_mixed.asp
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/asplib/mp_attractor.asp
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/asplib/mp_eval.asp
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/asplib/mp_positivereach-np.asp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:29.163205 mpbn-3.4/mpbn/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/cli/sim.py
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-03-28 14:33:19.000000 mpbn-3.4/mpbn/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:33:29.163205 mpbn-3.4/mpbn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-28 14:33:29.000000 mpbn-3.4/mpbn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-28 14:33:29.000000 mpbn-3.4/mpbn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:33:29.000000 mpbn-3.4/mpbn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 14:33:29.000000 mpbn-3.4/mpbn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 14:33:29.000000 mpbn-3.4/mpbn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 14:33:29.000000 mpbn-3.4/mpbn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:33:29.163205 mpbn-3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1128 2024-03-28 14:33:19.000000 mpbn-3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:32:07.931680 mpbn-3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 11:31:58.000000 mpbn-3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 11:32:07.931680 mpbn-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-30 11:31:58.000000 mpbn-3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:32:07.931680 mpbn-3.5/mpbn/
+-rw-r--r--   0 runner    (1001) docker     (127)    20578 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:32:07.931680 mpbn-3.5/mpbn/asplib/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/asplib/eval_circuit.asp
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/asplib/eval_mixed.asp
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/asplib/mp_attractor.asp
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/asplib/mp_eval.asp
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/asplib/mp_positivereach-np.asp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:32:07.931680 mpbn-3.5/mpbn/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/cli/sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-05-30 11:31:58.000000 mpbn-3.5/mpbn/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 11:32:07.931680 mpbn-3.5/mpbn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-30 11:32:07.000000 mpbn-3.5/mpbn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 11:32:07.000000 mpbn-3.5/mpbn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 11:32:07.000000 mpbn-3.5/mpbn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 11:32:07.000000 mpbn-3.5/mpbn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 11:32:07.000000 mpbn-3.5/mpbn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-30 11:32:07.000000 mpbn-3.5/mpbn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 11:32:07.935680 mpbn-3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1128 2024-05-30 11:31:58.000000 mpbn-3.5/setup.py
```

### Comparing `mpbn-3.4/PKG-INFO` & `mpbn-3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 3.4
+Version: 3.5
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-3.4/README.md` & `mpbn-3.5/README.md`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn/__init__.py` & `mpbn-3.5/mpbn/__init__.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn/asplib/eval_circuit.asp` & `mpbn-3.5/mpbn/asplib/eval_circuit.asp`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn/asplib/eval_mixed.asp` & `mpbn-3.5/mpbn/asplib/eval_mixed.asp`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn/asplib/mp_eval.asp` & `mpbn-3.5/mpbn/asplib/mp_eval.asp`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn/cli/__init__.py` & `mpbn-3.5/mpbn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn/cli/sim.py` & `mpbn-3.5/mpbn/cli/sim.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn/simulation.py` & `mpbn-3.5/mpbn/simulation.py`

 * *Files identical despite different names*

### Comparing `mpbn-3.4/mpbn.egg-info/PKG-INFO` & `mpbn-3.5/mpbn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpbn
-Version: 3.4
+Version: 3.5
 Summary: Simple implementation of Most Permissive Boolean networks
 Home-page: https://github.com/bnediction/mpbn
 Author: Loïc Paulevé
 Author-email: loic.pauleve@labri.fr
 License: CeCILL
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `mpbn-3.4/setup.py` & `mpbn-3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8
 
 from setuptools import setup, find_packages
 
 NAME = "mpbn"
-VERSION = "3.4"
+VERSION = "3.5"
 
 setup(name=NAME,
     version=VERSION,
     author="Loïc Paulevé",
     author_email="loic.pauleve@labri.fr",
     url="https://github.com/bnediction/mpbn",
     license="CeCILL",
```

