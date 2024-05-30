# Comparing `tmp/lsst_ctrl_bps_htcondor-27.2024.2100.tar.gz` & `tmp/lsst_ctrl_bps_htcondor-27.2024.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_ctrl_bps_htcondor-27.2024.2100.tar", last modified: Thu May 23 10:08:42 2024, max compression
+gzip compressed data, was "lsst_ctrl_bps_htcondor-27.2024.2200.tar", last modified: Thu May 30 09:56:24 2024, max compression
```

## Comparing `lsst_ctrl_bps_htcondor-27.2024.2100.tar` & `lsst_ctrl_bps_htcondor-27.2024.2200.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.122639 lsst_ctrl_bps_htcondor-27.2024.2100/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 10:08:42.122639 lsst_ctrl_bps_htcondor-27.2024.2100/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.114638 lsst_ctrl_bps_htcondor-27.2024.2100/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.118638 lsst_ctrl_bps_htcondor-27.2024.2100/doc/lsst.ctrl.bps.htcondor/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/doc/lsst.ctrl.bps.htcondor/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/doc/lsst.ctrl.bps.htcondor/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/doc/lsst.ctrl.bps.htcondor/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.114638 lsst_ctrl_bps_htcondor-27.2024.2100/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.114638 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.114638 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.114638 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.118638 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    74669 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/htcondor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    54062 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/lssthtc.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 10:08:41.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.122639 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-23 10:08:42.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-23 10:08:42.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:08:42.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 10:08:42.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:08:42.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:08:41.000000 lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-23 10:08:42.122639 lsst_ctrl_bps_htcondor-27.2024.2100/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:08:42.122639 lsst_ctrl_bps_htcondor-27.2024.2100/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/tests/test_htcondor_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-23 10:08:36.000000 lsst_ctrl_bps_htcondor-27.2024.2100/tests/test_lssthtc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.258935 lsst_ctrl_bps_htcondor-27.2024.2200/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 09:56:24.258935 lsst_ctrl_bps_htcondor-27.2024.2200/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.250935 lsst_ctrl_bps_htcondor-27.2024.2200/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.254935 lsst_ctrl_bps_htcondor-27.2024.2200/doc/lsst.ctrl.bps.htcondor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/doc/lsst.ctrl.bps.htcondor/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/doc/lsst.ctrl.bps.htcondor/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/doc/lsst.ctrl.bps.htcondor/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.250935 lsst_ctrl_bps_htcondor-27.2024.2200/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.250935 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.250935 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.250935 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.254935 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74669 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/htcondor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54062 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/lssthtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 09:56:24.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.254935 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 09:56:24.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 09:56:24.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:24.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 09:56:24.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 09:56:24.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 09:56:23.000000 lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 09:56:24.258935 lsst_ctrl_bps_htcondor-27.2024.2200/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 09:56:24.254935 lsst_ctrl_bps_htcondor-27.2024.2200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/tests/test_htcondor_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-30 09:56:18.000000 lsst_ctrl_bps_htcondor-27.2024.2200/tests/test_lssthtc.py
```

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/PKG-INFO` & `lsst_ctrl_bps_htcondor-27.2024.2200/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-htcondor
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: HTCondor plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_htcondor
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/README.rst` & `lsst_ctrl_bps_htcondor-27.2024.2200/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/bsd_license.txt` & `lsst_ctrl_bps_htcondor-27.2024.2200/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/doc/lsst.ctrl.bps.htcondor/CHANGES.rst` & `lsst_ctrl_bps_htcondor-27.2024.2200/doc/lsst.ctrl.bps.htcondor/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/doc/lsst.ctrl.bps.htcondor/index.rst` & `lsst_ctrl_bps_htcondor-27.2024.2200/doc/lsst.ctrl.bps.htcondor/index.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/doc/lsst.ctrl.bps.htcondor/userguide.rst` & `lsst_ctrl_bps_htcondor-27.2024.2200/doc/lsst.ctrl.bps.htcondor/userguide.rst`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/gpl-v3.0.txt` & `lsst_ctrl_bps_htcondor-27.2024.2200/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/pyproject.toml` & `lsst_ctrl_bps_htcondor-27.2024.2200/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/__init__.py` & `lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/handlers.py` & `lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/handlers.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/htcondor_service.py` & `lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/htcondor_service.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst/ctrl/bps/htcondor/lssthtc.py` & `lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst/ctrl/bps/htcondor/lssthtc.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO` & `lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps-htcondor
-Version: 27.2024.2100
+Version: 27.2024.2200
 Summary: HTCondor plugin for lsst-ctrl-bps.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps_htcondor
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt` & `lsst_ctrl_bps_htcondor-27.2024.2200/python/lsst_ctrl_bps_htcondor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/tests/test_handlers.py` & `lsst_ctrl_bps_htcondor-27.2024.2200/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/tests/test_htcondor_service.py` & `lsst_ctrl_bps_htcondor-27.2024.2200/tests/test_htcondor_service.py`

 * *Files identical despite different names*

### Comparing `lsst_ctrl_bps_htcondor-27.2024.2100/tests/test_lssthtc.py` & `lsst_ctrl_bps_htcondor-27.2024.2200/tests/test_lssthtc.py`

 * *Files identical despite different names*

